---
title: Defects
slug: defects-1
hidden: true
createdAt: '2023-02-21T19:34:57.238Z'
updatedAt: '2023-02-21T19:34:57.238Z'
---

# Defects

### How to create a defect?

In Qase, there are two ways to create a defect: you can create one on the spot, at will, for any issue that is not necessarily connected to a particular test case or test run. Another option is to file a defect upon failing a test case during a run.

#### Option 1: Creating a defect independently

To do this, click on "Create New Defect" in the "Defects" section and add all necessary details such as Defect Title, Actual Result, and Severity, fill out any custom fields applicable to Defects, and optionally add attachments. This type of defect is not connected to any test case or test run. However, it can be marked as "In Progress" (and then, consecutively, Resolved), Invalidated, or Edited.

You can also tie any defects filed during test runs to an existing defect you created manually.

This can be helpful when you are aware of the issues beforehand, even before performing a single test run, and want to document them in advance.

#### Option 2: During a test run, some of your test cases will likely fail.

To set up your Project, remember the "Fail case on step fail" setting:

* If this setting is on, failing a single step in a case during a test run will cause the entire test case to fail. You will then be prompted to create a new Defect.
* If this setting is off, failing a single step in a case will not cause the entire test case to fail. You can continue with other steps while still being prompted to create a Defect only if you fail the entire test case.

How to create a Defect:

* Mark a Test Case as "Failed".
* You will be prompted to a Run result window, where you can add comments, record time spent on the test case, attach files, and create/attach a defect.
* With the checkbox checked, you will be prompted to fill out other remaining Defect properties, including any custom fields you created. You can choose whether to create a new Defect or attach an existing one to the issue you found. You can also change its title, severity, and custom fields' values, and send a connected issue to other integrated third-party software systems.
* A new Defect will be created from the test run result and saved under the "Defects" section and the “Defects” tab of your test run.

Note: Defects viewed in a test run will show only defects filed in that test run. You can find all defects filed in a project under the “Defects” section.
