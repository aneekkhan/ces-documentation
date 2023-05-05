---
sidebar_position: 2
---

# Create Currency

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can add new coin/currency.


## 3. API

### Create Coin/Currency Request example:

```json
{
   "Data":{
      "Currency":{
         "Name":"Bitcoin",
         "Symbol":"BTC",
         "CoinType":"CRYPTO",
         "Icon":"btc.png",
         "CreatedBy":"456e4567-e89b-12d3-a456-426614174000"
      }
   }
}
```

### Create Coin/Currency Response example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000"
}
`