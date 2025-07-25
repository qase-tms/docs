# AIDEN - CI/CD Integration

AIDEN can run your auto-tests in [Qase cloud](../aiden/aiden-qa-architect.md#h_8203030372), eliminating the need for local test execution infrastructure.

The tests run entirely in the background, executing tests in the cloud while your development team continues their work. Once test execution completes, AIDEN populates the test results and detailed stack traces for any failures, into the Qase run.

This integration solves the problem of manual intervention in testing a release.

No development team wants to manually trigger test runs through a UI every time code changes are deployed. This approach breaks the automation flow and can become a significant bottleneck, especially when team members may not even be aware that releases are being pushed through various stages.

Consider the typical software release cycle, where:

* Developers push code changes to GitHub
* CI/CD pipelines automatically build and deploy applications
* Tests need to run alongside these automated processes

The integration offers a simple GitHub Action that bridges your CI/CD pipeline with AIDEN's cloud-based testing capabilities. This approach maintains the automated workflow that modern development teams require.

### Where do I find the code?

{% hint style="success" %}
GitHub repository link for **code examples**:\
[https://github.com/qase-tms/qase-cloud-ci-integrations](https://github.com/qase-tms/qase-cloud-ci-integrations)
{% endhint %}

### How does it work? <a href="#h_1cf9e93f1d" id="h_1cf9e93f1d"></a>

The integration process follows these key steps:

* Pipeline Trigger: The GitHub Action activates when your pipeline starts, typically after application builds complete.\
  ​
* Test Configuration: You can specify which tests to run, including specific case IDs for targeted testing\
  ​
* Background Execution: AIDEN begins test execution in the Cases cloud environment\
  ​
* Status Monitoring: The action continuously polls API endpoints to track run progress and results\
  ​
* Results Summary: Upon completion, the action provides comprehensive test results directly in your GitHub workflow

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

Crates a test run using the provided:

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
