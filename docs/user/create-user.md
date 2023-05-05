---
sidebar_position: 2
---

# Create User

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can be created two way.

##### i. User can be registerd

##### ii. Admin can invite new user

## 3. API

### Create User Request example:

```json
{
  "FirstName": "John",
  "LastName": "Smith",
  "Email": "mail@mail.com",
  "Phone": "1234567890",
  "Password": "password"
}
```

### Create User Response example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000",
  "FirstName": "John",
  "LastName": "Smith",
  "Email": "mail@mail.com",
  "Phone": "1234567890",
  "Password": "password",
  "CreatedAt": "2020-03-24T06:03:00.348+03:00",
  "CreatedBy": "2020-03-24T06:03:00.348+03:00",
  "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
  "UpdatedBy": "2020-03-24T06:03:00.348+03:00"
}
`
```
