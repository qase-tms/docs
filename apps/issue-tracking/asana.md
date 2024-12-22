# Asana

### What is Asana?

[Asana](https://asana.com/) is a web and mobile work management platform designed to help teams organize, track, and manage their work.

{% embed url="https://youtu.be/0m_xXVTR9A0" %}

### Why use Asana integration?

With the Asana app, you can:

* Link Qase [test case](../../general/get-started-with-the-qase-platform/test-cases/), [test run](../../general/get-started-with-the-qase-platform/create-a-test-run/), or [defects](../../general/issues/defects.md) to Asana tasks.
* Create a new Asana task or connect an existing Asana task when you file a [defect during a test run](../../general/issues/defects.md#h_357b732096) in Qase
* Sync status of a Qase Defect to a connect Asana task (i.e., as soon as you mark the defect as “Resolved” in a connected defect, the Asana Defect will be marked “Completed”).

### How to install Asana? <a href="#h_9b21192970" id="h_9b21192970"></a>

1. &#x20;Click "Apps" in your Qase workspace
2. Click Asana card, then hit "Install now":

<figure><img src="../../.gitbook/assets/41414.png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/80566.png" alt="" width="563"><figcaption></figcaption></figure>

3\. Log into Asana, if you are currently not:

<figure><img src="../../.gitbook/assets/64666.png" alt="" width="329"><figcaption></figcaption></figure>

4\. Click "Allow" to grant access to Asana for the Qase app:

<figure><img src="../../.gitbook/assets/4548.png" alt="" width="375"><figcaption></figcaption></figure>

5\. After the redirect, hit "Authorize" to finalize the installation:

<figure><img src="../../.gitbook/assets/6304.png" alt="" width="375"><figcaption></figcaption></figure>

6\. The app is now successfully installed:

<figure><img src="../../.gitbook/assets/11081.png" alt="" width="563"><figcaption></figcaption></figure>



## Usage: <a href="#h_9bb1df5c9c" id="h_9bb1df5c9c"></a>

***

First, copy your task link from Asana -

<figure><img src="../../.gitbook/assets/69602.png" alt="" width="563"><figcaption></figcaption></figure>

### 1. Linking a Qase test case: <a href="#h_fececdebad" id="h_fececdebad"></a>

* In the repository, select a test case and in the right sidebar, switch to Properties
* Scroll down to the "Link with Apps" dropdown and select "Asana"
* Paste your Asana task link into the field then hit "Link"
* The linked Asana tasks will appear below the "Link With Apps" field
* To unlink the Asana task, click "x" next to the task's title

<figure><img src="../../.gitbook/assets/Asana1.gif" alt="" width="563"><figcaption></figcaption></figure>

### 2. Linking a Qase test run: <a href="#h_165516d6fe" id="h_165516d6fe"></a>

* Navigate to the Test run you want to link to Asana
* Click on "Select an Integration"
* In the Integration dropdown, select Asana
* Insert the Asana task link into the field and click "Link"
* The linked Asana tasks will appear below "External Issues"
* To unlink the Asana task, click on the Trash icon next to it and it will be unlinked:

<figure><img src="../../.gitbook/assets/Asana2 (1).gif" alt="" width="563"><figcaption></figcaption></figure>

### 3. Linking a Qase defect <a href="#h_ed78ffead6" id="h_ed78ffead6"></a>

* Go to the Qase defect you want to link to Asana
* In the right sidebar, find the "Link with Apps" dropdown and select "Asana"
* Paste your Asana task link into the field then hit "Link"
* The linked Asana tasks will appear below the "Link With Apps" field and will also be visible from the main Defects view.
* To unlink the Asana task, click "x" next to the task's title

<figure><img src="../../.gitbook/assets/download (9).gif" alt="" width="563"><figcaption></figcaption></figure>

### 4. Create an Asana task from a Qase Test run: <a href="#h_78d1803698" id="h_78d1803698"></a>

* Inside the test run wizard, marking your test steps or test case as "Failed" or "Blocked" (or "Invalid" for test cases) will provide you with the option to "Create/Attach Defect".

<figure><img src="../../.gitbook/assets/15434.png" alt="" width="563"><figcaption></figcaption></figure>

* In the Defect creation form, the “Choose Integration” is available when you "Use existing" or "Create new Defect. You can select "Asana" and click on "Add defect":
* Fill in the details including the Asana Workspace, Team (if any) and Project, then hit "Create":

<figure><img src="../../.gitbook/assets/Untitled design (4).gif" alt="" width="563"><figcaption></figcaption></figure>

* Or you can select "Link" from the top tab and paste your existing Asana task link and click "Link".
* In the Qase Defect, you will now have connected a new or existing Asana issue link.

<figure><img src="../../.gitbook/assets/download (11).gif" alt="" width="563"><figcaption></figcaption></figure>
