# CELONIS REGION
EDT.CELONIS.push.mktg.mst.region


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   30.09.2019  |   2.0.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.1 and retested.    |
|   30.09.2019  |   2.0.1   |   C5215227    |   Documented workflow.    |
|   15.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   15.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   27.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads region information from a configurable schema within CRM and stores it in Celonis.


## Source

### System
ICP_DIP

### Schema
Configurable schema.

### Table
zbp_ctry_glreg_t

### Fields
- country
- global_region
- global_subregion
- landx


## Target

### Primary Key
No primary key.

### Table
ZBP_CTRY_GLREG_T

### Fields
- country
- global_region
- global_subregion
- landx