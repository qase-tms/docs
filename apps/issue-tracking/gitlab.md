# GitLab

### What is GitLab?

[GitLab](https://about.gitlab.com/) is a web-based DevOps lifecycle tool that provides a Git repository manager providing wiki, issue-tracking, and CI/CD pipeline features.

{% embed url="https://youtu.be/LBEUgW0YvcE" %}



With **Qase’s GitLab integration**, you can:

* Link Qase [test cases](https://docs.qase.io/general/get-started-with-the-qase-platform/test-cases) to GitLab issues
* Create a new issue in GitLab when you file a [defect](https://docs.qase.io/general/get-started-with-the-qase-platform/defects) during a test run in Qase
* Link Qase [test runs](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run) to GitLab issues
* Execute automated runs in GitLab from a Qase.

## Installation <a href="#h_ff8e665948" id="h_ff8e665948"></a>

For installation, you will require `GitLab URL` and the `Access token`.

1. First, sign-in to your GitLab account and navigate to the `Preferences` from the profile menu:

<figure><img src="../../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>

2. Go to the `Access tokens` page:

<figure><img src="../../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure>

3. To create a new `Personal Access Token`, select the scope `api` and click on the _Create Personal Access token_:

<figure><img src="../../.gitbook/assets/image (75).png" alt=""><figcaption></figcaption></figure>

4. Copy your token to clipboard.
5. On Qase, navigate to the [Apps](https://app.qase.io/apps) section, find the GitLab app and click `Install now`.

Here, provide the Access token from the previous step, and URL of your GitLab instance (_the field is pre-populated with the default value)_

<figure><img src="../../.gitbook/assets/image (76).png" alt=""><figcaption></figcaption></figure>

Click the `Install` button. After a few seconds, you will be redirected to the `Apps` page with a confirmation message as shown below.

<figure><img src="../../.gitbook/assets/image (77).png" alt=""><figcaption></figcaption></figure>

<mark style="background-color:yellow;">**​Note:**</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">If you prefer to use a group token, make sure that a "Maintainer" role level is required for such a group token.</mark>

### Usage <a href="#h_c5cfb8f18a" id="h_c5cfb8f18a"></a>

#### Linking from Qase to GitLab: <a href="#h_a405434ebc" id="h_a405434ebc"></a>

1\. To link a GitLab to a Qase test case from Qase:

* Select a case in the repository and switch to properties in the sidebar
* Click "Link GitLab app issues"
* Insert GitLab issue title into the field and hit "Link"
* Now the issue is linked:

<figure><img src="../../.gitbook/assets/link gitlab.gif" alt=""><figcaption></figcaption></figure>

2\. To unlink the GitLab issue, click "x" next to the card title:

<figure><img src="../../.gitbook/assets/image (78).png" alt=""><figcaption></figcaption></figure>

3\. Link Qase Test Runs to GitLab issues:

* Navigate to the Test Runs page
* Click on the Run
* In the Run's main page, locate the sidebar to the right
* Scroll down and under "External Issue" click on "Select an Integration"
* Select "GitLab app"
* Search for the issue's title and click on "Link"

<figure><img src="../../.gitbook/assets/link lab test runs.gif" alt=""><figcaption></figcaption></figure>

### Create a GitLab issue from a Qase Test Run <a href="#h_11228e75f2" id="h_11228e75f2"></a>

* In the test run, mark your case as Failed, Blocked, or Invalid and proceed with creating a Defect.
* in the Defect creation form, under “Choose Integrations” select "GitLab App" and click "Add defect"
* Fill in the required fields, then hit "Create"

<figure><img src="../../.gitbook/assets/lab create defect.gif" alt=""><figcaption></figcaption></figure>

* You can view the link to the GitLab issue in
  * Defects tag of the test run

<figure><img src="../../.gitbook/assets/Screenshot 2024-07-02 at 10.42.43.png" alt=""><figcaption></figcaption></figure>

* From the Qase defect screen

<figure><img src="../../.gitbook/assets/image (79).png" alt=""><figcaption></figcaption></figure>

### CI/CD Workflows <a href="#h_26230aa4af" id="h_26230aa4af"></a>

***

1. Create the `Automated Test Run`:

<figure><img src="../../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>

2. Select the `Gitlab` option in the `CI/CD System` field:

<figure><img src="../../.gitbook/assets/image (81).png" alt=""><figcaption></figcaption></figure>

3. Fill in all necessary fields and click the `Start a run` button:

<figure><img src="../../.gitbook/assets/image (82).png" alt=""><figcaption></figcaption></figure>
