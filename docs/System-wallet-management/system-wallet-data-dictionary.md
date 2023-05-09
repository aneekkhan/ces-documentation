---
sidebar_position: 1
---

# System Wallet Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

A user who wants to buy/sell cryptocurrency with fiat currency or another
cryptocurrency. They may be new to the cryptocurrency market and want to invest or trade in
various cryptocurrencies.

## 3. Data Dictionary (CES V1.0)

| Field Name      | Data Type      | Constraints                                 | Description                                                     |
| --------------- | -------------- | ------------------------------------------- | --------------------------------------------------------------- |
| id              | UUID           | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for the wallet                                |
| user_id         | UUID           | Foreign KEY                                 | ID of the user who owns the wallet                              |
| currency_id     | UUID           | Foreign KEY                                 | ID of the currency held in the wallet                           |
| name            | varchar(50)    | NOT NULL                                    | Name of the wallet                                              |
| symbol          | varchar(50)    | Foreign KEY                                 | symbol of the trades held in the wallet                         |
| balance         | decimal(30,10) | NOT NULL                                    | Current balance in the wallet                                   |
| is_default      | tinyint(1)     | DEFAULT 0                                   | Flag indicating whether the wallet is the user's default wallet |
| is_active       | tinyint(1)     | DEFAULT 0                                   | Flag indicating whether the wallet is 'Enable' or 'Disable'     |
| last_deposit    | TIMESTAMP      | NOT NULL                                    | Timestamp when the wallet was last updated                      |
| last_withdrawal | TIMESTAMP      | NOT NULL                                    | Timestamp of the last withdrawal made from the wallet           |
| created_at      | TIMESTAMP      | NOT NULL                                    | Timestamp of when the wallet was created                        |
| created_by      | UUID           | NOT NULL                                    | ID of admin who has created the Wallet                          |
| updated_at      | TIMESTAMP      | NOT NULL                                    | Timestamp when the wallet was last updated                      |
| updated_by      | UUID           | NOT NULL                                    | ID of admin who has updated the Wallet                          |

`
`

## 4. Enum Fields

#### **is_default**

&nbsp;

- IS_DEFAULT_TRUE
- IS_DEFAULT_FALSE

#### **is_active**

&nbsp;

- IS_ACTIVE_TRUE
- IS_ACTIVE_FALSE
