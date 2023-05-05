---
sidebar_position: 2
---

# List System Deposit

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can get System Deposit list.

## 3. API

### List System Deposit Request example:


```json
{
  "SortBy": "123e4567-e89b-12d3-a456-426614174000",
  "SortByColumn": "Asc",
  "Limit": "Limit",
  "Offset": "Offset",
  "SearchTerm": "SearchTerm",
  "StartDate": "2020-03-24T06:03:00.348+03:00",
  "EndDate": "2021-03-24T06:03:00.348+03:00"
}
```

### List System Deposit Response example:

```json
{
  "Data": {
    "Deposits": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "DepositDate": "2022-06-16 02:26:26",
        "Email": "admin@codemen.org",
        "BankName": "Weimann, Emmerich and Koch",
        "Symbol": "USD",
        "Amount": "677.26155146"
      }
    ]
  },
  "TotalWallets": 2
}
```
