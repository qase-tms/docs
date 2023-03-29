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

#### **Regular test run**

To create a regular test run:

1. Go to the "Test Runs" section.
2.  Click the "Start New Test Run" button.\


    <figure><img src="https://qase.intercom-attachments-7.com/i/o/597420795/ea9a99eb365b3fdc5684509a/WUBZGWDp5wDmW5j_cfcUKSQTP55S59lbdn0BO1vcRPD0FWbgxxCgAkLfUaAmqwwkKyJl0lC7BK_uLhW4X8usGcTZNJtB3Zuq11YMV-e7F8iV18EXabJlvb6VNeXojXH77GloD5-D0H12Zr-5SXMN547ZJPsazginDcvCQ9IQ-VGAJdS1A0XCdVJgUw" alt=""><figcaption></figcaption></figure>
3. Fill out the configuration form with the following information:
   * _Run title:_ the name of your test run (defaults to the current date).
   * _Description:_ additional details about the test run.
   * _Plan:_ choose which test plan should be performed in the test run.
   * _Environment:_ define in which environment the test run should be performed (testing, staging, production).
   * _Milestone:_ select which Milestone the test run is tied to.
   * _Default Assignee:_ choose whether all test cases within the test run should be automatically assigned to a specific teammate; leaving this field undefined will leave the test cases unassigned in the test run (you will then need to assign them manually).
   * _Tags:_ you can assign any of the tags that you have used previously, or create a new one.
   * _Test Cases:_ if you selected a test plan in the plan field earlier, all test cases contained in this test plan would be automatically included in the test run. However, if the test run does not encompass the entire test plan, you can choose which test cases from it should be performed, and which shouldn't.
   *   _Integrations:_ you can link any of the integrated apps’ issues with your new test run.\


       <figure><img src="https://qase.intercom-attachments-7.com/i/o/597420817/4512bf9d329a0984b6386e18/qN7T1HffeQv_N0ueP_1DPe4clf4V37e4yk-ANgH0w6xKAlMk5wmqhJ_qj40ZmfyfR3ntTsZLhebB5UsyLlDjFd6ZZATRwVZlPoLf7zJC4l9jDFpN1ofWIHtchJcRA2VcaNTF2JJ43UnMqAZGGswq5IP8xXOi5vnZSfxjIrNg0U9gnUI27-IjwPmYAA" alt=""><figcaption></figcaption></figure>
4.  Keep in mind that any settings established for test runs in the project settings will be applied to your test run.\


    <figure><img src="https://downloads.intercomcdn.com/i/o/609555539/dfbe57eec81a957724b876b3/image.png" alt=""><figcaption></figcaption></figure>
5. With the new test run configured, you will now see it in the Test Runs view with a condensed summary of it:
   * _Time:_ will show how much time has been spent so far on performing Test Cases in this run.
   * _Status:_ will show a summary of test cases per status - how many have passed, how many have been failed, skipped, blocked, invalidated, or untested.
   * [_Environment_](https://help.qase.io/en/articles/5563723-environments)_:_ will show the environment of the run, which was selected when the run was created.

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
