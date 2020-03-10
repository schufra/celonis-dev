# CELONIS SLIPPED SALES
EDT.CELONIS.push.sales.slipped


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   19.12.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   20.12.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   24.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   24.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads quote information from BW and stores it in Celonis from the past 2 years up to today for every quarter.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### View
corp.gspi.datamart.selfsvc/CL_GSPI_SELFSVC_SLIPPED_DEALS_HARMONIZED

### Fields
- ic_object_id
- slipped_deals_opp_flag_ntr
- slipped_deals_opp_flag_dtr


## Target

### Primary Key
IC_OBJECT_ID

### Table
SALES_SLIPPED

### Fields
- case_key
- slipped_deals_opp_flag_ntr
- slipped_deals_opp_flag_dtr