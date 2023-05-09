---
sidebar_position: 1
---

# System Deposit Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

A crypto exchange deposit system is a platform or feature provided by a cryptocurrency exchange that enables users to deposit cryptocurrencies into their exchange accounts. This allows them to trade, buy or sell cryptocurrencies on the exchange

## 3. Data Dictionary (CES V1.0)

| Field Name      | Data Type     | Constraints                                 | Description                                                    |
| --------------- | ------------- | ------------------------------------------- | -------------------------------------------------------------- |
| id              | UUID          | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for the deposit                              |
| user_id         | UUID          | Foreign KEY, index                          | ID of the user who made the deposit                            |
| currency_id     | UUID          | Foreign KEY                                 | ID of the currency deposited                                   |
| amount          | decimal(18,8) | NOT NULL                                    | Amount deposited                                               |
| fee             | decimal(18,8) | NOT NULL                                    | Fee charged for the deposit                                    |
| fee_type        | tinyint(1)    | DEFAULT 0                                   | Type of fee charged for the deposit (e.g. fixed percentage)    |
| deposit_status  | tinyint(1)    | DEFAULT 0                                   | Status of the deposit (e.g. pending, completed, rejected)      |
| transaction_id  | UUID          | NOT NULL                                    | ID of the transaction on the payment gateway                   |
| bank_account_id | UUID          | Foreign KEY NOT NULL                        | ID of the bank accounts                                        |
| payment_gateway | varchar(50)   | NOT NULL                                    | Name of the payment gateway used for the deposit               |
| deposit_method  | tinyint(1)    | DEFAULT 0                                   | Method used for the deposit (e.g. bank transfer, credit, card) |
| deposit_date    | TIMESTAMP     | NOT NULL                                    | Date and time of the deposit                                   |
| deposit_notes   | varchar(255)  | NOT NULL                                    | Notes about the deposit                                        |
| created_at      | TIMESTAMP     | NOT NULL                                    | Timestamp of when the wallet was created                       |
| created_by      | UUID          | NOT NULL                                    | ID of admin who has created the Deposit                        |
| updated_at      | TIMESTAMP     | NOT NULL                                    | Timestamp when the wallet was last updated                     |
| updated_by      | UUID          | NOT NULL                                    | ID of admin who has updated the Deposit                        |
| deleted_at      | TIMESTAMP     | NOT NULL                                    | Timestamp of when the deposit was soft deleted                 |
| deleted_by      | UUID          | NOT NULL                                    | ID of admin who has deleted the Deposit                        |

`
`

## 4. Enum Fields

#### **fee_type**

&nbsp;

- FEE_TYPE_UNKNOWN
- FEE_TYPE_PENDING
- FEE_TYPE_COMPLETED
- FEE_TYPE_REJECTED

#### **deposit_status**

&nbsp;

- DEPOSIT_STATUS_UNKNOWN
- DEPOSIT_STATUS_PENDING
- DEPOSIT_STATUS_COMPLETED
- DEPOSIT_STATUS_REJECTED

#### **deposit_method**

&nbsp;

- DEPOSIT_METHOD_UNKNOWN
- DEPOSIT_METHOD_BANK_TRANSFER
- DEPOSIT_METHOD_CREDIT_CARD
