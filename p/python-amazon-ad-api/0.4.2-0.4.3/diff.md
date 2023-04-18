# Comparing `tmp/python-amazon-ad-api-0.4.2.tar.gz` & `tmp/python-amazon-ad-api-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-amazon-ad-api-0.4.2.tar", last modified: Tue Apr 11 17:45:07 2023, max compression
+gzip compressed data, was "python-amazon-ad-api-0.4.3.tar", last modified: Tue Apr 18 09:10:01 2023, max compression
```

## Comparing `python-amazon-ad-api-0.4.2.tar` & `python-amazon-ad-api-0.4.3.tar`

### file list

```diff
@@ -1,125 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.373552 python-amazon-ad-api-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-04-11 17:45:07.373552 python-amazon-ad-api-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14879 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.353552 python-amazon-ad-api-0.4.2/ad_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.353552 python-amazon-ad-api-0.4.2/ad_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/advertising_test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/audiences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/brand_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/creative_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.357552 python-amazon-ad-api-0.4.2/ad_api/api/dsp/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/dsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/dsp/access_token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/dsp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/dsp/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/dsp/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/eligibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/insights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/invoices.py
--rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/manager_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.361552 python-amazon-ad-api-0.4.2/ad_api/api/sb/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/ad_groups_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/ads_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/brands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/campaigns_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/keywords_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/landing_page_asins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sb/targeting_recommendations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.361552 python-amazon-ad-api-0.4.2/ad_api/api/sd/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/creatives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/product_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sd/targeting_recommendations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.369552 python-amazon-ad-api-0.4.2/ad_api/api/sp/
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/ad_groups_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/bid_recommendations_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_initial_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_rules_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_consolidated_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_negative_keywords_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_negative_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaigns_budget_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaigns_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/campaings_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/keywords_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_keywords_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_product_targeting_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/product_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/product_ads_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/product_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/product_targeting_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/ranked_keywords_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/sp/suggested_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/api/validation_configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.369552 python-amazon-ad-api-0.4.2/ad_api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/auth/access_token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/auth/access_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/auth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.373552 python-amazon-ad-api-0.4.2/ad_api/base/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/marketplaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/ad_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:45:07.373552 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-04-11 17:45:07.000000 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-11 17:45:07.000000 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:45:07.000000 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-11 17:45:07.000000 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 17:45:07.000000 python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-11 17:45:07.373552 python-amazon-ad-api-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-11 17:44:55.000000 python-amazon-ad-api-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.825287 python-amazon-ad-api-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-04-18 09:10:01.825287 python-amazon-ad-api-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17119 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.789287 python-amazon-ad-api-0.4.3/ad_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.797287 python-amazon-ad-api-0.4.3/ad_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/advertising_test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/audiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/brand_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/creative_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.797287 python-amazon-ad-api-0.4.3/ad_api/api/dsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/dsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/dsp/access_token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/dsp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/dsp/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/dsp/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/eligibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/manager_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.805287 python-amazon-ad-api-0.4.3/ad_api/api/sb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/ad_groups_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/ads_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/brands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/campaigns_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/keywords_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/landing_page_asins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/targeting_recommendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.809287 python-amazon-ad-api-0.4.3/ad_api/api/sd/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/brand_safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/budget_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/campaigns_budget_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19461 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/creatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/product_ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/targeting_recommendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.817287 python-amazon-ad-api-0.4.3/ad_api/api/sp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/ad_groups_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/bid_recommendations_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_initial_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_rules_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_consolidated_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns_budget_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaings_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_product_targeting_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/product_ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/product_ads_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/product_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/product_targeting_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/ranked_keywords_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/suggested_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/validation_configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.821287 python-amazon-ad-api-0.4.3/ad_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/auth/access_token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/auth/access_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/auth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.821287 python-amazon-ad-api-0.4.3/ad_api/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/marketplaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.825287 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-04-18 09:10:01.000000 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-18 09:10:01.000000 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:10:01.000000 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 09:10:01.000000 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 09:10:01.000000 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-18 09:10:01.825287 python-amazon-ad-api-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/setup.py
```

### Comparing `python-amazon-ad-api-0.4.2/LICENSE` & `python-amazon-ad-api-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/PKG-INFO` & `python-amazon-ad-api-0.4.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,10 @@
-Metadata-Version: 2.1
-Name: python-amazon-ad-api
-Version: 0.4.2
-Summary: Python wrapper for the Amazon Advertising API
-Home-page: https://github.com/denisneuf/python-amazon-ad-api
-Author: Daniel Alvaro
-Author-email: info@leadtech.es
-License: MIT
-Project-URL: Bug Tracker, https://github.com/denisneuf/python-amazon-ad-api/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PYTHON-AMAZON-AD-API
 
