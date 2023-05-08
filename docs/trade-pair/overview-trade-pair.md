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
| id                   | UUID        | DEFAULT uuid_generate_v4() PRIMARY KEY| Unique identifier for the trade pair                 |
| name                 | varchar(50)  | NOT NULL                             | Name of the trade pair                               |
| base_currency_id     | int          | FOREIGN KEY                          | Identifier for the base currency                     |
| quote_currency_id    | int          | FOREIGN KEY                          | Identifier for the quote currency                    |
| price_decimal_places | int          | NOT NULL                             | Number of decimal places for the price of trade pair |
| minimum_order_amount | decimal(18,8)| NOT NULL                             | Minimum amount allowed for an order                  |
| last_price           | decimal(18,8)| NOT NULL                             | Last price for the trade pair                        |
| is_active            | tinyint(1)   | DEFAULT 0                            | Flag indicating whether the trade pair is active     |
| is_default           | tinyint(1)   | DEFAULT 0                            | Flag indicating whether the trade pair is default    |
| created_at           | datetime     | NOT NULL                             | Timestamp of when the trade pair was created         |
| updated_at           | datetime     | NOT NULL                             | Timestamp of when the trade pair was updated         |
| deleted_at           | datetime     | NOT NULL                             | Timestamp of when the trade pair was deleted         |
| maker_fee            | decimal(5,2) | NOT NULL        | Fee charged orders that for add liquidity to the order book (maker orders)|
| taker_fee            | decimal(5,2) | NOT NULL        | Fee charged orders that for add liquidity to the order book (taker orders)|

## 4. Enum fields

#### **IsActive**


      type: tinyint(1)
      field name: is_active 

    - title: INACTIVE
      const: 2
    - title: ACTIVE
      const: 1
    - title: UNKNOWN
      const: 0
    

#### **IsDefault**


      type: tinyint(1)
      field name: is_default 

    - title: IS_NOT_DEFAULT
      const: 2
    - title: IS_DEFAULT
      const: 1
    - title: UNKNOWN
      const: 0