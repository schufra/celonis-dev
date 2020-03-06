# CELONIS CLOSE PLAN
EDT.CELONIS.push.sales.close_plan.history


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   01.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   01.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   02.12.2019  |   2.2.2   |   C5215227    |   ITSXCEL-303.    |
|   26.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   26.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads opportunity information from CRM and stores it in Celonis from the past 2 years up to today where activity code is:

##### Activity
- 00
- 02
- 03

##### Operator
It uses the Celonis Adjust Operator to pass in the first day of the year two years ago.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- corp.acti.datamart/CL_CORP_ACTI_ACTIVITIES_ALL_BASE
- corp.gspi.core/CL_GSPI_IC_OPPORTUNITY_HEADERBASE

### Fields
- iobject_id
- activity_change_date
- activity_initiated_by
- zzacvty_code                                                             
- activity_description
- activity_dist_channel


## Target

### Primary Key
IC_OBJECT_ID

### Table
SALES_CLOSE_PLAN_HISTORY

### Fields
- CASE_KEY
- close_plan_activities_date
- activity_initiated_by
- close_plan_activity
- activity_description
- activity_dist_channel