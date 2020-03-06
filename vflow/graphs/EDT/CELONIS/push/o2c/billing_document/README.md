# CELONIS O2C BILLING DOCUMENT
EDT.CELONIS.push.o2c.billing_document


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   18.10.2019  |   2.1.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.2 and retested.    |
|   18.10.2019  |   2.1.1   |   C5215227    |   Documented workflow.    |
|   28.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   28.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads billing document information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
ISD_BWV

### Tables
- dfkkinvbill_h
- dfkkinvbill_i

### Fields
- crdate
- crtime
- vtref
- vtpos
- billdocno


## Target

### Primary Key
none

### Table
BILLING_DOCUMENT

### Fields
- create_date
- create_time
- provider_contract_id
- provider_contract_item_id
- invoice_id