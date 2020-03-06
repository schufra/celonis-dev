# CELONIS AUTOMATION
EDT.CELONIS.push.o2c.automation


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   15.10.2019  |   2.0.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.1 and retested.    |
|   15.10.2019  |   2.0.1   |   C5215227    |   Documented workflow.    |
|   17.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   17.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   27.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads quote information from CRM and stores it in Celonis where the process type is:

##### Change
- ZK02
- ZK04
- ZK09

##### Anonymization
Field username gets anonymized as either USER or AUTO.


## Source

### System
ICP_DIP

### Schema
Configurable schema.

### Tables
- crmd_orderadm_h
- cdhdr

### Fields
- h.object_id
- username


## Target

### Primary Key
none

### Table
AUTOMATION

### Fields
- order_id
- username