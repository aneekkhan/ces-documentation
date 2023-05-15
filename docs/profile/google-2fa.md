---
sidebar_position: 4
---

# Google 2fa

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system user can verify through google authentication.


## 3. API

### Google 2fa Request example:

```json
{
  "Data": {
    "User": {
      "Email": "mail@mail.com",
      "Password": "1234567890",
      "Code": "2fa_Code",
    }
  }
}
```

### Google 2fa Response example:

```json
{
  "Data": {
    "User": {
      "Code": "2fa_Code",
    }
  }
}

```
