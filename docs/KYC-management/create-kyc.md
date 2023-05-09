---
sidebar_position: 2
---

# Create KYC

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can add new kyc verification.


## 3. API

### Create KYC Verification Request example:

```json
{
   "Data":{
      "kyc":{
         "UserId":"456e4567-e89b-12d3-a456-426614174000",
         "DocumentType":"PASSPORT",
         "DocumentNumber":"123456789",
         "DocumentPhoto":"passport.png",
         "SelfieWithDocument":"passportselfie.png"
      }
   }
}
```

### Create KYC Verification Response example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000"
}
`