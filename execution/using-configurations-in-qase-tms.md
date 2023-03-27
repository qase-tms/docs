---
title: Using Configurations in Qase TMS
slug: using-configurations-in-qase-tms
hidden: true
createdAt: '2023-02-24T12:46:08.263Z'
updatedAt: '2023-02-24T12:46:08.263Z'
---

# Using Configurations in Qase TMS

{% embed url="https://youtu.be/msObZRlBYmM" %}

Configurations can be used to when you want to specify in a Test Run, which hardware or software configuration the  run should be performed on.

Configuration groups can be found in the Projects section of your workspace:

![](<../.gitbook/assets/image (10).png>)

Id=f for example your team is working on a web application, and you want to test its behavior in several different browsers. For this scenario, you can create a "Browsers" configuration group and list all the browsers you plan to be perform your testing in:

![](<../.gitbook/assets/image (4).png>)

![](<../.gitbook/assets/image (6).png>)

![](<../.gitbook/assets/image (1).png>)

After your configuration group has been successfully created, and you've added all possible individual configurations to test on, you can now specify this while creating a test run - all available configuration groups will be shown in the "Configurations" section:

![](<../.gitbook/assets/image (7).png>)

You can create multiple configuration groups and have combinations of them, for example, different browsers and different OS:

![](<../.gitbook/assets/image (8).png>)

You also have the ability to edit or delete both configuration groups and individual configurations after you have created them:

![](<../.gitbook/assets/image (2).png>)
