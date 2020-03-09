# CELONIS SALES OPPORTUNITY
EDT.CELONIS.push.sales.oppt


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   15.11.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   15.11.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   16.12.2019  |   2.2.2   |   C5215227    |   Updated, retested and redocumented workfow.    |
|   23.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   23.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   24.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |

## Description
Reads order information from CRM and stores it in Celonis from the past 2 years up to today where process type is:

##### Process Type
- ZOMM
- ZOFS
- ZOS1
- ZO4C
- ZOXX


## Source

### System
ICP_DIP

### Schema
Configurable schema

### Tables
- crmd_orderadm_h
- crmd_orderadm_i
- zs_1o_apptsv

### Fields
- object_id
- created_at
- changed_at


## Target

### Primary Key
OBJECT_ID

### Table
SALES_OPPT

### Fields
- case_key
- high_level_revenue_date
- eight_c_date