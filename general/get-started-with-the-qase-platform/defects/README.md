---
title: Defects
slug: defects-1
createdAt: '2023-02-21T19:34:57.238Z'
updatedAt: '2023-02-21T19:34:57.238Z'
---

# Defects

### How to create a defect?

In Qase, there are two ways to create a defect: you can create one on the spot, at will, for any issue that is not necessarily connected to a particular test case or test run. Another option is to file a defect upon failing a test case during a run.

{% embed url="https://www.youtube.com/watch?v=h4ibIxZ6Djk" %}

{% embed url="https://www.youtube.com/watch?v=a9IaRwOeTLs" %}

### Option 1: Creating a defect independently

To do this, click on "Create new defect" in the "Defects" section and add all necessary details such as defect fitle, actual result, and severity, fill out any custom fields applicable to defects, and optionally add attachments. This type of defect is not connected to any test case or test run. However, it can be marked as "In Progress" (and then, consecutively, resolved), invalidated, or edited.\
\
\


<figure><img src="https://qase.intercom-attachments-7.com/i/o/597420842/51e6d155df025728e0739bbf/j0OQ93o8t8ywChQIhOQL5oobFkW1YkxfKvXwkESqF54miQJmQKl-lJr47C9zwjwJgo6_hC3OwDO6f9Nc7PzdilpKjyq-am0ABzkKTsdCfFQMj08vrHTP9dMQl0Rt4YgdAWM9LvHcN453QWFmW8fnio2gRdEiRx3tpS4UaVLRVCVwh_5lZ2uP3Qd2Sg" alt=""><figcaption></figcaption></figure>

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597420846/428f8ce3e077a6b78a91095a/I3mJRpCQbAGOzzvVqEPlDnmD9CJNdFinjjNzvkkdlu9_z6Ckhj3jvXNx0hzLpe7rZ67o5xePn-GFXbuf8KjdgblIkUZdCxT9F2dIoV11Im9778LHKDv55KzjJf2pKUlFzCcl402C9ZfDS7oCucjc6Q5FDAt4es834AK3ZN7eqz9-Z7qzLgayPrR_DQ" alt=""><figcaption></figcaption></figure>

<figure><img src="https://qase.intercom-attachments-7.com/i/o/597420856/b68a2012d9bdeabed632b752/tV-yrtJrKQ3_Q2GXg463dTXZSGdrp7iAYKW4R6G9I9Y6XC4qkiVUTc2LnrrR7pL57teE2pbVH_vhEWgQsC6y-Jfr_ZlNcWmYYvT1qUVEqNTRR-j3__DR3jbciUXlitgN-5khRATDVw1gETJ8QL23KwGCkRpH6D1CG87Bl6GuoV0ZQ-9fP27n0tD4eA" alt=""><figcaption></figcaption></figure>

You can also tie any defects filed during test runs to an existing defect you created manually. This can be helpful when you are aware of the issues beforehand, even before performing a single test run, and want to document them in advance.\


<figure><img src="https://qase.intercom-attachments-7.com/i/o/597420865/a096576ff85f6238830819b3/NskCkBrRvwNSnpvHW-jl307UJy9zRkCMfZMoxoLidJv5rdeYDdqwS1u1Ycjn6BWJOYJdTTVJKklUjyQk5EqS6aaQqjM_qlUH7ewfi6A3oLy-iQ1jgy2F8adVpSFgeOhEPqAzEvcsJOmxJ7e0NELmYaOle3sdFUToiTR93tRYPBoUYCrn2qC7MRz1bw" alt=""><figcaption></figcaption></figure>

### Option 2: During a test run, some of your test cases will likely fail.

#### To set up your Project, remember the "Fail case on step fail" setting:

* If this setting is on, failing a single step in a case during a test run will cause the entire test case to fail. You will then be prompted to create a new defect.
*   If this setting is off, failing a single step in a case will not cause the entire test case to fail. You can continue with other steps while still being prompted to create a defect only if you fail the entire test case.\


    <figure><img src="https://downloads.intercomcdn.com/i/o/609555761/578cc9154f42e88a7c223387/image.png" alt=""><figcaption></figcaption></figure>

#### How to create a defect:

