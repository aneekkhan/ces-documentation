---
sidebar_position: 22
---

# List Role

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can get Role list.


## 3. API

### List Role Request example:

```json
{
  "SortBy": "Asc",
  "SortByColumn": "Name",
  "IsActive": "TRUE",
  "SearchTerm": "SearchTerm"
}
```

### List Role Response example:

```json
{
   "Data": {
       "Role": [
            {
              "ID": "123e4567-e89b-12d3-a456-426614174111", 
              "Name": "User",
              "Description": "Role Description",
              "AccessiableRoutes":  ["access"],
              "IsActive": "TRUE",
              "Slug":"",
              "Permissions":"",  
              "CreatedAt": "2023-05-08 09:12:15",
              "UpdatedAt": "2023-05-08 09:12:15",
              "CreatedBy": "123e4567-e89b-12d3-a456-426614174025",
              "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025"
            }, 
            {
              "ID": "123e4567-e89b-12d3-a456-426614174111", 
              "Name": "User",
              "Description": "Role Description",
              "AccessiableRoutes":  ["access"],
              "IsActive": "TRUE",
              "Slug":"",
              "Permissions":"",  
              "CreatedAt": "2023-05-08 09:12:15",
              "UpdatedAt": "2023-05-08 09:12:15",
              "CreatedBy": "123e4567-e89b-12d3-a456-426614174025",
              "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025"
            }
           ]
         },
   "TotalPages": 2
}
```
