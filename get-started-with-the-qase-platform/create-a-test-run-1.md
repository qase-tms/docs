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

There are two ways to perform a test run: an express test run and a regular test run.

#### **Express test run**

Express test runs are set up by selecting multiple test cases in the repository and hitting the "Run" button; optionally, you can choose which environment testing should be performed in, and which milestone a test run will be related to.\


<figure><img src="https://qase.intercom-attachments-7.com/i/o/597420631/c849b9bde959f63612ddddb4/iu7VUj0rrf8F8dW5u6LX6XutC8MN-ru7xOc-Ir31w3Fe2IpPS0-t0nguBngsSYkBnb8QySlSxnygVvh-q-NOWRAB2wZj3WgDtJWdUzlqVVNgLbiywGAKZBVmIMEo1WMpq222MW7NPySWINa7UExwRBS6TsW-QEz8hGuu9ragbRv66kUCjRLMMveguQ" alt=""><figcaption></figcaption></figure>

**Regular test run**

To create a regular test run:

1. Go to the "Test Runs" section.
2.  Click the "Start New Test Run" button.\


    <figure><img src="https://qase.intercom-attachments-7.com/i/o/597420795/ea9a99eb365b3fdc5684509a/WUBZGWDp5wDmW5j_cfcUKSQTP55S59lbdn0BO1vcRPD0FWbgxxCgAkLfUaAmqwwkKyJl0lC7BK_uLhW4X8usGcTZNJtB3Zuq11YMV-e7F8iV18EXabJlvb6VNeXojXH77GloD5-D0H12Zr-5SXMN547ZJPsazginDcvCQ9IQ-VGAJdS1A0XCdVJgUw" alt=""><figcaption></figcaption></figure>
3. Fill out the configuration form with the following information:
   * Run title: the name of your test run (defaults to the current date).
   * Description: additional details about the test run.
   * Plan: choose which test plan should be performed in the test run.
   * Environment: define in which environment the test run should be performed (testing, staging, production).
   * Milestone: select which Milestone the test run is tied to.
   * Default Assignee: choose whether all test cases within the test run should be automatically assigned to a specific teammate; leaving this field undefined will leave the test cases unassigned in the test run (you will then need to assign them manually).
   * Tags: you can assign any of the tags that you have used previously, or create a new one.
   * Test Cases: if you selected a test plan in the plan field earlier, all test cases contained in this test plan would be automatically included in the test run. However, if the test run does not encompass the entire test plan, you can choose which test cases from it should be performed, and which shouldn't.
   *   Integrations: you can link any of the integrated apps’ issues with your new test run.\


       <figure><img src="https://qase.intercom-attachments-7.com/i/o/597420817/4512bf9d329a0984b6386e18/qN7T1HffeQv_N0ueP_1DPe4clf4V37e4yk-ANgH0w6xKAlMk5wmqhJ_qj40ZmfyfR3ntTsZLhebB5UsyLlDjFd6ZZATRwVZlPoLf7zJC4l9jDFpN1ofWIHtchJcRA2VcaNTF2JJ43UnMqAZGGswq5IP8xXOi5vnZSfxjIrNg0U9gnUI27-IjwPmYAA" alt=""><figcaption></figcaption></figure>
4.  Keep in mind that any settings established for test runs in the project settings will be applied to your test run.\


    <figure><img src="https://downloads.intercomcdn.com/i/o/609555539/dfbe57eec81a957724b876b3/image.png" alt=""><figcaption></figcaption></figure>

