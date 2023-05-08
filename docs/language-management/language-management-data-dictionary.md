---
sidebar_position: 1
---

# Language Management Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In a crypto trading system, Language Management is about switching the language of user choice.

## 3. Data Dictionary (CES V1.0)

| Field Name                | Data Type    | Constraints                           | Description                                                                |
| ------------------------- | ------------ | ------------------------------------- | -------------------------------------------------------------------------- |
| id                        | UUID         | PRIMARY KEY, DEFAULT uuid_generate_v4(), NOT NULL                                                                               | Unique identifier for language                                                    |
| name                      | varchar(50)  | unique, NOT NULL                      | Unique name of language                                                           |
| short_code                | varchar(20)  | unique, NOT NULL                      | Short code of language                                                           |
| icon                      | varchar(255) | NOT NULL                              | Icon of the language                                                               |
| direction                 | varchar(20)  | NOT NULL                              | language starting direction                                                         |
| is_active                 | tinyint(1)   | DEFAULT 0                             | IsActive indicating whether the language active or not                              |
| created_at                | Timestamp    | NOT NULL                              | Timestamp when the bank account was created                                          |
| updated_at                | Timestamp    | NOT NULL                              | Timestamp when the bank account was last updated                                     |
| created_by                | UUID         | NOT NULL                              | ID of By whom Bank account is created                                               |
| updated_by                | UUID         | NOT NULL                              | ID of By whom Bank account  was last updated                                        |
``
``

