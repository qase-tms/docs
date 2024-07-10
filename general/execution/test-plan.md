# Test plan

### What is a test plan in software testing?

Test Plan is your way to organize the various [Test Cases](https://docs.qase.io/general/get-started-with-the-qase-platform/test-cases) into a cohesive scenario that will encompass various cases from different domains (i.e., different [Test Suites](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-suite)). Later on, when performing [Test Runs](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run), you will use a pre-created Test Plan, which already contains every Test Case and/or Test Suite necessary.

{% embed url="https://www.youtube.com/watch?v=vLZngELifvA" %}

When composing a new Test Plan, you can add standalone Test Cases and entire Test Suites alike.

To create a new Test Plan, navigate to the "Test Plans" section, and hit "Create Test Plan":

<figure><img src="../../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

Once in the Test Plan creation menu, fill in the Plan details:

1. Title:
2. Description:

<figure><img src="../../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

Next, choose which Test Cases or Test Suites your new Test Plan will contain. You can add standalone Test Cases by highlighting a Test Suite and picking Test Cases from it individually and you can add an entire Test Suite by checking the box for it in the left-hand column.

_Note_: You can also use the search bar to search for specific cases that you would like to include in the plan. Also, while selecting cases, you can assign specific cases to certain users. The assignments can then be carried over to all future test runs built based on this test plan.

Finally, confirm by hitting the "Create plan" button below.\


<figure><img src="../../.gitbook/assets/create a new test plan.gif" alt=""><figcaption></figcaption></figure>

After a new Test Plan has been created, you will find it in the "Test Plans" section, with some of the Plan attributes shown - run time, number of cases, time of creation, and update time.

<figure><img src="../../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

_Note_: Once a test run has been created from this plan, upon opening this plan you will see a tab “Test Runs” which shows all the runs started based on this plan.

<figure><img src="../../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>

From the Menu button "..." next to a test plan, you can Edit, Delete or Export your Test Plan as XLS:

<figure><img src="../../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

You can also select multiple test plans to delete them in bulk.

<figure><img src="../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

**Note:** If you introduce changes to a Test Plan (add or remove cases into/from it), it may affect your currently active test runs, that use this plan. The table below shows which changes will be happening:

|                                  | <p><mark style="background-color:red;">Active test run,</mark></p><p><mark style="background-color:red;">no results,</mark></p><p><mark style="background-color:red;">run not completed</mark></p> | <p><mark style="background-color:yellow;">Active test run,</mark></p><p><mark style="background-color:yellow;">results have been added, but the run is not completed</mark></p> | <mark style="background-color:green;">A completed test run</mark> |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| Test Case is added to a Plan     | Case is added to a run                                                                                                                                                                             | Case is added to a run                                                                                                                                                          | Case is NOT added to a run                                        |
| Test Case is removed from a Plan | Case is removed from a run                                                                                                                                                                         | Case is NOT removed from a run                                                                                                                                                  | Case is NOT removed from a run                                    |
