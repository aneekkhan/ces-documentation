---
sidebar_position: 1
---

# Create User

## 1. version control

| Version     | Date        | Description of Changes      |
| ----------- | ----------- | --------------------------- |
| CES V1.0    | May 3, 2023 | Initial Release             |


## 2. Overview

A user who wants to buy/sell cryptocurrency with fiat currency or another
cryptocurrency. They may be new to the cryptocurrency market and want to invest or trade in
various cryptocurrencies.

## 3. Data Dictionary

| Field Name     | Data Type        | Constraints                          | Description                    |
| -------------- | ---------------- | ------------------------------------ | ------------------------------ |
| id             | UUID             | PRIMARY KEY, AUTO_INCREMENT, NOT NULL| Unique identifier for the user |


## 4. API

### Request example:

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "email": "mail@mail.com",
  "phone": "1234567890",
  "password": "password",
}
```
### Response example:

```json
{
  "id": "123e4567-e89b-12d3-a456-426614174000",
}
```