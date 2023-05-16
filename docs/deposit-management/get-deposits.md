---
sidebar_position: 3
---

# Get System Bank Deposit

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

In cryptocurrency exchange system user's can view their deposit details

## 3. API

### Get System Bank Deposit Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000"
}
```

### Get System Bank Deposit Response example:

```json
{
  "Data": {
    "Deposits": {
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
  }
}
```
