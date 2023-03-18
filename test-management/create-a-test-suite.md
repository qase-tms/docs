# Test suites

### What is a test suite in software testing?

A test suite acts like a folder where we store our test cases organized by sections and subsections. You can create several test suites. For example, Functional and Non-Functional test suites or anything else that should be treated as a separate group of tests.

{% embed url="https://youtu.be/Gz5gfZ4_7WM" %}

### **To create a test suite:**

1. On the "Repository" page, click the "Create new suite" button, or click "+ Suite" next to the search bar at the top.
2. A popup window titled "Create Suite" will appear. Now let's fill in the fields:
   * Suite Name: give your Test Suite a descriptive name that allows you to unequivocally define which domain or area of development it will cover. Suite Name is the only mandatory field to create a Suite - other fields are optional and can be filled at a later stage or left empty.
   * Parent Suite: it is possible to have a multi-level hierarchy of Test Suites, so if a Suite you are configuring will be a part of a larger scope of testing scenarios, you can put it into a higher-level Parent Suite.
   * Description: provide additional details and context regarding which Test Cases should belong to a Test Suite.
   * Preconditions: describe the steps that should be completed before you can proceed with Test Cases from the newly created Suite.
3. To create a test suite, click "Create".
4. The repository will now display the newly created test suite.

Once you have created one or several test suites, your repository will reflect how they are structured and related to each other.

### Test suites controls

While in Repository view, hovering over "Test Suite" reveals several controls:

* _Collapse / Expand:_ Clicking on the name of the test suite collapses or expands it.
* _Create Case / Create Suite:_ Clicking on the "+" icon opens a menu with options to "Create Suite" or "Create Case."
* _Edit Suite:_ Clicking on the pencil icon allows you to edit the suite itself.
* _Clone Suite:_ Clicking on the two pages icon allows you to clone the suite. You can choose the project to which you want the suite cloned, its parent suite, clone strategy, and prefix. You also have the option to clone the suite with its children (suites and cases).
* _Delete Suite:_ Clicking on the trash can icon lets you delete the suite. Once deleted, you cannot restore the suite from the "[Trash Bin](https://docs.google.com/document/d/177K4qifjuaqi\_XumMX6ZBj81x-NE1j5U3eSY6ldOC6A/edit)."

### Navigation in suite structure

There are three suite tree layouts that you can use to move around your suite structure. You can switch between these layouts by using the "Views" dropdown menu located in the top-right corner of the repository interface.

* _Nested Tree view:_ shows all of the Suites in your project; use the Suite Tree sidebar to navigate between them.
* _Folders view:_ shows only the Test Suite and Test Cases in focus, while to navigate to a different Suite, you need to select it from the sidebar. This layout is better for massive structures with complicated hierarchy.
* _Mind Map view:_ displays all the suites and test cases within a project in the form of a mind map. Also allows you to create cases or suites by clicking on the + icon. You can also alter the hierarchy of display by dragging the suite up or down. You can also move a test case from one suite to another. Additionally, clicking on the case will allow you to update its title.

In both the Nested Tree view and the Folders view, you can click on the "..." menu icon to Edit, Close, Select and Unselect all, Create Suite, Create Case, and Delete.



