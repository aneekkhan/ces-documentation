---
sidebar_position: 2
---

# Invite User

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can be created two way.

##### i. Admin can invite new user

## 3. API

### Invite User Request example:

```json
{
  "FirstName": "John",
  "LastName": "Smith",
  "Email": "mail@mail.com",
  "Phone": "1234567890",
  "RoleID": "sdfhhjbad131151321"
}
```

### Create User Response example:

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
