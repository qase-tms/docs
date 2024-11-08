---
title: Test Run creation & management in Qase
slug: create-a-test-run-1
createdAt: '2023-02-08T03:29:25.607Z'
updatedAt: '2023-02-21T19:47:34.265Z'
---

# Test runs

### What is a test run in software testing?

A Test Run is a single instance of executing a specific set of test cases.

{% embed url="https://www.youtube.com/watch?v=7bLibOsfchs" %}

A Test Run may consist one Test case, a bunch of them, whole sets of Test cases ([Test Suite](https://help.qase.io/en/articles/5563702-test-runs)), or even Test cases from different areas bundled together in a Test Plan.

There are two ways to start a Test Run:\
1\. **Express Run** - from the Project's Repository page.\
2\. **Regular Run** - from Test Runs page.



***

### **Express Run**

You can quickly set up a Test Run for one or more test cases directly from the Repository.

​ Hit the "Run" button and proceed to select the Environment, Milestone, Configurations, or any other fields, as needed.



<figure><img src="../../../.gitbook/assets/express run.gif" alt=""><figcaption></figcaption></figure>

### **Regular test run**

To create a regular test run, navigate to "Test Runs" section, and hit the "Start New Test Run" button. You will see the same modal window as seen while creating a Test Run from the Repository page.

\


<figure><img src="../../../.gitbook/assets/normal run.gif" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

<details>

<summary>You can filter the Runs by Status, Assigned to, Environment, Milestone, Tags, Automation status, Creation date, and your <a href="https://docs.qase.io/administration/workspace-management/custom-fields">custom fields</a> (if any).</summary>

<img src="../../../.gitbook/assets/image (24).png" alt="" data-size="original">

</details>

<details>

<summary>From the "..." menu, you can do several things:</summary>

<img src="../../../.gitbook/assets/image (25).png" alt="" data-size="original">

</details>

<details>

<summary>You can bulk delete Test runs by selecting the runs you want to delete in bulk, clicking "Update selected" and then "Delete."<br></summary>

<img src="../../../.gitbook/assets/image (26).png" alt="" data-size="original">

</details>

A **Test run Status** will be assigned once the run is marked as complete.

A 'Passed' status is given only if all\* tests have a positive result. One or more test cases with a negative result will automatically assign a 'Failed' status to the run.

Please note, status once assigned will not be re-calculated for any subsequent changes.

\* [Muted tests](https://help.qase.io/en/articles/9217182-muted-tests) are not considered when calculating the final run status.

## Test Run Results <a href="#h_f59c8094eb" id="h_f59c8094eb"></a>

***

Your test runs have the following default statuses available to reflect the outcome of test cases:

<figure><img src="../../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

1. **Passed** - The test case has been executed successfully, and the expected results match the actual outcomes.
2. **Failed** - The test case has failed, indicating discrepancies between the expected and actual results.
3. **Blocked** - The test couldn't be executed or completed due to some blocking issue, such as a dependency not met, environmental issues, or other constraints.
4. **Skipped** - The test case was intentionally skipped during the test run, often due to its non-applicability or other reasons.
5. **Invalid** - The test run wasn't completed for some reason, and the results are inconclusive.\
   ​\
   Test run results statuses can also be customized by navigating to the [Fields section in Workspace management](https://app.qase.io/workspace/fields) and clicking "Result status" (Admin permissions is needed to modify fields).

<figure><img src="../../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

You also have the option to define the action associated with your custom statuses where you can determine if a status triggers a successful test case or a failed test case. ​ If a status triggers a failed test case then the defect creation workflow is triggered.

<figure><img src="../../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

Please take note that you only have the option to hide custom statuses once deleted to preserve the results history in the test runs.\
​\
Also, Custom Test Run "Result status" is only available to users on a [paid subscription](https://help.qase.io/en/collections/3564563-subscriptions).

## Dashboard <a href="#h_e2d602414a" id="h_e2d602414a"></a>

***

To go to the Run dashboard, simply click on the Test Run name.

Let's explore the options available in the dashboard -

<figure><img src="../../../.gitbook/assets/run dashboards options numbered.png" alt=""><figcaption></figcaption></figure>

1**. Open Wizard:** this will guide you through the Test Cases contained in the run, step-by-step.

2\. **Share Report:** turn on public link and easily share your Run report with anyone, even if they don't have an account in Qase.

<details>

<summary>Example of a Shared report</summary>

<img src="../../../.gitbook/assets/Share Report demo (1).gif" alt="" data-size="original">

</details>

3\. **Export:** you can download a CSV export of your Test Run.

4\. **(---) Menu:** Clone run option allows you to create a new identical copy of your run. You can edit the run details, abort it or go the Test Run settings from here.

5\. **Search and Filters:** search cases by their title or Id and filter by a specific parameter.

6**. Defects and Team stats:** view all associated defects from this run and see stats for results by assignee.

7\. T**he "..." menu button:** has options to Run wizard, assign case to a team member or View/edit the Test case itself.

8\. **Run details:** this side bar houses a completion chart and other test run configuration details like -

* Environment, Configurations, Milestones and tags
* Run status, author, create date and estimated time for completion.
* Linked External Issues.

<details>

<summary><em>Expand to learn more</em></summary>



* **Donut Graph** shows the breakdown of Test Cases in the Run by status. Hovering over a section of the graph you will see the actual number of Cases in a respective Status. If you click on a section of the graph, a quick filter will be applied to show you only the Cases in a specific status.
* **Completion Rate** represents the percentage of Cases in a run that have been performed so far.
* **Status** lets you know if the run is currently active or completed.
* **Started by and Started at**  provide details on who started this Test Run, and when.
* **Estimation** predicts how long your current Test Run will take based on the time spent in previous Test Runs on the same Test cases.
* **Duration** is the summary of time that has been spent on all Test Cases in the current Test Run so far.
* **Environment, Tags, Configurations, Milestones, and Custom Fields**: Details about the specific environment of the test run and the associated tags, Milestones and Custom fields.
*   **External Issue:** You can link a test run with an issue/task from any issue tracker Apps that you have installed.

    Here's an example of a JIRA issue linked to a test run:

<img src="../../../.gitbook/assets/attach jira issue 2.gif" alt="" data-size="original">

</details>

9\. **Bulk actions:** You can select multiple test cases to assign/re-test/submit result/delete with the respective button.

<details>

<summary>Example</summary>

<img src="../../../.gitbook/assets/bulk post results.gif" alt="" data-size="original">

</details>

### Assignment <a href="#h_964117eb5f" id="h_964117eb5f"></a>

You have the flexibility to assign test cases within a test run either to individual users or to [groups](https://help.qase.io/en/articles/5563740-workspace-management-groups).

**Individual assignment:**

* You can assign specific test cases to individual testers. This approach is particularly useful when you want to assign a suite of test cases related to a specific feature to a tester with specialized knowledge in that area.

<figure><img src="../../../.gitbook/assets/indivi as.gif" alt=""><figcaption></figcaption></figure>

**Group Assignment:**

In this assignment mode, you can select a [group](https://help.qase.io/en/articles/5563740-workspace-management-groups) that includes multiple testers.

1. **Even distribution:** this strategy ensures that test cases are distributed as evenly as possible among the group members. For instance, _if there are 10 test cases and 5 testers in a group, each tester will receive 2 test cases._

<figure><img src="../../../.gitbook/assets/even.gif" alt=""><figcaption></figcaption></figure>

**Load balanced distribution:** this strategy optimizes the distribution of test cases based on their complexity, measured by previous test durations with the goal of evenly distributing the workload among group members.

<figure><img src="../../../.gitbook/assets/load bal.gif" alt=""><figcaption></figcaption></figure>

For instance_, If there are five test cases with expected durations of 30, 10, 10, 5, and 5 minutes, and two testers in a group, the system will assign the 30-minute test case to one tester and the remaining four test cases (with a combined duration of 30 minutes) to the other tester. This way, both testers have an even workload despite the number of test cases being different._

**Assignment settings:**

The default assignment strategy can be configured under the Test Runs tab in your Project's settings.

<figure><img src="../../../.gitbook/assets/run assign sett.gif" alt=""><figcaption></figcaption></figure>

This setting determines the default assignment strategy that appears when you attempt to assign cases to a group.

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

<figure><img src="../../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

<details>

<summary>NB: If you've enabled the "Fail case on step fail" option in Project settings, failing any Test Case step will automatically result in the entire Test Case failing. To prevent this, adjust the setting.</summary>

<img src="../../../.gitbook/assets/image (31).png" alt="" data-size="original">

</details>

## Editing a completed Test Run <a href="#h_1cd6dc8def" id="h_1cd6dc8def"></a>

***

After finishing a Test Run, you can add results by enabling "Allow to add results for cases in closed runs" in settings.\
​\
Then, go to Test Runs, open the run using the "Open Wizard" option. In the wizard, click the edit icon (pencil) to adjust the run duration, add comments, and attachments.

Save changes with the green check mark or discard them with the red cross.

<figure><img src="../../../.gitbook/assets/edit completed run.gif" alt=""><figcaption></figcaption></figure>

## Test Run Settings <a href="#h_2b8f9ef7e0" id="h_2b8f9ef7e0"></a>

***

Under Project Settings, there's a dedicated section for modifying run behaviour.

<figure><img src="../../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

\


Let's look at each option in more detail:

| Option                                        | Behaviour                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| --------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fast Pass                                     | <ul><li><strong>Enabled:</strong> you won't be prompted to add extra details when marking a test case as "passed"/ "skipped."</li></ul><ul><li><strong>Disabled:</strong> A modal window appears for adding extra details like comments or attachments when marking a case as "passed"/ "skipped."</li></ul>                                                                                                                                                                                                                                 |
| Default create/attach defect checkbox         | <ul><li><strong>Enabled:</strong> The checkbox for creating a defect is checked by default when you fail, invalidate, or mark a case as "blocked."</li></ul><ul><li><strong>Disabled:</strong> The checkbox is unchecked by default in those scenarios.</li></ul>                                                                                                                                                                                                                                                                            |
| Auto complete                                 | <ul><li><strong>Enabled:</strong> A run is automatically marked as complete when all cases have a result.</li></ul><ul><li><strong>Disabled:</strong> You need to manually mark the run as complete, even when all cases have a result.</li></ul>                                                                                                                                                                                                                                                                                            |
| Auto passed                                   | <ul><li><strong>Enabled:</strong> Marking all steps of a case as "passed" automatically marks the entire case as "passed."</li></ul><ul><li><strong>Disabled:</strong> You need to separately mark the case as "passed," even if all steps are "passed."</li></ul>                                                                                                                                                                                                                                                                           |
| Auto assignee                                 | <ul><li><strong>Enabled:</strong> Unassigned test cases are automatically assigned to the first person who opens them in the Wizard.</li></ul><ul><li><strong>Disabled:</strong> Unassigned cases remain unassigned until explicitly assigned.</li></ul>                                                                                                                                                                                                                                                                                     |
| Auto create test cases                        | <p>For results reported via API or an API reporter.</p><ul><li><p><strong>Enabled:</strong> If the result refers to a test case that is not in your Qase repository, a new case is created. Also, any updates will be made</p><p>Later on, if something changes in that test case upon the next result submission, related test case in the repository will get updated accordingly with this option enabled</p></li></ul><ul><li><strong>Disabled</strong>: cases are not created/updated for results of non-existent test cases.</li></ul> |
| Fail case on step fail                        | <ul><li><strong>Enabled:</strong> Failing any step will cause the whole case to be marked as "failed," preventing you from recording results for the remaining steps.</li></ul><ul><li><strong>Disabled:</strong> You can proceed with the case even if a step has failed.</li></ul>                                                                                                                                                                                                                                                         |
| Allow to add results for cases in closed runs | <ul><li><strong>Enabled:</strong> You can continue submitting results or retesting cases in completed or aborted runs.</li></ul><ul><li><strong>Disabled:</strong> Closed runs do not allow further result submissions.</li></ul>                                                                                                                                                                                                                                                                                                            |
| Assignee result lock                          | <ul><li><strong>Enabled:</strong> Only the assignee can submit results; others must explicitly assign themselves to do so.</li></ul><ul><li><strong>Disabled:</strong> Any user, even if not assigned, can submit results, but results are associated with the submitter.</li></ul>                                                                                                                                                                                                                                                          |
| Redirect after adding result                  | <ul><li><strong>No redirect:</strong> Stay on the same case after submitting a result.</li></ul><ul><li><strong>First case in a run without result:</strong> Redirect to the first case without results.</li><li><strong>Next case in suite:</strong> Go directly to the next case in the suite without results.</li></ul>                                                                                                                                                                                                                   |
| Default Assignment Strategy                   | <p></p><ul><li><strong>Even:</strong> This strategy ensures <em>even distrubution of test cases</em> among group members regardless of complexity.</li><li><strong>Load balanced:</strong> This strategy allocates test cases based on complexity to <em>evenly distribute the workload</em> among group members.</li></ul>                                                                                                                                                                                                                  |

***



\
\
