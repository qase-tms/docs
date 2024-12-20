# Azure DevOps

What is Azure DevOps?

[Azure DevOps](https://azure.microsoft.com/en-us/products/devops/) or ADO, is a product that provides version control, reporting, requirements management, project management, automated builds, testing and release management capabilities, developed by Microsoft.

{% embed url="https://www.youtube.com/watch?v=G6Esy0oTN6U" %}

### Why use Azure DevOps integration?

With Azure DevOps app, you can:

* Link Qase test cases to Azure Link Qase [test cases](../../general/get-started-with-the-qase-platform/test-cases/), [test runs](../../general/execution/create-a-test-run.md), and [defects](../../general/get-started-with-the-qase-platform/defects/) to ADO issues. issues.
* Link Qase test runs Create a new issue in ADO when you file a [defect](../../general/get-started-with-the-qase-platform/defects/) during a test run in Qase.
*   The _statuses_ of the Qase defect and connected ADO work item are automatically synced.

    &#x20;\
    (i.e., _as soon as you mark the defect as “Resolved” in a connected defect, the Azure DevOps will be marked “Completed” - and vice versa_).

### How to install Azure DevOps? <a href="#h_2cce8d833b" id="h_2cce8d833b"></a>

1. Go to the 'Apps' section of your workspace and find the "Azure DevOps" app.

<figure><img src="../../.gitbook/assets/image (93).png" alt="" width="563"><figcaption></figcaption></figure>

2. Click the app card, then hit "Install now"

<figure><img src="../../.gitbook/assets/image (1) (2).png" alt="" width="563"><figcaption></figcaption></figure>

3. Log into Azure DevOps, if you are currently not:

<figure><img src="../../.gitbook/assets/image (2) (2).png" alt="" width="563"><figcaption></figcaption></figure>

4. After the redirect, hit "Authorize" to finalize the installation:

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1).png" alt="" width="375"><figcaption></figcaption></figure>

5. The app is now successfully installed

<figure><img src="../../.gitbook/assets/image (4) (2).png" alt="" width="563"><figcaption></figcaption></figure>



## Usage <a href="#h_b68ae0bf25" id="h_b68ae0bf25"></a>

***

### Link your Qase Test Cases <a href="#h_5b636fc068" id="h_5b636fc068"></a>

In your repository, click any test case to open its preview and switch to the Properties tab.

Scroll down to the "Link with Apps" section, and choose Azure DevOps. Then, proceed to search and link your issues.

Linked issues can be removed with the ( x ) icon.

<figure><img src="../../.gitbook/assets/azure link new.gif" alt="" width="563"><figcaption></figcaption></figure>

### Link your Qase Test runs <a href="#h_169122685a" id="h_169122685a"></a>

Test runs can be linked to a Azure DevOps issue, from the Run Dashboard.

Under the "External Issues" section, click 'Select an Integration' to proceed. Only one Azure DevOps issue can be linked to the Test run.

<figure><img src="../../.gitbook/assets/azure run link new.gif" alt="" width="563"><figcaption></figcaption></figure>

### Link your Qase Defects <a href="#h_9e78f71761" id="h_9e78f71761"></a>

Defects can be linked to a Azure DevOps issue, from the Defect Dashboard. Under the "External Issues" section, select the Azure DevOps app to proceed.

<figure><img src="../../.gitbook/assets/azure defect link new.gif" alt="" width="563"><figcaption></figcaption></figure>

### Create a new Azure DevOps issue from a Qase Test run <a href="#h_6ff1f26e7f" id="h_6ff1f26e7f"></a>

When you assign a negative result to a case during a test run, you will have the option to create or attach a Qase defect.

Additionally, you can select the ‘Azure DevOps’ option from the "Choose Integration" dropdown to either create or link a Azure DevOps issue.

The created or linked issue will be visible in both the defects tab of the test run and the defect section of the project.

<figure><img src="../../.gitbook/assets/azure result link new.gif" alt="" width="563"><figcaption></figcaption></figure>
