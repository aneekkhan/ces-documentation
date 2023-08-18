---
sidebar_position: 4
---

# List Sub Category

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can get sub-category list by ParentID.


## 3. API

### List Sub Category Request example:

```json
{
    "ParentID":"123e4567-e89b-12d3-a456-426614174111",
    "CategoryFilter":
    {
        "SortBy": "ASC",
        "SortByColumn": "CategoryName",
        "SearchTerm": "News",
        "CategoryName": "News",
        "StartDate": "2020-03-24T06:03:00.348+03:00",
        "EndDate": "2021-03-24T06:04:00.348+03:00"
    }
}

```

### List Sub Category Response example:

```json
{
  "Data": {
      "CategoryData": 
      [
        {
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
        }, 
        {
          "ID":"123e4567-e89b-12d3-a456-426614174001",
          "CategoryName":"Technology",
          "CategoryImage":["category.png"],
          "MetaTitle":"Title",
          "MetaDescription":"Description",
          "keyword":"tech , news",
          "ParentID":"123e4567-e89b-12d3-a456-426614174111",
          "CreatedAT":"2023-05-08 09:12:15",
          "CreatedBy":"123e4567-e89b-12d3-a456-426614174000",
          "DeletedAt":null
        }
      ]
    },
  "TotalPages": 2
}
```
