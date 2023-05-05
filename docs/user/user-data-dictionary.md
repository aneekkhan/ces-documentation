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

| Field Name                | Data Type                                   | Constraints | Description                                                                       |
| ------------------------- | ------------------------------------------- | ----------- | --------------------------------------------------------------------------------- |
| id                        | UUID DEFAULT uuid_generate_v4() PRIMARY KEY |             | Unique identifier for the user                                                    |
| role_id                   | UUID                                        | NOT NULL    | User's role id                                                                    |
| first_name                | varchar(255)                                | NOT NULL    | User's first name                                                                 |
| last_name                 | varchar(255)                                | NOT NULL    | User's last name                                                                  |
| email                     | varchar(255)                                | NOT NULL    | User's email address                                                              |
| phone_number              | varchar(255)                                | NOT NULL    | User's phone number                                                               |
| password                  | varchar(20)                                 | NOT NULL    | Hashed user's password                                                            |
| is_email_verified         | tinyint(1)                                  | NOT NULL    | Flag indicating whether user's the email address (e.g. verified, pending)         |
| status                    | tinyint(1)                                  | DEFAULT 1   | Flag indicating whether user's status (e.g. active, inactive)                     |
| account_status            | tinyint(1)                                  | DEFAULT 0   | Flag indicating whether user's account status (e.g. active, suspended or deleted) |
| financial_status          | tinyint(1)                                  | DEFAULT 1   | Flag indicating whether user's financial status (e.g. Active, Inactive)           |
| maintenance_access_status | tinyint(1)                                  | DEFAULT 1   | Flag indicating whether user's maintenance access status (e.g. Enable, Disable)   |
| is_phone_verified         | tinyint(1)                                  | DEFAULT 0   | Flag indicating whether user's the phone number is (e.g. verified, pending)       |
| is_mfa                    | tinyint(1)                                  | DEFAULT 0   | Flag indicating whether user's mfa have or not                                    |
| mfa_type                  | tinyint(1)                                  | DEFAULT 0   | Flag indicating whether user's mfa_type is (e.g. verified, pending)               |
| created_at                | TIMESTAMP                                   | NOT NULL    | Timestamp when the user account was created                                       |
| created_by                | varchar(255)                                | NOT NULL    | User created                                                                      |
| updated_at                | TIMESTAMP                                   | NOT NULL    | Timestamp when the user account was last updated                                  |
| updated_by                | varchar(255)                                | NOT NULL    | User updated                                                                      |

`
`
## 4. Enum Fields 

#### **is_email_verified**
&nbsp;
    - IS_EMAIL_FALSE
    - IS_EMAIL_TRUE

#### **status**
&nbsp;
    - STATUS_UNKNOWN  
    - STATUS_ACTIVE
    - STATUS_INACTIVE

#### **account_status**
&nbsp;
    - ACCOUNT_STATUS_UNKNOWN  
    - ACCOUNT_STATUS_ACTIVE
    - ACCOUNT_STATUS_SUSPENDED
    - ACCOUNT_STATUS_DELETED 

#### **financial_status**
&nbsp;
    - FINANCIAL_STATUS_UNKNOWN  
    - FINANCIAL_STATUS_ACTIVE
    - FINANCIAL_STATUS_INACTIVE


#### **maintenance_access_status**
&nbsp;
    - MAINTENANCE_ACCESS_STATUS_UNKNOWN  
    - MAINTENANCE_ACCESS_STATUS_ENABLE
    - MAINTENANCE_ACCESS_STATUS_DISABLE


#### **is_phone_verified**
&nbsp;
    - IS_PHONE_VERIFIED_FALSE
    - IS_PHONE_VERIFIED_TRUE


#### **is_mfa**
&nbsp;
    - IS_MFA_TRUE
    - IS_MFA_FALSE

#### **mfa_type**
&nbsp;
    - MFA_TYPE_PASS  
    - MFA_TYPE_TOTP
    - MFA_TYPE_CODE
    - MFA_TYPE_SMS 
    - MFA_TYPE_RECOVERY
    - MFA_TYPE_EMAIL


