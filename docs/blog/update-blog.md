---
sidebar_position: 15
---

# Update Blog

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can get details in two way.
##### i.  User can get by user ID
##### ii. User can get by user Email


## 3. API

### Get Blog by ID Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000"
}
```

### Get Blog by ID Response example:

```json
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
`
