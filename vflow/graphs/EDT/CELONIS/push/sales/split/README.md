# CELONIS SALES SPLIT DATE
EDT.CELONIS.push.sales.split


## Change Log
|   Date        |   Version |   User-ID     |   Comment                                             |
|   :--         |   :--     |   :--         |   :--                                                 |
|   20.12.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   20.12.2019  |   2.2.1   |   C5215227    |   Documented workflow.                                |
|   24.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.                          |
|   24.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.                        |
|   10.03.2020  |   4.0.0   |   C5215227    |   Updated to the new Celonis template.                |


## Description
Reads order information from CRM and stores it in Celonis from the past 2 years.


## Source

### System
ICP_DIP

### Schema
Configurable schema

### Tables
- crmd_orderadm_h
- zcrmd_opp_rpl_h
- cdhdr

### Fields
- object_id
- udate


## Target

### Primary Key
OBJECT_ID

### Table
SALES_OPPT_SPLIT

### Fields
- case_key
- split_party_date