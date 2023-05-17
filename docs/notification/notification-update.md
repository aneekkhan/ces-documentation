---
sidebar_position: 24
---

# Update Notifications

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can update the notification status.

## 3. API

### Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000",
  "IsRead": "TRUE",
}
```

### Response example:

```json
{
  "Data": {
    "Notification": {
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
        "Slug": "BdNews"
      },
  }
}
```
