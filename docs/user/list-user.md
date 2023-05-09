---
sidebar_position: 4
---

# List User

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can get user list.

## 3. API

### List User Request example:

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

### List User Response example:

```json
{
  "Data": {
    "Users": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "FirstName": "John",
        "LastName": "Smith",
        "Email": "mail@mail.com",
        "Phone": "1234567890",
        "Password": "password",
        "Status": "STATUS_UNKNOWN",
        "AccountStatus": "ACCOUNT_STATUS_UNKNOWN",
        "FinancialStatus": "FINANCIAL_STATUS_UNKNOWN",
        "MaintenanceAccessStatus": "MAINTENANCE_ACCESS_STATUS_UNKNOWN",
        "IsMfa": "IS_MFA_TRUE",
        "IsPhoneVerified": "IS_PHONE_VERIFIED_TRUE",
        "IsEmailVerified": "IS_EMAIL_TRUE",
        "MfaType": "MFA_TYPE_RECOVERY",
        "CreatedAt": "2020-03-24T06:03:00.348+03:00",
        "CreatedBy": "456e4567-e89b-12d3-a456-426614174000",
        "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
        "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
      }
    ]
  },
  "TotalPages": 2
}
```
