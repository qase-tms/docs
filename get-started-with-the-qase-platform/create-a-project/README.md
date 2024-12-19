# Projects

**What are projects in software testing?**

_Projects_ allow you to organize your [test suites](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-suite) and [test cases](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run) by putting them into separate spaces in Qase, thus preventing mixing up test cases related to different areas of development.

{% embed url="https://www.youtube.com/watch?v=kZCko4smO2s" %}

For example, if you manage and maintain a web application or website and accompanying mobile applications on iOS and Android, you can create three separate projects for the web application, iOS app, and Android app, respectively. In essence, a project is a container for all test cases pertaining to a specific app, website, etc.

To navigate to the list of your Projects, click "Projects" in the top-left corner of the workspace:

<figure><img src="../../.gitbook/assets/image (7) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

## Project Views <a href="#h_91be27eab1" id="h_91be27eab1"></a>

***

Once in the Projects view, you can choose between two layouts with the controller located in the top-right corner:

* **List view:**

<figure><img src="../../.gitbook/assets/list view.png" alt=""><figcaption></figcaption></figure>

* **Card view:**

<figure><img src="../../.gitbook/assets/card view.png" alt=""><figcaption></figcaption></figure>

In either List or Card view, you can mark a project as a favorite by clicking on the star icon while hovering over the left side of the project title in the list view and on the right side of the title on the card view. Marking a project as a favorite changes the order of appearance of the project. All projects marked as favorites appear above the other projects.

**List view:**

<figure><img src="../../.gitbook/assets/list view 2.png" alt=""><figcaption></figcaption></figure>

**Card view:**

<figure><img src="../../.gitbook/assets/card view star.png" alt=""><figcaption></figcaption></figure>

Additionally, in either of the views, you can also find the summary of each project:

* Unresolved defects that were filed during test runs in a project
* Number of test runs performed for the test cases belonging to a project
* Milestones related to a project
* Number of team members who have access to a project

List view features **Menu** icon where you can:

* edit Project settings (which can also be filled in when you create a new project)
* delete a project

<figure><img src="../../.gitbook/assets/Projects___Qase.jpg" alt="" width="563"><figcaption></figcaption></figure>

## Creating a new project <a href="#h_e19377e7df" id="h_e19377e7df"></a>

***

Once you are ready to start a new project, hit the "Create New Project" button:

<figure><img src="../../.gitbook/assets/new project.png" alt="" width="563"><figcaption></figcaption></figure>

Next, you will be prompted to fill out Project settings (which can also be edited later):

* **Project Name:** a descriptive name for your new project.​
* **Project Code:** a short name for your project, consisting of 2-6 symbols (only Latin characters and digits are allowed). Use this for nomenclature, and keep in mind that Project Code will be later added to any test cases created within that project.
* **Description:** use this field to provide extra context and additional details to anyone involved in your new project.

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.07.37 PM.png" alt="" width="375"><figcaption></figcaption></figure>

* **Project Access:** Projects can be made Public and Private. A Public project will be accessible to any users of the account, current, and anyone who will be joining later.\
  A Private Project can follow one of the three sharing rules:\
  ​
  1. _"Add all members to this project"_: every current account user you've invited will gain access to the project. Every new user who will join the account later will need to be granted access to this project manually.

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.10.25 PM.png" alt="" width="375"><figcaption></figcaption></figure>

2. _"Group access"_: with this option selected, you'll need to choose a [user group](https://docs.qase.io/administration/workspace-management/groups) you have created before - every user that belongs to a selected user group will then gain access to your new project.

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.12.52 PM.png" alt="" width="375"><figcaption></figcaption></figure>

3. _"Don't add members"_: With this option, you can limit access to yourself initially. Later, you can choose to share access with others as needed.

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.14.59 PM.png" alt="" width="375"><figcaption></figcaption></figure>

The final step is to confirm creating a new project by hitting the **"Create Project"** button below — once created, you are ready to build your project up with test cases.

{% hint style="info" %}
Owners of a workspace can view of projects, including private projects created by other users of the workspace.
{% endhint %}

## Project Settings <a href="#h_e70fd5f298" id="h_e70fd5f298"></a>

***

Once a Project is created, you can still manage who has access and have more control over your project in Settings.\
​

When you have opened the Project, navigate to Settings, where you will find several sections:

<figure><img src="../../.gitbook/assets/project setting.png" alt="" width="563"><figcaption></figcaption></figure>

### General settings: <a href="#h_542c61fba0" id="h_542c61fba0"></a>

Here, you can find and edit the same properties that you defined in the creation stage -

Project's Image, Name, Code, and Description.

<figure><img src="../../.gitbook/assets/general project settings.png" alt="" width="563"><figcaption></figcaption></figure>

