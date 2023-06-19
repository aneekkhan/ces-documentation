---
sidebar_position: 5
---

# Get trade-pair price history

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user/admin can get trade-pair price history.


## 3. API

### Get trade-pair price history Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
   "Interval":"15 minutes"
}
```

### Get trade-pair price history Response example:

```json
{
   "Data":{
      "History":[
        {
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "Date":"2020-03-24T06:03:00.348+03:00",
         "OpenPrice":"4353564.54",
         "ClosePrice":"4353564.54",
         "HighPrice":"4353564.54",
         "LowPrice":"4353564.54",
        },
         {
         "ID":"123e4567-e89b-12d3-a456-426613454000",
         "Date":"2020-03-24T06:03:00.348+03:00",
         "OpenPrice":"4353564.54",
         "ClosePrice":"4353564.54",
         "HighPrice":"4353564.54",
         "LowPrice":"4353564.54",
        }
      ]
    
   }
}
```