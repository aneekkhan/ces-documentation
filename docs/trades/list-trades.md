---
sidebar_position: 4
---

# List Trade

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

A crypto exchange system is a platform that allows users to buy, sell, and trade cryptocurrencies such as Bitcoin, Ethereum, and others. Trading on a crypto exchange system involves buying or selling cryptocurrencies at a particular price based on the demand and supply of the currency.

## 3. API

### Request example:

```json
{
  "SortBy": "123e4567-e89b-12d3-a456-426614174000",
  "SortByColumn": "John",
  "Status": "Smith",
  "Limit": "mail@mail.com",
  "Offset": "1234567890",
  "SearchTerm": "password",
  "StartDate": "Active",
  "EndDate": "Active"
}
```

### Response example:

```json
{
  "Data": {
    "Trades": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "TradePairId": "426614174000-e89b-12d3-a456-426614174000",
        "UserId": "12d3-e89b-12d3-a456-426614174000",
        "MakerID": "12d3-e89b-12d3-a456-426614174000",
        "Amount": 2000,
        "Price": 2000,
        "Total": 4029.96,
        "BuyId": "12d3-e89b-12d3-a456-426614174000",
        "BuyOrderId": "12d3-e89b-12d3-a456-426614174000",
        "BuyerId": "12d3-e89b-12d3-a456-426614174000",
        "BuyerFee": 100.25,
        "BuyerFeeCurrency": "USD",
        "SellId": "12d3-e89b-12d3-a456-426614174000",
        "SellOrderId": "12d3-e89b-12d3-a456-426614174000",
        "SellerId": "12d3-e89b-12d3-a456-426614174000",
        "SellerFee": 100.25,
        "SellerFeeCurrency": "USD",
        "TakerFee": 124.98,
        "TakerFeetype": "UNKNOWN",
        "MakerFee": 100.25,
        "MakerFeetype": "UNKNOWN",
        "CreatedAt": "12-12-2021 12:12:12",
        "UpdatedAt": "2020-03-24T06:03:00.348+03:00"
      },
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "TradePairId": "426614174000-e89b-12d3-a456-426614174000",
        "UserId": "12d3-e89b-12d3-a456-426614174000",
        "MakerID": "12d3-e89b-12d3-a456-426614174000",
        "Amount": 2000,
        "Price": 2000,
        "Total": 4029.96,
        "BuyId": "12d3-e89b-12d3-a456-426614174000",
        "BuyOrderId": "12d3-e89b-12d3-a456-426614174000",
        "BuyerId": "12d3-e89b-12d3-a456-426614174000",
        "BuyerFee": 100.25,
        "BuyerFeeCurrency": "USD",
        "SellId": "12d3-e89b-12d3-a456-426614174000",
        "SellOrderId": "12d3-e89b-12d3-a456-426614174000",
        "SellerId": "12d3-e89b-12d3-a456-426614174000",
        "SellerFee": 100.25,
        "SellerFeeCurrency": "USD",
        "TakerFee": 124.98,
        "TakerFeetype": "UNKNOWN",
        "MakerFee": 100.25,
        "MakerFeetype": "UNKNOWN",
        "CreatedAt": "12-12-2021 12:12:12",
        "UpdatedAt": "2020-03-24T06:03:00.348+03:00"
      }
    ],
    "TotalTrades": 2
  }
}
```
