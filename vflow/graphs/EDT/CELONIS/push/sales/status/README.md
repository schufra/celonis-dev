# CELONIS SALES STATUS
EDT.CELONIS.push.sales.status


## Change Log
|   Date        |   Version |   User-ID     |   Comment                                             |
|   :--         |   :--     |   :--         |   :--                                                 |
|   27.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   28.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.                                |
|   20.01.2020  |   2.2.2   |   C5215227    |   ITSXCEL-320.                                        |
|   27.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.                          |
|   27.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.                        |
|   09.03.2020  |   3.0.2   |   C5215227    |   ITSXCEL-353.                                        |


## Description
Reads opportunity information from BW and stores it in Celonis from the past 2 years up to today for every quarter.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### View
- corp.gspi.core/CL_GSPI_IC_OPPORTUNITY_CRM_CHANGE_HISTORY_BASE
- corp.gspi.core/CL_GSPI_IC_OPPORTUNITY_HEADERBASE
- corp.gspi.core.dimension/CL_IC_STATUS_TXT

### Fields
- object_id
- date_from
- time_from
- IC_STATUS_TXT

## Target

### Primary Key
OBJECT_ID

### Table
SALES_OPPT_STATUS

### Fields
- CASE_KEY
- date_from
- time_from
- STATUS