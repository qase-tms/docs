---
description: An explanation of Cypress and how to install the Cypress app in Qase.
---

# Cypress

{% hint style="info" %}
Documentation for Qase API and Reporters is at [https://developers.qase.io/docs/](https://developers.qase.io/docs/)
{% endhint %}

### What is Cypress?

Cypress is a purely JavaScript-based front-end testing tool built for the modern web. It aims to address the pain points developers or QA engineers face while testing an application. Cypress is a more developer-friendly tool that uses a unique DOM manipulation technique and operates directly in the browser.

### How to install Cypress?

To pass the results of your Cypress executions, you need to install the Cypress app.

1.  Navigate to the Apps page and switch to "Reporters" section, then click the "Cypress " card:\


    <figure><img src="https://downloads.intercomcdn.com/i/o/657803862/db0a6fcd4f55339477261d20/image.png" alt=""><figcaption></figcaption></figure>
2.  Click "Activate":\


    <figure><img src="https://downloads.intercomcdn.com/i/o/657804580/fb1de9c0c9c0a4cb01f1d338/image.png" alt=""><figcaption></figcaption></figure>
3.  Switch to "Access Tokens" and generate an API token that the Cypress app will be using:



    <figure><img src="https://downloads.intercomcdn.com/i/o/657806388/b06e8f271a650cce855544dc/image.png" alt=""><figcaption></figcaption></figure>
4.  Click "Guide" to access the [instruction](https://github.com/qase-tms/qase-javascript/tree/main/qase-cypress) on adding the Cypress reporter to your automation flow:\


    <figure><img src="https://downloads.intercomcdn.com/i/o/657805778/49ad73c2d26cfe590fe8cee5/image.png" alt=""><figcaption></figcaption></figure>

Once the Cypress app is installed, any test cases, test runs, and test results created and submitted will appear with Cypress as the author of said cases, runs or results (instead of a specific user whose API token has been used). Slack notifications will also appear with the Cypress app as the author.
