# CELONIS DEAL CONVERSION
EDT.CELONIS.push.sales.deal_conv


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   12.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.1 and retested.    |
|   12.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   24.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   24.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads cloud sales information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- corp.adrm.datamart.selfsvc/CL_ADRM_SELFSVC_DEAL_PIPE_CONVERSION
- corp.adrm.datamart.selfsvc/CL_ADRM_SELFSVC_DEAL_EXECUTION

### Fields
- ic_object_id
- ca_pipeline_conversion_dtr
- ca_pipeline_conversion_ntr
- ca_deal_conversion_dtr
- ca_deal_conversion_ntr
- ca_forecast_predictability_dtr
- ca_forecast_predictability_ntr


## Target

### Primary Key
IC_OBJECT_ID

### Table
DEAL_CONVERSION

### Fields
- CASE_KEY
- PIPELINE_CONV_DTR
- PIPELINE_CONV_NTR
- DEAL_CONV_DTR
- DEAL_CONV_NTR
- FORECAST_PREDICT_DTR
- FORECAST_PREDICT_NTR