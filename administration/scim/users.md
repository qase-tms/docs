# Users

With SCIM API you can manage users in your Enterprise account. You can get the full list of users, filter by attribute, add new users, update user's attributes, activate or deactivate users and delete users completely.

* [User attributes](users.md#user-attributes)
* [User methods](users.md#user-methods)
  * [Get users](users.md#get-users)
  * [Get user by ID](users.md#get-user-by-id)
  * [Create a new user](users.md#create-a-new-user)
  * [Replace user by ID](users.md#replace-user-by-id)
  * [Update user's attributes by ID](users.md#update-user-attribute-by-id)
  * [Delete user](users.md#delete-user-by-id)

### User attributes

We support the following user attributes.

<table><thead><tr><th width="155.33333333333331">IDP attribute name</th><th width="186">Qase attribute</th><th>Description</th></tr></thead><tbody><tr><td>Email</td><td><code>userName</code></td><td>User email. Mandatory field.</td></tr><tr><td>Name</td><td><code>name.givenName</code></td><td>Attribute is used if the value is not empty.<br><br><strong>Maximum:</strong> 60 characters.</td></tr><tr><td></td><td><code>name.familyName</code></td><td>Attribute is used if the <code>displayName</code> attribute is not provided, <code>name</code> attribute is provided and 'formatted' attribute value is not empty.<br><br><strong>Maximum:</strong> 60 characters.</td></tr><tr><td>User type</td><td><code>userType</code></td><td><p>Supported values: <code>regular</code>, <code>read-only</code> and <code>billing</code>.</p><p></p><p>When <code>userType=regular</code>, a user is upgraded to FULL license inside the Qase application.<br><br>When userType is not specified, user license is updated/set according to internal Qase logic, which depends on the organization plan.</p></td></tr><tr><td>Active</td><td><code>active</code></td><td>Supported value: <code>true</code> or <code>false</code></td></tr></tbody></table>

> 📘
>
> Qase attribute namespace
>
> 'urn:ietf:params:scim:schemas:core:2.0:User' is a default SCIM urn for basic fields. If your identity provider does not require defining namespace, the default namespace must be avoided.



### User methods

#### Get users

`GET: https://app.qase.io/scim/v2/Users`

Retrieves the list of users in your organization. Use `startIndex` and `count` query parameters to receive paginated results. Supports sorting and **the** filter parameter.

Response

```json
{
    "schemas": [
        "urn:ietf:params:scim:api:messages:2.0:ListResponse"
    ],
    "totalResults": 1,
    "itemsPerPage": 1,
    "startIndex": 1,
    "Resources": [
        {
            "schemas": [
                "urn:ietf:params:scim:schemas:core:2.0:User"
            ],
            "id": "1",
            "userName": "john@doe.com",
            "name": {
                "familyName": "John",
                "givenName": "Doe"
            },
            "active": true,
            "userType": "regular",
            "title": "CEO",
            "emails": [
                {
                    "value": "john@doe.com",
                    "primary": true
                }
            ],
            "meta": {
                "resourceType": "User",
                "location": "https://app.qase.io/scim/v2/Users/1"
            }
        }
    ]
}
```

**Sorting**

Sorting allows you to specify the order in which resources are returned by specifying a combination of `sortBy` and `sortOrder` URL parameters.\
The `sortBy` parameter specifies the attribute whose value will be used to order the returned responses. The `sortOrder` parameter defines the order in which the `sortBy` parameter is applied. Allowed values are `ascending` and `descending`.

**Filters**\
You can request a subset of resources by specifying the `filter` query parameter containing a filter expression. Attribute names and attribute operators used in filters are case insensitive. The `filter` parameter must contain at least one valid expression. Each expression must contain an attribute name followed by an attribute operator and an optional value.

<table data-header-hidden><thead><tr><th width="136"></th><th></th></tr></thead><tbody><tr><td><pre><code>eq
</code></pre></td><td>equal</td></tr><tr><td><pre><code>ne
</code></pre></td><td>not equal</td></tr><tr><td><pre><code>co
</code></pre></td><td>contains</td></tr><tr><td><pre><code>sw
</code></pre></td><td>starts with</td></tr><tr><td><pre><code>ew
</code></pre></td><td>ends with</td></tr><tr><td><pre><code>pr
</code></pre></td><td>preset (has value)</td></tr><tr><td><pre><code>gt
</code></pre></td><td>greater than</td></tr><tr><td><pre><code>ge
</code></pre></td><td>greater than or equal to</td></tr><tr><td><pre><code>lt
</code></pre></td><td>less than</td></tr><tr><td><pre><code>le
</code></pre></td><td>less than or equal to</td></tr><tr><td><pre><code>and
</code></pre></td><td>logical "and"</td></tr><tr><td><pre><code>or
</code></pre></td><td>logical "or"</td></tr><tr><td><pre><code>not
</code></pre></td><td>"not" function</td></tr><tr><td><pre><code>( )
</code></pre></td><td>precedence grouping</td></tr></tbody></table>



Example of complex request:\


```
GET: https://app.qase.io/scim/v2/Users?attributes=name,userName&filter=NOT(name.familyName eq "Green")&sortBy=name.givenName&sortOrder=ascending&startIndex=2&count=5
```



#### Get user by ID

`GET: https://app.qase.io/scim/v2/Users/1`

Retrieves a single user resource

Response

<pre class="language-json"><code class="lang-json"><strong>{
</strong>    "schemas": [
        "urn:ietf:params:scim:schemas:core:2.0:User"
    ],
    "id": "1",
    "userName": "john@doe.com",
    "name": {
        "familyName": "John",
        "givenName": "Doe"
    },
    "active": true,
    "userType": "regular",
    "title": "CEO",
    "emails": [
        {
            "value": "john@doe.com",
            "primary": true
        }
    ],
    "meta": {
        "resourceType": "User",
        "location": "https://app.qase.io/scim/v2/Users/1"
    }
}
</code></pre>



#### Create a new user

`POST: https://app.qase.io/scim/v2/Users`

Creates a new user. Payload must include `userName` attribute populated with an email address, `familyName`, and `givenName` attribute.

> 📘
>
> All newly provisioned users are added with a default role.

**Request**

```json
{
    "schemas":["urn:ietf:params:scim:schemas:core:2.0:User"],
    "userName":"john@doe.com",
    "name":{
        "familyName":"John",
        "givenName":"Doe"
    }
}
```

**Response**

```json
{
    "schemas": [
        "urn:ietf:params:scim:schemas:core:2.0:User"
    ],
    "id": "1",
    "meta": {
        "resourceType": "User",
        "location": "https://app.qase.io/scim/v2/Users/1"
    },
    "userName": "john@doe.com",
    "name": {
        "familyName": "John",
        "givenName": "Doe"
    },
    "active": true,
    "emails": [
        {
            "value": "john@doe.com",
            "primary": true
        }
    ]
}
```



#### Replace user by ID

`PUT: https://app.qase.io/scim/v2/Users/1`

Updates an existing user resource. This is the easiest way to replace the user information.

**Request**

```json
{
    "schemas": [
        "urn:ietf:params:scim:schemas:core:2.0:User"
    ],
    "id": "1",
    "meta": {
        "resourceType": "User",
        "location": "https://app.qase.io/scim/v2/Users/1"
    },
    "userName": "replace@example.com",
    "name": {
        "familyName": "Replace",
        "givenName": "Me"
    },
    "active": true,
    "userType": "regular",
    "emails": [
        {
            "value": "replace@example.com",
            "primary": true
        }
    ]
}
```

**Response**

```json
{
    "schemas": [
        "urn:ietf:params:scim:schemas:core:2.0:User"
    ],
    "id": "1",
    "meta": {
        "resourceType": "User",
        "location": "https://app.qase.io/scim/v2/Users/1"
    },
    "userName": "replace@example.com",
    "name": {
        "familyName": "Replace",
        "givenName": "Me"
    },
    "active": true,
    "userType": "regular",
    "emails": [
        {
            "value": "replace@example.com",
            "primary": true
        }
    ]
}
```



#### Update user attribute by ID

`PATCH: https://app.qase.io/scim/v2/Users/1`

Updates an existing user resource, overwriting values for specified attributes. Attributes that are not provided will remain unchanged. PATCH only updates the fields provided.

The body of a PATCH request must contain the attribute `Operations`, whose value is an array of one or more PATCH operations. Each PATCH operation object must have exactly one `op` member.

**Request to deactivate user**

```json
{
  "schemas": [
    "urn:ietf:params:scim:api:messages:2.0:PatchOp"
  ],
  "Operations": [
    {
      "op": "Replace",
      "path": "active",
      "value": false
    }
  ]
}
```

**Response**

```json
{
    "schemas": [
        "urn:ietf:params:scim:schemas:core:2.0:User"
    ],
    "id": "1",
    "meta": {
        "resourceType": "User",
        "location": "https://app.qase.io/scim/v2/Users/1"
    },
    "userName": "john@doe.com",
    "name": {
        "familyName": "John",
        "givenName": "Doe"
    },
    "active": true,
    "userType": "regular",
    "emails": [
        {
            "value": "john@doe.com",
            "primary": true
        }
    ]
}
```

**Request to rename user**

```json
{
  "schemas": [
    "urn:ietf:params:scim:api:messages:2.0:PatchOp"
  ],
  "Operations": [
    {
      "op": "Replace",
      "path": "name.givenName",
      "value": "New Given Name"
    }
  ]
}
```

**Request to upgrade user license to regular**

```json
{
  "schemas": [
    "urn:ietf:params:scim:api:messages:2.0:PatchOp"
  ],
  "Operations": [
    {
      "op": "Replace",
      "path": "userType",
      "value": "regular"
    }
  ]
}
```

**Request to update user email (userName)**

```json
{
    "schemas": [
        "urn:ietf:params:scim:api:messages:2.0:PatchOp"
    ],
    "Operations": [
        {
            "op": "Replace",
            "path": "userName",
            "value": "new@email.com"
        }
    ]
}
```



#### Delete user by ID

`DELETE: https://app.qase./scim/Users/1`

Deletes a single user from the organization.

> 🚧
>
> User removing restrictions:
>
> A user who is the workspace owner cannot be deleted. If you try to delete such user, the API returns a 409 error code.
