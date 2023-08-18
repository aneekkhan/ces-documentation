---
sidebar_position: 1
---

# Category Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

In a crypto trading system Blog categories organize your site and allow readers to find the information they want.

## 3. Data Dictionary (CES V1.0)

| Field Name       | Data Type    | Constraints                            | Description                                          |
| ------------     | ------------ | -------------------------------------- | ---------------------------------------------------- |
| id               | UUID         | DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for the category                   |
| category_name    | varchar(255) | NOT NULL                               | Name of the category                                 |
| category_img     | text array   | NOT NULL                               | Image of the category                                |
| parent_id        | varchar(100) | NOT NULL                               | Parent category ID                                   |
| meta_title       | varchar(255) | NOT NULL                               | Title of the category                                |
| meta_description | varchar(500)  | NOT NULL                               | Description of the category                          |
| keyword          | varchar(255) | NOT NULL                               | Keywords of the category                             |
| created_at       | TIMESTAMP    | NOT NULL                               | Timestamp of when the category was created           |
| deleted_at       | TIMESTAMP    | NOT NULL                               | Timestamp of when the category was last deleted      |
| created_by       | UUID         | NOT NULL                               | ID of admin who is created the category              |
| deleted_by       | UUID         | NOT NULL                               | ID of admin who is deleted the category              |
