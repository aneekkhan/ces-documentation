---
sidebar_position: 2
---

# Get Preference

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can get his profile Preference.

### 3. GET API

### Get Profile Preference Request example:

```json
{
  "ID": "456e4567-e89b-12d3-a456-426614174000"
}
```

### Get Profile Preference Response example:

```json
{
  "Data": {
    "Preference": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "DisplayLanguage": "English",
      "DefaultTradePair": "BTC_USD"
    }
  }
}
```

### 3. Edit API

### Edit Profile Preference Request example:

```json
{
  "Data": {
    "Preference": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "DisplayLanguage": "Spanish",
      "DefaultTradePair": "BTC_USD"
    }
  }
}
```

### Edit Profile Preference Response example:

```json
{
   "Data":{
      "Preference":{
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "DisplayLanguage":"Spanish",
         "DefaultTradePair":"BTC_USD",
         "UpdatedAt": "2023-05-08 09:12:15",
         "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025"
      }
   }
}
`
```
