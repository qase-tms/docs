---
title: Dashboards
slug: dashboards
createdAt: '2023-02-24T12:41:33.729Z'
updatedAt: '2023-02-24T12:41:33.729Z'
---

# Dashboards

## What are dashboards? <a href="#h_c79968f961" id="h_c79968f961"></a>

Dashboards are a feature designed to provide you with a comprehensive understanding of their projects through statistical and analytical data.

You can create as many dashboards as you need, and each dashboard is fully customizable and can be shared with team members or external stakeholders with just a few clicks.

_<mark style="background-color:purple;">Dashboards are available in</mark>_ [_<mark style="background-color:purple;">Startup</mark>_](https://help.qase.io/en/articles/5563728-startup-plan)_<mark style="background-color:purple;">,</mark>_ [_<mark style="background-color:purple;">Business</mark>_](https://help.qase.io/en/articles/5563727-business-plan)_<mark style="background-color:purple;">, and</mark>_ [_<mark style="background-color:purple;">Enterprise</mark>_](https://help.qase.io/en/articles/6640055-enterprise-plan) _<mark style="background-color:purple;">subscriptions.</mark>_

{% embed url="https://www.youtube.com/watch?v=RjnB9vheSno" %}

{% embed url="https://www.youtube.com/watch?v=pG6-3w79Ixs" %}

## The Get Started Dashboard <a href="#h_14f3532814" id="h_14f3532814"></a>

***

The Get Started Dashboard is designed to let you dive right into your analytics and customize as you go.

<figure><img src="../../../.gitbook/assets/get started.gif" alt=""><figcaption></figcaption></figure>



Setting up a dashboard from scratch can be time-consuming and overwhelming, especially when managing multiple projects and teams. To simplify this process, your workspace includes a Get Started Dashboard, providing an immediate overview of your team’s work.

This dashboard is automatically added to your workspace and comes included by default when you sign up. It features the most-used widgets from QA teams across the industry.

The Get Started Dashboard offers:

* **Pre-Configured Widgets:** Includes essential widgets that draw data from all projects in your workspace, offering a comprehensive view of your team’s activities.
* **Instant Insights:** Provides analytics without needing initial setup.
* **Customizability:** Allows you to:
  * Filter data based on various parameters.
  * Remove or add widgets to customize the view.
  * Change the dashboard name to better reflect its purpose.

## Creating a dashboard <a href="#h_0e60fadcdc" id="h_0e60fadcdc"></a>

***

If you prefer to build a dashboard from scratch to meet specific needs or preferences, let’s explore how you can create a custom dashboard tailored to your requirements.

* First off, give your dashboard a **Title** \[1] (mandatory) and add a brief **description** \[2]:
* Next up, choose the dashboard **visibility** \[3]: you can keep it private to yourself or make it public for the entire team to use:

<figure><img src="../../../.gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure>

* Finally, pick[ projects](https://docs.qase.io/general/get-started-with-the-qase-platform/create-a-project) to base your dashboard on. If you select "All projects," the dashboard will gather data on all projects available to you. You can also choose just one project or any selection of projects to feed the data into your dashboard. If a dashboard is made public, every user will only see data regarding the projects they have access to.

<figure><img src="../../../.gitbook/assets/select projects.gif" alt=""><figcaption></figcaption></figure>

Once configured, you can always go back to editing your dashboard's parameters via the Settings button:

<figure><img src="../../../.gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure>

## Dashboard Filters <a href="#h_7b846e864f" id="h_7b846e864f"></a>

***

You can retrieve precise data within your dashboard widgets with the help of Filters.

<figure><img src="../../../.gitbook/assets/new filter.gif" alt=""><figcaption></figcaption></figure>

Currently, the filters are available for the following widget types -

* Single Value
* Time Value
* Distribution Charts

_We’re expanding these filters to include more parameters, and extend the filters to Time Series widget type._



## Compare metrics across different projects / time periods <a href="#h_a33472ffa2" id="h_a33472ffa2"></a>

***

To gain a comprehensive understanding of your projects’ performance, you can _compare_ various metrics _across different projects_ or _time periods_ using the diverse widget types available.

<figure><img src="../../../.gitbook/assets/duplicate.gif" alt=""><figcaption><p><code>Easily duplicate widgets, to view the same metric across diffrent projects</code></p></figcaption></figure>

**Identify Trends**:  Track changes in metrics such as test case counts, defect statuses, or test results over selected [time periods](https://help.qase.io/en/articles/5563698-dashboards#h\_537d98ced2), and compare these trends across multiple projects to spot patterns or anomalies.

**Analyze Project Performance**:  Use widgets like [Time Series](https://help.qase.io/en/articles/5563698-dashboards#h\_c16702bf28) and [Distribution Charts](https://help.qase.io/en/articles/5563698-dashboards#h\_6a4018eda2) to assess the performance and distribution of metrics across different projects, helping to pinpoint strengths and areas for improvement.

**Benchmark Against Standards**:  Utilize [Single Value](https://help.qase.io/en/articles/5563698-dashboards#h\_f1f898c3a1) widgets to compare current metrics with historical data, providing insight into whether your projects are meeting predefined benchmarks or goals.



## Widgets: Types <a href="#h_d8cf1d9256" id="h_d8cf1d9256"></a>

***

When you are ready to begin adding widgets. hit the "+Add widget" button:

<figure><img src="../../../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

Several widgets are available; in the modal window, they are broken down into two groups: "**By Type**" and "**By Entity.**"

In the _Entities_ group, you can find widgets related to each specific entity - there are widgets for test cases, test runs, test results, defects, requirements, and custom fields.

_Type_ grouping collects different types of widgets:

* _**Single Value**:_ a single value chart shows a single value that represents the current state of the entity. This chart type answers the following question: “How many artifacts do we have at the moment?“.
* _**Timed Value**:_ a timed value chart shows a cumulative sum of events that happened to some entity. This chart answers the following question: “How many artifacts have been created this day/week/month?".
* _**Distribution charts**:_ this chart shows the current distribution of various test case properties or custom field values.
* _**Time-series:**_ a time-series chart shows changes for a specific entity type over a selected period of time.
* _**Table:**_ data is presented in a table format, with an option to display select columns.

Let's have a closer look at each of the widgets available:

### &#x20;Single Value <a href="#h_f1f898c3a1" id="h_f1f898c3a1"></a>

***

<figure><img src="../../../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

*   #### _Single Value: Test Cases Count_ <a href="#h_1fcb165132" id="h_1fcb165132"></a>

    _​_This widget shows the number of test cases you have in a project or projects at the moment and how it has increased or decreased over the specified time period.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.34.20 PM.png" alt=""><figcaption></figcaption></figure>



*   #### _Single Value: Opened Defects Count_ <a href="#h_99ebeeb888" id="h_99ebeeb888"></a>

    This widget shows the number of defects you have in a project or projects at the moment and how it has increased or decreased over the specified time period.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.36.37 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Single Value: Active Test Runs Count_ <a href="#h_7acf63fd10" id="h_7acf63fd10"></a>

This widget shows the number of active test runs you have in a project or projects at the moment and how it has increased or decreased over the specified time period.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.52.12 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Single Value: Requirements Count_ <a href="#h_ef76ad82f8" id="h_ef76ad82f8"></a>

This widget shows the number of requirements you have in a project or projects at the moment and how it has increased or decreased over the specified time period.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.52.30 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Single Value: Suite Count_ <a href="#h_efa23c2835" id="h_efa23c2835"></a>

This widget shows the number of suites you have in a project or projects at the moment and how it has increased or decreased over the specified time period.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.52.49 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Single Value: Open Review Requests_ <a href="#h_5274ffed5c" id="h_5274ffed5c"></a>

This widget shows the number of open (unprocessed) review requests you have in a project or projects at the moment and how it has increased or decreased over the specified time period.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.53.06 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Single Value: Test Cases Automation Ratio_ <a href="#h_f2dbcc6e36" id="h_f2dbcc6e36"></a>

This widget shows the percentage of automated test cases you have in a project or projects at the moment and how it has increased or decreased over the specified time period. It is based on an "Automation Status" property of test cases.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.53.30 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Single Value: Flaky Test Cases Count_ <a href="#h_4e8040f7ad" id="h_4e8040f7ad"></a>

This widget shows the number of flaky test cases you have in a project or projects at the moment and how it has increased or decreased over the specified time period. It is based on an "Is Flaky" property of test cases.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.53.53 PM.png" alt=""><figcaption></figcaption></figure>

**Note:** You can select the benchmark time period in the widget settings for all Single value widgets.

<figure><img src="../../../.gitbook/assets/benchmark time.gif" alt=""><figcaption></figcaption></figure>

### Timed Value <a href="#h_537d98ced2" id="h_537d98ced2"></a>

***

<figure><img src="../../../.gitbook/assets/image (57).png" alt=""><figcaption></figcaption></figure>

* #### _Timed Value: Test Cases Events_ <a href="#h_e6008bf395" id="h_e6008bf395"></a>

This widget shows the number of test cases that have been created, updated, or deleted in a project/projects over a specified period of time, and how this number has increased or decreased over a specified period of time.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.56.27 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Timed Value: Defects Events_ <a href="#h_7b571e1e31" id="h_7b571e1e31"></a>

This widget shows the number of defects that have been created, updated, or deleted in a project/projects over a specified period of time, and how this number has increased or decreased over a specified period of time.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.56.45 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Timed Value: Test Results Events_ <a href="#h_75a68b0f59" id="h_75a68b0f59"></a>

This widget shows the number of specific test results that have been submitted during test runs in a project/projects over a specified period of time, and how this number has increased or decreased over a specified period of time.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.57.05 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Timed Value: Test Run Events_ <a href="#h_883249c7ea" id="h_883249c7ea"></a>

This widget shows the number of test runs that have been created, completed, or aborted in a project/projects over a specified period of time, and how this number has increased or decreased over a specified period of time.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 4.57.23 PM.png" alt=""><figcaption></figcaption></figure>

**Note:** The type of event (created/completed/aborted) and the time range can be selected in the widget settings for all Timed Value widgets.



<figure><img src="../../../.gitbook/assets/image (58).png" alt=""><figcaption></figcaption></figure>

### Distribution Chart <a href="#h_6a4018eda2" id="h_6a4018eda2"></a>

***

<figure><img src="../../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

*   #### _Distribution Chart: Test Case Property Distribution_ <a href="#h_db943c6200" id="h_db943c6200"></a>

    This chart shows the distribution of test cases by one of their properties. It can be represented as either a donut graph or a bar graph. Available properties are Status, Type, Behavior, Priority, Severity, Automation, and Layer.

<figure><img src="../../../.gitbook/assets/image (60).png" alt=""><figcaption></figcaption></figure>

\


<figure><img src="../../../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

* #### _Distribution Chart: Custom Field Values Distribution_ <a href="#h_52022de51f" id="h_52022de51f"></a>

This chart shows the distribution of test cases by one of its custom field values. It can be represented as either a donut graph or a bar graph. Supported Custom Field data types are Select List (Single/Multi), Radiobutton, and Checkbox.

<figure><img src="../../../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

### Time Series <a href="#h_c16702bf28" id="h_c16702bf28"></a>

***

<figure><img src="../../../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

* #### _Time Series: Test Cases Count_ <a href="#h_fad8989888" id="h_fad8989888"></a>

This graph shows the number of test cases as of the current day as well as how it has been changing over the specified period.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 5.01.23 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Time Series: Test Cases Events_ <a href="#h_bc075fb847" id="h_bc075fb847"></a>

This graph shows the number of test case events (creation, updates, or deletions) as of the current day as well as how it has been changing over the specified period.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 5.01.51 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Time Series: Test Cases Automation Ratio_ <a href="#h_160f85dfd4" id="h_160f85dfd4"></a>

This graph shows how many automated test cases you have in a project or projects at the moment and how these numbers have been changing over time. It is based on an "Automation Status" property of test cases.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 5.02.10 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Time Series: Test Cases Automation Velocity:_ <a href="#h_2caf3f5e49" id="h_2caf3f5e49"></a>

This graph shows how quickly your test cases with a “To Be Automated” status have been automated and how these numbers have changed over time. It is based on an "Automation Status" property and only applies to the automation statuses “To Be Automated” and “Automated.”

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 5.02.36 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Time Series: Flaky Test Cases Count_ <a href="#h_2471838fe2" id="h_2471838fe2"></a>

This graph shows the number of flaky test cases and how these numbers have been changing over time. It is based on an "Is Flaky" property of test cases.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 5.02.56 PM.png" alt=""><figcaption></figcaption></figure>

* #### _Time Series: Test Results Events_ <a href="#h_8af8173f9f" id="h_8af8173f9f"></a>

This graph shows the number of test results recorded (creation, updates, or deletions) as of the current day as well as how it has been changing over the specified period and which results were recorded.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-07-10 at 5.03.15 PM.png" alt=""><figcaption></figcaption></figure>

**Note:** You can select the “Period” and “Dimension” in the widget settings for all Time Series widget type.

<figure><img src="../../../.gitbook/assets/time series.gif" alt=""><figcaption></figcaption></figure>

### Table: Qase Query Language (QQL) <a href="#h_9644c6d14d" id="h_9644c6d14d"></a>

***

<mark style="background-color:green;">With the</mark> [<mark style="background-color:green;">QQL</mark>](https://docs.qase.io/general/analytics/queries) <mark style="background-color:green;">widget, you can leverage advanced query searches, and pin</mark> [<mark style="background-color:green;">frequently used or preferred QQL searches</mark>](https://docs.qase.io/general/analytics/queries/saved-queries) <mark style="background-color:green;">to your dashboards to facilitate quicker and more comprehensive monitoring of testing activities.</mark>

<figure><img src="../../../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

This widget presents data in a table format based on your [_saved queries_](https://docs.qase.io/general/analytics/queries/saved-queries) _\[1]_. You have the flexibility to select and customize which _fields \[2]_ are displayed in the query table.



<figure><img src="../../../.gitbook/assets/qql-widget (1).gif" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/GIF Recording 2024-05-06 at 4.04.24 PM.gif" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>

\
You have the option to expand the widget to view additional rows or click "_see all_" to access the Query directly for more detailed information.

Additionally, you can create multiple widgets for the same query, each with different fields, allowing for easy comparison.

<figure><img src="../../../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>

_**Please note**_, once the widget is created:

* You can modify your widget configuration whenever necessary, as well as edit the original query.
* If changes are made to the original query and the new results don't align with your widget configuration, you will be prompted to adjust the configuration to display the updated results.
* Users with limited permissions will only see query information that aligns with their allowed access levels.

## Share Dashboard <a href="#h_d2a398d461" id="h_d2a398d461"></a>

***

Provide access to a report to anyone who needs to view project progress - even if they are not your Qase account members - with a public link.

\


<figure><img src="../../../.gitbook/assets/image 69.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>
