---
description: >-
  Learn how to use Muted Tests in Qase, which can be especially useful for
  handling flaky tests or those test cases that are currently less critical.
---

# Muted Tests



{% embed url="https://www.youtube.com/watch?v=HfKF0foo4yM" %}

Test cases in Qase can be marked muted. This functionality is especially useful for handling flaky tests or those test cases that are currently less critical. When a test is marked as "muted", its results will not affect the overall status of test runs. This means your test runs can still pass even if a muted test fails, preventing unnecessary delays in your release process.

***

#### How to mark a test case "muted": <a href="#h_f68b6c8793" id="h_f68b6c8793"></a>

<mark style="background-color:yellow;">**Ability to mute or unmute test cases is regulated by a user permission "Mute/Unmute" in the "Test cases" category of a**</mark> [<mark style="background-color:yellow;">**user role**</mark>](https://docs.qase.io/administration/workspace-management/roles)<mark style="background-color:yellow;">**.**</mark>

<mark style="background-color:yellow;">**Among the system roles, it is enabled for Owner and Administrator roles.**</mark>

\ <mark style="background-color:yellow;">**For custom user roles, it can be granted through editing a custom role.**</mark>

1. In the repository, open a test case in the preview sidebar, switch to the "Properties" tab and check the box for "Muted case":

<figure><img src="../../../.gitbook/assets/muted case.png" alt=""><figcaption></figcaption></figure>

2. Open a test case in edition mode, and check the box for "Muted case":

<figure><img src="../../../.gitbook/assets/muted case 2.png" alt=""><figcaption></figcaption></figure>

3. Select multiple cases in the repository and bulk edit them, checking the "Muted" box:

<figure><img src="../../../.gitbook/assets/multiple muted cases.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/bulk edit.png" alt=""><figcaption></figcaption></figure>

4. In a test run, select a test case and click the "Mute" button above the result statuses:

<figure><img src="../../../.gitbook/assets/mute button.png" alt=""><figcaption></figcaption></figure>

Muted test cases will appear as such:

* in the repository:

<figure><img src="../../../.gitbook/assets/repo.png" alt=""><figcaption></figcaption></figure>

* in the test runs where they have been added:

<figure><img src="../../../.gitbook/assets/muted in test runs.png" alt=""><figcaption></figcaption></figure>

<mark style="background-color:yellow;">**If a test case has been "muted" from a test run, it will also appear "muted" in the repository.**</mark>

Any previously muted test case can be "unmuted" at any time by unchecking the "Muted case" box when editing a test case - or by clicking an "Unmute" button when viewing the test case in a test run:

<figure><img src="../../../.gitbook/assets/unmute.png" alt=""><figcaption></figcaption></figure>



***

#### How do muted tests affect the test run test run status? <a href="#h_58ec2fe3e4" id="h_58ec2fe3e4"></a>

* if a test run includes a muted test case, then a Failed, Invalid, Blocked result (or a custom result of a "Failure" type) submitted for such a case will not affect the completion status of the test run, i.e. having failed a muted test case will not result in the test run getting marked failed:

<figure><img src="../../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

* if a test run already has a completion status (Passed/Failed), even after extra test cases were added into it or cases were muted - after the run was completed - the completion status of the run will not be recalculated;
* when [parametrized test cases](https://docs.qase.io/general/get-started-with-the-qase-platform/test-cases/test-case-parameters) are included in a run, marking one of the parametrized siblings "muted" will also mute all the other parametrized versions of such a test case.
