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
  "SortBy": "123e4567-e89b-12d3-a456-426614174000",
  "SortByColumn": "Asc",
  "Limit": "Limit",
  "Status": "Active",
  "Offset": "Offset",
  "SearchTerm": "SearchTerm",
  "StartDate": "2020-03-24T06:03:00.348+03:00",
  "EndDate": "2021-03-24T06:03:00.348+03:00"
}
```

### List Role Response example:

```json
{
   "Data": {
       "Role": [
            {
             "ID": "123e4567-e89b-12d3-a456-426614174000",
             "RoleName": "User",
             "Description": "Description is a",
             "Access": "access",
             "Status": "ACTIVE",
             "CreatedAt": "2023-05-08 09:12:15",
             "UpdatedAt": "2023-05-08 09:12:15",
             "CreatedBy": "123e4567-e89b-12d3-a456-426614174025",
             "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025"
            }, 
            {
             "ID": "123e4567-e89b-12d3-a456-426614174000",
             "RoleName": "User",
             "Description": "Description is a",
             "Access": "access",
             "Status": "ACTIVE",
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
