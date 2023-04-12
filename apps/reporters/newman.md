# Newman

### What is Newman?

Newman is a command-line Collection Runner for Postman. It enables you to run and test a Postman Collection directly from the command line. It's built with extensibility in mind so that you can integrate it with your continuous integration (CI) servers and build systems.

To pass the results of your Newman executions, you need to install the Newman app.

1.  Navigate to the[ Apps page](https://app.qase.io/apps) and switch to the "Reporters" section, then click the "Newman " card:

    [![](https://downloads.intercomcdn.com/i/o/658632364/bd6a3e4f7dd618681cecd473/image.png)](https://downloads.intercomcdn.com/i/o/658632364/bd6a3e4f7dd618681cecd473/image.png)
2.  Click "Activate":

    [![](https://downloads.intercomcdn.com/i/o/658632780/eae35998f64a8c2a1e7bf26e/image.png)](https://downloads.intercomcdn.com/i/o/658632780/eae35998f64a8c2a1e7bf26e/image.png)
3.  Switch to "Access Tokens" and generate an API token that the Newman app will be using:

    [![](https://downloads.intercomcdn.com/i/o/658633354/358d17de9e00a31974ae5255/image.png)](https://downloads.intercomcdn.com/i/o/658633354/358d17de9e00a31974ae5255/image.png)
4.  Click "Guide" to access the [instruction](https://github.com/qase-tms/qase-javascript/tree/master/qase-newman) on adding the Newman reporter to your automation flow:

    [![](https://downloads.intercomcdn.com/i/o/658634354/484eccc47cfa3dfdf35cab75/image.png)](https://downloads.intercomcdn.com/i/o/658634354/484eccc47cfa3dfdf35cab75/image.png)

Once the Newman app is installed, any test cases, test runs, and test results created and submitted will appear with the Newman as the author of said cases, runs or results (instead of a specific user whose API token has been used). [Slack notifications](https://help.qase.io/en/articles/6417209-slack) will also appear with the Newman app as the author.
