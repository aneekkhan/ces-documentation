---
sidebar_position: 2
---

# Create Trades

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
  "TradePairID": "52ad9477-1f35-48fd-a3b0-80b853defdd3",
  "UserID": "12d3-e89b-12d3-a456-426614174000",
  "MakerID": "12d3-e89b-12d3-a456-426614174000",
  "Amount": "2000",
  "Price": "2000",
  "Total": "4000",
  "BuyID": "559d9101-3c27-450c-8765-66b8ee9692df",
  "BuyOrderID": "13cf59cd-5890-4502-a99d-e02f7b66b515",
  "BuyerID": "12d3-e89b-12d3-a456-426614174000",
  "BuyerFee": "100",
  "BuyerFeeCurrency": "559d9101-3c27-450c-8765-66b8ee9692df",
  "SellID": "559d9101-3c27-450c-8765-66b8ee9692df",
  "SellOrderID": "13cf59cd-5890-4502-a99d-e02f7b66b515",
  "SellerID": "12d3-e89b-12d3-a456-426614174000",
  "SellerFee": "234",
  "SellerFeeCurrency": "559d9101-3c27-450c-8765-66b8ee9692df",
  "TakerFee": "234",
  "TakerFeetype": "UNKNOWN",
  "MakerFee": "23",
  "MakerFeetype": "UNKNOWN"
}
```

### Response example:

```json
{
  "Data": {
    "Trades": {
      "ID": "123e4567-e89b-12d3-a456-426614174000",
      "TradePairID": "52ad9477-1f35-48fd-a3b0-80b853defdd3",
      "UserID": "12d3-e89b-12d3-a456-426614174000",
      "MakerID": "12d3-e89b-12d3-a456-426614174000",
      "Amount": "2000",
      "Price": "2000",
      "Total": "4000",
      "BuyID": "559d9101-3c27-450c-8765-66b8ee9692df",
      "BuyOrderID": "13cf59cd-5890-4502-a99d-e02f7b66b515",
      "BuyerID": "12d3-e89b-12d3-a456-426614174000",
      "BuyerFee": "100",
      "BuyerFeeCurrency": "559d9101-3c27-450c-8765-66b8ee9692df",
      "SellID": "559d9101-3c27-450c-8765-66b8ee9692df",
      "SellOrderID": "13cf59cd-5890-4502-a99d-e02f7b66b515",
      "SellerID": "12d3-e89b-12d3-a456-426614174000",
      "SellerFee": "234",
      "SellerFeeCurrency": "559d9101-3c27-450c-8765-66b8ee9692df",
      "TakerFee": "234",
      "TakerFeetype": "UNKNOWN",
      "MakerFee": "23",
      "MakerFeetype": "UNKNOWN",
      "CreatedAt": "12-12-2021 12:12:12",
      "UpdatedAt": "2020-03-24T06:03:00.348+03:00"
    }
  }
}
```
