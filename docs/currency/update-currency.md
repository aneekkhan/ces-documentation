---
sidebar_position: 4
---

# Update Currency

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system coin/currency can Update currency.


## 3. API

### Update Coin/Cuerrncy Request example:

```json
{
   "ID":"123e4567-e89b-12d3-a456-426614174000",
   "Icon":"btcsssss.png",
   "ExchangeStatus":"ACTIVE",
   "DepositStatus":"ACTIVE",
   "WithdrawalStatus":"ACTIVE",
   "IsActive":"ACTIVE",
   "DepositFee":"10",
   "TotalDeposit":"0",
   "DepositFeeType":"DEPOSIT_FEE_TYPE_FIXED",
   "MinimumDepositAmount":"0",
   "MaximumDepositAmount":"1000",
   "DailyDepositLimit":"10000",
   "WithdrawalFee":"10",
   "TotalWithdrawal":"0",
   "WithdrawalFeeType":"WITHDRAWAL_FEE_TYPE_FIXED",
   "MinimumWithdrawalAmount":"0",
   "MaximumWithdrawalAmount":"1000",
   "DailyWithdrawalLimit":"10000",
}
```

### Get Coin/Cuerrncy Response example:

```json
{
   "Data":{
      "Currency":{
         "ID":"123e4567-e89b-12d3-a456-426614174000",
         "Name":"Bitcoin",
         "CoinType":"CRYPTO",
         "Symbol":"BTC",
         "Icon":"btc.png",
         "Decimals":0,
         "ExchangeStatus":"ACTIVE",
         "DepositStatus":"ACTIVE",
         "WithdrawalStatus":"ACTIVE",
         "IsActive":"ACTIVE",
         "DepositFee":"10",
         "TotalDeposit":"0",
         "DepositFeeType":"FEE_TYPE_FIXED",
         "MinimumDepositAmount":"0",
         "MaximumDepositAmount":"1000",
         "DailyDepositLimit":"10000",
         "WithdrawalFee":"10",
         "TotalWithdrawal":"0",
         "WithdrawalFeeType":"FEE_TYPE_FIXED",
         "MinimumWithdrawalAmount":"0",
         "MaximumWithdrawalAmount":"1000",
         "DailyWithdrawalLimit":"10000",
         "CreatedAt":"2020-03-24T06:03:00.348+03:00",
         "CreatedBy":"456e4567-e89b-12d3-a456-426614174000",
         "UpdatedAt":"2020-03-24T06:03:00.348+03:00",
         "UpdatedBy":"456e4567-e89b-12d3-a456-426614174000"
      }
   }
}
```