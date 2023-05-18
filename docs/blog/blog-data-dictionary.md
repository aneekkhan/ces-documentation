---
sidebar_position: 13
---

# Blog Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

 In a crypto trading system blog can be a valuable addition to enhance user
 engagement, provide educational resources, and improve overall customer experience.

## 3. Data Dictionary (CES V1.0)

| Field Name                | Data Type    | Constraints                           | Description                                                                |
| ------------------------- | ------------ | ------------------------------------- | -------------------------------------------------------------------------- |
| id                        | UUID         | DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for the blog                    |
| user_id                   | UUID         | Foreign KEY                            | User's id                                         |
| title                     | varchar(255) | NOT NULL                              | Title of the blog                                       |
| content                   | text         | NOT NULL                              | Content of the blog                                       |
| author_name               | varchar(100) | NOT NULL                              | Name of the author of the blog                         |
| category                  | varchar(50)  | NOT NULL                              | Category of the blog                                       |
| tags                      | varchar(255) | NOT NULL                              | Tags associated with the blog                              |
| image_url                 | varchar(255) | NOT NULL                              | URL of the main image for the blog                         |
| published_at              | TIMESTAMP    | NOT NULL                              | Timestamp of when the blog was published                     |
| is_published              | tinyint(1)   | DEFAULT 0                             | Flag indicating whether the blog is published or not       |
| is_featured               | tinyint(1)   | DEFAULT 0                             | Flag indicating whether the blog is featured or not        |
| views                     | int          | NOT NULL                              | Number of views for the blog                |
| created_at                | TIMESTAMP    | NOT NULL                              | Timestamp of when the blog was created                       |
| updated_at                | TIMESTAMP    | NOT NULL                              | Timestamp of when the blog was last updated                  |
| created_by                | UUID         | NOT NULL                              | ID of user/admin who is created the blog                    |
| updated_by                | UUID         | NOT NULL                              | ID of user/admin who is updated the blog     |
| slug                      | varchar(255) | NOT NULL,UNIQUE                       | Slug indicating  bolg's title or name                       |
| category_id               | UUID         | Foreign KEY                           | Category  id indicating  Category's id         |
``
``


## 4.Enum fields

#### **BooleanType**

&nbsp;

- FALSE
- TRUE