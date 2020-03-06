# CELONIS BILLING DATE
EDT.CELONIS.push.o2c.billing_date


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   17.10.2019  |   2.1.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.2 and retested.    |
|   17.10.2019  |   2.1.1   |   C5215227    |   Documented workflow.    |
|   28.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   28.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads billing date information from ERP and stores it in Celonis from the past 2 years up to today.


## Source

### System
ISP_DIP

### Schema
SAPISP

### Tables
- VBAK
- VBKD
- FPLT


### Fields
- afdat
- vbeln


## Target

### Primary Key
none

### Table
BILLING_DATE

### Fields
- PLANNED_BILLING_DATE
- ORDER_ID