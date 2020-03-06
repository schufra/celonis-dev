# CELONIS ACTIVITY
EDT.CELONIS.push.mktg.act.txns


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   01.10.2019  |   2.0.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.1 and retested.    |
|   01.10.2019  |   2.0.1   |   C5215227    |   Documented workflow.    |

## Description
Reads activity information from BW and stores it in Celonis from the past 2 years up to today.  Field ACTIVITY_CREATED_BY gets anonymized as either AUTO or USER.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Table
corp.gmar.core.activities/CL_GMAR_ACTIVITIES_AN

### Fields
- ACTIVITY_ID
- CREATED_AT_CET
- ACTIVITY_CREATED_BY
- ACTIVITY_PROCESS_TYPE
- ACTIVITY_STATUS
- ACTIVITY_INITIATED_BY
- CO_COMPANY_ID
- CAMP_CAMPAIGN_ID
- CAMP_CAMPAIGNTYPE
- CAMP_OBJECTIVE
- SALESBAG_LVL3
- DISTRIBUTION_CHANNEL_DESCRIPTION
- ACTIVITY_DIVISION
- ACTIVITY_SALES_ORG
- SALES_SALES_GROUP
- CAMP_MARKETING_SEGMENT
- CO_REGIONAL_BUYING_CLASSIFICATION
- CO_MASTERCODE
- CO_COUNTRY
- SALES_SAP_REGION
- SALES_BU_HUB_CNTRY
- SALES_MU_CNTRY_SUPER_REG
- ACTIVITY_REASON

## Target

### Primary Key
CASE_KEY

### Table
ACTIVITY

### Fields
- CASE_KEY
- CREATED_ON
- CREATED_BY
- PROCESS_TYPE
- STATUS
- INITIATOR
- ACCOUNT
- CAMPAIGN
- CAMPAIGN_TYPE
- CAMPAIGN_SUBTYPE
- SALES_BAG_LVL_3
- DIS_CHANNEL
- DIVISION
- SALES_ORG
- SALES_GROUP
- MKT_SEGMENT
- GTM_BUY_REG
- SAP_MASTER
- COUNTRY
- REGION
- SUBREGION
- MKT_UNIT
- REASON