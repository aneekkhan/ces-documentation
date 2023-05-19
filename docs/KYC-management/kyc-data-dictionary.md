---
sidebar_position: 1
---

# KYC Overview

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

KYC procedures typically involve collecting personal information, such as a user's name, address, and government-issued ID, and verifying this information through various means, such as online databases and third-party verification services.

## 3. Data Dictionary (CES V1.0)

| Field Name                | Data Type    | Constraints                                     | Description                                                                                               |
| ------------------------- | ------------ | ----------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| id                        | UUID         | UUID DEFAULT uuid_generate_v4() PRIMARY KEY     | Unique identifier for the Key verification request                                                        |
| user_id                   | NOT NULL     | NOT NULL                                     | ID of the user requesting verification                                                                    |
| status                    | tinyint(1)   | DEFAULT 0                                       | Status of the verification request (e.g. pending,approved,rejected)                                       |
| document_type             | tinyint(1)   | DEFAULT 0                                       | Type of document being submitted for verification (e.g. passport, driver's license, ID card)              |
| document_number           | VARCHAR(50)  | NOT NULL                                        | Document number being submitted for verification                                                          |
| document_photo            | text array   | NOT NULL                                        | URL or file path of the photo of the document being submitted                                             |
| selfie_with_document      | text array   | NOT NULL                                        | URL or file path of the selfie photo of the user holding the document and a paper with verification code  |
| submitted_at              | DATETIME     | NOT NULL                                        | Timestamp of when the verification request was submitted                                                  |
| approved_at               | DATETIME     | NOT NULL                                        |Timestamp when the verification request has been approved                                                  |
| approved_by               | varchar(50)  | NOT NULL                                     | ID of the admin who approved the verification request                                                     |
| rejected_at               | DATETIME     | NOT NULL                                        | Timestamp when the verification request has been rejected                                                 |
| rejected_by               | varchar(50)  | NOT NULL                                    | ID of the admin who rejected the verification request                                                     |
| rejection_reason          | VARCHAR(255) | NOT NULL                                        | Reason for rejection of the verification request                                                          |



## 4. Enum Fields 
#### **Status**
&nbsp;

      type: tinyint(1)

    - STATUS_PENDING
    - STATUS_APPROVED
    - STATUS_REJECTED

#### **DocumentType**
&nbsp;

      type: tinyint(1)

    - DOCUMENT_TYPE_UNKNOWN
    - DOCUMENT_TYPE_ID_CARD
    - DOCUMENT_TYPE_DRIVER_LICENSE
    - DOCUMENT_TYPE_PASSPORT

