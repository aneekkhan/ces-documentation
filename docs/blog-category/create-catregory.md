---
sidebar_position: 2
---

# Create Categeory

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can add new category.


## 3. API

### Create Category Request example:

```json
{
   "CategoryName":"News",
   "CategoryImage":["category.png"],
   "MetaTitle":"Title",
   "MetaDescription":"Description",
   "keyword":"tech , news",
   "ParentID":"123e4567-e89b-12d3-a456-426614174111"
}
```

### Create Category Response example:

```json
{
   "Data":{
      "Category":{
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "CategoryName":"News",
         "CategoryImage":["category.png"],
         "MetaTitle":"Title",
         "MetaDescription":"Description",
         "keyword":"tech , news",
         "ParentID":"123e4567-e89b-12d3-a456-426614174111",
         "CreatedAT":"2023-05-08 09:12:15",
         "CreatedBy":"123e4567-e89b-12d3-a456-426614174000",
         "DeletedAt":null
      }
   }
}
`