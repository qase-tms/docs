# Test case parameters

### What are parameters in software testing?

Testers can record the variables in the testing process as parameters. This enables them to use the same test case for multiple executions, instead of creating distinct test cases or multiple sets of steps.

{% embed url="https://youtu.be/ITkLO7T-Hgw" %}

### How do parameters work?

Once you have parameters in a case when such a case is added to a test run, it will get split into multiple identical copies of the same test case - one per each parameter value specified:\


<figure><img src="https://downloads.intercomcdn.com/i/o/597370856/23f5da102d91d07f4af21ccd/image.png" alt=""><figcaption></figcaption></figure>

### Example

Consider evaluating a web application's logon process, for instance. You could take the following actions:

1\. Launch your computer's browser

2\. Enter the website’s URL

3\. Type the appropriate fields for the user name and password.

4\. Press the Sign In button.

Consider that you wish to conduct this test with various browsers. Test parameters labelled browser can be created and incorporated into the test case when setting up a test case, as opposed to developing separate test cases with similar data.

### How to create a parameter?

Here’s how you can create a parameter while creating a new test case or editing an existing one (only one parameter can be created per test case).

#### New Case: <a href="#h_ff8229f5ff" id="h_ff8229f5ff"></a>

1. Navigate to the Repository
2. Click on “+ Case”
3. Fill in the required fields
4. Click on “+ Add Param”
5. Enter a title, eg. Browser and hit Enter
6. Add the first parameter, eg. Chrome
7. Hit Enter or click on “+ Add value”
8. Add another parameter, eg. Firefox
9. Repeat step 7 until you’ve added all required parameters
10. Proceed to create the Test Case

<figure><img src="https://downloads.intercomcdn.com/i/o/627751403/c331fb94d43db99b18a8523f/GIF+1.gif" alt=""><figcaption></figcaption></figure>

#### Edit existing test case: <a href="#h_ed06bedcee" id="h_ed06bedcee"></a>

1. Navigate to the repository
2. Click on the test case you require
3. Click on “Edit” in the sidebar
4. Fill in the required fields
5. Click on “+ Add Param”
6. Enter a title, eg. Browser, and hit Enter
7. Add the first parameter, eg. Chrome
8. Hit Enter or click on “+ Add value”
9. Add another parameter, eg. Firefox
10. Repeat step 8 until you’ve added all required parameters
11. Proceed to save the Test Case

<figure><img src="https://downloads.intercomcdn.com/i/o/627753741/c60d610413a1419676cdb479/GIF+1.gif" alt=""><figcaption></figcaption></figure>

You can also create several parameters with their respective parameter values.

### One more example

Consider that you wish to conduct the above-mentioned test with various browsers along with operating systems. You could take the following actions listed above and then do the next to add the operating system parameter with its values:

1. Fill in the first parameter along with its values as explained above.
2. Click on “+ Add Param”
3. Enter a title, eg. OS, and hit enter
4. Add the first parameter, eg. Windows
5. Hit enter or click on “+ Add value”
6. Add another parameter, eg. MacOS
7. Repeat step 5 until you’ve added all required parameters
8. Proceed to save the test case

<figure><img src="https://downloads.intercomcdn.com/i/o/627758047/7a86d48b4f443bc057491892/GIF+1.gif" alt=""><figcaption></figcaption></figure>
