# CELONIS CRM ORDERS
EDT.CELONIS.push.o2c.crm_orders


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   25.10.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   25.10.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   28.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads order information from CRM and stores it in Celonis from the past 2 years up to today where process type is:

##### Process type
- ZK02 
- ZK09
- ZK04


## Source

### System
BWP_DIP

### Schema
Configurabe schema

### Tables
- crmd_orderadm_h
- crmd_orderadm_i
- crmd_customer_i
- zzk_case_data


### Fields
- created_at
- object_id
- zzk_case_id
- itm_type
- zzfld0000tc
- zzk_extref_type
- zzk_renewaltype


## Target

### Primary Key
none

### Table
CRM_ORDERS

### Fields
- crm_order_created_at
- order_id
- cms_case_id
- line_of_business
- business_type
- ext_ref_type
- renewal_type