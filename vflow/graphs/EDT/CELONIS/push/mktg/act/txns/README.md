# CELONIS ACTIVITY
EDT.CELONIS.push.mktg.act.txns


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   28.09.2019  |   2.0.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.1 and retested.    |
|   28.09.2019  |   2.0.1   |   C5215227    |   Documented workflow.    |
|   26.02.2020  |   3.0.0   |   C5215227    |   Retrieved from SharePoint.    |
|   26.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |


## Description
Reads lead activity information from BW and stores it in Celonis from the past 2 years up to today where the activity process type is:

##### Activity Process Type
- ZM01

##### Anonymization
Field activity_created_by gets anonymized as either USER or AUTO.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### View
corp.gmar.core.activities/CL_GMAR_ACTIVITIES_AN

### Fields
- activity_id
- created_at_cet
- created_by
- activity_process_type
- activity_status
- activity_initiated_by
- co_company_id
- camp_campaign_id
- camp_campaigntype
- distribution_channel_description
- activity_division
- activity_sales_org
- sales_sales_group
- camp_marketing_segment
- co_regional_buying_classification
- co_mastercode
- co_country
- sales_sap_region
- sales_bu_hub_cntry
- sales_mu_cntry_super_reg
- activity_reason


## Target

### Primary Key
ACTIVITY_ID

### Table
ACTIVITY

### Fields
- case_key
- created_on
- activity_created_by
- process_type
- status
- initiator
- account
- campaign
- campaign_type
- campaign_subtype
- sales_bag_lvl_3
- dis_channel,
- sales_group
- camp_marketing_segment
- gtm_buy_reg
- sap_master
- country
- region
- subregion
- sales_mu_cntry_super_reg
- reason