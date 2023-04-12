# Webhooks

### What are webhooks for?

Webhooks in Qase allow you to create a connection between your own resources and Qase so that when a specific event takes place in Qase, it also sends a request to an endpoint you defined for that particular event.

_<mark style="background-color:purple;">Webhooks are available in</mark>_ [_<mark style="background-color:purple;">Startup</mark>_](https://help.qase.io/en/articles/5563728-startup-plan)_<mark style="background-color:purple;">,</mark>_ [_<mark style="background-color:purple;">Business</mark>_](https://help.qase.io/en/articles/5563727-business-plan)_<mark style="background-color:purple;">, and</mark>_ [_<mark style="background-color:purple;">Enterprise</mark>_](https://help.qase.io/en/articles/6640055-enterprise-plan) _<mark style="background-color:purple;">subscriptions</mark>_

### How to set up webhooks?

Setting up a webhook is easy: navigate to the _Settings_ of a project where webhooks will be needed, then select "Webhooks" and hit "Create new webhook":

<figure><img src="https://downloads.intercomcdn.com/i/o/607941903/3813e7aa6cd8c12c75591774/image.png" alt=""><figcaption></figcaption></figure>

There are a few parameters you need to define for a new webhook:

* _Basic:_
  * _Title:_ a name for your webhook.
  * _Endpoint:_ a URL address that is configured on your side and is accessible to the public web; this address will be where Qase sends a request upon a defined event happening.
  * _Secret:_ we are sending this text as an X-Qase-Secret header so that you can authenticate your webhook,
* _Events:_ in this section, you will set up a trigger for Qase to send a request to the endpoint; there are several to choose from, and it is also possible to enable multiple event-triggers for a single endpoint.
  * [_Test Cases_](https://help.qase.io/en/articles/5563704-test-cases)_:_
    * Create test case
    * Update test case
    * Delete test case
    * Clone test case
  * [_Test Suites_](https://help.qase.io/en/articles/5563705-test-suites)_:_
    * Create test suite
    * Update test suite
    * Delete test suite
    * Clone test suite
  * [_Test Plans_](https://help.qase.io/en/articles/5563703-test-plans)_:_
    * Create test plan
    * Update test plan
    * Delete test plan
  * [_Shared Steps_](https://help.qase.io/en/articles/5563709-shared-steps)_:_
    * Create shared step
    * Update shared step
    * Delete shared step
  * [_Milestones_](https://help.qase.io/en/articles/5563715-milestone)_:_
    * Create milestone
    * Update milestone
    * Delete milestone
  * [_Custom Fields_](https://help.qase.io/en/articles/5563701-custom-fields)_:_
    * Create custom field
    * Update custom field
    * Delete custom field
  * [_Test Runs_](https://help.qase.io/en/articles/5563702-test-runs)_:_
    * Test run start
    * Test run aborted
    * Test cases added to run
    * Delete test run
    * Complete test run
    * Public link turned on
  * [_Defects_](https://help.qase.io/en/articles/5563710-defects)_:_
    * Create defect
    * Resolve defect
    * Delete defect
  * [_Reviews_](https://help.qase.io/en/articles/5563713-test-case-review):
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
