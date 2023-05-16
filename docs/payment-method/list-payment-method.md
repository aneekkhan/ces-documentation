---
sidebar_position: 2
---

# List Payment Methods

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
  "SortBy": "DESC",
  "SortByColumn": "name",
  "SearchTerm": "B",
  "Status": "",
  "StartDate": "2020-03-24T06:03:00.348+03:00",
  "EndDate": ""
}
```

### Response example:

```json
{
  "Data": {
    "PaymentMethod": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "Name": "Payment",
        "Description": "Payment Method",
        "IsActive": "Active",
        "CreatedAt": "2021-10-10 12:00:00",
        "UpdatedAt": "2021-10-10 12:00:00",
        "DeletedAt": "2021-10-10 12:00:00"
      },
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "Name": "Payment",
        "Description": "Payment Method",
        "IsActive": "Active",
        "CreatedAt": "2021-10-10 12:00:00",
        "UpdatedAt": "2021-10-10 12:00:00",
        "DeletedAt": "2021-10-10 12:00:00"
      }
    ]
  },
  "Total": 2
}
```
