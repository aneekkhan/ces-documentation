---
sidebar_position: 2
---

# List System Bank Deposits

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

In cryptocurrency exchange system admin can get System Deposit list.

## 3. API

### List System Bank Deposits Request example:

```json
{
  "SortBy": "DESC",
  "SortByColumn": "id",
  "SearchTerm": "Like",
  "DepositStatus": "DEPOSIT_STATUS_UNKNOWN",
  "DepositeMethod": "DEPOSIT_STATUS_UNKNOWN",
  "StartDate": "2023-02-08 09:12:15",
  "EndDate": "2023-02-08 09:12:15"
}
```

### List System Bank Deposits Response example:

```json
{
  "Data": {
    "Deposits": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "FirstName": "John",
        "LastName": "Smith",
        "Symbol": "USD",
        "DepositStatus": "DEPOSIT_STATUS_UNKNOWN",
        "Amount": 677.26155146,
        "BankName": "Weimann, Emmerich and Koch",
        "Fee": 13.54523102,
        "TransactionTd": "bc5cf4da-da20-4144-948a-ad0e27367dd0",
        "DepositeMethod": "DEPOSIT_METHOD_CREDIT_CARD",
        "AccountName": "Prof. Kieran Howell Sr.",
        "AccountNumber": "538416559340",
        "SwiftCode": "BSWNARI6",
        "Iban": "RO88YTYQ53G6C7U8RZ6KKJ8B",
        "Country": "Palestinian Territory Occupied"
      }
    ]
  },
  "TotalWallets": 2
}
```
