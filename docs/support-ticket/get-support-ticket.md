---
sidebar_position: 3
---

# Get Support Ticket

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### Customer supporting system by ticketing.


## 3. API

### Request example:

```json
{
  "UserId": "123e4567-e89b-12d3-a456-426614174000",
  "SupportType": "technical",
  "Subject": "error in login",
  "Message": "i cant login to my account",
  "Attachment": "path to file",
  "Status": "open",
  "Priority": "high",
  "CreatedAt": "2021-10-10 12:00:00",
  "UpdatedAt": "2021-10-10 12:00:00",
  "AssignedTo": "123e4567-e89b-12d3-a456-426614174000",
  "UpdatedBy": "jhon doe",
  "CreatedBy": "jhon smith",
}
```
### Response example:

```json
{
  "Data":{
    "SupportTicket":{
      "UserId": "123e4567-e89b-12d3-a456-426614174000",
      "SupportType": "technical",
      "Subject": "error in login",
      "Message": "i cant login to my account",
      "Attachment": "path to file",
      "Status": "open",
      "Priority": "high",
      "CreatedAt": "2021-10-10 12:00:00",
      "UpdatedAt": "2021-10-10 12:00:00",
      "AssignedTo": "123e4567-e89b-12d3-a456-426614174000",
      "UpdatedBy": "jhon doe",
      "CreatedBy": "jhon smith",
    }
  }
}
```