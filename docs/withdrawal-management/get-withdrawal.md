---
sidebar_position: 2
---

# Get Withdrawal

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can get Withdrawal details by ID.

## 3. API

### Get Withdrawal by ID Request example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174000"
}
```

### Get Withdrawal by ID Response example:

```json
{
  "Data": {
    "Withdrawals": {
      "ID": "123e4567-e89b-12d3-a456-426614174111",
      "UserID": "123e4567-e89b-12d3-a456-426614174000",
      "UserEmail": "mail@mail.com",
      "CurrencySymbol": "BTC",
      "CurrencyName": "United States Dollar",
      "WithdrawalStatus": "WITHDRAWAL_STATUS_UNKNOWN",
      "Amount": 0.72934774,
      "NetAmount": 643.23359243,
      "FeeType": "FEE_TYPE_FLAT",
      "FeeAmount": 0.01458695,
      "WithdrawalMethod": "WITHDRAWAL_METHOD_BANK_TRANSFER",
      "WithdrawalAccount": "1234567890",
      "WithdrawalNote": "withdrawal_note",
      "PaymentGateway": "PAYMENT_GATEWAY_PAYPAL",
      "TransactionId": "SDFSD45GDKJDDJKGD",
      "WithdrawalDate": "2023-05-08 09:12:15",
      "ProcessedDate": "2023-05-08 09:12:15",
      "CreatedAt": "2023-05-08 09:12:15",
      "UpdatedAt": "2023-05-08 09:12:15",
      "CreatedBy": "123e4567-e89b-12d3-a456-426614174025",
      "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025"
    }
  }
}
```

## 4. Enum Fields

#### **WithdrawalStatus**

&nbsp;

    WITHDRAWAL_STATUS_UNKNOWN
    WITHDRAWAL_STATUS_PENDING
    WITHDRAWAL_STATUS_COMPLETED
    WITHDRAWAL_STATUS_PROCESSING
    WITHDRAWAL_STATUS_CANCELED

#### **FeeType**

&nbsp;

    FEE_TYPE_UNKNOWN
    FEE_TYPE_FLAT
    FEE_TYPE_PERCENTAGE

#### **WithdrawalMethod**

&nbsp;

    WITHDRAWAL_METHOD_UNKNOWN
    WITHDRAWAL_METHOD_BANK_TRANSFER
    WITHDRAWAL_METHOD_PAYPAL
    WITHDRAWAL_METHOD_STRIPE
    WITHDRAWAL_METHOD_WE_PAY

#### **PaymentGateway**

&nbsp;

    PAYMENT_GATEWAY_UNKNOWN
    PAYMENT_GATEWAY_PAYPAL
    PAYMENT_GATEWAY_STRIPE
    PAYMENT_GATEWAY_WE_PAY

