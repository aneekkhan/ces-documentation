---
sidebar_position: 16
---

# List Blog

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can get Blog list.


## 3. API

### List Blog Request example:

```json
{
  "SortBy": "123e4567-e89b-12d3-a456-426614174000",
  "SortByColumn": "John",
  "Status": "Smith",
  "Limit": "mail@mail.com",
  "Offset": "1234567890",
  "SearchTerm": "password",
  "StartDate": "Active",
  "EndDate": "Active"
}
```

### List Blog Response example:

```json
{
   "Data": {
    "Users":[
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "FirstName": "John",
        "LastName": "Smith",
        "Email": "mail@mail.com",
        "Phone": "1234567890",
        "Password": "password",
        "Status": "Active",
        "AccountStatus": "Active",
        "FinancialStatus": "Active",
        "MaintenanceAccessStatus": "Disable",
        "IsMfa": "True",
        "IsPhoneVerified": "Verified",
        "IsEmailVerified": "Verified",
        "MfaType": "MfaType",
        "CreatedAt": "2020-03-24T06:03:00.348+03:00",
        "CreatedBy": "2020-03-24T06:03:00.348+03:00",
        "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
        "UpdatedBy": "2020-03-24T06:03:00.348+03:00"
      }
    ]
   },
   "TotalPages": 2
}
```
