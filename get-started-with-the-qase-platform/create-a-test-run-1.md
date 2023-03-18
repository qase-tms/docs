---
title: Test Run creation & management in Qase
slug: create-a-test-run-1
hidden: true
createdAt: '2023-02-08T03:29:25.607Z'
updatedAt: '2023-02-21T19:47:34.265Z'
---

# Test runs

### What is a test run in software testing?

A test run is a set of test cases to be executed on a specific app build, along with information about their execution status. If we have 2 versions of the app, iOS and Android, we need to test both. So we perform the same test cases in 2 separate Test Runs for each version.

There are two ways to perform a Test Run: an Express Test Run and a regular Test Run.

#### **Express Test Run**

Express test runs are set up by selecting multiple Test Cases in the repository and hitting the "Run" button; optionally, you can choose which Environment testing should be performed in, and which Milestone a test run will be related to.

**Regular Test Run**

To create a regular test run:

1. Go to the "Test Runs" section.
2. Click the "Start New Test Run" button.
3. Fill out the configuration form with the following information:
   * Run title: the name of your test run (defaults to the current date).
   * Description: additional details about the test run.
   * Plan: choose which test plan should be performed in the test run.
   * Environment: define in which environment the test run should be performed (testing, staging, production).
   * Milestone: select which Milestone the test run is tied to.
   * Default Assignee: choose whether all test cases within the test run should be automatically assigned to a specific teammate; leaving this field undefined will leave the test cases unassigned in the test run (you will then need to assign them manually).
   * Tags: you can assign any of the tags that you have used previously, or create a new one.
   * Test Cases: if you selected a test plan in the plan field earlier, all test cases contained in this test plan would be automatically included in the test run. However, if the test run does not encompass the entire test plan, you can choose which test cases from it should be performed, and which shouldn't.
   * Integrations: you can link any of the integrated apps’ issues with your new test run.
4. Keep in mind that any settings established for test runs in the project settings will be applied to your test run.

