CELONIS WORKLIST ITEM
EDT.CELONIS.push.o2c.worklist_items


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   31.10.2019  |   2.2.0   |   C5215227    |   Implemented with Celonis Operator 0.8.3 and tested.    |
|   31.10.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   29.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads worklist information from ERP and stores it in Celonis from the past 2 years up to today.


## Source

### System
ISP_DIP

### Schema
SAPISP

### Table
UDM_COLL_ITEM

### Fields
- Substr(open_item_ref, 15, 10)
- to_timestamp(timestamp)


## Target

### Primary Key
open_item_ref

### Table
WORKLIST_ITEMS

### Fields
- INVOICE_ID
- WORKLIST_COLLECTION_CREATED_AT