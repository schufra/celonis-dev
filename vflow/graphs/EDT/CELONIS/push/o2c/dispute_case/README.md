# CELONIS DISPUTE CASE
EDT.CELONIS.push.o2c.dispute_case


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   18.10.2019  |   2.1.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.2 and retested.    |
|   25.10.2019  |   2.1.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   28.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads case information from ERP and stores it in Celonis from the past 2 years up to today.


## Source

### System
ISP_DIP

### Schema
SAPISP

### Tables
- fdm_dcproc
- scmg_t_case_attr
- udmcaseattr00

### Fields
- ext_key
- create_time
- obj_key


## Target

### Primary Key
none

### Table
DISPUTE_CASE

### Fields
- DISPUTE_CASE_ID
- CREATE_TIME
- INVOICE_ID