-![CodeQL](https://img.shields.io/badge/coverage-90%25-green)
+![CodeQL](https://img.shields.io/badge/coverage-95%25-green)
 ![CodeQL](https://img.shields.io/badge/Docs-sphinx-green)
 ![CodeQL](https://img.shields.io/github/v/release/denisneuf/python-amazon-ad-api)
 [![Documentation Status](https://readthedocs.org/projects/python-amazon-ad-api/badge/?version=latest)](https://python-amazon-ad-api.readthedocs.io/en/latest/?badge=latest)
 
 
 ## Amazon's Advertising API
 
@@ -234,58 +219,48 @@
 
 ### [Modules Available Common Resources](https://python-amazon-ad-api.readthedocs.io/en/latest/api.html)
 
 * [Profiles](https://python-amazon-ad-api.readthedocs.io/en/latest/api/profiles.html)
 * [Manager Accounts](https://python-amazon-ad-api.readthedocs.io/en/latest/api/manager_accounts.html)
 * [Portfolios](https://python-amazon-ad-api.readthedocs.io/en/latest/api/portfolios.html)
 * [Invoices](https://python-amazon-ad-api.readthedocs.io/en/latest/api/invoices.html)
-* Billing
+* [Billing](https://python-amazon-ad-api.readthedocs.io/en/latest/api/billing.html)
 * [Audiences](https://python-amazon-ad-api.readthedocs.io/en/latest/api/audiences.html)
 * [Change History open Beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/history.html)
 * [Creative Assets open Beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api//creative_assets.html)
 * [Elegibility](https://python-amazon-ad-api.readthedocs.io/en/latest/api/eligibility.html)
 * [Insights](https://python-amazon-ad-api.readthedocs.io/en/latest/api/insights.html)
 * [Localization](https://python-amazon-ad-api.readthedocs.io/en/latest/api/localization.html)
 * [Product Selector](https://python-amazon-ad-api.readthedocs.io/en/latest/api/metadata.html)
-* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/reports.html)
 * [Validation Configurations](https://python-amazon-ad-api.readthedocs.io/en/latest/api/validation_configurations.html)
+* [Tactical recommendations beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/recommendations.html)
 
 
-### Amazon Attribution open beta
-* Advertisers
-* Publishers
-* Attribution tags
-* Reports
+### [Amazon Attribution open beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html)
+* [Advertisers](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_advertisers)
+* [Publishers](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_publishers)
+* [Macro tags](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_macro_tag)
+* [Non Macro tags](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_non_macro_template_tag)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.post_report)
 
 ### [Brand Metrics open beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html)
 * [Post Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.post_report)
 * [Get Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.get_report)
 * [Download Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.download_report)
 
 ### [Advertising Test Account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html)
 * [Create test account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount)
 * [Get test account information](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount.AdvertisingTestAccount.get_test_account)
 
+
 ### [Modules Available Sponsored Products 2.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v2.html)
 
 Warning: [PLANNED DEPRECATION 6/30/2023]
 There is a new version 3 of Sponsored Product API, please check the [migration guide](https://advertising.amazon.com/API/docs/en-us/sponsored-products/v3-migration-guide).
 
-* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns.html)
-* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups.html)
-* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations.html)
-* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords.html)
-* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_keywords.html)
-* [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords.html)
-* [Suggested Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/suggested_keywords.html)
-* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_ads.html)
-* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_targeting.html)
-* [Negative Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_product_targeting.html)
-* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/reports.html)
-* [Snapshots](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/snapshots.html)
 
 ### [Modules Available Sponsored Products 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v3.html)
 
 
 * [ThemeBased Bid Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations_v3.html)
 * [Keyword Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ranked_keywords_recommendations.html)
 * [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords_v3.html)
@@ -300,51 +275,57 @@
 * [Budget Rules Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_rules_recommendations.html)
 * [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaignsv3.html)
 * [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups_v3.html)
 * [Consolidated Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns_consolidated_recommendations.html)
 * [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords_v3.html)
 * [Product Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_recommendations.html)
 * [Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_budget_usage.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/reports.html)
 
 
-### Modules Available Sponsored Brands 3.0
+### [Modules Available Sponsored Brands 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v3.html)
 
-* Campaigns
-* Ad Groups
-* Keywords
-* Negative Keywords
-* Product Targeting
-* Negative Product Targeting
-* Targeting Recommendations
-* Bid Recommendations
-* Stores
-* Landing Page Asins
-* Media
-* Brands
-* Moderation
-* Reports
+* Campaigns(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns.html)
+* Ad Groups(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups.html)
+* Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/keywords.html)
+* Negative Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_keywords.html)
+* Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/product_targeting.html)
+* Negative Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_product_targeting.html)
+* Targeting Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/targeting_recommendations.html)
+* Bid Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/bid_recommendations.html)
+* Stores(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/stores.html)
+* Landing Page Asins(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/landing_page_asins.html)
+* Media(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/media.html)
+* Brands(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/brands.html)
+* Moderation(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/moderation.html)
+* Reports(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/reports.html)
 * Snapshots
 
-### Modules Available Sponsored Brands 4.0
+### [Modules Available Sponsored Brands 4.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v4.html)
 
 * [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns_v4.html)
 * [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups_v4.html)
 * [Ads Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ads_v4.html)
 
-### Modules Available Sponsored Display
+### [Modules Available Sponsored Display](https://python-amazon-ad-api.readthedocs.io/en/latest/sd.html)
 
-* Campaigns
-* Ad Groups
-* Reports
-* Product Ads
-* Targets
-* Negative Targets
-* Targets Recommendations
-* Bid Recommendations
-* Creatives
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/campaigns.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/ad_groups.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/reports.html)
+* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/product_ads.html)
+* [Targets](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/product_targeting.html)
+* [Negative Targets](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/negative_product_targeting.html)
+* [Targets Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/targeting_recommendations.html)
+* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/bid_recommendations.html)
+* [Creatives](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/creatives.html)
+* [Brand Safety List](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/brand_safety.html)
+* [Budget Rules](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/budget_rules.html)
+* [Campaigns Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/campaign_budget_usage.html)
+* [Forecasts](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/forecast.html)
+* [Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/recommendations.html)
 
 ### Modules Available DSP
 
 * Reports
 
 ### Simple Example Usage Campaigns with Credentials
