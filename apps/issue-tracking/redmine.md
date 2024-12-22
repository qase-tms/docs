# Redmine

### What is Redmine?

[Redmine](https://www.redmine.org/) is a free and open-source, web-based project management and issue-tracking tool that allows users to manage multiple projects and associated sub-projects.

{% embed url="https://youtu.be/TLqam6Jk7bQ" %}

### Why use Redmine integration?

With the Redmine app, you can:

* Link Qase [test cases](../../general/get-started-with-the-qase-platform/test-cases/), [test runs](../../general/get-started-with-the-qase-platform/create-a-test-run/), and [defects](../../general/issues/defects.md) to Redmine issues.
* Create a new issue in Redmine when you file a defect [during a test run in Qase](../../general/issues/defects.md#h_357b732096)

### How to install Redmine? <a href="#h_3f1fa783ac" id="h_3f1fa783ac"></a>

1. From the "Apps" section of your workspace, find the Redmine App card, and click "Install now.

<figure><img src="../../.gitbook/assets/95470.png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/41731.png" alt="" width="563"><figcaption></figcaption></figure>

2. Sign in to Redmine and obtain your `Redmine URL` and `Authorization Token` then click “Install".

<figure><img src="../../.gitbook/assets/21113.png" alt="" width="375"><figcaption></figcaption></figure>

* You can generate an `API Token` from the "My account" page

<figure><img src="../../.gitbook/assets/60942.png" alt="" width="452"><figcaption></figcaption></figure>

* Additionally, make sure that REST API service is enabled:\
  ​ `Settings > API > Enable REST web service`

<figure><img src="../../.gitbook/assets/58735.png" alt="" width="563"><figcaption></figcaption></figure>

3. The app is now successfully installed:

<figure><img src="../../.gitbook/assets/50342.png" alt="" width="563"><figcaption></figcaption></figure>



## Usage <a href="#h_d40a094de3" id="h_d40a094de3"></a>

***

### Link your Qase Test Cases <a href="#h_91e4233359" id="h_91e4233359"></a>

In your repository, click any test case to open its preview and switch to the Properties tab.

Scroll down to the "Link with Apps" section, and choose Redmine. Then, proceed to search and link your issues.

Linked issues can be removed with the ( x ) icon.

<figure><img src="../../.gitbook/assets/Kapture 2024-09-22 at 12.31.32.gif" alt="" width="563"><figcaption></figcaption></figure>

### Link your Qase Test runs <a href="#h_0d6f979028" id="h_0d6f979028"></a>

Test runs can be linked to a Redmine issue, from the Run Dashboard.

Under the "External Issues" section, click 'Select an Integration' to proceed. Only one Redmine issue can be linked to the Test run.

<figure><img src="../../.gitbook/assets/Kapture 2024-09-22 at 12.33.01.gif" alt="" width="563"><figcaption></figcaption></figure>

### Link your Qase Defects <a href="#h_a936b3ae97" id="h_a936b3ae97"></a>

Defects can be linked to a Redmine issue, from the Defect Dashboard. Under the "External Issues" section, select the Redmine app to proceed.

<figure><img src="../../.gitbook/assets/Kapture 2024-09-22 at 12.33.56.gif" alt="" width="563"><figcaption></figcaption></figure>



### Create a new Redmine issue from a Qase Test run <a href="#h_25dabcf978" id="h_25dabcf978"></a>

When you assign a negative result to a case during a test run, you will have the option to create or attach a Qase defect.

Additionally, you can select the ‘Redmine’ option from the "Choose Integration" dropdown to either create or link a Redmine issue.

The created or linked issue will be visible in both the defects tab of the test run and the defect section of the project.

<figure><img src="../../.gitbook/assets/Kapture 2024-09-22 at 12.43.34.gif" alt="" width="563"><figcaption></figcaption></figure>













