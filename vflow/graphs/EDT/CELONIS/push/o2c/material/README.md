# CELONIS MATERIAL
EDT.CELONIS.push.o2c.material

## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   24.09.2019  |   1.0.0   |   C5237223    |   Implemented, tested and documented workflow. |
|   24.10.2019  |   2.1.0   |   C5237223    |   Upgraded to Celonis Operator 0.8.2 and retested.    |
|   24.10.2019  |   2.1.1   |   C5237223    |   ITSXCEL-267.    |
|   24.10.2019  |   2.1.2   |   I504339     |   Added runtime parameters for schema name    |
|   02.03.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   02.03.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads dunning information from ERP and stores it in Celonis from the past 2 years up to today.

## Source

### System
BWP_DIP

### Schema
ISPSAP

### Tables
-DFKK_VT_I
-MARA


### Fields
-ZZK_OD_SOL_TYPE
-MADAT
-PRDNR
-VKORG


## Target
### Primary Key


### Table
MATERIAL

### Fields
-CASE_KEY
-MATERIAL,
-SALES_ORG