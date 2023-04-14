# Webhooks

## Introduction

Welcome to the [Qase.io](https://qase.io/) Webhooks documentation! Webhooks provide a way to notify your services about changes in Qase. A webhook consists of:

* An entity - the resource that generates the events (e.g. Test Case).
* One or more events (e.g. created).
* A URL - the endpoint where you want Qase to send the event payloads when a matching event happens.

This documentation describes the structure of events and their payloads.

{% hint style="info" %}
Webhooks are available in [Startup](https://help.qase.io/en/articles/5563728-startup-plan), [Business](https://help.qase.io/en/articles/5563727-business-plan), and [Enterprise](https://help.qase.io/en/articles/6640055-enterprise-plan) subscriptions
{% endhint %}

### How to set up webhooks?

Setting up a webhook is easy: navigate to the _Settings_ of a project where webhooks will be needed, then select "Webhooks" and hit "Create new webhook":

<figure><img src="https://downloads.intercomcdn.com/i/o/607941903/3813e7aa6cd8c12c75591774/image.png" alt=""><figcaption></figcaption></figure>

There are a few parameters you need to define for a new webhook:

* _Basic:_
  * _Title:_ a name for your webhook.
  * _Endpoint:_ a URL address that is configured on your side and is accessible to the public web; this address will be where Qase sends a request upon a defined event happening.
  * _Secret:_ we are sending this text as an X-Qase-Secret header so that you can authenticate your webhook,
* _Events:_ in this section, you will set up a trigger for Qase to send a request to the endpoint; there are several to choose from, and it is also possible to enable multiple event-triggers for a single endpoint.
  * _Test Cases:_
    * Create test case
    * Update test case
    * Delete test case
    * Clone test case
  * _Test Suites:_
    * Create test suite
    * Update test suite
    * Delete test suite
    * Clone test suite
  * _Test Plans:_
    * Create test plan
    * Update test plan
    * Delete test plan
  * _Shared Steps:_
    * Create shared step
    * Update shared step
    * Delete shared step
  * _Milestones:_
    * Create milestone
    * Update milestone
    * Delete milestone
  * _Custom Fields:_
    * Create custom field
    * Update custom field
    * Delete custom field
  * _Test Runs:_
    * Test run start
    * Test run aborted
    * Test cases added to run
    * Delete test run
    * Complete test run
    * Public link turned on
  * _Defects:_
    * Create defect
    * Resolve defect
    * Delete defect
  * _Reviews_:
    * Create test review
    * Update test review
    * Approval status change
    * Reviewer added
    * Reviewer removed
    * Merge test review
    * Reopen test review
    * Comment test review
    * Decline test review
    * Delete test review

<figure><img src="https://downloads.intercomcdn.com/i/o/607943846/a34d632632766e769cf7cff9/GIF+1.gif" alt=""><figcaption></figcaption></figure>

## Event structure

Request example:

```json
{
  "event_name": "shared_step.created",
  "timestamp": 1650540646,
  "payload": {
    "hash": "2563d587b756110934vea4185ce31b2b0dbf457c",
    "title": "test",
    "steps": [
      {
        "hash": "ed285acb6c7e575bce2576810c195ed8335e2812",
        "action": "action",
        "expected_result": "",
        "data": "",
        "attachments": []
      }
    ]
  },
  "team_member_id": 40,
  "project_code": "ID"
}
```

All requests that are produced by Qase are `POST` requests with data in `JSON` format with following data structure:

| Parameter        | Type    | Description                                  |
| ---------------- | ------- | -------------------------------------------- |
| event\_name      | string  | Event name                                   |
| timestamp        | integer | Time when event has been triggered           |
| payload          | object  | An object with payload data related to event |
| team\_member\_id | integer | Action initiator                             |
| project\_code    | string  | Project code where the event takes place     |

\
