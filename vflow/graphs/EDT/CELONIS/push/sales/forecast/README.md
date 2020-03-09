# CELONIS SALES FORECAST
EDT.CELONIS.push.sales.forecast


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   25.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   25.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   04.02.2020  |   2.2.2   |   C5215227    |   ITSXCEL-333.    |
|   23.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   23.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   24.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |

## Description
Reads sales forecast information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- adrm.reporting/CL_ADRM_CLOUD_EXPRESS_FORECAST_TEMPLATE_FLEXCURR
- adrm.reporting/CL_ADRM_ONPREM_EXPRESS_FORECAST_REPORTING_FLEXCURR
- gssv.reporting/CL_GSSV_SERVICES_SALES_BOOKINGS_FORECAST

### Fields
- ca_object_id, object_id, opp_id
- prctr, profit_ctr, profit_center
- ic_status_txt, null, opp_status
- close_date, ic_expect_end, closing_date_char
- cm_adrm_acv_bud_flexcurr, adrm_forecast_bud_flexcurr, adrm_bc
- cm_adrm_acv_flexcurr, adrm_forecast_flexcurr, adrm_fc
- cm_adrm_acv_cc_flexcurr, upside_cc_flexcurr, upside_fc
- cm_prob_acv_cc_flexcurr, probable_cc_flexcurr, probable_fc


## Target

### Primary Key
CA_OBJECT_ID (CASE_KEY)

### Table
FORECAST

### Fields
- CASE_KEY
- PROFIT_CENTER
- OPPT_STATUS
- CLOSE_DATE
- ADRM_FORECAST_BUD_FLEXCURR
- ADRM_FORECAST_FLEXCURR
- UPSIDE_CC_FLEXCURR
- PROBABLE_CC_FLEXCURR