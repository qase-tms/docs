# AIDEN - QA Architect

{% hint style="info" %}
For pricing details, check [AIDEN pricing: explained](https://help.qase.io/en/articles/11737411-aiden-pricing-explained).
{% endhint %}

While Manual testing has been the cornerstone of software quality for decades, it is slow, costly, and error-prone. And, traditional test automation requires deep technical expertise, extensive infrastructure, and ongoing maintenance — and these are barriers that prevent many teams from adopting it effectively.

AIDEN eliminates these challenges by allowing users to create, execute, and maintain automated tests using natural language instead of working with code.

By leveraging Generative AI, AIDEN transforms test descriptions into executable test scripts in Qase Cloud, runs them in parallel across multiple browsers.

With AIDEN, you can analyse your repository, generate automated test code from your manual test cases, and execute the tests in Qase Cloud.

***

## Repository Advisor <a href="#h_4ba8164cb5" id="h_4ba8164cb5"></a>

Every repository has some test cases are perfect for automation — they’re stable, repetitive, and save a huge amount of time when automated.&#x20;

**Test Advisor** helps you quickly identify these high-value tests, so you can focus on what brings the biggest impact with the least effort.&#x20;

To start the advisor, select all the suites or test cases, and click '**Run Advisor**' button:

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1452918938/8cde0269aada88b7ae4435e1bbf4/35627.png?expires=1744675200&#x26;signature=e39a5b7cbb11d02a2ace531361b8cccd0598fcc7cd986ec74c82ca2257df981b&#x26;req=dSQiFMB%2FlYhcUfMW3nq%2BgWwTodIXhiQNQCZnKPhDijoI%2BlPkqP2Si7yazBN2%0A8TRW6P8xAwRh8vJVhpS6gDXPM8Q%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (107).png" alt="" width="563"><figcaption></figcaption></figure>



The analysis will take a moment, so feel free to sit back or tackle other tasks. AIDEN will automatically notify you with a summary as soon as it’s done.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1452919616/fd08f45c8e2a8bad09de8fc87465/analysis%2Bsuccessful%2Bnotification.png?expires=1744675200&#x26;signature=ac147730d5f28b943d6fcd1c3c210ecaaaf44215fbcb1ee74afdef5ae98a6f15&#x26;req=dSQiFMB%2FlIdeX%2FMW3nq%2BgWDdgeEOSUmg3IF0sqBgV7OivkQ2UR6LLsvJaXxb%0AdM1q8pTUtQkTlcQoJL5vB9Im91c%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Let's understand the results:

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453815589/b433f0d199b42dec17f633280541/55122.png?expires=1744675200&#x26;signature=3c12b04879ab73075b2d7ddfb5bf0ca49295ae9c2c911fc9fbf7fc77ef4d983d&#x26;req=dSQiFcF%2FmIRXUPMW3nq%2BgUTzYJpGAMnseHi%2FzYaIHJRqy%2BBk9SD9qFXkfm2D%0AWBx12R6YEzNhc%2Ftpztjq7j9lQLg%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

<details>

<summary>Green: These test cases are easy to automate, with minimal or no oversight.</summary>

![](https://downloads.intercomcdn.com/i/o/wsaz8vex/1453815171/2d333cbf626bd9ce8ff22fd9f649/automate-2Bwith-2Bai.png?expires=1744525800\&signature=5b60f56ef37302bd981945c05178479c7cf0d348b746b28cd346b829916b7d2c\&req=dSQiFcF%2FmIBYWPMW1HO4zVNef3q816ZDM2e2%2BamXFJxKNCzrWeit0d%2BfeUl%2B%0Aq1KY%0A)

</details>

<details>

<summary>Yellow: Test case has good potential for automation, it may be missing information.</summary>

![](https://downloads.intercomcdn.com/i/o/wsaz8vex/1453815353/991e984ef85de8c20549753aeee8/strong-2Bpotential-2Bto-2Bautomate.png?expires=1744525800\&signature=67ae7a50b36a7207907c58177e697e7fba1f16c18e215b0fe0f146b2f976902f\&req=dSQiFcF%2FmIJaWvMW1HO4zT1YFMLmBcSGmvJGfLfzwAmQRvrDEUKQxm5Ae2J0%0AEIa1%0A)

</details>

<details>

<summary>Red: This test case lacks essential details, such as test steps, or involves complex logic that makes automation challenging.</summary>

![](https://downloads.intercomcdn.com/i/o/wsaz8vex/1453816988/d2d22011def66f1556cd482c7403/reanlyse.png?expires=1744525800\&signature=48bb4790e6226e84dbe2c3e8879782606a3538cf592aa8fc073676657a284fc8\&req=dSQiFcF%2Fm4hXUfMW1HO4zW%2F3n4SK3lF6OvSXz27xe9xLeRRmDTNb%2Bk5cf769%0A6iVk%0A)

</details>

Based on the suggestions from AIDEN, once you edit your test cases that are not in Green, you can 'reanalyse' them.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453967433/9dfc2075666349548f043a1eaac3/92959.png?expires=1744675200&#x26;signature=bd32f3ac6faa8617811460374bb9b8e31fc6cf6f6b151346176847f6134a994d&#x26;req=dSQiFcB4moVcWvMW3nq%2BgSCfhCqYGbS9iTN79JExz2bOdDSQ08LyumPts203%0Ao1SuSeidtKHPiY%2BANjEH%2FGHaWHc%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453967355/f4880bb65118418be9b3deaa7d32/5420.png?expires=1744675200&#x26;signature=c5bdeb8121deee43963a7a0f265d190c9e375c27d627a1f30ae981f8ff73957e&#x26;req=dSQiFcB4moJaXPMW3nq%2BgaDqdAMa%2B79%2BLaZSyh2Ztx84g105zsEPui3lxW3b%0ANXZgPO5G0lwguu8yAhTTolC%2BAdQ%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

***

## Let's start automating! <a href="#h_c1c01a4ff1" id="h_c1c01a4ff1"></a>

### **a) Convert an existing Manual Test**&#x20;

Open any test case, and click the 'Automate with AI' button to begin:

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453818585/5c595ec1e792051ac066feef59a3/77639.png?expires=1744675200&#x26;signature=951c1828fe74dd5a34f0e096f9f32148067f877573be972c3e223839fd71b26b&#x26;req=dSQiFcF%2FlYRXXPMW3nq%2BgclsHm1%2BHAJFciA5mL%2BTOn0iNIE47Sn51hxELv%2Bo%0AOyQmP5A%2FcZCyq0q7o64c3fi9yBc%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Adding the environment <a href="#h_d5d07d1ca8" id="h_d5d07d1ca8"></a>

Your tests will run at a specific domain, so let's add the host environment:

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453819358/b0e5ffc24e353ddf2dbc223465f4/43433.png?expires=1744675200&#x26;signature=d4ed7dd8282442bc7300272ec3f267bf415122e6b1b728393c4e8dd754b3ba35&#x26;req=dSQiFcF%2FlIJaUfMW3nq%2BgTuUutkmD1HraJu9GP0tiEYf9wcLZ7tGtkv7jzln%0AE4Owk%2B55Q9%2BiL%2FFZ7sWVUWBacmw%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

If your host environment is not accessible from the public internet, you can help Qase tunnel to your private environment, here's a script that will help you set it up:

👉 [https://github.com/qase-tms/qase-frp](https://github.com/qase-tms/qase-frp)

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453849303/823336b6e880a98fd0af6ac91043/82820.png?expires=1744675200&#x26;signature=5429c93d0cd94e8ecc77ae2531cf5c5306bed6c577c8df6c3db52f01f3a87629&#x26;req=dSQiFcF6lIJfWvMW3nq%2BgVRNpDu1to%2BbXcTW1S%2FTPRVvO3YJ7B4QPje7QlrH%0Ay7DDBwdnrwr3k8NEvAUsx8EywdA%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Authorization <a href="#h_f541b141a3" id="h_f541b141a3"></a>

Most of test cases generally require authorization as a precondition. You can add your authorization steps and use them when starting auto-test generation.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453851884/d6f6e33ef0f5211c45426484e80b/63280.png?expires=1744675200&#x26;signature=e6be722c5b2de1948a937147026a7493c9ae10e1164b2e7515d4f027a5635c27&#x26;req=dSQiFcF7nIlXXfMW3nq%2BgcqltgfYzx%2F8vMliCVRR68W6f8Lst4SKAGT2%2FL9k%0AVT0j2FHys3euCrO%2BvkGkOw4KL1s%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453860286/0bc2dc049a06af3ca59bfd0e0a08/12279.png?expires=1744675200&#x26;signature=5469643606bfbc2f4d17b9fb12d028f0bcf374d041226035a2135cbd09ad86c4&#x26;req=dSQiFcF4nYNXX%2FMW3nq%2BgV4ZksrXF7uAYfoyjJdSL1qhM0NvPmtpKP0GAAx3%0AWpLaIrNaBozmDdlx6AnjtBsyr2s%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Generation <a href="#h_a76168e8f4" id="h_a76168e8f4"></a>

You can monitor the status and view the test case that is being used for generation at the top.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453867027/382d2ab7b3dbb5f73c0b0b085527/82772.png?expires=1744675200&#x26;signature=2eec690c4b2e760d1a351da1f7d69e20de6c6331604257379471e9130d441d7f&#x26;req=dSQiFcF4moFdXvMW3nq%2BgTt8dPtZW9RvMqGSIvLgp%2FemJBZHVCP6KUqD%2FfQG%0AjSLL95o9qXZSt3PzHbAtiaQC%2Fo8%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

The generator works by first breaking down your manual test case steps into proper actionable steps.

A 'Success' or 'Failure' message is displayed for each step, along with a screenshot to communicate progress.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1470743545/4359dd4a2b9c9f23f89de97eb276/start+generation.png?expires=1744675200&#x26;signature=a29ac87c3606add574c16952e57041e3bf48616686d4913f2691fcda8c3abf27&#x26;req=dSQgFs56noRbXPMW3nq%2Bga3SupQjw5iBL%2Bp0wI2jma8xDmNMKNSzLhJpYb6s%0ACO2FnPD7Nx676kDrAFW%2BLVLb5bA%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Edit Steps <a href="#h_009369db33" id="h_009369db33"></a>

If generation fails for a step, the status is updated as 'Error' and the particular steps with the problem will have the Error description.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1470744391/0415e8dc900c1198c16d617d3c35/error+step+final+edit.png?expires=1744675200&#x26;signature=06a9b09e442a44509a6dfc515301410887178216cfdd6a2e593630800450c7d5&#x26;req=dSQgFs56mYJWWPMW3nq%2BgXU1Sr90uvsIO9DKwGzuuVfS%2FP%2BJIOYU2mZeok3u%0AWSOfsaleV%2BroXnfgpC0wvCDy%2BPs%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

You can help AIDEN by editing the particular step. Click 'Edit steps' and just correct the step text in natural language.

You can also delete steps that are not needed, or even edit steps that are successfully generated if you need to change something.

Click 'Regenerate' and AIDEN updates the steps. If you edit a step that is not generated yet, it will simply update the step's text.

If edits are made to a step that is already generated, it'll restart generation from that step.

#### Action Editor <a href="#h_c28b4a518d" id="h_c28b4a518d"></a>

For scenarios where the error is a bit complicated, for example, if an element is not recognized as a button, you can use the JSON Action Editor to debug the step.

Follow the link below to understand how the action editor works.

👉  [guide-action-editor.md](../guide-action-editor.md "mention")

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453892326/b00ac717e960aca5a15607c2c689/27133.png?expires=1744675200&#x26;signature=44bc0e39b410a62ffbe0a2263814b96a18fcdb221df1e0fb7278aafe480c09dc&#x26;req=dSQiFcF3n4JdX%2FMW3nq%2Bgde0wOuKHmHx9rITXZ9dV8jZp4%2BzBfG21%2BSNg7Il%0AsKi%2Fk8CYIkZ4XacqJ0ioXanuwG4%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Notification widget <a href="#h_5f346667f9" id="h_5f346667f9"></a>

If you navigate away, to a different page in the middle of the generation. You can always check the progress from AIDEN's notification widget.

If the generation is successful, you can find the test case from the "For Review" tab.

Generation can also be paused. There's a tab to view all the test cases that are paused previously.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1454007028/12d169d4812c0139359d562dbc4f/notiifcation+widget.png?expires=1744675200&#x26;signature=b586fa0117e92cbe740930389f622c83d60ebc4344c78b9983e7468d87ebb830&#x26;req=dSQiEsl%2BmoFdUfMW3nq%2BgRbSLglpjBxdvCNbZ1laKxbiiY6kek%2BRlG7USaXT%0Aih%2Fc7vKzpsf7a7GxWzq8CD4f%2Bxk%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Review and Save <a href="#h_e18686fad3" id="h_e18686fad3"></a>

Once all test steps are successfully generated, the entire execution can be reviewed from the final step's attachment.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1470775569/0b20416fbd231c57a9ca127b8269/review+video+and+save.png?expires=1744675200&#x26;signature=4708e5cd865b9722465cce8a8f47cbe3be2b28467e2e8de0757adbe1368f3acb&#x26;req=dSQgFs55mIRZUPMW3nq%2BgWXq0HV%2FlyIDU2Orp4DjJ7i7t1UeMjxy7sPw7pdy%0AkHqWgVwr9D5teBdCqvA4CGBTHbA%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Click 'Save' to complete the generate and save the test case to the repository. You can differentiate this test case from the rest of the manual test cases with this symbol.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453961363/08fa6740393224ddbffc46e58dc5/35031.png?expires=1744675200&#x26;signature=dbfd0b155264b623c172b6eed05acf6d9976b19ccf419c23ef13919faeb92bb6&#x26;req=dSQiFcB4nIJZWvMW3nq%2BgfaxUC7h1%2BXZ5eXHVvFG2748nps8xMn7AIRpNZEC%0AhvSL1Cc3%2BvnNVAdb4WjajB%2BvqKc%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

### b) Creating an auto-test from scratch <a href="#h_470602d7a7" id="h_470602d7a7"></a>

To create a new automated test from scratch, start by selecting ‘Automate with AIDEN’ from the ‘New test’ dropdown.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1594838217/48d8ca4e4ca81eb635e2b7e90159/65009.png?expires=1751414400&#x26;signature=c067ad08fa5dd814f317783d223d5e47c37223cf337eddac84d7f38d079caad8&#x26;req=dSUuEsF9lYNeXvMW3nq%2BgTcEhFrc%2FlVxh4jO%2F1E4dlNh%2Bq8HEhlwUeQKUlxn%0Aoa%2FyZ0KtLWfoCYzdRp%2BFndQrZ6I%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Start the conversation:

In this workflow, you interact with AIDEN using natural language. Simply tell AIDEN what to test, and it will translate your instructions into executable test steps.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1594847766/4e114103764ea767de99b33b6917/67865.png?expires=1751414400&#x26;signature=e5b7cab1517b17d6268bdac2a35100af3c35c7d2ea7ec11ddf25d312d099f2ad&#x26;req=dSUuEsF6moZZX%2FMW3nq%2Bgenm0DUKetU0hdD62MpfzJUGE6TVRsFobRHwvuPs%0AkKG92Udnmr3tU3i6fuyZ0J%2FEP88%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Begin by providing the website or domain you want to test. For example, say: `let's use Google.com`

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1594850187/471b9bbea69b3afd1e0b561a7df7/7644.png?expires=1751414400&#x26;signature=b67617a447d642e701c52bbcc33f56fe996fb1d8d6fd49d7d2adb287818382cd&#x26;req=dSUuEsF7nYBXXvMW3nq%2Bgby1im0NOPv9RxJdP5xOLHzHApO9%2Fgr2sCxOHKSm%0AXU%2FQlA5M%2BDgbci%2FyrDqHNo%2BowgM%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Define Your Steps:

AIDEN will break down your instructions into actionable steps and display visual feedback (screenshots) for each one. You can:

* Give simple actions like: “Click the ‘Gmail’ button”
* Or compound instructions like: “Enter ‘[support@qase.io](mailto:support@qase.io)’ in the search box, then click ‘Next’”

<figure><img src="../.gitbook/assets/aiden (1).gif" alt="" width="563"><figcaption></figcaption></figure>

Each instruction is parsed and split into individual steps. As steps are generated, you’ll see both:

* A natural language summary of the action, as a step.
* A JSON block with selector and element type details

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1594865290/56f2595971196f55bfcce1d4b58f/89819.png?expires=1751414400&#x26;signature=fc97759debedcdfd063d2356ed1084d14a09429a4fb70713b7bfd77044613964&#x26;req=dSUuEsF4mINWWfMW3nq%2BgaVqXh%2F15kPtlhP40f90UgoB1ZrYS9Nf6O9sWT6e%0As1J36QOSzEJbch4EGqoYDJhAXYQ%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1594865050/3f82be9530aed8fcd457315fb914/98877.png?expires=1751414400&#x26;signature=7675a9a03524c71a82ce277c08630713cd28329518cfa79fbbe3e616d6f811bd&#x26;req=dSUuEsF4mIFaWfMW3nq%2Bgf8h4%2BuM1t7WW7CmEtojPF5yflnDrEZXOPCtGdKU%0A6DEXC705dHVCA8EA0l3dQ87ckto%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

#### Deleting steps:

To delete a specific step, type for example: “Delete step 4”

<figure><img src="../.gitbook/assets/aiden delete.gif" alt="" width="563"><figcaption></figcaption></figure>

## Download the test code <a href="#h_6a499bcdb6" id="h_6a499bcdb6"></a>

You can copy or download the generated test code with the **Export code** option. This option is available on both the repository, and while generating the auto-test.

If you had already saved the test case, simply click the test case to open in preview, and use the '`Export autotest`' option.

<figure><img src="../.gitbook/assets/export converted case.png" alt="" width="563"><figcaption></figcaption></figure>

Select the language and click '**Generate**' - it will take a quick moment to display the code. You can then copy or download the code.

<figure><img src="../.gitbook/assets/53429.png" alt="" width="563"><figcaption></figcaption></figure>

With the 'automate with AIDEN' workflow, you'll always have the option to export the code, at any point during generation:

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1594884670/6d7d6626bc684ffa269374b475c6/13491.png?expires=1751273100&#x26;signature=f8eaeb4fd5d540b7bdb943d094e2cf8caffa10fed4d2d0952b1dcd36ec379954&#x26;req=dSUuEsF2mYdYWfMW1HO4zQMuEtTDtaxkYZQQT4CBCMDrNKfn7WeVOPv4HtGn%0Am4pr2lgwBHASXcZzKBk%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

With the convertion workflow, the 'Export code' option will be active in two instances:

* Test is 100% converted; all steps are successfully generated

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1563246680/13cc84051c1962373d9c52ce1ad3/success+test+case.png?expires=1749664800&#x26;signature=a1735554b6b50409f7d6f6c058d02f9d6efea84b95baf3696543010a0131fb07&#x26;req=dSUhFct6m4dXWfMW3nq%2BgaBe1lFr6p7SoalJ2wATuR4PNv6bIPbeCo0wDEfM%0AuPjSIxODHcDsnVkuvA%2BEtZJWInA%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

* Test is partially converted; a failure occurred at any step

<figure><img src="../.gitbook/assets/failed test export.png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
Currently, code can only be exported to:

* **Javascript**
  * Playwright
  * Cypress
{% endhint %}





## Executing the automated tests <a href="#h_8203030372" id="h_8203030372"></a>

To run the tests in Qase Cloud, simply select the tests from the repository for an express test run.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453993258/1bc63e464c4e63438df02f43cb1d/92403.png?expires=1744675200&#x26;signature=4eeb67759688f260fedc47ff1c8e69b709b7e436af3dcbd7ee53ce0d1881c9c6&#x26;req=dSQiFcB3noNaUfMW3nq%2BgdyMMi87%2FQxJo836KFuAmqUEfndTqKRy6rhFgvwZ%0AY6SKGzIo2GtZBfHiGojIX6UoZJ8%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

In this window, select 'Cloud' and proceed to choose the Environment, and Configuration options.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1453996972/ab09c089ca97b16b5255e42812aa/10747.png?expires=1744675200&#x26;signature=f3c1093ad46ee2e00e136038c3a31faca4f96cccb64780c3383f557329a212a9&#x26;req=dSQiFcB3m4hYW%2FMW3nq%2BgdP9TJ%2Fs7GPhrz1HH9FLvW8%2BYVrOj8nbDKK9mpTN%0AC2DvqNH91nRG2qUmWYYI%2BrfdCH0%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Depending on the browser configuration, multiple test runs will be created and the execution for the selected test cases will be begin the cloud immediately.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1452930901/53356dc3d9efec58512c9c0702a4/three%2Bruns.png?expires=1744675200&#x26;signature=19336a84ce0c2d893d70f61aac7b405032a7ef004286834444780b2481882fad&#x26;req=dSQiFMB9nYhfWPMW3nq%2BgXlP70Fp%2BsourA67E2y3W5m7rG%2BCOMELUAvFyhD5%0AbCOgFZZ4GGViw0YkWNM8ImvAYq4%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

Once the tests are executed, the results will be posted back to the test run automatically.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1452930153/ee2bff3394e66f6b2314792d8307/inside%2Btest%2Brun.png?expires=1744675200&#x26;signature=a603604271f5ec3c91f8654f3099a066f191cbee7ee1b7bd7027235fd3f07200&#x26;req=dSQiFMB9nYBaWvMW3nq%2BgR9Zyj0RQzffWY7N0wlfFF%2Bo3%2FavptRsvR%2FAljlw%0AsWiGTrZoXpcqOE8zqETx7ftfrBw%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

A screenshot is captured at each test step along with a complete video of the entire execution, are attached to the result. You will also find a `.zip` file attached for the trace.
