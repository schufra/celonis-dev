# CELONIS QUOTE REVIEW
EDT.CELONIS.push.sales.quote.review.txns


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   19.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   19.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   24.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   24.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads opportunity information from BW and stores it in Celonis.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- corp.quot.datamart/CL_QUOT_REVIEW
- corp.quot.datamart/CL_QUOT_HEADER_ALL

### Fields
- quote_id
- opportunity_id
- request_date


## Target

### Primary Key
QUOTE_ID

### Table
QUOTE_REVIEW

### Fields
- QUOTE_ID
- OPPT_ID
- QUOTE_FOR_REVIEW_DATE