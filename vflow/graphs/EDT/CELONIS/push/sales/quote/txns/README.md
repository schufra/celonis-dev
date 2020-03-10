# CELONIS QUOTE
EDT.CELONIS.push.sales.quote.txns


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   20.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   20.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   20.01.2020  |   2.2.2   |   C5215227    |   ITSXCEL-321.    |
|   24.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   24.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads quote information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- corp.quot.datamart/CL_QUOT_HEADER_ALL
- corp.quot.datamart/CL_QUOT_ITEM_ALL
- corp.deal.dimensions/CL_DEAL_ODEAL01
- corp.deal.dimensions/CL_DEAL_ODEAL31


### Fields
- quote_id
- opportunity_id
- quote_creation_date
- main_quote_flag
- revenue_type


## Target

### Primary Key
QUOTE_ID

### Table
QUOTE

### Fields
- quote_id
- OPPT_ID
- CREATED_AT
- main_quote_flag
- REVENUE_TYPE