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
  "SortBy": "123e4567-e89b-12d3-a456-426614174000",
  "SortByColumn": "Asc",
  "Limit": "Limit",
  "Offset": "Offset",
  "SearchTerm": "SearchTerm",
  "StartDate": "2020-03-24T06:03:00.348+03:00",
  "EndDate": "2021-03-24T06:03:00.348+03:00"
}
```

### List System Wallet Response example:

```json
{
  "Data": {
    "Wallets": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "Icon": "https://demo-exchange.squaredbyte.com/storage/images/coin-icons/default.png",
        "Symbol": "USD",
        "Name": "United States Dollar",
        "Balance": "2000"
      },
      {
        "ID": "321e4567-e89b-12d3-a456-426614174000",
        "Icon": "https://demo-exchange.squaredbyte.com/storage/images/coin-icons/default.png",
        "Symbol": "BTC",
        "Name": "Bitcoin",
        "Balance": "0.00005000"
      }
    ]
  },
  "TotalWallets": 2
}
```
