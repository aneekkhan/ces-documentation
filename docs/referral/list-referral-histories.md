---
sidebar_position: 4
---

# List Referral Histories

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

A crypto exchange system is a platform that allows users to buy, sell, and trade cryptocurrencies such as Bitcoin, Ethereum, and others. Trading on a crypto exchange system involves buying or selling cryptocurrencies at a particular price based on the demand and supply of the currency.

## 3. API

### Request example:

```json
{
  "SortBy": "ASC",
  "SortByColumn": "BankName",
  "SortType": "similar",
  "SearchTerm": "Like",
  "StartDate": "2023-02-08 09:12:15",
  "EndDate": "2023-05-08 09:12:15"
}
```

### Response example:

```json
{
  "Data": {
    "Referral": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "ReferredId": "12d3-e89b-12d3-a456-426614174000",
        "ReferralID": "a456-e89b-12d3-a456-426614174000",
        "Amount": 2000,
        "CommissionCurrencyId": "426614174000-e89b-12d3-a456-426614174000",
        "ReferrerType": "REFERRER_TYPE_UNKNOWN",
        "CreatedAt": "2020-03-24T06:03:00.348+03:00"
      },
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "ReferredId": "12d3-e89b-12d3-a456-426614174000",
        "ReferralID": "a456-e89b-12d3-a456-426614174000",
        "Amount": 2000,
        "CommissionCurrencyId": "426614174000-e89b-12d3-a456-426614174000",
        "ReferrerType": "REFERRER_TYPE_UNKNOWN",
        "CreatedAt": "2020-03-24T06:03:00.348+03:00"
      }
    ],
    "Total": 2
  }
}
```
