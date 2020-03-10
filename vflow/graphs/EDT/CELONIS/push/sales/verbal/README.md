# CELONIS VERBAL
EDT.CELONIS.push.sales.verbal


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   05.02.2020  |   2.2.0   |   C5215227    |   Implemented and tested workflow.    |
|   05.02.2020  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   24.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   24.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads Verbal data required for ADRM vs Verbal KPI from BW.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- adrm.reporting/CL_ADRM_ONPREM_EXPRESS_FORECAST_REPORTING_FLEXCURR
- adrm.reporting/CL_ADRM_CLOUD_EXPRESS_FORECAST_TEMPLATE_FLEXCURR
- gssv.reporting/CL_GSSV_SERVICES_SALES_BOOKINGS_FORECAST

### Fields
- PROFIT_CTR
- GLOBAL_01_DESC
- GLOBAL_02_DESC
- GLOBAL_03_DESC
- VERBAL_FLEXCURR_SUM

## Target

### Primary Key
PROFIT_CENTER

### Table
SALES_VERBAL

### Fields
- PROFIT_CENTER
- LEVEL_01_DESC
- LEVEL_02_DESC
- LEVEL_03_DESC
- VERBAL_FLEXCURR_SUM