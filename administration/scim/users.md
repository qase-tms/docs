# Users

With SCIM API you can manage users in your Enterprise account. You can get the full list of users, filter by attribute, add new users, update user's attributes, activate or deactivate users and delete users completely.

* [User attributes](users.md#user-attributes)
* [User methods](users.md#user-methods)
  * [Get users](users.md#get-users)
  * [Create a new user](users.md#create-a-new-user)
  * [Update user's attributes](users.md#update-user-attribute-by-id)
  * [Delete user](users.md#delete-user-by-id)

### User attributes

We support the following user attributes.

| IDP attribute name | Qase attribute  | Description                                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Email              | userName        | User email. Mandatory field.                                                                                                                                                                                                                                                                                                                                 |
| Name               | name.givenName  | <p>Attribute is used if the value is not empty.<br><br><strong>Maximum:</strong> 60 characters.</p>                                                                                                                                                                                                                                                          |
|                    | name.familyName | <p>Attribute is used if the <code>displayName</code> attribute is not provided, <code>name</code> attribute is provided and 'formatted' attribute value is not empty.<br><br><strong>Maximum:</strong> 60 characters.</p>                                                                                                                                    |
| User type          | userType        | <p>Supported values: <code>regular</code>, <code>readonly</code> and <code>billing</code>.</p><p></p><p>When <code>userType=regular</code>, a user is upgraded to FULL license inside the Qase application.<br><br>When userType is not specified, user license is updated/set according to internal Qase logic, which depends on the organization plan.</p> |
| Active             | active          | Supported value: `true` or `false`                                                                                                                                                                                                                                                                                                                           |

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

`eq` equal

`ne` not equal

`co` contains

`sw` starts with

`ew` ends with

`pr` preset (has value)

`gt` greater than

`ge` greater than or equal to

`lt` less than

`le` less than or equal to

`and` Logical "and"

`or` Logical "or"

`not` "Not" function

`()` Precedence grouping

Example of complex request:\
`GET: https://app.qase.io/scim/v2/Users?attributes=name,userName&filter=NOT(name.familyName eq "Green")&sortBy=name.givenName&sortOrder=ascending&startIndex=2&count=5`

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
> User removing restrictions
>
> A user who is the workspace owner cannot be deleted. If you try to delete such user, the API returns a 409 error code.
