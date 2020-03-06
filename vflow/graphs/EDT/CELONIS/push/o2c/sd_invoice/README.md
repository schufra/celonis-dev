# CELONIS SD INVOICE
EDT.CELONIS.push.o2c.sd_invoice


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   31.10.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   31.10.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   29.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads invoice information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- corp.sdsd.invoices/CL_SDSD_VBRK
- corp.sdsd.invoices/CL_SDSD_VBRP

### Fields
- erdat
- erzet
- vgbel
- vbeln
- fkart
- vtweg
- bukrs


## Target

### Primary Key
none

### Table
SD_INVOICE

### Fields
- SD_INVOICE_CREAT_DT
- SD_INVOICE_CREAT_TIME
- ORDER_ID
- BILLING_DOC_ID
- BILLING_TYPE
- DISTRIBUTION_CHANNEL
- COMPANY_CODE