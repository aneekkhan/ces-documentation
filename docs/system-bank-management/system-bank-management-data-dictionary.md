---
sidebar_position: 1
---

# Bank Account Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In a crypto trading system, withdrawal refers to the process of transferring cryptocurrency or fiat currency from a user's trading account to an external wallet or bank account

## 3. Data Dictionary (CES V1.0)

| Field Name                | Data Type    | Constraints                           | Description                                                                |
| ------------------------- | ------------ | ------------------------------------- | -------------------------------------------------------------------------- |
| id                        | UUID          | PRIMARY KEY, DEFAULT uuid_generate_v4(), NOT NULL | Unique identifier for bank account                                                                       |
| user_id                   | varchar(50)          | FOREIGN KEY, INDEX, ON DELETE RESTRICT, ON UPDATE CASCADE                                                                            | ID of the user who owns the Key bank account                                                          |
| reference_number          | varchar(255) | NOT NULL                              | Reference Number of the Bank                                                                           |
| bank_name                 | varchar(255) | NOT NULL                       | Name of the bank where the account is held                                                          |
| account_name              | varchar(255) | NOT NULL                              | Name on the bank account                                                                            |
| account_number            | varchar(255) | NOT NULL                              | Bank account number                                                                             |
| account_holder            | varchar(255) | NOT NULL                              | Bank account holder Name                                                                               |
| routing_number            | varchar(255) | NOT NULL                              | Bank routing number                                                                             |
| swift_code                | varchar(255) | NOT NULL                              | SWIFT code for international transfers                                                            |
| iban                      | varchar(255) | NOT NULL                              | IBAN number for international transfers                                                            |
| bic                       | varchar(255) | NOT NULL                              | BIC number for international transfers                                                            |
| is_system                 | tinyint(1)   | DEFAULT 0                             | Indicates if this is the system bank account                                              |
| country_code                | varchar(20) | NOT NULL                                 | Country ID indicating the Bank location                                                                  |
| bank_address              | varchar(255) | NOT NULL                              | Bank Address  indicating the address of the Bank                                                 |
| account_holder_address    | varchar(255) | NOT NULL                              | Account Holder Address indicating the address of the account owner                                |
| is_verified               | tinyint(1)   | DEFAULT 0                             | IsVerified indicating whether the Bank account verified or not                                           |
| is_active                 | tinyint(1)   | DEFAULT 0                             | IsActive indicating whether the Bank Account active or not                                             |
| created_at                | Timestamp    | NOT NULL                              | Timestamp when the bank account was created                                                           |
| updated_at                | Timestamp    | NOT NULL                              | Timestamp when the bank account was last updated                                                      |
| created_by                | UUID         | NOT NULL                              | ID of By whom Bank account is created                                                                 |
| updated_by                | UUID         | NOT NULL                              | ID of By whom Bank account  was last updated                                                          |
``
``

## 4. Enum Fields
#### **BooleanType**

&nbsp;

- FALSE
- TRUE