```

### Comparing `python-amazon-ad-api-0.4.2/README.md` & `python-amazon-ad-api-0.4.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,25 @@
+Metadata-Version: 2.1
+Name: python-amazon-ad-api
+Version: 0.4.3
+Summary: Python wrapper for the Amazon Advertising API
+Home-page: https://github.com/denisneuf/python-amazon-ad-api
+Author: Daniel Alvaro
+Author-email: info@leadtech.es
+License: MIT
+Project-URL: Bug Tracker, https://github.com/denisneuf/python-amazon-ad-api/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PYTHON-AMAZON-AD-API
 
-![CodeQL](https://img.shields.io/badge/coverage-90%25-green)
+![CodeQL](https://img.shields.io/badge/coverage-95%25-green)
 ![CodeQL](https://img.shields.io/badge/Docs-sphinx-green)
 ![CodeQL](https://img.shields.io/github/v/release/denisneuf/python-amazon-ad-api)
 [![Documentation Status](https://readthedocs.org/projects/python-amazon-ad-api/badge/?version=latest)](https://python-amazon-ad-api.readthedocs.io/en/latest/?badge=latest)
 
 
 ## Amazon's Advertising API
 
@@ -219,58 +234,48 @@
 
 ### [Modules Available Common Resources](https://python-amazon-ad-api.readthedocs.io/en/latest/api.html)
 
 * [Profiles](https://python-amazon-ad-api.readthedocs.io/en/latest/api/profiles.html)
 * [Manager Accounts](https://python-amazon-ad-api.readthedocs.io/en/latest/api/manager_accounts.html)
 * [Portfolios](https://python-amazon-ad-api.readthedocs.io/en/latest/api/portfolios.html)
 * [Invoices](https://python-amazon-ad-api.readthedocs.io/en/latest/api/invoices.html)
-* Billing
+* [Billing](https://python-amazon-ad-api.readthedocs.io/en/latest/api/billing.html)
 * [Audiences](https://python-amazon-ad-api.readthedocs.io/en/latest/api/audiences.html)
 * [Change History open Beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/history.html)
 * [Creative Assets open Beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api//creative_assets.html)
 * [Elegibility](https://python-amazon-ad-api.readthedocs.io/en/latest/api/eligibility.html)
 * [Insights](https://python-amazon-ad-api.readthedocs.io/en/latest/api/insights.html)
 * [Localization](https://python-amazon-ad-api.readthedocs.io/en/latest/api/localization.html)
 * [Product Selector](https://python-amazon-ad-api.readthedocs.io/en/latest/api/metadata.html)
-* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/reports.html)
 * [Validation Configurations](https://python-amazon-ad-api.readthedocs.io/en/latest/api/validation_configurations.html)
+* [Tactical recommendations beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/recommendations.html)
 
 
-### Amazon Attribution open beta
-* Advertisers
-* Publishers
-* Attribution tags
-* Reports
+### [Amazon Attribution open beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html)
+* [Advertisers](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_advertisers)
+* [Publishers](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_publishers)
+* [Macro tags](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_macro_tag)
+* [Non Macro tags](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_non_macro_template_tag)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.post_report)
 
 ### [Brand Metrics open beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html)
 * [Post Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.post_report)
 * [Get Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.get_report)
 * [Download Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.download_report)
 
 ### [Advertising Test Account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html)
 * [Create test account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount)
 * [Get test account information](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount.AdvertisingTestAccount.get_test_account)
 
+
 ### [Modules Available Sponsored Products 2.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v2.html)
 
 Warning: [PLANNED DEPRECATION 6/30/2023]
 There is a new version 3 of Sponsored Product API, please check the [migration guide](https://advertising.amazon.com/API/docs/en-us/sponsored-products/v3-migration-guide).
 
-* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns.html)
-* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups.html)
-* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations.html)
-* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords.html)
-* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_keywords.html)
-* [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords.html)
-* [Suggested Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/suggested_keywords.html)
-* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_ads.html)
-* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_targeting.html)
-* [Negative Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_product_targeting.html)
-* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/reports.html)
-* [Snapshots](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/snapshots.html)
 
 ### [Modules Available Sponsored Products 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v3.html)
 
 
 * [ThemeBased Bid Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations_v3.html)
 * [Keyword Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ranked_keywords_recommendations.html)
 * [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords_v3.html)
@@ -285,51 +290,57 @@
 * [Budget Rules Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_rules_recommendations.html)
 * [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaignsv3.html)
 * [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups_v3.html)
 * [Consolidated Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns_consolidated_recommendations.html)
 * [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords_v3.html)
 * [Product Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_recommendations.html)
 * [Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_budget_usage.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/reports.html)
 
 
-### Modules Available Sponsored Brands 3.0
+### [Modules Available Sponsored Brands 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v3.html)
 
-* Campaigns
-* Ad Groups
-* Keywords
-* Negative Keywords
-* Product Targeting
-* Negative Product Targeting
-* Targeting Recommendations
-* Bid Recommendations
-* Stores
-* Landing Page Asins
-* Media
-* Brands
-* Moderation
-* Reports
+* Campaigns(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns.html)
+* Ad Groups(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups.html)
+* Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/keywords.html)
+* Negative Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_keywords.html)
+* Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/product_targeting.html)
+* Negative Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_product_targeting.html)
+* Targeting Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/targeting_recommendations.html)
+* Bid Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/bid_recommendations.html)
+* Stores(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/stores.html)
+* Landing Page Asins(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/landing_page_asins.html)
+* Media(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/media.html)
+* Brands(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/brands.html)
+* Moderation(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/moderation.html)
+* Reports(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/reports.html)
 * Snapshots
 
-### Modules Available Sponsored Brands 4.0
+### [Modules Available Sponsored Brands 4.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v4.html)
 
 * [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns_v4.html)
 * [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups_v4.html)
 * [Ads Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ads_v4.html)
 
-### Modules Available Sponsored Display
+### [Modules Available Sponsored Display](https://python-amazon-ad-api.readthedocs.io/en/latest/sd.html)
 
-* Campaigns
-* Ad Groups
-* Reports
-* Product Ads
-* Targets
-* Negative Targets
-* Targets Recommendations
-* Bid Recommendations
-* Creatives
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/campaigns.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/ad_groups.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/reports.html)
+* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/product_ads.html)
+* [Targets](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/product_targeting.html)
+* [Negative Targets](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/negative_product_targeting.html)
+* [Targets Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/targeting_recommendations.html)
+* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/bid_recommendations.html)
+* [Creatives](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/creatives.html)
+* [Brand Safety List](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/brand_safety.html)
+* [Budget Rules](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/budget_rules.html)
+* [Campaigns Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/campaign_budget_usage.html)
+* [Forecasts](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/forecast.html)
+* [Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/recommendations.html)
 
 ### Modules Available DSP
 
 * Reports
 
 ### Simple Example Usage Campaigns with Credentials
