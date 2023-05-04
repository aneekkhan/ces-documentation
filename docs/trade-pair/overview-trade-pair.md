---
sidebar_position: 1
---

# Trade Pair Overview

## 1. Version control

| Version     | Date        | Description of Changes      |
| ----------- | ----------- | --------------------------- |
| CES V1.0    | May 3, 2023 | Initial Release             |


## 2. Overview

Cryptocurrencies can be traded against other cryptocurrencies or against fiat
currencies, depending on the trading pairs offered by the platform.

## 3. Data Dictionary

| Field Name           | Data Type    | Constraints                          | Description                                          |
| ------------------   | ------------ | ------------------------------------ | ---------------------------------------------------- |
| id                   | UUID         | PRIMARY KEY, AUTO_INCREMENT, NOT NULL| Unique identifier for the trade pair                 |
| name                 | varchar(50)  |                                      | Name of the trade pair                               |
| base_currency_id     | int          | FOREIGN KEY                          | Identifier for the base currency                     |
| quote_currency_id    | int          | FOREIGN KEY                          | Identifier for the quote currency                    |
| price_decimal_places | int          |                                      | Number of decimal places for the price of trade pair |
| minimum_order_amount | decimal(18,8)|                                      | Minimum amount allowed for an order                  |
| last_price           | decimal(18,8)|                                      | Last price for the trade pair                        |
| is_active            | boolean      |                                      | Flag indicating whether the trade pair is active     |
| is_default           | boolean      |                                      | Flag indicating whether the trade pair is default    |
| created_at           | datetime     |                                      | Timestamp of when the trade pair was created         |
| updated_at           | datetime     |                                      | Timestamp of when the trade pair was updated         |
| deleted_at           | datetime     |                                      | Timestamp of when the trade pair was deleted         |
| maker_fee            | decimal(5,2) |                 | Fee charged orders that for add liquidity to the order book (maker orders)|
| taker_fee            | decimal(5,2) |                 | Fee charged orders that for add liquidity to the order book (taker orders)|
