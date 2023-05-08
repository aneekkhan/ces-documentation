---
sidebar_position: 2
---

# Create Trade Pair

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### Cryptocurrencies can be traded against other cryptocurrencies or against fiat currencies, depending on the trading pairs offered by the platform.


## 3. API

### Request example:

```json
{
  "BaseCurrencyId": "1234",
  "QuoteCurrencyId": "456",
  "LastPrice": "124.98",
  "IsActive": true,
  "IsDefault": false,
  "PriceDecimalPlaces": "3",
  "MinimumOrderAmount": "22.56",
  "MaximumOrderAmount": "65.89",
  "MakerFee": "99.00",
  "TakerFee": "90.89",
}
```
### Response example:

```json
{
  "Data":{
    "Id": "123e4567-e89b-12d3-a456-426614174000",
  }
}
```