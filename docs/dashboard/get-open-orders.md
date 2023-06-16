---
sidebar_position: 3
---

# Get user open orders history

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user/admin can get user open orders history.


## 3. API

### Get user open orders history Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
}
```

### Get user open orders history Response example:

```json
{
   "Data":{
      "Orders":[
        {
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "Date":"2020-03-24T06:03:00.348+03:00",
         "Type":"BUY",
         "UnitPrice":"4353564.54",
         "Amount":"004.54",
         "OpenAmount":"4564.54",
         "FilledAmount":"245.54",
         "TotalPrice":"45344545.56",
         "TriggerCondition":"8947.90000009",
        },
         {
         "ID":"123e4567-e89b-12d3-a456-426613454000",
         "Date":"2020-03-24T06:03:00.348+03:00",
         "Type":"SELL",
         "UnitPrice":"4353564.54",
         "Amount":"004.54",
         "OpenAmount":"4564.54",
         "FilledAmount":"245.54",
         "TotalPrice":"45344545.56",
         "TriggerCondition":"8947.90000009",
        }
      ]
    
   }
}
```