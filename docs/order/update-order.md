---
sidebar_position: 4
---

# Update Order

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system coin/currency can get details by ID or Symbol or Name.


## 3. API

### Update Order Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
   "UserId":"456e4567-e89b-12d3-a456-426614174000",
   "TradePairId":"3456786e-e89b-12d3-a456-46456234556",
   "Category":"STOP_LOSS",
   "Type":"BUY",
   "Status":"COMPLETED",
   "Quantity":"0.09356620",
   "Price":"8947.90000000",
   "StopLimit":"8947.90000009",
   "Total":"837.22103699",
   "FeeType":"MAKER",
   "FeeAmount":"0.00000020",
   "FeeCurrencyId":"3456786e-e89b-12d3-a456-4645626778",
   "ExecutedQuantity":".0004",
   "ExecutedTotal":"4.0006",
   "UpdatedBy":"456e4567-e89b-12d3-a456-426614174000"
}
```

###  Update Order Response example:

```json
{
   "Data":{
      "Order":{
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "UserId":"456e4567-e89b-12d3-a456-426614174000",
         "TradePairId":"3456786e-e89b-12d3-a456-46456234556",
         "Category":"STOP_LOSS",
         "Type":"BUY",
         "Status":"OPEN",
         "Quantity":"0.09356620",
         "Price":"8947.90000000",
         "StopLimit":"8947.90000009",
         "Total":"837.22103699",
         "FeeType":"MAKER",
         "FeeAmount":"0.00000020",
         "FeeCurrencyId":"3456786e-e89b-12d3-a456-4645626778",
         "ExecutedQuantity":".0004",
         "ExecutedTotal":"4.0006",
         "CreatedBy":"456e4567-e89b-12d3-a456-426614174000",
         "CreatedAt":"2020-03-24T06:03:00.348+03:00",
         "UpdatedBy":"",
         "UpdatedAt":"",
         "CancelledAt":""
      }
   }
}
```