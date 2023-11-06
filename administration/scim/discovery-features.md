# Discovery features

### ServiceProviderConfig

`GET: https://app.qase.io/scim/v2/ServiceProviderConfig`

Returns supported operations and SCIM API basic configuration.

### ResourceTypes

`GET: https://app.qase.io/scim/v2/ResourceTypes`

Returns information about which resources are supported. Currently, we support Users only.

`GET: https://app.qase.io/scim/v2/ResourceTypes/User`

Will return metadata for User resource type.

### Schemas

`GET: https://app.qase.io/scim/v2/Schemas`

Will return metadata about Users attributes that are currently supported.

`GET: https://app.qase.io/scim/v2/Schemas/urn:ietf:params:scim:schemas:core:2.0:User`

Will provide information on how users are formatted.
