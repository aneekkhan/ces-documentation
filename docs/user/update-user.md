---
sidebar_position: 3
---

# Update User

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

In cryptocurrency exchange system admin can Update user list.

## 3. API

### Request example:

```json
{
  "FirstName": "John",
  "LastName": "Smith",
  "RoleName": "John",
  "is_email_verified": "IS_EMAIL_TRUE",
  "account_status": "ACCOUNT_STATUS_UNKNOWN",
  "financial_status": "FINANCIAL_STATUS_UNKNOWN",
  "maintenance_access_status": "MAINTENANCE_ACCESS_STATUS_UNKNOWN"
}
```

### Response example:

```json
{
  "Data": {
    "User": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "FirstName": "John",
      "LastName": "Smith",
      "Email": "mail@mail.com",
      "Phone": "1234567890",
      "Password": "password",
      "RoleName": "John",
      "is_email_verified": "IS_EMAIL_TRUE",
      "account_status": "ACCOUNT_STATUS_UNKNOWN",
      "financial_status": "FINANCIAL_STATUS_UNKNOWN",
      "maintenance_access_status": "MAINTENANCE_ACCESS_STATUS_UNKNOWN",
      "CreatedAt": "2020-03-24T06:03:00.348+03:00",
      "CreatedBy": "456e4567-e89b-12d3-a456-426614174000",
      "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
      "UpdatedBy": "456e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```
