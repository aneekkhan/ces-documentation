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
   "SortByColumn":"name",
   "SearchTerm":"B",
   "IsActive":"TRUE"
}
```
### Response example:

```json
{
   "Data":{
      "TradePairs":[
         {
            "ID":"123e4567-e89b-12d3-a456-426614174000",
            "Name":"BTC_USD",
            "BaseCurrency":"56756756-e89b-12d3-a456-426614174000",
            "QuoteCurrencyId":"123e4567-e89b-12d3-a456-56464r4534",
            "PriceDecimalPlaces":"3",
            "MinimumOrderAmount":"22.56",
            "MaximumOrderAmount":"65.89",
            "LastPrice":"124.98",
            "IsActive":"TRUE",
            "IsDefault":"FALSE",
            "MakerFee":"99.00",
            "TakerFee":"90.89",
            "FeeType":"FEE_TYPE_FIXED",
            "CreatedAt":"12-12-2021 12:12:12",
            "UpdatedAt":"",
            "DeletedAt":null
         },
         {
            "ID":"123e4567-e89b-12d3-a456-34534534544",
            "Name":"BTC_ETH",
            "BaseCurrency":"56756756-e89b-12d3-a456-426614174000",
            "QuoteCurrencyId":"123e4567-e89b-12d3-a456-232423t345",
            "PriceDecimalPlaces":"3",
            "MinimumOrderAmount":"22.56",
            "MaximumOrderAmount":"65.89",
            "LastPrice":"124.98",
            "IsActive":"TRUE",
            "IsDefault":"FALSE",
            "MakerFee":"99.00",
            "TakerFee":"90.89",
            "FeeType":"FEE_TYPE_FIXED",
            "CreatedAt":"12-12-2021 12:12:12",
            "UpdatedAt":"",
            "DeletedAt":null
         }
      ],
      "Total":2
   }
}
```