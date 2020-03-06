# CELONIS CREDIT NOTE
EDT.CELONIS.push.o2c.credit_note


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   21.01.2020  |   2.2.0   |   C5215227    |   Implemented with Celonis Operator 0.8.3 and tested.    |
|   21.01.2020  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   28.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads billing information from ERP and stores it in Celonis from the past 2 years up to today.


## Source

### System
ISP_DIP

### Schema
SAPISP

### Tables
- VBAK
- VBFA
- FDM_DCPROC
- SCMG_T_CASE_ATTR
- VBRK


### Fields
- vbelv
- erdat
- erzet
- 'Credit memo'
- ext_key
- create_time
- Substr(obj_key, 5, 10)


## Target

### Primary Key
vbelv

### Table
CREDIT_NOTE

### Fields
- INVOICE_ID
- CREATED_ON
- CONTRACT_AT
- NOTE_TYPE
- DISPUTE_CASE_ID
- create_time
- INVOICE_ID