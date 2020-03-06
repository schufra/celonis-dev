# CELONIS BILLABLE RAW
EDT.CELONIS.push.o2c.billable_raw


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   14.10.2019  |   2.0.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.2 and retested.    |
|   14.10.2019  |   2.0.1   |   C5215227    |   Documented workflow.    |
|   28.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   28.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads contract information from ERP and stores it in Celonis from the past 2 years up to today.


## Source

### System
ISP_DIP

### Schema
ISPSAP

### Tables
- /1FE/0Z1000IT
- /1FE/0Z1010IT
- /1FE/0Z3000IT
- /1FE/0Z1001IT
- /1FE/0Z1011IT
- /1FE/0Z3001IT

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
BILLABLE_RAW

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