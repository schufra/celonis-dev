# CELONIS CONTRACT STATUS
EDT.CELONIS.push.sales.contract.status


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   11.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   11.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   27.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   27.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads opportunity and quote information from ERP and stores it in Celonis from the past 2 years up to today where the type is:

##### Type
- 10
- 12
- 19
- 35
- 45
- 48
- 56
- 67
- 91


## Source

### System
ISP_DIP

### Schema
SAPISP

### Tables
- srmprotocol
- srmrmspdir_clnt 
- d_rcmgen_ol
- zzv_d_rcmgen_ol

### Fields
- object_id
- object_id
- arg2
- ref_type
- timestamp


## Target

### Primary Key
QUOTE_ID

### Table
CONTRACT_STATUS

### Fields
- quote_id
- oppt_id
- status
- ref_type
- timestamp