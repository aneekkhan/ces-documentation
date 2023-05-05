---
sidebar_position: 13
---

# Blog Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

A user who wants to buy/sell cryptocurrency with fiat currency or another
cryptocurrency. They may be new to the cryptocurrency market and want to invest or trade in
various cryptocurrencies.

## 3. Data Dictionary (CES V1.0)

| Field Name                | Data Type    | Constraints                           | Description                                                                |
| ------------------------- | ------------ | ------------------------------------- | -------------------------------------------------------------------------- |
| id                        | UUID         | PRIMARY KEY, AUTO_INCREMENT, NOT NULL | Unique identifier for the blog                                             |
| user_id                   | UUID         | NOT NULL                              | User's id                                                             |
| title                     | varchar(255) | NOT NULL                              | User's first name                                                          |
| last_name                 | varchar(255) | NOT NULL                              | User's last name                                                           |
| email                     | varchar(255) | NOT NULL                              | User's email address                                                       |
| phone_number              | varchar(255) | NOT NULL                              | User's phone number                                                        |
| password                  | varchar(20)  | NOT NULL                              | Hashed user's password                                                     |
| is_email_verified         | BOOLEAN      | NOT NULL                              | Flag indicating whether user's the email address verified or not           |
| status                    | BOOLEAN      | DEFAULT TRUE                          | Flag indicating whether user's status active or not                        |
| account_status            | tinyint(1)   | DEFAULT TRUE                          | Flag indicating whether user's account status active, suspended or deleted |
| financial_status          | BOOLEAN      | DEFAULT TRUE                          | Flag indicating whether user's financial status active or not              |
| maintenance_access_status | BOOLEAN      | DEFAULT TRUE                          | Flag indicating whether user's maintenance access status enable or not     |
| is_phone_verified         | BOOLEAN      | NOT NULL                              | Flag indicating whether user's the phone number is verified or not         |
| is_mfa                    | BOOLEAN      | NOT NULL                              | Flag indicating whether user's mfa have or not                             |
| mfa_type                  | BOOLEAN      | NOT NULL                              | Flag indicating whether user's mfa_type is verified or not                 |
| created_at                | varchar(20)  | NOT NULL                              | Timestamp when the user account was created                                |
| updated_at                | varchar(20)  | NOT NULL                              | Timestamp when the user account was last updated                           |
``
``

