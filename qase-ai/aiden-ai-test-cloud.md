# AIDEN - AI Test Cloud

Before reading this article, please check:

* ### [AIDEN - QA Architect](https://help.qase.io/en/articles/11012497-aiden-qa-architect) <a href="#h_d7215c6345" id="h_d7215c6345"></a>

## Executing the automated tests <a href="#h_81c0d71a1b" id="h_81c0d71a1b"></a>

To run the tests in Qase Cloud, simply select the tests from the repository for an express test run.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1664209723/53ac9806c02e7e7b2b84fe1178e4/92403.png?expires=1758218400&#x26;signature=7f6b85ea6667d5d0187db73fb041b796ef6f944ed5a8870adf974a819c640e05&#x26;req=dSYhEst%2BlIZdWvMW3nq%2BgSVZWwSS%2BLacLOPQtify5uQK54OGcZ%2FCxtlVNYDJ%0A4zwRzAp2SXgF7wpzdHtyaa1F33M%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

In this window, select 'Cloud' and proceed to choose the Environment, and Configuration options.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1729684054/7e5e30dbca5b693800671330e65c/82745.png?expires=1758218400&#x26;signature=ea37b1a9d0ccadf7a5fae75bb809dcd974225b734df1fea9b4ed0598869334a9&#x26;req=dSclH892mYFaXfMW3nq%2BgUKViIfRed4W%2BRkRfiT2XvlYBsJXW0i63lt4mx0f%0ABx4EtAZYEGJaudLDxj5am7fuCz4%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Depending on the browser configuration, multiple test runs will be created and the execution for the selected test cases will be begin the cloud immediately.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1664209726/ea87460e7245d38319030eef6b04/three-2Bruns.png?expires=1758218400&#x26;signature=99cecdf8b5ba0618c8d37812fad6a75a59ed1e0da223c86390aa49e9535cfa23&#x26;req=dSYhEst%2BlIZdX%2FMW3nq%2BgdU3FkGg289XWYDd67D09BBAk66EgpZ172ar7G9U%0AoQ2oi2JNon6PORlAnVpni5gTyZk%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Once the tests are executed, the results will be posted back to the test run automatically.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1664209724/39e859a075a339b1f3139c86ffba/inside-2Btest-2Brun.png?expires=1758218400&#x26;signature=641a0613820841483ff36d559ae0118209e024fad454aeeb93b3216576f7648f&#x26;req=dSYhEst%2BlIZdXfMW3nq%2BgTxePYHy2DRQZ%2B0vsZjmhqpcddEyR2tmSg%2F5R%2FPn%0AcvGLryDllhbJopDMxXmExtFR%2F4Q%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

A screenshot is captured at each test step along with a complete video of the entire execution, are attached to the result. You will also find a `.zip` file attached for the trace.

***

## Integrating with your CI/CD pipeline <a href="#h_78e5f0088c" id="h_78e5f0088c"></a>

AIDEN can run your auto-tests in [Qase cloud](https://help.qase.io/en/articles/11012497-aiden-qa-architect#h_8203030372), eliminating the need for local test execution infrastructure.

The tests run entirely in the background, executing tests in the cloud while your development team continues their work. Once test execution completes, AIDEN populates the test results and detailed stack traces for any failures, into the Qase run.

This integration solves the problem of manual intervention in testing a release.

No development team wants to manually trigger test runs through a UI every time code changes are deployed. This approach breaks the automation flow and can become a significant bottleneck, especially when team members may not even be aware that releases are being pushed through various stages.

Consider the typical software release cycle, where:

* Developers push code changes to GitHub
* CI/CD pipelines automatically build and deploy applications
* Tests need to run alongside these automated processes

The integration offers a simple GitHub Action that bridges your CI/CD pipeline with AIDEN's cloud-based testing capabilities. This approach maintains the automated workflow that modern development teams require.

### Where do I find the code? <a href="#h_a04c622275" id="h_a04c622275"></a>

GitHub respository link for code examples:

[https://github.com/qase-tms/qase-cloud-ci-integrations](https://github.com/qase-tms/qase-cloud-ci-integrations)

### How does it work? <a href="#h_1cf9e93f1d" id="h_1cf9e93f1d"></a>

The integration process follows these key steps:

* Pipeline Trigger: The GitHub Action activates when your pipeline starts, typically after application builds complete.\
  ​
* Test Configuration: You can specify which tests to run, including specific case IDs for targeted testing\
  ​
* Background Execution: AIDEN begins test execution in the Qase's cloud environment\
  ​
* Status Monitoring: The action continuously polls API endpoints to track run progress and results\
  ​
* Results Summary: Upon completion of the run, the workflow will fail, if there are test failures.

### What happens in each step? <a href="#h_4e39441490" id="h_4e39441490"></a>

#### 1. Initialization & Setup <a href="#h_90834b15f5" id="h_90834b15f5"></a>

GitHub Action Trigger: The action is triggered in a GitHub workflow

Docker Container: Runs in an Alpine Linux container with required tools (bash, curl, jq, qasectl)

#### 2. Environment management (optional) <a href="#h_d17d859ad0" id="h_d17d859ad0"></a>

1. If `env_slug` is provided:\
   uses `qasectl` (qase's cli tool) to create or retrieve the specified environment\
   ​
2. If both `env_slug` and `env_title` are provided:\
   uses `qasectl` to create a new environment and uses that.

#### 3. Test Run Creation <a href="#h_c1a794e418" id="h_c1a794e418"></a>

Creates a test run using the provided:

* Run title
* Test case IDs (comma-separated list)
* Browser configuration (chromium, firefox, or webkit)
* Environment slug (if specified)

_Once the cloud run is created from this step, AIDEN kicks in automatically to run them in Qase cloud. The results are automatically published to the same run and it is marked as complete._

#### 4. Test Run Monitoring <a href="#h_14b855b857" id="h_14b855b857"></a>

At this stage, the test run is continuously monitored, and the following polling options are configurable:

* Polling Interval: Default 10 seconds
* Timeout: Default 600 seconds

The run is polled for:

* Total number of results in the run
* The status of the run (`in_progress` / `passed` / `failed`)

It is polled until the status changes to either `passed` or `failed`.

#### 5: Result Evaluation <a href="#h_3acef63f9b" id="h_3acef63f9b"></a>

The step exists with:

* 0: All tests passed ✅
* 1: Tests failed or timeout reached ❌
