# Custom field

### Created Custom Field

Payload example:

```json
{
  "event_name": "custom_field.created",
  "timestamp": 1650533521,
  "payload": {
    "id": 208,
    "title": "test",
    "isRequired": false,
    "isFilterable": false,
    "isVisible": true,
    "default_value": "5",
    "value": "[]",
    "type": "number",
    "entity": "case"
  },
  "team_member_id": 40,
  "project_code": "ID"
}
```

> #### 📘
>
> This event is being sent when a new custom field is created.

#### Event name

`custom_field.created`

#### Payload fields

| Parameter      | Type    | Description                                                                                         |
| -------------- | ------- | --------------------------------------------------------------------------------------------------- |
| id             | integer | Custom field ID                                                                                     |
| title          | string  | Custom field title                                                                                  |
| isRequired     | boolean | A boolean value that indicates, that custom field should be filled on case create/update page.      |
| isFilterable   | boolean | A boolean value that indicates, that custom field will be shown in filters                          |
| isVisible      | boolean | A boolean value that indicates, that custom field will be visible in preview and on test case page. |
| default\_value | string  | Default value for custom field                                                                      |
| value          | string  |                                                                                                     |
| type           | string  | Custom field type. Available values: `number`, `string`, `text`, `selectbox`, `checkbox`.           |
| entity         | string  | Custom field entity. Available values: `case`, `defect`, `run`                                      |

### Deleted Custom Field

Payload example:

```json
{
  "event_name": "custom_field.deleted",
  "timestamp": 1650533655,
  "payload": {
    "id": 208,
    "title": "test",
    "isRequired": false,
    "isFilterable": false,
    "isVisible": true,
    "default_value": "5",
    "value": "[]",
    "type": "number",
    "entity": "case"
  },
  "team_member_id": 40,
  "project_code": "ID"
}
```

> #### 📘
>
> This event is being sent when a custom field is deleted.

#### Event name

`custom_field.deleted`

#### Payload fields

| Parameter      | Type    | Description                                                                                         |
| -------------- | ------- | --------------------------------------------------------------------------------------------------- |
| id             | integer | Custom field ID                                                                                     |
| title          | string  | Custom field title                                                                                  |
| isRequired     | boolean | A boolean value that indicates, that custom field should be filled on case create/update page.      |
| isFilterable   | boolean | A boolean value that indicates, that custom field will be shown in filters                          |
| isVisible      | boolean | A boolean value that indicates, that custom field will be visible in preview and on test case page. |
| default\_value | string  | Default value for custom field                                                                      |
| value          | string  |                                                                                                     |
| type           | string  | Custom field type. Available values: `number`, `string`, `text`, `selectbox`, `checkbox`.           |
| entity         | string  | Custom field entity. Available values: `case`, `defect`, `run`                                      |

### Updated Custom Field

Payload example:

```json
{
  "event_name": "custom_field.updated",
  "timestamp": 1650533629,
  "payload": {
    "id": 208,
    "title": "test",
    "isRequired": false,
    "isFilterable": false,
    "isVisible": true,
    "default_value": "5",
    "value": "[]",
    "type": "number",
    "entity": "case"
  },
  "team_member_id": 40,
  "project_code": "ID"
}
```

> #### 📘
>
> This event is being sent when a custom field is updated.

#### Event name

`custom_field.updated`

#### Payload fields

| Parameter      | Type    | Description                                                                                         |
| -------------- | ------- | --------------------------------------------------------------------------------------------------- |
| id             | integer | Custom field ID                                                                                     |
| title          | string  | Custom field title                                                                                  |
| isRequired     | boolean | A boolean value that indicates, that custom field should be filled on case create/update page.      |
| isFilterable   | boolean | A boolean value that indicates, that custom field will be shown in filters                          |
| isVisible      | boolean | A boolean value that indicates, that custom field will be visible in preview and on test case page. |
| default\_value | string  | Default value for custom field                                                                      |
| value          | string  |                                                                                                     |
| type           | string  | Custom field type. Available values: `number`, `string`, `text`, `selectbox`, `checkbox`.           |
| entity         | string  | Custom field entity. Available values: `case`, `defect`, `run`                                      |

\
