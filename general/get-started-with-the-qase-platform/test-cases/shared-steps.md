# Shared steps

### What are shared steps?

Shared steps are a unique feature of Qase that allows you to create a single step that can be shared across multiple test cases. This eliminates the need to recreate the same step manually for each test case and ensures consistency across all test cases in which the shared step is used.

{% embed url="https://www.youtube.com/watch?v=wFHEW64TigY" %}

IShared steps are a unique feature of Qase that allows you to create a single step that can be shared across multiple test cases. This eliminates the need to recreate the same step manually for each test case and ensures consistency across all test cases in which the shared step is used.

Imagine that you have two different cases for a test suite - both require authorization into the internal system to proceed, so it will be one of the steps to recreate.

You could manually add an “Authorization” step to each test case individually, but it’s better to create a single shared step that you can consistently use across multiple test cases.

{% hint style="info" %}
Shared steps are available both at a project level, and also at a workspace level.
{% endhint %}

### Create a Shared step <a href="#h_3df4e51159" id="h_3df4e51159"></a>

Go to the Shared Steps section and create a new shared step

<figure><img src="../../../.gitbook/assets/69756.png" alt="" width="563"><figcaption></figcaption></figure>

Provide a title for your shared step to identify it easily.

<figure><img src="../../../.gitbook/assets/image (95).png" alt="" width="563"><figcaption></figcaption></figure>

A shared step can either be a single step or a group of multiple steps.

* Use the +Add Step button (located below the title field) to add individual steps, just like when creating steps for a test case.

<figure><img src="../../../.gitbook/assets/20235.png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
It is currently not possible create nested steps inside of a shared step.
{% endhint %}

### Convert existing step: <a href="#h_2631b7d236" id="h_2631b7d236"></a>

While editing a test case, you can convert a regular step into a shared step. Adjust the newly created shared step later in the Shared Steps section.

<div data-full-width="true"><figure><img src="../../../.gitbook/assets/convert shared step.gif" alt="" width="563"><figcaption></figcaption></figure></div>

### Global Shared Steps (workspace-level) <a href="#h_e9184f903d" id="h_e9184f903d"></a>

Global shared steps work much like regular shared steps, but they are available across every project in your workspace instead of being limited to just one.

For instance, you might be testing the same product on web, iOS, and Android. All these test cases may require the same action such as logging into the application.

Instead of creating the same shared step in each project, you can create one global shared step and use it wherever it is needed.

You can create a global (workspace-level) Shared step, from [workpsace >> shared steps](https://app.qase.io/workspace/shared-parameters).

<div data-full-width="true"><figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1861040567/08478e3367d54fbb33b2e146ecfb/78384303-b8c6-4393-bf99-890375846a09?expires=1764828000&#x26;signature=b0d05937c31ebc5b32658e3acf886a1aab026762631f9498b6f9b4dd008e9921&#x26;req=dSghF8l6nYRZXvMW3nq%2BgdYd0q5yjkjCT5Whx9NPQrUAnggcid5ohFo90hW0%0AEUY%2BftPpihY02sw3bmy9LA8Pcwg%3D%0A" alt="" width="563"><figcaption></figcaption></figure></div>

Please note that steps that already exist in test cases or shared steps within a project cannot be converted into global shared steps.

### Add Shared step to a test case: <a href="#h_411dadaf24" id="h_411dadaf24"></a>

When you create or edit a test case, select the Add Shared Step button to include either a project-level shared step or a global shared step.

You can preview a step before adding it to the test case.

Global shared steps have a 🌐 icon at the beginning so you can tell them apart.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1861052612/2a1fe173e3d5841187636819e8dc/shared+steps+global+add.gif?expires=1764828000&#x26;signature=304b08feeff9c6364cb0918194aa278a45cb18a2ad8251f380c37d67cfd9d733&#x26;req=dSghF8l7n4deW%2FMW3nq%2BgXXNq%2FgmnTjWdY1Ei2%2F%2Bn4l1M7PcI4bEYiJRqMNe%0AsZYGwp1a11lR3K8AOirfq7CHglI%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

### Edit Shared step: <a href="#h_c96a481c59" id="h_c96a481c59"></a>

You can update the shared step or global shared steps by selecting the Edit button in the Shared Steps section.

_Any changes you make and save will automatically apply to every test case that uses that shared step, which helps keep everything consistent and up to date._

<figure><img src="../../../.gitbook/assets/modify shared step.gif" alt="" width="563"><figcaption></figcaption></figure>

### View linked test cases. <a href="#h_8415af9269" id="h_8415af9269"></a>

Clicking the links in the ‘Attached to’ column for a shared step will open the repository page, showing only the test cases that include that shared step.

For shared steps, clicking the links in the ‘Attached to’ column will open the repository and show all the test cases where that step is used.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1804188555/ed899c5a1160e0f9081e9b3cc4d6/image.png?expires=1761912000&#x26;signature=41afb506733950a9f8afb8ae26dfffa937d9415459c12348b6e18a5d96466e00&#x26;req=dSgnEsh2lYRaXPMW3nq%2BgUC0vo2BT3Sq1tt8teU44tY3bsPJBSmRKXUJcdr7%0AwSDnyqkxEYQp28t7hqxCzircAj4%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1804189388/bb70eac5c2a57f0bdb374476b30c/image.png?expires=1761912000&#x26;signature=22d43590135e8c1db7cd0a49d57edcbd329c94b5ab520a80f89e397da6f73208&#x26;req=dSgnEsh2lIJXUfMW3nq%2BgReH4nPHMCvruanW5e7xIPUdkDvb55HAUpS5ebAf%0AENWjnylAAhCMQLRKCZbvbq0V65g%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

### Deleting Shared steps: <a href="#h_24a0876700" id="h_24a0876700"></a>

\
When you choose to delete a shared step, you can choose between two options for all the cases that use that particular shared step.

1. Delete the shared step and remove if from all associated test cases.
2. Convert the shared step into a regular step before deleting the actual shared step.

<figure><img src="https://downloads.intercomcdn.com/i/o/wsaz8vex/1861010977/9499289aacf1543467de1853f2a3/image.png?expires=1764828000&#x26;signature=c6b3038a9108cfd878133e18c44c8468c984cc1381d77cf591291c7751f4114c&#x26;req=dSghF8l%2FnYhYXvMW3nq%2BgUBeyddoCrFNLGQvECMM7Nn9JO0iuyCAOCCez46b%0AttLOtvBoLho2pmZNi5SSekR5m8s%3D%0A" alt="" width="563"><figcaption></figcaption></figure>

