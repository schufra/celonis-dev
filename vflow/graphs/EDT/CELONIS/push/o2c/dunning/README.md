# CELONIS DUNNING INFORMATION
EDT.CELONIS.push.o2c.dunning

## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   14.11.2019  |   2.0.0   |   C5234626    |   Implemented, tested and documented workflow. |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   28.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads dunning information from ERP and stores it in Celonis from the past 2 years up to today.

## Source

### System
ISP_DIP

### Schema
ISPSAP

### Tables
-BSEG
-BKPF


### Fields
-BUKRS
-MADAT
-MANST 
-AWKEY


## Target
### Primary Key


### Table
DUNNING

### Fields
-COMPANY_CODE
-DUNNING_LEVEL
-INVOICE_ID
-LAST_DUNNED_DATE