---
sidebar_position: 1
---

# Payment Method Overview

## 1. Version control

| Version     | Date        | Description of Changes      |
| ----------- | ----------- | --------------------------- |
| CES V1.0    | May 3, 2023 | Initial Release             |


## 2. Overview

customer supporting system by ticketing.

## 3. Data Dictionary

| Field Name           | Data Type    | Constraints                          | Description                                          |
| ------------------   | ------------ | ------------------------------------ | ---------------------------------------------------- |
| id                   | UUID         | PRIMARY KEY, AUTO_INCREMENT, NOT NULL| Unique identifier for the payment method             |
| name                 | varchar(50)  | FOREIGN KEY                          | Name of the payment method                           |
| description          | varchar(255) | NOT NULL                             | Description of the payment method                    |
| is_active            | tinyint(1)   | NOT NULL                             | Flag indicating whether the payment method is active |
| created_at           | datetime     | NOT NULL                             | Timestamp of when the support ticket was created     |
| updated_at           | datetime     | NOT NULL                             | Timestamp of when the support ticket was updated     |
| deleted_at           | datetime     | NOT NULL                             | Timestamp of when the support ticket was deleted     |


## 4. Enum fields

#### **IsActive**


      type: tinyint(1)
      field name: is_active 

    - title: ACTIVE
      const: 2
    - title: INACTIVE
      const: 1
    - title: UNKNOWN
      const: 0