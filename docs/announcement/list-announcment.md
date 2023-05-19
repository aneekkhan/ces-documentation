---
sidebar_position: 4
---

# List Announcement

## 1. version control

| Version  | Date        | Description of Changes |
| -------- | ----------- | ---------------------- |
| CES V1.0 | May 3, 2023 | Initial Release        |

## 2. Overview

#### Announcement is a message posted in the announcement section of the website. It is used to inform users about the latest news, updates, and other important information.

## 3. API

### Request example:

```json
{
  "SortBy": "DESC",
  "SearchTerm": "B",
  "IsActive": "TRUE",
  "AnnouncmentType":"WARNING",
  "SortByColumn": "name",
  "StartDate": "2020-03-24T06:03:00.348+03:00",
  "EndDate": ""
}
```

### Response example:

```json
{
  "Data": {
    "Announcment": [
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "AuthorId": "123e4567-e89b-12d3-a456-426614174000",
        "Title": "vacation",
        "Content": "i will be on vacation for 2 weeks",
        "IsActive": "Active",
        "Type": "INFO",
        "StartDate": "2021-10-10 12:00:00",
        "EndDate": "2021-10-10 12:00:00",
        "CreatedAt": "2021-10-10 12:00:00",
        "UpdatedAt": "2021-10-10 12:00:00"
      },
      {
        "ID": "123e4567-e89b-12d3-a456-426614174000",
        "AuthorId": "123e4567-e89b-12d3-a456-426614174000",
        "Title": "vacation",
        "Content": "i will be on vacation for 2 weeks",
        "IsActive": "Active",
        "Type": "INFO",
        "StartDate": "2021-10-10 12:00:00",
        "EndDate": "2021-10-10 12:00:00",
        "CreatedAt": "2021-10-10 12:00:00",
        "UpdatedAt": "2021-10-10 12:00:00"
      }
    ]
  },
  "Total": 2
}
```
