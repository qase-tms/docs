# XCTest

{% hint style="info" %}
Documentation for Qase API and Reporters is at [https://reporters.qase.io/](https://reporters.qase.io/)
{% endhint %}

### What is XCTest?

XCTest is a testing framework that allows you to create and run UI tests, unit tests, and performance tests for your Xcode projects in Swift and Objective-C languages. It is pre-built with Xcode.

### How to install XCTest?

To pass the results of your XCTest executions, you can use our [Qase CLI](./) tool.

1.  Navigate to the[ Apps page](https://app.qase.io/apps) and switch to "Reporters" section, then click the "XCTest " card:



    <figure><img src="https://downloads.intercomcdn.com/i/o/657822683/9295ef3b031b7365b9ed7080/image.png" alt=""><figcaption></figcaption></figure>
2.  Click "Activate":\


    <figure><img src="https://downloads.intercomcdn.com/i/o/657823776/dddaaec4775f1edf6b9134ca/image.png" alt=""><figcaption></figcaption></figure>
3.  Switch to "Access Tokens" and generate an API token that the XCTest app will be using:



    <figure><img src="https://downloads.intercomcdn.com/i/o/657829090/57a1a2ef00b6262b97869485/image.png" alt=""><figcaption></figcaption></figure>
4.  Use the [Qase CLI tool](https://github.com/qase-tms/qasectl) to publish your XCTest results.\


    <figure><img src="https://downloads.intercomcdn.com/i/o/657828405/7c188061dad7ee1b58c5ae4d/image.png" alt=""><figcaption></figcaption></figure>

Once the XCTest app is installed, any test cases, test runs, and test results created and submitted will appear with the XCTest as the author of said cases, runs or results (instead of a specific user whose API token has been used). Slack notifications will also appear with the XCTest app as the author.
