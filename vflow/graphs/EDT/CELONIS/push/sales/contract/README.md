# CELONIS CONTRACT
EDT.CELONIS.push.sales.contract


## Change Log
|   Date        |   Version |   User-ID     |   Comment                                             |
|   :--         |   :--     |   :--         |   :--                                                 |
|   25.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   26.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.                                |
|   22.12.2019  |   2.2.2   |   C5215227    |   Documented workflow.                                |
|   27.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.                          |
|   27.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.                        |
|   06.03.2020  |   3.0.2   |   C5215227    |   ITSXCEL-318.                                        |


## Description
Reads opportunity and quote information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- corp.sdsd.provcont.dm/CL_SDSD_CONTRACT_I_DM
- corp.mada.sac.core/CL_CORP_MD_D1DOCN0_SOURCE


### Fields
- _b230_s_opptnumb
- _b230_s_doc_numb
- _b230_s_doc_type
- md.doc_categ
- _b230_s_sc07scsd
- _b230_s_createdo


## Target

### Primary Key
- QUOTE_ID
- OPPT_ID

### Table
CONTRACT

### Fields
- oppt_id
- doc_number
- doc_type
- doc_category
- create_contract_dt
- create_order_dt