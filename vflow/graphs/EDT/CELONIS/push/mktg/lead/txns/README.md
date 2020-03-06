# CELONIS LEAD
EDT.CELONIS.push.mktg.lead.txns


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   30.09.2019  |   2.0.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.1 and retested.    |
|   30.09.2019  |   2.0.1   |   C5215227    |   Documented workflow.    |
|   15.10.2019  |   2.1.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.2 and retested.    |
|   16.10.2019  |   2.1.1   |   C5215227    |   ITSXCEL-266.    |
|   31.01.2020  |   2.2.0   |   C5215227    |   ITSXCEL-278.    |
|   15.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   15.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   27.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads lead information from BW and stores it in Celonis from the past 2 years up to today. Field lead_creator gets anonymized as either USER or AUTO.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### Views
- corp.gmar.datamart/CL_GMAR_LEADS_CORP
- corp.gmar.core.leads/CL_GMAR_LEAD_CHNGLOG

### Fields
- lead_id
- flag_passed_to_sales
- lead_created_date_cet
- lead_lead_type
- lead_status
- co_company_id
- camp_crm_marketing_element_id
- camp_campaign_type
- camp_campaign_subtype
- prod_sales_bag_level3
- prod_sales_bag_level4
- sales_distribution_channel
- sales_org_desc
- sales_office
- sales_sales_group
- co_internal_market_segment_text
- co_regional_buying_classification
- co_sap_master_code
- co_bp_country_name
- sales_sap_region
- sales_bu_hub_cntry
- sales_mu_cntry_super_reg
- lead_disposition_reason
- lead_requal_date
- camp_business_owner
- co_internal_account_classification
- days_create_to_convert
- days_to_accept
- days_to_reject
- lead_create_year
- lead_status
- manually_routed_flag
- occurrences_lead_id
- prod_item_category
- lead_lead_creator_bp
- lead_prior_id
- lead_status_year
- lead_status_date
- camp_crm_marketing_element_desc
- 8c_lead_score


## Target

### Primary Key
LEAD_ID

### Table
LEAD

### Fields
- CASE_KEY
- FLAG_PASSED_TO_SALES
- CREATED_AT
- LEAD_TYPE
- LEAD_STATUS
- ACCOUNT
- CAMPAIGN
- CAMPAIGN_TYPE
- CAMPAIGN_SUBTYPE
- SALES_BAG_LVL_3
- SALES_BAG_LVL_4
- DIS_CHANNEL
- SALES_ORG
- SALES_OFFICE
- SALES_GROUP
- MKT_SEGMENT
- GTM_BUY_REG
- SAP_MASTER
- COUNTRY
- REGION
- SUBREGION
- MKT_UNIT
- REASON
- REQUALIFICATION_DT
- CAMP_BUSINESS_OWNER
- CO_INTERNAL_ACCOUNT_CLASSIFICATION
- DAYS_CREATE_TO_CONVERT
- DAYS_TO_ACCEPT
- DAYS_TO_REJECT
- LEAD_CREATE_YEAR
- MANUALLY_ROUTED_FLAG
- OCCURRENCES_LEAD_ID
- PROD_ITEM_CATEGORY
- CREATED_BY
- ACTIVITY_ID
- LEAD_STATUS_YEAR
- STATUS_SINCE
- CAMP_CRM_MARKETING_
- CAMP_CRM_MARKETING_ELEMENT_DESC,
- 8C_LEAD_SCORE
