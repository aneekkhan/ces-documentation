---
sidebar_position: 2
---

# Create Bank Account

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### In cryptocurrency exchange system bank accounts can be created two way.
##### i.  Admin can be create
##### ii. User can be create with if he/she got permission


## 3. API

### Create Bank Account Request example:

```json
{
	"ReferenceNumber": "37421575175977",
	"BankName": "Sonali Bank",
	"AccountName": "Deposite",
	"AccountNumber": "1234567890",
	"AccountHolder": "Amit Golder",
	"RoutingNumber": "5456",
	"SWIFTCODE": "SDFSD45",
	"IBAN":"SJ5FGSD45",
	"BIC": "WI5EUR8",
	"IsSystem": "FALSE",
	"CountryCode": "BD",
	"BankAddress": "KDA 17 Khulna Bangladesh",
	"AccountHolderAddress":"Sonadanga 2nd area",
	"IsActive": "FALSE"
}
```

### Create Bank Account Response example:

```json
{
  "Data": {
    "BankAccount": {
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
			"IsSystem": "FALSE",
			"CountryCode": "BD",
			"BankAddress": "KDA 17 Khulna Bangladesh",
			"AccountHolderAddress":"Sonadanga 2nd area",
			"IsActive": "FALSE",
			"IsVerified": "FALSE",
			"CreatedAt": "2023-05-08 09:12:15",
			"UpdatedAt": "2023-05-08 09:12:15",
			"CreatedBy": "123e4567-e89b-12d3-a456-426614174025",
			"UpdatedBy": "123e4567-e89b-12d3-a456-426614174025"
    }
  }
}
```

