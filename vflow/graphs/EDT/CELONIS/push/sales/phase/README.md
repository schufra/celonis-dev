# CELONIS SALES PHASE
EDT.CELONIS.push.sales.phase


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   18.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   18.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   28.11.2019  |   2.2.2   |   C5215227    |   ITSXCEL-300.    |
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
corp.gspi.core/CL_GSPI_IC_OPPORTUNITY_CRM_CHANGE_HISTORY_BASE

### Fields
- object_id
- date_from
- time_from
- value_new

## Target

### Primary Key
OBJECT_ID

### Table
SALES_OPPT_PHASE

### Fields
- case_key
- date_from
- time_from
- value_new