---
sidebar_position: 2
---

# Create Support Ticket

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
  "SortBy":"DESC",
  "OrderByData":"name",
  "SearchTerm":"B",
  "Limit":"10",
  "Offset":"0",
  "Status":"",
  "StartDate":"2020-03-24T06:03:00.348+03:00",
  "EndDate":""
}
```
### Response example:

```json
{
   "Data": {
    "PaymentMethod":[
      {
        "Id": "123e4567-e89b-12d3-a456-426614174000",
        "Name": "Payment",
        "Description": "Payment Method",
        "IsActive": "Pay With Cash",
        "CreatedAt": "2021-10-10 12:00:00",
        "UpdatedAt": "2021-10-10 12:00:00",
        "DeletedAt": "2021-10-10 12:00:00",
      },
      {
        "Id": "123e4567-e89b-12d3-a456-426614174000",
        "Name": "Payment",
        "Description": "Payment Method",
        "IsActive": "Pay With Cash",
        "CreatedAt": "2021-10-10 12:00:00",
        "UpdatedAt": "2021-10-10 12:00:00",
        "DeletedAt": "2021-10-10 12:00:00",
      }
    ]
   },
   "Total": 2
}
```