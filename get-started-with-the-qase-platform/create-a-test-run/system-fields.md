# System fields

### **How to Configure Fields**

You can access the fields section in multiple ways:

* Click on “Fields” on the Workspace page
* Click on “Configure fields” when creating or editing a test case.

To turn system fields on or off, follow these steps:

1. Click the "Configure fields" button
2. Select the field you want to configure
3. Click on the “Enable for all projects button”
4. Configure the field as desired.

### **Values**

You can change the values of system fields if you're on the Startup, Business, or Enterprise plans. These fields include:

* _Conditions:_ Here you can say what needs to happen before (_Pre-conditions_) and after (_Post-conditions_) the Test Case is performed.
* _Tags:_ A quick way to label your test cases with values that doesn't require any preliminary configuration.
* _Custom Fields:_ It's hard to know what unique parameters or properties your Test Case will require. You can create your own Custom Fields with different data types to store any extra information about your test cases that isn't covered by the standard options. If you haven't created any Custom Fields yet, you won't see this section in the Test Case configuration.
* _Attachments:_ Upload images, screenshots, video snippets, or other documents to your Test Case to make it clearer or give more context. You can't attach a single file that's larger than 32MB.
* _Parameters:_ You can set up your test case to be parametrized and to be performed during a test run in several iterations, depending on how many parameter values you define. You can also add multiple parameters and have multiple values within each parameter that you create.

If you add a parametrized case to a test run, there will be several instances of it in the run, each representing a specific parameter value.

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

* Test Case Steps: This section outlines the actions required to perform a test case and the expected results for each step. For instance, if I want to test a software module that provides GPS for connectivity, I'll need to explain which action needs to be performed and what the expected outcome is. You can choose between two types of steps: Classic or Gherkin. Each test case can have multiple steps that must be completed. To add a new step, click the "+ Add Step" button at the bottom.
