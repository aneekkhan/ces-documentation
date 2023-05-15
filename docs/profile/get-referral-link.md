---
sidebar_position: 4
---

# Get Referral

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can get his referral link.


## 3. API

### Get referral link Request example:

```json
{
   "Data":{
      "User":
         {
            "ID":"123e4567-e89b-12d3-a456-426614174000",
         }
   }
}
```

### Get referral link Response example:

```json
{
   "Data":{
      "User":
         {
            "ID":"123e4567-e89b-12d3-a456-426614174000",
            "Link":"https://demo-exchange.squaredbyte.com/register?ref=8lDb96EgCm0yml4w"
         }
   }
}

```
