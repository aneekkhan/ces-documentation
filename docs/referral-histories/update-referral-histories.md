---
sidebar_position: 3
---

# Update Referral Histories

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
  "CommissionAmount": 2000,
  "Status": "TYPE_UNKNOWN"
}
```
### Response example:

```json
{
  "Data": {
    "ReferralHistories": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "UserId": "12d3-e89b-12d3-a456-426614174000",
      "ReferralUserId": "a456-e89b-12d3-a456-426614174000",
      "CommissionAmount": 2000,
      "CommissionCurrencyId": "426614174000-e89b-12d3-a456-426614174000",
      "Status": "TYPE_UNKNOWN",
      "FeeCurrency": "USD",
      "IsMaker": "IS_MAKER_TRUE",
      "CreatedAt": "2020-03-24T06:03:00.348+03:00",
      "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
      "DeletedAt": "2020-03-24T06:03:00.348+03:00"
    }
  }
}
```