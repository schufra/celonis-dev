# CELONIS CLOSE PLAN
EDT.CELONIS.push.sales.close_plan


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   01.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   01.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   29.11.2019  |   2.2.2   |   C5215227    |   ITSXCEL-301.    |
|   22.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   22.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   25.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |

## Description
Reads opportunity information from CRM and stores it in Celonis from the past 2 years up to today where activity code is:

##### Activity
- 00
- 02
- 03


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- corp.acti.datamart/CL_CORP_ACTI_ACTIVITIES_ALL_BASE
- corp.gspi.core/CL_GSPI_IC_OPPORTUNITY_HEADERBASE


### Fields
- ic_object_id
- created_at
- act.activity_planned_date_to


## Target

### Primary Key
IC_OBJECT_ID

### Table
SALES_CLOSE_PLAN

### Fields
- case_key
- close_plan_create_date
- close_plan_due_date