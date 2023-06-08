---
sidebar_position: 4
---

# List Order

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can get order list.


## 3. API

### List order Request example:

```json
{
   "SortBy":"DESC",
   "SortByColumn":"id",
   "SearchTerm":"",
   "Status":"",
   "TradePairId":"3456786e-e89b-12d3-a456-46456234556",
   "Type":"",
   "OrderCategory":"",
}
```

### List order Response example:

```json
{
   "Data":{
      "Orders":[
         {
            "ID":"123e4567-e89b-12d3-a456-426614174000",
            "UserId":"456e4567-e89b-12d3-a456-426614174000",
            "TradePairId":"3456786e-e89b-12d3-a456-46456234556",
            "OrderCategory":"ORDER_CATEGORY_STOP_LOSS",
            "Type":"BUY",
            "Status":"OPEN",
            "Quantity":"0.09356620",
            "Price":"8947.90000000",
            "StopLimit":"8947.90000009",
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
         },
         {
            "ID":"85655r43-e89b-12d3-a456-2343534456556",
            "UserId":"456e4567-e89b-12d3-a456-426614174000",
            "TradePairId":"3456786e-e89b-12d3-a456-46456234556",
            "OrderCategory":"ORDER_CATEGORY_MARKET",
            "Type":"SELL",
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
      ],
      "Total":2
   }
}

```