```

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/__init__.py` & `python-amazon-ad-api-0.4.3/ad_api/api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from . import sb as sponsored_brands
 from . import sd as sponsored_display
 from .attribution import Attribution
 from .brand_metrics import BrandMetrics
 from .advertising_test_account import AdvertisingTestAccount
 from .reports import Reports
 from .validation_configurations import ValidationConfigurations
+from .recommendations import Recommendations
 
 __all__ = [
     "sp",
     "sb",
     "sd",
     "sponsored_products",
     "sponsored_brands",
@@ -38,9 +39,10 @@
     "Audiences",
     "Portfolios",
     "Insights",
     "Attribution",
     "BrandMetrics",
     "AdvertisingTestAccount",
     "Reports",
-    "ValidationConfigurations"
+    "ValidationConfigurations",
+    "Recommendations"
 ]
```

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/advertising_test_account.py` & `python-amazon-ad-api-0.4.3/ad_api/api/advertising_test_account.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/attribution.py` & `python-amazon-ad-api-0.4.3/ad_api/api/attribution.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/audiences.py` & `python-amazon-ad-api-0.4.3/ad_api/api/audiences.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/brand_metrics.py` & `python-amazon-ad-api-0.4.3/ad_api/api/brand_metrics.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/creative_assets.py` & `python-amazon-ad-api-0.4.3/ad_api/api/creative_assets.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/dsp/client.py` & `python-amazon-ad-api-0.4.3/ad_api/api/dsp/client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/dsp/credential_provider.py` & `python-amazon-ad-api-0.4.3/ad_api/api/dsp/credential_provider.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/dsp/reports.py` & `python-amazon-ad-api-0.4.3/ad_api/api/dsp/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/eligibility.py` & `python-amazon-ad-api-0.4.3/ad_api/api/eligibility.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/history.py` & `python-amazon-ad-api-0.4.3/ad_api/api/history.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/insights.py` & `python-amazon-ad-api-0.4.3/ad_api/api/insights.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/invoices.py` & `python-amazon-ad-api-0.4.3/ad_api/api/invoices.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/localization.py` & `python-amazon-ad-api-0.4.3/ad_api/api/localization.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/manager_accounts.py` & `python-amazon-ad-api-0.4.3/ad_api/api/manager_accounts.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/metadata.py` & `python-amazon-ad-api-0.4.3/ad_api/api/metadata.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/portfolios.py` & `python-amazon-ad-api-0.4.3/ad_api/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/profiles.py` & `python-amazon-ad-api-0.4.3/ad_api/api/profiles.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/reports.py` & `python-amazon-ad-api-0.4.3/ad_api/api/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/__init__.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/ad_groups.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/ad_groups.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/ad_groups_v4.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/ad_groups_v4.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/ads_v4.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/ads_v4.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/bid_recommendations.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/brands.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/brands.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/campaigns.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/campaigns.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/campaigns_v4.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/campaigns_v4.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/keywords.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/landing_page_asins.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/landing_page_asins.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/media.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/media.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/moderation.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/moderation.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/negative_keywords.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/negative_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/negative_product_targeting.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/negative_product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/product_targeting.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/reports.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/snapshots.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/stores.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/stores.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sb/targeting_recommendations.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sb/targeting_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sd/ad_groups.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sd/ad_groups.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sd/bid_recommendations.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sd/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sd/campaigns.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sd/campaigns.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sd/negative_product_targeting.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sd/negative_product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sd/product_ads.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sd/product_ads.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sd/product_targeting.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sd/product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sd/reports.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sd/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sd/snapshots.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sd/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sd/targeting_recommendations.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sd/targeting_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/__init__.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/ad_groups.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/ad_groups.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/ad_groups_v3.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/ad_groups_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/bid_recommendations.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/bid_recommendations_v3.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/bid_recommendations_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_initial_recommendation.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_initial_recommendation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse, Utils
 
 class InitialBudgetRecommendation(Client):
     @sp_endpoint('/sp/campaigns/initialbudgetrecommendation', method='POST')
     def initial_campaign_budget_recommendation(self, **kwargs) -> ApiResponse:
