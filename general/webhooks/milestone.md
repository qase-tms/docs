# Milestone

### Created Milestone

Payload example:

```json
{
  "event_name": "milestone.created",
  "timestamp": 1650533865,
  "payload": {
    "id": 70673,
    "title": "example",
    "description": "description"
  },
  "team_member_id": 40,
  "project_code": "ID"
}
```

> #### 📘
>
> This event is being sent when a new milestone is created.

#### Event name

`milestone.created`

#### Payload fields

| Parameter   | Type    | Description           |
| ----------- | ------- | --------------------- |
| id          | integer | Milestone ID          |
| title       | string  | Milestone title       |
| description | string  | Milestone description |

### Deleted Milestone

Payload example:

```json
{
  "event_name": "milestone.deleted",
  "timestamp": 1650533914,
  "payload": {
    "id": 1
  },
  "team_member_id": 40,
  "project_code": "ID"
}
```

> #### 📘
>
> This event is being sent when a milestone is deleted.

#### Event name

`milestone.deleted`

#### Payload fields

| Parameter | Type    | Description  |
| --------- | ------- | ------------ |
| id        | integer | Milestone ID |

### Updated Milestone

Payload example:

```json
{
  "event_name": "milestone.updated",
  "timestamp": 1650533896,
  "payload": {
    "id": 1
  },
  "team_member_id": 40,
  "project_code": "ID"
}
```

> #### 📘
>
> This event is being sent when a milestone is updated.

#### Event name

`milestone.updated`

#### Payload fields

| Parameter | Type    | Description  |
| --------- | ------- | ------------ |
| id        | integer | Milestone ID |

\
