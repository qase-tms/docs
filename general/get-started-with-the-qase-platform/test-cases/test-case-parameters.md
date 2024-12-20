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
