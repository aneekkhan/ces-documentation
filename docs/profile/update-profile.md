---
sidebar_position: 5
---

# Update Profile

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

In cryptocurrency exchange system user can Update his profile info.

## 3. API

### Request example:

```json
{
  "Data": {
    "User": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "FirstName": "John",
      "LastName": "Smith",
      "Email": "john@gmail.com",
      "ProfileImage": "pic.png",
    }
  }
}
```

### Response example:

```json
{
  "Data": {
    "User": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
    }
  }
}
```
