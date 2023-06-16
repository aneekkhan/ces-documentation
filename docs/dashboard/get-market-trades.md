---
sidebar_position: 2
---

# Get market trade history

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user/admin can get market trade history.


## 3. API

### Get market trade history Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
}
```

### Get market trade history Response example:

```json
{
   "Data":{
      "Trades":[
        {
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "Date":"2020-03-24T06:03:00.348+03:00",
         "Price":"4353564.54",
         "Amount":"004.54",
         "TotalPrice":"45344545.56",
        },
         {
         "ID":"123e4567-e89b-12d3-a456-426613454000",
         "Date":"2020-03-24T06:03:00.348+03:00",
         "Price":"4353564.54",
         "Amount":"004.54",
         "TotalPrice":"45344545.56",
        }
      ]
    
   }
}
```