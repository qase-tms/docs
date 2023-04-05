# Roles

### What are the roles in Qase?

Roles are an important tool that allows you to define what your [teammates](https://help.qase.io/en/articles/5563739-workspace-management-users) can and cannot do in your Qase account. When defining a role, you can specify restrictions down to a very granular level, ensuring that those who need more control have it. In contrast, anybody who should have a limited scope and visibility is properly restricted.

_<mark style="background-color:purple;">Custom roles are available in</mark>_ [_<mark style="background-color:purple;">Business</mark>_](https://help.qase.io/en/articles/5563727-business-plan) _<mark style="background-color:purple;">and</mark>_ [_<mark style="background-color:purple;">Enterprise</mark>_](https://help.qase.io/en/articles/6640055-enterprise-plan) _<mark style="background-color:purple;">subscriptions</mark>_

{% embed url="https://youtu.be/A0xIgnbSxAg" %}

### Pre-configured roles

By default, your Qase account comes pre-configured with three roles already set up:

* _Owner:_ An owner of the account, a person that registered the account initially, has full control of the account's features (Including private projects created by other users in the account) and can manage all aspects of the application.
* _Admin:_ An administrative role in the account similar to the owner.
* _Member:_ A common role that grants access to all the basic Qase features; it is set as the default role in your new account, which means that any new member that is being invited gets _member_ role restrictions assigned to them - but you can set a different user role (except for _owner_ user role) to be a default one at any time.

Note: Type of license is always stronger than the role. You can have an administrator _role_ but be a read-only user: you will be read-only first, it will be a stronger setting. Same for the _billing_ user.

### Create a new user role <a href="#h_08e07ce250" id="h_08e07ce250"></a>

You are not limited to the pre-configured user roles. To create a new user role, go to "Roles" in workspace management, and click "Create a new role":

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597195687/32c3d4602991457452e3fbe1/rSdm1a0F-pa9lQ14mMFwDT4vqw6FGPbeP_cwWcz10ZUT3TtbeRfIbX7HZwsaYpfBp1LF6LrOGuXmhObBH4qHPK15zLio8NwBU51NIIQzGT6luveeE2G6F8fNizjwv22RRB6Ug9nz8eIlb7txpJxPes111P_lrGB6AwJn21B6BvHR98se8bmQa5R0uw" alt=""><figcaption></figcaption></figure>

In the creation menu, fill in the role settings:

[![](https://qase.intercom-attachments-7.com/i/o/597195696/d38243bcc101c28944c7a586/sa65MU88SfdeVzW\_c7y2AvpNmHbX\_y\_mQ-3D0X1q35oZIOjs2AG9hn8xpixoyzUo1xIDvyi1f7bXkTYRAVRqJPyevjeHTESdC7hSWiixRiBr2LhYKR91e4WTP4VzreXoQo5\_xmx1zZwRJYrz2Vk8CjEOwiN8vMoJ28gPotmsITyrc25c1wgXwUOQsw)](https://qase.intercom-attachments-7.com/i/o/597195696/d38243bcc101c28944c7a586/sa65MU88SfdeVzW\_c7y2AvpNmHbX\_y\_mQ-3D0X1q35oZIOjs2AG9hn8xpixoyzUo1xIDvyi1f7bXkTYRAVRqJPyevjeHTESdC7hSWiixRiBr2LhYKR91e4WTP4VzreXoQo5\_xmx1zZwRJYrz2Vk8CjEOwiN8vMoJ28gPotmsITyrc25c1wgXwUOQsw)

* _Role Title_
* _Role Description_
* _Set as default role -_ check the box to apply this user role's settings to any new member joining the account.

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597195705/f56bc18c4b5d416e4ff15e79/jLjJBCoiT5i1U06DXN0uqs7T17gin5IT7Q3Ce7KtWC9JtlCfJHASdmiis0yqQ2sSzOBlQlXo6kP8URcxWLfuAkhNo_Hiyr7uQprEbKrh0sZbUxkXgpC1Xdq20g6-MNy9bgILN-H3FGF7nylVH4XCbNechPan7uMSoJ4Q1HxzF5t3Uf3bvFXx9F_mDg" alt=""><figcaption></figcaption></figure>

### Role access rights

The following section is dedicated to role access rights. Here, you will define which entities and actions will be available to users with a specific role. Each entity can be fully restricted or fully allowed, and each action with an entity can be made available or unavailable.

* Entity: **Projects**
  * _Create / update:_ This rule allows users to create new projects and update their settings.users
  * _Remove:_ This rule allows users to delete projects.
  * _Access Control:_ This rule allows users to manage access to the project, adding or removing members.
  * _Import:_ This rule allows users to import test cases from various sources.
  * _Export:_ This rule allows users to export test cases.
* Entity: **Project integrations**
  * _View:_ This rule allows users to view a list of installed and available integrations.
  * _Add/Update:_ This rule allows users to add new integrations to project or update their settings.
  * _Remove:_ This rule allows users to remove installed integrations.
* Entity: **Test cases**
  * _Repository:_ This rule allows users to view test cases in the test case repository.
  * _Create/Update:_ This rule allows users to create or update test cases in the test case repository.
  * _Remove:_ This rule allows users to delete test cases.
  * _Change sort order:_ This rule allows users to drag-n-drop test cases on the repository page.
  * _Approve / decline:_ This rule allows users to approve or decline test case changes during the review process.
  * _Rollback:_ This rule allows users to undo changes done to test cases.
* Entity: **Test suites**
  * _Create/Update:_ This rule allows users to create or update test suites.
  * _Remove:_ This rule allows users to delete the test suite and move its content to another suite
  * _Change suite position:_ This rule allows users to drag-n-drop test suites on the repository page.
* Entity: **Test reviews**
  * _View:_ This rule allows users to view a list of existing reviews.
* Entity: **Milestones**
  * _View:_ This rule allows users to view a list of existing milestones.
  * _Create/Update:_ This rule allows users to create or update milestones.
  * _Remove:_ This rule allows users to delete milestones.
* Entity: **Shared steps**
  * _View:_ This rule allows users to view a list of existing shared steps.
  * _Create/Update:_ This rule allows users to create or update shared steps.
  * _Remove:_ This rule allows users to delete shared steps.
* Entity: **Test plans**
  * _View:_ This rule allows users to view a list of existing test plans.
  * _Create/Update:_ This rule allows users to create or update test plans.
  * _Remove:_ This rule allows users to delete test plans.
* Entity: **Test runs**
  * _View:_ This rule allows users to view a list of existing test runs.
  * _Create/Update:_ This rule allows users to create or update test runs.
  * _Submit results:_ This rule allows users to submit run results.
  * _Assign:_ This rule allows users to set “assignee.”
  * _Remove:_ This rule allows users to delete test runs.
  * _Synchronize:_ This rule allows users to sync a test case in a run with the test case in the repository.
  * _Manage configurations:_ This rule allows users to create, update or delete configurations.
* Entity: **Defects**
  * _View:_ This rule allows users to view a list of existing defects.
  * _Create/Update_: This rule allows users to create or update defects.
  * _Resolve:_ This rule allows users to resolve open defects.
  * _Remove:_ This rule allows users to delete defects.
* Entity: **Webhooks**
  * _View:_ This rule allows users to view a list of existing webhooks.
  * _Create/Update:_ This rule allows users to create or update webhooks.
  * _Remove:_ This rule allows users to delete webhooks.
* Entity: **Workspace**
  * _Update settings:_ This rule allows users to update team settings.
  * _Invite:_ This rule allows users to invite new members to the team.
  * _Activate/Deactivate:_ This rule allows users to activate or deactivate team members.
  * _Workspace User Update:_ This rule allows users to change team member details and roles.
  * _Users view:_ This rule allows users to view users.
  * _Logs_: This rule allows users to view [logs](https://help.qase.io/en/articles/5563743-workspace-management-audit-logs).
* Entity: **Team groups**
  * _View:_ This rule allows users to view a list of existing groups.
  * _Create/Update:_ This rule allows users to create or update team groups. It also allows users to add or remove team members from groups.
  * _Remove:_ This rule allows users to delete team groups.
* Entity: **Team roles**
  * _View:_ This rule allows users to view a list of existing roles.
  * _Create/Update:_ This rule allows users to create or update team roles.
  * _Remove:_ This rule allows users to delete team roles.
* Entity: **Environments**
  * _View:_ This rule allows users to view a list of existing environments_._
  * _Create/Update:_ This rule allows users to create or update environments.
  * _Remove:_ This rule allows users to delete environments.
* Entity: **Fields**
  * _View:_ This rule allows users to view a list of existing fields.
  * _Create:_ This rule allows users to create custom fields.
  * _Update:_ This rule allows users to update custom fields.
  * _Remove:_ This rule allows users to delete custom fields.
* Entity: **Tags**
  * _Create:_ This rule allows users to create tags on fly.
  * _View:_ This rule allows users to view a list of existing tags in workspace.
  * _Delete:_ This rule allows users to delete tags in workspace.
* Entity: **Attachments**
  * _View:_ This rule allows users to view a list of existing attachments.
  * _Remove:_ This rule allows users to delete attachments.
* Entity: **Billing**
  * _Manage:_ This rule grants all access to the billing section and allows users to manage subscriptions, payment methods, and billing details.
* Entity: **Requirements**
  * _View:_ This rule allows users to view existing requirements.
  * _Create/update:_ This rule allows users to create or update requirements.
  * _Remove:_ This rule allows users to delete requirements.
* Entity: **Dashboard**
  * _View:_ This rule allows users to view existing dashboards.
  * _Create:_ This rule allows users to create dashboards.
  * _Update:_ This rule allows users to update any dashboards.
  * _Remove:_ This rule allows users to delete any dashboards.
* Entity: **Security**
  * _SSO:_ This rule allows users to configure SSO.
