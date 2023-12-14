---
description: >-
  Jira is a proprietary issue-tracking product developed by Atlassian that
  allows bug tracking and agile project management.
---

# Jira Server/Datacenter Plugin installation

### Jira Server/DC plugin?

With Jira Server/DC plugin for Qase, you can install the integration and get access to these possibilities:

* link issues from your Jira with [test cases](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run) in Qase
* link [test runs](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run-1) in Qase to issues in Jira
* create new issues in Jira simultaneously with creating a [defect](https://docs.qase.io/general/get-started-with-the-qase-platform/defects) in Qase during a test run, passing all defect details and information, and synchronizing the statuses of issues and defects between the systems.

### How to install Jira plugin

Here's how to install the plugin:

1. Download the plugin package found at the end of the article\
   **​NB:** if you are using Jira DC, you can install the app from Jira Marketplace instead of using the package provided in this article. Once you do so, proceed to step 6 of this instruction.
2. Go to the "Manage apps" page in Jira:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597261241/087200c11e51831d86465907/twOGof3Xd9dXVASBVwpXaTKdbcuYvBdUQCkcpNpmEVzKssSbleCn-rads7EU5qva-TsXPWKma3_cHledauq8V00HqhEo6W3zNLtokMZ00MZOm3srYHc0V-y_xNt4kz3Oi7oSjzW7N4kYy53V0k9reOqi0Aj4y6QgxYZbrDdwhA-cME7jS0biYudocQ" alt=""><figcaption></figcaption></figure>

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597261246/77ad2e26efde877351707f62/J4ynasH5skW3uT9q8M2xum2dGer-D6hrLeENRkV9YHlXf-hsKvEveFjcYNeq_YbqflXcU4m0dpDcZDBrZL4DBuKK4KQ5m8YnU-Cn35sXhmkuNbYDA_8Z6oG5RB6gB1UCpPjZIR34-nJUePCfX2ZR_5R4s_TLGgcY3FXy2CIII0uEDvirDQXBaPJjMA" alt=""><figcaption></figcaption></figure>

* Click "Upload app"
* Select the plugin package you've downloaded:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597261251/2537613cfae9663730d08dfe/vwoRJHuJifSIGkyJ90LSc9vGsvNPhs-4FRkeut5RBB3XONWC3-sm5FwZS_gamz-GLP2sOIzVDk1xEVtvs5BX1IwkpKfko61HbdvnG1oU1NxDov_paXfanWCiXzSSGcEAvOy62mJV_slmZgY_OFalz5ePSb6C0aGuHcfLwdPFi97kNkIg2IqnW0ik3g" alt=""><figcaption></figcaption></figure>

* Click "Upload"
* After installation, click the "Configure" button and link Jira with Qase:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597261254/26d88f96b2ed11034edf4bb9/sdYq3Bnw8Aa6tPTHWxTK7Ez-XhnfDwypvTbFH24EzlD0FPt31a3ku08uM_xgE1DiJZ3lidOV5pW2749CphSwZLiadASsLbAtTfL5ONTj-TFsVzxrMS9-8gb6b7JjUJ0kwHXONlS_Jwa2WcD2aoUBfqFi66S3qo4Ujx5DR95qv_Qckz-AUbMG2dde_A" alt=""><figcaption></figcaption></figure>

That's it, you're ready to go!

* Once the app has been installed, you can now map the Jira status and Qase Defects. To do so, click on the 3 dots icon and click "Settings":

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-14 at 11.23.18 AM.png" alt=""><figcaption></figcaption></figure>

* Select the Project, Issue Type and click on "Add transition" and select the Defect Mapping and Save the changes:

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-14 at 11.33.54 AM.png" alt=""><figcaption></figcaption></figure>

You have an option to "Do nothing" in terms of status update of a Qase defect, once the associated Jira issue gets transitioned into a specific status - then, the Qase defect will remain in the status it was.

## Usage <a href="#h_303ea547de" id="h_303ea547de"></a>

### Linking from Qase to Jira: <a href="#h_fcf8cae57d" id="h_fcf8cae57d"></a>

1\. To link a Jira issue to a Qase test case from Qase:

* Select a case in the repository and switch to Properties in the sidebar
* Click "Link Jira Cloud issues"
* Insert Jira issue title or ID into the field and hit "Link"
* Now the Jira issue is linked:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597257744/5f9461576d625a3073fed723/qe_wLZL98RiUJr7BSHZw5_gc_59ppQi2QwOh-HWnWfTiII9XJdiYxVKCtKeZ5wtq2J44FSMXW_2Tve7uaigjENPLs2xzjRiFlUamsu52h3aveXDnlFqqzU-1eb1z39X2ryc-jwXH-h2MmaeG9ePGWIclbtYXtxhTEk20K7WIoMXsJwxRv8kFGJ4N" alt=""><figcaption></figcaption></figure>

* To unlink the Jira issue, click "x" next to the card title:

[![](https://qase.intercom-attachments-7.com/i/o/597257758/33affc49f0805d94818b09cc/a26pNkYDFYQjY\_Icz\_w49zU63ZUxeD4uyoOJE8TCDvFLDaPCcDh5PNz6jfq5180knW-DwtjijBWBFufGAiJV1aXX4rTdR6spEbV6Kk1M4e6Si8LnybnYv7uyRx7wGbV3zAeAHtyjUWVsDp9xFDRfY6Yd\_fsakykAgCYpZKQQWVrLmRu7oGBYnT-q)](https://qase.intercom-attachments-7.com/i/o/597257758/33affc49f0805d94818b09cc/a26pNkYDFYQjY\_Icz\_w49zU63ZUxeD4uyoOJE8TCDvFLDaPCcDh5PNz6jfq5180knW-DwtjijBWBFufGAiJV1aXX4rTdR6spEbV6Kk1M4e6Si8LnybnYv7uyRx7wGbV3zAeAHtyjUWVsDp9xFDRfY6Yd\_fsakykAgCYpZKQQWVrLmRu7oGBYnT-q)

2\. Link Qase Test Runs to Jira issues: There are two ways to create a Test Run - Express Run (from the repository) and New Test Run (from the Test Runs page).

Here’s how you can link a Jira issue to a Test Run:

* Navigate to the Test run you want to link to Jira Server
* Click on "Select an Integration" and choose "Jira Server" in the Integration pop-up that appears.

<figure><img src="https://downloads.intercomcdn.com/i/o/646931641/68155ca9e4286226142bbb51/image.png" alt=""><figcaption></figcaption></figure>

* In the “Link Jira Server issues” pop-up, enter the title of the issue or the id of the issue and then click on “Link”:

<figure><img src="https://downloads.intercomcdn.com/i/o/646932122/7971dfbd205475b23f5a083e/image+(23).png" alt=""><figcaption></figcaption></figure>

* Now the Jira Server issue is linked:

<figure><img src="https://downloads.intercomcdn.com/i/o/646935339/ecdf1651562e2d6bebf4f258/image.png" alt=""><figcaption></figcaption></figure>

*   To unlink the Jira Server issue, click on the trash bin icon for the particular run and it will be unlinked:



    <figure><img src="https://downloads.intercomcdn.com/i/o/646935999/d89f196ad47fb8c3ea0ba33c/image.png" alt=""><figcaption></figcaption></figure>

### Linking from Jira to Qase: <a href="#h_8987a8d07f" id="h_8987a8d07f"></a>

1\. To link a Qase test case to Jira issue from Jira:

* Click "Open Test cases" in Jira sidebar
* Click "Link a case"
* Insert test case title or its Case ID into the field and click "Link"

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597258021/9feaa7d113d81ec9fa30640c/mVkWrufPgKeHPfBCE9AOz_a-eH0xRnFLMERzwcEWsBOQFmUGBH8rutRNgBQo-54vgfghvWPJD2BaNXlbgl8AAFxKjHOsoEZ2_aZgxed3reQ2L9DTSF7CsQIE5AAXD9SH86W-FgAK4TuOIa-5-y14P9d2qpj0jM-STlLPB49PLitAk6NhimBRxubz" alt=""><figcaption></figcaption></figure>

* To unlink a case, click the "Trash Bin" icon in the sidebar next to the test case you want to unlink (an icon will appear when you hover over the linked case):

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597258030/755ee2b501f62b5824c26ce6/mcHdDtT_a3yAmrTnpyRc0Tkg7Wqqsh1ciFH9kQMqv4iutn-ypUxCorDafc9oJNYMuOQ5ucbLlAPHLwt4ixNHX3l2sY4jxhNNOXOCAWWmGJbDl67NzQI97NA7FZlxTsfct1obTs7SIvMhgohRedCSHULlib32hNDbS_8J2ldh9Y22RgLfKdQ64h1B" alt=""><figcaption></figcaption></figure>

2\. To link a Qase test run to a Jira issue:

*   Switch on "Qase: Runs" module through the options:



    <figure><img src="https://downloads.intercomcdn.com/i/o/597254552/502413c599f921b3d21d8224/image.png" alt=""><figcaption></figcaption></figure>
*   In the module that appeared, click "Link a run":



    <figure><img src="https://downloads.intercomcdn.com/i/o/597255084/00c6d3eb55222bb347165e22/image.png" alt=""><figcaption></figcaption></figure>
*   Use the search box to find the needed run by title, and click Link to attach it to the issue:



    <figure><img src="https://downloads.intercomcdn.com/i/o/597255637/243654aa80d426308f3373ec/image.png" alt=""><figcaption></figcaption></figure>
*   Linked run and the statuses of cases in it are now shown in the issue:



    <figure><img src="https://downloads.intercomcdn.com/i/o/597256162/042d75d36c8bba885ed01e22/image.png" alt=""><figcaption></figcaption></figure>
*   _Note:_ a Jira issue can have multiple runs attached to it:\


    <figure><img src="https://downloads.intercomcdn.com/i/o/597256561/6dc56592a1e85d41e6dfe77a/image.png" alt=""><figcaption></figcaption></figure>
* _Note:_ any runs you have linked to Jira issues while setting up a run in Qase will also be shown in the "Qase: Runs" module.

### Create Jira issue while creating a defect in Qase <a href="#h_eed4b4d9bc" id="h_eed4b4d9bc"></a>

* In the test run, mark your case as Failed, Blocked, or Invalid and proceed with creating a Defect.
* in the Defect creation form, under “Choose Integrations” select "Jira Cloud" and click "Add defect"
* Choose the Jira Project to create an issue in, type of an issue, fill out other fields, then hit "Create"

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597258128/e46098d833d4374e4991ddfa/J_cWegCtDSGPC6zbHg28PYUPtNh9aXEBd4F4SuusalHMcj-FYiMezh5pEjJI40a1LYoXumaiM06uwJIrpLq2MrJxjZHZRwjYSDjHo3YJR4n2XCCemp84ti1qm5CN03ZLT7yXiPCnzqGXgiJ42C5x8XaC1J7m1dLGWCxwQdQ-_MkjnwLo62ZfCSAM" alt=""><figcaption></figcaption></figure>

*   In the Qase Defect you will now have a connected Jira issue link:\


    <figure><img src="https://qase.intercom-attachments-7.com/i/o/597258141/13a885066240b99824020841/-y6DpimqxpTICAgDDvX_A7AJkhDMlvZTJgGgzWkFcBXlpa8_2ZXLUieujKiSNbZdFB37TaPi4oXxtAGIGEe2BJTR7L0vZj2jLxwwd4FOqkF8P8nW_11IExy_JHJn2RPcqzIIR775EYYRtqL-a_K0nmof2aQACo3JooY2SnIcD9rot1DRR6QspDJF" alt=""><figcaption><p><br></p></figcaption></figure>



    <figure><img src="https://qase.intercom-attachments-7.com/i/o/597258146/4faca6fed3a048223fa26637/a_nG3a7-0PyjlLW-8cr-N4QXYe6CSpDpIw6lHeQBDnE2BcJqKhc0Vz6Pc5tDx3rYgqWTK6e3S2EDmXE2zV5t_cINqz86fcrA4-FMOl7kLJgtm_E3MX8crB2ssnadFPxn5f-uubEXxZ58hii5fnVKYzDa-GVr4LKcBZXEeQBDupX8FvXZzdZKDEum" alt=""><figcaption></figcaption></figure>



    * Once a Defect has been created and if you update the status of the Defect, you'll notice that you have the option to select the status for the associated Jira issue to be transitioned into:&#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-14 at 11.36.05 AM.png" alt=""><figcaption></figcaption></figure>

{% file src="../../.gitbook/assets/qase.jira.cloud-1.0.3.obr" %}
