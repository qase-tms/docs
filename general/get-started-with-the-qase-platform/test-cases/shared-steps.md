# Shared steps

### What are shared steps?

Shared steps are a unique feature of Qase that allows you to create a single step that can be shared across multiple test cases. This eliminates the need to recreate the same step manually for each test case and ensures consistency across all test cases in which the shared step is used.

{% embed url="https://www.youtube.com/watch?v=Lqc7JgV4svg" %}

### How to create shared steps?

Let's imagine that I have two different cases for my test suite - both require authorization into the internal system to proceed, so it will be one of the steps to recreate.

I could go into each one of these test cases and create an "Authorization" step for each of them manually, but I'd rather create a single shared step that will be uniform and will be used across various test cases.

1. To do that, I'll navigate to the "Shared steps" section and create a new shared step:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595211174/84339b199921d0a48b2a8dde/Rze-riuigtx66rpzzEKIkPjy2UArkkvgjsJk_211S7OInQWcDiRYyJcLs4OXiL3H4rULf6eyjS90rwgKPmYFoXK3EC7ndzeU_-dCw3bsaGvFP5VZvy-Pl9DqLxtBNBPiZYnshPL-kNF9G8imMnsWhhCcgb5w0tKrsBOvJx6jvfd70Veox_G5gauEHQ" alt=""><figcaption></figcaption></figure>

2. Give your shared step a title:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595211198/d0a3b44a9851f78cfb2151c2/vfoz6NxpFGL8rVWhm6kMhr0CRY8V3DLrzi0vywf3oFu1CAR7KmK6GPhqiytmAXSZcbKn-3WlmQfn4V6aD2ieJaVDzWe4YNFowXP7sQrcXVfbMjanxQUaILQ8KEtt6OCw0AfGtio8RXo5tPR-Q3Lfvb1kSqKIB0_Hdhe0Yyyd4QP-38P1densD1uYAg" alt=""><figcaption></figcaption></figure>

3. _Steps to reproduce:_ A shared step can be configured as a single step - or as a group of steps. Under the title field, there is a "+Add step" button: just like when creating a test case and adding steps to it, you can add multiple steps to reproduce into a shared step group. That way, instead of adding multiple shared steps one by one when your scenario requires multiple consistent actions in many test cases, you can simply configure an entire shared step group with several individual steps to reproduce featured in it:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595211212/ad30aaa86391a1be47dfb306/xB7FHBj5mXH_CaCAOynP4299c7i9k7wNmoZySQY7-_aeX_P_PMRVvFwMDjnzKqWTP_gJTUHzmnt7s-kHa0aonlp4JUs-CjiaNUeJ2U3U7RxY0oBlPz1CxARGtJHOomWPIcs-hSL7Xol75_RBAeJ7N71rGxLM2-7iHKiDuQ7TnG164vhV36cOGavq0g" alt=""><figcaption></figcaption></figure>

### What else?

_Edit:_ When editing a test case, you can also convert any regular step into a shared step and adjust the newly created shared step later from the shared steps section:

<figure><img src="https://qase.intercom-attachments-7.com/i/o/595211229/6b8d49bb26e66d8bf99ad022/8kqQK-neXHsSGxZHCdeiDiH-wmeF8P4DqF9hR3m9R1WN8TMp0bXY5Gvru-FdM_M-uMyPX2RIWZuzByAybLR7fIFxmsiXgZcXQNnDhA4Kkx4h-uBN_-BxipzpSF-nmFXWUv2QgTf2c9gAiRxXYA2wa3iZfupE_MTdwfn_M3M854YYyN1fUIccDtefMg" alt=""><figcaption></figcaption></figure>

_Add to a test case:_ After creating a shared step, you can add it to a test case when creating or editing a test case by clicking the “Add shared step” button. You can also preview the shared step you want to add:

<figure><img src="https://downloads.intercomcdn.com/i/o/689763098/a6d4547ead7c8a393754a518/GIF+1.gif" alt=""><figcaption></figcaption></figure>

_Convert:_ After adding a shared step to a test case, you can convert it to a regular step and then edit the steps within the test case you are creating:

<figure><img src="https://downloads.intercomcdn.com/i/o/690535575/c43d0be1b728f759a3fbe8ec/GIF+1.gif" alt=""><figcaption></figcaption></figure>

_Modify:_ You can also modify the shared step itself: if you click "Edit" button, you will be taken to modify the shared step - apply the necessary changes, save them, and those changes will be applied to all cases where the shared step is used:\


<figure><img src="https://downloads.intercomcdn.com/i/o/691267778/91dd55d934c502f1dd0aad84/image.png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://downloads.intercomcdn.com/i/o/691268035/24aefe1d1b7e83f40fc2190a/image.png" alt=""><figcaption></figcaption></figure>
