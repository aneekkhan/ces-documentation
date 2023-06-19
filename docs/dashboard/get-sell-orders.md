---
sidebar_position: 4
---

# Get user sell orders history

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user/admin can get user sell orders history.


## 3. API

### Get user sell orders history Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
}
```

### Get user sell orders history Response example:

```json
{
   "Data":{
      "SellOrders":[
        {
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "Price":"86455.34",
         "Amount":"03.00",
         "Total":"4353564.54",
        },
        {
         "ID":"123e4567-e89b-12d3-a456-4266345474000",
         "Price":"134.34",
         "Amount":"09.00",
         "Total":"345.54",
        }
      ]
    
   }
}
```