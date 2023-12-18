# GitHub

### What is GitHub?

[GitHub](https://github.com/) is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

{% embed url="https://youtu.be/rhzWY0oh2AI" %}

With the GitHub app, you can:

* create a new issue in GitHub when you file a [defect](https://help.qase.io/en/articles/5563710-defects) during a [test run](https://help.qase.io/en/articles/5563702-test-runs) in Qase.
* connect a GitHub workflow to Qase.
* execute automated runs in GitHub from a Qase test run.

## Installation <a href="#h_638b057e77" id="h_638b057e77"></a>

***

<details>

<summary>Go to the 'Apps' section of your workspace:</summary>

[![](https://qase.intercom-attachments-7.com/i/o/597262858/6345d95eecf41310e09a89ff/lqgVeB1yc\_MKiXnQqLagQpFsW9u3hnirPVlcw4vZrjBqx38lYIGVO8RicQgSEePUPN81FjSJy\_Qa9hr7oaBdmz8i1mrkA6BBLsh4Lp2Fj0I4sKUuBlm9MkaKN8EBjg\_kBRoKmhceZrzsukuIs674Y9Oyr1jWdRbDVIs5hCczTLi-LzhMvNME0dfZGA)](https://qase.intercom-attachments-7.com/i/o/597262858/6345d95eecf41310e09a89ff/lqgVeB1yc\_MKiXnQqLagQpFsW9u3hnirPVlcw4vZrjBqx38lYIGVO8RicQgSEePUPN81FjSJy\_Qa9hr7oaBdmz8i1mrkA6BBLsh4Lp2Fj0I4sKUuBlm9MkaKN8EBjg\_kBRoKmhceZrzsukuIs674Y9Oyr1jWdRbDVIs5hCczTLi-LzhMvNME0dfZGA)

</details>

To install the app, follow these steps:

1. Click the GitHub card, and hit "Install now"
2. Log in to GitHub, if you're not already.
3. Select the GitHub Repositories where you want to install the app, then hit "Install"
4. After the redirect, hit "Authorize" to complete the installation.
5. The app is now installed successfully.

<mark style="background-color:purple;">**Step 4**</mark> <mark style="background-color:purple;"></mark><mark style="background-color:purple;">is important because it authorizes GitHub to access your Qase workspace.</mark>\


<figure><img src="https://qase.intercom-attachments-7.com/i/o/597262963/9b1ce15067dd9bbe2dd944b5/fK0dSgk8x9jmI34J847RbL1CmbB2eZa0XI3VGOBQfzLgch1_WI5FVMYU0WbwFArW9Ay-rh1eF26wNnS73NUzUBV8MR4zh9Uv8oBX9uawXe9sPnBqpQ_VXXKbsecmlRQcoBaR9yIAVUXg8F0wpArxnGmiPU_vUbt4tthNdhTMPHwnaeXi6UmwkbHWpw" alt=""><figcaption></figcaption></figure>

## Usage <a href="#h_7b2567480e" id="h_7b2567480e"></a>

***

### 1. Issue-tracking <a href="#h_db20e6b636" id="h_db20e6b636"></a>

### a. Creating a GitHub issue <a href="#h_1278f6a768" id="h_1278f6a768"></a>

To create a GitHub issue together with a defect in Qase:

1. In the test run, mark your test case as Failed, Blocked, or Invalid and proceed with creating a Defect
2. In the Defect creation form, under “Choose Integrations”, select "GitHub App" and click "Add defect"
3. Choose the GitHub repository to create an issue in, then hit "Create"
4. In the Qase Defect you will now have a connected GitHub issue link
5. The statuses of the Qase Defect and the connected GitHub issue synced, meaning marking one as closed resolves the other (and vice versa).

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597263092/e11f0e507d8f9c15a8281cc8/O-FM2DmK-TDZ3HPQrOY7st8Iiw-hmVZXOeJfVPYOCsxKxWxNX9W1lKeYQnadDirByfuPJpEhL9XzELIsw1Wfd98y4Xe0dlao9fWj1I_YqSzTuygg78RX9_Upg-jv9hYbPeD_Z1VQcOG6dxj0inePKsET37J9bwssofpv3gv_RrlmgmSyID20YT_CfA" alt=""><figcaption></figcaption></figure>

### b. Link a GitHub issue to Test cases/Runs. <a href="#h_4711086d55" id="h_4711086d55"></a>

For Test cases -

1. Click on the test case you want to link the GitHub issue to.
2. Switch to the properties tab in the preview window.
3. Scroll down and click on "Link GitHub app issue"
4. In the modal window- select your repository, search for the issue and click on 'link'.

For Test runs -

1. Go to your Test runs view and click on the run you want to link the GitHub issue to.
2. In the Run dashboard, to the bottom right, find the button 'Select an integration' under External issue.
3. In the modal window- select your repository, search for the issue and click on 'link'.



**CI/CD Workflows**

To connect a GitHub workflow to Qase:

1. One of Qase reporter apps should be used in order to receive the test run results.
2.  Create a token in Qase and add it to the QASE\_API\_TOKEN secret in your [GitHub repository settings](https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository).



    <figure><img src="https://downloads.intercomcdn.com/i/o/686415821/6a017b8cffd368b175928f12/Untitled+(1).png" alt=""><figcaption></figcaption></figure>
3.  The inputs and env variables that are required need to be defined in a workflow:\


    ```
    on:
      workflow_dispatch:
        inputs:
          qase_api_base_url:
            description: 'Qase API URL'
            required: true
          qase_report:
            description: 'Enabled/disabled reporting to Qase'
            required: true
          qase_project_code:
            description: 'Qase project code'
            required: true
          qase_run_id:
            description: 'Qase Run ID'
            required: true
          qase_autocomplete_run:
            description: 'Qase Run autocomplete'
            required: true
    env:
      QASE_API_BASE_URL: ${{ inputs.qase_api_base_url }}
      QASE_REPORT: ${{ inputs.qase_report }}
      QASE_PROJECT_CODE: ${{ inputs.qase_project_code }}
      QASE_RUN_ID: ${{ inputs.qase_run_id }}
      QASE_COMPLETE_RUN_AFTER_SUBMIT: ${{ inputs.qase_autocomplete_run }}
      QASE_API_TOKEN: ${{ secrets.QASE_API_TOKEN }}
    ```
4.  Add a step to the first place in the job. It allows to link a GitHub workflow run with a Qase test run.\


    ```
    jobs:
      build-php:
        runs-on: ubuntu-latest
        steps:
          - uses: qase-tms/qase-link-run@main
            env:
              QASE_API_TOKEN: ${{ env.QASE_API_TOKEN }}
    ```
5. Add additional steps to execute your tests.

After the workflow is connected, you can initiate automated test runs from Qase:

1.  Start a new automated test run:



    <figure><img src="https://downloads.intercomcdn.com/i/o/686417783/f1ed2ade17bda74fdd94e8ce/Untitled+(2).png" alt=""><figcaption></figcaption></figure>
2.  Choose a CI/CD system to use (Github):



    <figure><img src="https://downloads.intercomcdn.com/i/o/686418072/1882d85fa68a2a67509062f8/Untitled+(3).png" alt=""><figcaption></figcaption></figure>
3.  Fill in the required fields:



    <figure><img src="https://downloads.intercomcdn.com/i/o/686418234/87e54a03cc218ea37b7bfecf/Untitled+(4).png" alt=""><figcaption></figcaption></figure>
4. Click "Start a run" button.
5.  You will be redirected to a test run you started. In the test run details section, you will see a link to the workflow run in GitHub and the current status.



    <figure><img src="https://downloads.intercomcdn.com/i/o/686418577/a39c6e87fbe8a37c7f10e383/Untitled+(5).png" alt=""><figcaption></figcaption></figure>
6.  When the tests have been executed, the test run will contain all the results sent by a reporter (it should be properly configured):



    <figure><img src="https://downloads.intercomcdn.com/i/o/686418932/9c8fe859543d42e402f4b44d/Untitled+(6).png" alt=""><figcaption></figcaption></figure>

### Troubleshooting: <a href="#h_d58df6962e" id="h_d58df6962e"></a>

If integration with GitHub has already been enabled before, it’s required to accept new permissions in the GitHub application settings.

In case of insufficient permissions after clicking on the “Start a run” button, a message with an error will appear.

<figure><img src="https://downloads.intercomcdn.com/i/o/686421060/896eaedb391fe7e3c4a673b4/Untitled+(7).png" alt=""><figcaption></figcaption></figure>

### Useful resource <a href="#h_cdd81132bc" id="h_cdd81132bc"></a>

An example of Github integration: [https://github.com/qase-tms/qase-javascript/tree/master/examples/github-qase-integration](https://github.com/qase-tms/qase-javascript/tree/master/examples/github-qase-integration)

\
