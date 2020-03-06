# CELONIS ERP ORDERS
EDT.CELONIS.push.o2c.erp_orders


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   25.10.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   25.10.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   19.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   19.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   28.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads order information from ERP and stores it in Celonis from the past 2 years up to today where order type is:

##### Order type
- ZK02
- ZK04
- ZK09


## Source

### System
ISP_DIP

### Schema
SAPISP

### Table
vbak

### Fields
- erdat
- erzet
- vbeln
- vkorg
- vtweg


## Target

### Primary Key
none

### Table
ERP_ORDERS

### Fields
- ORDER_CREATE_DATE
- ORDER_CREATE_TIME
- ORDER_ID
- SALES_ORG
- DISTRIBUTION_CHANNEL