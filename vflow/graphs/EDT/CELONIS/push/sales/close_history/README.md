# CELONIS SALES OPPT CLOSE HISTORY
EDT.CELONIS.push.sales.close_history


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   02.12.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   03.12.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   03.12.2019  |   2.2.2   |   C5215227    |   Populated property column_type_dict.    |


## Description
Reads opportunity history information from BW and stores it in Celonis from the past 2 years up to today for every quarter.


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
SALES_OPPT_CLOSE_HISTORY

### Fields
- CASE_KEY
- date_from
- time_from
- value_new