---
sidebar_position: 1
---

# Currency Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

Coin is a form of a currency.It can be of various types (e.g fiat,cryptocurrency).Trader will buy/sell cryptocurrency with fiat currency or another
cryptocurrency.

## 3. Data Dictionary (CES V1.0)

| Field Name                | Data Type    | Constraints                                     | Description                                                                |
| ------------------------- | ------------ | ----------------------------------------------- | -------------------------------------------------------------------------- |
| id                        | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY     | Unique identifier for currency                                             |
| symbol                    | VARCHAR(10)  | NOT NULL,UNIQUE                                 | Unique identifier for currency                                             |
| name                      | VARCHAR(50)  | NOT NULL                                        | currency name                                                              |
| coin_type                 | tinyint(1)   | DEFAULT 0                                       | Type of currency                                                           |
| icon                      | VARCHAR(100) | NOT NULL                                        | Icon for currency                                                          |
| decimals                  | INT          | NOT NULL                                        | Number of decimal places for the currency                                  |
| exchange_status           | tinyint(1)   | DEFAULT 0                                       | Flag indicating whether currency exchange status active or not             |
| deposit_status            | tinyint(1)   | DEFAULT 0                                       | Flag indicating whether currency deposit status active or not              |
| withdrawal_status         | tinyint(1)   | DEFAULT 0                                       | Flag indicating whether currency withdrawal status active or not           |
| is_active                 | tinyint(1)   | DEFAULT 0                                       | Flag indicating whether the currency is active                             |
| minimum_deposit_amount    | VARCHAR(50)  | NOT NULL                                        | Minimum amount that can be deposited                                       |
| maximum_deposit_amount    | VARCHAR(50)  | NOT NULL                                        | Minimum amount that can be deposited                                       |
| daily_deposit_limit       | VARCHAR(50)  | NOT NULL                                        | Maximum amount that can be deposited in a day                              |
| deposit_fee               | VARCHAR(50)  | NOT NULL                                        | Value of the fee charged on each deposit                                   |
| deposit_fee_type          | tinyint(1)   | DEFAULT 0                                       | Type of fee charged on each deposit (e.g. fixed,percentage)                |
| total_deposit             | VARCHAR(50)  | NOT NULL                                        | Maximum amount of currency deposited                                       |
| withdrawal_fee            | VARCHAR(50)  | NOT NULL                                        | Value of the fee charged on each withdrawal                                |
| withdrawal_fee_type       | tinyint(1)   | DEFAULT 0                                       | Type of fee charged on each withdrawal(e.g. fixed, percentage)             |
| minimum_withdrawal_amount | VARCHAR(50)  | NOT NULL                                        | Minimum amount that can be withdrawan                                      |
| maximum_withdrawal_amount | VARCHAR(50)  | NOT NULL                                        | Minimum amount that can be withdrawn                                       |
| daily_withdrawal_limit    | VARCHAR(50)  | NOT NULL                                        | Maximum amount that can be withdrawn in a day                              |
| total_withdrawal          | VARCHAR(50)  | NOT NULL                                        | Maximum amount of currency withdrawn                                       |
| created_at                | DATETIME     | NOT NULL                                        | Timestamp when the currency was added                                      |
| created_by                | UUID         | NOT NULL                                        | ID of admin who has added the currency                                     |
| updated_at                | DATETIME     | NOT NULL                                        | Timestamp when the currency was last updated                               |
| updated_by                | UUID         | NOT NULL                                        | ID of admin who has updated the currency                                   |
``
``

## 4. Enum Fields 
#### **CoinType**
&nbsp;

    - COIN_TYPE_UNKNOWN
    - COIN_TYPE_FIAT
    - COIN_TYPE_CRYPTO

#### **ExchangeStatus**
&nbsp;

    - EXCHANGE_STATUS_UNKNOWN
    - EXCHANGE_STATUS_ACTIVE
    - EXCHANGE_STATUS_INACTIVE

#### **DepositStatus**
&nbsp;

    - DEPOSIT_STATUS_UNKNOWN
    - DEPOSIT_STATUS_ACTIVE
    - DEPOSIT_STATUS_INACTIVE

#### **WithdrawalStatus**
&nbsp;
    
    - WITHDRAWAL_STATUS_UNKNOWN
    - WITHDRAWAL_STATUS_ACTIVE
    - WITHDRAWAL_STATUS_INACTIVE

#### **IsActive**
&nbsp;

    - IS_ACTIVE_TRUE
    - IS_ACTIVE_FALSE

#### **DepositFeeType**
&nbsp;

    - DEPOSIT_FEE_TYPE_UNKNOWN
    - DEPOSIT_FEE_TYPE_FEE_TYPE_FIXED
    - DEPOSIT_FEE_TYPE_FEE_TYPE_PERCENTAGE
    

#### **WithdrawalFeeType**
&nbsp;

    - WITHDRAWAL_FEE_TYPE_UNKNOWN
    - WITHDRAWAL_FEE_TYPE_FEE_TYPE_FIXED
    - WITHDRAWAL_FEE_TYPE_FEE_TYPE_PERCENTAGE