*   Mark a test case as "Failed".\


    <figure><img src="https://qase.intercom-attachments-7.com/i/o/597420875/0dd1646d1c45383e6eba470b/JEkoyalk8pw-kle4LjskYxzL091xtrNUYCawdKxmLid8M2HA6lSuFoDi4MKfRlIekppeZYF9l9exbqceKCBjM8VNJhAXGCX8edOf11KaUbqd2K5WypTpwfHmoFWKIhOxnp8F2AdefJCJxZOQLhAPiEAN_Kl5axgvAgb5WgzQjfkpWXieZEPVYTHfkg" alt=""><figcaption></figcaption></figure>
* You will be prompted to a run result window, where you can add comments, record time spent on the test case, attach files, and create/attach a defect.\
  \
  [![](https://qase.intercom-attachments-7.com/i/o/597420881/24590ad923835a248ec634ec/-L34nNTbPPB\_GhnsoY\_Yech9BLW2Nw-cAcaIWHcPRFwOm1iYIesbyudACMpBvUSg7kDDKK\_rY1AktjPS2p2lIOlQ3NT7lJ7-HWWzjPwbps\_IklYMUni5Ozu223gI8Z5aGJUqroTGcysO3-H7kt6gm0Cfn9GF6GMmyEB2CAlDijqjwqT1yi1RxPvvTg)](https://qase.intercom-attachments-7.com/i/o/597420881/24590ad923835a248ec634ec/-L34nNTbPPB\_GhnsoY\_Yech9BLW2Nw-cAcaIWHcPRFwOm1iYIesbyudACMpBvUSg7kDDKK\_rY1AktjPS2p2lIOlQ3NT7lJ7-HWWzjPwbps\_IklYMUni5Ozu223gI8Z5aGJUqroTGcysO3-H7kt6gm0Cfn9GF6GMmyEB2CAlDijqjwqT1yi1RxPvvTg)
* With the checkbox checked, you will be prompted to fill out other remaining defect properties, including any custom fields you created. You can choose whether to create a new defect or attach an existing one to the issue you found. You can also change its title, severity, and custom fields' values, and send a connected issue to other integrated third-party software systems.\
  \
  [![](https://qase.intercom-attachments-7.com/i/o/597420893/56c503761319fc5d37e9301d/ojLkJ7hOAal0ZnqOrdLPVChLHzcos\_KRvVmh16QPdRcx-dU-qQuci8trNmnetph1ikwhz6bOYZmg0PCPMxgwww\_oEmFU3uOLqv2RTnkdNku45FfnCnYEbiHHSIZWamM9HTHp\_ZFiTAN3yhk-Off7G9pfnkqkj2UA71GLhLzKDlglub8Zq-KVNCwfqw)](https://qase.intercom-attachments-7.com/i/o/597420893/56c503761319fc5d37e9301d/ojLkJ7hOAal0ZnqOrdLPVChLHzcos\_KRvVmh16QPdRcx-dU-qQuci8trNmnetph1ikwhz6bOYZmg0PCPMxgwww\_oEmFU3uOLqv2RTnkdNku45FfnCnYEbiHHSIZWamM9HTHp\_ZFiTAN3yhk-Off7G9pfnkqkj2UA71GLhLzKDlglub8Zq-KVNCwfqw)
*   A new defect will be created from the test run result and saved under the "Defects" section and the “Defects” tab of your test run.\


    <figure><img src="https://qase.intercom-attachments-7.com/i/o/597420896/271c8d40f061b50b48eb9645/5Kx-0Wlpefwhyk4TsTct6roTVVF6Xmi9EN6EFC2WTmT6xCDtCVjcVOZlecArLn79wdhcFrGqsYS-XG_jDSpORqOuo8gkVrn0SjIZAl3zNxIM3b4IA2w5BVao7asN-XdljR5Q2G1ID_bimuHvIe3xVCG4ATLqYgoiWhXvrzRpT1LmVLuuP7kKxsJxgA" alt=""><figcaption></figcaption></figure>

    <figure><img src="https://qase.intercom-attachments-7.com/i/o/597420902/312db97256556d89c94437f6/92mdKk7uFQRpjzGTnCetZhQf10CwTAyaMzNCjgqswabQC8sWIQHqgWbPYhIUhK89mQnDKebh9_HSPNZ0RHB0HLSdqamGpCrqCK2OiS4NvqcNoWxqRosef13OUITJ7L1TgdzHD3yzitI13cY67U6mvCj5ct9N8oeCOd2eQchqH5m4k1VcDvIeaFiDCA" alt=""><figcaption></figcaption></figure>

Note: Defects viewed in a test run will show only defects filed in that test run. You can find all defects filed in a project under the “Defects” section.
