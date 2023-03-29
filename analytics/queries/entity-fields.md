# Entity fields

### Test case: <a href="#h_0d166dbe38" id="h_0d166dbe38"></a>

| _Attribute_                                                                                                                                                                                                                      | _Description_                                                                                                        | _Examples_                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <pre><code>id
</code></pre>                                                                                                                                                                                                      | identifier                                                                                                           | <pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>not id in [1, 2, 10]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| <pre><code>title
</code></pre><pre><code>preconditions
</code></pre><pre><code>postconditions
</code></pre><pre><code>description
</code></pre>                                                                                  | Test case title, pre/postconditions, description                                                                     | <pre><code>title is "first test"
</code></pre><pre><code>title = "first test"
</code></pre><pre><code>title ~ "rst"
</code></pre><pre><code>title in ["first test", "second test"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <pre><code>author
</code></pre>                                                                                                                                                                                                  | A user that has created a test case                                                                                  | <pre><code>author in ["user1", "user2"]
</code></pre><pre><code>author = "user1" or author = "user2"
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| <pre><code>author
</code></pre>                                                                                                                                                                                                  | If a test case has been created by a reporter app                                                                    | <pre><code>author = playwright-reporter
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
</code></pre> |
| <pre><code>cf
</code></pre>                                                                                                                                                                                                      | Custom fields. A complicated attribute with a specific syntax, see examples                                          | <pre><code>cf["Epic"] = "Auth"
</code></pre><pre><code>cf["Story"] in ["Story 1", "Story 2"]
</code></pre><pre><code>cf["Epic"] is null
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| <pre><code>cfv
</code></pre>                                                                                                                                                                                                     | Custom field values. (by all custom fields)                                                                          | <pre><code>cfv = "Auth"
</code></pre><pre><code>cfv in ["Story 1", "Story 2"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| <pre><code>status
</code></pre><pre><code>type
</code></pre><pre><code>behavior
</code></pre><pre><code>automation
</code></pre><pre><code>layer
</code></pre><pre><code>priority
</code></pre><pre><code>severity
</code></pre> | Case status, type, behavior, automation, layer                                                                       | <pre><code>status is "Draft"
</code></pre><pre><code>status = "Active"
</code></pre><pre><code>status != "Deprecated"
</code></pre><pre><code>status in ["Draft", "Active"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| <pre><code>created
</code></pre>                                                                                                                                                                                                 | Time of case creation                                                                                                | <pre><code>created >= now("-14d")
</code></pre><pre><code>created >= startOfDay("-1m")
</code></pre><pre><code>created &#x3C; 1569430502709
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| <pre><code>createdBy
</code></pre>                                                                                                                                                                                               | The user who created the case                                                                                        | <pre><code>createdBy in ["user1", "user2"]
</code></pre><pre><code>createdBy = "user1" or createdBy = "user2"
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| <pre><code>updated
</code></pre>                                                                                                                                                                                                 | Last modified date                                                                                                   | <pre><code>updated >= now("-7d")
</code></pre><pre><code>updated >= startOfDay()
</code></pre><pre><code>updated &#x3C; 1569430502709
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| <pre><code>isDeleted
</code></pre>                                                                                                                                                                                               | Check whether the case has been deleted or not                                                                       | <pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| <pre><code>isFlaky
</code></pre>                                                                                                                                                                                                 | Check whether the case has been flagged as flaky                                                                     | <pre><code>isFlaky is false
</code></pre><pre><code>isFlaky = true
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <pre><code>project
</code></pre>                                                                                                                                                                                                 | Project's code, where to search case. If not specified, the search is performed among all available to user projects | <pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| <pre><code>suite
</code></pre>                                                                                                                                                                                                   | Test case's suite title                                                                                              | <pre><code>suite ~ 'auth'
</code></pre><pre><code>suite != 'auth'
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| <pre><code>milestone
</code></pre>                                                                                                                                                                                               | Test case's milestone title                                                                                          | <pre><code>milestone = 'Sprint 24'
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <pre><code>tags
</code></pre>                                                                                                                                                                                                    | Test case's tags                                                                                                     | <pre><code>tags not in ['tag']
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

### Defects: <a href="#h_d6d0c91118" id="h_d6d0c91118"></a>

| _Attribute_                            | _Description_                                                               | _Examples_                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| -------------------------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <pre><code>id
</code></pre>            | identifier                                                                  | <pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>not id in [1, 2, 10]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| <pre><code>title
</code></pre>         | Defect title                                                                | <pre><code>title is "first test"
</code></pre><pre><code>title = "first test"
</code></pre><pre><code>title ~ "rst"
</code></pre><pre><code>title in ["first test", "second test"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <pre><code>actual_result
</code></pre> | Actual result                                                               | <pre><code>actual_result is "first"
</code></pre><pre><code>actual_result = "first"
</code></pre><pre><code>actual_result ~ "rst"
</code></pre><pre><code>actual_result in ["first", "second"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| <pre><code>project
</code></pre>       | Project                                                                     | <pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| <pre><code>status
</code></pre>        | Status (open, resolved, in progress, invalid)                               | <pre><code>status is "Open"
</code></pre><pre><code>status = "Resolved"
</code></pre><pre><code>status != "Invalid"
</code></pre><pre><code>status in ["Open", "Invalid"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| <pre><code>severity
</code></pre>      | Severity (undefined, blocker, critical, major, normal, minor, trivial)      | <pre><code>severity is "blocker"
</code></pre><pre><code>severity = "blocker"
</code></pre><pre><code>severity != "blocker"
</code></pre><pre><code>severity in ["blocker", "critical"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| <pre><code>author
</code></pre>        | The user who created the defect                                             | <pre><code>author in ["user1", "user2"]
</code></pre><pre><code>author = "user1"
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| <pre><code>author
</code></pre>        | If a defect has been created by a reporter app                              | <pre><code>author = playwright-reporter
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
</code></pre> |
| <pre><code>createdBy
</code></pre>     | The user who created the defect                                             | <pre><code>createdBy in ["user1", "user2"]
</code></pre><pre><code>createdBy = "user1" or createdBy = "user2"
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| <pre><code>created
</code></pre>       | Time of creation                                                            | <pre><code>created >= now("-14d")
</code></pre><pre><code>created >= startOfDay("-1m")
</code></pre><pre><code>created &#x3C; 1569430502709
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| <pre><code>updated
</code></pre>       | Time of update                                                              | <pre><code>updated >= now("-14d")
</code></pre><pre><code>updated >= startOfDay("-1m")
</code></pre><pre><code>updated &#x3C; 1569430502709
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| <pre><code>resolved
</code></pre>      | Time of resolution                                                          | <pre><code>resolved >= now("-14d")
</code></pre><pre><code>resolved >= startOfDay("-1m")
</code></pre><pre><code>resolved &#x3C; 1569430502709
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| <pre><code>isDeleted
</code></pre>     | Whether the defect is deleted                                               | <pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| <pre><code>isResolved
</code></pre>    | Whether the defect is resolved                                              | <pre><code>isResolved is false
</code></pre><pre><code>isResolved = true
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| <pre><code>milestone
</code></pre>     | Defect's milestone title                                                    | <pre><code>milestone = 'Milestone title'
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| <pre><code>cfv
</code></pre>           | Custom field values (by all custom fields)                                  | <pre><code>cfv = "Auth"
</code></pre><pre><code>cfv in ["Story 1", "Story 2"]
</code></pre><pre><code>cfv is empty
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <pre><code>cf
</code></pre>            | Custom fields. A complicated attribute with a specific syntax, see examples | <pre><code>cf["Epic"] = "Auth"
</code></pre><pre><code>cf["Story"] in ["Story 1", "Story 2"]
</code></pre><pre><code>cf["Epic"] is null
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| <pre><code>tags
</code></pre>          | Defect's tags                                                               | <pre><code>tags not in ['tag']
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

### Test run: <a href="#h_340289e352" id="h_340289e352"></a>

| _Attribute_                          | _Description_                                                               | _Examples_                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ------------------------------------ | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <pre><code>id
</code></pre>          | Identifier                                                                  | <pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>id not in [1, 2, 10]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| <pre><code>title
</code></pre>       | Title                                                                       | <pre><code>title is "first test"
</code></pre><pre><code>title = "first test"
</code></pre><pre><code>title ~ "rst"
</code></pre><pre><code>title in ["first test", "second test"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <pre><code>description
</code></pre> | Description                                                                 | <pre><code>description is "first"
</code></pre><pre><code>description = "first"
</code></pre><pre><code>description ~ "rst"
</code></pre><pre><code>description in ["first", "second"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| <pre><code>project
</code></pre>     | Project                                                                     | <pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| <pre><code>plan
</code></pre>        | Title of the plan used                                                      | <pre><code>plan = 'Regression'
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| <pre><code>status
</code></pre>      | Status                                                                      | <pre><code>status is "Open"
</code></pre><pre><code>status = "Resolved"
</code></pre><pre><code>status != "Invalid"
</code></pre><pre><code>status in ["Open", "Invalid"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| <pre><code>author
</code></pre>      | The user who created the run                                                | <pre><code>author in ["user1", "user2"]
</code></pre><pre><code>author = "user1" or createdBy = "user2"
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| <pre><code>author
</code></pre>      | If a test run has been created by a reporter app                            | <pre><code>author = playwright-reporter
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
</code></pre> |
| <pre><code>createdBy
</code></pre>   | The user who created the run                                                | <pre><code>createdBy in ["user1", "user2"]
</code></pre><pre><code>createdBy = "user1" or createdBy = "user2"
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| <pre><code>started
</code></pre>     | Time of start                                                               | <pre><code>started >= now("-14d")
</code></pre><pre><code>started >= startOfDay("-1m")
</code></pre><pre><code>started &#x3C; 1569430502709
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| <pre><code>ended
</code></pre>       | Time of finish                                                              | <pre><code>ended >= now("-14d")
</code></pre><pre><code>ended >= startOfDay("-1m")
</code></pre><pre><code>ended &#x3C; 1569430502709
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| <pre><code>deleted
</code></pre>     | Time of removal                                                             | <pre><code>deleted >= now("-14d")
</code></pre><pre><code>deleted >= startOfDay("-1m")
</code></pre><pre><code>deleted &#x3C; 1569430502709
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| <pre><code>isDeleted
</code></pre>   | Whether the run is deleted                                                  | <pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| <pre><code>isStarted
</code></pre>   | Whether the run is started                                                  | <pre><code>isStarted is false
</code></pre><pre><code>isStarted = true
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| <pre><code>isEnded
</code></pre>     | Whether the run is ended                                                    | <pre><code>isEnded is false
</code></pre><pre><code>isEnded = true
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <pre><code>isPublic
</code></pre>    | Whether the run has a public link                                           | <pre><code>isPublic is false
</code></pre><pre><code>isPublic = true
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| <pre><code>isAutotest
</code></pre>  | Whether the run is automated                                                | <pre><code>isAutotest is false
</code></pre><pre><code>isAutotest = true
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| <pre><code>Milestone
</code></pre>   | Run's milestone title                                                       | <pre><code>milestone = 'Milestone title'
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| <pre><code>cfv
</code></pre>         | Custom field values (by all custom fields)                                  | <pre><code>cfv = "Auth"
</code></pre><pre><code>cfv in ["Story 1", "Story 2"]
</code></pre><pre><code>cfv is empty
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <pre><code>cf
</code></pre>          | Custom fields. A complicated attribute with a specific syntax, see examples | <pre><code>cf["Epic"] = "Auth"
</code></pre><pre><code>cf["Story"] in ["Story 1", "Story 2"]
</code></pre><pre><code>cf["Epic"] is null
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| <pre><code>tags
</code></pre>        | Run's tags                                                                  | <pre><code>tags not in ['tag']
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

### Test run results: <a href="#h_442329b3b5" id="h_442329b3b5"></a>

| _Attribute_                                                      | _Description_                                                                    | _Examples_                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ---------------------------------------------------------------- | -------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <pre><code>id
</code></pre>                                      | Identifier                                                                       | <pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>not id in [1, 2, 10]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| <pre><code>comment
</code></pre>                                 | Comment                                                                          | <pre><code>comment is "first test"
</code></pre><pre><code>comment = "first test"
</code></pre><pre><code>comment ~ "rst"
</code></pre><pre><code>comment in ["first test", "second test"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| <pre><code>case
</code></pre>                                    | Test Run Result's case title                                                     | <pre><code>case is "first"
</code></pre><pre><code>case = "first"
</code></pre><pre><code>case ~ "rst"
</code></pre><pre><code>case in ["first", "second"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| <pre><code>run
</code></pre>                                     | Test Run title                                                                   | <pre><code>run is "first"
</code></pre><pre><code>run = "first"
</code></pre><pre><code>run ~ "rst"
</code></pre><pre><code>run in ["first", "second"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| <pre><code>project
</code></pre>                                 | Project                                                                          | <pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| <pre><code>status
</code></pre>                                  | Status (Passed, Failed, Blocked, Retest, Skipped, Deleted, In progress, Invalid) | <pre><code>status is "Invalid"
</code></pre><pre><code>status = "Invalid"
</code></pre><pre><code>status != "Invalid"
</code></pre><pre><code>status in ["Invalid", "Failed"]
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| <pre><code>author
</code></pre><pre><code>assignee
</code></pre> | The user who created the result                                                  | <pre><code>author in ["user1", "user2"]
</code></pre><pre><code>author = "user1" or createdBy = "user2"
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| <pre><code>author
</code></pre><pre><code>assignee
</code></pre> | If a test run result has been created by a reporter app                          | <pre><code>author = playwright-reporter
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
</code></pre> |
| <pre><code>createdBy
</code></pre>                               | The user who created the run                                                     | <pre><code>createdBy in ["user1", "user2"]
</code></pre><pre><code>createdBy = "user1" or createdBy = "user2"
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| <pre><code>ended
</code></pre>                                   | Time of finish                                                                   | <pre><code>ended >= now("-14d")
</code></pre><pre><code>ended >= startOfDay("-1m")
</code></pre><pre><code>ended &#x3C; 1569430502709
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| <pre><code>deleted
</code></pre>                                 | Time of removal                                                                  | <pre><code>deleted >= now("-14d")
</code></pre><pre><code>deleted >= startOfDay("-1m")
</code></pre><pre><code>deleted &#x3C; 1569430502709
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| <pre><code>isDeleted
</code></pre>                               | Whether the result is deleted                                                    | <pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| <pre><code>isEnded
</code></pre>                                 | Whether the result is ended                                                      | <pre><code>isEnded is false
</code></pre><pre><code>isEnded = true
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <pre><code>timeSpent
</code></pre>                               | Time spent (in milliseconds)                                                     | <pre><code>timeSpent > 10000
</code></pre>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

### Test plan: <a href="#h_e9113559bb" id="h_e9113559bb"></a>

| _Attribute_                          | _Description_               | _Examples_                                                                                                                                                                                                               |
| ------------------------------------ | --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <pre><code>id
</code></pre>          | Identifier                  | <pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>not id in [1, 2, 10]
</code></pre>                                 |
| <pre><code>title
</code></pre>       | Title                       | <pre><code>title is "first test"
</code></pre><pre><code>title = "first test"
</code></pre><pre><code>title ~ "rst"
</code></pre><pre><code>title in ["first test", "second test"]
</code></pre>                         |
| <pre><code>description
</code></pre> | Plan's description          | <pre><code>description is "first test"
</code></pre><pre><code>description = "first test"
</code></pre><pre><code>description ~ "rst"
</code></pre><pre><code>description in ["first test", "second test"]
</code></pre> |
| <pre><code>project
</code></pre>     | Project                     | <pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre>                                                                             |
| <pre><code>created
</code></pre>     | Time of creation            | <pre><code>created >= now("-14d")
</code></pre><pre><code>created >= startOfDay("-1m")
</code></pre><pre><code>created &#x3C; 1569430502709
</code></pre>                                                                |
| <pre><code>updated
</code></pre>     | Time of the last update     | <pre><code>updated >= now("-14d")
</code></pre><pre><code>updated >= startOfDay("-1m")
</code></pre><pre><code>updated &#x3C; 1569430502709
</code></pre>                                                                |
| <pre><code>deleted
</code></pre>     | Time of deletion            | <pre><code>deleted >= now("-14d")
</code></pre><pre><code>deleted >= startOfDay("-1m")
</code></pre><pre><code>deleted &#x3C; 1569430502709
</code></pre>                                                                |
| <pre><code>isDeleted
</code></pre>   | Whether the plan is deleted | <pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre>                                                                                                                                     |

### Requirement: <a href="#h_c47f8c5b2f" id="h_c47f8c5b2f"></a>

| _Attribute_                          | _Description_                                                                      | _Examples_                                                                                                                                                                                                               |
| ------------------------------------ | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <pre><code>id
</code></pre>          | Identifier                                                                         | <pre><code>id = 17
</code></pre><pre><code>id != 20
</code></pre><pre><code>id is 17
</code></pre><pre><code>id in [1, 2, 10]
</code></pre><pre><code>not id in [1, 2, 10]
</code></pre>                                 |
| <pre><code>parent
</code></pre>      | Parent requirement's title                                                         | <pre><code>parent is "first test"
</code></pre><pre><code>parent = "first test"
</code></pre><pre><code>parent ~ "rst"
</code></pre><pre><code>parent in ["first test", "second test"]
</code></pre>                     |
| <pre><code>project
</code></pre>     | Project                                                                            | <pre><code>project = 'DEMO'
</code></pre><pre><code>project in ['DEMO', 'QTC']
</code></pre><pre><code>project not in ['DEMO']
</code></pre>                                                                             |
| <pre><code>author
</code></pre>      | The user who created the requirement                                               | <pre><code>author in ["user1", "user2"]
</code></pre><pre><code>author = "user1" or createdBy = "user2"
</code></pre>                                                                                                    |
| <pre><code>createdBy
</code></pre>   | The user who created the requirement                                               | <pre><code>createdBy in ["user1", "user2"]
</code></pre><pre><code>createdBy = "user1" or createdBy = "user2"
</code></pre>                                                                                              |
| <pre><code>title
</code></pre>       | Title                                                                              | <pre><code>title is "first test"
</code></pre><pre><code>title = "first test"
</code></pre><pre><code>title ~ "rst"
</code></pre><pre><code>title in ["first test", "second test"]
</code></pre>                         |
| <pre><code>description
</code></pre> | Description                                                                        | <pre><code>description is "first test"
</code></pre><pre><code>description = "first test"
</code></pre><pre><code>description ~ "rst"
</code></pre><pre><code>description in ["first test", "second test"]
</code></pre> |
| <pre><code>status
</code></pre>      | Status (valid, draft, review, rework, finish, implemented, not-testable, obsolete) | <pre><code>status = 'valid'
</code></pre>                                                                                                                                                                                |
| <pre><code>type
</code></pre>        | Type (epic, user-story, feature)                                                   | <pre><code>type = 'epic'
</code></pre>                                                                                                                                                                                   |
| <pre><code>created
</code></pre>     | Time of creation                                                                   | <pre><code>created >= now("-14d")
</code></pre><pre><code>created >= startOfDay("-1m")
</code></pre><pre><code>created &#x3C; 1569430502709
</code></pre>                                                                |
| <pre><code>updated
</code></pre>     | Time of last update                                                                | <pre><code>updated >= now("-14d")
</code></pre><pre><code>updated >= startOfDay("-1m")
</code></pre><pre><code>updated &#x3C; 1569430502709
</code></pre>                                                                |
| <pre><code>deleted
</code></pre>     | Time of deletion                                                                   | <pre><code>deleted >= now("-14d")
</code></pre><pre><code>deleted >= startOfDay("-1m")
</code></pre><pre><code>deleted &#x3C; 1569430502709
</code></pre>                                                                |
| <pre><code>isDeleted
</code></pre>   | Whether the requirement is deleted                                                 | <pre><code>isDeleted is false
</code></pre><pre><code>isDeleted = true
</code></pre>                                                                                                                                     |

\
