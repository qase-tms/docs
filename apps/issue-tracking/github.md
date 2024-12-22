# GitHub

### What is GitHub?

[GitHub](https://github.com/) is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

{% embed url="https://www.youtube.com/watch?v=QfQu7uaDIEo" %}

With the GitHub app, you can:

* link an existing issue in GitHub to a Qase [test case](../../general/get-started-with-the-qase-platform/test-cases/), [test run](../../general/get-started-with-the-qase-platform/create-a-test-run/), or [defect](../../general/issues/defects.md).
* create a new issue or connect an existing issue in GitHub when you [file a defect during a test run](../../general/issues/defects.md#h_357b732096) in Qase.
* [connect a GitHub workflow](../ci-cd/github.md#ci-cd-workflows) to Qase and execute automated runs in GitHub from a Qase test run.

## Installation <a href="#h_638b057e77" id="h_638b057e77"></a>

***

<details>

<summary>Go to the 'Apps' section of your workspace:</summary>

[![](https://qase.intercom-attachments-7.com/i/o/597262858/6345d95eecf41310e09a89ff/lqgVeB1yc_MKiXnQqLagQpFsW9u3hnirPVlcw4vZrjBqx38lYIGVO8RicQgSEePUPN81FjSJy_Qa9hr7oaBdmz8i1mrkA6BBLsh4Lp2Fj0I4sKUuBlm9MkaKN8EBjg_kBRoKmhceZrzsukuIs674Y9Oyr1jWdRbDVIs5hCczTLi-LzhMvNME0dfZGA)](https://qase.intercom-attachments-7.com/i/o/597262858/6345d95eecf41310e09a89ff/lqgVeB1yc_MKiXnQqLagQpFsW9u3hnirPVlcw4vZrjBqx38lYIGVO8RicQgSEePUPN81FjSJy_Qa9hr7oaBdmz8i1mrkA6BBLsh4Lp2Fj0I4sKUuBlm9MkaKN8EBjg_kBRoKmhceZrzsukuIs674Y9Oyr1jWdRbDVIs5hCczTLi-LzhMvNME0dfZGA)

</details>

To install the app, follow these steps:

1. Click the GitHub card, and hit "Install now"
2. Log in to GitHub, if you're not already.
3. Select the GitHub Repositories where you want to install the app, then hit "Install"
4. After the redirect, hit "Authorize" to complete the installation.
5. The app is now installed successfully.

{% hint style="info" %}
**Step 4** is important because it authorizes GitHub to access your Qase workspace.
{% endhint %}

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597262963/9b1ce15067dd9bbe2dd944b5/fK0dSgk8x9jmI34J847RbL1CmbB2eZa0XI3VGOBQfzLgch1_WI5FVMYU0WbwFArW9Ay-rh1eF26wNnS73NUzUBV8MR4zh9Uv8oBX9uawXe9sPnBqpQ_VXXKbsecmlRQcoBaR9yIAVUXg8F0wpArxnGmiPU_vUbt4tthNdhTMPHwnaeXi6UmwkbHWpw" alt="" width="563"><figcaption></figcaption></figure>

## Usage <a href="#h_7b2567480e" id="h_7b2567480e"></a>

***

### 1. Issue-tracking <a href="#h_db20e6b636" id="h_db20e6b636"></a>

### 1. Creating a new GitHub issue from Qase <a href="#h_522cfed7ca" id="h_522cfed7ca"></a>

If you encounter a defect during a test run, you can either create a new Github issue directly from Qase or link an existing Github issue.

* In the test run, mark your test case as Failed, Blocked, or Invalid and proceed with creating a Defect
* In the Defect creation form, under “Choose Integrations”, select "GitHub App" and click "Add defect"
* Choose the GitHub repository to create an issue in, then hit "Create"

<figure><img src="../../.gitbook/assets/create github issue.gif" alt="" width="563"><figcaption></figcaption></figure>

* Or select the Link tab at the top and select your repository search for the issue and click on "Link".

<figure><img src="../../.gitbook/assets/Github1.gif" alt="" width="563"><figcaption></figcaption></figure>

* In the Qase Defect, you will now have a connected GitHub issue link
* The statuses of the Qase Defect and the connected GitHub issue synced, meaning marking one as closed resolves the other (and vice versa).



### 2. Linking existing issues <a href="#h_84c4c654ff" id="h_84c4c654ff"></a>

In addition to creating new GitHub issues, you can also link test cases, runs, and defects to a GitHub issue -

#### a. Linking Test cases <a href="#h_1054e57c92" id="h_1054e57c92"></a>

1. In the repository, click on the test case you want to link the GitHub issue to.
2. Switch to the properties tab in the preview window.
3. Scroll down and click on "Link GitHub app issue"
4. In the modal window, select your repository, search for the issue, and click "Link".

<figure><img src="../../.gitbook/assets/Github2.gif" alt="" width="563"><figcaption></figcaption></figure>

#### b. Linking Test runs <a href="#h_5331cf6d03" id="h_5331cf6d03"></a>

1. In the Test runs view, click on the run you want to link the GitHub issue to.
2. In the Run dashboard, to the bottom right, find the button 'Select an integration' under External issue.
3. In the modal window, select your repository, search for the issue, and click "Link".

<figure><img src="../../.gitbook/assets/Github3.gif" alt="" width="563"><figcaption></figcaption></figure>

#### c. Linking defects <a href="#h_06564c952b" id="h_06564c952b"></a>

1. In the Defects section, click on a defect you want to link the GitHub issue to.
2. Inside the Defect view, find the "Link with Apps" dropdown on the bottom right and select "GitHub App".
3. In the modal window, select your repository, search for the issue, and click "Link".

<figure><img src="../../.gitbook/assets/Github4.gif" alt="" width="563"><figcaption></figcaption></figure>
