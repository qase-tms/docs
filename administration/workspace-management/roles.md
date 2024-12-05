# Roles

### What are the roles in Qase?

**Roles** are an important tool that allows you to define what your [teammates](https://help.qase.io/en/articles/5563739-workspace-management-users) can and cannot do in your Qase account. When defining a role, you can specify restrictions down to a very granular level, ensuring that those who need more control have it. In contrast, anybody who should have a limited scope and visibility is properly restricted.

_<mark style="background-color:purple;">Custom roles are available in</mark>_ [_<mark style="background-color:purple;">Business</mark>_](https://help.qase.io/en/articles/5563727-business-plan) _<mark style="background-color:purple;">and</mark>_ [_<mark style="background-color:purple;">Enterprise</mark>_](https://help.qase.io/en/articles/6640055-enterprise-plan) _<mark style="background-color:purple;">subscriptions</mark>_

{% embed url="https://youtu.be/A0xIgnbSxAg" %}

{% embed url="https://www.youtube.com/watch?v=mHtnivFRBck" %}

### Pre-configured roles

By default, your Qase account comes pre-configured with three Roles already set up:

* _Owner:_ An owner of the account, a person that registered the account initially, has full control of the account's features (Including private projects created by other users in the account) and can manage all aspects of the application.
* _Admin:_ An administrative role in the account similar to the Owner.
* _Member:_ A common role that grants access to all the basic Qase features; it is set as the Default role in your new account, which means that any new member that is being invited gets _Member_ role restrictions assigned to them - but you can set a different User Role (except for _Owner_ user role) to be a Default one at any time.

**Note:** Type of license is always stronger than the role. You can have an administrator _role_ but be a read-only user: you will be read-only first, it will be a stronger setting. Same for the _Billing_ user.

### Create a new user role <a href="#h_08e07ce250" id="h_08e07ce250"></a>

You are not limited to the pre-configured user roles. To create a new user role, go to "Roles" in workspace management, and click "Create a new role":

<figure><img src="../../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>

In the creation menu, fill in the Role Settings:

* _Role Title_
* _Role Description_
* _Set as default role -_ Check the box to apply this User Role's settings to any new member joining the workspace.

<figure><img src="../../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>

### Role access rights

The next block is dedicated to the Role access rights - this is where you will define which entities and which kinds of actions will be available to users granted this User Role. Each entity can be restricted or allowed, and each action with an entity can be made available or unavailable.

<figure><img src="../../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>

* **Entity**: [Attachments](https://docs.qase.io/administration/workspace-management/attachments)
  * _View:_ This rule allows users to view a list of existing attachments.
  * _Remove:_ This rule allows users to delete attachments.
* **Entity:** [Billing](https://docs.qase.io/administration/billing)
  * _Manage:_ This rule grants all access to the billing section and allows to manage subscriptions, payments and billing details.
* **Entity:** [Test Cases](https://docs.qase.io/general/get-started-with-the-qase-platform/test-cases)
  * _Repository:_ This rule allows users to view test cases in the test case repository.
  * _Create/Update:_ This rule allows users to create or update test cases in the test case repository.
  * _Remove:_ This rule allows users to delete test cases.
  * _Change sort order:_ This rule allows users to drag and drop test cases on the repository page.
  * _Approve/Decline:_ This rule allows users to approve or decline test case changes during the review process.
  * _Rollback:_ This rule allows users to undo changes done to test cases.
  * _Mute/Unmute:_ This rule allows user to mute or unmute a test case.
* **Entity:** [Dashboard](https://docs.qase.io/general/analytics/dashboards)
  * _View:_ This rule allows users to view existing dashboards.
  * _Create:_ This rule allows users to create dashboards.
  * _Update:_ This rule allows users to update any dashboards.
  * _Remove:_ This rule allows users to delete any dashboards.
* **Entity:** [Defects](https://docs.qase.io/general/get-started-with-the-qase-platform/defects)
  * _View:_ This rule allows users to view a list of existing defects.
  * _Create/Update_: This rule allows users to create or update defects.
  * _Remove:_ This rule allows users to delete defects.
  * _Resolve:_ This rule allows users to resolve open defects.
* **Entity:** [Environments](https://docs.qase.io/general/execution/environments)
  * _View:_ This rule allows users to view a list of existing environment&#x73;_._
  * _Create/Update:_ This rule allows users to create or update environments.
  * _Remove:_ This rule allows users to delete environments.
* **Entity:** [Fields](https://docs.qase.io/administration/workspace-management/fields)
  * _View:_ This rule allows users to view a list of existing fields.
  * _Update:_ This rule allows users to update custom fields.
  * _Create:_ This rule allows users to create custom fields.
  * _Remove:_ This rule allows users to delete custom fields.
* **Entity:** [Team Groups](https://docs.qase.io/administration/workspace-management/groups)
  * _View:_ This rule allows users to view a list of existing groups.
  * _Create/Update:_ This rule allows users to create or update team groups. It also allows users to add or remove team members from groups.
  * _Remove:_ This rule allows users to delete team groups.
* **Entity:** [Applications](https://help.qase.io/en/collections/3564516-apps)
  * _View:_ This rule allows users to view a list of installed and available applications.
  * _Install:_ This rule allows users to add an application.
  * _Uninstall:_ This rule allows users to remove an application.
  * _Update:_ This rule allows users to update application settings.
* **Entity:** [Milestones](https://docs.qase.io/general/issues/milestones)
  * _View:_ This rule allows users to view a list ofte existing milestones.
  * _Create/Update:_ This rule allows users to create or update milestones.
  * _Remove:_ This rule allows users to delete milestones.
* **Entity:** [Test Plans](https://docs.qase.io/general/execution/test-plan)
  * _View:_ This rule allows users to view a list of existing test plans.
  * _Create/Update:_ This rule allows users to create or update test plans.
  * _Remove:_ This rule allows users to delete test plans.
* **Entity:** [Projects](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-project)
  * _Create/Update:_ This rule allows users to create new projects and update their settings.
  * _Remove:_ This rule allows users to delete projects.
  * _Access Control:_ This rule allows users to manage access to the project: add or remove members.
  * _Change ownership_: This rule allows users to change the project owner.
  * _Import:_ This rule allows users to import test cases from various sources.
  * _Export:_ This rule allows users to export test cases.
* **Entity**: [Requirements](https://docs.qase.io/general/issues/requirements)
  * _View:_ This rule allows users to view existing requirements.
  * _Create/update:_ This rule allows users to create or update requirements.
  * _Remove:_ This rule allows users to delete requirements.
* **Entity:** [Test reviews](https://docs.qase.io/general/get-started-with-the-qase-platform/test-cases/test-case-review)
  * _View:_ This rule allows users to view a list of existing reviews.
* **Entity:** [Team Roles](https://docs.qase.io/administration/workspace-management/roles)
  * _View:_ This rule allows users to view a list of existing roles.
  * _Create/Update:_ This rule allows users to create or update team roles.
  * _Remove:_ This rule allows users to delete team roles.
* **Entity:** [Test Runs](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run)
  * _View:_ This rule allows users to view a list of existing test runs.
  * _Create/Update:_ This rule allows users to create or update test runs.
  * _Remove:_ This rule allows users to delete test runs.
  * _Submit results:_ This rule allows users to submit run results.
  * _Assign:_ This rule allows users to set “assignee.”
  * _Manage configurations:_ This rule allows users to create, update, or delete configurations.
* **Entity:** [Security](https://docs.qase.io/administration/security)
  * _SSO:_ This rule allows users to configure SSO.
* **Entity:** [Shared Steps](https://docs.qase.io/general/get-started-with-the-qase-platform/test-cases/shared-steps)
  * _View:_ This rule allows users to view a list of existing shared steps.
  * _Create/Update:_ This rule allows users to create or update shared steps.
  * _Remove:_ This rule allows users to delete shared steps.
* **Entity:** [Test Suites](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-suite)
  * _Create/Update:_ This rule allows users to create or update test suites.
  * _Remove:_ This rule allows users to delete the test suite and move its content to another suite
  * _Change suite position:_ This rule allows users to drag and drop test suites on the repository page.
* **Entity**: [Tags](https://docs.qase.io/administration/workspace-management/tags)
  * _View:_ This rule allows users to view a list of existing tags in the workspace.
  * _Create/update:_ This rule allows users to create tags on the fly.
  * _Remove:_ This rule allows users to delete tags in the workspace.
* **Entity:** [Workspace](https://docs.qase.io/administration/workspace-management/users)
  * _Update settings:_ This rule allows users to update workspace settings.
  * _Invite:_ This rule allows users to invite new members to the workspace.
  * _Activate/Deactivate:_ This rule allows users to activate or deactivate users.
  * _Workspace User Update:_ This rule allows users to change team member details and roles.
  * _Users view:_ This rule allows users to view users.
  * _Logs_: This rule allows users to view [logs](https://docs.qase.io/administration/workspace-management/audit-logs).
* **Entity:** [Webhooks](https://docs.qase.io/general/webhooks)
  * _View:_ This rule allows users to view a list of existing webhooks.
  * _Create/Update:_ This rule allows users to create or update webhooks.
  * _Remove:_ This rule allows users to delete webhooks.
* Entity: [QQL](https://docs.qase.io/general/analytics/queries)
  * View: This rule allows users to execute a QQL and view a list of existing QQL.
  * Create/update: This rule allows users to create or update saved QQL.
  * Remove: This rule allows users to delete saved QQL.
