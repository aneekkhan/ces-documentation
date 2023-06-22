---
sidebar_position: 6
---

# Get Trade-pair List

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user/admin can get Trade-pair List.


## 3. API

### Get Trade-pair List Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
}
```

### Get Trade-pair List Response example:

```json
{
   "Data":{
      "List":[
         {
            "ID":"123e4567-e89b-12d3-a456-426614174000",
            "BaseCurrency":"USD",
            "QuoteCurrency":"BTC",
            "Price":"123.00",
            "Volume":"0.00",
         },
         {
            "ID":"123e4567-e89b-12d3-a456-426614174678",
            "BaseCurrency":"ETH",
            "QuoteCurrency":"BTC",
            "Price":"6555.00",
            "Volume":"0.00",
         }
      ]
   }
}
```