---
sidebar_position: 4
---

# List Trade Pair

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
   "SortBy":"DESC",
   "OrderByData":"name",
   "SearchTerm":"B",
   "Limit":"10",
   "Offset":"0",
   "Status":"",
   "StartDate":"2020-03-24T06:03:00.348+03:00",
   "EndDate":""
}
```
### Response example:

```json
{
   "Data": {
    "TradePair":[
      {
        "ID":"123e4567-e89b-12d3-a456-426614174000",
        "BaseCurrencyId": "1234",
        "QuoteCurrencyId": "456",
        "LastPrice": "124.98",
        "IsActive": "ACTIVE",
        "IsDefault": "ACTIVE",
        "PriceDecimalPlaces": "3",
        "MinimumOrderAmount": "22.56",
        "MaximumOrderAmount": "65.89",
        "MakerFee": "99.00",
        "TakerFee": "90.89",
        "CreatedAt": "2020-03-24T06:03:00.348+03:00",
        "CreatedBy": "123e4567-e89b-12d3-a456-426614174000",
        "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
        "UpdatedBy": "123e4567-e89b-12d3-a456-426614174000"
      },
      {
        "ID":"123e4567-e89b-12d3-a456-426614174000",
        "BaseCurrencyId": "1234",
        "QuoteCurrencyId": "456",
        "LastPrice": "124.98",
        "IsActive": "ACTIVE",
        "IsDefault": "ACTIVE",
        "PriceDecimalPlaces": "3",
        "MinimumOrderAmount": "22.56",
        "MaximumOrderAmount": "65.89",
        "MakerFee": "99.00",
        "TakerFee": "90.89",
        "CreatedAt": "2020-03-24T06:03:00.348+03:00",
        "CreatedBy": "123e4567-e89b-12d3-a456-426614174000",
        "UpdatedAt": "2020-03-24T06:03:00.348+03:00",
        "UpdatedBy": "123e4567-e89b-12d3-a456-426614174000"
      }
    ]
   },
   "Total": 2
}
```