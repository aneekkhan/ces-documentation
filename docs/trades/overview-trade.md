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

| Field Name    | Data Type      | Constraints                            | Description                                           |
| ------------- | -------------- | -------------------------------------- | ----------------------------------------------------- |
| id            | UUID           | DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for the trade pair                  |
| order_id      | UUID           | FOREIGN KEY                            | ID of the order associated with the trade             |
| trade_pair_id | UUID           | FOREIGN KEY                            | ID of the trade pair involved in the trade            |
| user_id       | UUID           | FOREIGN KEY                            | ID of the user who initiated the trade                |
| type          | tinyint(1)     | DEFAULT 0                              | Type of trade (e.g. buy, sell)                        |
| price         | decimal(20,10) | NOT NULL                               | Price of the traded asset                             |
| amount        | decimal(20,10) | NOT NULL                               | Amount of the traded asset                            |
| total         | decimal(20,10) | NOT NULL                               | total of the traded asset                             |
| fee           | decimal(20,10) | NOT NULL                               | Fee charged for the trade                             |
| fee_currency  | varchar(10)    | NOT NULL                               | Currency in which the fee was charged                 |
| is_maker      | tinyint(1)     | DEFAULT 0                              | Flag indicating whether the user was a maker or taker |
| created_at    | datetime       | NOT NULL                               | Timestamp of when the trade pair was created          |
| updated_at    | datetime       | NOT NULL                               | Timestamp of when the trade pair was updated          |

## 4. Enum Fields

#### **type**

&nbsp; 
 - TYPE_UNKNOWN  
 - TYPE_BUY 
 - TYPE_SELL

#### **is_maker**

&nbsp; 
 - IS_MAKER_UNKNOWN  
 - IS_MAKER_TRUE 
 - IS_MAKER_FALSE
