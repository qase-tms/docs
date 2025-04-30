# GitLab

### What is GitLab?

[GitLab](https://about.gitlab.com/) is a web-based DevOps lifecycle tool that provides a Git repository manager providing wiki, issue-tracking, and CI/CD pipeline features.

{% embed url="https://youtu.be/zfjep6wM_Vw" %}

With **Qase’s GitLab integration**, you can:

* Link Qase [test cases](../../general/get-started-with-the-qase-platform/test-cases/), [test runs](../../general/get-started-with-the-qase-platform/create-a-test-run/), and [defects](../../general/issues/defects.md) to GitLab issues.
* Create a new issue in GitLab when you file a defect [during a test run in Qase](../../general/issues/defects.md#h_357b732096) and their statuses are automatically synchronized, in both directions. \[Qase <> GitLab].
* [Execute automated runs](../ci-cd/gitlab.md) in GitLab from a Qase.

## Installation <a href="#h_ff8e665948" id="h_ff8e665948"></a>

For installation, you will require `GitLab URL` and the `Access token`.

1. First, sign-in to your GitLab account and navigate to the `Preferences` from the profile menu:

<figure><img src="../../.gitbook/assets/image (73).png" alt="" width="563"><figcaption></figcaption></figure>

2. Go to the `Access tokens` page:

<figure><img src="../../.gitbook/assets/image (74).png" alt="" width="563"><figcaption></figcaption></figure>

3. To create a new `Personal Access Token`, select the scope `api` and click on the _Create Personal Access token_:

<figure><img src="../../.gitbook/assets/image (75).png" alt="" width="563"><figcaption></figcaption></figure>

4. Copy your token to clipboard.
5. On Qase, navigate to the [Apps](https://app.qase.io/apps) section, find the GitLab app and click `Install now`.

Here, provide the Access token from the previous step, and URL of your GitLab instance (_the field is pre-populated with the default value)_

<figure><img src="../../.gitbook/assets/image (76).png" alt=""><figcaption></figcaption></figure>

6. Click the `Install` button. After a few seconds, you will be redirected to the `Apps` page with a confirmation message as shown below.

<figure><img src="../../.gitbook/assets/image (77).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
_Please note, a `Maintainer` role is required if you choose to use a `Group token`_&#x20;
{% endhint %}



## Usage <a href="#h_c5cfb8f18a" id="h_c5cfb8f18a"></a>

***

### Linking your Qase Test cases <a href="#h_fe7ca549cb" id="h_fe7ca549cb"></a>

In your repository, click any test case to open its preview and switch to the Properties tab.

Scroll down to the "Link with Apps" section, and choose the GitLab app. Then, proceed to search and link your issues.

Linked issues can be removed with the ( x ) icon.

<figure><img src="../../.gitbook/assets/link gitlab.gif" alt="" width="563"><figcaption></figcaption></figure>

2\. To unlink the GitLab issue, click "x" next to the card title:

<figure><img src="../../.gitbook/assets/image (78).png" alt="" width="563"><figcaption></figcaption></figure>

### Linking your Qase Test runs <a href="#h_2219d0f79e" id="h_2219d0f79e"></a>

Test runs can be linked to a GitLab issue, from the Run Dashboard.

Under the "External Issues" section, click 'Select an Integration' to proceed. Only one GitLab issue can be linked to the Test run.

<figure><img src="../../.gitbook/assets/link lab test runs.gif" alt="" width="563"><figcaption></figcaption></figure>

### Linking your Qase Defects <a href="#h_99f0d9e5c9" id="h_99f0d9e5c9"></a>

Defects can be linked to a GitLab issue, from the Defect Dashboard.

Under the "External Issues" section, select the GitLab app to proceed.

<figure><img src="../../.gitbook/assets/gitlab defect link.gif" alt="" width="563"><figcaption></figcaption></figure>



### Create a GitLab issue from a Qase Test Run <a href="#h_bd0af7de02" id="h_bd0af7de02"></a>

When you assign a negative result to a case during a test run, you will have the option to create or attach a Qase defect.

Additionally, you can select the ‘GitLab’ app from the "Choose Integration" dropdown to either create a new GitLab issue, or link an existing one.

The created or linked issue will be visible in both the defects tab of the test run and the defect section of the project.

<figure><img src="../../.gitbook/assets/gitlab create new.gif" alt="" width="563"><figcaption></figcaption></figure>

* You can view the link to the GitLab issue in
  * Defects tag of the test run

<figure><img src="../../.gitbook/assets/Screenshot 2024-07-02 at 10.42.43.png" alt="" width="563"><figcaption></figcaption></figure>

* From the Qase defect screen

<figure><img src="../../.gitbook/assets/image (79).png" alt="" width="563"><figcaption></figcaption></figure>
