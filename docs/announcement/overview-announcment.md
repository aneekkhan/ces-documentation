---
sidebar_position: 1
---

# Announcement Overview

## 1. Version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

announcement is a message posted in the announcement section of the website. It is used to inform users about the latest news, updates, and other important information.

## 3. Data Dictionary

| Field Name           | Data Type    | Constraints                          | Description                                          |
| ------------------   | ------------ | ------------------------------------ | ---------------------------------------------------- |
| id                   | UUID         | PRIMARY KEY, AUTO_INCREMENT, NOT NULL| Unique identifier for the announcement               |
| author_id            | UUID         | FOREIGN KEY                          | ID of the user who created the announcement          |
| title                | varchar(255) | NOT NULL                             | Title of the announcement                            |
| content              | text         | NOT NULL                             | Body text of the announcement                        |
| is_active            | tinyint(1)   | DEFAULT 0                            | Flag indicating whether announcement is active       |
| announcmentType      | tinyint(1)   | DEFAULT 0                            | Flag indicating type of the announcement             |
| start_date           | datetime     | NOT NULL                             | Start date of the announcement                       |
| end_date             | datetime     | NOT NULL                             | End date of the announcement                         |
| created_at           | datetime     | NOT NULL                             | Timestamp of when the support ticket was created     |
| updated_at           | datetime     | NOT NULL                             | Timestamp of when the support ticket was updated     |


## 4. Enum fields

#### **IsActive**

      type: tinyint(1)
      field name: is_active

    - title: TRUE
      const: 1
    - title: FALSE
      const: 0

#### **AnnouncmentType**

      type: tinyint(1)
      field name: AnnouncmentType 

    - title: WARNING
      const: 3
    - title: CRITICAL
      const: 2
    - title: INFO
      const: 1
    - title: UNKNOWN
      const: 0
