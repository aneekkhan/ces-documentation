---
sidebar_position: 3
---

# Get User

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can get details in two way.

##### i. User can get by user ID

##### ii. User can get by user Email

## 3. API

### Get User by ID Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000"
}
```

### Get User by ID Response example:

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
      "Status": "STATUS_UNKNOWN",
      "AccountStatus": "ACCOUNT_STATUS_UNKNOWN",
      "FinancialStatus": "FINANCIAL_STATUS_UNKNOWN",
      "MaintenanceAccessStatus": "MAINTENANCE_ACCESS_STATUS_UNKNOWN",
      "IsMfa": "IS_MFA_TRUE",
      "IsPhoneVerified": "IS_PHONE_VERIFIED_TRUE",
      "IsEmailVerified": "IS_EMAIL_TRUE",
      "MfaType": "MFA_TYPE_RECOVERY",
      "CreatedAt": "2020-03-24T06:03:00.348+03:00",
      "CreatedBy": "mail@mail.com",
      "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
      "UpdatedBy": "mail@mail.com"
    }
  }
}
```

### Get User by Email Request example:

```json
{
  "Email": "mail@mail.com"
}
```
### Get User by Email Response example:

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
  }
}
`
```
