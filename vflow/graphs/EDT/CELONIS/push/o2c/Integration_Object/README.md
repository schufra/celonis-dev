# CELONIS INTEGRATION OBJECT
EDT.CELONIS.push.o2c.integration_object


## Change Log
|   Date        |   Version |   User-ID     |   Comment                         |
|   :--         |   :--     |   :--         |   :--                             |
|   02.02.2020  |   2.0.0   |   I504339     |   Documented workflow.            |
|   28.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.      |
|   28.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   28.02.2020  |   3.0.2   |   C5215227    |   Added Run Configuration.        |
|   05.03.2020  |   3.0.3   |   C5215227    |   ITSXCEL-345.                    |


## Description
Reads Integration Object information from CRM and stores it in Celonis where the process type is:

##### Change
- ZZ01
- ZZ04

##### Anonymization
NA


## Source

### System
ICP_DIP

### Schema
Configurable schema.

### Tables
- crmd_orderadm_h
- zzk_case_date
- CRMD_ORDERADM_I

### Fields
- ltrim(ZZK_CASE_DATA.ZZK_CASE_ID,'0') as CASE_KEY
- CRMD_ORDERADM_H.OBJECT_ID as INTEGRATION_OBJECT
- to_date(CRMD_ORDERADM_H.CREATED_AT,'YYYYMMDDHH24MISS') as CREATED_AT


## Target

### Primary Key
none

### Table
INTEGRATION_OBJECT

### Fields
- CASE_KEY
- INTEGRATION_OBJECT
- CREATED_AT