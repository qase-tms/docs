# Custom fields

{% hint style="info" %}
Custom Fields are available in [Startup](../subscriptions/startup-plan.md), [Business](../subscriptions/business-plan.md), and [Enterprise](../subscriptions/enterprise-plan.md) subscriptions
{% endhint %}

### What are custom fields in Qase?

Obviously, test scenarios come with all varieties of data connected to them. It is pretty much impossible for us at Qase to predict every single data point you want to record for your [Test Cases](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run), [Test Runs](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-test-run-1), or [Defects](https://docs.qase.io/general/get-started-with-the-qase-platform/defects).&#x20;

So instead of trying to cover all bases or giving a bare minimum, we provide you with Custom Fields - a tool to create your own custom data entry points.

{% embed url="https://www.youtube.com/watch?v=o7YiwJpRmkA" %}

You'll need to create these Custom Fields first to be able to fill them in. To get started, navigate to the Workspace settings' "Fields" section:

<figure><img src="../../.gitbook/assets/95842.png" alt="" width="375"><figcaption></figcaption></figure>

### Create custom fields

Create a new Custom Field by clicking "+ Create New Custom Field", configure your Custom Field, and define what it will be representing:

* _Title:_ give a brief descriptive name to your Custom Field (Title is the only mandatory parameter).\


<figure><img src="../../.gitbook/assets/33247.png" alt="" width="375"><figcaption></figcaption></figure>

* _Entity:_ define which Qase entities your Custom Field will apply to - Test Cases, Test Runs, or Defects. This parameter is a single-choice one, so you cannot select "Test Cases" AND "Test Runs"; if you need to track similar data for both Runs and Cases, you'll need to create two separate Custom Fields for that.

<figure><img src="../../.gitbook/assets/85821.png" alt="" width="375"><figcaption></figcaption></figure>

* _Type:_ select from a dropdown which data type will be used in this Custom Field. Depending on the type of data selected, the options below will be different.\
  **​**_**NB:** once a custom field has been created, its type cannot be changed._

<figure><img src="../../.gitbook/assets/297.png" alt="" width="373"><figcaption></figcaption></figure>

* _Enable for all projects:_ choose which Projects your custom field should be applied to. If you have to capture the same data uniformly in multiple projects, you don't have to create duplicates of a field for each project - create a custom field once and apply it to various projects:

<figure><img src="../../.gitbook/assets/3158.png" alt="" width="374"><figcaption></figcaption></figure>

* _Placeholder:_ provide a sample value that will be appearing in a field in a faded color, while the Custom Field remains empty. This can help avoid confusion about what should go into the field.\

* _Default value:_ to avoid having Custom Fields left blank, you can automatically insert a default value

<figure><img src="../../.gitbook/assets/30459 (1).png" alt="" width="374"><figcaption></figcaption></figure>

* _Required field_ checkbox: checking this box will make a field mandatory; an entity with such Custom Field will not be created until Custom Field is filled in.

<figure><img src="../../.gitbook/assets/62850.png" alt="" width="374"><figcaption></figcaption></figure>

* _Values:_ Available for Multiselect and Selectbox types of data, this area allows you to define values to choose from when filling out a custom field:

<figure><img src="../../.gitbook/assets/44271.png" alt="" width="373"><figcaption></figcaption></figure>

Creating Values:

1. Click and hold the 6 dots to drag and drop your values when organizing their order.
2. Click the default "plus" icon to open the icon customization options.
3. You can choose from the default colors or input the Hex color code for the icon.
4. You can enter the icon code starting with "fas fa-" followed by the icon name chosen from the provided external link.
5. Add a new value input field
6. Delete a value input field

<figure><img src="../../.gitbook/assets/97365.png" alt="" width="373"><figcaption></figcaption></figure>

When exporting into CSV, your Custom Fields will appear as new columns on the far right of your CSV file.​They will be named "`cf_1`", "`cf_2`", "`cf_3`"... following the order of creation of your custom field in your Workspace Fields settings.

<figure><img src="../../.gitbook/assets/81717.png" alt=""><figcaption></figcaption></figure>

***

### Sort the Custom Fields <a href="#h_877aacb3cc" id="h_877aacb3cc"></a>

By default, custom fields are arranged in chronological order based on their creation time, meaning the most recently created field appears at the bottom of the list.

However, if you want certain fields to be displayed at the top for easier access, you can adjust their order.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1416110020/6f83c1d4aeed3a96469a30557b9c/57653.png?expires=1741824000&#x26;signature=61064bdf999ad7b67ba5950b082634c1c2193cae87a2b9b48173088db6c7f7a8&#x26;req=dSQmEMh%2FnYFdWfMW3nq%2BgV%2FoTpdi2%2BNMlrZDLpFAU1wNTgpuErRxzt3hT91F%0AUidpD7WeuroNStpn4vMrZPKmlHQ%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

To do this, go to Workspace > Fields, select any custom field, and update its order value to change its position.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1416108445/4f91d98fc80cb6e0ff4f3e7f7648/18592.png?expires=1741824000&#x26;signature=8759ba3f16115a1c52514dece592e86f5983f5cf41119366bab1f4d5d60c4cc2&#x26;req=dSQmEMh%2BlYVbXPMW3nq%2BgR3gMUWL9ML4CIGOs%2FvNKkiHj75j4DFjPe9lJgMv%0AS5xSPieINFUyN1742%2B2ceIOE0tQ%3D%0A" alt="" width="375"><figcaption></figcaption></figure>

You can also sort the list by the order field to view the updated arrangement.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1416114615/1dcf91237249e6dca4d77509aeb5/85978.png?expires=1741824000&#x26;signature=af93c96d12d4febc389edc908650b2d23cf285810e0e6dcea6f2e4414be037fd&#x26;req=dSQmEMh%2FmYdeXPMW3nq%2BgR9hOdVVDTgfjAPOIhkKoGlMeDDyt5CrF%2F%2FQz4OT%0A7mIynM2OpTC9mWCZyhn9sjOxWto%3D%0A" alt="" width="563"><figcaption></figcaption></figure>



