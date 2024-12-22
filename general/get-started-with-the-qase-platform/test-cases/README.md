# Test cases

{% embed url="https://www.youtube.com/watch?v=bidHMkx3OdM" %}

### What is a test case in software testing?

A test case contains all the details about our test. In Qase, a test case is a specific set of instructions and conditions that outline a test to be carried out successfully.&#x20;

It includes testing procedures, necessary inputs, execution conditions, and expected results to achieve a testing objective.

In Qase, you can define various parameters and expected outcomes of a particular testing scenario.



## Create Test Case

***

#### **a. Create a Quick test case**

Quickly create a test case by clicking the "**+ Create case**" button in a Suite, by providing a title, and add other details later if needed.

<figure><img src="../../../.gitbook/assets/Case1.gif" alt="" width="563"><figcaption></figcaption></figure>

#### b. Create a Detailed case <a href="#h_d28f22cf2c" id="h_d28f22cf2c"></a>

The second method lets you fully detail your new Test Case. Click the "+ Case" button above the Suite structure in the repository to begin.

You'll be guided in setting up your new Test Case and providing all the necessary information.

<figure><img src="../../../.gitbook/assets/Case2.gif" alt="" width="563"><figcaption></figcaption></figure>

## Test Case Properties <a href="#h_5493a9da30" id="h_5493a9da30"></a>

***

Test Case properties can be divided into several sections:

