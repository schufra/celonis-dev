# CELONIS OPPORTUNITY
EDT.CELONIS.push.mktg.oppt.txns


## Change Log
|   Date        |   Version |   User-ID     |   Comment     |
|   :--         |   :--     |   :--         |   :--         |
|   01.10.2019  |   2.0.0   |   C5215227    |   Upgraded to Celonis Operator 0.8.1 and retested.    |
|   01.10.2019  |   2.0.1   |   C5215227    |   Documented workflow.    |
|   15.02.2020  |   3.0.0   |   C5215227    |   Retrieved from Tenant Workspace.    |
|   15.02.2020  |   3.0.1   |   C5215227    |   Added resource restrictions.    |
|   27.02.2020  |   3.0.2   |   C5215227    |   Validated against SharePoint.    |


## Description
Reads opportunity information from BW and stores it in Celonis from the past 2 years up to today. Field at_ic_opp_owner_partner gets anonymized as either USER or AUTO.


## Source

### System
BWP_DIP

### Schema
_SYS_BIC

### View
corp.gmar.datamart/CL_GMAR_GSPI_OPPORTUNITY

### Fields
- ic_object_id
- opp_mgo_creation_date
- at_ic_opp_owner_partner
- ic_process_type
- ic_status_txt
- opp_mgo_crm_marketing_element_id
- camp_campaign_type_text
- camp_campaign_subtype_desc
- ff_level_03_desc
- ff_level_04_desc
- ca_dist_channel_desc_nb
- sp_sales_org_txt
- erp_sales_off_text
- erp_sales_grp
- ic_int_market_segment
- ic_reg_buy_class_txt
- ic_master_code_txt
- ic_acc_country
- ca_na_global_level_01_desc
- ca_na_global_level_02_desc
- ca_na_global_level_03_desc
- ic_opp_reason_ltxt
- ‘Closing_YEAR’
- ‘CM_REVENUE_ACV_kEUR’
- ic_drm_category_txt
- opp_pipe_build_type_desc
- opp_pipe_build_type_id
- global_country_desc
- opp_mgo_prior_trans_id


## Target

### Primary Key
case_key

### Table
OPPT

### Fields
- case_key
- created_at
- created_by
- process_type
- status
- campaign
- campaign_type
- campaign_subtype
- sales_bag_lvl_3
- sales_bag_lvl_4
- dis_channel
- sales_org
- sales_office
- sales_group
- mkt_segment
- gtm_buy_reg
- sap_master
- country
- region
- subregion
- mkt_unit
- reason
- closing_year
- cm_revenue_acv_keur
- ic_drm_category_txt
- opp_pipe_build_type_desc
- opp_pipe_build_type_id
- global_country
- lead_id