-        json_version = 'application/vnd.spinitialbudgetrecommendation.v3+json'
+        json_version = 'application/vnd.spinitialbudgetrecommendation.v3.4+json'
 
         headers = {
             "Content-Type": json_version
         }
         return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False), params=kwargs, headers=headers)
```

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_recommendations.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_rules.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_rules.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/budget_rules_recommendations.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_rules_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_consolidated_recommendations.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_consolidated_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_negative_keywords.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_keywords.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse
+from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse, Utils
 
 class CampaignNegativeKeywords(Client):
 
     @sp_endpoint('/v2/sp/campaignNegativeKeywords/{}', method='GET')
+    @Utils.deprecated
     def get_campaign_negative_keyword(self, keywordId, **kwargs) -> ApiResponse:
         r"""
 
         get_campaign_negative_keyword(self, keywordId, \*\*kwargs) -> ApiResponse
 
         Gets a campaign negative keyword specified by identifier.
 
@@ -17,14 +18,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), keywordId), params=kwargs)
 
     @sp_endpoint('/v2/sp/campaignNegativeKeywords/{}', method='DELETE')
+    @Utils.deprecated
     def delete_campaign_negative_keyword(self, keywordId, **kwargs) -> ApiResponse:
         r"""
 
         delete_campaign_negative_keyword(self, keywordId, \*\*kwargs) -> ApiResponse
 
         Archives a campaign negative keyword.
 
@@ -35,14 +37,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), keywordId), params=kwargs)
 
     @sp_endpoint('/v2/sp/campaignNegativeKeywords/extended/{}', method='GET')
+    @Utils.deprecated
     def get_campaign_negative_keyword_extended(self, keywordId, **kwargs) -> ApiResponse:
         r"""
 
         get_campaign_negative_keyword_extended(self, keywordId, \*\*kwargs) -> ApiResponse
 
         Gets a campaign negative keyword that has extended data fields.
 
@@ -52,14 +55,15 @@
 
             ApiResponse
 
         """
         return self._request(fill_query_params(kwargs.pop('path'), keywordId), params=kwargs)
 
     @sp_endpoint('/v2/sp/campaignNegativeKeywords/extended', method='GET')
+    @Utils.deprecated
     def list_campaign_negative_keywords_extended(self, **kwargs) -> ApiResponse:
         r"""
         list_campaign_negative_keywords_extended(self, \*\*kwargs) -> ApiResponse
 
         Gets a list of campaign negative keywords that have extended data fields.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
@@ -78,14 +82,15 @@
 
             ApiResponse
 
             """
         return self._request(kwargs.pop('path'), params=kwargs)
 
     @sp_endpoint('/v2/sp/campaignNegativeKeywords', method='GET')
+    @Utils.deprecated
     def list_campaign_negative_keywords(self, **kwargs) -> ApiResponse:
         r"""
         list_campaign_negative_keywords(self, \*\*kwargs) -> ApiResponse
 
         Gets a list of campaign negative keywords.
 
             query **startIndex**:*integer* | Optional. 0-indexed record offset for the result set. Default value : 0
@@ -104,14 +109,15 @@
 
             ApiResponse
 
             """
         return self._request(kwargs.pop('path'), params=kwargs)
 
     @sp_endpoint('/v2/sp/campaignNegativeKeywords', method='POST')
+    @Utils.deprecated
     def create_campaign_negative_keywords(self, **kwargs) -> ApiResponse:
         r"""
         create_campaign_negative_keywords(self, \*\*kwargs) -> ApiResponse:
 
         Creates one or more campaign negative keywords.
 
         body: | REQUIRED {'description': 'An array of keyword objects.}'
@@ -125,14 +131,15 @@
 
             ApiResponse
 
         """
         return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
 
     @sp_endpoint('/v2/sp/campaignNegativeKeywords', method='PUT')
+    @Utils.deprecated
     def edit_campaign_negative_keywords(self, **kwargs) -> ApiResponse:
         r"""
         edit_campaign_negative_keywords(self, \*\*kwargs) -> ApiResponse:
 
         Updates one or more campaign negative keywords.
 
         body: | REQUIRED {'description': 'An array of campaign negative keywords with updated values.'}
```

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_negative_keywords_v3.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_keywords_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/campaign_negative_targets.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_targets.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/campaigns.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/campaigns_budget_usage.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns_budget_usage.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/campaigns_v3.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/campaings_optimization.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaings_optimization.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/keywords.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/keywords_v3.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/keywords_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_keywords.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_keywords_v3.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_keywords_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_product_targeting.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/negative_product_targeting_v3.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_product_targeting_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/product_ads.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/product_ads.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/product_ads_v3.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/product_ads_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/product_targeting.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/product_targeting_v3.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/product_targeting_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/ranked_keywords_recommendations.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/ranked_keywords_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/reports.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/snapshots.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/sp/suggested_keywords.py` & `python-amazon-ad-api-0.4.3/ad_api/api/sp/suggested_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/api/validation_configurations.py` & `python-amazon-ad-api-0.4.3/ad_api/api/validation_configurations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/auth/access_token_client.py` & `python-amazon-ad-api-0.4.3/ad_api/auth/access_token_client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/base/__init__.py` & `python-amazon-ad-api-0.4.3/ad_api/base/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/base/api_response.py` & `python-amazon-ad-api-0.4.3/ad_api/base/api_response.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/base/base_client.py` & `python-amazon-ad-api-0.4.3/ad_api/base/base_client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/base/client.py` & `python-amazon-ad-api-0.4.3/ad_api/base/client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/base/config.py` & `python-amazon-ad-api-0.4.3/ad_api/base/config.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/base/credential_provider.py` & `python-amazon-ad-api-0.4.3/ad_api/base/credential_provider.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/base/exceptions.py` & `python-amazon-ad-api-0.4.3/ad_api/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/base/helpers.py` & `python-amazon-ad-api-0.4.3/ad_api/base/helpers.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/base/marketplaces.py` & `python-amazon-ad-api-0.4.3/ad_api/base/marketplaces.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/ad_api/base/utils.py` & `python-amazon-ad-api-0.4.3/ad_api/base/utils.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/PKG-INFO` & `python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: python-amazon-ad-api
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python wrapper for the Amazon Advertising API
 Home-page: https://github.com/denisneuf/python-amazon-ad-api
 Author: Daniel Alvaro
 Author-email: info@leadtech.es
 License: MIT
 Project-URL: Bug Tracker, https://github.com/denisneuf/python-amazon-ad-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PYTHON-AMAZON-AD-API
 
