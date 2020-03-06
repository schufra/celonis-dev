# CELONIS LEAD ACTION
EDT.CELONIS.push.mktg.lead.act


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   26.09.2019  |   2.0.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.1 and retested.    |
|   27.09.2019  |   2.0.1   |   C5215227    |   Documented workflow.    |
|   15.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   15.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   27.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads lead history information from BW and stores it in Celonis from the past 2 years up to today where the change to the lead had been:

##### Change
- Open
- Marketing Qualification
- Convert into Opportunity
- Handover as Lead
- Sales Qualification
- Discontinued by Marketing
- Discontinued by Sales
- MKT Action Requested by Sales
- Completed
- Rejected / Cancelled by Sales

##### Anonymization
Field changedby_id gets anonymized as either USER or AUTO.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### View
gmar.reporting/CL_GMAR_LEAD_CHANGE_HISTORY

### Fields
- LEAD_ID
- CHANGEDBY_ID
- CHANGED_ON
- CHANGED_AT


## Target

### Primary Key
CASE_KEY

### Table
LEAD_ACTION

### Fields
- CASE_KEY
- CHANGED_BY
- CHANGED_ON
- CHANGED_AT