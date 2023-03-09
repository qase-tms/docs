---
title: "Test Run creation & management in Qase"
slug: "create-a-test-run-1"
hidden: true
createdAt: "2023-02-08T03:29:25.607Z"
updatedAt: "2023-02-21T19:47:34.265Z"
---
[block:api-header]
{
  "title": "Create Test Run"
}
[/block]
Test Runs represent a set of test cases to be executed on a specific app build along with the status of their execution. We can have 2 versions of the app: iOS and Android. Both need testing, so for each version, we will perform the same test cases in 2 separate Test Runs.

There are two ways to perform a Test Run: an Express Test Run and a regular Test Run.

**Express Test Run**
Express test runs are set up by selecting multiple Test Cases in the repository and hitting the "Run" button; optionally, you can choose which Environment testing should be performed in, and which Milestone a test run will be related to:

##Regular Test Run

To create a regular test run, navigate to "Test Runs" section, and hit the "Start New Test Run" button

In the configuration form, there are several fields you can fill out

  * Run title: the name of your test run, this field is pre-filled in with the current date, but you can change it to whichever nomenclature you use.
  * Description: additional details about the test run.
  * Plan: choose which Test Plan should be performed in the Test Run.
  * Environment: define in which environment should the test run be performed (i.e., testing, staging, production).
  * Milestone: select which Milestone the Test Run is tied to.
  * Default Assignee: choose whether all Test Cases within the Test Run should be automatically assigned to a specific teammate; leaving this field undefined will leave the Test Cases unassigned in the Test Run (you will then need to assign them manually).
  * Tags: You can assign any of the tags that you have used previously. Or you can create a new tag as well.
  * Test Cases: if you selected a Test Plan in the Plan field earlier, all Test Cases contained in this Test Plan would be automatically included in the Test Run. However, if the Test Run does not encompass the entire Test Plan, you can choose which Test Cases from it should be performed, and which shouldn't.
  * Integrations: You can link any of the integrated apps’ issues with your new test run as well. 

Keep in mind that any settings established for Test Runs in the Project Settings will be applied to your Test Run

With the new Test Run configured, you will now see it in the Test Runs view with some condensed summary of it

* Time will show how much time has been spent so far on performing Test Cases in this run.
* Status will show a summary of test cases per status - how many have passed, how many have been failed, skipped, blocked, invalidated or untested.
* Environment will show the environment of the run which was selected when the run was created.

Test Runs section is filtered to show only Active Runs by default, but you can switch it with the help of the “Add filters” option. You can filter by Status, Assigned to, Environment, Milestone, Tags, Automation status, and Creation date.