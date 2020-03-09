# CELONIS DEMAND MANAGEMENT
EDT.CELONIS.push.sales.dmd


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   15.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   15.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   24.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   24.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads opportunity information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### View
gspi.dmd.reporting/CL_GSPI_DMD_SELF_SERVICE

### Fields
- opportunity_id
- opp_status_txt
- profit_center
- closing_date
- untouched_pipeline
- unweighted_pipeline
- stalled_pipeline
- ef_pipeline
- unweighted_pipeline_bc
- budget_geo
- wonbooked_pipeline_bc


## Target

### Primary Key
OPPORTUNITY_ID

### Table
DEMAND_MANAGEMENT

### Fields
- CASE_KEY
- STATUS
- profit_center
- CLOSE_DATE
- untouched_pipeline
- unweighted_pipeline
- stalled_pipeline
- ef_pipeline
- unweighted_pipeline_bc
- budget_geo
- wonbooked_pipeline_bc