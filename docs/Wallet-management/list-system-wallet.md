---
sidebar_position: 2
---

# List Wallet

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin or user can get Wallet list.

## 3. API

### List Wallet Request example:

```json
{
  "SortBy": "DESC",
  "SortByColumn": "id",
  "SearchTerm": "",
  "StartDate": "2020-03-24T06:03:00.348+03:00",
  "EndDate": "",
  "IsSystem": "IS_SYSTEM_FALSE",
  "UserID": "321e4567-e89b-12d3-a456-867676887",
}
```

### List Wallet Response example:

```json
{
  "Data": {
    "Wallets": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "UserId":"321e4567-e89b-12d3-a456-867676887",
        "CurrencyId":"321e4567-e89b-12d3-a456-867676887",
        "Name": "United States Dollar",
        "Icon": "https://demo-exchange.squaredbyte.com/storage/images/coin-icons/default.png",
        "CurrencySymbol": "USD",
        "Balance": 2000,
        "IsDefault":,
        "IsActive":,
        "IsSystem": "IS_SYSTEM_FALSE",
        "LastDeposit":,
        "LastWithdrawal":,
        "CreatedAt": "123e4567-e89b-12d3-a456-426614174000",
        "CreatedBy": "2020-03-24T06:03:00.348+03:00",
        "UpdatedAt": "",
        "UpdatedBy": "",
        },
      {
        "ID": "565676745656-e89b-12d3-a456-426614174000",
        "UserId":"321e4567-e89b-12d3-a456-867676887",
        "CurrencyId":"321e4567-e89b-12d3-a456-867676887",
        "Name": "Bitcoin",
        "Icon": "https://demo-exchange.squaredbyte.com/storage/images/coin-icons/default.png",
        "CurrencySymbol": "BTC",
        "Balance": 2000,
        "IsDefault":,
        "IsActive":,
        "IsSystem": "IS_SYSTEM_FALSE",
        "LastDeposit":,
        "LastWithdrawal":,
        "CreatedAt": "123e4567-e89b-12d3-a456-426614174000",
        "CreatedBy": "2020-03-24T06:03:00.348+03:00",
        "UpdatedAt": "",
        "UpdatedBy": "",
      }
    ]
  },
  "TotalWallets": 2
}
```
