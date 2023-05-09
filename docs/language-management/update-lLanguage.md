---
sidebar_position: 4
---

# Update Language

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can update Language.


## 3. API

### Update Language Request Example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174111",
  "Name": "Arabic",
  "ShortCode": "arb",
  "Direction": "PAGE_DIRECTION_RIGHT_TO_LEFT",
  "Icon": "https://demo-exchange.squaredbyte.com/storage/images/coin-icons/default.png",
  "IsActive": "IS_ACTIVE_TRUE"
}
```
### Update Language Response Example:

```json
{
  "Data": {
    "Language": {
      "ID": "123e4567-e89b-12d3-a456-426614174111",
      "Name": "Arabic",
      "ShortCode": "arb",
      "Direction": "PAGE_DIRECTION_RIGHT_TO_LEFT",
      "Icon": "https://demo-exchange.squaredbyte.com/storage/images/coin-icons/default.png",
      "IsActive": "IS_ACTIVE_TRUE",
      "UpdatedAt": "2023-05-08 09:12:15",
      "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025"
    }
  }
}
```

## 4. Enum Fields
#### **direction**
&nbsp;

	PAGE_DIRECTION_LEFT_TO_RIGHT
	PAGE_DIRECTION_RIGHT_TO_LEFT

#### **IsActive**
&nbsp;

	IS_ACTIVE_FALSE
	IS_ACTIVE_TRUE
	