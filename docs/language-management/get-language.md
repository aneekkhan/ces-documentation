---
sidebar_position: 2
---

# Get Language

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can get Language Management details by ID.

## 3. API

### Get Language by ID Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000"
}
```

### Get Language by ID Response example:

```json
{
  "Data": {
  "Language": {
    "ID": "123e4567-e89b-12d3-a456-426614174000",
    "Name": "Bangla",
    "ShortCode": "Ban",
    "Direction": "PAGE_DIRECTION_LEFT_TO_RIGHT",
    "Icon": "https://demo-exchange.squaredbyte.com/storage/images/coin-icons/default.png",
    "IsActive": "IS_ACTIVE_TRUE",
    "CreatedAt": "2023-05-08 09:12:15",
    "UpdatedAt": "2023-05-08 09:12:15",
    "CreatedBy": "123e4567-e89b-12d3-a456-426614174025",
    "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025"
    }
  }
}
```
