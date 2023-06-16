---
sidebar_position: 1
---

# Get user buy orders history

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user/admin can get user buy orders history.


## 3. API

### Get user buy orders history Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
}
```

### Get user buy orders history Response example:

```json
{
   "Data":{
      "SellOrders":[
        {
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "Price":"86455.34",
         "Amount":"0.00",
         "Total":"4353564.54",
        }
      ]
    
   }
}
```