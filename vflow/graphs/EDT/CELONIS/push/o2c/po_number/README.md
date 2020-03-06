# CELONIS PO NUMBER
EDT.CELONIS.push.o2c.po_number


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   29.10.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   29.10.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   28.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads order information from ERP and stores it in Celonis from the past 2 years up to today.


## Source

### System
ISP_DIP

### Schema
SAPISP

### Tables
- VBKD
- CDHSD
- CDPOS

### Fields
- udate
- utime
- vbeln
- bstkd


## Target

### Primary Key
ORDER_ID

### Table
PO_NUMBER

### Fields
- PO_UPDATE_DATE
- PO_UPDATE_TIME
- ORDER_ID
- PO_NUMBER