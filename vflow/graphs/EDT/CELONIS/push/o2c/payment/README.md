# CELONIS PAYMENT
EDT.CELONIS.push.o2c.payment


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   28.10.2019  |   2.2.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.3 and retested.    |
|   28.10.2019  |   2.2.1   |   C5215227    |   Documented workflow.    |
|   28.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   28.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads payment information from BW and stores it in Celonis from the past 2 years up to today.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- corp.fare.core/CL_FARE_BSEG
- corp.fare.core/CL_FARE_BSAD
- corp.fare.core/CL_FARE_BKPF

### Fields
- cpudt
- cputm
- belnr


## Target

### Primary Key
none

### Table
PAYMENT

### Fields
- PAYMENT_RECIEVED_ON
- PAYMENT_RECIEVED_AT
- OPEN_ITEM