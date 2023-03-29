# Test run setting

### Where test run settings are located? <a href="#h_2b8f9ef7e0" id="h_2b8f9ef7e0"></a>

If you navigate to project settings, you will find a section dedicated to the options that define how the test run behaves.\


<figure><img src="https://downloads.intercomcdn.com/i/o/610014375/9a470ae62733b2b704ad4894/image.png" alt=""><figcaption></figcaption></figure>

### What changes can I make with a test run?

Let's take a look at those settings and how they change the behavior of the run.

* _Fast Pass:_ if this option is turned on, you won't need to add extra details like comments or attachments when you mark a test case as "passed." If you turn off this option, you'll see a window where you can add extra details when you mark a case as "passed."
* _Default create/attach defect checkbox:_ with this option enabled, the state of the checkbox for creating/attaching a defect will be checked, with the option disabled, the checkbox state will be unchecked by default when you fail or invalidate a case or mark it as "blocked":\


<figure><img src="https://downloads.intercomcdn.com/i/o/597143659/990f84c362fe23d9eaff0b15/image.png" alt=""><figcaption></figcaption></figure>

* _Auto complete:_ with this option enabled, as soon as you submit results for all cases of a run (regardless of which results those are, but _Skipped_ result does not count here) the run itself will get marked completed automatically. With this option disabled, you'll need to mark the run completed manually, even if all the results have been submitted.
* _Auto passed:_ when this option is enabled, once you mark all steps of a case "passed", the entire case will also get marked "passed" automatically. If you have this option disabled, you will need to mark the case "passed" separately, even if all of its steps have been marked as "passed".
* _Auto assignee:_ enabling this option will result in any unassigned test cases getting automatically assigned to the first person opening them in the Wizard. Conversely, if you have this setting switched off, the unassigned cases will remain unassigned even if opened by someone, until they are explicitly assigned to someone specific.
* _Auto create test cases:_ this option relates specifically to automated executions. With this option switched on, if you are sending an automated execution result for a test case that is not yet represented in your Qase repository, such a case will be created automatically (later on, if something changes in that test case upon the next result submission, related test case in the repository will get updated accordingly with this option enabled). With the option switched off, there will be no new cases created, if an automated execution result refers to a non-existent test case in the repository.
* _Fail case on step fail:_ with this option enabled, failing any step of a test case will result in the immediate termination of the entire case and marking it "failed" as well. If you disable the option, even after one of the steps has failed, you will be able to proceed further with the case.
* _Allow to add results for cases in closed runs:_ when this option is enabled, it allows you to continue submitting results for cases, or retest cases in those runs that have been marked complete or aborted. If you switch that option off, any runs that have been completed or aborted would not allow any further result submissions.
* _Assignee result lock:_ when this option is enabled, it restricts other users but the assignee from submitting the results - for someone to submit a result in such a case, they would need to assign themselves to a case explicitly. Conversely, if this option is disabled, any user - even if not assigned to a case - will be able to submit a result for it (however, even though the case would stay assigned to the original assignee, the result itself will be associated with the exact person that submitted the result).
*   _Allow submitting results in bulk:_ when this option is enabled, it allows you to submit a result for multiple test cases - keep in mind that for all cases you can submit the same status, the "time spent" you insert is distributed evenly between the cases you submit a result for, and the comments and attachments added will get attached to every case you submit a result for in bulk:\




    <figure><img src="https://downloads.intercomcdn.com/i/o/597151589/d7690a7b04a8e68211c039e2/image.png" alt=""><figcaption></figcaption></figure>

    <figure><img src="https://downloads.intercomcdn.com/i/o/597151796/05bbe8185dc52bd02c57589e/image.png" alt=""><figcaption></figcaption></figure>

Conversely, if the option is switched off, there will be no way to submit results for cases in bulk.

* _Redirect after adding result:_ this option establishes the policy for where you will be taken after the result has been submitted, there are three options:
  * No redirect - you will stay on the same case for which you have submitted a result;
  * First case in a run without result - you will be redirected to the first case that has no result yet;
  * Next case in suite - you will be taken directly to the next following case in the suite that does not have any result yet.
