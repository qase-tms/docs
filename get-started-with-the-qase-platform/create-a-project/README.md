# Projects

**What are projects in software testing?**

_Projects_ allow you to organize your [test suites](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-suite) and [test cases](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run) by putting them into separate spaces in Qase, thus preventing mixing up test cases related to different areas of development.

{% embed url="https://www.youtube.com/watch?v=VKsnZ3f5Ak8" %}

For example, if you manage and maintain a web application or website and accompanying mobile applications on iOS and Android, you can create three separate projects for the web application, iOS app, and Android app, respectively. In essence, a project is a container for all test cases pertaining to a specific app, website, etc.

To navigate to the list of your Projects, click "Projects" in the top-left corner of the workspace:

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 1.58.42 PM.png" alt=""><figcaption></figcaption></figure>

Once in the Projects view, you can choose between two layouts with the controller located in the top-right corner:

* **List view:**

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 1.59.20 PM.png" alt=""><figcaption></figcaption></figure>

* **Card view:**

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.00.53 PM.png" alt=""><figcaption></figcaption></figure>

In either List or Card view, you can mark a project as a favorite by clicking on the star icon while hovering over the left side of the project title in the list view and on the right side of the title on the card view. Marking a project as a favorite changes the order of appearance of the project. All projects marked as favorites appear above the other projects.

**List view:**

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.01.28 PM.png" alt=""><figcaption></figcaption></figure>

**Card view:**\


<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.05.18 PM.png" alt=""><figcaption></figcaption></figure>

Additionally, in either of the views, you can also find the summary of each project:

* Unresolved defects that were filed during test runs in a project
* Number of test runs performed for the test cases belonging to a project
* Milestones related to a project
* Number of team members who have access to a project

List view features **Menu** icon where you can:

* edit Project settings (which can also be filled in when you create a new project)
* set up integrations with 3rd party tools for a project
* delete a project

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.06.27 PM.png" alt=""><figcaption></figcaption></figure>

## New Project <a href="#h_e19377e7df" id="h_e19377e7df"></a>

Once you are ready to start a new project, hit the "Create New Project" button:

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.06.58 PM.png" alt=""><figcaption></figcaption></figure>

Next, you will be prompted to fill out Project settings (which can also be edited later):

* **Project Name:** a descriptive name for your new project.​
* **Project Code:** a short name for your project, consisting of 2-6 symbols (only Latin characters and digits are allowed). Use this for nomenclature, and keep in mind that Project Code will be later added to any test cases created within that project.
* **Description:** use this field to provide extra context and additional details to anyone involved in your new project.

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.07.37 PM.png" alt=""><figcaption></figcaption></figure>

* **Project Access:** Projects can be made Public and Private. A Public project will be accessible to any users of the account, current, and anyone who will be joining later.\
  A Private Project can follow one of the three sharing rules:\
  ​
  1. _"Add all members to this project"_: every current account user you've invited will gain access to the project. Every new user who will join the account later will need to be granted access to this project manually.

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.10.25 PM.png" alt=""><figcaption></figcaption></figure>

2. _"Group access"_: with this option selected, you'll need to choose a [user group](https://docs.qase.io/administration/workspace-management/groups) you have created before - every user that belongs to a selected user group will then gain access to your new project.

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.12.52 PM.png" alt=""><figcaption></figcaption></figure>

3. _"Don't add members"_: with this option, you can keep your project private for the time being and share it with others once you're ready.

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.14.59 PM.png" alt=""><figcaption></figcaption></figure>

The final step is to confirm creating a new project by hitting the **"Create Project"** button below - once created, you are ready to build your project up with test cases.

\
**​N/B:** Owners of a workspace can view all projects including private projects created by other users of the workspace.

## Project Access and Project Settings <a href="#h_e70fd5f298" id="h_e70fd5f298"></a>

Once a Project is created, you can still manage who can access and see it and have more control over your project in Settings.

**Project Settings:** When you have opened the Project, navigate to Settings, where you will find several sections:

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.23.35 PM.png" alt=""><figcaption></figcaption></figure>

_General:_ Here, you can find and edit the same properties that you defined in the creation stage - Project Name, Project Code, Description, and Project access type.\
​\
The option to share the project with a user group is also available in this page. You can only share a private project with a group.

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.24.07 PM.png" alt=""><figcaption></figcaption></figure>

* _Repository_: Here, you'll find options pertaining to the Repository itself.

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.24.35 PM.png" alt=""><figcaption></figcaption></figure>

* [_Webhooks_](https://docs.qase.io/general/webhooks)_:_ In this section, you will find the webhooks that have been configured for this Project so far, or create a new webhook to connect Qase with another third-party solution you use.\
  ​
* _Test Run:_ Here, you can customize various requirements and automation for [Test Runs](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run-1)

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.35.20 PM.png" alt=""><figcaption></figcaption></figure>

Also, you can choose which [Test Case](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run) settings you want to have enabled and which ones are not necessary. To view a detailed list of all the fields available to you, you can click on the “All Fields” hyperlink which will redirect you to the “Fields” section of your project:\


<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.28.23 PM.png" alt=""><figcaption></figcaption></figure>

Once new settings have been selected, don't forget to hit "Update Settings" to apply changes:

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.29.45 PM.png" alt=""><figcaption></figcaption></figure>

## Archiving a Project <a href="#h_705f39cb9a" id="h_705f39cb9a"></a>

Once a project has been completed, you might want to hide it from plain view - it should still be accessible for reference but shouldn't obstruct the view of the currently active projects.

For that, you can Archive your Project from the Project Settings:

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.30.20 PM.png" alt=""><figcaption></figcaption></figure>

And now, while in the Projects area, you can switch between viewing Active or Archived projects or view them all at once simultaneously:

<figure><img src="../../.gitbook/assets/Screenshot 2023-12-04 at 2.30.59 PM.png" alt=""><figcaption></figcaption></figure>
