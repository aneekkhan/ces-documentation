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
  "SortBy": "DESC",
  "SortByColumn": "id",
  "Limit": "10",
  "Offset": "0",
  "SearchTerm": "",
  "Email":"",
  "DepositeMethod":"",
  "TransactionId":"",
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
        "DepositStatus": "DEPOSIT_STATUS_UNKNOWN",
        "DepositeMethod":"DEPOSIT_METHOD_CREDIT_CARD",
        "TransactionId":"34567654327657567",
      }
    ]
  },
  "TotalWallets": 1
}
```
