# AIDEN - Role based access control

Control who can [create tests using AIDEN](https://help.qase.io/en/articles/9653096-aiden-test-designer), execute on [Test cloud](https://help.qase.io/en/articles/11851804-aiden-ai-test-cloud), and access other [AI-powered features](https://help.qase.io/en/collections/12458870-qase-ai) with granular permissions.

These settings help you balance team productivity with security and budget requirements by allowing different levels of access to AIDEN's capabilities.

***

### Understanding AIDEN Permissions <a href="#h_60af0e898f" id="h_60af0e898f"></a>

<figure><img src="../.gitbook/assets/image (108).png" alt="" width="563"><figcaption></figcaption></figure>

In the role's permissions, the AIDEN section allows you to customize access based on team roles and organizational policies.

Instead of an all-or-nothing approach, you can now enable specific AIDEN capabilities while restricting others.

***

### Available Permission Types <a href="#h_bd45730d44" id="h_bd45730d44"></a>

[Manual Testing – Create](https://help.qase.io/en/articles/9653096-aiden-test-designer): Controls access to AI-powered manual test case generation through the "Create with AI" feature.

[Automation – Create](https://help.qase.io/en/articles/11012497-aiden-qa-architect): Manages the ability to generate automated test cases using AIDEN's automation capabilities.

[Automation – Execute](https://help.qase.io/en/articles/11851804-aiden-ai-test-cloud): Determines who can run automated tests on the Test Cloud platform.

[Advisor – Analyse](https://help.qase.io/en/articles/11981696-aiden-test-advisor): Controls access to AIDEN's Test advisor feature for existing test cases.

[Code Download](https://help.qase.io/en/articles/11981749-aiden-automation-engineer): Manages the ability to export and download AI-generated test code.

***

### Know the defaults <a href="#h_68af9d2f3d" id="h_68af9d2f3d"></a>

**Standard system roles:**

\- Admin, Owner, Member: Full access to all AIDEN capabilities by default

\- Read-Only: No access to any AIDEN features

**Custom roles:**

You can configure permissions for each AIDEN capability, when creating or editing the role.

Read more about custom roles, [here.](https://help.qase.io/en/articles/5563741-workspace-management-roles-permissions)

***

### What happens when a permission is disabled for a role? <a href="#h_f8e2e2bac8" id="h_f8e2e2bac8"></a>

When a permission is disabled, the corresponding feature disappears from the user interface to maintain clarity and prevent confusion.

***

### Why might I need RBAC for AIDEN? <a href="#h_b5884abc44" id="h_b5884abc44"></a>

Budget Control: You may want to use only a specific feature and disable others to prevent accidental usage, or unexpected costs.

Security Policy Compliance: for example, your organization needs to prevent code export while allowing test creation.

Tiered Access: Different teams/roles require different AIDEN capabilities.

***

To completely disable all AI features in your workspace, please check [this page](https://app.qase.io/workspace/settings).
