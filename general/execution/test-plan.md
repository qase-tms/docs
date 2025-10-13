# Test plan

### What is a test plan in software testing?

Test Plan is your way to organize the various [Test Cases](https://docs.qase.io/general/get-started-with-the-qase-platform/test-cases) into a cohesive scenario that will encompass various cases from different domains (i.e., different [Test Suites](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-suite)).&#x20;

Later on, when performing [Test Runs](../get-started-with-the-qase-platform/create-a-test-run/), you will use a pre-created Test Plan, which already contains every Test Case and/or Test Suite necessary.

When composing a new Test Plan, you can add standalone Test Cases and entire Test Suites alike.&#x20;

{% embed url="https://www.youtube.com/watch?v=vLZngELifvA" %}

To create a new Test Plan, navigate to the "Test Plans" section, and hit "Create Test Plan":

<figure><img src="../../.gitbook/assets/image (40).png" alt="" width="563"><figcaption></figcaption></figure>

Once in the Test Plan creation menu, fill in the Plan details:

1. Title:
2. Description:

<figure><img src="../../.gitbook/assets/image (41).png" alt="" width="563"><figcaption></figcaption></figure>

Next, choose which Test Cases or Test Suites your new Test Plan will contain. You can add standalone Test Cases by highlighting a Test Suite and picking Test Cases from it individually and you can add an entire Test Suite by checking the box for it in the left-hand column.

_Note_: You can also use the search bar to search for specific cases that you would like to include in the plan. Also, while selecting cases, you can assign specific cases to certain users. The assignments can then be carried over to all future test runs built based on this test plan.

Finally, confirm by hitting the "Create plan" button below.\


<figure><img src="../../.gitbook/assets/create a new test plan.gif" alt="" width="563"><figcaption></figcaption></figure>

After a new Test Plan has been created, you will find it in the "Test Plans" section, with some of the Plan attributes shown - run time, number of cases, time of creation, and update time.

<figure><img src="../../.gitbook/assets/image (42).png" alt="" width="563"><figcaption></figcaption></figure>

_Note_: Once a test run has been created from this plan, upon opening this plan you will see a tab “Test Runs” which shows all the runs started based on this plan.

<figure><img src="../../.gitbook/assets/image (43).png" alt="" width="563"><figcaption></figcaption></figure>

From the Menu button "..." next to a test plan, you can Edit, Delete or Export your Test Plan as XLS:

<figure><img src="../../.gitbook/assets/image (44).png" alt="" width="563"><figcaption></figcaption></figure>

You can also select multiple test plans to delete them in bulk.

<figure><img src="../../.gitbook/assets/image (45).png" alt="" width="563"><figcaption></figcaption></figure>



### Clone a test plan <a href="#h_03d7d74503" id="h_03d7d74503"></a>

You can clone a test plan w/ or w/o the assignees. You can edit the name of the new plan before cloning.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1775959390/076fde12fc24320fa06d43bd0b12/image.png?expires=1760373150&#x26;signature=e6718d5e58ad1f4300221bab6c0b35cf77c80d9604c63ac0bd2bb0cbf9f8ef6f&#x26;req=dScgE8B7lIJWWfMU3HP0gD%2B4IYDSqyxMfvFv6SbvhURESIvu0vw%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1775962810/ae2883e414cbde3053d30de47bf8/image.png?expires=1760373150&#x26;signature=744ea372cc55007e958f896ce7f5e5aeef2cf3599479a6cb88a0095f401c71f5&#x26;req=dScgE8B4n4leWfMU3HP0gBV%2BRnNNzX%2Fbq0sdbzwMhZUBtf47l64%3D%0A" alt="" width="375"><figcaption></figcaption></figure>

**Note:** If you introduce changes to a Test Plan (add or remove cases into/from it), it may affect your currently active test runs, that use this plan. The table below shows which changes will be happening:

<table data-header-hidden><thead><tr><th></th><th width="182"></th><th width="184"></th><th></th></tr></thead><tbody><tr><td></td><td><p><mark style="background-color:orange;">Active test run - (Run NOT completed),</mark></p><p><mark style="background-color:orange;">No results</mark></p></td><td><p><mark style="background-color:orange;">Active test run,</mark></p><p><mark style="background-color:orange;">results have been added, but the run is not completed</mark></p></td><td><mark style="color:orange;background-color:orange;">A completed test run</mark></td></tr><tr><td><mark style="background-color:green;">Test Case is added to a Plan</mark></td><td>Case is added to a run</td><td>Case is added to a run</td><td>Case is NOT added to a run</td></tr><tr><td><mark style="background-color:red;">Test Case is removed from a Plan</mark></td><td>Case is removed from a run</td><td>Case is NOT removed from a run</td><td>Case is NOT removed from a run</td></tr></tbody></table>
