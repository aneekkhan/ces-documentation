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
      "Status": "STATUS_UNKNOWN",
      "IsPhoneVerified": "IS_PHONE_VERIFIED_FALSE",
      "IsEmailVerified": "IS_EMAIL_FALSE",
      "IsMfa": "IS_MFA_FALSE",
      "MfaType": "MFA_TYPE_RECOVERY",
      "KYCLevel":"KYC_LEVEL_UNKNOWN",
      "CreatedAt": "123e4567-e89b-12d3-a456-426614174000",
      "CreatedBy": "2020-03-24T06:03:00.348+03:00",
      "UpdatedAt": "",
      "UpdatedBy": "",
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
      "Status": "STATUS_UNKNOWN",
      "IsPhoneVerified": "IS_PHONE_VERIFIED_FALSE",
      "IsEmailVerified": "IS_EMAIL_FALSE",
      "IsMfa": "IS_MFA_FALSE",
      "MfaType": "MFA_TYPE_RECOVERY",
      "KYCLevel":"KYC_LEVEL_UNKNOWN",
      "CreatedAt": "123e4567-e89b-12d3-a456-426614174000",
      "CreatedBy": "2020-03-24T06:03:00.348+03:00",
      "UpdatedAt": "",
      "UpdatedBy": "",
    }
  }
}
`
```
