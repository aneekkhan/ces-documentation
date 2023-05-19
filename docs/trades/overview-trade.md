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
| trade_pair_id       | UUID           | FOREIGN KEY                            | ID of the trade pair involved in the trade           |
| user_id             | varchar(50)    | NOT NULL                               | ID of the user who initiated the trade               |
| maker_id            | varchar(50)    | NOT NULL                               | ID of the user associated with the maker             |
| amount              | BIGINT         | NOT NULL                               | Amount of the traded asset                           |
| price               | BIGINT         | NOT NULL                               | Price of the traded asset                            |
| total               | BIGINT         | NOT NULL                               | total of the traded asset                            |
| buy_id              | UUID           | FOREIGN KEY                            | ID of the crypto that is bought                      |
| buy_order_id        | UUID           | FOREIGN KEY                            | ID of the order by which the buyer sell the crypto   |
| buyer_id            | varchar(50)    | NOT NULL                               | ID of the user who bought the crypto                 |
| buyer_fee           | BIGINT         | NOT NULL                               | Fee charged for the trade buyer                      |
| buyer_fee_currency  | UUID           | FOREIGN KEY                            | Fee Currency in which the buyer was charged          |
| sell_id             | UUID           | FOREIGN KEY                            | ID of the crypto that is sold                        |
| sell_order_id       | UUID           | FOREIGN KEY                            | ID of the order by which the seller sell the crypto  |
| seller_id           | varchar(50)    | NOT NULL                               | ID of the user who sold the crypto                   |
| seller_fee          | BIGINT         | NOT NULL                               | Fee charged for the trade seller                     |
| seller_fee_currency | UUID           | FOREIGN KEY                            | Fee Currency in which the seller was charged         |
| taker_fee           | BIGINT         | NOT NULL                               | Fee charged for the trade taker                      |
| taker_fee_type      | tinyint(1)     | NOT NULL                               | taker_fee_type of the trades (e.g. FIXED PERCENTAGE) |
| maker_fee           | BIGINT         | NOT NULL                               | Fee charged for the trade maker                      |
| maker_fee_type      | tinyint(1)     | NOT NULL                               | maker_fee_type of the trades (e.g. FIXED PERCENTAGE) |
| created_at          | datetime       | NOT NULL                               | Timestamp of when the trade pair was created         |
| updated_at          | datetime       | NOT NULL                               | Timestamp of when the trade pair was updated         |

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
