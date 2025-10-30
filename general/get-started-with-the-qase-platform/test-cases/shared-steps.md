# Shared steps

### What are shared steps?

Shared steps are a unique feature of Qase that allows you to create a single step that can be shared across multiple test cases. This eliminates the need to recreate the same step manually for each test case and ensures consistency across all test cases in which the shared step is used.

{% embed url="https://www.youtube.com/watch?v=wFHEW64TigY" %}

Imagine that you have two different cases for a test suite - both require authorization into the internal system to proceed, so it will be one of the steps to recreate.

You could manually add an “Authorization” step to each test case individually, but it’s better to create a single shared step that you can consistently use across multiple test cases.



### Create a Shared step <a href="#h_3df4e51159" id="h_3df4e51159"></a>

Go to the Shared Steps section and create a new shared step

<figure><img src="../../../.gitbook/assets/69756.png" alt="" width="563"><figcaption></figcaption></figure>

Provide a title for your shared step to identify it easily.

<figure><img src="../../../.gitbook/assets/image (95).png" alt="" width="563"><figcaption></figcaption></figure>

A shared step can either be a single step or a group of multiple steps.

* Use the +Add Step button (located below the title field) to add individual steps, just like when creating steps for a test case.
* If your scenario involves multiple consistent actions across several test cases, group these steps into one shared step for better reusability.

<figure><img src="../../../.gitbook/assets/20235.png" alt="" width="563"><figcaption></figcaption></figure>

### Convert existing step: <a href="#h_2631b7d236" id="h_2631b7d236"></a>

While editing a test case, you can convert a regular step into a shared step. Adjust the newly created shared step later in the Shared Steps section.

<figure><img src="../../../.gitbook/assets/convert shared step.gif" alt="" width="563"><figcaption></figcaption></figure>

### Add Shared step to a test case: <a href="#h_411dadaf24" id="h_411dadaf24"></a>

When creating or editing a test case, click the Add Shared Step button to include a shared step. You can preview the shared step before adding it to the test case.

<figure><img src="../../../.gitbook/assets/Add shared step.gif" alt="" width="563"><figcaption></figcaption></figure>

### Edit Shared step: <a href="#h_c96a481c59" id="h_c96a481c59"></a>

After adding a shared step to a test case, you can:

* Convert it into a regular step and edit it within the test case.
* Modify the shared step itself by clicking the Edit button in the Shared Steps section.
* Any changes you make and save will automatically apply to all test cases that use the shared step.

<figure><img src="../../../.gitbook/assets/modify shared step.gif" alt="" width="563"><figcaption></figcaption></figure>

### View linked test cases. <a href="#h_8415af9269" id="h_8415af9269"></a>

Clicking the links in the ‘Attached to’ column for a shared step will open the repository page, showing only the test cases that include that shared step.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1804188555/ed899c5a1160e0f9081e9b3cc4d6/image.png?expires=1761912000&#x26;signature=41afb506733950a9f8afb8ae26dfffa937d9415459c12348b6e18a5d96466e00&#x26;req=dSgnEsh2lYRaXPMW3nq%2BgUC0vo2BT3Sq1tt8teU44tY3bsPJBSmRKXUJcdr7%0AwSDnyqkxEYQp28t7hqxCzircAj4%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1804189388/bb70eac5c2a57f0bdb374476b30c/image.png?expires=1761912000&#x26;signature=22d43590135e8c1db7cd0a49d57edcbd329c94b5ab520a80f89e397da6f73208&#x26;req=dSgnEsh2lIJXUfMW3nq%2BgReH4nPHMCvruanW5e7xIPUdkDvb55HAUpS5ebAf%0AENWjnylAAhCMQLRKCZbvbq0V65g%3D%0A" alt="" width="563"><figcaption></figcaption></figure>
