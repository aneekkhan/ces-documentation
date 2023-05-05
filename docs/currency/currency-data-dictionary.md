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
| deposit_fee               | VARCHAR(50)  | NOT NULL                                        | Value of the fee charged on each deposit                                   |
| deposit_fee_type          | tinyint(1)   | DEFAULT 0                                       | Type of fee charged on each deposit (e.g. fixed,percentage)                |
| minimum_deposit_amount    | VARCHAR(50)  | NOT NULL                                        | Minimum amount that can be deposited                                       |
| maximum_deposit_amount    | VARCHAR(50)  | NOT NULL                                        | Minimum amount that can be deposited                                       |
| daily_deposit_limit       | VARCHAR(50)  | NOT NULL                                        | Maximum amount that can be deposited in a day                              |
| total_deposit             | VARCHAR(50)  | NOT NULL                                        | Maximum amount of currency deposited                                       |
| withdrawal_fee            | VARCHAR(50)  | NOT NULL                                        | Value of the fee charged on each withdrawal                                |
| withdrawal_fee_type       | tinyint(1)   | DEFAULT 0                                       | Type of fee charged on each withdrawal(e.g. fixed, percentage)             |
| minimum_withdrawal_amount | VARCHAR(50)  | NOT NULL                                        | Minimum amount that can be withdrawan                                      |
| maximum_withdrawal_amount | VARCHAR(50)  | NOT NULL                                        | Minimum amount that can be withdrawn                                       |
| daily_withdrawal_limit    | VARCHAR(50)  | NOT NULL                                        | Maximum amount that can be withdrawn in a day                              |
| total_withdrawal          | VARCHAR(50)  | NOT NULL                                        | Maximum amount of currency withdrawn                                       |
| created_at                | DATETIME     | NOT NULL                                        | Timestamp when the currency was added                                      |
| created_by                | UUID         | NOT NULL                                        | ID of admin who has added the currency                                     |
| updated_at                | VARCHAR(20)  | NOT NULL                                        | Timestamp when the currency was last updated                               |
| updated_by                | DATETIME     | NOT NULL                                        | ID of admin who has updated the currency                                   |
``
``

## 4. Enum Fields 
#### **CoinType**
&nbsp;

      type: tinyint(1)
      field name: coin_type 

    - title: FIAT
      const: 2
    - title: CRYPTO
      const: 1
    - title: UNKNOWN
      const: 0

#### **ExchangeStatus**
&nbsp;

      type: tinyint(1)
      field name: exchange_status 

    - title: INACTIVE
      const: 2
    - title: ACTIVE
      const: 1
    - title: UNKNOWN
      const: 0

#### **DepositStatus**
&nbsp;

      type: tinyint(1)
      field name: deposit_status 

    - title: INACTIVE
      const: 2
    - title: ACTIVE
      const: 1
    - title: UNKNOWN
      const: 0

#### **WithdrawalStatus**
&nbsp;

      type: tinyint(1)
      field name: withdrawal_status 

    - title: INACTIVE
      const: 2
    - title: ACTIVE
      const: 1
    - title: UNKNOWN
      const: 0

#### **IsActive**
&nbsp;

      type: tinyint(1)
      field name: is_active 

    - title: INACTIVE
      const: 2
    - title: ACTIVE
      const: 1
    - title: UNKNOWN
      const: 0

#### **DepositFeeType**
&nbsp;

      type: tinyint(1)
      field name: deposit_fee_type 

    - title: FEE_TYPE_PERCENTAGE
      const: 2
    - title: FEE_TYPE_FIXED
      const: 1
    - title: UNKNOWN
      const: 0

#### **WithdrawalFeeType**
&nbsp;

      type: tinyint(1)
      field name: withdrawal_fee_type 

    - title: FEE_TYPE_PERCENTAGE
      const: 2
    - title: FEE_TYPE_FIXED
      const: 1
    - title: UNKNOWN
      const: 0

