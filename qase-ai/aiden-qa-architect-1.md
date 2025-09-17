# AIDEN - QA Architect

{% embed url="https://www.youtube.com/watch?v=Mcx-hx7D4GA" %}

Before reading this article, please check:

* ### [AIDEN - Test Advisor](broken-reference) <a href="#h_f3707b42f6" id="h_f3707b42f6"></a>

While Manual testing has been the cornerstone of software quality for decades, it is slow, costly, and error-prone. And, traditional test automation requires deep technical expertise, extensive infrastructure, and ongoing maintenance — and these are barriers that prevent many teams from adopting it effectively.

AIDEN eliminates these challenges by allowing users to create, execute, and maintain automated tests using natural language instead of working with code.

By leveraging Generative AI, AIDEN transforms test descriptions into executable test scripts in Qase Cloud, runs them in parallel across multiple browsers.

{% hint style="info" %}
With AIDEN, you can analyse your repository, generate automated test code from your manual test cases, and execute the tests in Qase Cloud.
{% endhint %}

e Cloud.

Advantages:

* No Coding Skills Required: Leverage powerful test automation without programming expertise.
* User-Friendly Interface: Simplified testing processes with an intuitive and accessible interface.
* Time Efficiency: Quickly convert manual tests to automated scripts with minimal effort.

***

## AIDEN - QA Architect <a href="#h_c1c01a4ff1" id="h_c1c01a4ff1"></a>

Once our test cases have been analysed, we can proceed to automating them.

### a) Convert an existing Manual Test <a href="#h_d41584fd98" id="h_d41584fd98"></a>

Open any test case, and click the 'Automate with AI' button to begin:

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1729687024/f7b33cd84868d41ed1802be14b81/83618.png?expires=1758218400&#x26;signature=e03f9913619c83f15508e5e96ebdbf63337e5433c3f480b473240dea4af1a8ef&#x26;req=dSclH892moFdXfMW3nq%2BgcNWu1VX8e97tc4JejCgWvnsFcalgJ1gLCiY5qNx%0ARO3XUE%2FHqQQ8oV%2B2%2FQ1us6Pe6X4%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Adding the environment <a href="#h_773e5eb449" id="h_773e5eb449"></a>

Your tests will run at a specific domain, so let's add the host environment:

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453819358/b0e5ffc24e353ddf2dbc223465f4/43433.png?expires=1758218400&#x26;signature=a5fda3d6039e49e640fb1c7379cd857e713958c9828720edc68f04e0852af7b7&#x26;req=dSQiFcF%2FlIJaUfMW3nq%2BgTuUutknA1XtZZ29GP0tiEYwZd%2FfEgd6VUO6kjbQ%0A3400C0f0Ba%2Bb9RuBdqe7AeoJ62g%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

If your host environment is not accessible from the public internet, you can help Qase tunnel to your private environment, here's a script that will help you set it up:

