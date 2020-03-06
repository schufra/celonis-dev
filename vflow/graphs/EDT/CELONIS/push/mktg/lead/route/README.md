# CELONIS LEAD ROUTE
EDT.CELONIS.push.mktg.lead.route


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   30.09.2019  |   2.0.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.1 and retested.    |
|   30.09.2019  |   2.0.1   |   C5215227    |   Documented workflow.    |
|   27.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   27.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads lead information from a configurable schema CRM and stores it in Celonis from the past 2 years up to today where the change indicator to the lead had been:

##### Change
- ZLLEAC01
- ZMMKTQR
- ZMSLSQR


##### Anonymization
Field username gets anonymized as either USER or AUTO.


## Source

### System
ICP_DIP

### Schema
Configurable schema.

### Tables
- zcrmd_bw_lead_h
- cdhdr
- cdpos

### Fields
- object_id
- chngind
- tabkey
- username


## Target

### Primary Key
case_key

### Table
LEAD_ROUTE

### Fields
- case_key
- chngind
- tabkey
- username
