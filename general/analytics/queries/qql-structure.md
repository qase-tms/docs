# QQL structure

### What does QQL consist of?

QQL consists of two parts: "Entity" + "Query". They both are required to perform a search query to the backend. Some examples of queries:

```
entity = "defect" and status = "open"

entity = "case" and project = "DEMO" and title ~ "auth" order by id desc

entity = "result" and status = "failed" and timeSpent > 5000 and 
milestone ~ "Sprint 12"

entity = "case" and isFlaky = false and automation = "To be automated"
```

Entity by default is 'case'. Projects by default include all projects available to user

### Entities <a href="#h_a2d0a1493b" id="h_a2d0a1493b"></a>

* Test case
* Test run
* Test run result
* Test plan
* Defect
* Requirement

### Query <a href="#h_8651b79247" id="h_8651b79247"></a>

Currently, QQL supports seven expression types. They are listed here in the decreasing priority order:

Expressions:

| _Expression Type_            | _Example_                                                            |
| ---------------------------- | -------------------------------------------------------------------- |
| Parenthesis                  | <pre><code>( expression )
</code></pre>                              |
| Negation                     | <pre><code>not expression
</code></pre>                              |
| Logical Expression           | <pre><code>true
</code></pre><p>or</p><pre><code>false
</code></pre> |
| Logical AND                  | <pre><code>expression and expression
</code></pre>                   |
| Logical OR                   | <pre><code>expression or expression
</code></pre>                    |
| Checking the attribute value | <pre><code>attribute operand value
</code></pre>                     |
| Sorting by field             | <pre><code>ORDER BY field ASC/DESC
</code></pre>                     |

#### Supported operands:

| Operand      | Meaning                  | Works with    |
| ------------ | ------------------------ | ------------- |
| <            | less than                | integer       |
| <=           | less than or equal to    | integer       |
| >            | greater than             | integer       |
| >=           | greater than or equal to | integer       |
| =, is        | equal to                 | integer, bool |
| !=           | not equal to             | integer, bool |
| \~           | includes                 | string, text  |
| in           | includes (array)         | array         |
| not in       | does not include (array) | array         |
| is empty     | no value                 |               |
| is not empty | value exists             |               |

#### Data types:

| Data type | Possible values                                | Supported operands  |
| --------- | ---------------------------------------------- | ------------------- |
| Integer   | 110                                            | >, >=, <, <=, =, != |
| String    | Some text                                      | \~                  |
| Boolean   | True or False                                  | is                  |
| Array     | \['Text1', 'Text2']; ('text 1', 'text 2'); \[] | in                  |
| Null      | null                                           |                     |

#### Functions:

| Name          | Return type | Arguments                                                                                                                                                                                                                                                                                                                                                                               | Description                   |
| ------------- | ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------- |
| currentUser() | integer     | -                                                                                                                                                                                                                                                                                                                                                                                       | Returns an ID of current user |
| now()         | integer     | <p>"+Nd" - modifies returned value, adding N days.</p><p>"-Nd" - modifies returned value, substracting N days.</p><p>"+Nw" - modifies returned value, adding N weeks.</p><p>"-Nw" - modifies returned value, substracting N weeks.</p><p>"+Nm" - modifies returned value, adding N months.</p><p>"-Nm" - modifies returned value, substracting N months.</p><p>N must be an integer</p> | Returns current timestamp     |

\
