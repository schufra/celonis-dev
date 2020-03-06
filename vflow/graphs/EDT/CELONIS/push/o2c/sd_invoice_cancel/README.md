# CELONIS SD INVOICE CANCEL
EDT.CELONIS.push.o2c.sd_invoice_cancel


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   31.10.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   31.10.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   29.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads invoice information from ERP and stores it in Celonis from the past 2 years up to today where the object type is:

##### Object Type
- ZK02
- ZK04
- ZK09


## Source

### System
ISP_DIP

### Schema
SAPISP

### Tables
- SCMG_T_CASE_ATTR
- ZZV_D_RCMGEN_OL
- VBFA
- VBRK

### Fields
- ext_key
- erdat
- erzet
- vf_status


## Target

### Primary Key
none

### Table
SD_INVOICE_CANCEL

### Fields
- CASE_KEY
- SD_INVOCE_CANCEL_DATE
- SD_INVOICE_CANCEL_TIME
- BILLING_STATUS