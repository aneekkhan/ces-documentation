---
sidebar_position: 3
---

# Change Password

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can change his password.


## 3. API

### change password Request example:

```json
{
   "Data":{
      "User":{
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "CurrentPassword":"Bitcoin",
         "NewPassword":"Bitcoin",
      }
   }
}
```

### change password Response example:

```json
{
   "Data":{
      "User":{
         "ID":"123e4567-e89b-12d3-a456-426614174000",
      }
   }
}
```