---
title: How to use Environments in Qase
slug: environments-1
hidden: true
createdAt: '2023-02-24T12:53:22.196Z'
updatedAt: '2023-02-27T18:47:35.491Z'
---

# How to use Environments in Qase

What are environments in a test case management system?

Environments in a test case management system are an additional entity which allows you to represent your real-life infrastructure environments and then specify which of the environment a Test Run should be executed in.&#x20;

{% embed url="https://www.youtube.com/watch?v=7XLLVD8c8x4" %}

In order to create an environment in Qase, go to the Project's "Environments" tab, then click "Create new environment":

![](<../.gitbook/assets/image (3).png>)&#x20;

Define the environment's properties:

![](<../.gitbook/assets/image (5).png>)

Fix a Title: mandatory field, descriptive name of an environment which will be appearing in the test runs (i.e., Production Env)

Insert a Slug: This is a mandatory field of a URL-friendly shortened version of the title (i.e., “prod”)

Input a Description: This is an optional field for extra context about the environment and what it's to be used for

Include a Host: This is another optional field and should be the URL address of the environment (as a reference)

Once completed, your new environment can be used as a property of a Test run when creating or editing Test runs:&#x20;

![](../.gitbook/assets/image.png)
