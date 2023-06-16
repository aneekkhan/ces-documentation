---
sidebar_position: 23
---

# Notifications Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

In crypto exchange system notifications is a feature that many crypto exchange systems use to
provide real-time updates and alerts to their users.

## 3. Data Dictionary (CES V1.0)

| Field Name      | Data Type      | Constraints                                 | Description                                                     |
| --------------- | -------------- | ------------------------------------------- | --------------------------------------------------------------- |
| id              | UUID           | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for the notification                       |
| user_id         | varchar(100)   |  NOT NULL                                   | ID of the user who creates  the notification                       |
| title            | varchar(50)   | NOT NULL                                    | Title of the notification                       |
| details          | varchar(255)  | NOT NULL                                    | Details of the notification message                            |
| read_at          | TIMESTAMP     | NOT NULL                                    | Timestamp of when the notification was read               |
| is_read          | VARCHAR(50)   | NOT NULL DEFAULT 'FALSE'                    | Flag indicating whether the notification is 'read' or 'unread'|
| created_at      | TIMESTAMP      | NOT NULL                                    | Timestamp of when the notification was created           |
| created_by      | varchar(100)   | NOT NULL                                    | User created by                                 |
| updated_at      | TIMESTAMP      | NOT NULL                                    | Timestamp when the notification was last updated           |
| updated_by      | varchar(100)   | NOT NULL                                    | User updated by                                 |
| reference       | varchar(255)   | NOT NULL                                    | Slug indicating notification's title             |

`
`

## 4. Enum Fields

#### **is_read**

&nbsp;

      type: tinyint(1)
      field name: is_read

    - title: FALSE
      const: 0
    - title: TRUE
      const: 1
