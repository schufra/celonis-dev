# CELONIS PROVIDER CONTRACT
EDT.CELONIS.push.o2c.provider_contract


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   30.10.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   30.09.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   29.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads contract information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- corp.sdsd.provcont.core/CL_SDSD_PRVCON_ITM
- corp.sdsd.provcont.core/CL_SDSD_ZCRMD_BW_AGTM_I
- corp.sdsd.provcont.core/CL_SDSD_PROVCONT_IS_H

### Fields
- created_at
- zzscms_case_id
- vtkey
- vtpos
- erdat
- ertim


## Target

### Primary Key
none

### Table
PROVIDER_CONTRACT

### Fields
- CRM_PC_CREATED_AT
- CRM_PC_ITM_ID
- ERP_PROVIDER_CONTRACT
- ERP_PC_ITM_NUM
- ERP_CREATE_DATE
- ERP_CREATE_TIME