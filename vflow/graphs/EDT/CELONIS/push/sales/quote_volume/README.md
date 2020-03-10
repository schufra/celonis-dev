# CELONIS QUOTE VOLUME
EDT.CELONIS.push.sales.quote_volume


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   21.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.1 and retested.    |
|   21.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   20.10.2020  |   2.2.2   |   C5215227    |   ITSXCEL-322.    |
|   24.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   24.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   24.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads opportunity information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### View
corp.quot.datamart/CL_QUOT_HEADER_ALL

### Fields
- opportunity_id
- Count(DISTINCT quote_id)


## Target

### Primary Key
OPPT_ID

### Table
QUOTE_VOLUME

### Fields
- OPPT_ID
- QUOTE_VOLUME