# CELONIS CLOUD BASE
EDT.CELONIS.push.sales.cloud_base


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   04.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.1 and retested.    |
|   04.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   28.11.2019  |   2.2.2   |   C5215227    |   ITSXCEL-304.    |
|   23.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   23.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   25.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads cloud sales information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### View
gspi.reporting/CL_GSPI_IC_PIPELINE_CLOUD_HISTORY

### Fields
- cca_object_id
- CM_REVENUE_ACV
- CM_TCV_KFLEX

## Target

### Primary Key
IC_OBJECT_ID

### Table
CLOUD_BASE

### Fields
- CASE_KEY
- CM_REVENUE_ACV_SUM
- CM_REVENUE_TCV_SUM