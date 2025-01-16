---
description: >-
  Jira is a proprietary issue-tracking product developed by Atlassian that
  allows bug tracking and agile project management.
---

# Jira Server/Datacenter Plugin installation

Qase offers a robust integration with Jira, enabling you to link [test cases](../../general/get-started-with-the-qase-platform/test-cases/), [test runs](../../general/get-started-with-the-qase-platform/create-a-test-run/), and [defects](../../general/issues/defects.md) to Jira issues both, from Qase, and from Jira.

The statuses of a Qase defect and its linked Jira issue are [synchronized](jira-server-datacenter-plugin-installation.md#h_6f0f4a388d). When a Jira issue is set to a completed status, the corresponding Qase defect is marked as resolved, and vice versa.



## Installation <a href="#h_60484613bd" id="h_60484613bd"></a>

***

{% hint style="info" %}
​If you are using **Jira Data Center, you can install the app from Jira Marketplace** instead of using the package provided in this article.

Once you do so, proceed directly, to the **step 6** of this instruction.
{% endhint %}

1. Download the plugin package attached at the end of the article.

<figure><img src="../../.gitbook/assets/49822.png" alt="" width="563"><figcaption></figcaption></figure>

2.  Go to "Manage apps" page in Jira:

    \


    <figure><img src="../../.gitbook/assets/91892.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/65571 (1).png" alt="" width="563"><figcaption></figcaption></figure>

3.  Select the plugin package you've downloaded, and click "Upload".\


    <figure><img src="../../.gitbook/assets/67417.png" alt="" width="375"><figcaption></figcaption></figure>
4. Select the plugin package you've downloaded, and click "Upload".
5.  After installation, click the "Configure" button and link Jira with Qase:\


    <figure><img src="../../.gitbook/assets/96847.png" alt="" width="563"><figcaption></figcaption></figure>

6\. You will be re-directed to Qase, click "Authorize" on the this step.

That's it, you're ready to go!



## Mapping Statuses Between Qase and Jira <a href="#h_6f0f4a388d" id="h_6f0f4a388d"></a>

***

Qase Defects have the following statuses: **Open**, **In-progress**, **Resolved**, **Invalid**

<figure><img src="../../.gitbook/assets/19125.png" alt=""><figcaption></figcaption></figure>

To map the statuses, click on the app card, and then, choose "Settings" from the (--) menu.

You might have several _projects ¹_ in your Jira instance, each with different and potentially unique statuses for each _issue type ²_

\
Select the Project, Issue Type and click on "Add transition" and select the Defect Mapping and Save the changes:

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1).png" alt="" width="240"><figcaption></figcaption></figure>

You have an option to "Do nothing" in terms of status update of a Qase defect, once the associated Jira issue gets transitioned into a specific status - then, the Qase defect will remain in the status it was.



## Link from Qase

***

### 1. Link Jira issues to Qase Test cases <a href="#h_07d6df02f1" id="h_07d6df02f1"></a>

\
In your repository, click any test case to open its preview and switch to the Properties tab.

Scroll down to the "Link with Apps" section, and choose Jira Server. Then, proceed to search and link your issues.

Linked issues can be removed with the ( x ) icon.

<figure><img src="../../.gitbook/assets/link+jira.gif" alt="" width="563"><figcaption></figcaption></figure>

`Unlink a test case.`

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1).png" alt="" width="375"><figcaption></figcaption></figure>



### 2. Link Jira issues to a Qase Test run: <a href="#h_b193d1c8cf" id="h_b193d1c8cf"></a>

\
Test runs can be linked to a Jira issue, from the Run Dashboard.

Under the "External Issues" section, click 'Select an Integration' to proceed. Only one Jira issue can be linked to the Test run.

<figure><img src="../../.gitbook/assets/link-run (1).gif" alt="" width="563"><figcaption></figcaption></figure>

The option to link Jira issue can be found in the Test run Dashboard, under External Issues.



### 3. Link Jira issues to a Qase defect: <a href="#h_e99a946d85" id="h_e99a946d85"></a>

#### a) From Test runs

If you encounter a defect during a test run, you can either create a new Jira issue directly from Qase or link an existing Jira issue.

1. In the test run, mark your case as Failed, Blocked, or Invalid and proceed with creating a Defect.
2. In the Defect creation form, under “Choose Integrations” select "Jira Server" and click "Add defect"

`creating a new Jira issue from a Qase Test run`

<figure><img src="../../.gitbook/assets/JIRA1 (1) (1).gif" alt="" width="563"><figcaption></figcaption></figure>

`Linking an existing Jira issue from a Qase Test run`

<figure><img src="../../.gitbook/assets/JIRA2 (1).gif" alt="" width="563"><figcaption></figcaption></figure>

#### b) From Defects

If you’re creating a defect that isn’t linked to any result from the defects section, you can link a Jira issue from the defect dashboard using the “Link with apps” section.​

`Linking a Qase defect to a Jira issue`

<figure><img src="../../.gitbook/assets/JIRA3 (1).gif" alt="" width="563"><figcaption></figcaption></figure>

Once linked, the defect will be visible under the External column in the Defects section of your project.

<figure><img src="../../.gitbook/assets/72322.png" alt="" width="563"><figcaption></figcaption></figure>

​And, also in the defect dashboard here -

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

Once a Defect has been created and if you update the status of the Defect, you'll notice that you have the option to select the status for the associated Jira issue to be transitioned into:

<figure><img src="../../.gitbook/assets/35096.png" alt="" width="375"><figcaption></figcaption></figure>

## Link from Jira <a href="#h_dabaf2ad50" id="h_dabaf2ad50"></a>

***

### 1. Test cases <a href="#h_03cf3d75ca" id="h_03cf3d75ca"></a>

* Click "Link a case"
* Insert test case title or its Case ID into the field and click "Link"

<figure><img src="../../.gitbook/assets/mVkWrufPgKeHPfBCE9AOz_a-eH0xRnFLMERzwcEWsBOQFmUGBH8rutRNgBQo-54vgfghvWPJD2BaNXlbgl8AAFxKjHOsoEZ2_aZgxed3reQ2L9DTSF7CsQIE5AAXD9SH86W-FgAK4TuOIa-5-y14P9d2qpj0jM-STlLPB49PLitAk6NhimBRxubz.GIF" alt="" width="563"><figcaption></figcaption></figure>

* To unlink a case, click the "Trash Bin" icon in the sidebar next to the test case you want to unlink (an icon will appear when you hover over the linked case):

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

### 2. Test runs <a href="#h_a0c5567764" id="h_a0c5567764"></a>

* Switch on "Qase: Runs" module through the options:

<figure><img src="../../.gitbook/assets/95611.png" alt="" width="563"><figcaption></figcaption></figure>

* In the module that appeared, click "Link a run":

<figure><img src="../../.gitbook/assets/99847.png" alt="" width="563"><figcaption></figcaption></figure>

* Use the search box to find the needed run by title, and click Link to attach it to the issue:

<figure><img src="../../.gitbook/assets/image (5) (1) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

* Linked run and the statuses of cases in it are now shown in the issue:

<figure><img src="../../.gitbook/assets/image (6) (1) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

_Note:_ `a Jira issue can have multiple runs attached to it`

<figure><img src="../../.gitbook/assets/4469.png" alt="" width="563"><figcaption></figcaption></figure>

Any runs you have linked to Jira issues while setting up a run in Qase will also be shown in the "Qase: Runs" module.



{% file src="../../.gitbook/assets/qase.jira.cloud-1.0.9.obr" %}
