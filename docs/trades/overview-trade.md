---
sidebar_position: 1
---

# Trades Overview

## 1. Version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

A crypto exchange system is a platform that allows users to buy, sell, and trade cryptocurrencies such as Bitcoin, Ethereum, and others. Trading on a crypto exchange system involves buying or selling cryptocurrencies at a particular price based on the demand and supply of the currency.

## 3. Data Dictionary (CES V1.0)

| Field Name          | Data Type      | Constraints                            | Description                                          |
| ------------------- | -------------- | -------------------------------------- | ---------------------------------------------------- |
| id                  | UUID           | DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for the trade pair                 |
| order_id            | UUID           | FOREIGN KEY                            | ID of the order associated with the trade            |
| trade_pair_id       | UUID           | FOREIGN KEY                            | ID of the trade pair involved in the trade           |
| user_id             | UUID           | FOREIGN KEY                            | ID of the user who initiated the trade               |
| price               | decimal(20,10) | NOT NULL                               | Price of the traded asset                            |
| amount              | decimal(20,10) | NOT NULL                               | Amount of the traded asset                           |
| total               | decimal(20,10) | NOT NULL                               | total of the traded asset                            |
| maker_id            | UUID           | FOREIGN KEY                            | ID of the user associated with the maker             |
| created_at          | datetime       | NOT NULL                               | Timestamp of when the trade pair was created         |
| updated_at          | datetime       | NOT NULL                               | Timestamp of when the trade pair was updated         |
| buy_id              | UUID           | FOREIGN KEY                            | ID of the crypto that is bought                      |
| sell_id             | UUID           | FOREIGN KEY                            | ID of the crypto that is sold                        |
| buyer_id            | UUID           | FOREIGN KEY                            | ID of the user who bought the crypto                 |
| seller_id           | UUID           | FOREIGN KEY                            | ID of the user who sold the crypto                   |
| sell_order_id       | UUID           | FOREIGN KEY                            | ID of the order by which the seller sell the crypto  |
| buy_order_id        | UUID           | FOREIGN KEY                            | ID of the order by which the buyer sell the crypto   |
| taker_fee           | decimal(20,10) | NOT NULL                               | Fee charged for the trade taker                      |
| maker_fee           | decimal(20,10) | NOT NULL                               | Fee charged for the trade maker                      |
| taker_fee_type      | tinyint(1)     | NOT NULL                               | taker_fee_type of the trades (e.g. FIXED PERCENTAGE) |
| maker_fee_type      | tinyint(1)     | NOT NULL                               | maker_fee_type of the trades (e.g. FIXED PERCENTAGE) |
| buyer_fee_currency  | varchar(10)    | NOT NULL                               | Fee Currency in which the buyer was charged          |
| seller_fee_currency | varchar(10)    | NOT NULL                               | Fee Currency in which the seller was charged         |

## 4. Enum Fields

#### **TakerFeeType**

&nbsp;

- TAKER_FEE_TYPE_UNKNOWN
- TAKER_FEE_TYPE_FIXED
- TAKER_FEE_TYPE_PERCENTAGE

#### **MakerFeeType**

&nbsp;

- MAKER_FEE_TYPE_UNKNOWN
- MAKER_FEE_TYPE_FIXED
- MAKER_FEE_TYPE_PERCENTAGE
