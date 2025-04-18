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

<table><thead><tr><th width="158">Status</th><th>Description</th></tr></thead><tbody><tr><td>400</td><td>Bad Request.<br><br>Unexpected request.<br>The <code>detail</code> attribute of the resource should provide information on what request/attribute value is unexpected.</td></tr><tr><td>401</td><td>Unauthorized.<br><br>Qase cannot authorize the organization with the authorization token.</td></tr><tr><td>403</td><td>Forbidden.<br><br>SCIM integration is disabled.</td></tr><tr><td>404</td><td>Not Found.<br><br>The requested resource wasn't found by looking up its ID.</td></tr><tr><td>405</td><td>Method not allowed.<br><br>Qase doesn't support the requested method.</td></tr><tr><td>409</td><td>Conflict.<br><br>Qase cannot update a resource because of a business logic conflict.<br>The logic conflict can vary, depending on the real-life scenario.</td></tr><tr><td>413</td><td>Payload too large.<br><br>The payload exceeds the maximum payload of 800000 bytes.</td></tr><tr><td>415</td><td>Unsupported Media Type.<br><br>The endpoint doesn't support the provided media type.</td></tr><tr><td>429</td><td>Too many requests.</td></tr><tr><td>500</td><td>Internal Server Error.<br><br>An unexpected error of application.<br>Please, contact Qase support to clarify the reason for such an error.</td></tr></tbody></table>