### Access control: <a href="#h_b93cdae88e" id="h_b93cdae88e"></a>

<figure><img src="../../.gitbook/assets/access control.png" alt="" width="563"><figcaption></figcaption></figure>

From this tab, you can change the project owner and control who can access the project by adding individual members or groups.

If a project is set to public, all users of your workspace will have access. However, if Private is selected, you will have more options:



<details>

<summary>Add groups - select and add multiple groups to your project.</summary>

<img src="../../.gitbook/assets/add groups.png" alt="" data-size="original">

<img src="../../.gitbook/assets/private.png" alt="" data-size="original">

_All groups the have access to the project are listed here, along with the number of users in each group. Use the options from (---) menu to view, or revoke access of a specific group._

</details>

<details>

<summary>Add individual members - this is helpful if you need to add specific members.</summary>

<img src="../../.gitbook/assets/add users.png" alt="" data-size="original">

<img src="../../.gitbook/assets/members.png" alt="" data-size="original">

_You can view each member's Role and Role title here, and also remove access from the (--) menu._

</details>

{% hint style="success" %}
Adding individual members grants specific access to particular users, ensuring consistent access even if group memberships change. Conversely, adding users under groups provides access based on the group's membership, which may change over time.
{% endhint %}



### Repository: <a href="#h_7359bc0835" id="h_7359bc0835"></a>

<figure><img src="../../.gitbook/assets/repository.png" alt="" width="563"><figcaption></figcaption></figure>

Here, you have the options to:

<details>

<summary><strong>Enable Delete confirmation</strong> - if enabled, you will see a pop-up that requires you to type CONFIRM when bulk deleting test cases.</summary>

<img src="../../.gitbook/assets/delete test case.png" alt="" data-size="original">

</details>

<details>

<summary><strong>Enable Reviews</strong> - options to enable test case review. If "Review is mandatory" is enabled, the test case cannot be saved without sending for review.</summary>

If "Allow self-merge" is checked, the user who submitted the case for review will be able to merge changes once the minimum approvals required are met. If not enabled, submitter cannot merge changes.

If you specify a number in 'approvals required', changes to test cases cannot be merged unless the those minimum no.of approvals are met.

<img src="../../.gitbook/assets/send to review.png" alt="" data-size="original">

\


</details>

<details>

<summary>Show links - If enabled, cloned test cases will display a hyperlink to the original test case it was cloned from.</summary>

<img src="../../.gitbook/assets/show links.png" alt="" data-size="original">

</details>

### Test Run:

{% hint style="success" %}
There are option to modify both manual and automated Test runs. Refer to the [Test Run Settings](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run) section for a detailed description of these options.
{% endhint %}

### Test case: <a href="#h_54c17c77fd" id="h_54c17c77fd"></a>

<figure><img src="../../.gitbook/assets/test case settings.png" alt="" width="563"><figcaption></figcaption></figure>

<details>

<summary>Milestone field and Steps to reproduce section can be hidden by disabling these options.</summary>

<img src="../../.gitbook/assets/milestone.png" alt="" data-size="original">

</details>

<details>

<summary>Similarly, Tags and dataset can also be disabled from your project.</summary>

<img src="../../.gitbook/assets/tags.png" alt="" data-size="original">

</details>

The default test case steps type allows you to choose between Classic and Gherkin steps.

“All Fields” hyperlink which will redirect you to the “[Fields](https://app.qase.io/workspace/fields)” section of your workspace.

<details>

<summary>Once new settings have been selected, don't forget to hit "Update Settings" to apply changes.</summary>

<img src="../../.gitbook/assets/update settings.png" alt="" data-size="original">

</details>

### Webhooks: <a href="#h_aad86de7dd" id="h_aad86de7dd"></a>

<details>

<summary>In this section, you will find the webhooks that have been configured for this Project so far, or create a new webhook to connect Qase with other third-party solution you use.</summary>

When creating a new webhook, you can choose specific events that are going to trigger the endpoint.\


<img src="../../.gitbook/assets/create a webhook.png" alt="" data-size="original">

</details>

## Archiving a Project <a href="#h_705f39cb9a" id="h_705f39cb9a"></a>

Once a project has been completed, you might want to hide it from plain view - it should still be accessible for reference but shouldn't obstruct the view of the currently active projects.

For that, you can Archive your Project from the Project Settings:

<figure><img src="../../.gitbook/assets/archive project.png" alt=""><figcaption></figcaption></figure>

And now, while in the Projects area, you can switch between viewing Active or Archived projects or view them all at once simultaneously:

<figure><img src="../../.gitbook/assets/archived.png" alt="" width="563"><figcaption></figcaption></figure>
