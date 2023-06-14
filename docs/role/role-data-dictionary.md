---
sidebar_position: 18
---

# Role Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

Role management is a feature in crypto exchange system that allows administrators to manage user access to various system features and resources based on predefined roles. With this feature, administrators can create, modify, and delete roles as well as assign specific permissions and access levels to each role.But an "administrator" role might have full access to all system
features and resources.

## 3. Data Dictionary (CES V1.0)

| Field Name        | Data Type    | Constraints                            | Description                                                   |
| ----------------- | ------------ | -------------------------------------- | ------------------------------------------------------------- |
| id                | UUID         | DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for the role                                |
| role_name         | varchar(50)  | NOT NULL                               | Name of the role                                              |
| role_description  | VARCHAR(255) | NOT NULL                               | Description of the role                                       |
| is_active         | varchar(50)  | DEFAULT 'FALSE'                        | Flag indicating whether the role is currently active or not   |
| created_at        | TIMESTAMP    | NOT NULL                               | Timestamp of when the role was created                        |
| updated_at        | TIMESTAMP    | NOT NULL                               | Timestamp of when the role was last updated                   |
| created_by        | varchar(50)  | NOT NULL                               | ID of user/admin who is created the role                      |
| updated_by        | varchar(50)  | NOT NULL                               | ID of user/admin who is updated the role                      |
| slug              | varchar(255) | NOT NULL,UNIQUE                        | Slug indicating role's name                                   |
| permissions       | varchar(50)  | NOT NULL                               | Permissions indicating role's permissions                     |
| accessible_routes | TEXT[]       | NOT NULL DEFAULT '{}'                  | Indicating the route which the admin/user is currently access |
| deleted_at        | TIMESTAMP    | DEFAULT NULL                           | Timestamp of when the role was deleted                        |
| deleted_by        | varchar(50)  | DEFAULT NULL                           | ID of user/admin who has deleted the role                     |


## 4.Enum fields

#### **BooleanType**


    - FALSE
    - TRUE
