---
sidebar_position: 4
---

# List Deposit Histories

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

In cryptocurrency exchange system admin can get Deposit Histories list.

## 3. API

### List Deposit Histories Request example:


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

### List Deposit Histories Response example:

```json
{
  "Data": {
    "Deposits": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "DepositDate": "2022-06-16 02:26:26",
        "Email": "admin@codemen.org",
        "Symbol": "USD",
        "Amount": 677.26155146,
        "DepositStatus": "DEPOSIT_STATUS_UNKNOWN"
      }
    ]
  },
  "TotalWallets": 2
}
```
