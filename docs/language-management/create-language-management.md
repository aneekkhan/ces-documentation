---
sidebar_position: 2
---

# Create Language Management

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In a crypto trading system, Language Management is about switching the language of user choice.


## 3. API

### Create Language Request example:

```json
{
    "Name": "Bangla",
    "ShortCode": "Ban",
    "Icon": "https://demo-exchange.squaredbyte.com/storage/images/coin-icons/default.png",
    "Direction": "PAGE_DIRECTION_LEFT_TO_RIGHT",
    "IsActive": "IS_ACTIVE_TRUE"
}
```

### Create Language Response example:

```json
{
  	"ID": "123e4567-e89b-12d3-a456-426614174111",
	"Name": "Bangla",
    "ShortCode": "Ban",
    "Icon": "https://demo-exchange.squaredbyte.com/storage/images/coin-icons/default.png",
    "Direction": "PAGE_DIRECTION_LEFT_TO_RIGHT",
    "IsActive": "IS_ACTIVE_TRUE",
	"CreatedAt": "2023-05-08 09:12:15",
	"UpdatedAt": "2023-05-08 09:12:15",
	"CreatedBy": "123e4567-e89b-12d3-a456-426614174025",
	"UpdatedBy": "123e4567-e89b-12d3-a456-426614174025"
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
	