👉 [https://github.com/qase-tms/qase-frp](https://github.com/qase-tms/qase-frp)

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453849303/823336b6e880a98fd0af6ac91043/82820.png?expires=1758218400&#x26;signature=c9453d27115e79bc1a249c2c1649b4e57dfd5b62e0dc096b5000844c0fc3aee2&#x26;req=dSQiFcF6lIJfWvMW3nq%2BgVRNpDu0uoudUMLW1S%2FTPRX9UQN7V2yEOcc8TQ%2FL%0AIHLzyCHnejtDEWcnYpw6OxqDcI8%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Authorization <a href="#h_df8ae74eb6" id="h_df8ae74eb6"></a>

Most of test cases generally require authorization as a precondition. You can add your authorization steps and use them when starting auto-test generation.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453860286/0bc2dc049a06af3ca59bfd0e0a08/12279.png?expires=1758218400&#x26;signature=a49edb9669bc630ee56c600d63b08abbab5c3b99ea9a9f5ccfe47c221ce95f7c&#x26;req=dSQiFcF4nYNXX%2FMW3nq%2BgV4ZksrWG7%2BGbPwyjJdSL1r5UjsDyzsHY52iUy6M%0A0lQMaJ7EleDy%2FlxQxyKIehJQErA%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453851884/d6f6e33ef0f5211c45426484e80b/63280.png?expires=1758218400&#x26;signature=bfcb7df7a6a54afa99bd44936dd64f8707a1c9126514d58aea3d83627aa688b3&#x26;req=dSQiFcF7nIlXXfMW3nq%2BgcqltgfZwxv6sc9iCVRR68U5fT6Cg2Ra8QRTFBIQ%0ANNF39LYOsMORqcAcJ67SCg1J3YQ%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Generation <a href="#h_469592a650" id="h_469592a650"></a>

You can monitor the status and view the test case that is being used for generation at the top.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1729691547/d584c65ffcd48a3ca65939ffb92a/50274.png?expires=1758218400&#x26;signature=f578fe3ab319fda912aa7ee049655e79aaef751190f95748c8c29cd1137b9f40&#x26;req=dSclH893nIRbXvMW3nq%2BgZvNn24JHD7aIkNLuJjtGhpyZi3L2oc4MNn%2BdsVF%0AwCk%2FawllENr8CMjEZddi0LIe%2B4g%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

The generator works by first breaking down your manual test case steps into proper actionable steps.

A 'Success' or 'Failure' message is displayed for each step, along with a screenshot to communicate progress.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1470743545/4359dd4a2b9c9f23f89de97eb276/start+generation.png?expires=1758218400&#x26;signature=2f24be7d8f6ee2fe8e0aa7fb2c63e4131a4b07401a618eb05796ca39e99c9f44&#x26;req=dSQgFs56noRbXPMW3nq%2Bga3SupQiz5yHIux0wI2jma%2F931DFNTwrHoMTjCNv%0AVSgwTtAR2POqOsjU7hSRjEZRN%2Fc%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Edit Steps <a href="#h_51e4d874c7" id="h_51e4d874c7"></a>

If generation fails for a step, the status is updated as 'Error' and the particular steps with the problem will have the Error description.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1470744391/0415e8dc900c1198c16d617d3c35/error+step+final+edit.png?expires=1758218400&#x26;signature=88327ad9a0fbc7f46b7f25f4a684d54ad146a83a043896bd38aa1cea6292835a&#x26;req=dSQgFs56mYJWWPMW3nq%2BgXU1Sr91tv8ONtbKwGzuuVciODkckiWZefi3gsEJ%0AY4%2FitmVjIIelP5jPPGqEqRZ%2F%2FA8%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

You can help AIDEN by editing the particular step. Click 'Edit steps' and just correct the step text in natural language.

You can also delete steps that are not needed, or even edit steps that are successfully generated if you need to change something.

Click 'Regenerate' and AIDEN updates the steps. If you edit a step that is not generated yet, it will simply update the step's text.

If edits are made to a step that is already generated, it'll restart generation from that step.

#### Action Editor <a href="#h_c28b4a518d" id="h_c28b4a518d"></a>

For scenarios where the error is a bit complicated, for example, if an element is not recognized as a button, you can use the JSON Action Editor to debug the step.

Follow the link below to understand how the action editor works.

👉 [https://help.qase.io/en/articles/10705702-guide-action-editor](https://help.qase.io/en/articles/10705702-guide-action-editor)

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453892326/b00ac717e960aca5a15607c2c689/27133.png?expires=1758218400&#x26;signature=13a90c67a074fbe1bea0d942239469ddf6e2df763c96c96fc622a7d0f6339816&#x26;req=dSQiFcF3n4JdX%2FMW3nq%2Bgde0wOuLEmX3%2B7QTXZ9dV8jytsxc3XQrf7xbsBeq%0AXyuQpBQShnOUkqEBorc%2BrvjN%2Bk8%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Notification widget <a href="#h_5f346667f9" id="h_5f346667f9"></a>

If you navigate away, to a different page in the middle of the generation. You can always check the progress from AIDEN's notification widget.

If the generation is successful, you can find the test case from the "For Review" tab.

Generation can also be paused. There's a tab to view all the test cases that are paused previously.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1454007028/12d169d4812c0139359d562dbc4f/notiifcation+widget.png?expires=1758218400&#x26;signature=67479888289fc2aa8704db5612f6c074f5a7d73358eda706cdc310c91564a4ad&#x26;req=dSQiEsl%2BmoFdUfMW3nq%2BgRbSLglogBhbsSVbZ1laKxapueF4%2FKhiajQtnckV%0ANxm2aDcQc%2B98iphrZk1YQfObZCo%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Review and Save <a href="#h_e18686fad3" id="h_e18686fad3"></a>

Once all test steps are successfully generated, the entire execution can be reviewed from the final step's attachment.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1470775569/0b20416fbd231c57a9ca127b8269/review+video+and+save.png?expires=1758218400&#x26;signature=8b21ecd1a9c465b1c11a31463a1821639552e3cc39d1f723bec97b6a5236f295&#x26;req=dSQgFs55mIRZUPMW3nq%2BgWXq0HV%2BmyYFXmWrp4DjJ7isujtbdQpyMmMgzrgk%0Ax1xv84%2F1Cvv7qicJ2yEkLU%2BnGLY%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Click 'Save' to complete the generate and save the test case to the repository. You can differentiate this test case from the rest of the manual test cases with this symbol.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453961363/08fa6740393224ddbffc46e58dc5/35031.png?expires=1758218400&#x26;signature=28f49baa208dfd129d682bc77289c2f70071c3e0fc8797af866206490e9a4c75&#x26;req=dSQiFcB4nIJZWvMW3nq%2BgfaxUC7g2%2BHf6OPHVvFG277C0Z%2Fs5vwM9qMyaYwz%0AmLziHNbE0Jek9pIOcLnfpq5mUgg%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

***

### b) Creating an auto-test from scratch <a href="#h_470602d7a7" id="h_470602d7a7"></a>

To create a new automated test from scratch, start by selecting ‘AIDEN autotest’ from the ‘New test’ dropdown.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1729696227/fdb405ebb702c2f2cf6b06b72b00/69537.png?expires=1758218400&#x26;signature=2be86aa20303673a578c391a083c8c7bea00700eaf05d95292abe820d3e885b2&#x26;req=dSclH893m4NdXvMW3nq%2BgX6F5JcJCEdrhm1SxaBxoXetQLOt4WKmgvQMeE%2Bp%0Afaha27qr%2BxRybzBl6TuuqRzZElM%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Start the conversation:

In this workflow, you interact with AIDEN using natural language. Simply tell AIDEN what to test, and it will translate your instructions into executable test steps.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1729698511/4639bd6e896367137917184ac0d3/43292.png?expires=1758218400&#x26;signature=c7302e21be74f647d4d51dbd43b0f691f5101f14a96d18fd5da4a321888c833b&#x26;req=dSclH893lYReWPMW3nq%2BgTrpMJf70TFCTA1oQ7hc8v6LrlqiLMCl%2F9%2FJ9aSg%0ACPukHuD97kkfrn%2F0bl%2BJtPJBGhM%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Begin by providing the website or domain you want to test. For example, say: `let's test Google.com`

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1729697445/17c891d52e85d9bb43a1aca3ad5d/image.png?expires=1758218400&#x26;signature=d079a0591d9889b0b5b165b85c1a1aa7ba46c46dbedc906fab53b56d227db789&#x26;req=dSclH893moVbXPMW3nq%2BgTDrraG1ePwxq%2FGnzCISeULEvYqE%2BL83ddInxrpC%0APXwSXv6CRnnMQ99uJJw8TidAnws%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Define Your Steps:

AIDEN will break down your instructions into actionable steps and display visual feedback (screenshots) for each one. You can:

* Give simple actions like: “Click the ‘Gmail’ button”
* Or compound instructions like: “Enter ‘[support@qase.io](mailto:support@qase.io)’ in the search box, then click ‘Next’”

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1594861982/a1bef046d8be83b40f0687fac5ee/aiden.gif?expires=1758218400&#x26;signature=d998c4bb113e943183f1115c3401e02f591c36f13f52cc653e38f73bd94908ba&#x26;req=dSUuEsF4nIhXW%2FMW3nq%2BgfWtk1DFtWkAJpNF2Sxt5Mldlz8GaVERhdabU8I0%0ArBnnm9AQDl6re17Pbut1PAtagzo%3D%0A" alt=""><figcaption></figcaption></figure>

Each instruction is parsed and split into individual steps. As steps are generated, you’ll see both:

* A natural language summary of the action, as a step.
* A JSON block with selector and element type details

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1594865050/3f82be9530aed8fcd457315fb914/98877.png?expires=1758218400&#x26;signature=971ffaa3167d4b52567eaecfdac867146348735239a80f8d18694e27d9309d0c&#x26;req=dSUuEsF4mIFaWfMW3nq%2Bgf8h4%2BuM39jWV7CmEtojPF5oo7N3OWR6SC8rkTwj%0AgkAEb7D4dIh2b8NMKBY7TFhfHJQ%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1594865290/56f2595971196f55bfcce1d4b58f/89819.png?expires=1758218400&#x26;signature=c005d2af289872a47fcd7bb80adab21b4363b0f0d3f4e89939a7d52a7c44da5c&#x26;req=dSUuEsF4mINWWfMW3nq%2BgaVqXh%2F170XtmhP40f90UgoqgxTEZ7xNpatPYNSu%0Ag9cy4puOOyjcY9hOSPIjLthu4GA%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Deleting steps:

To delete a specific step, type for example: “Delete step 4”

<figure><img src="../.gitbook/assets/20527.png" alt="" width="563"><figcaption></figcaption></figure>

***

After reading this article, please check:

* ### [AIDEN - Automation Engineer](https://help.qase.io/en/articles/11981749-aiden-automation-engineer) <a href="#h_cf02f5a2ff" id="h_cf02f5a2ff"></a>
* ### [AIDEN - AI Test Cloud](https://help.qase.io/en/articles/11851804-aiden-ai-test-cloud) <a href="#h_9db3246623" id="h_9db3246623"></a>
