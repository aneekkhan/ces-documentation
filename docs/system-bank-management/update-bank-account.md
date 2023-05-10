---
sidebar_position: 4
---

# Update Bank Account

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system admin can update bank account.


## 3. API

### Update Bank Account Request Example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174111",
  "IsActive": "IS_ACTIVE_TRUE"
}
```
### Update Bank Account Response Example:

```json
{
  "ID": "123e4567-e89b-12d3-a456-426614174111",
  "UserID": "123e4567-e89b-12d3-a456-426614174000",
  "ReferenceNumber": "37421575175977",
  "BankName": "Sonali Bank",
  "AccountName": "Deposite",
  "AccountNumber": "1234567890",
  "AccountHolder": "Amit Golder",
  "RoutingNumber": "5456",
  "SWIFT": "SDFSD45",
  "IBAN":"SJ5FGSD45",
  "BIC": "WI5EUR8",
  "IsSystem": "SYSTEM",
  "CountryID": 564513164515,
  "BankAddress": "KDA 17 Khulna Bangladesh",
  "AccountHolderAddress":"Sonadanga 2nd area",
  "IsActive": "IS_ACTIVE_TRUE",
  "IsVerified": "IS_VERIFIED_FALSE",
  "UpdatedAt": "2023-05-08 09:12:15",
  "UpdatedBy": "123e4567-e89b-12d3-a456-426614174025"
}
```

## 4. Enum Fields
#### **IsSystem**
&nbsp;

	IS_SYSTEM_FALSE
	IS_SYSTEM_TRUE

#### **IsActive**
&nbsp;

	IS_ACTIVE_FALSE
	IS_ACTIVE_TRUE
	
#### **IsVerified**
&nbsp;

	IS_VERIFIED_FALSE
	IS_VERIFIED_TRUE
