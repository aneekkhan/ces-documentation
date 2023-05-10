---
sidebar_position: 5
---

# List KYC

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can get kyc verification list.


## 3. API

### List kyc verification Request example:

```json
{
   "SortBy":"DESC",
   "OrderByData":"submitted_at",
   "SearchTerm":"",
   "Limit":"10",
   "Offset":"0",
   "Status":"",
   "StartDate":"2020-03-24T06:03:00.348+03:00",
   "EndDate":"",
   "Status":"",
   "UserId":"",
   "DocumentType":"",
}
```

### List kyc verification Response example:

```json
{
   "Data":{
      "kyc":[
         {
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
         },
         {
            "ID":"6867867e344-e89b-12d3-a456-426614174000",
            "UserId":"1234435r5-e89b-12d3-a456-426614174000",
            "Status":"APPROVED",
            "DocumentType":"DRIVER_LICENSE",
            "DocumentNumber":"47567566444",
            "DocumentPhoto":["passport.png"],
            "SelfieWithDocument":["passportselfie.png"],
            "SubmittedAt":"2020-03-24T06:03:00.348+03:00",
            "ApprevedAt":"2020-03-24T06:03:00.348+03:00",
            "ApprovedBy":"123e4567-e89b-12d3-a456-426614174000",
            "RejectedAt":"",
            "RejectedBy":"",
            "RejectedReason":""
         }
      ],
      "Total":2
   }
}

```
