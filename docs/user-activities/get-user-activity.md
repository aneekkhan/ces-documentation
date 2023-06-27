---
sidebar_position: 3
---

# Get User Activities 

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can get user activity details by ID.


## 3. API

### Request example:

```json
{
   "ID": "123e4567-e89b-12d3-a456-426614174111",
}
```
### Response example:


```json
{
  "Data":{
    "UserActivity":{
        "ID": "123e4567-e89b-12d3-a456-426614174111",
        "UserID": "123e4567-e89b-12d3-a456-426614174000", 
        "Browser": "Firefox/v-114.0.2",
        "OperatingSystem": "Linux",
        "Country": "Bangladesh",
        "City": "Khulna",
        "Activity": "Login",
        "Device": "Laptop",
        "IPAddress": "192.168.44.20",
        "CreatedAt": "2023-05-08 09:12:15",
    }
  }
}
```