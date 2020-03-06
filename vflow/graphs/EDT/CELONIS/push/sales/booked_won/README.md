# CELONIS SALES BOOKED WON
EDT.CELONIS.push.sales.booked_won


## Change Log
|   Date        |   Version |   User-ID     |   Comment                                             |
|   :--         |   :--     |   :--         |   :--                                                 |
|   25.11.2019  |   2.2.0   |   C5215227    |   Implemented with Celonis Operator 0.8.3 and tested. |
|   25.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.                                |
|   27.11.2019  |   2.2.2   |   C5215227    |   Added column_type_dict.                             |
|   20.01.2020  |   2.2.3   |   C5215227    |   ITSXCEL-323.                                        |
|   25.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.                          |
|   25.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.                        |
|   06.03.2020  |   3.0.2   |   C5215227    |   ITSXCEL-352.                                        |


## Description
Reads opportunity information from BW and stores it in Celonis from the past 2 years up to today for every quarter.


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
SALES_OPPT_BOOKED_WON

### Fields
- CASE_KEY
- date_from
- time_from
- value_new