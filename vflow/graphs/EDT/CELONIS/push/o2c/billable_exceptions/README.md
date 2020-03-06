# CELONIS BILLABLE EXCEPTIONS
EDT.CELONIS.push.o2c.billable_exceptions

## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   08.09.2019  |   1.0.0   |   C5215227    |   Implemented, tested and documented workflow. |
|   17.10.2019  |   2.1.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.2 and retested.    |
|   17.10.2019  |   2.1.1   |   C5215227    |   ITSXCEL-269.    |
|   17.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   17.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   27.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads contract information from ERP and stores it in Celonis from the past 2 years up to today.

## Source

### System
ISP_DIP

### Schema
ISPSAP

### Tables
- /1FE/0Z1003IT
- /1FE/0Z1013IT
- /1FE/0Z3003IT

### Fields
- BITCRDATE
- BITCRTIME
- VTREF
- VTPOS

## Target
### Primary Key
CONTRACT_ID

### Table
BILLABLE_EXCEPTIONS

### Fields
- CREATED_ON
- CREATED_AT
- CONTRACT_ID
- CONTRACT_ITEM_NUMBER