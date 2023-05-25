---
sidebar_position: 1
---

# User Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

A user who wants to buy/sell cryptocurrency with fiat currency or another
cryptocurrency. They may be new to the cryptocurrency market and want to invest or trade in
various cryptocurrencies.

## 3. Data Dictionary (CES V1.0)

| Field Name        | Data Type    | Constraints                                 | Description                                                                 |
| ----------------- | ------------ | ------------------------------------------- | --------------------------------------------------------------------------- |
| id                | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY | Unique identifier for the user                                              |
| role_id           | UUID         | NOT NULL                                    | User's role id                                                              |
| first_name        | varchar(255) | NOT NULL                                    | User's first name                                                           |
| last_name         | varchar(255) | NOT NULL                                    | User's last name                                                            |
| profile_image     | varchar(255) | NOT NULL                                    | User's profile image                                                        |
| email             | varchar(255) | NOT NULL                                    | User's email address                                                        |
| phone_number      | varchar(255) | NOT NULL                                    | User's phone number                                                         |
| password          | varchar(20)  | NOT NULL                                    | Hashed user's password                                                      |
| is_phone_verified | tinyint(1)   | DEFAULT 0                                   | Flag indicating whether user's the phone number is (e.g. verified, pending) |
| is_email_verified | tinyint(1)   | NOT NULL                                    | Flag indicating whether user's the email address (e.g. verified, pending)   |
| is_mfa            | tinyint(1)   | DEFAULT 0                                   | Flag indicating whether user's mfa have or not                              |
| mfa_type          | tinyint(1)   | DEFAULT 0                                   | Flag indicating whether user's mfa_type is (e.g. verified, pending)         |
| status            | tinyint(1)   | DEFAULT 1                                   | Flag indicating whether user's status (e.g. active, inactive)               |
| kyc_level         | tinyint(1)   | DEFAULT 0                                   | Flag indicating user's kyc level(e.g. silver,gold,platinum)                 |
| created_at        | TIMESTAMP    | NOT NULL                                    | Timestamp when the user account was created                                 |
| created_by        | UUID         | NOT NULL                                    | ID of admin who has created the User                                        |
| updated_at        | TIMESTAMP    | NOT NULL                                    | Timestamp when the user account was last updated                            |
| updated_by        | UUID         | NOT NULL                                    | ID of admin who has updated the User                                        |

## 4. Enum Fields

#### **IsPhoneVerified**

&nbsp;

- IS_PHONE_VERIFIED_TRUE
- IS_PHONE_VERIFIED_FALSE

#### **IsEmailVerified**

&nbsp;

- IS_EMAIL_TRUE
- IS_EMAIL_FALSE

#### **IsMfa**

&nbsp;

- IS_MFA_TRUE
- IS_MFA_FALSE

#### \*MfaType\*\*

&nbsp;

- MFA_TYPE_UNKNOWN
- QR_CODE
- QR_CODE

#### **Status**

&nbsp;

- STATUS_ACTIVE
- STATUS_INACTIVE
- STATUS_UNKNOWN

#### **KYCLevel**

&nbsp;

- KYC_LEVEL_PLATINUM
- KYC_LEVEL_GOLD
- KYC_LEVEL_SILVER
- KYC_LEVEL_UNKNOWN
