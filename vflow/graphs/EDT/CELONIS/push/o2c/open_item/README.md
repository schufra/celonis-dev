# CELONIS OPEN ITEM
EDT.CELONIS.push.o2c.open_item


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   28.10.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   29.10.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   28.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads open item information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- corp.fare.core/CL_FARE_BSID
- corp.fare.core/CL_FARE_BKPF
- corp.fare.core/CL_FARE_BSEG

### Fields
- cpudt
- cputm
- xblnr
- netdt
- belnr
- xreversing


## Target

### Primary Key
BILLING_DOC_ID

### Table
OPEN_ITEM

### Fields
- OPEN_ITEM_CREATE_DATE
- OPEN_ITEM_CREATE_TIME
- BILLING_DOC_ID
- PAYMENT_DUE_DATE
- OPEN_ITEM
- REVERSAL_FLAG