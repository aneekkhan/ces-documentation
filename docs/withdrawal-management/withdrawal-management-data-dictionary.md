---
sidebar_position: 1
---

# Withdrawal Management Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In a crypto trading system, withdrawal refers to the process of transferring cryptocurrency or fiat currency from a user's trading account to an external wallet or bank account

## 3. Data Dictionary (CES V1.0)

| Field Name         | Data Type     | Constraints                                                         | Description                                      |
| ------------------ | ------------- | ------------------------------------------------------------------- | ------------------------------------------------ |
| id                 | UUID          | DEFAULT uuid_generate_v4, PRIMARY KEY, NOT NULL                     | Unique identifier for withdrawal                 |
| user_id            | UUID          | FOREIGN KEY, INDEX, ON DELETE RESTRICT, ON UPDATE CASCADE, NOT NULL | ID of the user who owns the Key bank account     |
| currency_id        | UUID          | FOREIGN KEY, INDEX, ON DELETE RESTRICT, ON UPDATE CASCADE, NOT NULL | CurrencyID of the Currency Table                 |
| wallet_id          | UUID          | FOREIGN KEY, INDEX, ON DELETE RESTRICT, ON UPDATE CASCADE, NOT NULL | WalletID of the Wallet Table                     |
| bank_account_id    | UUID          | FOREIGN KEY, INDEX, ON DELETE RESTRICT, ON UPDATE CASCADE           | BankAccountID of the BankAccount Table           |
| amount             | decimal(16,8) | NOT NULL                                                            | Amount of currency being withdrawn               |
| withdrawal_status  | tinyint(1)    | DEFAULT 0                                                           | Status of the withdrawal                         |
| fee_type           | tinyint(1)    | NOT NULL                                                            | Type of the fee (FIXED PERCENTAGE)               |
| fee_amount         | decimal(16,8) | NOT NULL                                                            | Amount of the fee for the withdrawal             |
| total_amount       | decimal(16,8) | NOT NULL                                                            | Total amount to be withdrawn, including fee      |
| withdrawal_method  | varchar(50)   | NOT NULL                                                            | Method of withdrawal                             |
| withdrawal_account | varchar(255)  | NOT NULL                                                            | Account details for the withdrawal method        |
| withdrawal_date    | datetime      | NOT NULL                                                            | Date and Time when the withdrawal was initiated  |
| processed_date     | datetime      | NOT NULL                                                            | Date and Time when the withdrawal was processed  |
| withdrawal_note    | text          | DEFAULT ''                                                          | Ant additional notes regarding the withdrawal    |
| payment_gateway    | varchar(50)   | NOT NULL                                                            | Payment gateway used for the withdrawal          |
| transaction_id     | varchar(255)  | DEFAULT ''                                                          | ID of the transaction on the payment gateway     |
| created_at         | Timestamp     | NOT NULL                                                            | Timestamp when the bank account was created      |
| updated_at         | Timestamp     | NOT NULL                                                            | Timestamp when the bank account was last updated |
| created_by         | UUID          | NOT NULL                                                            | ID of By whom Bank account is created            |
| updated_by         | UUID          | NOT NULL                                                            | ID of By whom Bank account was last updated      |

`
`

## 4. Enum Fields

#### **FeeType**

&nbsp;

- FEE_TYPE_UNKNOWN
- FEE_TYPE_FIXED
- FEE_TYPE_PERCENTAGE
