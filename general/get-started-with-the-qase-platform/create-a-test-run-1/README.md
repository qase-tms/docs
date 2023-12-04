---
title: Test Run creation & management in Qase
slug: create-a-test-run-1
hidden: true
createdAt: '2023-02-08T03:29:25.607Z'
updatedAt: '2023-02-21T19:47:34.265Z'
---

# Test runs

### What is a test run in software testing?

A Test Run is a single instance of executing a specific set of test cases.

{% embed url="https://www.youtube.com/watch?v=7bLibOsfchs" %}

A Test Run may consist one Test case, a bunch of them, whole sets of Test cases ([Test Suite](https://help.qase.io/en/articles/5563702-test-runs)), or even Test cases from different areas bundled together in a Test Plan.

There are two ways to start a Test Run:\
1\. **Express Run** - from the Project Repository page.\
2\. **Regular Run** - from Test Runs page.



***

### **Express Run**

You can quickly set up a Test Run for one or more test cases directly from the Repository.

​ Hit the "Run" button and proceed to select the Environment, Milestone, Configurations, or any other fields, as needed.

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597420631/c849b9bde959f63612ddddb4/iu7VUj0rrf8F8dW5u6LX6XutC8MN-ru7xOc-Ir31w3Fe2IpPS0-t0nguBngsSYkBnb8QySlSxnygVvh-q-NOWRAB2wZj3WgDtJWdUzlqVVNgLbiywGAKZBVmIMEo1WMpq222MW7NPySWINa7UExwRBS6TsW-QEz8hGuu9ragbRv66kUCjRLMMveguQ" alt=""><figcaption></figcaption></figure>

### **Regular test run**

To create a regular test run, navigate to "Test Runs" section, and hit the "Start New Test Run" button. You will see the same modal window as seen while creating a Test Run from the Repository page.\


<figure><img src="https://qase.intercom-attachments-7.com/i/o/597420795/ea9a99eb365b3fdc5684509a/WUBZGWDp5wDmW5j_cfcUKSQTP55S59lbdn0BO1vcRPD0FWbgxxCgAkLfUaAmqwwkKyJl0lC7BK_uLhW4X8usGcTZNJtB3Zuq11YMV-e7F8iV18EXabJlvb6VNeXojXH77GloD5-D0H12Zr-5SXMN547ZJPsazginDcvCQ9IQ-VGAJdS1A0XCdVJgUw" alt=""><figcaption></figcaption></figure>

#### **Run Properties**

* **Run title:** it is automatically set to the current date. You can replace it with your preferred title.
  * _`Eg: "Regression Test - Release 2.0"`_
* **Description:** give additional details about the test run.
  * _`Eg: "This test run verifies new features and bug fixes in the latest release.`_\
    _`​`_
* [Environment](https://docs.qase.io/general/execution/environments): define in which environment the test run should be performed.
  * _`Eg: testing, staging, production.`_
* [Milestone](https://docs.qase.io/general/issues/milestones): select which Milestone tied to the Test Run.
  * _`Eg: Release 2.0`_
* [Configuration](https://docs.qase.io/general/execution/using-configurations-in-qase-tms): choose from pre-defined configuration options.
  * _`Eg: OS: Windows ; Browser: Chrome`_
* [Custom Fields](https://docs.qase.io/administration/workspace-management/custom-fields): set custom field values if previously configured.

**Choosing Test cases:** Here, you'll be presented with three options.

From Respository.

From Test Plan: You can choose all or select Test cases from a Test Plan.

<details>

<summary>From Saved Queries: You can read more about Saved Queries <a href="https://help.qase.io/en/articles/6417205-saved-queries">here</a>.</summary>

[![](https://downloads.intercomcdn.com/i/o/861868721/89a9e6373dd34a9c59596efb/image.png)](https://downloads.intercomcdn.com/i/o/861868721/89a9e6373dd34a9c59596efb/image.png)

</details>

<mark style="background-color:green;">​NB: Queries are available with</mark> [<mark style="background-color:green;">Business</mark>](https://help.qase.io/en/articles/5563727-business-plan) <mark style="background-color:green;">and</mark> [<mark style="background-color:green;">Enterprise</mark>](https://help.qase.io/en/articles/6640055-enterprise-plan) <mark style="background-color:green;">subscriptions.</mark>

## Test runs view <a href="#h_18ef56a071" id="h_18ef56a071"></a>

***

Here, you can look at all of your Test runs, with their Author, [Environment](https://docs.qase.io/general/execution/environments), Time Spent and Status with a visual summary of their results.

<figure><img src="https://downloads.intercomcdn.com/i/o/825234220/aa01041e1290a0c05f428522/TR+01.jpeg" alt=""><figcaption></figcaption></figure>

<details>

<summary>You can filter the Runs by Status, Assigned to, Environment, Milestone, Tags, Automation status, Creation date, and your <a href="https://docs.qase.io/administration/workspace-management/custom-fields">custom fields</a> (if any).</summary>

<img src="../../../.gitbook/assets/TR 01.jpeg" alt="" data-size="original">

</details>

<details>

<summary>From the "..." menu, you can do several things:</summary>

<img src="../../../.gitbook/assets/Screenshot 2023-12-04 at 3.36.42 PM.png" alt="" data-size="original">

</details>

## Dashboard <a href="#h_e2d602414a" id="h_e2d602414a"></a>

***

To go to the Run dashboard, simply click on the Test Run name.

Let's explore the options available in the dashboard -

<figure><img src="https://downloads.intercomcdn.com/i/o/866886676/766e27b2b417028680b9bb51/rundashnumbered.png" alt=""><figcaption></figcaption></figure>

1**. Open Wizard:** this will guide you through the Test Cases contained in the run, step-by-step.

2\. **Share Report:** turn on public link and easily share your Run report with anyone, even if they don't have an account in Qase.

<details>

<summary>Example of a Shared report</summary>

<img src="../../../.gitbook/assets/Share Report demo.gif" alt="" data-size="original">

</details>

3\. **Export:** you can download a CSV export of your Test Run.

4\. **(---) Menu:** Clone run option allows you to create a new identical copy of your run. You can edit the run details, abort it or go the Test Run settings from here.

5\. **Search and Filters:** search cases by their title or Id and filter by a specific parameter.

6**. Defects and Team stats:** view all associated defects from this run and see stats for results by assignee.

​

7\. T**he "..." menu button:** has options to Run wizard, assign case to a team member or View/edit the Test case itself.

8\. **Run details:** this side bar houses a completion chart and other test run configuration details like -

* Environment, Configurations, Milestones and tags
* Run status, author, create date and estimated time for completion.
* Linked External Issues.

<details>

<summary><em>Expand to learn more</em></summary>



* Donut Graph shows the breakdown of Test Cases in the Run by status. Hovering over a section of the graph you will see the actual number of Cases in a respective Status. If you click on a section of the graph, a quick filter will be applied to show you only the Cases in a specific status.
* Completion Rate represents the percentage of Cases in a run that have been performed so far.
* Status_:_ This lets you know if the run is currently active or completed.
* Started by and Started at - provide details on who started this Test Run, and when.
* Estimation: It predicts how long your current Test Run will take based on the time spent in previous Test Runs on the same Test cases.
* Duration: the summary of time that has been spent on all Test Cases in the current Test Run so far.
* Environment, Tags, Configurations, Milestones, and Custom Fields: Details about the specific environment of the test run and the associated tags, Milestones and Custom fields.
*   External Issue: You can link a test run with an issue/task from any issue tracker Apps that you have installed.

    Here's an example of a JIRA issue linked to a test run:

<img src="../../../.gitbook/assets/GIF.gif" alt="" data-size="original">

</details>

9\. **Bulk action:** You can select multiple test cases and click on 'Update selected' to retest / submit result / manage assignee / remove test case from run.

<details>

<summary>Example</summary>

<img src="../../../.gitbook/assets/Screenshot 2023-12-04 at 3.39.34 PM.png" alt="" data-size="original">

</details>

**Defects Tab:**

<details>

<summary>The Defects tab provides information about failed test cases in the run, including the reporter, assignee, third-party app connections, and status.</summary>

<img src="../../../.gitbook/assets/Screenshot 2023-12-04 at 3.40.19 PM.png" alt="" data-size="original">

</details>

**Team Stats Tab:**

<details>

<summary>The Team Stats tab provides information about your teammates in the Test Run, including their work time, results, and a performance trend chart.</summary>

<img src="../../../.gitbook/assets/Screenshot 2023-12-04 at 3.40.48 PM.png" alt="" data-size="original">

</details>

## Test Run Wizard <a href="#h_c61f64e291" id="h_c61f64e291"></a>

***

Opening is the wizard is easy, just click on a test case in a Run. You can also get to the wizard in the following ways:

1. Click "Open Wizard" in the Dashboard:
2. Click 'Open Wizard' in the Test Runs Menu
3. Click "Run Wizard" in the "..." menu of a Test Case:

<figure><img src="https://downloads.intercomcdn.com/i/o/869079455/39df908cb68cb414ed1a87e9/Open+Wizard.gif" alt=""><figcaption></figcaption></figure>

In the wizard, can you advance through Test Cases, add comments, attachments, and log results for both individual steps and the entire Test Case.

<figure><img src="https://downloads.intercomcdn.com/i/o/869367531/818786a401bf702c3b7f218a/Record+results+in+wizard.gif" alt=""><figcaption></figcaption></figure>

You can also file defects as you work through the test case. Check the [defects](https://docs.qase.io/general/get-started-with-the-qase-platform/defects) article for more information.

In the wizard, use the "View/Edit Case" buttons to open a test case in a new tab for viewing or making changes.

<figure><img src="https://downloads.intercomcdn.com/i/o/869084642/dfe2697085d82920c009cf9d/slack_J0zUslKKIh.png" alt=""><figcaption></figcaption></figure>

<details>

<summary>NB: If you've enabled the "Fail case on step fail" option in Project settings, failing any Test Case step will automatically result in the entire Test Case failing. To prevent this, adjust the setting.</summary>

<img src="../../../.gitbook/assets/Screenshot 2023-12-04 at 3.42.18 PM.png" alt="" data-size="original">

</details>

## Editing a completed Test Run <a href="#h_1cd6dc8def" id="h_1cd6dc8def"></a>

***

After finishing a Test Run, you can add results by enabling "Allow to add results for cases in closed runs" in settings.\
​\
Then, go to Test Runs, open the run using the "Open Wizard" option. In the wizard, click the edit icon (pencil) to adjust the run duration, add comments, and attachments.

Save changes with the green check mark or discard them with the red cross.

<figure><img src="https://downloads.intercomcdn.com/i/o/869123577/e6f80665161c5eb67785f3c6/add+comments+after+test+run+is+completed.gif" alt=""><figcaption></figcaption></figure>

## Test Run Settings <a href="#h_2b8f9ef7e0" id="h_2b8f9ef7e0"></a>

***

Under Project Settings, there's a dedicated section for modifying run behaviour.\
​

<figure><img src="https://downloads.intercomcdn.com/i/o/610014375/9a470ae62733b2b704ad4894/image.png" alt=""><figcaption></figcaption></figure>

Let's look at each option in more detail:

| Option                                        | Behaviour                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| --------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fast Pass                                     | <ul><li>Enabled: you won't be prompted to add extra details when marking a test case as "passed"/ "skipped."</li></ul><ul><li>Disabled: A modal window appears for adding extra details like comments or attachments when marking a case as "passed"/ "skipped."</li></ul>                                                                                                                                                                                                                                 |
| Default create/attach defect checkbox         | <ul><li>Enabled: The checkbox for creating a defect is checked by default when you fail, invalidate, or mark a case as "blocked."</li></ul><ul><li>Disabled: The checkbox is unchecked by default in those scenarios.</li></ul>                                                                                                                                                                                                                                                                            |
| Auto complete                                 | <ul><li>Enabled: A run is automatically marked as complete when all cases have a result.</li></ul><ul><li>Disabled: You need to manually mark the run as complete, even when all cases have a result.</li></ul>                                                                                                                                                                                                                                                                                            |
| Auto passed                                   | <ul><li>Enabled: Marking all steps of a case as "passed" automatically marks the entire case as "passed."</li></ul><ul><li>Disabled: You need to separately mark the case as "passed," even if all steps are "passed."</li></ul>                                                                                                                                                                                                                                                                           |
| Auto assignee                                 | <ul><li>Enabled: Unassigned test cases are automatically assigned to the first person who opens them in the Wizard.</li></ul><ul><li>Disabled: Unassigned cases remain unassigned until explicitly assigned.</li></ul>                                                                                                                                                                                                                                                                                     |
| Auto create test cases                        | <p>For results reported via API or an API reporter.</p><ul><li><p>Enabled: If the result refers to a test case that is not in your Qase repository, a new case is created. Also, any updates will be made</p><p>Later on, if something changes in that test case upon the next result submission, related test case in the repository will get updated accordingly with this option enabled</p></li></ul><ul><li>Disabled: cases are not created/updated for results of non-existent test cases.</li></ul> |
| Fail case on step fail                        | <ul><li>Enabled: Failing any step will cause the whole case to be marked as "failed," preventing you from recording results for the remaining steps.</li></ul><ul><li>Disabled: You can proceed with the case even if a step has failed.</li></ul>                                                                                                                                                                                                                                                         |
| Allow to add results for cases in closed runs | <ul><li>Enabled: You can continue submitting results or retesting cases in completed or aborted runs.</li></ul><ul><li>Disabled: Closed runs do not allow further result submissions.</li></ul>                                                                                                                                                                                                                                                                                                            |
| Assignee result lock                          | <ul><li>Enabled: Only the assignee can submit results; others must explicitly assign themselves to do so.</li></ul><ul><li>Disabled: Any user, even if not assigned, can submit results, but results are associated with the submitter.</li></ul>                                                                                                                                                                                                                                                          |
| Redirect after adding result                  | <ul><li>No redirect: Stay on the same case after submitting a result.</li></ul><ul><li>First case in a run without result: Redirect to the first case without results.</li><li>Next case in suite: Go directly to the next case in the suite without results.</li></ul>                                                                                                                                                                                                                                    |

***

Related Articles[Getting Started](https://help.qase.io/en/articles/5563688-getting-started)[Defects](https://help.qase.io/en/articles/5563710-defects)[Milestones](https://help.qase.io/en/articles/5563715-milestones)[ClickUp](https://help.qase.io/en/articles/6417208-clickup)[GitHub](https://help.qase.io/en/articles/7210938-github)Did this answer your question?😞😐😃

***

[![Qase Help Center](https://downloads.intercomcdn.com/i/o/444276/b9f73a5efc21c8b8534fe131/3244aa26a7406f15b86f7a29338576a1.png)](https://help.qase.io/en/)1007 N Orange St. 4th Floor, Suite #1686, Wilmington, DE 19801, USA[We run on Intercom](https://www.intercom.com/intercom-link?company=Qase\&solution=customer-support\&utm\_campaign=intercom-link\&utm\_content=We+run+on+Intercom\&utm\_medium=help-center\&utm\_referrer=https%3A%2F%2Fhelp.qase.io%2Fen%2Farticles%2F5563702-test-runs\&utm\_source=desktop-web)

* [![](https://intercom.help/qase/assets/svg/icon:social-linkedin/d6d4d6)](https://www.linkedin.com/company/qaseio)
* [![](https://intercom.help/qase/assets/svg/icon:social-facebook/d6d4d6)](https://www.facebook.com/qase.io)
* [![](https://intercom.help/qase/assets/svg/icon:social-twitter-x/d6d4d6)](https://www.twitter.com/qase\_io)
* [![](https://intercom.help/qase/assets/svg/icon:social-github/d6d4d6)](https://github.com/qase-tms)
* [![](https://intercom.help/qase/assets/svg/icon:social-youtube/d6d4d6)](https://www.youtube.com/channel/UCvJ5CYaKZBcpD3OK4I-M\_kA)

<details>

<summary>From Saved Queries: You can read more about Saved Queries <a href="https://help.qase.io/en/articles/6417205-saved-queries">here</a>.</summary>

[![](https://downloads.intercomcdn.com/i/o/861868721/89a9e6373dd34a9c59596efb/image.png)](https://downloads.intercomcdn.com/i/o/861868721/89a9e6373dd34a9c59596efb/image.png)

</details>

\
\


<figure><img src="https://downloads.intercomcdn.com/i/o/609555539/dfbe57eec81a957724b876b3/image.png" alt=""><figcaption></figcaption></figure>

1. With the new test run configured, you will now see it in the Test Runs view with a condensed summary of it:
   * _Time:_ will show how much time has been spent so far on performing Test Cases in this run.
   * _Status:_ will show a summary of test cases per status - how many have passed, how many have been failed, skipped, blocked, invalidated, or untested.
   * _Environment:_ will show the environment of the run, which was selected when the run was created.

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597136810/38299ec2ee688929eb1d4101/yi62DXxzp81XizHNw0_XHjtj8qU9djtMnCoRBAe7hBL18REg2p0im4gRGqwI1PAIW5bSF0kZQ3w6RJFtUvmPHSO62Q_-Do1Sxn5NjalrMvZtxQY9ok8PRayGERXxOHqVE6G72xo6dsEsNaZlaupoFwWBPXcqiDHm-eqzDa8OFqfnyfDqWHlqe3IUUQ" alt=""><figcaption></figcaption></figure>

#### Filtering

You can filter by Status, Assigned to, Environment, Milestone, Tags, Automation status, and Creation date.

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597136814/6c495e548884def4d4832831/TmLVNE0TMUH3e9b6ts_dVlU4BterNbCQ_nqXdL-wJdByLWCvBjxWalMqIvDu2xjsrsAcdFOfCv0SAQ1OWrrTNtpdYp6H1G8L6ZdzIK776Qzvz-VpnnoKlwcxU6NT5vR8wD5lfN2cGK4-Jeq5jR6Z2gObcGRU7uQifg_MTaxJBd2gYNe2NSUpJ8y34A" alt=""><figcaption></figcaption></figure>

#### Three-dots-menu options

From the three-dots-menu, you can do several things:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597136820/e12770bc16c1f39b8de8ec76/hJnIE5leUSKI2zC7_L52HDzzGYVF8XKQvbocuraLH9atQfrNz_aYbd2bXvsS_P0-Z9yNW0M99R9bfWOKYiZ8CBiWwmwt6Oi46AWAhjjuifEwEBt0_TiVTiqEop2yhBIsc3fGW8Cfpou7wppeh6usiWQrYvUED-hoSL9-KfbHZ_nrB41a0UjfnWxXcQ" alt=""><figcaption></figcaption></figure>

* Access test run dashboard
*   _Open Wizard:_ this option will take you to the list of test cases that need to be performed, and you can go through them one by one:\




    \


    <figure><img src="https://qase.intercom-attachments-7.com/i/o/597136824/9764341b81f38ad00d678410/Cuj9OsxhiwMiA9mB2SA1j9krQUbVmkejejGiqxlI1xH7D9re6RrqlgP5NYvCP4dNHngUmUDTHpZaDJff1RyVOlGq8A22IOhQzTdpIRlDrTkGa8VhNPLj-nECakUJHjEG3xcyZBAer5qQMkUsH518hcMm35kZ0Y2Bu9aI83OrtpOmc2mtMIvB_QEhuA" alt=""><figcaption></figcaption></figure>
* _Clone Run:_ quickly create an identical instance of a test run, if you want to perform it again from scratch
* _Edit run:_ change the parameters of the test run
* Delete test run

\
