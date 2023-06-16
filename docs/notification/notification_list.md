---
sidebar_position: 24
---

# List Notifications

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can get the notification list.

## 3. API

### List Notifications Request example:

```json
{
  "SortBy": "",
  "SortByColumn": "",
  "Status": "TRUE",
  "SearchTerm": "SearchTerm",
  "StartDate": "2020-03-24T06:03:00.348+03:00",
  "EndDate": "2021-03-24T06:03:00.348+03:00"
}
```

### List Notifications Response example:

```json
{
   "Data": {
    "Notification":[
      {
        "ID": "123e4567-e89b-12d3-a456-426614174111",
        "UserID": "123e4567-e89b-12d3-a456-426614174000",
        "Title": "Bank News",
        "Details": "This is a details",
        "ReadAt": "2023-05-08 09:12:15",
        "IsRead": "TRUE",
        "CreatedAt": "2023-05-08 09:12:15",
        "UpdatedAt": "2023-05-08 09:12:15",
        "CreatedBy": "123e4567-e89b-12d3-a456-426614174025",
        "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025",
        "Reference": "This is a details reference"
      },
      {
        "ID": "123e4567-e89b-12d3-a456-426614174111",
        "UserID": "123e4567-e89b-12d3-a456-426614174000",
        "Title": "Bank News",
        "Details": "This is a details",
        "ReadAt": "2023-05-08 09:12:15",
        "IsRead": "TRUE",
        "CreatedAt": "2023-05-08 09:12:15",
        "UpdatedAt": "2023-05-08 09:12:15",
        "CreatedBy": "123e4567-e89b-12d3-a456-426614174025",
        "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025",
        "Reference": "This is a details reference"
      }
    ]
   },
   "TotalPages": 2
}
```
