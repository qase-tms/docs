# BitBucket

### What is BitBucket?

BitBucket is a Git-based source code repository hosting service owned by Atlassian. BitBucket offers both commercial plans and free accounts with an unlimited number of private repositories.

### Why use BitBucket integration?

Qase integration for BitBucket allows you to start your automated runs directly from Qase, without the need to go to BitBucket to set them up separately.



## How to install BitBucket? <a href="#h_0e2ef7993d" id="h_0e2ef7993d"></a>

1. You need to install the [Qase Bitbucket app](https://marketplace.atlassian.com/apps/1230226/qase-for-bitbucket?hosting=cloud\&tab=overview) from the Atlassian Marketplace.
2. Click the “Get it now” button:

<figure><img src="../../.gitbook/assets/88642.png" alt="" width="563"><figcaption></figcaption></figure>

3. Click the “Add” button:

<figure><img src="../../.gitbook/assets/58395.png" alt="" width="563"><figcaption></figcaption></figure>

4. Click the “Grant Access” button.
5. Refresh the page and click the “Manage” button.
6.  Scroll down the right panel until you see “Qase for Bitbucket”. Click the “Qase integration config…” and after that, click on the “Link with Qase” button:



    <figure><img src="https://qase.intercom-attachments-1.com/i/o/689974457/cb658cad45ab949bae334db8/https-3A-2F-2Fs3-us-west-2.amazonaws.com-2Fsecure.notion-static.com-2Fec65038a-1270-4426-8541-f85f95255106-2FUntitled.png" alt="" width="563"><figcaption></figcaption></figure>
7.  You will be redirected to the Qase page. Click the “Authorize” button:



    <figure><img src="https://qase.intercom-attachments-1.com/i/o/689974477/9a4ff2533984580bf048d6da/https-3A-2F-2Fs3-us-west-2.amazonaws.com-2Fsecure.notion-static.com-2F5c1654b5-4017-4871-850e-2566dc68c89c-2FUntitled.png" alt="" width="563"><figcaption></figcaption></figure>
8. Finally, you will be logged in automatically (or need to log in if you have an outdated session), and that's it.
9. Go to Apps → Continuous Integration and take a look at the BitBucket app to be sure that integration was installed successfully.

<figure><img src="../../.gitbook/assets/97832.png" alt="" width="563"><figcaption></figcaption></figure>



## Usage <a href="#h_838e3035b9" id="h_838e3035b9"></a>

1. Start a new automated test run:

<figure><img src="../../.gitbook/assets/27320.png" alt="" width="563"><figcaption></figcaption></figure>

2. Choose a CI/CD system to use (BitBucket):

<figure><img src="../../.gitbook/assets/91506.png" alt="" width="375"><figcaption></figcaption></figure>

3. Fill in all necessary fields except the “Pipeline field”:

<figure><img src="../../.gitbook/assets/40373.png" alt="" width="375"><figcaption></figcaption></figure>

4. Fill in the “Pipeline” field and click the “Start a run” button.

{% hint style="info" %}
You must manually enter the Pipeline name from your Bitbucket.&#x20;



You only need to do this once. Once added, this Pipeline will appear in the drop-down list and will be remembered in Qase. You can see the names of the Pipelines in your Bitbucket (Please check the instruction below to figure out how to do it)
{% endhint %}

5. You will be redirected to a test run you started. In the test run details section, you will see a link to the workflow run in GitHub and the current status.

<figure><img src="../../.gitbook/assets/27831.png" alt="" width="563"><figcaption></figcaption></figure>

6. When the tests have been executed, the rest run will contain all the results sent by a reporter (it should be properly configured):

<figure><img src="../../.gitbook/assets/83742.png" alt="" width="563"><figcaption></figcaption></figure>

## How to find the correct pipeline name in Bitbucket? <a href="#h_03ca438a95" id="h_03ca438a95"></a>

1. Open your company Bitbucket.
2. Open the repository.
3. Click on the pipeline's section.
4.  Click on the Run pipeline button:



    <figure><img src="https://qase.intercom-attachments-1.com/i/o/689974581/f18a33aceba87b5fd097f72f/https-3A-2F-2Fs3-us-west-2.amazonaws.com-2Fsecure.notion-static.com-2F896a75bc-cc92-4796-a218-0fe42c2833db-2FUntitled.png" alt="" width="563"><figcaption></figcaption></figure>
5.  In the modal window, choose the branch which you would like to start:



    <figure><img src="https://qase.intercom-attachments-1.com/i/o/689974599/911811d3b56c74534a4caf2f/https-3A-2F-2Fs3-us-west-2.amazonaws.com-2Fsecure.notion-static.com-2Ffd740ee5-3129-4c50-af68-6c82146ba742-2FUntitled.png" alt="" width="563"><figcaption></figcaption></figure>
6. Click on the select box with the name `Pipeline` and you will see a list of pipelines. So, let's assume that I would like to run the first one. In this case, the name of my pipeline is `api_tests`. \
   If I want to start the second one - the name is `default.`
7. After you figure out which pipeline name needs to be used, you need to add it in the last field on the "Create Automatic Run modal" (”Pipeline” field).
