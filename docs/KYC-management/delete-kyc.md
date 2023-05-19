---
sidebar_position: 6
---

# Delete KYC Verification

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can delete kyc verification by ID.


## 3. API

### Request example:

```json
{
  "ID":"123e4567-e89b-12d3-a456-426614174000",
}
```
### Response example:

```json
{
  "Data":{
    "Kyc":{
      "IsDeleted": true
    }
  }
}
```