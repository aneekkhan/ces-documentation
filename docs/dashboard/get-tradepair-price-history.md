---
sidebar_position: 6
---

# Get Trade-pair history price history

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user/admin can get Trade-pair price history.


## 3. API

### Get Trade-pair price history Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
}
```

### Get Trade-pair price history Response example:

```json
{
   "Data":{
      "History":{
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "LastPrice":"86455.34",
         "Change":"0.00",
         "HighPrice":"4353564.54",
         "LowPrice":"0.00",
         "Volume":"123.00",
      }
   }
}
```