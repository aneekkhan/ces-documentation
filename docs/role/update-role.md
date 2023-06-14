---
sidebar_position: 20
---

# Update Role

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can update role


## 3. API

### Update Role by ID Request example:

```json
{
   "ID": "123e4567-e89b-12d3-a456-426614174111",
   "Name": "User",
   "Description": "Role Description",
   "AccessiableRoutes": ["access"],
   "IsActive": "TRUE",
   "Slug":"",
   "Permissions":"",
   "UpdatedAt": "2023-05-08 09:12:15",
   "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025",
}
```

### Update Role by ID Response example:

```json
{ 
 "Data": {
    "Role": {            
      "ID": "123e4567-e89b-12d3-a456-426614174111", 
      "Name": "User",
      "Description": "Role Description",
      "AccessiableRoutes": ["access"],
      "IsActive": "TRUE",
      "Slug":"",
      "Permissions":"",
      "CreatedAt": "2023-05-08 09:12:15",
      "UpdatedAt": "2023-05-08 09:12:15",
      "CreatedBy": "123e4567-e89b-12d3-a456-426614174025",
      "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025",
      }
   }
}
```

