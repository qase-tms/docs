# Test case review



_<mark style="background-color:purple;">Review is available in</mark>_ [_<mark style="background-color:purple;">Business</mark>_](https://docs.qase.io/administration/subscriptions/business-plan) _<mark style="background-color:purple;">and</mark>_ [_<mark style="background-color:purple;">Enterprise</mark>_](https://docs.qase.io/administration/subscriptions/enterprise-plan) _<mark style="background-color:purple;">subscriptions.</mark>_



{% embed url="https://www.youtube.com/watch?v=eOpK3hR7SnM" %}

In Qase, it is possible to ensure that the [Test Cases](https://docs.qase.io/general/get-started-with-the-qase-platform/test-cases) being created are first verified by someone superior, be it a QA team manager, supervisor, CTO, or else. In the [Project Settings](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-project), you can define several options regarding Test Case Review:

<figure><img src="https://downloads.intercomcdn.com/i/o/609559905/86d52d438bc3802945719c4f/image.png" alt=""><figcaption></figcaption></figure>

* _Review enabled:_ If selected, you and your teammates will have the option to send a test case to review.
* _Review is mandatory:_ If selected, any changes submitted for a test case cannot be updated unless it’s sent to review.
* _Self Merge:_ This option permits the initiator of the review to merge the changes requested in the review.
* _Approvals required:_ In order to merge the changes, the number of approvals (determined by the Administrator/Owner) will have to be met.

Let's go about creating a new Test Case and submitting it for Review:

* Just like with a regular flow of creating Test Cases, navigate to the Repository, and create a new Case:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595240857/054db9e52a2145f32bfe651c/zbf9Z4dGst0oRK-kPfwG836WU-R9sMnc7BKZ2KAJcB8Q1VLv229GtAUAeoI1x5rlZzsmvh3GbMbvc6JgHIZYqiK3HJoLFTk_-ZaG7OR6f_aOLSCEIz74DFa-3vuDKGS_VAsbBSZucHAdxJNlvoh3DYZ2-Cp2DGbct7pnUlNRw5kwxBY_8hVR3NukeQ" alt=""><figcaption></figcaption></figure>

* Fill in all the necessary details, define steps, etc. Once ready, hit the "Send to Review" button at the bottom of the screen:

<figure><img src="../../../.gitbook/assets/send to review1.png" alt=""><figcaption></figcaption></figure>

\
In a scenario where a Review is set to "Mandatory", there will be no option to "Save" or "Save and create another" - only send your Test Case to review

\


<figure><img src="../../../.gitbook/assets/review .png" alt=""><figcaption></figcaption></figure>

* Once a Test Case has been sent to review, you will now find a new Case Review Request under the "Review" section:\


<figure><img src="../../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>



* If you’re creating a new case and have sent the case to review, you will see the Type as “New case”. However, if you’re making changes to an existing test case and send it to review, the type will reflect “Update”

<figure><img src="../../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

* From the "Review" section, you can go into every particular review there is. In a review, you will find a change log of a Test Case and comments that have been left regarding this review:\


<figure><img src="../../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

* For an author and a reviewer, available actions will be different - a reviewer will also be able to "Approve" or "Request changes"
* Both a review author and other reviewers can leave comments and see others' comments left before.

Once a review is approved (again, depending on the pre-defined requirements in Project Settings), a Review can be merged. After that, a new Test Case will appear in the repository, or the reviewed updates will be set for an existing Test Case:

Step 1: Before review



<figure><img src="../../../.gitbook/assets/review-1.gif" alt=""><figcaption></figcaption></figure>

Step 2: Merging review

<figure><img src="../../../.gitbook/assets/review-2.gif" alt=""><figcaption></figcaption></figure>

_For Reviewers:_

If you are a reviewer and not the author who sent the Test Case to Review. You will be able to see five options on the right-hand side of the page, which are - Merge, Approve, Request Changes, Edit, and Decline.

When you click on _Merge_, the suggested changes are accepted and updated to the test case. _Approve_ allows you to cast your vote for the change while other reviewers still have the chance to look at the suggested updates.

_Request Changes_ allows you to update your status for the review as someone who has requested changes. This feature is a visual indicator to the other reviewers that you’ve requested for changes.

_Edit_ allows you to suggest further changes to the review.

_Decline_ allows you to decline the review request.

\


<figure><img src="../../../.gitbook/assets/Screenshot 2024-05-15 at 10.02.20 AM.png" alt=""><figcaption></figcaption></figure>

_For Authors:_

If you’re the person who created the review, you will be able to Merge the review yourself if the following two conditions are met:

1. If the option to self-merge is enabled in the settings
2. If the required approvals number is not set

Here’s what the page would look like for the author if the conditions stated above are met. You will have three options available to you: Merge, Edit, and Decline.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-05-15 at 10.03.09 AM.png" alt=""><figcaption></figcaption></figure>

Here’s what the page would look like if the conditions stated above were not met. You will have the option to Edit and Decline the review.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-05-15 at 10.04.05 AM.png" alt=""><figcaption></figcaption></figure>

**Note:** If you are the author and the self-review option is enabled in the settings, you will still be able to merge the review even if the required approvals are two or more. You will supersede the settings as you are, in fact, the author, and since the Self-review option is enabled.
