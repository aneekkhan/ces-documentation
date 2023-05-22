---
sidebar_position: 1
---

# Support Ticket Overview

## 1. Version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

customer supporting system by ticketing.

## 3. Data Dictionary

| Field Name   | Data Type    | Constraints                           | Description                                                        |
| ------------ | ------------ | ------------------------------------- | ------------------------------------------------------------------ |
| id           | UUID         | PRIMARY KEY, AUTO_INCREMENT, NOT NULL | Unique identifier for the support ticket                           |
| user_id      | varchar(50)  | NOT NULL                              | ID of the user who created the Key support ticket                  |
| support_type | varchar(20)  | NOT NULL                              | Type of support request (e.g. technical, billing, general inquiry) |
| subject      | varchar(20)  | NOT NULL                              | Subject of the support request                                     |
| message      | text         | NOT NULL                              | Body of the support request message                                |
| attachment   | varchar(255) | NOT NULL                              | Path to any attached file(s) related to the support request        |
| status       | tinyint(1)   | DEFAULT 0                             | Current status of the support request (e.g. open, closed, pending) |
| priority     | varchar(20)  | NOT NULL                              | Priority level of the support request (e.g. high, medium, low)     |
| created_at   | timestamp    | NOT NULL                              | Timestamp of when the support ticket was created                   |
| updated_at   | timestamp    | NOT NULL                              | Timestamp of when the support ticket was updated                   |
| resolved_at  | timestamp    | NOT NULL                              | Timestamp of when the support ticket was resolved                  |
| assigned_to  | UUID         | NOT NULL                              | ID of the admin who is assigned support ticket                     |
| created_by   | UUID         | NOT NULL                              | ID of the admin who is assigned support ticket                     |
| updated_by   | UUID         | NOT NULL                              | ID of the admin who is assigned support ticket                     |

## 4. Enum fields

#### **Status**

      type: tinyint(1)
      field name: status

    - title: OPEN
      const: 4
    - title: PROGRESSING
      const: 3
    - title: RESOLVED
      const: 2
    - title: CLOSED
      const: 1
    - title: UNKNOWN
      const: 0

#### **Priority**

      type: tinyint(1)
      field name: priority

    - title: HIGH
      const: 3
    - title: MEDIUM
      const: 2
    - title: LOW
      const: 1
    - title: UNKNOWN
      const: 0

#### **Support Type**

      type: tinyint(1)
      field name: support_type

    - title: HIGH
      const: 3
    - title: MEDIUM
      const: 2
    - title: LOW
      const: 1
    - title: UNKNOWN
      const: 0
