---
sidebar_position: 3
---

# Update Support Ticket

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
  "ID": "123e4567-e89b-12d3-a456-426614174000",
  "SupportType": "technical",
  "Subject": "error in login",
  "Message": "i cant login to my account",
  "Attachment": "path to file",
  "Status": "open",
  "Priority": "high",
  "AssignedTo": "123e4567-e89b-12d3-a456-426614174000",
}
```
### Response example:

```json
{
  "Data":{
    "SupportTicket":{
      "ID":"123e4567-e89b-12d3-a456-426614174000",
      "UserId": "123e4567-e89b-12d3-a456-426614174000",
      "SupportType": "technical",
      "Subject": "error in login",
      "Message": "i cant login to my account",
      "Attachment": "path to file",
      "Status": "open",
      "Priority": "high",
      "CreatedAt": "2021-10-10 12:00:00",
      "UpdatedAt": "2021-10-10 12:00:00",
      "ResolvedAt": "2021-10-10 12:00:00",
      "AssignedTo": "123e4567-e89b-12d3-a456-426614174000",
      "UpdatedBy": "123e4567-e89b-12d3-a456-426614174000",
      "CreatedBy": "123e4567-e89b-12d3-a456-426614174000"
    }
  }
}
```