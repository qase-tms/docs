# Entity fields

{% hint style="info" %}
This page is archived, please find the up to date content [here](../analytics/queries-qql-qase-query-language.md#h_06385495fe).
{% endhint %}

### Test case: <a href="#h_0d166dbe38" id="h_0d166dbe38"></a>

<table data-header-hidden><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td><em>Attribute</em></td><td><em>Description</em></td><td><em>Examples</em></td></tr><tr><td><pre><code>id
</code></pre></td><td>identifier</td><td><pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>not id in [1, 2, 10]
</code></pre></td></tr><tr><td><pre><code>title
</code></pre><pre><code>preconditions
</code></pre><pre><code>postconditions
</code></pre><pre><code>description
</code></pre></td><td>Test case title, pre/postconditions, description</td><td><pre><code>title is "first test"
</code></pre><pre><code>title = "first test"
</code></pre><pre><code>title ~ "rst"
</code></pre><pre><code>title in ["first test", "second test"]
</code></pre></td></tr><tr><td><pre><code>author
</code></pre></td><td>A user that has created a test case</td><td><pre><code>author in ["user1", "user2"]
</code></pre><pre><code>author = "user1" or author = "user2"
</code></pre></td></tr><tr><td><pre><code>author
</code></pre></td><td>If a test case has been created by a reporter app</td><td><pre><code>author = playwright-reporter
</code></pre><pre><code>author = cucumberjs-reporter
</code></pre><pre><code>author = cypress-reporter
</code></pre><pre><code>author = jest-reporter
</code></pre><pre><code>author = newman-reporter
</code></pre><pre><code>author = testcafe-reporter
</code></pre><pre><code>author = cucumber3-reporter
</code></pre><pre><code>author = cucumber4-reporter
</code></pre><pre><code>author = cucumber5-reporter
</code></pre><pre><code>author = junit4-reporter
</code></pre><pre><code>author = junit5-reporter
</code></pre><pre><code>author = testng-reporter
</code></pre><pre><code>author = pytest-reporter
</code></pre><pre><code>author = robotframework-reporter
</code></pre><pre><code>author = xctest-reporter
</code></pre><pre><code>author = phpunit-reporter
</code></pre><pre><code>author = codeception-reporter
</code></pre></td></tr><tr><td><pre><code>cf
</code></pre></td><td>Custom fields. A complicated attribute with a specific syntax, see examples</td><td><pre><code>cf["Epic"] = "Auth"
</code></pre><pre><code>cf["Story"] in ["Story 1", "Story 2"]
</code></pre><pre><code>cf["Epic"] is null
</code></pre></td></tr><tr><td><pre><code>cfv
</code></pre></td><td>Custom field values. (by all custom fields)</td><td><pre><code>cfv = "Auth"
</code></pre><pre><code>cfv in ["Story 1", "Story 2"]
</code></pre></td></tr><tr><td><pre><code>status
</code></pre><pre><code>type
</code></pre><pre><code>behavior
</code></pre><pre><code>automation
</code></pre><pre><code>layer
</code></pre><pre><code>priority
</code></pre><pre><code>severity
</code></pre></td><td>Case status, type, behavior, automation, layer</td><td><pre><code>status is "Draft"
</code></pre><pre><code>status = "Active"
</code></pre><pre><code>status != "Deprecated"
</code></pre><pre><code>status in ["Draft", "Active"]
</code></pre></td></tr><tr><td><pre><code>created
</code></pre></td><td>Time of case creation</td><td><pre><code>created >= now("-14d")
</code></pre><pre><code>created >= startOfDay("-1m")
</code></pre><pre><code>created &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>createdBy
</code></pre></td><td>The user who created the case</td><td><pre><code>createdBy in ["user1", "user2"]
</code></pre><pre><code>createdBy = "user1" or createdBy = "user2"
</code></pre></td></tr><tr><td><pre><code>updated
</code></pre></td><td>Last modified date</td><td><pre><code>updated >= now("-7d")
</code></pre><pre><code>updated >= startOfDay()
</code></pre><pre><code>updated &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>isDeleted
</code></pre></td><td>Check whether the case has been deleted or not</td><td><pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre></td></tr><tr><td><pre><code>isFlaky
</code></pre></td><td>Check whether the case has been flagged as flaky</td><td><pre><code>isFlaky is false
</code></pre><pre><code>isFlaky = true
</code></pre></td></tr><tr><td><pre><code>project
</code></pre></td><td>Project's code, where to search case. If not specified, the search is performed among all available to user projects</td><td><pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre></td></tr><tr><td><pre><code>suite
</code></pre></td><td>Test case's suite title</td><td><pre><code>suite ~ 'auth'
</code></pre><pre><code>suite != 'auth'
</code></pre></td></tr><tr><td><pre><code>milestone
</code></pre></td><td>Test case's milestone title</td><td><pre><code>milestone = 'Sprint 24'
</code></pre></td></tr><tr><td><pre><code>tags
</code></pre></td><td>Test case's tags</td><td><pre><code>tags not in ['tag']
</code></pre></td></tr></tbody></table>

### Defects: <a href="#h_d6d0c91118" id="h_d6d0c91118"></a>

<table data-header-hidden><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td><em>Attribute</em></td><td><em>Description</em></td><td><em>Examples</em></td></tr><tr><td><pre><code>id
</code></pre></td><td>identifier</td><td><pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>not id in [1, 2, 10]
</code></pre></td></tr><tr><td><pre><code>title
</code></pre></td><td>Defect title</td><td><pre><code>title is "first test"
</code></pre><pre><code>title = "first test"
</code></pre><pre><code>title ~ "rst"
</code></pre><pre><code>title in ["first test", "second test"]
</code></pre></td></tr><tr><td><pre><code>actual_result
</code></pre></td><td>Actual result</td><td><pre><code>actual_result is "first"
</code></pre><pre><code>actual_result = "first"
</code></pre><pre><code>actual_result ~ "rst"
</code></pre><pre><code>actual_result in ["first", "second"]
</code></pre></td></tr><tr><td><pre><code>project
</code></pre></td><td>Project</td><td><pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre></td></tr><tr><td><pre><code>status
</code></pre></td><td>Status (open, resolved, in progress, invalid)</td><td><pre><code>status is "Open"
</code></pre><pre><code>status = "Resolved"
</code></pre><pre><code>status != "Invalid"
</code></pre><pre><code>status in ["Open", "Invalid"]
</code></pre></td></tr><tr><td><pre><code>severity
</code></pre></td><td>Severity (undefined, blocker, critical, major, normal, minor, trivial)</td><td><pre><code>severity is "blocker"
</code></pre><pre><code>severity = "blocker"
</code></pre><pre><code>severity != "blocker"
</code></pre><pre><code>severity in ["blocker", "critical"]
</code></pre></td></tr><tr><td><pre><code>author
</code></pre></td><td>The user who created the defect</td><td><pre><code>author in ["user1", "user2"]
</code></pre><pre><code>author = "user1"
</code></pre></td></tr><tr><td><pre><code>author
</code></pre></td><td>If a defect has been created by a reporter app</td><td><pre><code>author = playwright-reporter
</code></pre><pre><code>author = cucumberjs-reporter
</code></pre><pre><code>author = cypress-reporter
</code></pre><pre><code>author = jest-reporter
</code></pre><pre><code>author = newman-reporter
</code></pre><pre><code>author = testcafe-reporter
</code></pre><pre><code>author = cucumber3-reporter
</code></pre><pre><code>author = cucumber4-reporter
</code></pre><pre><code>author = cucumber5-reporter
</code></pre><pre><code>author = junit4-reporter
</code></pre><pre><code>author = junit5-reporter
</code></pre><pre><code>author = testng-reporter
</code></pre><pre><code>author = pytest-reporter
</code></pre><pre><code>author = robotframework-reporter
</code></pre><pre><code>author = xctest-reporter
</code></pre><pre><code>author = phpunit-reporter
</code></pre><pre><code>author = codeception-reporter
</code></pre></td></tr><tr><td><pre><code>createdBy
</code></pre></td><td>The user who created the defect</td><td><pre><code>createdBy in ["user1", "user2"]
</code></pre><pre><code>createdBy = "user1" or createdBy = "user2"
</code></pre></td></tr><tr><td><pre><code>created
</code></pre></td><td>Time of creation</td><td><pre><code>created >= now("-14d")
</code></pre><pre><code>created >= startOfDay("-1m")
</code></pre><pre><code>created &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>updated
</code></pre></td><td>Time of update</td><td><pre><code>updated >= now("-14d")
</code></pre><pre><code>updated >= startOfDay("-1m")
</code></pre><pre><code>updated &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>resolved
</code></pre></td><td>Time of resolution</td><td><pre><code>resolved >= now("-14d")
</code></pre><pre><code>resolved >= startOfDay("-1m")
</code></pre><pre><code>resolved &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>isDeleted
</code></pre></td><td>Whether the defect is deleted</td><td><pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre></td></tr><tr><td><pre><code>isResolved
</code></pre></td><td>Whether the defect is resolved</td><td><pre><code>isResolved is false
</code></pre><pre><code>isResolved = true
</code></pre></td></tr><tr><td><pre><code>milestone
</code></pre></td><td>Defect's milestone title</td><td><pre><code>milestone = 'Milestone title'
</code></pre></td></tr><tr><td><pre><code>cfv
</code></pre></td><td>Custom field values (by all custom fields)</td><td><pre><code>cfv = "Auth"
</code></pre><pre><code>cfv in ["Story 1", "Story 2"]
</code></pre><pre><code>cfv is empty
</code></pre></td></tr><tr><td><pre><code>cf
</code></pre></td><td>Custom fields. A complicated attribute with a specific syntax, see examples</td><td><pre><code>cf["Epic"] = "Auth"
</code></pre><pre><code>cf["Story"] in ["Story 1", "Story 2"]
</code></pre><pre><code>cf["Epic"] is null
</code></pre></td></tr><tr><td><pre><code>tags
</code></pre></td><td>Defect's tags</td><td><pre><code>tags not in ['tag']
</code></pre></td></tr></tbody></table>

### Test run: <a href="#h_340289e352" id="h_340289e352"></a>

<table data-header-hidden><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td><em>Attribute</em></td><td><em>Description</em></td><td><em>Examples</em></td></tr><tr><td><pre><code>id
</code></pre></td><td>Identifier</td><td><pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>id not in [1, 2, 10]
</code></pre></td></tr><tr><td><pre><code>title
</code></pre></td><td>Title</td><td><pre><code>title is "first test"
</code></pre><pre><code>title = "first test"
</code></pre><pre><code>title ~ "rst"
</code></pre><pre><code>title in ["first test", "second test"]
</code></pre></td></tr><tr><td><pre><code>description
</code></pre></td><td>Description</td><td><pre><code>description is "first"
</code></pre><pre><code>description = "first"
</code></pre><pre><code>description ~ "rst"
</code></pre><pre><code>description in ["first", "second"]
</code></pre></td></tr><tr><td><pre><code>project
</code></pre></td><td>Project</td><td><pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre></td></tr><tr><td><pre><code>plan
</code></pre></td><td>Title of the plan used</td><td><pre><code>plan = 'Regression'
</code></pre></td></tr><tr><td><pre><code>status
</code></pre></td><td>Status</td><td><pre><code>status is "Open"
</code></pre><pre><code>status = "Resolved"
</code></pre><pre><code>status != "Invalid"
</code></pre><pre><code>status in ["Open", "Invalid"]
</code></pre></td></tr><tr><td><pre><code>author
</code></pre></td><td>The user who created the run</td><td><pre><code>author in ["user1", "user2"]
</code></pre><pre><code>author = "user1" or createdBy = "user2"
</code></pre></td></tr><tr><td><pre><code>author
</code></pre></td><td>If a test run has been created by a reporter app</td><td><pre><code>author = playwright-reporter
</code></pre><pre><code>author = cucumberjs-reporter
</code></pre><pre><code>author = cypress-reporter
</code></pre><pre><code>author = jest-reporter
</code></pre><pre><code>author = newman-reporter
</code></pre><pre><code>author = testcafe-reporter
</code></pre><pre><code>author = cucumber3-reporter
</code></pre><pre><code>author = cucumber4-reporter
</code></pre><pre><code>author = cucumber5-reporter
</code></pre><pre><code>author = junit4-reporter
</code></pre><pre><code>author = junit5-reporter
</code></pre><pre><code>author = testng-reporter
</code></pre><pre><code>author = pytest-reporter
</code></pre><pre><code>author = robotframework-reporter
</code></pre><pre><code>author = xctest-reporter
</code></pre><pre><code>author = phpunit-reporter
</code></pre><pre><code>author = codeception-reporter
</code></pre></td></tr><tr><td><pre><code>createdBy
</code></pre></td><td>The user who created the run</td><td><pre><code>createdBy in ["user1", "user2"]
</code></pre><pre><code>createdBy = "user1" or createdBy = "user2"
</code></pre></td></tr><tr><td><pre><code>started
</code></pre></td><td>Time of start</td><td><pre><code>started >= now("-14d")
</code></pre><pre><code>started >= startOfDay("-1m")
</code></pre><pre><code>started &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>ended
</code></pre></td><td>Time of finish</td><td><pre><code>ended >= now("-14d")
</code></pre><pre><code>ended >= startOfDay("-1m")
</code></pre><pre><code>ended &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>deleted
</code></pre></td><td>Time of removal</td><td><pre><code>deleted >= now("-14d")
</code></pre><pre><code>deleted >= startOfDay("-1m")
</code></pre><pre><code>deleted &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>isDeleted
</code></pre></td><td>Whether the run is deleted</td><td><pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre></td></tr><tr><td><pre><code>isStarted
</code></pre></td><td>Whether the run is started</td><td><pre><code>isStarted is false
</code></pre><pre><code>isStarted = true
</code></pre></td></tr><tr><td><pre><code>isEnded
</code></pre></td><td>Whether the run is ended</td><td><pre><code>isEnded is false
</code></pre><pre><code>isEnded = true
</code></pre></td></tr><tr><td><pre><code>isPublic
</code></pre></td><td>Whether the run has a public link</td><td><pre><code>isPublic is false
</code></pre><pre><code>isPublic = true
</code></pre></td></tr><tr><td><pre><code>isAutotest
</code></pre></td><td>Whether the run is automated</td><td><pre><code>isAutotest is false
</code></pre><pre><code>isAutotest = true
</code></pre></td></tr><tr><td><pre><code>Milestone
</code></pre></td><td>Run's milestone title</td><td><pre><code>milestone = 'Milestone title'
</code></pre></td></tr><tr><td><pre><code>cfv
</code></pre></td><td>Custom field values (by all custom fields)</td><td><pre><code>cfv = "Auth"
</code></pre><pre><code>cfv in ["Story 1", "Story 2"]
</code></pre><pre><code>cfv is empty
</code></pre></td></tr><tr><td><pre><code>cf
</code></pre></td><td>Custom fields. A complicated attribute with a specific syntax, see examples</td><td><pre><code>cf["Epic"] = "Auth"
</code></pre><pre><code>cf["Story"] in ["Story 1", "Story 2"]
</code></pre><pre><code>cf["Epic"] is null
</code></pre></td></tr><tr><td><pre><code>tags
</code></pre></td><td>Run's tags</td><td><pre><code>tags not in ['tag']
</code></pre></td></tr></tbody></table>

### Test run results: <a href="#h_442329b3b5" id="h_442329b3b5"></a>

<table data-header-hidden><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td><em>Attribute</em></td><td><em>Description</em></td><td><em>Examples</em></td></tr><tr><td><pre><code>id
</code></pre></td><td>Identifier</td><td><pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>not id in [1, 2, 10]
</code></pre></td></tr><tr><td><pre><code>comment
</code></pre></td><td>Comment</td><td><pre><code>comment is "first test"
</code></pre><pre><code>comment = "first test"
</code></pre><pre><code>comment ~ "rst"
</code></pre><pre><code>comment in ["first test", "second test"]
</code></pre></td></tr><tr><td><pre><code>case
</code></pre></td><td>Test Run Result's case title</td><td><pre><code>case is "first"
</code></pre><pre><code>case = "first"
</code></pre><pre><code>case ~ "rst"
</code></pre><pre><code>case in ["first", "second"]
</code></pre></td></tr><tr><td><pre><code>run
</code></pre></td><td>Test Run title</td><td><pre><code>run is "first"
</code></pre><pre><code>run = "first"
</code></pre><pre><code>run ~ "rst"
</code></pre><pre><code>run in ["first", "second"]
</code></pre></td></tr><tr><td><pre><code>project
</code></pre></td><td>Project</td><td><pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre></td></tr><tr><td><pre><code>status
</code></pre></td><td>Status (Passed, Failed, Blocked, Retest, Skipped, Deleted, In progress, Invalid)</td><td><pre><code>status is "Invalid"
</code></pre><pre><code>status = "Invalid"
</code></pre><pre><code>status != "Invalid"
</code></pre><pre><code>status in ["Invalid", "Failed"]
</code></pre></td></tr><tr><td><pre><code>author
</code></pre><pre><code>assignee
</code></pre></td><td>The user who created the result</td><td><pre><code>author in ["user1", "user2"]
</code></pre><pre><code>author = "user1" or createdBy = "user2"
</code></pre></td></tr><tr><td><pre><code>author
</code></pre><pre><code>assignee
</code></pre></td><td>If a test run result has been created by a reporter app</td><td><pre><code>author = playwright-reporter
</code></pre><pre><code>author = cucumberjs-reporter
</code></pre><pre><code>author = cypress-reporter
</code></pre><pre><code>author = jest-reporter
</code></pre><pre><code>author = newman-reporter
</code></pre><pre><code>author = testcafe-reporter
</code></pre><pre><code>author = cucumber3-reporter
</code></pre><pre><code>author = cucumber4-reporter
</code></pre><pre><code>author = cucumber5-reporter
</code></pre><pre><code>author = junit4-reporter
</code></pre><pre><code>author = junit5-reporter
</code></pre><pre><code>author = testng-reporter
</code></pre><pre><code>author = pytest-reporter
</code></pre><pre><code>author = robotframework-reporter
</code></pre><pre><code>author = xctest-reporter
</code></pre><pre><code>author = phpunit-reporter
</code></pre><pre><code>author = codeception-reporter
</code></pre></td></tr><tr><td><pre><code>createdBy
</code></pre></td><td>The user who created the run</td><td><pre><code>createdBy in ["user1", "user2"]
</code></pre><pre><code>createdBy = "user1" or createdBy = "user2"
</code></pre></td></tr><tr><td><pre><code>ended
</code></pre></td><td>Time of finish</td><td><pre><code>ended >= now("-14d")
</code></pre><pre><code>ended >= startOfDay("-1m")
</code></pre><pre><code>ended &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>deleted
</code></pre></td><td>Time of removal</td><td><pre><code>deleted >= now("-14d")
</code></pre><pre><code>deleted >= startOfDay("-1m")
</code></pre><pre><code>deleted &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>isDeleted
</code></pre></td><td>Whether the result is deleted</td><td><pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre></td></tr><tr><td><pre><code>isEnded
</code></pre></td><td>Whether the result is ended</td><td><pre><code>isEnded is false
</code></pre><pre><code>isEnded = true
</code></pre></td></tr><tr><td><pre><code>timeSpent
</code></pre></td><td>Time spent (in milliseconds)</td><td><pre><code>timeSpent > 10000
</code></pre></td></tr></tbody></table>

### Test plan: <a href="#h_e9113559bb" id="h_e9113559bb"></a>

<table data-header-hidden><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td><em>Attribute</em></td><td><em>Description</em></td><td><em>Examples</em></td></tr><tr><td><pre><code>id
</code></pre></td><td>Identifier</td><td><pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>not id in [1, 2, 10]
</code></pre></td></tr><tr><td><pre><code>title
</code></pre></td><td>Title</td><td><pre><code>title is "first test"
</code></pre><pre><code>title = "first test"
</code></pre><pre><code>title ~ "rst"
</code></pre><pre><code>title in ["first test", "second test"]
</code></pre></td></tr><tr><td><pre><code>description
</code></pre></td><td>Plan's description</td><td><pre><code>description is "first test"
</code></pre><pre><code>description = "first test"
</code></pre><pre><code>description ~ "rst"
</code></pre><pre><code>description in ["first test", "second test"]
</code></pre></td></tr><tr><td><pre><code>project
</code></pre></td><td>Project</td><td><pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre></td></tr><tr><td><pre><code>created
</code></pre></td><td>Time of creation</td><td><pre><code>created >= now("-14d")
</code></pre><pre><code>created >= startOfDay("-1m")
</code></pre><pre><code>created &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>updated
</code></pre></td><td>Time of the last update</td><td><pre><code>updated >= now("-14d")
</code></pre><pre><code>updated >= startOfDay("-1m")
</code></pre><pre><code>updated &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>deleted
</code></pre></td><td>Time of deletion</td><td><pre><code>deleted >= now("-14d")
</code></pre><pre><code>deleted >= startOfDay("-1m")
</code></pre><pre><code>deleted &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>isDeleted
</code></pre></td><td>Whether the plan is deleted</td><td><pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre></td></tr></tbody></table>

### Requirement: <a href="#h_c47f8c5b2f" id="h_c47f8c5b2f"></a>

<table data-header-hidden><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td><em>Attribute</em></td><td><em>Description</em></td><td><em>Examples</em></td></tr><tr><td><pre><code>id
</code></pre></td><td>Identifier</td><td><pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>not id in [1, 2, 10]
</code></pre></td></tr><tr><td><pre><code>parent
</code></pre></td><td>Parent requirement's title</td><td><pre><code>parent is "first test"
</code></pre><pre><code>parent = "first test"
</code></pre><pre><code>parent ~ "rst"
</code></pre><pre><code>parent in ["first test", "second test"]
</code></pre></td></tr><tr><td><pre><code>project
</code></pre></td><td>Project</td><td><pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre></td></tr><tr><td><pre><code>author
</code></pre></td><td>The user who created the requirement</td><td><pre><code>author in ["user1", "user2"]
</code></pre><pre><code>author = "user1" or createdBy = "user2"
</code></pre></td></tr><tr><td><pre><code>createdBy
</code></pre></td><td>The user who created the requirement</td><td><pre><code>createdBy in ["user1", "user2"]
</code></pre><pre><code>createdBy = "user1" or createdBy = "user2"
</code></pre></td></tr><tr><td><pre><code>title
</code></pre></td><td>Title</td><td><pre><code>title is "first test"
</code></pre><pre><code>title = "first test"
</code></pre><pre><code>title ~ "rst"
</code></pre><pre><code>title in ["first test", "second test"]
</code></pre></td></tr><tr><td><pre><code>description
</code></pre></td><td>Description</td><td><pre><code>description is "first test"
</code></pre><pre><code>description = "first test"
</code></pre><pre><code>description ~ "rst"
</code></pre><pre><code>description in ["first test", "second test"]
</code></pre></td></tr><tr><td><pre><code>status
</code></pre></td><td>Status (valid, draft, review, rework, finish, implemented, not-testable, obsolete)</td><td><pre><code>status = 'valid'
</code></pre></td></tr><tr><td><pre><code>type
</code></pre></td><td>Type (epic, user-story, feature)</td><td><pre><code>type = 'epic'
</code></pre></td></tr><tr><td><pre><code>created
</code></pre></td><td>Time of creation</td><td><pre><code>created >= now("-14d")
</code></pre><pre><code>created >= startOfDay("-1m")
</code></pre><pre><code>created &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>updated
</code></pre></td><td>Time of last update</td><td><pre><code>updated >= now("-14d")
</code></pre><pre><code>updated >= startOfDay("-1m")
</code></pre><pre><code>updated &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>deleted
</code></pre></td><td>Time of deletion</td><td><pre><code>deleted >= now("-14d")
</code></pre><pre><code>deleted >= startOfDay("-1m")
</code></pre><pre><code>deleted &#x3C; 1569430502709
</code></pre></td></tr><tr><td><pre><code>isDeleted
</code></pre></td><td>Whether the requirement is deleted</td><td><pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre></td></tr></tbody></table>

\
