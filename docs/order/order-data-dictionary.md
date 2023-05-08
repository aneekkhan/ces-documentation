---
sidebar_position: 1
---

# Order Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

Crypto exchange platforms typically offer different types of orders, such as market orders, limit orders, and stop-loss orders, which allow users to specify the price and timing of their trades.

## 3. Data Dictionary (CES V1.0)

| Field Name                | Data Type    | Constraints                                     | Description                                                                |
| ------------------------- | ------------ | ----------------------------------------------- | -------------------------------------------------------------------------- |
| id                        | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY     | Unique identifier for order                                                |
| user_id                   | UUID         | FOREIGN KEY                                     | ID of the user who placed the order                                        |
| trade_pair_id             | UUID         | FOREIGN KEY                                     | ID od the trade pair associated with the order                             |
| category                  | tinyint(1)   | DEFAULT 0                                       | Category of order(market,limit or stop-loss)                               |
| type                      | tinyint(1)   | DEFAULT 0                                       | Type of order(buy or sell)                                                 |
| status                    | tinyint(1)   | DEFAULT 0                                       | Status of the order (e.g.open, completed, cancelled)                       |
| quantity                  | VARCHAR(50)  | NOT NULL                                        | Quantity of base currency in the order                                     |
| price                     | VARCHAR(50)  | NOT NULL                                        | Price per unit of the quote currency in the order                          |
| stop_limit                | VARCHAR(50)  | NOT NULL                                        | Stop limit price per unit of the quote currency in the order               |
| total                     | VARCHAR(50)  | NOT NULL                                        | Total value of the order(quantity * price)                                 |
| fee_type                  | tinyint(1)   | DEFAULT 0                                       | Type of fee charged for the order (e.g. maker,taker)                       |
| fee_amount                | VARCHAR(50)  | NOT NULL                                        | Amount of fee charged forthe order                                         |
| fee_currency_id           | UUID         | FOREIGN KEY                                     | ID of the currency used to pay the fee                                     |
| executed_quantity         | VARCHAR(50)  | NOT NULL                                        | Quantity of base currency executed in the order                            |
| executed_total            | VARCHAR(50)  | NOT NULL                                        | Total value of executed orders (quantity * price)                          |
| created_at                | DATETIME     | NOT NULL                                        | Timestamp when the order was placed                                        |
| created_by                | UUID         | NOT NULL                                        | ID of user who has added the currency                                      |
| updated_at                | DATETIME     | NOT NULL                                        | Timestamp when the order was last updated                                  |
| cancelled_at              | DATETIME     | NOT NULL                                        | Timestamp when the order was cancelled                                     |
| updated_by                | UUID         | NOT NULL                                        | ID of user who has updated the order                                       |
``
``

## 4. Enum Fields 
#### **Category**
&nbsp;

      type: tinyint(1)

    - CATEGORY_MARKET
    - CATEGORY_LIMIT
    - CATEGORY_STOP_LOSS
    - CATEGORY_UNKNOWN

#### **Type**
&nbsp;

      type: tinyint(1)

    - TYPE_BUY
    - TYPE_SELL
    - TYPE_UNKNOWN

#### **Status**
&nbsp;

      type: tinyint(1)

    - STATUS_OPEN
    - STATUS_COMPLETED
    - STATUS_CANCELLED
    - STATUS_UNKNOWN

#### **FeeType**
&nbsp;

      type: tinyint(1)

    - FEE_TYPE_MAKER
    - FEE_TYPE_TAKER
    - FEE_TYPE_UNKNOWN

