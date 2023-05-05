---
sidebar_position: 1
---

# Support Ticket Overview

## 1. Version control

| Version     | Date        | Description of Changes      |
| ----------- | ----------- | --------------------------- |
| CES V1.0    | May 3, 2023 | Initial Release             |


## 2. Overview

customer supporting system by ticketing.

## 3. Data Dictionary

| Field Name           | Data Type    | Constraints                          | Description                                          |
| ------------------   | ------------ | ------------------------------------ | ---------------------------------------------------- |
| id                   | UUID         | PRIMARY KEY, AUTO_INCREMENT, NOT NULL| Unique identifier for the support ticket             |
| user_id              | UUID         | FOREIGN KEY                          | ID of the user who created the Key support ticket    |
| support_type         | varchar(20)  |                        | Type of support request (e.g. technical, billing, general inquiry) |
| subject              | varchar(20)  |                                      | Subject of the support request                       |
| message              | text         |                                      | Body of the support request message                  |
| attachment           | varchar(255) |                                | Path to any attached file(s) related to the support request|
| status               | varchar(20)  |                     | Current status of the support request (e.g. open, closed, pending)    |
| priority             | varchar(20)  |                         | Priority level of the support request (e.g. high, medium, low)    |
| created_at           | datetime     |                                      | Timestamp of when the support ticket was created     |
| updated_at           | datetime     |                                      | Timestamp of when the support ticket was updated     |
| resolved_at          | datetime     |                                      | Timestamp of when the support ticket was resolved    |
| assigned_to          | UUID         |                                      | ID of the admin who is assigned support ticket       |
| created_by           | VARCHAR(100) |                                      | ID of the admin who is assigned support ticket       |
| updated_by           | VARCHAR(100) |                                      | ID of the admin who is assigned support ticket       |
