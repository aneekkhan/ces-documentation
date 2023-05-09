---
sidebar_position: 2
---

# Create Payment Method

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### Payment method is a way to pay for the order.


## 3. API

### Request example:

```json
{
  "Name": "Payment",
  "Description": "Payment Method",
  "IsActive": "Pay With Cash",
}
```
### Response example:

```json
{
  "Data":{
    "Id": "123e4567-e89b-12d3-a456-426614174000",
  }
}
```