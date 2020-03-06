# CELONIS BOOKINGS FORECAST
EDT.CELONIS.push.sales.bookings_forecast


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   19.12.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   19.12.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   25.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   25.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Loops through the months of the last two years to read forecast information from BW and stores it in Celonis.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### View
corp.gssv.datamart/CL_GSSV_IC_SERVICES_SALES_FORECAST_SNAPSHOTS

### Fields
- ADRM_FC
- CM_VERBAL_FC
- OPPT_ID
- OPP_STATUS
- PROBABLE_CC
- PRODUCT_ID
- PROFIT_CENTER
- SNAPSHOT_PERIODS
- UPSIDE_CC


## Target

### Primary Key
none

### Table
BOOKINGS_FORECAST

### Fields
- ADRM_FC
- CM_VERBAL_FC
- OPPT_ID
- OPP_STATUS
- PROBABLE_CC
- PRODUCT_ID
- PROFIT_CENTER
- snapshot_periods
- UPSIDE_CC