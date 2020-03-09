# CELONIS DEAL EXECUTION
EDT.CELONIS.push.sales.deal_exec


## Change Log
|   Date        |   Version |   User-ID     |   Comment                                             |
|   :--         |   :--     |   :--         |   :--                                                 |
|   14.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   14.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.                                |
|   16.12.2019  |   2.2.2   |   C5215227    |   Updated, retested and re-documented workflow.       |
|   23.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.                    |
|   23.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.                        |
|   24.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.                       |
|   09.03.2020  |   4.0.0   |   C5215227    |   Updated to the new Celonis template.                |


## Description
Reads deal execution information from a parameterised calculation view from BW and stores it in Celonis.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### View
adrm.reporting.selfsvc/CL_ADRM_SELFSERVICE_DEAL_EXECUTION

### Fields
- object_id
- ca_closing_quarter
- ca_8c_score_dtr_flag
- ca_8c_score_ntr_flag
- ca_zzreview_dat
- ca_closeplan_planned_or_validated_dtr_flag
- ca_closeplan_planned_or_validated_ntr_flag
- ff_level_03_desc
- ff_level_04_desc
- ca_close_plan_object
- ca_main_quote_create_date
- total_pipeline_kflexcurr


## Target

### Primary Key
OBJECT_ID

### Table
DEAL_EXECUTION

### Fields
- CASE_KEY
- CLOSING_QTR
- 8C_DTR_FLAG
- 8C_NTR_FLAG
- DEAL_REVIEW_COMPLETED
- CLOSEPLAN_DTR_FLAG
- CLOSEPLAN_NTR_FLAG
- SALES_BAG_03
- SALES_BAG_04
- CLOSE_PLAN_STATUS
- MAIN_QUOTE_CREATE_DT
- TOTAL_PIPELINE_KFLEXCURR