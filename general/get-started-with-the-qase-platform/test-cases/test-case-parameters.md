# Test Case Parameters

### What are parameters in software testing?

In your testing process, Parameters allow you to capture variables that can be reused across [multiple executions](../create-a-test-run/test-run-dashboard.md) of the same [Test Case](./#what-is-a-test-case-in-software-testing). This eliminates the need to create separate test cases or duplicate steps for different conditions.&#x20;

{% embed url="https://youtu.be/Vtyza2ubkbk" %}
Parameters explained using a common testing scenario.&#x20;
{% endembed %}

### How Parameters help? <a href="#h_feaec674fe" id="h_feaec674fe"></a>

Consider a scenario where you need to test the sign-in functionality of a web application under various conditions. For each user, you’ll need to test each website twice under different conditions (VPN, WiFi, HTTPS, SSO, Cookies), both enabled and disabled.

**Parameter 1**

| <mark style="color:yellow;">Browser</mark> | Chromium | Firefox | Safari | Microsoft Edge |
| ------------------------------------------ | -------- | ------- | ------ | -------------- |

**Parameter 2**

| <mark style="color:yellow;">Website</mark> | qase.io | blog.qase.io | help.qase.io |
| ------------------------------------------ | ------- | ------------ | ------------ |

Group 1 is a **Secure network**; Group 2 is an **In-secure network**.

| <mark style="color:yellow;">is on VPN?</mark> | <mark style="color:yellow;">is on WiFi?</mark> | <mark style="color:yellow;">is HTTPS?</mark> | <mark style="color:yellow;">Using SSO?</mark> | <mark style="color:yellow;">Cookies Accepted?</mark> |
| --------------------------------------------- | ---------------------------------------------- | -------------------------------------------- | --------------------------------------------- | ---------------------------------------------------- |
| Yes                                           | No                                             | Yes                                          | No                                            | No                                                   |
| No                                            | Yes                                            | No                                           | Yes                                           | No                                                   |



### Create a test case with Parameters - <a href="#h_4ecd8db223" id="h_4ecd8db223"></a>

***

Go to your repository, to select an existing test case, or create a new one.

<figure><img src="../../../.gitbook/assets/9019.png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (22).png" alt="" width="563"><figcaption></figcaption></figure>

When you either create or edit an existing test case, you can scroll down to find the "Parameters" section and simply click on the "+ Add Parameter' button.

<figure><img src="../../../.gitbook/assets/56273.png" alt="" width="563"><figcaption></figcaption></figure>

**Then**, proceed to add the following test case steps

* Check the network condition specified (Secure/ Insecure)
* Launch the specified browser.
* Navigate to the specified website.
* Enter the login credentials for the specified site.
* Click the "Sign In" button.



## Executing a Parameterized test case - <a href="#h_f60972ba23" id="h_f60972ba23"></a>

***

When a test case with Parameters is included in a test run, it generates multiple instances of the test case, each corresponding to a specific combination of parameter values.

<figure><img src="../../../.gitbook/assets/71312.png" alt=""><figcaption></figcaption></figure>

For example:

* Test 1: Browser = `Chromium`, Website = `https://www.qase.io`, Secure = `VPN = Yes, WiFi = Yes, HTTPS = Yes, SSO = Yes, Cookies = Yes`\
  ​
* Test 2: Browser = `Chromium`, Website = `https://blog.qase.io`, Secure = `VPN = Yes, WiFi = Yes, HTTPS = Yes, SSO = Yes, Cookies = Yes`

(and so on, until all combinations are covered)

* Test 24: Browser = `Microsoft Edge`, Website = `https://help.qase.io`, Insecure = `VPN = Yes, WiFi = Yes, HTTPS = Yes, SSO = Yes, Cookies = Yes`

With single parameters, the total number of test cases is the product of the number of values for each parameter. For example, with two parameters having 3 and 4 values, you get (3\*4) 12 test cases.

Given the network security conditions (Secured and Unsecured), it’s impractical to list each component as a separate parameter. Instead, all components are either enabled in a secured network or disabled in an unsecured network. This is where Parameter Groups become useful.



### How is a Parameter group different from a single parameter? <a href="#h_ade6ec7615" id="h_ade6ec7615"></a>

To further streamline the testing process, you can group related parameters into "Parameter Groups." For example:

* Network security: Is on VPN, Is on WiFi, Is HTTPS, SSO sign-in, Cookies enabled
* Account status: is Active; has a custom role; is a regular user, is Owner

Parameter Groups are useful when not all combinations of parameters are relevant or meaningful. For instance, with “Account Status” parameter, a combination of “not active” and “not Owner” might not exist in your system or be applicable.

In such cases, Parameter Groups help you focus only on practical and realistic combinations, eliminating unnecessary tests. This ensures that your testing is efficient and covers only meaningful scenarios.

In our example, although we initially had 12 combinations for the single parameters, each of these needs to be tested on both Secure and Insecure network groups. As a result, the total number of test cases in the run will now be 24.

{% hint style="info" %}
In a test run, the total number of parameter combinations for a case cannot exceed 1,024.
{% endhint %}



### Find your parameter siblings from the Run wizard <a href="#h_01f891c7fd" id="h_01f891c7fd"></a>

In the Test Run dashboard, selecting a parameterized test case will display a ‘siblings’ tab. This tab shows copies of the test case for all other parameter values associated with the selected case.

<figure><img src="../../../.gitbook/assets/64217.png" alt="" width="563"><figcaption></figcaption></figure>



## Shared Parameters <a href="#h_b35fcc1160" id="h_b35fcc1160"></a>

Shared Parameters allow you to create reusable parameters at the workspace level that can be applied across multiple test cases and projects. Instead of creating the same parameters repeatedly in individual test cases, you can now define them once and share them wherever needed.

If you change a shared parameter, these changes will automatically apply to all test cases using this parameter.

### Creating Shared Parameters <a href="#h_55a9f4841c" id="h_55a9f4841c"></a>

1.  From the workspace , go to "Shared Parameters" and create your Single or Group shared parameters.\


    <figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1657992629/a5248d070c8f8ebac51fd296f93b/image.png?expires=1754654400&#x26;signature=275211fda4e279011a93a7590d672b4aa3c3fdaee575477ee8b58a981e790dcb&#x26;req=dSYiEcB3n4ddUPMW3nq%2BgZL0d93D2yPf7zyzCYVg%2Ft1RfRmwzsLdPkFnu%2FTv%0AaQH6j7DXSlEyLNgYaZXuYTrN7uI%3D%0A" alt="" width="563"><figcaption></figcaption></figure>


2.  You can select which projects should have access to this shared parameter\
    ​

    <figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1657993435/155ff506b5abb9b651eef3f62cfe/image.png?expires=1754654400&#x26;signature=fd21b2e077087cb428ba5a50390313de3f0eb19efc23abc473e7a5fb6f8d8e93&#x26;req=dSYiEcB3noVcXPMW3nq%2BgY%2BLnnWUNTffcrT%2FkcmbwuTlobQ%2B9t6hlMFRKJ%2BE%0AUGeaepNfF0C5hIuwFvdT5IrC3iQ%3D%0A" alt="" width="563"><figcaption></figcaption></figure>


3. And, save your shared parameter

Once created, you'll see your shared parameters listed with the following information:

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1657993811/ecd34d69660f3dfc84d582efde93/image.png?expires=1754654400&#x26;signature=63990c90f164a255a9a7f3785753754c20a854acb44b30dc4a9bf34ad3eab6ab&#x26;req=dSYiEcB3noleWPMW3nq%2BgRiIjmzHpnLlrB0PHC5waVVciiSD6ivbMo5mPThC%0AJviefR53F%2BnhZjQPgaxIOWlFKms%3D%0A" alt=""><figcaption></figcaption></figure>

* Parameter name and type (single or group)
* Which projects have access
* Number of test cases currently using the parameter



### Attaching Shared Parameters to Test Cases <a href="#h_f9202a45f6" id="h_f9202a45f6"></a>

When editing or creating a test case, you'll notice the Parameters section now includes separate options:

* Single Parameters (local to the test case)
* Group Parameters (local to the test case)
*   Shared Parameters (workspace-level parameters)



    <figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1657994425/2b5e5a204fe72abadde3396a20fc/image.png?expires=1754654400&#x26;signature=0b5dc55bed612fb6dffd9b6239c7547eeb15251bf68dc38cf16ccc091b2785f3&#x26;req=dSYiEcB3mYVdXPMW3nq%2BgTDLoiqrQefwj%2B8Uy%2F2RMAZ47NvrZY9kuxS760dU%0A9w9DICRHrJyI4qOU10xuMRiD02M%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

\*\*Note\*\*: Shared parameters cannot be edited directly from within individual test cases. You can only attach or detach them. All modifications must be made from the main Shared Parameters section.



### Deleting Shared Parameters <a href="#h_a16e7acaa6" id="h_a16e7acaa6"></a>

When deleting a shared parameter, you have two options:

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1657995096/0e53602807fd4ba7f07226fd27de/image.png?expires=1754654400&#x26;signature=e837a3eec2a4fefc0bc9bcd44fd46126024964e51adf5ca4d2136693afb321d2&#x26;req=dSYiEcB3mIFWX%2FMW3nq%2BgephUzyCW4wHXLtRl1GJsA5rLD4xo0wuZMtcdhvC%0APsJg3q5DZJ8nQHOy%2BoShsM6wxoQ%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

1. Convert to Local Parameters: Transform the shared parameter into individual local parameters within each test case.\
   ​
2. Delete from All Test Cases: Completely remove the parameter from all associated test cases.

### Tracking Usage of your shared parameter <a href="#h_e3a86b5228" id="h_e3a86b5228"></a>

You can view the usage of a shared parameter from the Edit screen by navigating to the Usage tab. This tab provides a detailed overview of:

* All projects that have access to the shared parameter.
* The number of test cases in the repository that use the shared parameter.
* The number of test cases submitted for review that include the shared parameter.

This allows you to quickly understand where and how your shared parameters are being utilized across your projects.

<figure><img src="../../../.gitbook/assets/86794.png" alt="" width="563"><figcaption></figcaption></figure>
