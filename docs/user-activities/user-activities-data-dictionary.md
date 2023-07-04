---
sidebar_position: 1
---

# User Activities Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

User activities is the interactions between a User and the Platform, including use of the Company's services and API

## 3. Data Dictionary (CES V1.0)

| Field Name           | Data Type    | Constraints                                 | Description                                                                                              |
| -------------------- | ------------ | ------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| id                   | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for the Key verification request                                                       |
| user_id              | VARCHAR(100) | NOT NULL                                    | ID of the user requesting verification                                                                   |
| browser              | VARCHAR(100) | NOT NULL                                    | Browser Name and version of the user.                                                                    |
| operation_system     | VARCHAR(100) | NOT NULL                                    | Operation System of the user's system.                                                                   |
| ip_address           | VARCHAR(255) | NOT NULL                                    | Ip Address of the user's system.                                                                         |
| country              | VARCHAR(100) | NOT NULL                                    | Country of the user.                                                                                     |
| city                 | VARCHAR(100) | NOT NULL                                    | City of the user.                                                                                        |
| activity             | VARCHAR(255) | NOT NULL                                    | Activity of the user.                                                                                    |
| device               | VARCHAR(100) | NOT NULL                                    | Device type of the user.                                                                                 | 
| created_at           | TIMESTAMP    | NOT NULL                                    | Timestamp of when the user activity was created                                                          |
