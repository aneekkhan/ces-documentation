---
sidebar_position: 2
---

# List System Wallet

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can get System Wallet list.

## 3. API

### List System Wallet Request example:

```json
{
  "SortBy": "DESC",
  "SortByColumn": "id",
  "Limit": "10",
  "Offset": "0",
  "SearchTerm": "",
}
```

### List System Wallet Response example:

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
        "Symbol": "USD",
        "Balance": 2000,
        "IsDefault":,
        "IsActive":,
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
        "Symbol": "BTC",
        "Balance": 2000,
        "IsDefault":,
        "IsActive":,
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
