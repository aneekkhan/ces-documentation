---
sidebar_position: 4
---

# Update KYC

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user/admin can update kyc.


## 3. API

### update kyc verification Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
   "Status":"APPROVED"
}
```

### update kyc verification Response example:

```json
{
   "Data":{
      "kyc":{
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "UserId":"456e4567-e89b-12d3-a456-426614174000",
         "Status":"PENDING",
         "DocumentType":"PASSPORT",
         "DocumentNumber":"123456789",
         "DocumentPhoto":["passport.png"],
         "SelfieWithDocument":["passportselfie.png"],
         "SubmittedAt":"2020-03-24T06:03:00.348+03:00",
         "ApprevedAt":"",
         "ApprovedBy":"",
         "RejectedAt":"",
         "RejectedBy":"",
         "RejectedReason":""
      }
   }
}

```