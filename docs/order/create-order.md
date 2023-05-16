---
sidebar_position: 2
---

# Create Order

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can add new buy or sell order.


## 3. API

### Create order Request example:

```json
{
   "TradePairId":"3456786e-e89b-12d3-a456-46456234556",
   "OrderCategory":"ORDER_CATEGORY_STOP_LOSS",
   "Type":"BUY",
   "Quantity":"0.09356620",
   "Price":"8947.90000000",
   "StopLimit":"",
   "TotalAmount":"837.22103699",
}
```

### Create Coin/Currency Response example:

```json
{
   "Data":{
      "Order":{
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "UserId":"456e4567-e89b-12d3-a456-426614174000",
         "TradePairId":"3456786e-e89b-12d3-a456-46456234556",
         "OrderCategory":"ORDER_CATEGORY_STOP_LOSS",
         "Type":"BUY",
         "Status":"OPEN",
         "Quantity":"0.09356620",
         "Price":"8947.90000000",
         "StopLimit":"",
         "TotalAmount":"837.22103699",
         "ExecutedQuantity":".0004",
         "ExecutedTotal":"4.0006",
         "CreatedBy":"456e4567-e89b-12d3-a456-426614174000",
         "CreatedAt":"2020-03-24T06:03:00.348+03:00",
         "UpdatedBy":"",
         "UpdatedAt":"",
         "CancelledAt":"",
         "CancelledAmount":"",
         "SettlementAmount":"",
      }
   }
}
```