---
sidebar_position: 21
---

# Get Role

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user/admin can get role details by ID or role Name.


## 3. API

### Get Role Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
}
```

### Get Role Response example:

```json
{
  "Data": {
     "Role": {
         "ID": "123e4567-e89b-12d3-a456-426614174111", 
         "Name": "User",
         "Description": "Role Description",
         "AccessiableRoutes": "access",
         "IsActive": "TRUE",
         "CreatedAt": "2023-05-08 09:12:15",
         "UpdatedAt": "2023-05-08 09:12:15",
         "CreatedBy": "123e4567-e89b-12d3-a456-426614174025",
         "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025"
      }
   }
 }
```