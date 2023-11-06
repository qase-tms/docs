# Errors

Interacting with our APIs may result in an error instead of the expecting result. Qase tries to respond with a detailed error message that will help you figure out what went wrong and how to fix it.

[SCIM error schema](https://www.rfc-editor.org/rfc/rfc7644.html#section-3.12)\
Error response example:

```json
{
    "schemas": [
        "urn:ietf:params:scim:api:messages:2.0:Error"
    ],
    "status": "400",
    "scimType": "invalidValue",
    "detail": "User name 'email@example.com' is invalid: 'not unique'"
}
```

Possible errors:

| Status | Description                                                                                                                                                                   |
| ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 400    | <p>Bad Request.<br><br>Unexpected request.<br>The <code>detail</code> attribute of the resource should provide information on what request/attribute value is unexpected.</p> |
| 401    | <p>Unauthorized.<br><br>Qase cannot authorize the organization with the authorization token.</p>                                                                              |
| 403    | <p>Forbidden.<br><br>SCIM integration is disabled.</p>                                                                                                                        |
| 404    | <p>Not Found.<br><br>The requested resource wasn't found by looking up its ID.</p>                                                                                            |
| 405    | <p>Method not allowed.<br><br>Qase doesn't support the requested method.</p>                                                                                                  |
| 409    | <p>Conflict.<br><br>Qase cannot update a resource because of a business logic conflict.<br>The logic conflict can vary, depending on the real-life scenario.</p>              |
| 413    | <p>Payload too large.<br><br>The payload exceeds the maximum payload of 800000 bytes.</p>                                                                                     |
| 415    | <p>Unsupported Media Type.<br><br>The endpoint doesn't support the provided media type.</p>                                                                                   |
| 429    | Too many requests.                                                                                                                                                            |
| 500    | <p>Internal Server Error.<br><br>An unexpected error of application.<br>Please, contact Qase support to clarify the reason for such an error.</p>                             |
