# CELONIS PO NUMBER PC
EDT.CELONIS.push.o2c.po_number_pc


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   30.10.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   30.10.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   28.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads purchase order information from ERP and stores it in Celonis from the past 2 years up to today.


## Source

### System
ICP_DIP

### Schema
Configurable schema.

### Tables
- crmd_ist_ita3
- crmd_orderadm_i
- CRMD_CUSTOMER_I

### Fields
- created_at
- a3extref
- zzscms


## Target

### Primary Key
none

### Table
PO_NUMBER_PC

### Fields
- po_number_updated_at
- contract_id
- case_key