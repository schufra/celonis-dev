# CELONIS O2C QUOTE STATUS
EDT.CELONIS.push.o2c.quote_status


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   11.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   11.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   29.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |
|   02.03.2020  |   3.0.3   |   C5215227    |   ITSXCEL-344.    |


## Description
Reads quote information from ERP and stores it in Celonis from the past 2 years up to today.


## Source

### System
ISP_DIP

### Schema
SAPISP

### Tables
- SRMRMSPDIR_CLNT
- SRMPROTOCOL
- ZZV_V_RCMGEN_DBV
- ZZV_D_RCMGEN_OL

### Fields
- object_id
- display_name
- arg1
- arg2
- timestamp
- callidus_flag´
- z.c4c_flag
- z.created_by
- z.sales_org


## Target

### Primary Key
none

### Table
O2C_QUOTE_STATUS

### Fields
- QUOTE_ID
- CMS_CASE_ID
- CMS_PREVIOUS_STATUS
- CMS_STATUS
- STATUS_CHANGE_TIME
- callidus_flag
- z.c4c_flag
- created_by
- z.sales_org