---
title: "Create a test case"
slug: "create-a-test-run"
hidden: true
createdAt: "2023-02-08T03:24:51.276Z"
updatedAt: "2023-02-21T19:51:57.615Z"
---
***What is a test case in software testing? ***

A test case contains all the details about our test. A title is enough to create a quick test case. For a more detailed test case, you can define prerequisites, steps, expected and actual results, etc.


##Create Test Case

**Quick test case**
1. On the page, under your test suite click on the link “+ Create quick test”

2. The cursor will start blinking on the page, and you can start typing the title. Click Enter to save the test case. As a result, a new test case under the test suite is shown with ID and a title.

This is the fastest way to add a test case, let’s see how to create a more sophisticated one.

##Detailed test case
[block:html]
{
  "html": "<div>\n  <ol>\n    <li>On the main repository page, click on the button “+ Case”</li>\n\n<li>As a result, a new page “Create test case” is shown. Let’s fill in the most important fields:</li>\n\n<li>Title: describes what is being tested by the test case</li>\n\n<li>Status: denotes the status of the case itself</li>\n\n<li>Suite: which suite the test case belongs to</li>\n\n<li>Priority: how important is this test case during test execution?</li>\n\n<li>Severity: what is the impact on our app’s quality status if this test case fails?</li>\n\n<li>Is flaky: determines if the test case is flaky</li>\n\n<li>Automation status: denotes if the test case is automated, to be automated, or not automated</li>\n\n<li>Pre-conditions: the prerequisites for our test</li>\n\n<li>Steps to reproduce: list of actions and expected results after each action</li>\n\n<li>To save a test case click on the button “Save”. As a result, the page “Test repository” is shown with a new test case. Icons with arrows in front show the priority and severity of the test case</li>\n\n<li>We have added our first test cases, let’s execute them in a new test run</li>\n  </ol>\n  \n\n</div>"
}
[/block]