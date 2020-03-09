# CELONIS OPPORTUNITY ADDITIONAL DATA
EDT.CELONIS.push.sales.oppt_data


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   21.11.2019  |   2.2.0   |   C5215227    |   Implemented and ocumented workflow.    |
|   22.11.2019  |   2.2.1   |   C5215227    |   Incorporated review feedback.    |
|   27.11.2019  |   2.2.2   |   C5215227    |   Field column_type_dict updated.    |
|   27.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   27.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   27.02.2020  |   3.0.2   |   C5215227    |   Corrected date conversion.    |


## Description
Reads order information from BW and stores it in Celonis from the past 2 years up to today.

##### Anonymization
Field changedby_id gets anonymized as either USER or AUTO.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### View
corp.gspi.core/CL_GSPI_IC_OPPORTUNITY_HEADERBASE

### Fields
- IC_OBJECT_ID
- CREATED_AT
- CREATED_BY
- IC_EXPECT_END
- IC_SOURCE
- ZZREVMET_DAT
- ZZREVIEW_DAT
- IC_CURR_PHASE
- PHASE_SINCE_DATE_SQL
- IC_STATUS_TXT
- STATUS_SINCE_DATE_SQL
- IC_EXPECT_END_DATE_SQL
- REVENUE_START_DATE_SQL
- REVENUE_END_DATE_SQL
- H_FF_REGION
- SALES_OFFICE_DESC
- H_SALES_ORG_TXT
- SALES_GROUP_DESC
- IC_DIST_CHANNEL
- H_FF_MARKET_UNIT
- IC_EXPECT_END_CALQUARTER_TXT
- IC_MASTER_CODE


## Target

### Primary Key
IC_OBJECT_ID

### Table
SALES_OPPT_DATA

### Fields
- CASE_KEY
- CREATED_AT
- CREATED_BY
- CLOSE_DATE
- SOURCE
- PLAN_REVIEW_MTG_DATE
- DEAL_QUALIFICATION_DATE
- CURR_PHASE
- PHASE_SINCE
- STATUS
- STATUS_SINCE
- EXPECT_END
- REVENUE_START_DATE
- REVENUE_END_DATE
- REGION
- SALES_OFFICE
- SALES_ORG
- SALES_GROUP
- DIS_CHANNEL
- PROFIT_CENTER
- QUARTER
- MASTER_CODE