* [Basic Fields](./#h_e668c8881a)
* [Conditions](./#h_564c734a0e)
* [Tags](./#h_2e6441f7a0)
* [Attachments](./#h_f96083cf3f)
* [Parameters](./#h_1066185940)
* [Test Case Steps](./#h_8b8d83c628)

<figure><img src="../../../.gitbook/assets/case 3.png" alt="" width="563"><figcaption></figcaption></figure>

### Basic fields <a href="#h_e668c8881a" id="h_e668c8881a"></a>

You will define the following Test Case properties:

<table><thead><tr><th width="67">No</th><th width="125">Field</th><th width="594">Description</th></tr></thead><tbody><tr><td>1</td><td>Title</td><td>define the name of a test case</td></tr><tr><td>2</td><td>Status</td><td>can be either Active, Draft, or Deprecated</td></tr><tr><td>3</td><td>Description</td><td>additional details for more context about a test case</td></tr><tr><td>4</td><td>Suite</td><td>choose here which Test Suite your new case belongs to</td></tr><tr><td>5</td><td>Severity</td><td>can be either Trivial, Minor, Normal, Major, Critical, Blocker, or Not Set</td></tr><tr><td>6</td><td>Priority</td><td>can be either Low, Medium, High, or Not Set</td></tr><tr><td>7</td><td>Type</td><td>select what type of testing is applicable for your test case</td></tr><tr><td>8</td><td>Layer</td><td>pick a layer of the test case, whether it's an end-to-end, API, or a unit test</td></tr><tr><td>9</td><td>Is Flaky</td><td>if a test case is unstable, you can mark it as flaky</td></tr><tr><td>10</td><td>Milestone</td><td>select whether a test case is related to one of your Milestones, which you can create separately</td></tr><tr><td>11</td><td>Behavior</td><td>can be either Destructive, Negative, Positive, or Not Set</td></tr><tr><td>12</td><td>Automation Status</td><td>you can choose between Manual and Automated</td></tr><tr><td>13</td><td>To be Automated?</td><td>a checkbox property only available for those cases that have a "Manual" automation status</td></tr><tr><td>14</td><td>Is Muted?</td><td>checkbox marking tests as muted so their results will not affect the overall status of test runs where it can pass even if the muted test fails.</td></tr></tbody></table>

System fields can be optionally switched on and off via the fields section. Click the "Configure fields" button and select the field you want to configure. Click on the “Enable for all projects button” and then configure:

{% hint style="info" %}
You can make your own [Custom Fields](../../../administration/workspace-management/custom-fields.md) with different data types to store extra information about your test cases not included in default properties. You won't find this field If you haven't created any Custom Fields yet.
{% endhint %}



### Conditions <a href="#h_564c734a0e" id="h_564c734a0e"></a>

Here, you can outline what needs to happen before conducting the Test Case (Pre-conditions) and the actions to be taken after the Test Case is completed (Post-conditions).

<figure><img src="../../../.gitbook/assets/3722.png" alt="" width="563"><figcaption></figcaption></figure>

### Tags: <a href="#h_2e6441f7a0" id="h_2e6441f7a0"></a>

Tags are a quick way to label your test cases with values that doesn't require any preliminary configuration.

<figure><img src="../../../.gitbook/assets/99209.png" alt="" width="375"><figcaption></figcaption></figure>

### Attachments: <a href="#h_f96083cf3f" id="h_f96083cf3f"></a>

Add clarity and additional context to your Test Case by uploading images, screenshots, video snippets, or other documents.

<figure><img src="../../../.gitbook/assets/attachments.png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="success" %}
There is a **128 MB** maximum size limit for a single file that can be attached.
{% endhint %}

## [Parameters](test-case-parameters.md): <a href="#h_1066185940" id="h_1066185940"></a>

You can set up your test case to be parametrized and run it through multiple iterations during a test run, depending on the parameter values you define.

<figure><img src="../../../.gitbook/assets/99682 (1).png" alt="" width="563"><figcaption></figcaption></figure>

You have the flexibility to add multiple parameters, each with multiple values.

Once you include a parametrised case in a test run, multiple instances of it will be added to the run, each representing a specific parameter value.

<figure><img src="../../../.gitbook/assets/60091.png" alt="" width="563"><figcaption></figcaption></figure>



## Test Case Steps: <a href="#h_8b8d83c628" id="h_8b8d83c628"></a>

***

This section outlines the actions to be taken and the expected results for each step when executing a test case. For instance, when testing a software module offering GPS connectivity, you must specify the actions to perform and the anticipated outcomes.

There are two types of steps to pick from -

**a) Classic**

<figure><img src="../../../.gitbook/assets/classic.png" alt="" width="563"><figcaption></figcaption></figure>

1. **Step Action**: A specific operation or task carried out within the test case step, such as interacting with an application interface or system.
2. **Data**: Input parameters or information utilized during the execution of a test, the influences the behavior of the system under test.
   * _This field can be disabled from the project's settings, under test case -> 'Dataset"_
3. **Expected Result**: The anticipated outcome or behavior that is considered correct for the given test case step.



**b) Gherkin**

<figure><img src="../../../.gitbook/assets/gherkin.png" alt="" width="563"><figcaption></figcaption></figure>

Test Case can consist of several steps that must be performed; for every new step, hit the "**+ Add Step**" button on the bottom.

<figure><img src="../../../.gitbook/assets/add step.png" alt=""><figcaption></figcaption></figure>

#### Nested Steps <a href="#h_6cd2f4d2d2" id="h_6cd2f4d2d2"></a>

This is a list of sub-steps to be executed within a main step. This relationship forms a parent-child structure, where a step contains smaller steps within it.

To create a nested step, click on the three-dots menu of a step and select "Add child step."

<figure><img src="../../../.gitbook/assets/image (8) (1).png" alt="" width="563"><figcaption></figcaption></figure>

#### Shared Steps <a href="#h_66a5891687" id="h_66a5891687"></a>

To save time on repetitive tasks for Steps common to multiple Test Cases in a Project, consider creating Shared Steps.

Once you have at least one Shared Step in the "[Shared Steps](shared-steps.md)" view of your project, you'll find a "+ Add Shared Step" button when creating or editing a case.

<figure><img src="../../../.gitbook/assets/61139.png" alt="" width="563"><figcaption></figcaption></figure>

When configuring a Case Step, you can customize it using the buttons beside the "Expected result" field:

<figure><img src="../../../.gitbook/assets/10935.png" alt="" width="563"><figcaption></figcaption></figure>

1. You can create a Shared step / or turn a Shared step into a Regular step.
2. You can duplicate/clone a step.
3. You can edit a Shared step.
4. You can add a nested step.
5. You can delete a step,
6. You can attach files from your existing files in Qase or your computer.



### Test Case Actions <a href="#h_91f8dfe2ce" id="h_91f8dfe2ce"></a>

***

Once you have filled in all the information about your Test Case, you can:

<figure><img src="../../../.gitbook/assets/12209.png" alt="" width="375"><figcaption></figcaption></figure>

* [_Send to review_](test-case-review.md)_:_ in this case, a new Test Case Review request will be created, and a person responsible for reviews will then decide on a submitted Test Case.
* _Save your Test Case_
* _Save and create another_
* _Cancel:_ exit Test Case creation; your changes will not be saved.

#### **Find your test case after saving:**

After saving the Test Case, it will be visible in your Repository structure alongside Test Suites and other Test Cases.

The Test Case will receive an automatically assigned code, combining the Project Code with a number (e.g., "DEMO-9," where "DEMO" is the project code, and "9" indicates the ninth Test Case created in this Project).

<figure><img src="../../../.gitbook/assets/84096.png" alt="" width="563"><figcaption></figcaption></figure>

When you click on a Test Case in the Repository view, a sidebar with a summary will appear on the right side of the screen. You can view the Test Case properties and access options to Edit, Clone, or Delete it.

<figure><img src="../../../.gitbook/assets/4889.png" alt="" width="563"><figcaption></figcaption></figure>

**Restoring deleted cases**

If you have deleted a Test Case, it will reside in the [Trash Bin](trash-bin.md) located in the three-dots-menu:

<figure><img src="../../../.gitbook/assets/44915.png" alt="" width="563"><figcaption></figcaption></figure>

From the Trash Bin, you can restore a previously deleted Test case:

<figure><img src="../../../.gitbook/assets/56905.png" alt="" width="563"><figcaption></figcaption></figure>

## Filters <a href="#h_8861baa88d" id="h_8861baa88d"></a>

***

When in the Repository view, you can apply Filters to find Test Cases with specific properties:

<figure><img src="../../../.gitbook/assets/40351.png" alt="" width="563"><figcaption></figcaption></figure>

In the example below, there are two filters applied - Cases that are of Normal severity and that are Manual:

<figure><img src="../../../.gitbook/assets/30293.png" alt="" width="563"><figcaption></figcaption></figure>

To look up a test case by name, you can use the search box - start typing the name of a test case, and you will be shown matching test cases:

<figure><img src="../../../.gitbook/assets/53194.png" alt="" width="563"><figcaption></figcaption></figure>

## Bulk actions <a href="#h_7bc690437f" id="h_7bc690437f"></a>

***

Once you have multiple Test Cases, you can perform bulk edits. Check the boxes of several Test Cases to:

* Edit multiple cases' properties:

<figure><img src="../../../.gitbook/assets/Jan-16-2024 19-47-41.gif" alt="" width="563"><figcaption></figcaption></figure>

* Perform an Express [Test Run](https://help.qase.io/en/articles/5563702-test-runs) of selected Test Cases:

<figure><img src="../../../.gitbook/assets/run cases.gif" alt="" width="563"><figcaption></figcaption></figure>

* Delete Test Cases in bulk; when attempting to delete multiple Cases, you have to type "CONFIRM" into the field to prevent accidental deletion.

<figure><img src="../../../.gitbook/assets/bulk delete.gif" alt="" width="563"><figcaption></figcaption></figure>

<details>

<summary>NB: This behavior is determined by a setting in project settings and can be switched on/off:</summary>

![](<../../../.gitbook/assets/76755 (1).png>)

</details>
