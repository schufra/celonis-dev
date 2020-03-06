# CELONIS BILLABLE ITEM
EDT.CELONIS.push.o2c.billable_item


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   17.10.2019  |   2.1.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.2 and retested.    |
|   17.10.2019  |   2.1.1   |   C5215227    |   Documented workflow.    |
|   18.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   18.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   27.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads contract information from ERP and stores it in Celonis from the past 2 years up to today.


## Source

### System
ISP_DIP

### Schema
ISPSAP

### Tables
- /1FE/0Z1002IT
- /1FE/0Z1012IT
- /1FE/0Z3002IT

### Fields
- BITCRDATE
- BITCRTIME
- VTREF
- VTPOS
- BITCRDATE
- BITCRTIME
- VTREF
- VTPOS
- BITCRDATE
- BITCRTIME
- VTREF
- VTPOS


## Target

### Primary Key
CONTRACT_ID

### Table
BILLABLE_ITEM

### Fields
- CREATED_ON
- CREATED_AT
- CONTRACT_ID
- CONTRACT_ITEM_NUMBER
- CREATED_ON
- CREATED_AT
- CONTRACT_ID
- CONTRACT_ITEM_NUMBER
- CREATED_ON
- CREATED_AT
- CONTRACT_ID
- CONTRACT_ITEM_NUMBER