-![CodeQL](https://img.shields.io/badge/coverage-90%25-green)
+![CodeQL](https://img.shields.io/badge/coverage-95%25-green)
 ![CodeQL](https://img.shields.io/badge/Docs-sphinx-green)
 ![CodeQL](https://img.shields.io/github/v/release/denisneuf/python-amazon-ad-api)
 [![Documentation Status](https://readthedocs.org/projects/python-amazon-ad-api/badge/?version=latest)](https://python-amazon-ad-api.readthedocs.io/en/latest/?badge=latest)
 
 
 ## Amazon's Advertising API
 
@@ -234,58 +234,48 @@
 
 ### [Modules Available Common Resources](https://python-amazon-ad-api.readthedocs.io/en/latest/api.html)
 
 * [Profiles](https://python-amazon-ad-api.readthedocs.io/en/latest/api/profiles.html)
 * [Manager Accounts](https://python-amazon-ad-api.readthedocs.io/en/latest/api/manager_accounts.html)
 * [Portfolios](https://python-amazon-ad-api.readthedocs.io/en/latest/api/portfolios.html)
 * [Invoices](https://python-amazon-ad-api.readthedocs.io/en/latest/api/invoices.html)
-* Billing
+* [Billing](https://python-amazon-ad-api.readthedocs.io/en/latest/api/billing.html)
 * [Audiences](https://python-amazon-ad-api.readthedocs.io/en/latest/api/audiences.html)
 * [Change History open Beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/history.html)
 * [Creative Assets open Beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api//creative_assets.html)
 * [Elegibility](https://python-amazon-ad-api.readthedocs.io/en/latest/api/eligibility.html)
 * [Insights](https://python-amazon-ad-api.readthedocs.io/en/latest/api/insights.html)
 * [Localization](https://python-amazon-ad-api.readthedocs.io/en/latest/api/localization.html)
 * [Product Selector](https://python-amazon-ad-api.readthedocs.io/en/latest/api/metadata.html)
-* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/reports.html)
 * [Validation Configurations](https://python-amazon-ad-api.readthedocs.io/en/latest/api/validation_configurations.html)
+* [Tactical recommendations beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/recommendations.html)
 
 
-### Amazon Attribution open beta
-* Advertisers
-* Publishers
-* Attribution tags
-* Reports
+### [Amazon Attribution open beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html)
+* [Advertisers](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_advertisers)
+* [Publishers](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_publishers)
+* [Macro tags](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_macro_tag)
+* [Non Macro tags](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.get_non_macro_template_tag)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/attribution.html#ad_api.api.Attribution.Attribution.post_report)
 
 ### [Brand Metrics open beta](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html)
 * [Post Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.post_report)
 * [Get Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.get_report)
 * [Download Report](https://python-amazon-ad-api.readthedocs.io/en/latest/api/brand_metrics.html#ad_api.api.BrandMetrics.BrandMetrics.download_report)
 
 ### [Advertising Test Account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html)
 * [Create test account](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount)
 * [Get test account information](https://python-amazon-ad-api.readthedocs.io/en/latest/api/advertising_test_account.html#ad_api.api.AdvertisingTestAccount.AdvertisingTestAccount.get_test_account)
 
+
 ### [Modules Available Sponsored Products 2.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v2.html)
 
 Warning: [PLANNED DEPRECATION 6/30/2023]
 There is a new version 3 of Sponsored Product API, please check the [migration guide](https://advertising.amazon.com/API/docs/en-us/sponsored-products/v3-migration-guide).
 
-* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns.html)
-* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups.html)
-* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations.html)
-* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords.html)
-* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_keywords.html)
-* [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords.html)
-* [Suggested Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/suggested_keywords.html)
-* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_ads.html)
-* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/product_targeting.html)
-* [Negative Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/negative_product_targeting.html)
-* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/reports.html)
-* [Snapshots](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/snapshots.html)
 
 ### [Modules Available Sponsored Products 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sp_v3.html)
 
 
 * [ThemeBased Bid Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/bid_recommendations_v3.html)
 * [Keyword Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ranked_keywords_recommendations.html)
 * [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/keywords_v3.html)
@@ -300,51 +290,57 @@
 * [Budget Rules Recommendation](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_rules_recommendations.html)
 * [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaignsv3.html)
 * [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/ad_groups_v3.html)
 * [Consolidated Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaigns_consolidated_recommendations.html)
 * [Campaign Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_negative_keywords_v3.html)
 * [Product Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_recommendations.html)
 * [Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_budget_usage.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/reports.html)
 
 
-### Modules Available Sponsored Brands 3.0
+### [Modules Available Sponsored Brands 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v3.html)
 
-* Campaigns
-* Ad Groups
-* Keywords
-* Negative Keywords
-* Product Targeting
-* Negative Product Targeting
-* Targeting Recommendations
-* Bid Recommendations
-* Stores
-* Landing Page Asins
-* Media
-* Brands
-* Moderation
-* Reports
+* Campaigns(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns.html)
+* Ad Groups(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups.html)
+* Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/keywords.html)
+* Negative Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_keywords.html)
+* Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/product_targeting.html)
+* Negative Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_product_targeting.html)
+* Targeting Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/targeting_recommendations.html)
+* Bid Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/bid_recommendations.html)
+* Stores(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/stores.html)
+* Landing Page Asins(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/landing_page_asins.html)
+* Media(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/media.html)
+* Brands(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/brands.html)
+* Moderation(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/moderation.html)
+* Reports(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/reports.html)
 * Snapshots
 
-### Modules Available Sponsored Brands 4.0
+### [Modules Available Sponsored Brands 4.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v4.html)
 
 * [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns_v4.html)
 * [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups_v4.html)
 * [Ads Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ads_v4.html)
 
-### Modules Available Sponsored Display
+### [Modules Available Sponsored Display](https://python-amazon-ad-api.readthedocs.io/en/latest/sd.html)
 
-* Campaigns
-* Ad Groups
-* Reports
-* Product Ads
-* Targets
-* Negative Targets
-* Targets Recommendations
-* Bid Recommendations
-* Creatives
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/campaigns.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/ad_groups.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/reports.html)
+* [Product Ads](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/product_ads.html)
+* [Targets](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/product_targeting.html)
+* [Negative Targets](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/negative_product_targeting.html)
+* [Targets Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/targeting_recommendations.html)
+* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/bid_recommendations.html)
+* [Creatives](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/creatives.html)
+* [Brand Safety List](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/brand_safety.html)
+* [Budget Rules](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/budget_rules.html)
+* [Campaigns Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/campaign_budget_usage.html)
+* [Forecasts](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/forecast.html)
+* [Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/recommendations.html)
 
 ### Modules Available DSP
 
 * Reports
 
 ### Simple Example Usage Campaigns with Credentials
```

### Comparing `python-amazon-ad-api-0.4.2/python_amazon_ad_api.egg-info/SOURCES.txt` & `python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ad_api/api/insights.py
 ad_api/api/invoices.py
 ad_api/api/localization.py
 ad_api/api/manager_accounts.py
 ad_api/api/metadata.py
 ad_api/api/portfolios.py
 ad_api/api/profiles.py
+ad_api/api/recommendations.py
 ad_api/api/reports.py
 ad_api/api/validation_configurations.py
 ad_api/api/dsp/__init__.py
 ad_api/api/dsp/access_token_client.py
 ad_api/api/dsp/client.py
 ad_api/api/dsp/credential_provider.py
 ad_api/api/dsp/reports.py
@@ -48,19 +49,24 @@
 ad_api/api/sb/reports.py
 ad_api/api/sb/snapshots.py
 ad_api/api/sb/stores.py
 ad_api/api/sb/targeting_recommendations.py
 ad_api/api/sd/__init__.py
 ad_api/api/sd/ad_groups.py
 ad_api/api/sd/bid_recommendations.py
+ad_api/api/sd/brand_safety.py
+ad_api/api/sd/budget_rules.py
 ad_api/api/sd/campaigns.py
+ad_api/api/sd/campaigns_budget_usage.py
 ad_api/api/sd/creatives.py
+ad_api/api/sd/forecast.py
 ad_api/api/sd/negative_product_targeting.py
 ad_api/api/sd/product_ads.py
 ad_api/api/sd/product_targeting.py
+ad_api/api/sd/recommendations.py
 ad_api/api/sd/reports.py
 ad_api/api/sd/snapshots.py
 ad_api/api/sd/targeting_recommendations.py
 ad_api/api/sp/__init__.py
 ad_api/api/sp/ad_groups.py
 ad_api/api/sp/ad_groups_v3.py
 ad_api/api/sp/bid_recommendations.py
```

### Comparing `python-amazon-ad-api-0.4.2/setup.cfg` & `python-amazon-ad-api-0.4.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-amazon-ad-api
-version = 0.4.2
+version = 0.4.3
 author = Daniel Alvaro
 author_email = denisneuf@hotmail.com
 description = Python wrapper for the Amazon Advertising API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/denisneuf/python-amazon-ad-api
 project_urls =
```

### Comparing `python-amazon-ad-api-0.4.2/setup.py` & `python-amazon-ad-api-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='python-amazon-ad-api',
-    version='0.4.2',
+    version='0.4.3',
     install_requires=[
         "requests>=2.27.1,<2.29.0",
         "six~=1.16.0",
         "cachetools>=5.0,<5.4",
         "pycryptodome>=3.13,<3.18",
         "python-dotenv>=0.19.2,<1.1.0",
         "pytz>=2021.3,<2024.0",
```

