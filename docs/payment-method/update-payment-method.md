---
sidebar_position: 3
---

# Update Payment Method

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
  "Id": "123e4567-e89b-12d3-a456-426614174000",
  "Name": "Payment",
  "Description": "Payment Method",
  "IsActive": "Pay With Cash",
  "CreatedAt": "2021-10-10 12:00:00",
  "UpdatedAt": "2021-10-10 12:00:00",
  "DeletedAt": "",
}
```
### Response example:

```json
{
  "Data":{
    "PaymentMethod": {
      "Id": "123e4567-e89b-12d3-a456-426614174000",
      "Name": "Payment",
      "Description": "Payment Method",
      "IsActive": "Pay With Cash",
      "CreatedAt": "2021-10-10 12:00:00",
      "UpdatedAt": "2021-10-10 12:00:00",
      "DeletedAt": "",
    }
 }
}
```