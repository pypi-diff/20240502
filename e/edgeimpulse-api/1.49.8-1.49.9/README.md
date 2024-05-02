# Comparing `tmp/edgeimpulse_api-1.49.8.tar.gz` & `tmp/edgeimpulse_api-1.49.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse_api-1.49.8.tar", max compression
+gzip compressed data, was "edgeimpulse_api-1.49.9.tar", max compression
```

## Comparing `edgeimpulse_api-1.49.8.tar` & `edgeimpulse_api-1.49.9.tar`

### file list

```diff
@@ -1,925 +1,925 @@
--rw-r--r--   0        0        0      377 2024-04-16 20:23:18.641007 edgeimpulse_api-1.49.8/README.md
--rw-r--r--   0        0        0    88508 2024-04-16 20:23:51.496719 edgeimpulse_api-1.49.8/edgeimpulse_api/__init__.py
--rw-r--r--   0        0        0     2172 2024-04-16 20:23:18.641007 edgeimpulse_api-1.49.8/edgeimpulse_api/api/__init__.py
--rw-r--r--   0        0        0   386649 2024-04-16 20:23:18.645007 edgeimpulse_api-1.49.8/edgeimpulse_api/api/admin_api.py
--rw-r--r--   0        0        0    11231 2024-04-16 20:23:18.645007 edgeimpulse_api-1.49.8/edgeimpulse_api/api/auth_api.py
--rw-r--r--   0        0        0     6235 2024-04-16 20:23:18.645007 edgeimpulse_api-1.49.8/edgeimpulse_api/api/cdn_api.py
--rw-r--r--   0        0        0    59980 2024-04-16 20:23:18.649006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/classify_api.py
--rw-r--r--   0        0        0    72480 2024-04-16 20:23:18.649006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/deployment_api.py
--rw-r--r--   0        0        0    80789 2024-04-16 20:23:18.649006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/devices_api.py
--rw-r--r--   0        0        0   139045 2024-04-16 20:23:18.653006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/dsp_api.py
--rw-r--r--   0        0        0    19442 2024-04-16 20:23:18.653006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/email_verification_api.py
--rw-r--r--   0        0        0     6435 2024-04-16 20:23:18.653006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/export_api.py
--rw-r--r--   0        0        0     5996 2024-04-16 20:23:18.653006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/feature_flags_api.py
--rw-r--r--   0        0        0    11921 2024-04-16 20:23:18.653006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/health_api.py
--rw-r--r--   0        0        0    49621 2024-04-16 20:23:18.653006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/impulse_api.py
--rw-r--r--   0        0        0   238420 2024-04-16 20:23:18.653006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/jobs_api.py
--rw-r--r--   0        0        0   154112 2024-04-16 20:23:18.653006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/learn_api.py
--rw-r--r--   0        0        0     6483 2024-04-16 20:23:18.653006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/login_api.py
--rw-r--r--   0        0        0    17897 2024-04-16 20:23:18.653006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/metrics_api.py
--rw-r--r--   0        0        0    85275 2024-04-16 20:23:18.653006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/optimization_api.py
--rw-r--r--   0        0        0   197840 2024-04-16 20:23:18.657006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_blocks_api.py
--rw-r--r--   0        0        0    92715 2024-04-16 20:23:18.657006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_create_project_api.py
--rw-r--r--   0        0        0   331750 2024-04-16 20:23:18.657006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_data_api.py
--rw-r--r--   0        0        0    80882 2024-04-16 20:23:18.657006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_data_campaigns_api.py
--rw-r--r--   0        0        0    58218 2024-04-16 20:23:18.661006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_jobs_api.py
--rw-r--r--   0        0        0    53291 2024-04-16 20:23:18.661006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_pipelines_api.py
--rw-r--r--   0        0        0    45490 2024-04-16 20:23:18.661006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_portals_api.py
--rw-r--r--   0        0        0   505317 2024-04-16 20:23:18.661006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/organizations_api.py
--rw-r--r--   0        0        0    60377 2024-04-16 20:23:18.665006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/performance_calibration_api.py
--rw-r--r--   0        0        0   270960 2024-04-16 20:23:18.669006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/projects_api.py
--rw-r--r--   0        0        0   414581 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/raw_data_api.py
--rw-r--r--   0        0        0    35671 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/themes_api.py
--rw-r--r--   0        0        0    43486 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/third_party_auth_api.py
--rw-r--r--   0        0        0    45692 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/upload_portal_api.py
--rw-r--r--   0        0        0   247228 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/user_api.py
--rw-r--r--   0        0        0    42135 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/api/whitelabels_api.py
--rw-r--r--   0        0        0    29331 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/api_client.py
--rw-r--r--   0        0        0    15659 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/configuration.py
--rw-r--r--   0        0        0     5113 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/exceptions.py
--rw-r--r--   0        0        0    85883 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/__init__.py
--rw-r--r--   0        0        0     2897 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
--rw-r--r--   0        0        0     1982 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/activate_user_or_verify_email_request.py
--rw-r--r--   0        0        0     2052 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_api_key_request.py
--rw-r--r--   0        0        0     1963 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_collaborator_request.py
--rw-r--r--   0        0        0     2223 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_hmac_key_request.py
--rw-r--r--   0        0        0     2299 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_member_request.py
--rw-r--r--   0        0        0     2418 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_api_key_request.py
--rw-r--r--   0        0        0     2122 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_api_key_request_all_of.py
--rw-r--r--   0        0        0     2806 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_bucket_request.py
--rw-r--r--   0        0        0     2794 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     2469 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2152 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     4230 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2359 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2042 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
--rw-r--r--   0        0        0     2269 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2816 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2248 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2054 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_secret_request.py
--rw-r--r--   0        0        0     2266 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_secret_response.py
--rw-r--r--   0        0        0     1949 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_secret_response_all_of.py
--rw-r--r--   0        0        0     4885 2024-04-16 20:23:18.673006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     2339 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     6169 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_transformation_block_request.py
--rw-r--r--   0        0        0     2325 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2001 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     2659 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_project_api_key_request.py
--rw-r--r--   0        0        0     2370 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_project_api_key_request_all_of.py
--rw-r--r--   0        0        0     1940 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
--rw-r--r--   0        0        0     1961 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
--rw-r--r--   0        0        0     2661 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_organization_api_key_request.py
--rw-r--r--   0        0        0     2542 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_organization_user_request.py
--rw-r--r--   0        0        0     2246 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
--rw-r--r--   0        0        0     2344 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_project_api_key_request.py
--rw-r--r--   0        0        0     2044 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py
--rw-r--r--   0        0        0     2146 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_project_user_request.py
--rw-r--r--   0        0        0     2097 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_user_request.py
--rw-r--r--   0        0        0     5903 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_api_organization.py
--rw-r--r--   0        0        0     2396 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_api_organization_all_of.py
--rw-r--r--   0        0        0     3259 2024-04-16 20:23:18.677006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_api_project.py
--rw-r--r--   0        0        0     7087 2024-04-16 20:23:18.681006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_api_user.py
--rw-r--r--   0        0        0     5318 2024-04-16 20:23:18.681006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_api_user_all_of.py
--rw-r--r--   0        0        0     2386 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_create_organization_data_export_request.py
--rw-r--r--   0        0        0     2262 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_create_organization_request.py
--rw-r--r--   0        0        0     2718 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_create_project_request.py
--rw-r--r--   0        0        0     1905 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_enable_feature_request.py
--rw-r--r--   0        0        0     2546 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_data_migration_response.py
--rw-r--r--   0        0        0     2222 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
--rw-r--r--   0        0        0     2735 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_data_migrations_response.py
--rw-r--r--   0        0        0     2428 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
--rw-r--r--   0        0        0     2318 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
--rw-r--r--   0        0        0     2022 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
--rw-r--r--   0        0        0     2217 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_metrics_response.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
--rw-r--r--   0        0        0     3148 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py
--rw-r--r--   0        0        0     2647 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organization_usage_report_response.py
--rw-r--r--   0        0        0     2323 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py
--rw-r--r--   0        0        0     3029 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py
--rw-r--r--   0        0        0     2729 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py
--rw-r--r--   0        0        0     3046 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organizations_response.py
--rw-r--r--   0        0        0     2746 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
--rw-r--r--   0        0        0     3409 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
--rw-r--r--   0        0        0     2243 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
--rw-r--r--   0        0        0     1947 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
--rw-r--r--   0        0        0     2914 2024-04-16 20:23:18.685006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_sso_settings_response.py
--rw-r--r--   0        0        0     2614 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
--rw-r--r--   0        0        0     2096 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
--rw-r--r--   0        0        0     2208 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_ids_response.py
--rw-r--r--   0        0        0     1901 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
--rw-r--r--   0        0        0     2245 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_metrics_response.py
--rw-r--r--   0        0        0     2452 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_response.py
--rw-r--r--   0        0        0     2128 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_response_all_of.py
--rw-r--r--   0        0        0     2507 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_trial_response.py
--rw-r--r--   0        0        0     2183 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
--rw-r--r--   0        0        0     2807 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_users_response.py
--rw-r--r--   0        0        0     2500 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_users_response_all_of.py
--rw-r--r--   0        0        0     2878 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
--rw-r--r--   0        0        0     2445 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_list_projects.py
--rw-r--r--   0        0        0     2836 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_list_projects_response.py
--rw-r--r--   0        0        0     4245 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_organization_info_response.py
--rw-r--r--   0        0        0     3084 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_organization_info_response_all_of.py
--rw-r--r--   0        0        0     2158 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_toggle_data_migration_request.py
--rw-r--r--   0        0        0     2397 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_update_organization_data_export_request.py
--rw-r--r--   0        0        0     3936 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_update_organization_request.py
--rw-r--r--   0        0        0     2015 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_update_user_permissions_request.py
--rw-r--r--   0        0        0     2830 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_update_user_request.py
--rw-r--r--   0        0        0     2532 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_update_user_trial_request.py
--rw-r--r--   0        0        0     2525 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/akida_edge_learning_config.py
--rw-r--r--   0        0        0      512 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_capacity.py
--rw-r--r--   0        0        0     2512 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_gmm_metadata.py
--rw-r--r--   0        0        0     2212 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py
--rw-r--r--   0        0        0     5499 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_model_metadata.py
--rw-r--r--   0        0        0     5221 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
--rw-r--r--   0        0        0     2151 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
--rw-r--r--   0        0        0     4079 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_response.py
--rw-r--r--   0        0        0     3812 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_response_all_of.py
--rw-r--r--   0        0        0     2044 2024-04-16 20:23:18.689006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_response_all_of_axes.py
--rw-r--r--   0        0        0     3188 2024-04-16 20:23:18.693006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_result.py
--rw-r--r--   0        0        0     3029 2024-04-16 20:23:18.693006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_trained_features_response.py
--rw-r--r--   0        0        0     2729 2024-04-16 20:23:18.693006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2375 2024-04-16 20:23:18.693006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     3358 2024-04-16 20:23:18.693006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/application_budget.py
--rw-r--r--   0        0        0      506 2024-04-16 20:23:18.693006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/augmentation_policy_image_enum.py
--rw-r--r--   0        0        0     3635 2024-04-16 20:23:18.693006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/augmentation_policy_spectrogram.py
--rw-r--r--   0        0        0     1895 2024-04-16 20:23:18.693006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/autotune_dsp_request.py
--rw-r--r--   0        0        0      505 2024-04-16 20:23:18.697006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/block_display_category.py
--rw-r--r--   0        0        0      560 2024-04-16 20:23:18.697006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/block_type.py
--rw-r--r--   0        0        0     2044 2024-04-16 20:23:18.697006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/bounding_box.py
--rw-r--r--   0        0        0     2151 2024-04-16 20:23:18.697006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/bounding_box_with_score.py
--rw-r--r--   0        0        0     2197 2024-04-16 20:23:18.697006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/build_on_device_model_request.py
--rw-r--r--   0        0        0     2433 2024-04-16 20:23:18.697006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/build_organization_on_device_model_request.py
--rw-r--r--   0        0        0     2459 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
--rw-r--r--   0        0        0     2041 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/change_password_request.py
--rw-r--r--   0        0        0     3701 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response.py
--rw-r--r--   0        0        0     3394 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response_all_of.py
--rw-r--r--   0        0        0     3769 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
--rw-r--r--   0        0        0     2055 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
--rw-r--r--   0        0        0     3255 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response_page.py
--rw-r--r--   0        0        0     2948 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response_page_all_of.py
--rw-r--r--   0        0        0     4026 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_sample_response.py
--rw-r--r--   0        0        0     3759 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_sample_response_all_of.py
--rw-r--r--   0        0        0     6252 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_sample_response_classification.py
--rw-r--r--   0        0        0     2755 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_sample_response_classification_details.py
--rw-r--r--   0        0        0     3816 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_sample_v2200_response.py
--rw-r--r--   0        0        0     3004 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/convert_user_request.py
--rw-r--r--   0        0        0     3495 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/cosine_similarity_data.py
--rw-r--r--   0        0        0     3114 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/cosine_similarity_issue.py
--rw-r--r--   0        0        0     3241 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py
--rw-r--r--   0        0        0     2484 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py
--rw-r--r--   0        0        0     2183 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/count_samples_response.py
--rw-r--r--   0        0        0     1859 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/count_samples_response_all_of.py
--rw-r--r--   0        0        0     2255 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_block_version_response.py
--rw-r--r--   0        0        0     1938 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_block_version_response_all_of.py
--rw-r--r--   0        0        0     2404 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_developer_profile_response.py
--rw-r--r--   0        0        0     2125 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_developer_profile_response_all_of.py
--rw-r--r--   0        0        0     2387 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_device_request.py
--rw-r--r--   0        0        0     2850 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_enterprise_trial_response.py
--rw-r--r--   0        0        0     2319 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py
--rw-r--r--   0        0        0     6569 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_enterprise_trial_user_request.py
--rw-r--r--   0        0        0     4092 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py
--rw-r--r--   0        0        0     2491 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_evaluation_user_response.py
--rw-r--r--   0        0        0     2185 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
--rw-r--r--   0        0        0     2600 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_portal_request.py
--rw-r--r--   0        0        0     2830 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_portal_response.py
--rw-r--r--   0        0        0     2551 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     1990 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_request.py
--rw-r--r--   0        0        0     2454 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_response.py
--rw-r--r--   0        0        0     2148 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_response_all_of.py
--rw-r--r--   0        0        0     2155 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_usage_report_body.py
--rw-r--r--   0        0        0     2185 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_pipeline_response.py
--rw-r--r--   0        0        0     2504 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_project_request.py
--rw-r--r--   0        0        0     2378 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_project_response.py
--rw-r--r--   0        0        0     2072 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_project_response_all_of.py
--rw-r--r--   0        0        0     2276 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_signed_upload_link_request.py
--rw-r--r--   0        0        0     2414 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_signed_upload_link_response.py
--rw-r--r--   0        0        0     2135 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
--rw-r--r--   0        0        0     2413 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_third_party_auth_request.py
--rw-r--r--   0        0        0     2450 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_third_party_auth_response.py
--rw-r--r--   0        0        0     2144 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     4197 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_request.py
--rw-r--r--   0        0        0     2393 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_response.py
--rw-r--r--   0        0        0     2114 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_response_all_of.py
--rw-r--r--   0        0        0     2919 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_third_party_request.py
--rw-r--r--   0        0        0     2672 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_third_party_response.py
--rw-r--r--   0        0        0     2393 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_third_party_response_all_of.py
--rw-r--r--   0        0        0     4384 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_whitelabel_request.py
--rw-r--r--   0        0        0     2438 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_whitelabel_response.py
--rw-r--r--   0        0        0     2121 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2094 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/created_updated_by_user.py
--rw-r--r--   0        0        0     2051 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/crop_sample_request.py
--rw-r--r--   0        0        0     2248 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/crop_sample_response.py
--rw-r--r--   0        0        0     1943 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/crop_sample_response_all_of.py
--rw-r--r--   0        0        0     2368 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/cross_validation_data.py
--rw-r--r--   0        0        0     3412 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/cross_validation_data_scores_inner.py
--rw-r--r--   0        0        0     4054 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign.py
--rw-r--r--   0        0        0     2989 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_dashboard.py
--rw-r--r--   0        0        0     2786 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_graph.py
--rw-r--r--   0        0        0     3352 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
--rw-r--r--   0        0        0     2047 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
--rw-r--r--   0        0        0     1934 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_link.py
--rw-r--r--   0        0        0     1957 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_query.py
--rw-r--r--   0        0        0     3292 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_explorer_predictions_response.py
--rw-r--r--   0        0        0     3003 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
--rw-r--r--   0        0        0     2838 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_explorer_settings.py
--rw-r--r--   0        0        0     2149 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dataset_ratio_data.py
--rw-r--r--   0        0        0     2111 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dataset_ratio_data_ratio.py
--rw-r--r--   0        0        0     1898 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/delete_portal_file_request.py
--rw-r--r--   0        0        0     2230 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dependency_data.py
--rw-r--r--   0        0        0     2280 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
--rw-r--r--   0        0        0     2408 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
--rw-r--r--   0        0        0     2155 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
--rw-r--r--   0        0        0     2484 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
--rw-r--r--   0        0        0     2344 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
--rw-r--r--   0        0        0     2780 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
--rw-r--r--   0        0        0     2200 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
--rw-r--r--   0        0        0     4397 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_request.py
--rw-r--r--   0        0        0     2833 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
--rw-r--r--   0        0        0     8503 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
--rw-r--r--   0        0        0     8065 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
--rw-r--r--   0        0        0     5950 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deployment_target.py
--rw-r--r--   0        0        0     1926 2024-04-16 20:23:18.701006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deployment_target_badge.py
--rw-r--r--   0        0        0      737 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deployment_target_engine.py
--rw-r--r--   0        0        0     2702 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deployment_targets_response.py
--rw-r--r--   0        0        0     2395 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     2248 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_board_created_response.py
--rw-r--r--   0        0        0     2032 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_board_request.py
--rw-r--r--   0        0        0     2134 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_board_request_update.py
--rw-r--r--   0        0        0     2113 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_board_response.py
--rw-r--r--   0        0        0     2864 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_boards_response.py
--rw-r--r--   0        0        0     2564 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_boards_response_all_of.py
--rw-r--r--   0        0        0     2030 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_keys.py
--rw-r--r--   0        0        0     2400 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_keys_response.py
--rw-r--r--   0        0        0     4816 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/device.py
--rw-r--r--   0        0        0      516 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/device_debug_stream_type.py
--rw-r--r--   0        0        0     2811 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/device_inference_info.py
--rw-r--r--   0        0        0     2199 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/device_name_response.py
--rw-r--r--   0        0        0     1920 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/device_name_response_all_of.py
--rw-r--r--   0        0        0     2231 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/device_sensors_inner.py
--rw-r--r--   0        0        0     2094 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/download.py
--rw-r--r--   0        0        0     1912 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/download_portal_file_request.py
--rw-r--r--   0        0        0     2260 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/download_portal_file_response.py
--rw-r--r--   0        0        0     1954 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/download_portal_file_response_all_of.py
--rw-r--r--   0        0        0     2724 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_autotuner_results.py
--rw-r--r--   0        0        0     2417 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
--rw-r--r--   0        0        0     1968 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
--rw-r--r--   0        0        0     3660 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_block.py
--rw-r--r--   0        0        0     1834 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_config_request.py
--rw-r--r--   0        0        0     3092 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_config_response.py
--rw-r--r--   0        0        0     2813 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_config_response_all_of.py
--rw-r--r--   0        0        0     3016 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_importance_response.py
--rw-r--r--   0        0        0     2728 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
--rw-r--r--   0        0        0     2058 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
--rw-r--r--   0        0        0     2572 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
--rw-r--r--   0        0        0     2216 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_labels_response.py
--rw-r--r--   0        0        0     1920 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
--rw-r--r--   0        0        0     2294 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_group.py
--rw-r--r--   0        0        0     4216 2024-04-16 20:23:18.705006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_group_item.py
--rw-r--r--   0        0        0     2190 2024-04-16 20:23:18.709006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
--rw-r--r--   0        0        0     2195 2024-04-16 20:23:18.709006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_group_item_show_if.py
--rw-r--r--   0        0        0     4848 2024-04-16 20:23:18.709006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_info.py
--rw-r--r--   0        0        0     2376 2024-04-16 20:23:18.709006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_info_features.py
--rw-r--r--   0        0        0     1885 2024-04-16 20:23:18.709006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_info_performance.py
--rw-r--r--   0        0        0     5462 2024-04-16 20:23:18.709006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_metadata.py
--rw-r--r--   0        0        0     2025 2024-04-16 20:23:18.709006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
--rw-r--r--   0        0        0     2566 2024-04-16 20:23:18.709006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_metadata_output_config.py
--rw-r--r--   0        0        0     2531 2024-04-16 20:23:18.709006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
--rw-r--r--   0        0        0     5820 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_metadata_response.py
--rw-r--r--   0        0        0     1963 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_named_axis.py
--rw-r--r--   0        0        0     3019 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_performance_all_variants_response.py
--rw-r--r--   0        0        0     2729 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2278 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
--rw-r--r--   0        0        0     4639 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_graph.py
--rw-r--r--   0        0        0     1899 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
--rw-r--r--   0        0        0     2677 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_request_with_features.py
--rw-r--r--   0        0        0     2151 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_request_without_features.py
--rw-r--r--   0        0        0     2030 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
--rw-r--r--   0        0        0     3697 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_response.py
--rw-r--r--   0        0        0     3418 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_response_all_of.py
--rw-r--r--   0        0        0     1969 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
--rw-r--r--   0        0        0     4579 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_response_with_sample.py
--rw-r--r--   0        0        0     4312 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
--rw-r--r--   0        0        0     3342 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_sample_features_response.py
--rw-r--r--   0        0        0     3042 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
--rw-r--r--   0        0        0     2748 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
--rw-r--r--   0        0        0     2213 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
--rw-r--r--   0        0        0     3353 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_trained_features_response.py
--rw-r--r--   0        0        0     3053 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2773 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     2205 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
--rw-r--r--   0        0        0     1893 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/edit_sample_label_request.py
--rw-r--r--   0        0        0     4246 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/enterprise_trial.py
--rw-r--r--   0        0        0     2960 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py
--rw-r--r--   0        0        0     2885 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/entitlement_limits.py
--rw-r--r--   0        0        0     2367 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/entity_created_response.py
--rw-r--r--   0        0        0     2077 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/entity_created_response_all_of.py
--rw-r--r--   0        0        0     2656 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/evaluate_job_response.py
--rw-r--r--   0        0        0     2349 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/evaluate_job_response_all_of.py
--rw-r--r--   0        0        0     2099 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/evaluate_result_value.py
--rw-r--r--   0        0        0     2366 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_block_response.py
--rw-r--r--   0        0        0     2060 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_block_response_all_of.py
--rw-r--r--   0        0        0     2511 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_get_url_response.py
--rw-r--r--   0        0        0     2244 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_get_url_response_all_of.py
--rw-r--r--   0        0        0     2116 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_keras_block_data_request.py
--rw-r--r--   0        0        0     2373 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_original_data_request.py
--rw-r--r--   0        0        0     2021 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_wav_data_request.py
--rw-r--r--   0        0        0      500 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/feature.py
--rw-r--r--   0        0        0     2206 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_segment_sample_request.py
--rw-r--r--   0        0        0     2804 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_segment_sample_response.py
--rw-r--r--   0        0        0     2497 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_segment_sample_response_all_of.py
--rw-r--r--   0        0        0     2090 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
--rw-r--r--   0        0        0     2665 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_user_response.py
--rw-r--r--   0        0        0     2358 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_user_response_all_of.py
--rw-r--r--   0        0        0     2322 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_user_response_all_of_users.py
--rw-r--r--   0        0        0     2507 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/generate_features_request.py
--rw-r--r--   0        0        0     2083 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/generic_api_response.py
--rw-r--r--   0        0        0     2764 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_imported_from_response.py
--rw-r--r--   0        0        0     2457 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
--rw-r--r--   0        0        0     2156 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
--rw-r--r--   0        0        0     2698 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_third_party_auth_response.py
--rw-r--r--   0        0        0     2391 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     2713 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_whitelabels_response.py
--rw-r--r--   0        0        0     2406 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
--rw-r--r--   0        0        0     3527 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_auto_labeler_response.py
--rw-r--r--   0        0        0     3260 2024-04-16 20:23:18.713006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_auto_labeler_response_all_of.py
--rw-r--r--   0        0        0     2588 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py
--rw-r--r--   0        0        0     1954 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py
--rw-r--r--   0        0        0     2345 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py
--rw-r--r--   0        0        0     2078 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py
--rw-r--r--   0        0        0     3400 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_data_explorer_features_response.py
--rw-r--r--   0        0        0     3122 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0     3752 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_data_explorer_settings_response.py
--rw-r--r--   0        0        0     2402 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
--rw-r--r--   0        0        0     2349 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_deployment_response.py
--rw-r--r--   0        0        0     2071 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_deployment_response_all_of.py
--rw-r--r--   0        0        0     2434 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_device_response.py
--rw-r--r--   0        0        0     2137 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_device_response_all_of.py
--rw-r--r--   0        0        0     2752 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_diversity_data_response.py
--rw-r--r--   0        0        0     2455 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_diversity_data_response_all_of.py
--rw-r--r--   0        0        0     4251 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
--rw-r--r--   0        0        0     2859 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
--rw-r--r--   0        0        0     2456 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_email_verification_code_response.py
--rw-r--r--   0        0        0     2177 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_email_verification_code_response_all_of.py
--rw-r--r--   0        0        0     2350 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_email_verification_status_response.py
--rw-r--r--   0        0        0     2045 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_email_verification_status_response_all_of.py
--rw-r--r--   0        0        0     2788 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_feature_flags_response.py
--rw-r--r--   0        0        0     2488 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_feature_flags_response_all_of.py
--rw-r--r--   0        0        0     2118 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py
--rw-r--r--   0        0        0     3930 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_blocks_response.py
--rw-r--r--   0        0        0     3630 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
--rw-r--r--   0        0        0     2429 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_records_request.py
--rw-r--r--   0        0        0     2007 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_records_request_range.py
--rw-r--r--   0        0        0     2454 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_response.py
--rw-r--r--   0        0        0     2157 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_response_all_of.py
--rw-r--r--   0        0        0     2374 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_job_response.py
--rw-r--r--   0        0        0     2077 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_job_response_all_of.py
--rw-r--r--   0        0        0     3070 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_jwt_request.py
--rw-r--r--   0        0        0     2431 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_jwt_response.py
--rw-r--r--   0        0        0     2152 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_jwt_response_all_of.py
--rw-r--r--   0        0        0     2580 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_label_noise_data_response.py
--rw-r--r--   0        0        0     2256 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_label_noise_data_response_all_of.py
--rw-r--r--   0        0        0     3358 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py
--rw-r--r--   0        0        0     3578 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_last_deployment_build_response.py
--rw-r--r--   0        0        0     3300 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
--rw-r--r--   0        0        0     2869 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
--rw-r--r--   0        0        0     2572 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_notes_response.py
--rw-r--r--   0        0        0     2265 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_notes_response_all_of.py
--rw-r--r--   0        0        0     2556 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_bucket_response.py
--rw-r--r--   0        0        0     2232 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2701 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2377 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     2890 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
--rw-r--r--   0        0        0     2583 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
--rw-r--r--   0        0        0     3158 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2939 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaigns_response.py
--rw-r--r--   0        0        0     2632 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
--rw-r--r--   0        0        0     2921 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
--rw-r--r--   0        0        0     2601 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_export_response.py
--rw-r--r--   0        0        0     2277 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_export_response_all_of.py
--rw-r--r--   0        0        0     2982 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_exports_response.py
--rw-r--r--   0        0        0     2682 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py
--rw-r--r--   0        0        0     2561 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_item_response.py
--rw-r--r--   0        0        0     2237 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
--rw-r--r--   0        0        0     3411 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
--rw-r--r--   0        0        0     3111 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
--rw-r--r--   0        0        0     3532 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
--rw-r--r--   0        0        0     2576 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_dataset_response.py
--rw-r--r--   0        0        0     2252 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
--rw-r--r--   0        0        0     2690 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2373 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py
--rw-r--r--   0        0        0     2627 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2310 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py
--rw-r--r--   0        0        0     2603 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_pipelines_response.py
--rw-r--r--   0        0        0     2279 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     3670 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_portal_response.py
--rw-r--r--   0        0        0     3391 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2323 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_projects_data_count_response.py
--rw-r--r--   0        0        0     2906 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     2589 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py
--rw-r--r--   0        0        0     2858 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2541 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     2612 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_usage_report_response.py
--rw-r--r--   0        0        0     2905 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
--rw-r--r--   0        0        0     2598 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
--rw-r--r--   0        0        0     3012 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
--rw-r--r--   0        0        0     2712 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
--rw-r--r--   0        0        0     2722 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
--rw-r--r--   0        0        0     2425 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
--rw-r--r--   0        0        0     2922 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
--rw-r--r--   0        0        0     2615 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
--rw-r--r--   0        0        0     3151 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_status_response.py
--rw-r--r--   0        0        0     2884 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
--rw-r--r--   0        0        0     3761 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_pretrained_model_response.py
--rw-r--r--   0        0        0     3483 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     4031 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
--rw-r--r--   0        0        0     2978 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
--rw-r--r--   0        0        0     3058 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
--rw-r--r--   0        0        0     2397 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_public_metrics_response.py
--rw-r--r--   0        0        0     2073 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_public_metrics_response_all_of.py
--rw-r--r--   0        0        0     2767 2024-04-16 20:23:18.717006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_sample_metadata_response.py
--rw-r--r--   0        0        0     3044 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_sample_response.py
--rw-r--r--   0        0        0     2462 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_syntiant_posterior_response.py
--rw-r--r--   0        0        0     2184 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
--rw-r--r--   0        0        0     2694 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_target_constraints_response.py
--rw-r--r--   0        0        0     2404 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_target_constraints_response_all_of.py
--rw-r--r--   0        0        0     2414 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_theme_response.py
--rw-r--r--   0        0        0     2117 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_theme_response_all_of.py
--rw-r--r--   0        0        0     2592 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_themes_response.py
--rw-r--r--   0        0        0     2285 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_themes_response_all_of.py
--rw-r--r--   0        0        0     2495 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_third_party_auth_response.py
--rw-r--r--   0        0        0     2171 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     3543 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_user_need_to_set_password_response.py
--rw-r--r--   0        0        0     3276 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
--rw-r--r--   0        0        0     7721 2024-04-16 20:23:18.721006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_user_response.py
--rw-r--r--   0        0        0     5497 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_user_response_all_of.py
--rw-r--r--   0        0        0     2395 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
--rw-r--r--   0        0        0     2307 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_whitelabel_domain_response.py
--rw-r--r--   0        0        0     2021 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
--rw-r--r--   0        0        0     2514 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_whitelabel_response.py
--rw-r--r--   0        0        0     2217 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2776 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/has_data_explorer_features_response.py
--rw-r--r--   0        0        0     2498 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0      580 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/image_input_scaling.py
--rw-r--r--   0        0        0     3738 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse.py
--rw-r--r--   0        0        0     6723 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse_block_version.py
--rw-r--r--   0        0        0     6814 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse_dsp_block.py
--rw-r--r--   0        0        0     1967 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse_dsp_block_organization.py
--rw-r--r--   0        0        0     8958 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse_input_block.py
--rw-r--r--   0        0        0     5612 2024-04-16 20:23:18.725006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse_learn_block.py
--rw-r--r--   0        0        0     2627 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/input_block.py
--rw-r--r--   0        0        0     2323 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/invite_organization_member_request.py
--rw-r--r--   0        0        0     4172 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job.py
--rw-r--r--   0        0        0     2066 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_created_by_user.py
--rw-r--r--   0        0        0     5203 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_details.py
--rw-r--r--   0        0        0     2736 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_details_all_of.py
--rw-r--r--   0        0        0     2613 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_details_response.py
--rw-r--r--   0        0        0     2316 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_details_response_all_of.py
--rw-r--r--   0        0        0     2257 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_failure_details.py
--rw-r--r--   0        0        0     2657 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_logs_response.py
--rw-r--r--   0        0        0     2350 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_logs_response_all_of.py
--rw-r--r--   0        0        0     3297 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_metrics_response.py
--rw-r--r--   0        0        0     3007 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_metrics_response_all_of.py
--rw-r--r--   0        0        0      546 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_parent_type_enum.py
--rw-r--r--   0        0        0     2944 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_state.py
--rw-r--r--   0        0        0     1966 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_state_execution_details.py
--rw-r--r--   0        0        0      598 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_status.py
--rw-r--r--   0        0        0     2965 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_step.py
--rw-r--r--   0        0        0     2713 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_summary_response.py
--rw-r--r--   0        0        0     2406 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_summary_response_all_of.py
--rw-r--r--   0        0        0     2089 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_summary_response_all_of_summary.py
--rw-r--r--   0        0        0     1961 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py
--rw-r--r--   0        0        0     1993 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_custom_metric.py
--rw-r--r--   0        0        0     2510 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_layer.py
--rw-r--r--   0        0        0     2093 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_layer_input.py
--rw-r--r--   0        0        0     2101 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_layer_output.py
--rw-r--r--   0        0        0     5707 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_metadata.py
--rw-r--r--   0        0        0     5440 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_metadata_all_of.py
--rw-r--r--   0        0        0     5421 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_metadata_metrics.py
--rw-r--r--   0        0        0     4495 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
--rw-r--r--   0        0        0     2497 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
--rw-r--r--   0        0        0      562 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_type_enum.py
--rw-r--r--   0        0        0      524 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_variant_enum.py
--rw-r--r--   0        0        0    11377 2024-04-16 20:23:18.729006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_response.py
--rw-r--r--   0        0        0    11110 2024-04-16 20:23:18.733006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_response_all_of.py
--rw-r--r--   0        0        0     3392 2024-04-16 20:23:18.733006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_visual_layer.py
--rw-r--r--   0        0        0     2310 2024-04-16 20:23:18.733006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_visual_layer_type.py
--rw-r--r--   0        0        0     2529 2024-04-16 20:23:18.733006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/last_modification_date_response.py
--rw-r--r--   0        0        0     2239 2024-04-16 20:23:18.733006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/last_modification_date_response_all_of.py
--rw-r--r--   0        0        0     2633 2024-04-16 20:23:18.733006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/latency_device.py
--rw-r--r--   0        0        0     3146 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/learn_block.py
--rw-r--r--   0        0        0      933 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/learn_block_type.py
--rw-r--r--   0        0        0     2788 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_api_keys_response.py
--rw-r--r--   0        0        0     2488 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2704 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2619 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_devices_response.py
--rw-r--r--   0        0        0     2312 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_devices_response_all_of.py
--rw-r--r--   0        0        0     2726 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_email_response.py
--rw-r--r--   0        0        0     2426 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_email_response_all_of.py
--rw-r--r--   0        0        0     2918 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_email_response_all_of_emails.py
--rw-r--r--   0        0        0     2767 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_enterprise_trials_response.py
--rw-r--r--   0        0        0     2467 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py
--rw-r--r--   0        0        0     2813 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_hmac_keys_response.py
--rw-r--r--   0        0        0     2513 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
--rw-r--r--   0        0        0     2381 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
--rw-r--r--   0        0        0     2745 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_jobs_response.py
--rw-r--r--   0        0        0     2445 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_jobs_response_all_of.py
--rw-r--r--   0        0        0     2200 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_models_response.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_models_response_all_of.py
--rw-r--r--   0        0        0     2921 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_api_keys_response.py
--rw-r--r--   0        0        0     2621 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2760 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2752 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_buckets_response.py
--rw-r--r--   0        0        0     2445 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
--rw-r--r--   0        0        0     2902 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_buckets_user_response.py
--rw-r--r--   0        0        0     2595 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
--rw-r--r--   0        0        0     2760 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
--rw-r--r--   0        0        0     3310 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_data_response.py
--rw-r--r--   0        0        0     3031 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_data_response_all_of.py
--rw-r--r--   0        0        0     3430 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
--rw-r--r--   0        0        0     2887 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
--rw-r--r--   0        0        0     2587 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
--rw-r--r--   0        0        0     2824 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
--rw-r--r--   0        0        0     2524 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
--rw-r--r--   0        0        0     3353 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_files_response.py
--rw-r--r--   0        0        0     3074 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_files_response_all_of.py
--rw-r--r--   0        0        0     2792 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_pipelines_response.py
--rw-r--r--   0        0        0     2485 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     2857 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_portals_response.py
--rw-r--r--   0        0        0     2550 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_portals_response_all_of.py
--rw-r--r--   0        0        0     2858 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
--rw-r--r--   0        0        0     3449 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_projects_data_response.py
--rw-r--r--   0        0        0     3142 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
--rw-r--r--   0        0        0     2271 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
--rw-r--r--   0        0        0     2857 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_secrets_response.py
--rw-r--r--   0        0        0     2550 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
--rw-r--r--   0        0        0     2819 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
--rw-r--r--   0        0        0     3103 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
--rw-r--r--   0        0        0     2803 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
--rw-r--r--   0        0        0     3055 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2755 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2988 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_usage_reports_response.py
--rw-r--r--   0        0        0     2688 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py
--rw-r--r--   0        0        0     2786 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organizations_response.py
--rw-r--r--   0        0        0     2486 2024-04-16 20:23:18.737006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organizations_response_all_of.py
--rw-r--r--   0        0        0     2512 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_portal_files_in_folder_request.py
--rw-r--r--   0        0        0     2872 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_portal_files_in_folder_response.py
--rw-r--r--   0        0        0     2593 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2290 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_projects.py
--rw-r--r--   0        0        0     2681 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_projects_response.py
--rw-r--r--   0        0        0     3122 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2822 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2553 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_projects.py
--rw-r--r--   0        0        0     2944 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_projects_response.py
--rw-r--r--   0        0        0     2815 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_versions_response.py
--rw-r--r--   0        0        0     2508 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_versions_response_all_of.py
--rw-r--r--   0        0        0     2290 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2754 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_samples_response.py
--rw-r--r--   0        0        0     2454 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_samples_response_all_of.py
--rw-r--r--   0        0        0     2615 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_tuner_runs_response.py
--rw-r--r--   0        0        0     2308 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_tuner_runs_response_all_of.py
--rw-r--r--   0        0        0     3933 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_versions_response.py
--rw-r--r--   0        0        0     3633 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_versions_response_all_of.py
--rw-r--r--   0        0        0     2353 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
--rw-r--r--   0        0        0     2053 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
--rw-r--r--   0        0        0     3960 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2367 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/log_analytics_event_request.py
--rw-r--r--   0        0        0     2900 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/log_stdout_response.py
--rw-r--r--   0        0        0     2600 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/log_stdout_response_all_of.py
--rw-r--r--   0        0        0     2441 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
--rw-r--r--   0        0        0     2191 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/log_website_pageview_request.py
--rw-r--r--   0        0        0     2217 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/login_response.py
--rw-r--r--   0        0        0     1911 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/login_response_all_of.py
--rw-r--r--   0        0        0     2528 2024-04-16 20:23:18.741006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/memory_spec.py
--rw-r--r--   0        0        0     2746 2024-04-16 20:23:18.745006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/metrics_all_variants_response.py
--rw-r--r--   0        0        0     2449 2024-04-16 20:23:18.745006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/metrics_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2128 2024-04-16 20:23:18.749006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/metrics_for_model_variant.py
--rw-r--r--   0        0        0     2430 2024-04-16 20:23:18.749006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/migration.py
--rw-r--r--   0        0        0      571 2024-04-16 20:23:18.749006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/model_engine_short_enum.py
--rw-r--r--   0        0        0     3010 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/model_prediction.py
--rw-r--r--   0        0        0     2895 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/model_result.py
--rw-r--r--   0        0        0     5046 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/model_variant_stats.py
--rw-r--r--   0        0        0     2128 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/move_raw_data_request.py
--rw-r--r--   0        0        0     2784 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/neighbors_data.py
--rw-r--r--   0        0        0     3584 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/neighbors_score.py
--rw-r--r--   0        0        0     2736 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py
--rw-r--r--   0        0        0     2687 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/note.py
--rw-r--r--   0        0        0     2221 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_auto_label_request.py
--rw-r--r--   0        0        0     2994 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_auto_label_response.py
--rw-r--r--   0        0        0     2705 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
--rw-r--r--   0        0        0     2275 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
--rw-r--r--   0        0        0     2368 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_label_queue_count_response.py
--rw-r--r--   0        0        0     2051 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
--rw-r--r--   0        0        0     2887 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_label_queue_response.py
--rw-r--r--   0        0        0     2580 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
--rw-r--r--   0        0        0      775 2024-04-16 20:23:18.753006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_last_layer.py
--rw-r--r--   0        0        0     6491 2024-04-16 20:23:18.757006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_config.py
--rw-r--r--   0        0        0     6949 2024-04-16 20:23:18.757006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_config_response.py
--rw-r--r--   0        0        0     1920 2024-04-16 20:23:18.757006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_config_response_all_of.py
--rw-r--r--   0        0        0     2056 2024-04-16 20:23:18.757006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_config_target_device.py
--rw-r--r--   0        0        0     2271 2024-04-16 20:23:18.757006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_dsp_parameters_response.py
--rw-r--r--   0        0        0     1964 2024-04-16 20:23:18.757006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
--rw-r--r--   0        0        0     2756 2024-04-16 20:23:18.757006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_space_response.py
--rw-r--r--   0        0        0     2456 2024-04-16 20:23:18.757006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_space_response_all_of.py
--rw-r--r--   0        0        0     5546 2024-04-16 20:23:18.757006 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_state_response.py
--rw-r--r--   0        0        0     5279 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_state_response_all_of.py
--rw-r--r--   0        0        0     3284 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_state_response_all_of_status.py
--rw-r--r--   0        0        0     2273 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
--rw-r--r--   0        0        0     2749 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
--rw-r--r--   0        0        0     2425 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
--rw-r--r--   0        0        0     4717 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
--rw-r--r--   0        0        0     5801 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization.py
--rw-r--r--   0        0        0     2700 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_add_data_folder_request.py
--rw-r--r--   0        0        0     2498 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_add_data_folder_response.py
--rw-r--r--   0        0        0     2209 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
--rw-r--r--   0        0        0     2835 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_add_dataset_request.py
--rw-r--r--   0        0        0     2493 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
--rw-r--r--   0        0        0     2820 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_bucket.py
--rw-r--r--   0        0        0     2711 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_compute_time_usage.py
--rw-r--r--   0        0        0     9492 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project.py
--rw-r--r--   0        0        0      605 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py
--rw-r--r--   0        0        0     2262 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_path_filter.py
--rw-r--r--   0        0        0     7464 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_request.py
--rw-r--r--   0        0        0     2543 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_response.py
--rw-r--r--   0        0        0     2237 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_response_all_of.py
--rw-r--r--   0        0        0     2704 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_status_response.py
--rw-r--r--   0        0        0     2407 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
--rw-r--r--   0        0        0     2754 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_transformation_summary.py
--rw-r--r--   0        0        0    10387 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_with_files.py
--rw-r--r--   0        0        0     2744 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
--rw-r--r--   0        0        0     3483 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
--rw-r--r--   0        0        0     2559 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_campaign_diff_request.py
--rw-r--r--   0        0        0     2327 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
--rw-r--r--   0        0        0     3041 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_campaign_diff_response.py
--rw-r--r--   0        0        0     2741 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
--rw-r--r--   0        0        0     2468 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
--rw-r--r--   0        0        0     3483 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_export.py
--rw-r--r--   0        0        0     3476 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_item.py
--rw-r--r--   0        0        0     2303 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_item_files_inner.py
--rw-r--r--   0        0        0     4007 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_dataset.py
--rw-r--r--   0        0        0     2800 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_dataset_bucket.py
--rw-r--r--   0        0        0     6005 2024-04-16 20:23:18.761005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_deploy_block.py
--rw-r--r--   0        0        0     4962 2024-04-16 20:23:18.765005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_dsp_block.py
--rw-r--r--   0        0        0     3037 2024-04-16 20:23:18.765005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_get_create_projects_response.py
--rw-r--r--   0        0        0     2737 2024-04-16 20:23:18.765005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
--rw-r--r--   0        0        0     7063 2024-04-16 20:23:18.765005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
--rw-r--r--   0        0        0     6864 2024-04-16 20:23:18.765005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response.py
--rw-r--r--   0        0        0     6574 2024-04-16 20:23:18.769005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of.py
--rw-r--r--   0        0        0     3915 2024-04-16 20:23:18.769005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
--rw-r--r--   0        0        0     2267 2024-04-16 20:23:18.769005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
--rw-r--r--   0        0        0     2338 2024-04-16 20:23:18.769005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
--rw-r--r--   0        0        0     2458 2024-04-16 20:23:18.769005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
--rw-r--r--   0        0        0     2101 2024-04-16 20:23:18.769005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of_performance.py
--rw-r--r--   0        0        0      525 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_member_role.py
--rw-r--r--   0        0        0     2639 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_metrics_response.py
--rw-r--r--   0        0        0     2315 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_metrics_response_all_of.py
--rw-r--r--   0        0        0     4480 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
--rw-r--r--   0        0        0     6143 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline.py
--rw-r--r--   0        0        0     2595 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
--rw-r--r--   0        0        0     2275 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
--rw-r--r--   0        0        0     2314 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_item_count.py
--rw-r--r--   0        0        0     4129 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_run.py
--rw-r--r--   0        0        0     5330 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_run_step.py
--rw-r--r--   0        0        0     6532 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_step.py
--rw-r--r--   0        0        0     2351 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
--rw-r--r--   0        0        0     2344 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
--rw-r--r--   0        0        0     2037 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_projects_data_batch_request.py
--rw-r--r--   0        0        0     7242 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_transfer_learning_block.py
--rw-r--r--   0        0        0      611 2024-04-16 20:23:18.773005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
--rw-r--r--   0        0        0     8670 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_transformation_block.py
--rw-r--r--   0        0        0     3918 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_update_pipeline_body.py
--rw-r--r--   0        0        0     3351 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_usage_report.py
--rw-r--r--   0        0        0     4440 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_user.py
--rw-r--r--   0        0        0     2294 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_user_all_of.py
--rw-r--r--   0        0        0     2104 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_detection.py
--rw-r--r--   0        0        0     3434 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_false_positive.py
--rw-r--r--   0        0        0     3770 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_ground_truth.py
--rw-r--r--   0        0        0     2477 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
--rw-r--r--   0        0        0     4880 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_parameter_set.py
--rw-r--r--   0        0        0     2255 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
--rw-r--r--   0        0        0     4092 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
--rw-r--r--   0        0        0     3007 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_parameters.py
--rw-r--r--   0        0        0     2585 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_parameters_standard.py
--rw-r--r--   0        0        0     2250 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_raw_detection.py
--rw-r--r--   0        0        0     2366 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
--rw-r--r--   0        0        0     2412 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
--rw-r--r--   0        0        0     2106 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
--rw-r--r--   0        0        0     1839 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/permission.py
--rw-r--r--   0        0        0     2491 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/portal_file.py
--rw-r--r--   0        0        0     2537 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/portal_info_response.py
--rw-r--r--   0        0        0     2666 2024-04-16 20:23:18.777005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/pretrained_model_tensor.py
--rw-r--r--   0        0        0     2403 2024-04-16 20:23:18.781005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/preview_default_files_in_folder_request.py
--rw-r--r--   0        0        0     3734 2024-04-16 20:23:18.781005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/preview_default_files_in_folder_response.py
--rw-r--r--   0        0        0     3467 2024-04-16 20:23:18.785005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2955 2024-04-16 20:23:18.785005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_info.py
--rw-r--r--   0        0        0     3117 2024-04-16 20:23:18.785005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_info_memory.py
--rw-r--r--   0        0        0     1918 2024-04-16 20:23:18.785005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_info_memory_eon.py
--rw-r--r--   0        0        0     2065 2024-04-16 20:23:18.785005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_info_memory_tflite.py
--rw-r--r--   0        0        0     4335 2024-04-16 20:23:18.785005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_table.py
--rw-r--r--   0        0        0     2780 2024-04-16 20:23:18.785005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_table_mcu.py
--rw-r--r--   0        0        0     3042 2024-04-16 20:23:18.785005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_table_mcu_memory.py
--rw-r--r--   0        0        0     2250 2024-04-16 20:23:18.785005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_table_mpu.py
--rw-r--r--   0        0        0     2201 2024-04-16 20:23:18.785005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_tf_lite_request.py
--rw-r--r--   0        0        0     3292 2024-04-16 20:23:18.785005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_tf_lite_response.py
--rw-r--r--   0        0        0     7873 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project.py
--rw-r--r--   0        0        0     4103 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_collaborator.py
--rw-r--r--   0        0        0     1895 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_collaborator_all_of.py
--rw-r--r--   0        0        0     2416 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_data_axes_summary_response.py
--rw-r--r--   0        0        0     2116 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
--rw-r--r--   0        0        0     2281 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_data_interval_response.py
--rw-r--r--   0        0        0     1964 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_data_interval_response_all_of.py
--rw-r--r--   0        0        0     2235 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_data_summary.py
--rw-r--r--   0        0        0     6854 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_deployment_target.py
--rw-r--r--   0        0        0     2706 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_deployment_target_all_of.py
--rw-r--r--   0        0        0     2780 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_deployment_targets_response.py
--rw-r--r--   0        0        0     2473 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     1943 2024-04-16 20:23:18.789005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_dismiss_notification_request.py
--rw-r--r--   0        0        0     2680 2024-04-16 20:23:18.793005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_downloads_response.py
--rw-r--r--   0        0        0     2373 2024-04-16 20:23:18.793005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_downloads_response_all_of.py
--rw-r--r--   0        0        0    14783 2024-04-16 20:23:18.793005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response.py
--rw-r--r--   0        0        0    14516 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of.py
--rw-r--r--   0        0        0     4174 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
--rw-r--r--   0        0        0     2723 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
--rw-r--r--   0        0        0     2997 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
--rw-r--r--   0        0        0     3200 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
--rw-r--r--   0        0        0     2339 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_experiments.py
--rw-r--r--   0        0        0     2285 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_impulse.py
--rw-r--r--   0        0        0     2726 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_performance.py
--rw-r--r--   0        0        0     1977 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_readme.py
--rw-r--r--   0        0        0     2225 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
--rw-r--r--   0        0        0     2735 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_urls.py
--rw-r--r--   0        0        0     2478 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_summary_response.py
--rw-r--r--   0        0        0     2172 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_summary_response_all_of.py
--rw-r--r--   0        0        0     3554 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_private_data.py
--rw-r--r--   0        0        0     4127 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_public_data.py
--rw-r--r--   0        0        0     1928 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_public_data_readme.py
--rw-r--r--   0        0        0     2404 2024-04-16 20:23:18.797005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_sample_metadata.py
--rw-r--r--   0        0        0      576 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_tier_enum.py
--rw-r--r--   0        0        0     2804 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_training_data_summary_response.py
--rw-r--r--   0        0        0     2487 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
--rw-r--r--   0        0        0     2253 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py
--rw-r--r--   0        0        0      606 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_type.py
--rw-r--r--   0        0        0     2316 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_version_request.py
--rw-r--r--   0        0        0      504 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_visibility.py
--rw-r--r--   0        0        0     4991 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/public_organization_transformation_block.py
--rw-r--r--   0        0        0     2664 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/raw_sample_data.py
--rw-r--r--   0        0        0     3440 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/raw_sample_payload.py
--rw-r--r--   0        0        0     2537 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/rebalance_dataset_response.py
--rw-r--r--   0        0        0     1984 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/remove_collaborator_request.py
--rw-r--r--   0        0        0     1805 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/remove_member_request.py
--rw-r--r--   0        0        0     1867 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/rename_device_request.py
--rw-r--r--   0        0        0     2081 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/rename_portal_file_request.py
--rw-r--r--   0        0        0     1867 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/rename_sample_request.py
--rw-r--r--   0        0        0     2028 2024-04-16 20:23:18.801005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/request_email_verification_request.py
--rw-r--r--   0        0        0     1873 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/request_reset_password_request.py
--rw-r--r--   0        0        0     2031 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/reset_password_request.py
--rw-r--r--   0        0        0     1896 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/resource_range.py
--rw-r--r--   0        0        0     1985 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/restore_project_from_public_request.py
--rw-r--r--   0        0        0     2265 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/restore_project_request.py
--rw-r--r--   0        0        0     2421 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/run_auto_labeler_request.py
--rw-r--r--   0        0        0     2669 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/run_organization_pipeline_response.py
--rw-r--r--   0        0        0     2352 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
--rw-r--r--   0        0        0    11134 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/sample.py
--rw-r--r--   0        0        0     2443 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/sample_bounding_boxes_request.py
--rw-r--r--   0        0        0     2000 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/sample_metadata.py
--rw-r--r--   0        0        0     2517 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/save_auto_labeler_clusters_request.py
--rw-r--r--   0        0        0     2071 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py
--rw-r--r--   0        0        0     2341 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/save_auto_labeler_clusters_response.py
--rw-r--r--   0        0        0     2024 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py
--rw-r--r--   0        0        0     2756 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/save_pretrained_model_request.py
--rw-r--r--   0        0        0     3327 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/score_trial_response.py
--rw-r--r--   0        0        0     3003 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/score_trial_response_all_of.py
--rw-r--r--   0        0        0     2240 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/score_trial_response_all_of_latency.py
--rw-r--r--   0        0        0     1914 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/score_trial_response_all_of_ram.py
--rw-r--r--   0        0        0     2405 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/segment_sample_request.py
--rw-r--r--   0        0        0     2055 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/segment_sample_request_segments_inner.py
--rw-r--r--   0        0        0     3346 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/send_user_feedback_request.py
--rw-r--r--   0        0        0     1981 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/sensor.py
--rw-r--r--   0        0        0     2142 2024-04-16 20:23:18.805005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_anomaly_parameter_request.py
--rw-r--r--   0        0        0     9364 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_keras_parameter_request.py
--rw-r--r--   0        0        0     1893 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_member_datasets_request.py
--rw-r--r--   0        0        0     1905 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_member_role_request.py
--rw-r--r--   0        0        0     2219 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_optimize_space_request.py
--rw-r--r--   0        0        0     2254 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_optimize_space_request_all_of.py
--rw-r--r--   0        0        0     1923 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_organization_data_dataset_request.py
--rw-r--r--   0        0        0     1974 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_project_compute_time_request.py
--rw-r--r--   0        0        0     2011 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_project_dsp_file_size_request.py
--rw-r--r--   0        0        0     1919 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_sample_metadata_request.py
--rw-r--r--   0        0        0     2531 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_sample_structured_labels_request.py
--rw-r--r--   0        0        0     1915 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_syntiant_posterior_request.py
--rw-r--r--   0        0        0     2140 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_user_password_request.py
--rw-r--r--   0        0        0     2536 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/socket_token_response.py
--rw-r--r--   0        0        0     2239 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/socket_token_response_all_of.py
--rw-r--r--   0        0        0     2059 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/socket_token_response_all_of_token.py
--rw-r--r--   0        0        0     1971 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/split_sample_in_frames_request.py
--rw-r--r--   0        0        0     2110 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/staff_info.py
--rw-r--r--   0        0        0     2292 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_device_debug_stream_response.py
--rw-r--r--   0        0        0     1975 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py
--rw-r--r--   0        0        0     2178 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py
--rw-r--r--   0        0        0     5388 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_enterprise_trial_request.py
--rw-r--r--   0        0        0     2226 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_job_response.py
--rw-r--r--   0        0        0     1909 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_job_response_all_of.py
--rw-r--r--   0        0        0     2883 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_performance_calibration_request.py
--rw-r--r--   0        0        0     2838 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_sampling_request.py
--rw-r--r--   0        0        0     2189 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_sampling_response.py
--rw-r--r--   0        0        0     1892 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_sampling_response_all_of.py
--rw-r--r--   0        0        0     2795 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_training_request_anomaly.py
--rw-r--r--   0        0        0     1926 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/stop_device_debug_stream_request.py
--rw-r--r--   0        0        0     1967 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/store_segment_length_request.py
--rw-r--r--   0        0        0     3394 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/structured_classify_result.py
--rw-r--r--   0        0        0     2270 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/structured_label.py
--rw-r--r--   0        0        0     4399 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/target_constraints.py
--rw-r--r--   0        0        0     2923 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/target_constraints_device.py
--rw-r--r--   0        0        0     2347 2024-04-16 20:23:18.809005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/target_memory.py
--rw-r--r--   0        0        0     3751 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/target_processor.py
--rw-r--r--   0        0        0     2433 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/test_pretrained_model_request.py
--rw-r--r--   0        0        0     3074 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/test_pretrained_model_response.py
--rw-r--r--   0        0        0     2784 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3251 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/theme.py
--rw-r--r--   0        0        0     2239 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/theme_colors.py
--rw-r--r--   0        0        0     2764 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/theme_favicon.py
--rw-r--r--   0        0        0     2721 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/theme_logos.py
--rw-r--r--   0        0        0     2245 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/third_party_auth.py
--rw-r--r--   0        0        0     1921 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/time_series_data_point.py
--rw-r--r--   0        0        0     2031 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/track_objects_request.py
--rw-r--r--   0        0        0     2736 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/track_objects_response.py
--rw-r--r--   0        0        0     2436 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/track_objects_response_all_of.py
--rw-r--r--   0        0        0     5380 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/transfer_learning_model.py
--rw-r--r--   0        0        0     2012 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/transfer_ownership_organization_request.py
--rw-r--r--   0        0        0     2585 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/transformation_block_additional_mount_point.py
--rw-r--r--   0        0        0      548 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/transformation_job_operates_on_enum.py
--rw-r--r--   0        0        0      588 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/transformation_job_status_enum.py
--rw-r--r--   0        0        0     2578 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_create_trial_impulse.py
--rw-r--r--   0        0        0     2462 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_run.py
--rw-r--r--   0        0        0     2570 2024-04-16 20:23:18.813005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_space_impulse.py
--rw-r--r--   0        0        0     4991 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_trial.py
--rw-r--r--   0        0        0     2739 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_trial_blocks_inner.py
--rw-r--r--   0        0        0     1935 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
--rw-r--r--   0        0        0     2211 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_trial_impulse.py
--rw-r--r--   0        0        0     2028 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_job_request.py
--rw-r--r--   0        0        0     2281 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_add_collaborator_request.py
--rw-r--r--   0        0        0     2882 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_bucket_request.py
--rw-r--r--   0        0        0     2828 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_create_empty_project_request.py
--rw-r--r--   0        0        0     2428 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_create_project_request.py
--rw-r--r--   0        0        0     2913 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     4154 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2158 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_data_item_request.py
--rw-r--r--   0        0        0     2977 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_dataset_request.py
--rw-r--r--   0        0        0     2518 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_dataset_request_bucket.py
--rw-r--r--   0        0        0     2881 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2724 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_portal_response.py
--rw-r--r--   0        0        0     2445 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2766 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_request.py
--rw-r--r--   0        0        0     5211 2024-04-16 20:23:18.817005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     6072 2024-04-16 20:23:18.821005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_transformation_block_request.py
--rw-r--r--   0        0        0    11806 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_project_request.py
--rw-r--r--   0        0        0     1877 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_project_tags_request.py
--rw-r--r--   0        0        0     2259 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_theme_colors_request.py
--rw-r--r--   0        0        0     2895 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_theme_logos_request.py
--rw-r--r--   0        0        0     2205 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_third_party_auth_request.py
--rw-r--r--   0        0        0     1865 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_tuner_run_request.py
--rw-r--r--   0        0        0     2375 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_user_request.py
--rw-r--r--   0        0        0     1886 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_version_request.py
--rw-r--r--   0        0        0     2393 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
--rw-r--r--   0        0        0     2237 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
--rw-r--r--   0        0        0     2125 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
--rw-r--r--   0        0        0     2155 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py
--rw-r--r--   0        0        0     2059 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_whitelabel_request.py
--rw-r--r--   0        0        0     2168 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/upload_asset_response.py
--rw-r--r--   0        0        0     1882 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/upload_asset_response_all_of.py
--rw-r--r--   0        0        0     2199 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/upload_readme_image_response.py
--rw-r--r--   0        0        0     2185 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/upload_user_photo_response.py
--rw-r--r--   0        0        0     1872 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/upload_user_photo_response_all_of.py
--rw-r--r--   0        0        0     3888 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user.py
--rw-r--r--   0        0        0     1991 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_by_third_party_activation_request.py
--rw-r--r--   0        0        0     1956 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py
--rw-r--r--   0        0        0     1922 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_dismiss_notification_request.py
--rw-r--r--   0        0        0     2192 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_experiment.py
--rw-r--r--   0        0        0     2425 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_generate_new_mfa_key_response.py
--rw-r--r--   0        0        0     2119 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py
--rw-r--r--   0        0        0     4606 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_organization.py
--rw-r--r--   0        0        0     2144 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_set_totp_mfa_key_request.py
--rw-r--r--   0        0        0     2480 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_set_totp_mfa_key_response.py
--rw-r--r--   0        0        0     2191 2024-04-16 20:23:18.825005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py
--rw-r--r--   0        0        0      543 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_tier_enum.py
--rw-r--r--   0        0        0     1844 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_dsp_block_url_request.py
--rw-r--r--   0        0        0     2604 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_dsp_block_url_response.py
--rw-r--r--   0        0        0     2307 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
--rw-r--r--   0        0        0     3049 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
--rw-r--r--   0        0        0     2633 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_email_response.py
--rw-r--r--   0        0        0     2354 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_email_response_all_of.py
--rw-r--r--   0        0        0     2708 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_organization_bucket_request.py
--rw-r--r--   0        0        0     3432 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_organization_bucket_response.py
--rw-r--r--   0        0        0     3155 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2187 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
--rw-r--r--   0        0        0     1961 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_organization_existing_bucket_request.py
--rw-r--r--   0        0        0     1937 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_reset_password_request.py
--rw-r--r--   0        0        0     8565 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/whitelabel.py
--rw-r--r--   0        0        0     2534 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
--rw-r--r--   0        0        0     2085 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py
--rw-r--r--   0        0        0     2120 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
--rw-r--r--   0        0        0     2885 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/window_settings_response.py
--rw-r--r--   0        0        0     2585 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/window_settings_response_all_of.py
--rw-r--r--   0        0        0     2848 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
--rw-r--r--   0        0        0    12674 2024-04-16 20:23:18.829005 edgeimpulse_api-1.49.8/edgeimpulse_api/rest.py
--rw-r--r--   0        0        0     1019 2024-04-16 20:23:51.492719 edgeimpulse_api-1.49.8/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 edgeimpulse_api-1.49.8/PKG-INFO
+-rw-r--r--   0        0        0      377 2024-04-17 10:43:42.926402 edgeimpulse_api-1.49.9/README.md
+-rw-r--r--   0        0        0    88508 2024-04-17 10:44:15.302117 edgeimpulse_api-1.49.9/edgeimpulse_api/__init__.py
+-rw-r--r--   0        0        0     2172 2024-04-17 10:43:42.926402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/__init__.py
+-rw-r--r--   0        0        0   386649 2024-04-17 10:43:42.930402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/admin_api.py
+-rw-r--r--   0        0        0    11231 2024-04-17 10:43:42.930402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/auth_api.py
+-rw-r--r--   0        0        0     6235 2024-04-17 10:43:42.930402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/cdn_api.py
+-rw-r--r--   0        0        0    59980 2024-04-17 10:43:42.934402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/classify_api.py
+-rw-r--r--   0        0        0    72480 2024-04-17 10:43:42.934402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/deployment_api.py
+-rw-r--r--   0        0        0    80789 2024-04-17 10:43:42.934402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/devices_api.py
+-rw-r--r--   0        0        0   139045 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/dsp_api.py
+-rw-r--r--   0        0        0    19442 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/email_verification_api.py
+-rw-r--r--   0        0        0     6435 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/export_api.py
+-rw-r--r--   0        0        0     5996 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/feature_flags_api.py
+-rw-r--r--   0        0        0    11921 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/health_api.py
+-rw-r--r--   0        0        0    49621 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/impulse_api.py
+-rw-r--r--   0        0        0   238420 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/jobs_api.py
+-rw-r--r--   0        0        0   154112 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/learn_api.py
+-rw-r--r--   0        0        0     6483 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/login_api.py
+-rw-r--r--   0        0        0    17897 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/metrics_api.py
+-rw-r--r--   0        0        0    85275 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/optimization_api.py
+-rw-r--r--   0        0        0   197840 2024-04-17 10:43:42.942402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_blocks_api.py
+-rw-r--r--   0        0        0    92715 2024-04-17 10:43:42.942402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_create_project_api.py
+-rw-r--r--   0        0        0   331750 2024-04-17 10:43:42.942402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_data_api.py
+-rw-r--r--   0        0        0    80882 2024-04-17 10:43:42.946402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_data_campaigns_api.py
+-rw-r--r--   0        0        0    58218 2024-04-17 10:43:42.946402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_jobs_api.py
+-rw-r--r--   0        0        0    53291 2024-04-17 10:43:42.946402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_pipelines_api.py
+-rw-r--r--   0        0        0    45490 2024-04-17 10:43:42.946402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_portals_api.py
+-rw-r--r--   0        0        0   505317 2024-04-17 10:43:42.946402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organizations_api.py
+-rw-r--r--   0        0        0    60377 2024-04-17 10:43:42.950402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/performance_calibration_api.py
+-rw-r--r--   0        0        0   270960 2024-04-17 10:43:42.954402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/projects_api.py
+-rw-r--r--   0        0        0   414581 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/raw_data_api.py
+-rw-r--r--   0        0        0    35671 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/themes_api.py
+-rw-r--r--   0        0        0    43486 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/third_party_auth_api.py
+-rw-r--r--   0        0        0    45692 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/upload_portal_api.py
+-rw-r--r--   0        0        0   247228 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/user_api.py
+-rw-r--r--   0        0        0    42135 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/whitelabels_api.py
+-rw-r--r--   0        0        0    29331 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api_client.py
+-rw-r--r--   0        0        0    15659 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/configuration.py
+-rw-r--r--   0        0        0     5113 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/exceptions.py
+-rw-r--r--   0        0        0    85883 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/__init__.py
+-rw-r--r--   0        0        0     2897 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
+-rw-r--r--   0        0        0     1982 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/activate_user_or_verify_email_request.py
+-rw-r--r--   0        0        0     2052 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_api_key_request.py
+-rw-r--r--   0        0        0     1963 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_collaborator_request.py
+-rw-r--r--   0        0        0     2223 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_hmac_key_request.py
+-rw-r--r--   0        0        0     2299 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_member_request.py
+-rw-r--r--   0        0        0     2418 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2122 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_api_key_request_all_of.py
+-rw-r--r--   0        0        0     2806 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_bucket_request.py
+-rw-r--r--   0        0        0     2794 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     2469 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2152 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     4230 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2359 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2042 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
+-rw-r--r--   0        0        0     2269 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2816 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2248 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2054 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_request.py
+-rw-r--r--   0        0        0     2266 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_response.py
+-rw-r--r--   0        0        0     1949 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_response_all_of.py
+-rw-r--r--   0        0        0     4885 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     2339 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     6169 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     2325 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2001 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     2659 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_project_api_key_request.py
+-rw-r--r--   0        0        0     2370 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_project_api_key_request_all_of.py
+-rw-r--r--   0        0        0     1940 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
+-rw-r--r--   0        0        0     1961 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
+-rw-r--r--   0        0        0     2661 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2542 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_user_request.py
+-rw-r--r--   0        0        0     2246 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
+-rw-r--r--   0        0        0     2344 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_api_key_request.py
+-rw-r--r--   0        0        0     2044 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py
+-rw-r--r--   0        0        0     2146 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_user_request.py
+-rw-r--r--   0        0        0     2097 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_user_request.py
+-rw-r--r--   0        0        0     5903 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_organization.py
+-rw-r--r--   0        0        0     2396 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_organization_all_of.py
+-rw-r--r--   0        0        0     3259 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_project.py
+-rw-r--r--   0        0        0     7529 2024-04-17 10:43:42.966402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_user.py
+-rw-r--r--   0        0        0     5318 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_user_all_of.py
+-rw-r--r--   0        0        0     2386 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_organization_data_export_request.py
+-rw-r--r--   0        0        0     2262 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_organization_request.py
+-rw-r--r--   0        0        0     2718 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_project_request.py
+-rw-r--r--   0        0        0     1905 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_enable_feature_request.py
+-rw-r--r--   0        0        0     2546 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migration_response.py
+-rw-r--r--   0        0        0     2222 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
+-rw-r--r--   0        0        0     2735 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migrations_response.py
+-rw-r--r--   0        0        0     2428 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
+-rw-r--r--   0        0        0     2318 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
+-rw-r--r--   0        0        0     2022 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
+-rw-r--r--   0        0        0     2217 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_metrics_response.py
+-rw-r--r--   0        0        0     1910 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3148 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py
+-rw-r--r--   0        0        0     2647 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_report_response.py
+-rw-r--r--   0        0        0     2323 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py
+-rw-r--r--   0        0        0     3029 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py
+-rw-r--r--   0        0        0     2729 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py
+-rw-r--r--   0        0        0     3046 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response.py
+-rw-r--r--   0        0        0     2746 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
+-rw-r--r--   0        0        0     3409 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
+-rw-r--r--   0        0        0     2243 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
+-rw-r--r--   0        0        0     1947 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
+-rw-r--r--   0        0        0     2914 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response.py
+-rw-r--r--   0        0        0     2614 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
+-rw-r--r--   0        0        0     2096 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
+-rw-r--r--   0        0        0     2208 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_ids_response.py
+-rw-r--r--   0        0        0     1901 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
+-rw-r--r--   0        0        0     2245 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_metrics_response.py
+-rw-r--r--   0        0        0     2452 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_response.py
+-rw-r--r--   0        0        0     2128 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_response_all_of.py
+-rw-r--r--   0        0        0     2507 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_trial_response.py
+-rw-r--r--   0        0        0     2183 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
+-rw-r--r--   0        0        0     2807 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response.py
+-rw-r--r--   0        0        0     2500 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response_all_of.py
+-rw-r--r--   0        0        0     2878 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
+-rw-r--r--   0        0        0     2445 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_list_projects.py
+-rw-r--r--   0        0        0     2836 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_list_projects_response.py
+-rw-r--r--   0        0        0     4245 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_organization_info_response.py
+-rw-r--r--   0        0        0     3084 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_organization_info_response_all_of.py
+-rw-r--r--   0        0        0     2158 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_toggle_data_migration_request.py
+-rw-r--r--   0        0        0     2397 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_organization_data_export_request.py
+-rw-r--r--   0        0        0     3936 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_organization_request.py
+-rw-r--r--   0        0        0     2015 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_permissions_request.py
+-rw-r--r--   0        0        0     2830 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_request.py
+-rw-r--r--   0        0        0     2532 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_trial_request.py
+-rw-r--r--   0        0        0     2525 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/akida_edge_learning_config.py
+-rw-r--r--   0        0        0      512 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_capacity.py
+-rw-r--r--   0        0        0     2512 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_gmm_metadata.py
+-rw-r--r--   0        0        0     2212 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py
+-rw-r--r--   0        0        0     5499 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata.py
+-rw-r--r--   0        0        0     5221 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
+-rw-r--r--   0        0        0     2151 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
+-rw-r--r--   0        0        0     4079 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response.py
+-rw-r--r--   0        0        0     3812 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response_all_of.py
+-rw-r--r--   0        0        0     2044 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response_all_of_axes.py
+-rw-r--r--   0        0        0     3188 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_result.py
+-rw-r--r--   0        0        0     3029 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response.py
+-rw-r--r--   0        0        0     2729 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2375 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     3358 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/application_budget.py
+-rw-r--r--   0        0        0      506 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/augmentation_policy_image_enum.py
+-rw-r--r--   0        0        0     3635 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/augmentation_policy_spectrogram.py
+-rw-r--r--   0        0        0     1895 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/autotune_dsp_request.py
+-rw-r--r--   0        0        0      505 2024-04-17 10:43:42.982402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/block_display_category.py
+-rw-r--r--   0        0        0      560 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/block_type.py
+-rw-r--r--   0        0        0     2044 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/bounding_box.py
+-rw-r--r--   0        0        0     2151 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/bounding_box_with_score.py
+-rw-r--r--   0        0        0     2197 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/build_on_device_model_request.py
+-rw-r--r--   0        0        0     2433 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/build_organization_on_device_model_request.py
+-rw-r--r--   0        0        0     2459 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
+-rw-r--r--   0        0        0     2041 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/change_password_request.py
+-rw-r--r--   0        0        0     3701 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response.py
+-rw-r--r--   0        0        0     3394 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of.py
+-rw-r--r--   0        0        0     3769 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
+-rw-r--r--   0        0        0     2055 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
+-rw-r--r--   0        0        0     3255 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_page.py
+-rw-r--r--   0        0        0     2948 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_page_all_of.py
+-rw-r--r--   0        0        0     4026 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response.py
+-rw-r--r--   0        0        0     3759 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_all_of.py
+-rw-r--r--   0        0        0     6252 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_classification.py
+-rw-r--r--   0        0        0     2755 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_classification_details.py
+-rw-r--r--   0        0        0     3816 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_v2200_response.py
+-rw-r--r--   0        0        0     3004 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/convert_user_request.py
+-rw-r--r--   0        0        0     3495 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_data.py
+-rw-r--r--   0        0        0     3114 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue.py
+-rw-r--r--   0        0        0     3241 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py
+-rw-r--r--   0        0        0     2484 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py
+-rw-r--r--   0        0        0     2183 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/count_samples_response.py
+-rw-r--r--   0        0        0     1859 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/count_samples_response_all_of.py
+-rw-r--r--   0        0        0     2255 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_block_version_response.py
+-rw-r--r--   0        0        0     1938 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_block_version_response_all_of.py
+-rw-r--r--   0        0        0     2404 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_developer_profile_response.py
+-rw-r--r--   0        0        0     2125 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_developer_profile_response_all_of.py
+-rw-r--r--   0        0        0     2387 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_device_request.py
+-rw-r--r--   0        0        0     2850 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_response.py
+-rw-r--r--   0        0        0     2319 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py
+-rw-r--r--   0        0        0     6569 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_user_request.py
+-rw-r--r--   0        0        0     4092 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py
+-rw-r--r--   0        0        0     2491 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_evaluation_user_response.py
+-rw-r--r--   0        0        0     2185 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
+-rw-r--r--   0        0        0     2600 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_request.py
+-rw-r--r--   0        0        0     2830 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_response.py
+-rw-r--r--   0        0        0     2551 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     1990 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_request.py
+-rw-r--r--   0        0        0     2454 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_response.py
+-rw-r--r--   0        0        0     2148 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_response_all_of.py
+-rw-r--r--   0        0        0     2155 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_usage_report_body.py
+-rw-r--r--   0        0        0     2185 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_pipeline_response.py
+-rw-r--r--   0        0        0     2504 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_request.py
+-rw-r--r--   0        0        0     2378 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_response.py
+-rw-r--r--   0        0        0     2072 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_response_all_of.py
+-rw-r--r--   0        0        0     2276 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_request.py
+-rw-r--r--   0        0        0     2414 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_response.py
+-rw-r--r--   0        0        0     2135 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
+-rw-r--r--   0        0        0     2413 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_request.py
+-rw-r--r--   0        0        0     2450 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_response.py
+-rw-r--r--   0        0        0     2144 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     4197 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_request.py
+-rw-r--r--   0        0        0     2393 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_response.py
+-rw-r--r--   0        0        0     2114 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_response_all_of.py
+-rw-r--r--   0        0        0     2919 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_request.py
+-rw-r--r--   0        0        0     2672 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_response.py
+-rw-r--r--   0        0        0     2393 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_response_all_of.py
+-rw-r--r--   0        0        0     4384 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_request.py
+-rw-r--r--   0        0        0     2438 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_response.py
+-rw-r--r--   0        0        0     2121 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2094 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/created_updated_by_user.py
+-rw-r--r--   0        0        0     2051 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_request.py
+-rw-r--r--   0        0        0     2248 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_response.py
+-rw-r--r--   0        0        0     1943 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_response_all_of.py
+-rw-r--r--   0        0        0     2368 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cross_validation_data.py
+-rw-r--r--   0        0        0     3412 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cross_validation_data_scores_inner.py
+-rw-r--r--   0        0        0     4054 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign.py
+-rw-r--r--   0        0        0     2989 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_dashboard.py
+-rw-r--r--   0        0        0     2786 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph.py
+-rw-r--r--   0        0        0     3352 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
+-rw-r--r--   0        0        0     2047 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
+-rw-r--r--   0        0        0     1934 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_link.py
+-rw-r--r--   0        0        0     1957 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_query.py
+-rw-r--r--   0        0        0     3292 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_predictions_response.py
+-rw-r--r--   0        0        0     3003 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
+-rw-r--r--   0        0        0     2838 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_settings.py
+-rw-r--r--   0        0        0     2149 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dataset_ratio_data.py
+-rw-r--r--   0        0        0     2111 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dataset_ratio_data_ratio.py
+-rw-r--r--   0        0        0     1898 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/delete_portal_file_request.py
+-rw-r--r--   0        0        0     2230 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dependency_data.py
+-rw-r--r--   0        0        0     2280 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
+-rw-r--r--   0        0        0     2408 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
+-rw-r--r--   0        0        0     2155 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
+-rw-r--r--   0        0        0     2484 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
+-rw-r--r--   0        0        0     2344 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
+-rw-r--r--   0        0        0     2780 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
+-rw-r--r--   0        0        0     2200 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
+-rw-r--r--   0        0        0     4397 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request.py
+-rw-r--r--   0        0        0     2833 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
+-rw-r--r--   0        0        0     8503 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
+-rw-r--r--   0        0        0     8065 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
+-rw-r--r--   0        0        0     5950 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target.py
+-rw-r--r--   0        0        0     1926 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target_badge.py
+-rw-r--r--   0        0        0      737 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target_engine.py
+-rw-r--r--   0        0        0     2702 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_targets_response.py
+-rw-r--r--   0        0        0     2395 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     2248 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_created_response.py
+-rw-r--r--   0        0        0     2032 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_request.py
+-rw-r--r--   0        0        0     2134 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_request_update.py
+-rw-r--r--   0        0        0     2113 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_response.py
+-rw-r--r--   0        0        0     2864 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_boards_response.py
+-rw-r--r--   0        0        0     2564 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_boards_response_all_of.py
+-rw-r--r--   0        0        0     2030 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_keys.py
+-rw-r--r--   0        0        0     2400 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_keys_response.py
+-rw-r--r--   0        0        0     4816 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device.py
+-rw-r--r--   0        0        0      516 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_debug_stream_type.py
+-rw-r--r--   0        0        0     2811 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_inference_info.py
+-rw-r--r--   0        0        0     2199 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_name_response.py
+-rw-r--r--   0        0        0     1920 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_name_response_all_of.py
+-rw-r--r--   0        0        0     2231 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_sensors_inner.py
+-rw-r--r--   0        0        0     2094 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/download.py
+-rw-r--r--   0        0        0     1912 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_request.py
+-rw-r--r--   0        0        0     2260 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_response.py
+-rw-r--r--   0        0        0     1954 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_response_all_of.py
+-rw-r--r--   0        0        0     2724 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results.py
+-rw-r--r--   0        0        0     2417 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
+-rw-r--r--   0        0        0     1968 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
+-rw-r--r--   0        0        0     3660 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_block.py
+-rw-r--r--   0        0        0     1834 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_request.py
+-rw-r--r--   0        0        0     3092 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_response.py
+-rw-r--r--   0        0        0     2813 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_response_all_of.py
+-rw-r--r--   0        0        0     3016 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response.py
+-rw-r--r--   0        0        0     2728 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
+-rw-r--r--   0        0        0     2058 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
+-rw-r--r--   0        0        0     2572 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
+-rw-r--r--   0        0        0     2216 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_labels_response.py
+-rw-r--r--   0        0        0     1920 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
+-rw-r--r--   0        0        0     2294 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group.py
+-rw-r--r--   0        0        0     4216 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item.py
+-rw-r--r--   0        0        0     2190 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
+-rw-r--r--   0        0        0     2195 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item_show_if.py
+-rw-r--r--   0        0        0     4848 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info.py
+-rw-r--r--   0        0        0     2376 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info_features.py
+-rw-r--r--   0        0        0     1885 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info_performance.py
+-rw-r--r--   0        0        0     5462 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata.py
+-rw-r--r--   0        0        0     2025 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
+-rw-r--r--   0        0        0     2566 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_output_config.py
+-rw-r--r--   0        0        0     2531 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
+-rw-r--r--   0        0        0     5820 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_response.py
+-rw-r--r--   0        0        0     1963 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_named_axis.py
+-rw-r--r--   0        0        0     3019 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response.py
+-rw-r--r--   0        0        0     2729 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2278 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
+-rw-r--r--   0        0        0     4639 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_graph.py
+-rw-r--r--   0        0        0     1899 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
+-rw-r--r--   0        0        0     2677 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_with_features.py
+-rw-r--r--   0        0        0     2151 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_without_features.py
+-rw-r--r--   0        0        0     2030 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
+-rw-r--r--   0        0        0     3697 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response.py
+-rw-r--r--   0        0        0     3418 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_all_of.py
+-rw-r--r--   0        0        0     1969 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
+-rw-r--r--   0        0        0     4579 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_with_sample.py
+-rw-r--r--   0        0        0     4312 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
+-rw-r--r--   0        0        0     3342 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response.py
+-rw-r--r--   0        0        0     3042 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
+-rw-r--r--   0        0        0     2748 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2213 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     3353 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response.py
+-rw-r--r--   0        0        0     3053 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2773 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2205 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     1893 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/edit_sample_label_request.py
+-rw-r--r--   0        0        0     4246 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/enterprise_trial.py
+-rw-r--r--   0        0        0     2960 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py
+-rw-r--r--   0        0        0     2885 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/entitlement_limits.py
+-rw-r--r--   0        0        0     2367 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/entity_created_response.py
+-rw-r--r--   0        0        0     2077 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/entity_created_response_all_of.py
+-rw-r--r--   0        0        0     2656 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_job_response.py
+-rw-r--r--   0        0        0     2349 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_job_response_all_of.py
+-rw-r--r--   0        0        0     2099 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_result_value.py
+-rw-r--r--   0        0        0     2366 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_block_response.py
+-rw-r--r--   0        0        0     2060 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_block_response_all_of.py
+-rw-r--r--   0        0        0     2511 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_get_url_response.py
+-rw-r--r--   0        0        0     2244 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_get_url_response_all_of.py
+-rw-r--r--   0        0        0     2116 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_keras_block_data_request.py
+-rw-r--r--   0        0        0     2373 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_original_data_request.py
+-rw-r--r--   0        0        0     2021 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_wav_data_request.py
+-rw-r--r--   0        0        0      500 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/feature.py
+-rw-r--r--   0        0        0     2206 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_request.py
+-rw-r--r--   0        0        0     2804 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response.py
+-rw-r--r--   0        0        0     2497 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response_all_of.py
+-rw-r--r--   0        0        0     2090 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
+-rw-r--r--   0        0        0     2665 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response.py
+-rw-r--r--   0        0        0     2358 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response_all_of.py
+-rw-r--r--   0        0        0     2322 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response_all_of_users.py
+-rw-r--r--   0        0        0     2507 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/generate_features_request.py
+-rw-r--r--   0        0        0     2083 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/generic_api_response.py
+-rw-r--r--   0        0        0     2764 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response.py
+-rw-r--r--   0        0        0     2457 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
+-rw-r--r--   0        0        0     2156 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
+-rw-r--r--   0        0        0     2698 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_third_party_auth_response.py
+-rw-r--r--   0        0        0     2391 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     2713 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_whitelabels_response.py
+-rw-r--r--   0        0        0     2406 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
+-rw-r--r--   0        0        0     3527 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response.py
+-rw-r--r--   0        0        0     3260 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of.py
+-rw-r--r--   0        0        0     2588 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py
+-rw-r--r--   0        0        0     1954 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py
+-rw-r--r--   0        0        0     2345 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py
+-rw-r--r--   0        0        0     2078 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py
+-rw-r--r--   0        0        0     3400 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_features_response.py
+-rw-r--r--   0        0        0     3122 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0     3752 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_settings_response.py
+-rw-r--r--   0        0        0     2402 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
+-rw-r--r--   0        0        0     2349 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_deployment_response.py
+-rw-r--r--   0        0        0     2071 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_deployment_response_all_of.py
+-rw-r--r--   0        0        0     2434 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_device_response.py
+-rw-r--r--   0        0        0     2137 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_device_response_all_of.py
+-rw-r--r--   0        0        0     2752 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response.py
+-rw-r--r--   0        0        0     2455 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of.py
+-rw-r--r--   0        0        0     4251 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
+-rw-r--r--   0        0        0     2859 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2456 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_code_response.py
+-rw-r--r--   0        0        0     2177 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_code_response_all_of.py
+-rw-r--r--   0        0        0     2350 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_status_response.py
+-rw-r--r--   0        0        0     2045 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_status_response_all_of.py
+-rw-r--r--   0        0        0     2788 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response.py
+-rw-r--r--   0        0        0     2488 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response_all_of.py
+-rw-r--r--   0        0        0     2118 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py
+-rw-r--r--   0        0        0     3930 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_blocks_response.py
+-rw-r--r--   0        0        0     3630 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2429 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_records_request.py
+-rw-r--r--   0        0        0     2007 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_records_request_range.py
+-rw-r--r--   0        0        0     2454 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_response.py
+-rw-r--r--   0        0        0     2157 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_response_all_of.py
+-rw-r--r--   0        0        0     2374 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_job_response.py
+-rw-r--r--   0        0        0     2077 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_job_response_all_of.py
+-rw-r--r--   0        0        0     3070 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_request.py
+-rw-r--r--   0        0        0     2431 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_response.py
+-rw-r--r--   0        0        0     2152 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_response_all_of.py
+-rw-r--r--   0        0        0     2580 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response.py
+-rw-r--r--   0        0        0     2256 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response_all_of.py
+-rw-r--r--   0        0        0     3358 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py
+-rw-r--r--   0        0        0     3578 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response.py
+-rw-r--r--   0        0        0     3300 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
+-rw-r--r--   0        0        0     2869 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
+-rw-r--r--   0        0        0     2572 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_notes_response.py
+-rw-r--r--   0        0        0     2265 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_notes_response_all_of.py
+-rw-r--r--   0        0        0     2556 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_bucket_response.py
+-rw-r--r--   0        0        0     2232 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2701 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2377 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     2890 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
+-rw-r--r--   0        0        0     2583 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
+-rw-r--r--   0        0        0     3158 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2939 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response.py
+-rw-r--r--   0        0        0     2632 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
+-rw-r--r--   0        0        0     2921 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
+-rw-r--r--   0        0        0     2601 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_export_response.py
+-rw-r--r--   0        0        0     2277 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_export_response_all_of.py
+-rw-r--r--   0        0        0     2982 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_exports_response.py
+-rw-r--r--   0        0        0     2682 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py
+-rw-r--r--   0        0        0     2561 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_response.py
+-rw-r--r--   0        0        0     2237 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
+-rw-r--r--   0        0        0     3411 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
+-rw-r--r--   0        0        0     3111 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
+-rw-r--r--   0        0        0     3532 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
+-rw-r--r--   0        0        0     2576 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dataset_response.py
+-rw-r--r--   0        0        0     2252 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
+-rw-r--r--   0        0        0     2690 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2373 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py
+-rw-r--r--   0        0        0     2627 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2310 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py
+-rw-r--r--   0        0        0     2603 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2279 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     3670 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_portal_response.py
+-rw-r--r--   0        0        0     3391 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2323 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_projects_data_count_response.py
+-rw-r--r--   0        0        0     2906 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     2589 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py
+-rw-r--r--   0        0        0     2858 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2541 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     2612 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_usage_report_response.py
+-rw-r--r--   0        0        0     2905 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
+-rw-r--r--   0        0        0     2598 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
+-rw-r--r--   0        0        0     3012 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
+-rw-r--r--   0        0        0     2712 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
+-rw-r--r--   0        0        0     2722 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
+-rw-r--r--   0        0        0     2425 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2922 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
+-rw-r--r--   0        0        0     2615 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
+-rw-r--r--   0        0        0     3151 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_status_response.py
+-rw-r--r--   0        0        0     2884 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
+-rw-r--r--   0        0        0     3761 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response.py
+-rw-r--r--   0        0        0     3483 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     4031 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
+-rw-r--r--   0        0        0     2978 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
+-rw-r--r--   0        0        0     3058 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
+-rw-r--r--   0        0        0     2397 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_public_metrics_response.py
+-rw-r--r--   0        0        0     2073 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_public_metrics_response_all_of.py
+-rw-r--r--   0        0        0     2767 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_sample_metadata_response.py
+-rw-r--r--   0        0        0     3044 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_sample_response.py
+-rw-r--r--   0        0        0     2462 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_syntiant_posterior_response.py
+-rw-r--r--   0        0        0     2184 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
+-rw-r--r--   0        0        0     2694 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_target_constraints_response.py
+-rw-r--r--   0        0        0     2404 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_target_constraints_response_all_of.py
+-rw-r--r--   0        0        0     2414 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_theme_response.py
+-rw-r--r--   0        0        0     2117 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_theme_response_all_of.py
+-rw-r--r--   0        0        0     2592 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_themes_response.py
+-rw-r--r--   0        0        0     2285 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_themes_response_all_of.py
+-rw-r--r--   0        0        0     2495 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_third_party_auth_response.py
+-rw-r--r--   0        0        0     2171 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     3543 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_need_to_set_password_response.py
+-rw-r--r--   0        0        0     3276 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
+-rw-r--r--   0        0        0     8163 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response.py
+-rw-r--r--   0        0        0     5497 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response_all_of.py
+-rw-r--r--   0        0        0     2395 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
+-rw-r--r--   0        0        0     2307 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_domain_response.py
+-rw-r--r--   0        0        0     2021 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
+-rw-r--r--   0        0        0     2514 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_response.py
+-rw-r--r--   0        0        0     2217 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2776 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/has_data_explorer_features_response.py
+-rw-r--r--   0        0        0     2498 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0      580 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/image_input_scaling.py
+-rw-r--r--   0        0        0     3738 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse.py
+-rw-r--r--   0        0        0     6723 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_block_version.py
+-rw-r--r--   0        0        0     6814 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_dsp_block.py
+-rw-r--r--   0        0        0     1967 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_dsp_block_organization.py
+-rw-r--r--   0        0        0     8958 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_input_block.py
+-rw-r--r--   0        0        0     5612 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_learn_block.py
+-rw-r--r--   0        0        0     2627 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/input_block.py
+-rw-r--r--   0        0        0     2323 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/invite_organization_member_request.py
+-rw-r--r--   0        0        0     4172 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job.py
+-rw-r--r--   0        0        0     2066 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_created_by_user.py
+-rw-r--r--   0        0        0     5203 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details.py
+-rw-r--r--   0        0        0     2736 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_all_of.py
+-rw-r--r--   0        0        0     2613 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_response.py
+-rw-r--r--   0        0        0     2316 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_response_all_of.py
+-rw-r--r--   0        0        0     2257 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_failure_details.py
+-rw-r--r--   0        0        0     2657 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_logs_response.py
+-rw-r--r--   0        0        0     2350 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_logs_response_all_of.py
+-rw-r--r--   0        0        0     3297 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_metrics_response.py
+-rw-r--r--   0        0        0     3007 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_metrics_response_all_of.py
+-rw-r--r--   0        0        0      546 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_parent_type_enum.py
+-rw-r--r--   0        0        0     2944 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_state.py
+-rw-r--r--   0        0        0     1966 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_state_execution_details.py
+-rw-r--r--   0        0        0      598 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_status.py
+-rw-r--r--   0        0        0     2965 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_step.py
+-rw-r--r--   0        0        0     2713 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response.py
+-rw-r--r--   0        0        0     2406 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response_all_of.py
+-rw-r--r--   0        0        0     2089 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response_all_of_summary.py
+-rw-r--r--   0        0        0     1961 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py
+-rw-r--r--   0        0        0     1993 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_custom_metric.py
+-rw-r--r--   0        0        0     2510 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer.py
+-rw-r--r--   0        0        0     2093 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer_input.py
+-rw-r--r--   0        0        0     2101 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer_output.py
+-rw-r--r--   0        0        0     5707 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata.py
+-rw-r--r--   0        0        0     5440 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_all_of.py
+-rw-r--r--   0        0        0     5421 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics.py
+-rw-r--r--   0        0        0     4495 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
+-rw-r--r--   0        0        0     2497 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
+-rw-r--r--   0        0        0      562 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_type_enum.py
+-rw-r--r--   0        0        0      524 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_variant_enum.py
+-rw-r--r--   0        0        0    11377 2024-04-17 10:43:43.018401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_response.py
+-rw-r--r--   0        0        0    11110 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_response_all_of.py
+-rw-r--r--   0        0        0     3392 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_visual_layer.py
+-rw-r--r--   0        0        0     2310 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_visual_layer_type.py
+-rw-r--r--   0        0        0     2529 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/last_modification_date_response.py
+-rw-r--r--   0        0        0     2239 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/last_modification_date_response_all_of.py
+-rw-r--r--   0        0        0     2633 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/latency_device.py
+-rw-r--r--   0        0        0     3146 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/learn_block.py
+-rw-r--r--   0        0        0      933 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/learn_block_type.py
+-rw-r--r--   0        0        0     2788 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     2488 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2704 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2619 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_devices_response.py
+-rw-r--r--   0        0        0     2312 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_devices_response_all_of.py
+-rw-r--r--   0        0        0     2726 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response.py
+-rw-r--r--   0        0        0     2426 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response_all_of.py
+-rw-r--r--   0        0        0     2918 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response_all_of_emails.py
+-rw-r--r--   0        0        0     2767 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_enterprise_trials_response.py
+-rw-r--r--   0        0        0     2467 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py
+-rw-r--r--   0        0        0     2813 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response.py
+-rw-r--r--   0        0        0     2513 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
+-rw-r--r--   0        0        0     2381 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
+-rw-r--r--   0        0        0     2745 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_jobs_response.py
+-rw-r--r--   0        0        0     2445 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_jobs_response_all_of.py
+-rw-r--r--   0        0        0     2200 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_models_response.py
+-rw-r--r--   0        0        0     1910 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_models_response_all_of.py
+-rw-r--r--   0        0        0     2921 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response.py
+-rw-r--r--   0        0        0     2621 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2760 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2752 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_response.py
+-rw-r--r--   0        0        0     2445 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
+-rw-r--r--   0        0        0     2902 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response.py
+-rw-r--r--   0        0        0     2595 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
+-rw-r--r--   0        0        0     2760 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
+-rw-r--r--   0        0        0     3310 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response.py
+-rw-r--r--   0        0        0     3031 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response_all_of.py
+-rw-r--r--   0        0        0     3430 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2887 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
+-rw-r--r--   0        0        0     2587 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2824 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
+-rw-r--r--   0        0        0     2524 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3353 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_files_response.py
+-rw-r--r--   0        0        0     3074 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_files_response_all_of.py
+-rw-r--r--   0        0        0     2792 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2485 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     2857 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response.py
+-rw-r--r--   0        0        0     2550 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response_all_of.py
+-rw-r--r--   0        0        0     2858 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
+-rw-r--r--   0        0        0     3449 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response.py
+-rw-r--r--   0        0        0     3142 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
+-rw-r--r--   0        0        0     2271 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
+-rw-r--r--   0        0        0     2857 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response.py
+-rw-r--r--   0        0        0     2550 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
+-rw-r--r--   0        0        0     2819 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
+-rw-r--r--   0        0        0     3103 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
+-rw-r--r--   0        0        0     2803 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3055 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2755 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2988 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_usage_reports_response.py
+-rw-r--r--   0        0        0     2688 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py
+-rw-r--r--   0        0        0     2786 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organizations_response.py
+-rw-r--r--   0        0        0     2486 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organizations_response_all_of.py
+-rw-r--r--   0        0        0     2512 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_request.py
+-rw-r--r--   0        0        0     2872 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_response.py
+-rw-r--r--   0        0        0     2593 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2290 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_projects.py
+-rw-r--r--   0        0        0     2681 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_projects_response.py
+-rw-r--r--   0        0        0     3122 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2822 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2553 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_projects.py
+-rw-r--r--   0        0        0     2944 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_projects_response.py
+-rw-r--r--   0        0        0     2815 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response.py
+-rw-r--r--   0        0        0     2508 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response_all_of.py
+-rw-r--r--   0        0        0     2290 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2754 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_samples_response.py
+-rw-r--r--   0        0        0     2454 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_samples_response_all_of.py
+-rw-r--r--   0        0        0     2615 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_tuner_runs_response.py
+-rw-r--r--   0        0        0     2308 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_tuner_runs_response_all_of.py
+-rw-r--r--   0        0        0     3933 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response.py
+-rw-r--r--   0        0        0     3633 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of.py
+-rw-r--r--   0        0        0     2353 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
+-rw-r--r--   0        0        0     2053 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
+-rw-r--r--   0        0        0     3960 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2367 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_analytics_event_request.py
+-rw-r--r--   0        0        0     2900 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response.py
+-rw-r--r--   0        0        0     2600 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response_all_of.py
+-rw-r--r--   0        0        0     2441 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
+-rw-r--r--   0        0        0     2191 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_website_pageview_request.py
+-rw-r--r--   0        0        0     2217 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/login_response.py
+-rw-r--r--   0        0        0     1911 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/login_response_all_of.py
+-rw-r--r--   0        0        0     2528 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/memory_spec.py
+-rw-r--r--   0        0        0     2746 2024-04-17 10:43:43.034402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_all_variants_response.py
+-rw-r--r--   0        0        0     2449 2024-04-17 10:43:43.034402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2128 2024-04-17 10:43:43.038401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_for_model_variant.py
+-rw-r--r--   0        0        0     2430 2024-04-17 10:43:43.038401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/migration.py
+-rw-r--r--   0        0        0      571 2024-04-17 10:43:43.038401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_engine_short_enum.py
+-rw-r--r--   0        0        0     3010 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_prediction.py
+-rw-r--r--   0        0        0     2895 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_result.py
+-rw-r--r--   0        0        0     5046 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_variant_stats.py
+-rw-r--r--   0        0        0     2128 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/move_raw_data_request.py
+-rw-r--r--   0        0        0     2784 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_data.py
+-rw-r--r--   0        0        0     3584 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_score.py
+-rw-r--r--   0        0        0     2736 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py
+-rw-r--r--   0        0        0     2687 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/note.py
+-rw-r--r--   0        0        0     2221 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_request.py
+-rw-r--r--   0        0        0     2994 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response.py
+-rw-r--r--   0        0        0     2705 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
+-rw-r--r--   0        0        0     2275 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
+-rw-r--r--   0        0        0     2368 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_count_response.py
+-rw-r--r--   0        0        0     2051 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
+-rw-r--r--   0        0        0     2887 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_response.py
+-rw-r--r--   0        0        0     2580 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
+-rw-r--r--   0        0        0      775 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_last_layer.py
+-rw-r--r--   0        0        0     6491 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config.py
+-rw-r--r--   0        0        0     6949 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_response.py
+-rw-r--r--   0        0        0     1920 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_response_all_of.py
+-rw-r--r--   0        0        0     2056 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_target_device.py
+-rw-r--r--   0        0        0     2271 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_dsp_parameters_response.py
+-rw-r--r--   0        0        0     1964 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_space_response.py
+-rw-r--r--   0        0        0     2456 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_space_response_all_of.py
+-rw-r--r--   0        0        0     5546 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response.py
+-rw-r--r--   0        0        0     5279 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of.py
+-rw-r--r--   0        0        0     3284 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of_status.py
+-rw-r--r--   0        0        0     2273 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
+-rw-r--r--   0        0        0     2749 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
+-rw-r--r--   0        0        0     2425 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
+-rw-r--r--   0        0        0     4717 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
+-rw-r--r--   0        0        0     5801 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization.py
+-rw-r--r--   0        0        0     2700 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_request.py
+-rw-r--r--   0        0        0     2498 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_response.py
+-rw-r--r--   0        0        0     2209 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
+-rw-r--r--   0        0        0     2835 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_dataset_request.py
+-rw-r--r--   0        0        0     2493 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
+-rw-r--r--   0        0        0     2820 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_bucket.py
+-rw-r--r--   0        0        0     2711 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_compute_time_usage.py
+-rw-r--r--   0        0        0     9492 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project.py
+-rw-r--r--   0        0        0      605 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py
+-rw-r--r--   0        0        0     2262 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_path_filter.py
+-rw-r--r--   0        0        0     7464 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_request.py
+-rw-r--r--   0        0        0     2543 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_response.py
+-rw-r--r--   0        0        0     2237 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_response_all_of.py
+-rw-r--r--   0        0        0     2704 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_status_response.py
+-rw-r--r--   0        0        0     2407 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
+-rw-r--r--   0        0        0     2754 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_transformation_summary.py
+-rw-r--r--   0        0        0    10387 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files.py
+-rw-r--r--   0        0        0     2744 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
+-rw-r--r--   0        0        0     3483 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
+-rw-r--r--   0        0        0     2559 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_request.py
+-rw-r--r--   0        0        0     2327 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
+-rw-r--r--   0        0        0     3041 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response.py
+-rw-r--r--   0        0        0     2741 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
+-rw-r--r--   0        0        0     2468 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
+-rw-r--r--   0        0        0     3483 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_export.py
+-rw-r--r--   0        0        0     3476 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_item.py
+-rw-r--r--   0        0        0     2303 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_item_files_inner.py
+-rw-r--r--   0        0        0     4007 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dataset.py
+-rw-r--r--   0        0        0     2800 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dataset_bucket.py
+-rw-r--r--   0        0        0     6005 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_deploy_block.py
+-rw-r--r--   0        0        0     4962 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dsp_block.py
+-rw-r--r--   0        0        0     3037 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response.py
+-rw-r--r--   0        0        0     2737 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
+-rw-r--r--   0        0        0     7063 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
+-rw-r--r--   0        0        0     6864 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response.py
+-rw-r--r--   0        0        0     6574 2024-04-17 10:43:43.058401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of.py
+-rw-r--r--   0        0        0     3915 2024-04-17 10:43:43.058401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
+-rw-r--r--   0        0        0     2267 2024-04-17 10:43:43.058401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
+-rw-r--r--   0        0        0     2338 2024-04-17 10:43:43.058401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
+-rw-r--r--   0        0        0     2458 2024-04-17 10:43:43.058401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
+-rw-r--r--   0        0        0     2101 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_performance.py
+-rw-r--r--   0        0        0      525 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_member_role.py
+-rw-r--r--   0        0        0     2639 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response.py
+-rw-r--r--   0        0        0     2315 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response_all_of.py
+-rw-r--r--   0        0        0     4480 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
+-rw-r--r--   0        0        0     6143 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline.py
+-rw-r--r--   0        0        0     2595 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
+-rw-r--r--   0        0        0     2275 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
+-rw-r--r--   0        0        0     2314 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_item_count.py
+-rw-r--r--   0        0        0     4129 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_run.py
+-rw-r--r--   0        0        0     5330 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_run_step.py
+-rw-r--r--   0        0        0     6532 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_step.py
+-rw-r--r--   0        0        0     2351 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
+-rw-r--r--   0        0        0     2344 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
+-rw-r--r--   0        0        0     2037 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_request.py
+-rw-r--r--   0        0        0     7242 2024-04-17 10:43:43.066401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transfer_learning_block.py
+-rw-r--r--   0        0        0      611 2024-04-17 10:43:43.066401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
+-rw-r--r--   0        0        0     8670 2024-04-17 10:43:43.066401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transformation_block.py
+-rw-r--r--   0        0        0     3918 2024-04-17 10:43:43.066401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_update_pipeline_body.py
+-rw-r--r--   0        0        0     3351 2024-04-17 10:43:43.066401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_usage_report.py
+-rw-r--r--   0        0        0     4882 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_user.py
+-rw-r--r--   0        0        0     2294 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_user_all_of.py
+-rw-r--r--   0        0        0     2104 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_detection.py
+-rw-r--r--   0        0        0     3434 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_false_positive.py
+-rw-r--r--   0        0        0     3770 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_ground_truth.py
+-rw-r--r--   0        0        0     2477 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
+-rw-r--r--   0        0        0     4880 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameter_set.py
+-rw-r--r--   0        0        0     2255 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
+-rw-r--r--   0        0        0     4092 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
+-rw-r--r--   0        0        0     3007 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameters.py
+-rw-r--r--   0        0        0     2585 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameters_standard.py
+-rw-r--r--   0        0        0     2250 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_raw_detection.py
+-rw-r--r--   0        0        0     2366 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
+-rw-r--r--   0        0        0     2412 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
+-rw-r--r--   0        0        0     2106 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
+-rw-r--r--   0        0        0     1839 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/permission.py
+-rw-r--r--   0        0        0     2491 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/portal_file.py
+-rw-r--r--   0        0        0     2537 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/portal_info_response.py
+-rw-r--r--   0        0        0     2666 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/pretrained_model_tensor.py
+-rw-r--r--   0        0        0     2403 2024-04-17 10:43:43.074401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_request.py
+-rw-r--r--   0        0        0     3734 2024-04-17 10:43:43.074401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_response.py
+-rw-r--r--   0        0        0     3467 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2955 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info.py
+-rw-r--r--   0        0        0     3117 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory.py
+-rw-r--r--   0        0        0     1918 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory_eon.py
+-rw-r--r--   0        0        0     2065 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory_tflite.py
+-rw-r--r--   0        0        0     4335 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table.py
+-rw-r--r--   0        0        0     2780 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mcu.py
+-rw-r--r--   0        0        0     3042 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mcu_memory.py
+-rw-r--r--   0        0        0     2250 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mpu.py
+-rw-r--r--   0        0        0     2201 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_tf_lite_request.py
+-rw-r--r--   0        0        0     3292 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_tf_lite_response.py
+-rw-r--r--   0        0        0     7873 2024-04-17 10:43:43.082401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project.py
+-rw-r--r--   0        0        0     4545 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_collaborator.py
+-rw-r--r--   0        0        0     1895 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_collaborator_all_of.py
+-rw-r--r--   0        0        0     2416 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_axes_summary_response.py
+-rw-r--r--   0        0        0     2116 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
+-rw-r--r--   0        0        0     2281 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_interval_response.py
+-rw-r--r--   0        0        0     1964 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_interval_response_all_of.py
+-rw-r--r--   0        0        0     2235 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_summary.py
+-rw-r--r--   0        0        0     6854 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_target.py
+-rw-r--r--   0        0        0     2706 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_target_all_of.py
+-rw-r--r--   0        0        0     2780 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_targets_response.py
+-rw-r--r--   0        0        0     2473 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     1943 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_dismiss_notification_request.py
+-rw-r--r--   0        0        0     2680 2024-04-17 10:43:43.090401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_downloads_response.py
+-rw-r--r--   0        0        0     2373 2024-04-17 10:43:43.090401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_downloads_response_all_of.py
+-rw-r--r--   0        0        0    14783 2024-04-17 10:43:43.090401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response.py
+-rw-r--r--   0        0        0    14516 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of.py
+-rw-r--r--   0        0        0     4174 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
+-rw-r--r--   0        0        0     2723 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
+-rw-r--r--   0        0        0     2997 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
+-rw-r--r--   0        0        0     3200 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
+-rw-r--r--   0        0        0     2339 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_experiments.py
+-rw-r--r--   0        0        0     2285 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_impulse.py
+-rw-r--r--   0        0        0     2726 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_performance.py
+-rw-r--r--   0        0        0     1977 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_readme.py
+-rw-r--r--   0        0        0     2225 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
+-rw-r--r--   0        0        0     2735 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_urls.py
+-rw-r--r--   0        0        0     2478 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_summary_response.py
+-rw-r--r--   0        0        0     2172 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_summary_response_all_of.py
+-rw-r--r--   0        0        0     3554 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_private_data.py
+-rw-r--r--   0        0        0     4127 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_public_data.py
+-rw-r--r--   0        0        0     1928 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_public_data_readme.py
+-rw-r--r--   0        0        0     2404 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_sample_metadata.py
+-rw-r--r--   0        0        0      576 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_tier_enum.py
+-rw-r--r--   0        0        0     2804 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response.py
+-rw-r--r--   0        0        0     2487 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
+-rw-r--r--   0        0        0     2253 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py
+-rw-r--r--   0        0        0      606 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_type.py
+-rw-r--r--   0        0        0     2316 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_version_request.py
+-rw-r--r--   0        0        0      504 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_visibility.py
+-rw-r--r--   0        0        0     4991 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/public_organization_transformation_block.py
+-rw-r--r--   0        0        0     2664 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/raw_sample_data.py
+-rw-r--r--   0        0        0     3440 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/raw_sample_payload.py
+-rw-r--r--   0        0        0     2537 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/rebalance_dataset_response.py
+-rw-r--r--   0        0        0     1984 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/remove_collaborator_request.py
+-rw-r--r--   0        0        0     1805 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/remove_member_request.py
+-rw-r--r--   0        0        0     1867 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_device_request.py
+-rw-r--r--   0        0        0     2081 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_portal_file_request.py
+-rw-r--r--   0        0        0     1867 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_sample_request.py
+-rw-r--r--   0        0        0     2028 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/request_email_verification_request.py
+-rw-r--r--   0        0        0     1873 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/request_reset_password_request.py
+-rw-r--r--   0        0        0     2031 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/reset_password_request.py
+-rw-r--r--   0        0        0     1896 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/resource_range.py
+-rw-r--r--   0        0        0     1985 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/restore_project_from_public_request.py
+-rw-r--r--   0        0        0     2265 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/restore_project_request.py
+-rw-r--r--   0        0        0     2421 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_auto_labeler_request.py
+-rw-r--r--   0        0        0     2669 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_organization_pipeline_response.py
+-rw-r--r--   0        0        0     2352 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
+-rw-r--r--   0        0        0    11134 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample.py
+-rw-r--r--   0        0        0     2443 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample_bounding_boxes_request.py
+-rw-r--r--   0        0        0     2000 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample_metadata.py
+-rw-r--r--   0        0        0     2517 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_request.py
+-rw-r--r--   0        0        0     2071 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py
+-rw-r--r--   0        0        0     2341 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_response.py
+-rw-r--r--   0        0        0     2024 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_pretrained_model_request.py
+-rw-r--r--   0        0        0     3327 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response.py
+-rw-r--r--   0        0        0     3003 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of.py
+-rw-r--r--   0        0        0     2240 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of_latency.py
+-rw-r--r--   0        0        0     1914 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of_ram.py
+-rw-r--r--   0        0        0     2405 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/segment_sample_request.py
+-rw-r--r--   0        0        0     2055 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/segment_sample_request_segments_inner.py
+-rw-r--r--   0        0        0     3346 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/send_user_feedback_request.py
+-rw-r--r--   0        0        0     1981 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/sensor.py
+-rw-r--r--   0        0        0     2142 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_anomaly_parameter_request.py
+-rw-r--r--   0        0        0     9364 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_keras_parameter_request.py
+-rw-r--r--   0        0        0     1893 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_member_datasets_request.py
+-rw-r--r--   0        0        0     1905 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_member_role_request.py
+-rw-r--r--   0        0        0     2219 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_optimize_space_request.py
+-rw-r--r--   0        0        0     2254 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_optimize_space_request_all_of.py
+-rw-r--r--   0        0        0     1923 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_organization_data_dataset_request.py
+-rw-r--r--   0        0        0     1974 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_project_compute_time_request.py
+-rw-r--r--   0        0        0     2011 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_project_dsp_file_size_request.py
+-rw-r--r--   0        0        0     1919 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_sample_metadata_request.py
+-rw-r--r--   0        0        0     2531 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_sample_structured_labels_request.py
+-rw-r--r--   0        0        0     1915 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_syntiant_posterior_request.py
+-rw-r--r--   0        0        0     2140 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_user_password_request.py
+-rw-r--r--   0        0        0     2536 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response.py
+-rw-r--r--   0        0        0     2239 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response_all_of.py
+-rw-r--r--   0        0        0     2059 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response_all_of_token.py
+-rw-r--r--   0        0        0     1971 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/split_sample_in_frames_request.py
+-rw-r--r--   0        0        0     2110 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/staff_info.py
+-rw-r--r--   0        0        0     2292 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_debug_stream_response.py
+-rw-r--r--   0        0        0     1975 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py
+-rw-r--r--   0        0        0     2178 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py
+-rw-r--r--   0        0        0     5388 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_enterprise_trial_request.py
+-rw-r--r--   0        0        0     2226 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_job_response.py
+-rw-r--r--   0        0        0     1909 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_job_response_all_of.py
+-rw-r--r--   0        0        0     2883 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_performance_calibration_request.py
+-rw-r--r--   0        0        0     2838 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_request.py
+-rw-r--r--   0        0        0     2189 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_response.py
+-rw-r--r--   0        0        0     1892 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_response_all_of.py
+-rw-r--r--   0        0        0     2795 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_training_request_anomaly.py
+-rw-r--r--   0        0        0     1926 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/stop_device_debug_stream_request.py
+-rw-r--r--   0        0        0     1967 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/store_segment_length_request.py
+-rw-r--r--   0        0        0     3394 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/structured_classify_result.py
+-rw-r--r--   0        0        0     2270 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/structured_label.py
+-rw-r--r--   0        0        0     4399 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_constraints.py
+-rw-r--r--   0        0        0     2923 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_constraints_device.py
+-rw-r--r--   0        0        0     2347 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_memory.py
+-rw-r--r--   0        0        0     3751 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_processor.py
+-rw-r--r--   0        0        0     2433 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_request.py
+-rw-r--r--   0        0        0     3074 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_response.py
+-rw-r--r--   0        0        0     2784 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3251 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme.py
+-rw-r--r--   0        0        0     2239 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_colors.py
+-rw-r--r--   0        0        0     2764 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_favicon.py
+-rw-r--r--   0        0        0     2721 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_logos.py
+-rw-r--r--   0        0        0     2245 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/third_party_auth.py
+-rw-r--r--   0        0        0     1921 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/time_series_data_point.py
+-rw-r--r--   0        0        0     2031 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_request.py
+-rw-r--r--   0        0        0     2736 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_response.py
+-rw-r--r--   0        0        0     2436 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_response_all_of.py
+-rw-r--r--   0        0        0     5380 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/transfer_learning_model.py
+-rw-r--r--   0        0        0     2012 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/transfer_ownership_organization_request.py
+-rw-r--r--   0        0        0     2585 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_block_additional_mount_point.py
+-rw-r--r--   0        0        0      548 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_job_operates_on_enum.py
+-rw-r--r--   0        0        0      588 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_job_status_enum.py
+-rw-r--r--   0        0        0     2578 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_create_trial_impulse.py
+-rw-r--r--   0        0        0     2462 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_run.py
+-rw-r--r--   0        0        0     2570 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_space_impulse.py
+-rw-r--r--   0        0        0     4991 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial.py
+-rw-r--r--   0        0        0     2739 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_blocks_inner.py
+-rw-r--r--   0        0        0     1935 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
+-rw-r--r--   0        0        0     2211 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_impulse.py
+-rw-r--r--   0        0        0     2028 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_job_request.py
+-rw-r--r--   0        0        0     2281 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_add_collaborator_request.py
+-rw-r--r--   0        0        0     2882 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_bucket_request.py
+-rw-r--r--   0        0        0     2828 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_create_empty_project_request.py
+-rw-r--r--   0        0        0     2428 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_create_project_request.py
+-rw-r--r--   0        0        0     2913 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     4154 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2158 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_item_request.py
+-rw-r--r--   0        0        0     2977 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dataset_request.py
+-rw-r--r--   0        0        0     2518 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dataset_request_bucket.py
+-rw-r--r--   0        0        0     2881 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2724 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_portal_response.py
+-rw-r--r--   0        0        0     2445 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2766 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_request.py
+-rw-r--r--   0        0        0     5211 2024-04-17 10:43:43.118401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     6072 2024-04-17 10:43:43.122401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_transformation_block_request.py
+-rw-r--r--   0        0        0    11806 2024-04-17 10:43:43.122401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_project_request.py
+-rw-r--r--   0        0        0     1877 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_project_tags_request.py
+-rw-r--r--   0        0        0     2259 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_theme_colors_request.py
+-rw-r--r--   0        0        0     2895 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_theme_logos_request.py
+-rw-r--r--   0        0        0     2205 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_third_party_auth_request.py
+-rw-r--r--   0        0        0     1865 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_tuner_run_request.py
+-rw-r--r--   0        0        0     2375 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_user_request.py
+-rw-r--r--   0        0        0     1886 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_version_request.py
+-rw-r--r--   0        0        0     2393 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
+-rw-r--r--   0        0        0     2237 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
+-rw-r--r--   0        0        0     2125 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
+-rw-r--r--   0        0        0     2155 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py
+-rw-r--r--   0        0        0     2059 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_request.py
+-rw-r--r--   0        0        0     2168 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_asset_response.py
+-rw-r--r--   0        0        0     1882 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_asset_response_all_of.py
+-rw-r--r--   0        0        0     2199 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_readme_image_response.py
+-rw-r--r--   0        0        0     2185 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_user_photo_response.py
+-rw-r--r--   0        0        0     1872 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_user_photo_response_all_of.py
+-rw-r--r--   0        0        0     4330 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user.py
+-rw-r--r--   0        0        0     1991 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_by_third_party_activation_request.py
+-rw-r--r--   0        0        0     1956 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py
+-rw-r--r--   0        0        0     1922 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_dismiss_notification_request.py
+-rw-r--r--   0        0        0     2192 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_experiment.py
+-rw-r--r--   0        0        0     2425 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_generate_new_mfa_key_response.py
+-rw-r--r--   0        0        0     2119 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py
+-rw-r--r--   0        0        0     4606 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_organization.py
+-rw-r--r--   0        0        0     2144 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_request.py
+-rw-r--r--   0        0        0     2480 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_response.py
+-rw-r--r--   0        0        0     2191 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py
+-rw-r--r--   0        0        0      543 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_tier_enum.py
+-rw-r--r--   0        0        0     1844 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_request.py
+-rw-r--r--   0        0        0     2604 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response.py
+-rw-r--r--   0        0        0     2307 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
+-rw-r--r--   0        0        0     3049 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
+-rw-r--r--   0        0        0     2633 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_email_response.py
+-rw-r--r--   0        0        0     2354 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_email_response_all_of.py
+-rw-r--r--   0        0        0     2708 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_request.py
+-rw-r--r--   0        0        0     3432 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response.py
+-rw-r--r--   0        0        0     3155 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2187 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
+-rw-r--r--   0        0        0     1961 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_existing_bucket_request.py
+-rw-r--r--   0        0        0     1937 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_reset_password_request.py
+-rw-r--r--   0        0        0     8565 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel.py
+-rw-r--r--   0        0        0     2534 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
+-rw-r--r--   0        0        0     2085 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py
+-rw-r--r--   0        0        0     2120 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
+-rw-r--r--   0        0        0     2885 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response.py
+-rw-r--r--   0        0        0     2585 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response_all_of.py
+-rw-r--r--   0        0        0     2848 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
+-rw-r--r--   0        0        0    12674 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/rest.py
+-rw-r--r--   0        0        0     1019 2024-04-17 10:44:15.302117 edgeimpulse_api-1.49.9/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 edgeimpulse_api-1.49.9/PKG-INFO
```

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/__init__.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.49.8" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+__version__ = "1.49.9" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 
 # import apis into sdk package
 from edgeimpulse_api.api.admin_api import AdminApi
 from edgeimpulse_api.api.auth_api import AuthApi
 from edgeimpulse_api.api.cdn_api import CDNApi
 from edgeimpulse_api.api.classify_api import ClassifyApi
 from edgeimpulse_api.api.dsp_api import DSPApi
```

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/__init__.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/admin_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/auth_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/cdn_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/cdn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/classify_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/classify_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/deployment_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/deployment_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/devices_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/devices_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/dsp_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/dsp_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/email_verification_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/email_verification_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/export_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/feature_flags_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/feature_flags_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/health_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/health_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/impulse_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/impulse_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/jobs_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/learn_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/learn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/login_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/login_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/metrics_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/optimization_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/optimization_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_blocks_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_blocks_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_create_project_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_create_project_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_data_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_data_campaigns_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_data_campaigns_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_jobs_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_pipelines_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_pipelines_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/organization_portals_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_portals_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/organizations_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/performance_calibration_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/performance_calibration_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/projects_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/raw_data_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/raw_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/themes_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/themes_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/third_party_auth_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/third_party_auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/upload_portal_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/upload_portal_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/user_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/user_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api/whitelabels_api.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api/whitelabels_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/api_client.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/api_client.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/configuration.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/configuration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/exceptions.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/__init__.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/activate_user_or_verify_email_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/activate_user_or_verify_email_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_api_key_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_collaborator_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_hmac_key_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_hmac_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_member_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_api_key_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_api_key_request_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_bucket_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_deploy_block_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_dsp_block_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_dsp_block_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_secret_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_secret_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_secret_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_transformation_block_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_transformation_block_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_project_api_key_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_project_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/add_project_api_key_request_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_project_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_organization_api_key_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_organization_user_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_project_api_key_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_project_user_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_add_user_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_api_organization.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_api_organization_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_organization_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_api_project.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_api_user.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,23 +39,25 @@
     pending: StrictBool = ...
     last_tos_acceptance_date: Optional[datetime] = Field(None, alias="lastTosAcceptanceDate")
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
     permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
     company_name: Optional[StrictStr] = Field(None, alias="companyName")
     activated: StrictBool = ...
     mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
+    stripe_customer_id: Optional[StrictStr] = Field(None, alias="stripeCustomerId", description="Stripe customer ID, if any.")
+    has_pending_payments: Optional[StrictBool] = Field(None, alias="hasPendingPayments", description="Whether the user has pending payments.")
     organizations: List[UserOrganization] = Field(..., description="Organizations that the user is a member of. Only filled when requesting information about yourself.")
     projects: List[Project] = ...
     experiments: List[UserExperiment] = Field(..., description="Experiments the user has access to. Enabling experiments can only be done through a JWT token.")
     evaluation: Optional[StrictBool] = Field(None, description="Whether this is an ephemeral evaluation account.")
     ambassador: Optional[StrictBool] = Field(None, description="Whether this user is an ambassador.")
     tier: UserTierEnum = ...
     suspended: StrictBool = Field(..., description="Whether the user is suspended.")
     trials: List[EnterpriseTrial] = Field(..., description="Current or past enterprise trials.")
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "organizations", "projects", "experiments", "evaluation", "ambassador", "tier", "suspended", "trials"]
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "organizations", "projects", "experiments", "evaluation", "ambassador", "tier", "suspended", "trials"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -130,14 +132,16 @@
             "pending": obj.get("pending"),
             "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
             "job_title": obj.get("jobTitle"),
             "permissions": obj.get("permissions"),
             "company_name": obj.get("companyName"),
             "activated": obj.get("activated"),
             "mfa_configured": obj.get("mfaConfigured"),
+            "stripe_customer_id": obj.get("stripeCustomerId"),
+            "has_pending_payments": obj.get("hasPendingPayments"),
             "organizations": [UserOrganization.from_dict(_item) for _item in obj.get("organizations")] if obj.get("organizations") is not None else None,
             "projects": [Project.from_dict(_item) for _item in obj.get("projects")] if obj.get("projects") is not None else None,
             "experiments": [UserExperiment.from_dict(_item) for _item in obj.get("experiments")] if obj.get("experiments") is not None else None,
             "evaluation": obj.get("evaluation"),
             "ambassador": obj.get("ambassador"),
             "tier": obj.get("tier"),
             "suspended": obj.get("suspended"),
```

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_api_user_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_create_organization_data_export_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_organization_data_export_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_create_organization_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_create_project_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_enable_feature_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_enable_feature_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_data_migration_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migration_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_data_migrations_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migrations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_metrics_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_metrics_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organization_usage_report_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organizations_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organizations_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_sso_settings_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_ids_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_ids_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_metrics_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_trial_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_users_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_users_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_get_users_response_all_of_users.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_list_projects.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_list_projects_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_organization_info_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_organization_info_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_toggle_data_migration_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_toggle_data_migration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_update_organization_data_export_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_organization_data_export_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_update_organization_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_update_user_permissions_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_permissions_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_update_user_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/admin_update_user_trial_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_trial_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/akida_edge_learning_config.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/akida_edge_learning_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_capacity.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_capacity.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_gmm_metadata.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_gmm_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_model_metadata.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_model_metadata_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_response_all_of_axes.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response_all_of_axes.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_result.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_trained_features_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/application_budget.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/application_budget.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/augmentation_policy_spectrogram.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/augmentation_policy_spectrogram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/autotune_dsp_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/autotune_dsp_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/block_type.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/block_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/bounding_box.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/bounding_box_with_score.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/bounding_box_with_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/build_on_device_model_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/build_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/build_organization_on_device_model_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/build_organization_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/calculate_data_quality_metrics_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/calculate_data_quality_metrics_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/change_password_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/change_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response_page.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_page.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_job_response_page_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_page_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_sample_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_sample_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_sample_response_classification.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_sample_response_classification_details.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_classification_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/classify_sample_v2200_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_v2200_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/convert_user_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/convert_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/cosine_similarity_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/cosine_similarity_issue.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/count_samples_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/count_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/count_samples_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/count_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_block_version_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_block_version_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_block_version_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_block_version_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_developer_profile_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_developer_profile_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_developer_profile_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_developer_profile_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_device_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_enterprise_trial_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_enterprise_trial_user_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_evaluation_user_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_evaluation_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_evaluation_user_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_evaluation_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_portal_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_portal_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_portal_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_organization_usage_report_body.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_usage_report_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_pipeline_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_project_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_project_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_project_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_signed_upload_link_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_signed_upload_link_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_third_party_auth_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_third_party_auth_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_third_party_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_third_party_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_user_third_party_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_whitelabel_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_whitelabel_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/create_whitelabel_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/created_updated_by_user.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/created_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/crop_sample_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/crop_sample_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/crop_sample_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/cross_validation_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cross_validation_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/cross_validation_data_scores_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cross_validation_data_scores_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_dashboard.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_dashboard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_graph.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_link.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_link.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_campaign_query.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_query.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_explorer_predictions_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_predictions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/data_explorer_settings.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dataset_ratio_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dataset_ratio_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dataset_ratio_data_ratio.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dataset_ratio_data_ratio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/delete_portal_file_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/delete_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dependency_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dependency_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_input_image.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_image.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_input_other.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_other.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deployment_target.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deployment_target_badge.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target_badge.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deployment_target_engine.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target_engine.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deployment_targets_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/deployment_targets_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_board_created_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_created_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_board_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_board_request_update.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_request_update.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_board_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_boards_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_boards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_boards_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_boards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_keys.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/development_keys_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/device.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/device_debug_stream_type.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_debug_stream_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/device_inference_info.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_inference_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/device_name_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_name_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/device_name_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_name_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/device_sensors_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_sensors_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/download.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/download.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/download_portal_file_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/download_portal_file_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/download_portal_file_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_autotuner_results.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_autotuner_results_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_config_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_config_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_config_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_importance_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_labels_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_labels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_group.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_group_item.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_group_item_select_options_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item_select_options_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_group_item_show_if.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item_show_if.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_info.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_info_features.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_info_performance.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_metadata.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_metadata_output_config.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_output_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_metadata_output_config_shape.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_output_config_shape.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_metadata_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_named_axis.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_named_axis.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_performance_all_variants_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_graph.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_graph_axis_labels.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_graph_axis_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_request_with_features.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_with_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_request_without_features.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_without_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_response_all_of_performance.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_response_with_sample.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_with_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_sample_features_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_sample_features_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_trained_features_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_trained_features_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/edit_sample_label_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/edit_sample_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/enterprise_trial.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/enterprise_trial.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/entitlement_limits.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/entitlement_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/entity_created_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/entity_created_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/entity_created_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/entity_created_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/evaluate_job_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/evaluate_job_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/evaluate_result_value.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_result_value.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_block_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_block_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_get_url_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_get_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_get_url_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_get_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_keras_block_data_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_keras_block_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_original_data_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_original_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/export_wav_data_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_wav_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_segment_sample_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_segment_sample_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_segment_sample_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_user_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_user_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/find_user_response_all_of_users.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/generate_features_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/generate_features_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/generic_api_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/generic_api_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_imported_from_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_imported_from_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_third_party_auth_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_whitelabels_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_whitelabels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_auto_labeler_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_auto_labeler_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_data_explorer_features_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_data_explorer_settings_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_deployment_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_deployment_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_deployment_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_deployment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_device_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_device_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_device_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_device_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_diversity_data_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_diversity_data_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_email_verification_code_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_code_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_email_verification_code_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_code_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_email_verification_status_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_email_verification_status_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_feature_flags_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_feature_flags_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_blocks_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_records_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_records_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_records_request_range.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_records_request_range.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_impulse_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_job_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_job_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_jwt_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_jwt_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_jwt_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_label_noise_data_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_label_noise_data_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_last_deployment_build_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_notes_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_notes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_notes_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_notes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_bucket_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_bucket_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_bucket_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaign_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaigns_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_export_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_export_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_export_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_export_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_exports_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_exports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_item_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_item_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_dataset_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_dataset_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dataset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_deploy_block_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_dsp_block_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_pipelines_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_portal_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_portal_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_projects_data_count_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_projects_data_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_transformation_block_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_organization_usage_report_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_parameters_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_status_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_pretrained_model_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_public_metrics_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_public_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_public_metrics_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_public_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_sample_metadata_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_sample_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_sample_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_syntiant_posterior_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_syntiant_posterior_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_target_constraints_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_target_constraints_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_target_constraints_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_target_constraints_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_theme_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_theme_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_theme_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_theme_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_themes_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_themes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_themes_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_themes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_third_party_auth_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_user_need_to_set_password_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_need_to_set_password_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_user_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,24 +41,26 @@
     pending: StrictBool = ...
     last_tos_acceptance_date: Optional[datetime] = Field(None, alias="lastTosAcceptanceDate")
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
     permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
     company_name: Optional[StrictStr] = Field(None, alias="companyName")
     activated: StrictBool = ...
     mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
+    stripe_customer_id: Optional[StrictStr] = Field(None, alias="stripeCustomerId", description="Stripe customer ID, if any.")
+    has_pending_payments: Optional[StrictBool] = Field(None, alias="hasPendingPayments", description="Whether the user has pending payments.")
     organizations: List[UserOrganization] = Field(..., description="Organizations that the user is a member of. Only filled when requesting information about yourself.")
     projects: List[Project] = ...
     experiments: List[UserExperiment] = Field(..., description="Experiments the user has access to. Enabling experiments can only be done through a JWT token.")
     evaluation: Optional[StrictBool] = Field(None, description="Whether this is an ephemeral evaluation account.")
     ambassador: Optional[StrictBool] = Field(None, description="Whether this user is an ambassador.")
     tier: UserTierEnum = ...
     whitelabels: Optional[List[GetUserResponseAllOfWhitelabels]] = Field(None, description="List of white labels the user is a member of")
     suspended: StrictBool = Field(..., description="Whether the user is suspended.")
     notifications: List[StrictStr] = Field(..., description="List of notifications to show to the user")
-    __properties = ["success", "error", "id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "organizations", "projects", "experiments", "evaluation", "ambassador", "tier", "whitelabels", "suspended", "notifications"]
+    __properties = ["success", "error", "id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "organizations", "projects", "experiments", "evaluation", "ambassador", "tier", "whitelabels", "suspended", "notifications"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -135,14 +137,16 @@
             "pending": obj.get("pending"),
             "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
             "job_title": obj.get("jobTitle"),
             "permissions": obj.get("permissions"),
             "company_name": obj.get("companyName"),
             "activated": obj.get("activated"),
             "mfa_configured": obj.get("mfaConfigured"),
+            "stripe_customer_id": obj.get("stripeCustomerId"),
+            "has_pending_payments": obj.get("hasPendingPayments"),
             "organizations": [UserOrganization.from_dict(_item) for _item in obj.get("organizations")] if obj.get("organizations") is not None else None,
             "projects": [Project.from_dict(_item) for _item in obj.get("projects")] if obj.get("projects") is not None else None,
             "experiments": [UserExperiment.from_dict(_item) for _item in obj.get("experiments")] if obj.get("experiments") is not None else None,
             "evaluation": obj.get("evaluation"),
             "ambassador": obj.get("ambassador"),
             "tier": obj.get("tier"),
             "whitelabels": [GetUserResponseAllOfWhitelabels.from_dict(_item) for _item in obj.get("whitelabels")] if obj.get("whitelabels") is not None else None,
```

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_user_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_whitelabel_domain_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_domain_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_whitelabel_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/get_whitelabel_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/has_data_explorer_features_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/has_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/image_input_scaling.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/image_input_scaling.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse_block_version.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_block_version.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse_dsp_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse_dsp_block_organization.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_dsp_block_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse_input_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/impulse_learn_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/input_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/invite_organization_member_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/invite_organization_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_created_by_user.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_created_by_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_details.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_details_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_details_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_details_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_failure_details.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_failure_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_logs_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_logs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_logs_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_logs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_metrics_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_metrics_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_parent_type_enum.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_parent_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_state.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_state.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_state_execution_details.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_state_execution_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_status.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_step.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_summary_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_summary_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/job_summary_response_all_of_summary.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response_all_of_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_custom_metric.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_custom_metric.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_layer.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_layer_input.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_layer_output.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer_output.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_metadata.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_metadata_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_metadata_metrics.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_type_enum.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_model_variant_enum.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_variant_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_visual_layer.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_visual_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/keras_visual_layer_type.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_visual_layer_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/last_modification_date_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/last_modification_date_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/last_modification_date_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/last_modification_date_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/latency_device.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/latency_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/learn_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/learn_block_type.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/learn_block_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_api_keys_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_api_keys_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_devices_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_devices_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_devices_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_devices_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_email_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_email_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_email_response_all_of_emails.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response_all_of_emails.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_enterprise_trials_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_enterprise_trials_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_hmac_keys_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_hmac_keys_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_jobs_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_jobs_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_models_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_models_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_api_keys_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_buckets_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_buckets_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_buckets_user_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_data_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_data_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_data_response_all_of_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_deploy_blocks_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_deploy_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_dsp_blocks_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_dsp_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_files_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_files_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_files_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_files_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_pipelines_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_portals_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_portals_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_projects_data_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_secrets_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_secrets_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_usage_reports_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_usage_reports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organizations_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_organizations_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_portal_files_in_folder_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_portal_files_in_folder_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_projects.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_projects_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_projects.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_projects_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_versions_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_versions_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_samples_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_samples_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_tuner_runs_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_tuner_runs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_tuner_runs_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_tuner_runs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_versions_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_versions_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_versions_response_all_of_bucket.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/list_versions_response_all_of_versions.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/log_analytics_event_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_analytics_event_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/log_stdout_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/log_stdout_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/log_website_pageview_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_website_pageview_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/login_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/login_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/login_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/login_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/memory_spec.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/memory_spec.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/metrics_all_variants_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/metrics_all_variants_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/metrics_for_model_variant.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_for_model_variant.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/migration.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/migration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/model_engine_short_enum.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_engine_short_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/model_prediction.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_prediction.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/model_result.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/model_variant_stats.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_variant_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/move_raw_data_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/move_raw_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/neighbors_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/neighbors_score.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/note.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/note.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_auto_label_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_auto_label_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_label_queue_count_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_label_queue_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/object_detection_last_layer.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_last_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_config.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_config_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_config_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_config_target_device.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_target_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_dsp_parameters_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_dsp_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_space_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_space_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_space_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_space_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_state_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_state_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_state_response_all_of_status.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_state_response_all_of_workers.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of_workers.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_transfer_learning_models_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_add_data_folder_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_add_data_folder_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_add_dataset_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_add_dataset_request_bucket.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_dataset_request_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_bucket.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_compute_time_usage.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_compute_time_usage.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_path_filter.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_path_filter.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_status_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_status_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_transformation_summary.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_transformation_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_with_files.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_with_files_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_campaign_diff_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_campaign_diff_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_export.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_export.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_item.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_data_item_files_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_item_files_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_dataset.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_dataset_bucket.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dataset_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_deploy_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_deploy_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_dsp_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_get_create_projects_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_info_response_all_of_performance.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_member_role.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_member_role.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_metrics_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_metrics_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_item_count.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_item_count.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_run.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_run_step.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_run_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_pipeline_step.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_projects_data_batch_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_transfer_learning_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transfer_learning_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_transfer_learning_operates_on.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transfer_learning_operates_on.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_transformation_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_update_pipeline_body.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_update_pipeline_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_usage_report.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_usage_report.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_user.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,19 +35,21 @@
     pending: StrictBool = ...
     last_tos_acceptance_date: Optional[datetime] = Field(None, alias="lastTosAcceptanceDate")
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
     permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
     company_name: Optional[StrictStr] = Field(None, alias="companyName")
     activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
     mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
+    stripe_customer_id: Optional[StrictStr] = Field(None, alias="stripeCustomerId", description="Stripe customer ID, if any.")
+    has_pending_payments: Optional[StrictBool] = Field(None, alias="hasPendingPayments", description="Whether the user has pending payments.")
     added: datetime = ...
     role: OrganizationMemberRole = ...
     project_count: StrictInt = Field(..., alias="projectCount")
     datasets: List[StrictStr] = ...
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "added", "role", "projectCount", "datasets"]
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "added", "role", "projectCount", "datasets"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -94,14 +96,16 @@
             "pending": obj.get("pending"),
             "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
             "job_title": obj.get("jobTitle"),
             "permissions": obj.get("permissions"),
             "company_name": obj.get("companyName"),
             "activated": obj.get("activated"),
             "mfa_configured": obj.get("mfaConfigured"),
+            "stripe_customer_id": obj.get("stripeCustomerId"),
+            "has_pending_payments": obj.get("hasPendingPayments"),
             "added": obj.get("added"),
             "role": obj.get("role"),
             "project_count": obj.get("projectCount"),
             "datasets": obj.get("datasets")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/organization_user_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_detection.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_false_positive.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_false_positive.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_ground_truth.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_ground_truth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_parameter_set.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameter_set.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_parameters.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_parameters_standard.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameters_standard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_raw_detection.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_raw_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/permission.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/permission.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/portal_file.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/portal_file.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/portal_info_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/portal_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/pretrained_model_tensor.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/pretrained_model_tensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/preview_default_files_in_folder_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/preview_default_files_in_folder_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_info.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_info_memory.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_info_memory_eon.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory_eon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_info_memory_tflite.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_table.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_table_mcu.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mcu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_table_mcu_memory.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mcu_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_model_table_mpu.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mpu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_tf_lite_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_tf_lite_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/profile_tf_lite_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_tf_lite_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_collaborator.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_collaborator.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,16 +34,18 @@
     pending: StrictBool = ...
     last_tos_acceptance_date: Optional[datetime] = Field(None, alias="lastTosAcceptanceDate")
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
     permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
     company_name: Optional[StrictStr] = Field(None, alias="companyName")
     activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
     mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
+    stripe_customer_id: Optional[StrictStr] = Field(None, alias="stripeCustomerId", description="Stripe customer ID, if any.")
+    has_pending_payments: Optional[StrictBool] = Field(None, alias="hasPendingPayments", description="Whether the user has pending payments.")
     is_owner: StrictBool = Field(..., alias="isOwner")
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "isOwner"]
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "isOwner"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -90,11 +92,13 @@
             "pending": obj.get("pending"),
             "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
             "job_title": obj.get("jobTitle"),
             "permissions": obj.get("permissions"),
             "company_name": obj.get("companyName"),
             "activated": obj.get("activated"),
             "mfa_configured": obj.get("mfaConfigured"),
+            "stripe_customer_id": obj.get("stripeCustomerId"),
+            "has_pending_payments": obj.get("hasPendingPayments"),
             "is_owner": obj.get("isOwner")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_collaborator_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_collaborator_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_data_axes_summary_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_axes_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_data_interval_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_interval_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_data_interval_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_interval_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_data_summary.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_deployment_target.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_deployment_target_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_target_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_deployment_targets_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_deployment_targets_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_dismiss_notification_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_dismiss_notification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_downloads_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_downloads_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_downloads_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_downloads_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_compute_time.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_compute_time.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_experiments.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_experiments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_impulse.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_performance.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_readme.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_response_all_of_urls.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_urls.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_summary_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_info_summary_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_private_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_private_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_public_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_public_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_public_data_readme.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_public_data_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_sample_metadata.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_tier_enum.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_tier_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_training_data_summary_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_training_data_summary_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_type.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/project_version_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/public_organization_transformation_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/public_organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/raw_sample_data.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/raw_sample_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/raw_sample_payload.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/raw_sample_payload.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/rebalance_dataset_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/rebalance_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/remove_collaborator_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/remove_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/remove_member_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/remove_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/rename_device_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/rename_portal_file_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/rename_sample_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/request_email_verification_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/request_email_verification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/request_reset_password_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/request_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/reset_password_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/resource_range.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/resource_range.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/restore_project_from_public_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/restore_project_from_public_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/restore_project_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/restore_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/run_auto_labeler_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_auto_labeler_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/run_organization_pipeline_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_organization_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/sample.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/sample_bounding_boxes_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample_bounding_boxes_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/sample_metadata.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/save_auto_labeler_clusters_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/save_auto_labeler_clusters_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/save_pretrained_model_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/score_trial_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/score_trial_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/score_trial_response_all_of_latency.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of_latency.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/score_trial_response_all_of_ram.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of_ram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/segment_sample_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/segment_sample_request_segments_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/segment_sample_request_segments_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/send_user_feedback_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/send_user_feedback_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/sensor.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/sensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_anomaly_parameter_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_anomaly_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_keras_parameter_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_keras_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_member_datasets_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_member_datasets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_member_role_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_member_role_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_optimize_space_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_optimize_space_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_optimize_space_request_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_optimize_space_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_organization_data_dataset_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_organization_data_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_project_compute_time_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_project_compute_time_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_project_dsp_file_size_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_project_dsp_file_size_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_sample_metadata_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_sample_metadata_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_sample_structured_labels_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_sample_structured_labels_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_syntiant_posterior_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_syntiant_posterior_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/set_user_password_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_user_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/socket_token_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/socket_token_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/socket_token_response_all_of_token.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response_all_of_token.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/split_sample_in_frames_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/split_sample_in_frames_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/staff_info.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/staff_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_device_debug_stream_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_debug_stream_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_enterprise_trial_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_enterprise_trial_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_job_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_job_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_performance_calibration_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_performance_calibration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_sampling_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_sampling_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_sampling_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/start_training_request_anomaly.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_training_request_anomaly.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/stop_device_debug_stream_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/stop_device_debug_stream_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/store_segment_length_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/store_segment_length_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/structured_classify_result.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/structured_classify_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/structured_label.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/structured_label.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/target_constraints.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_constraints.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/target_constraints_device.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_constraints_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/target_memory.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/target_processor.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_processor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/test_pretrained_model_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/test_pretrained_model_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/test_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/theme.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/theme_colors.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_colors.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/theme_favicon.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_favicon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/theme_logos.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_logos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/third_party_auth.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/third_party_auth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/time_series_data_point.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/time_series_data_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/track_objects_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/track_objects_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/track_objects_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/transfer_learning_model.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/transfer_ownership_organization_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/transfer_ownership_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/transformation_block_additional_mount_point.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_block_additional_mount_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/transformation_job_operates_on_enum.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_job_operates_on_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/transformation_job_status_enum.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_job_status_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_create_trial_impulse.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_create_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_run.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_space_impulse.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_space_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_trial.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_trial_blocks_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_trial_dsp_job_id.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_dsp_job_id.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/tuner_trial_impulse.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_job_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_job_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_add_collaborator_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_bucket_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_create_empty_project_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_create_empty_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_create_project_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_data_campaign_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_data_item_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_item_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_dataset_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_dataset_request_bucket.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dataset_request_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_dsp_block_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_portal_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_portal_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_organization_transformation_block_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_project_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_project_tags_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_project_tags_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_theme_colors_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_theme_colors_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_theme_logos_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_theme_logos_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_third_party_auth_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_tuner_run_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_tuner_run_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_user_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_version_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/update_whitelabel_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/upload_asset_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_asset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/upload_asset_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_asset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/upload_readme_image_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_readme_image_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/upload_user_photo_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_user_photo_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/upload_user_photo_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_user_photo_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,17 @@
     pending: StrictBool = ...
     last_tos_acceptance_date: Optional[datetime] = Field(None, alias="lastTosAcceptanceDate")
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
     permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
     company_name: Optional[StrictStr] = Field(None, alias="companyName")
     activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
     mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured"]
+    stripe_customer_id: Optional[StrictStr] = Field(None, alias="stripeCustomerId", description="Stripe customer ID, if any.")
+    has_pending_payments: Optional[StrictBool] = Field(None, alias="hasPendingPayments", description="Whether the user has pending payments.")
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -88,11 +90,13 @@
             "staff_info": StaffInfo.from_dict(obj.get("staffInfo")) if obj.get("staffInfo") is not None else None,
             "pending": obj.get("pending"),
             "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
             "job_title": obj.get("jobTitle"),
             "permissions": obj.get("permissions"),
             "company_name": obj.get("companyName"),
             "activated": obj.get("activated"),
-            "mfa_configured": obj.get("mfaConfigured")
+            "mfa_configured": obj.get("mfaConfigured"),
+            "stripe_customer_id": obj.get("stripeCustomerId"),
+            "has_pending_payments": obj.get("hasPendingPayments")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_by_third_party_activation_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_by_third_party_activation_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_dismiss_notification_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_dismiss_notification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_experiment.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_experiment.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_generate_new_mfa_key_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_generate_new_mfa_key_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_organization.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_set_totp_mfa_key_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_set_totp_mfa_key_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/user_tier_enum.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_tier_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_dsp_block_url_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_dsp_block_url_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_email_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_email_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_email_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_organization_bucket_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_organization_bucket_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_organization_existing_bucket_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_existing_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/verify_reset_password_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/whitelabel.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/window_settings_response.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/window_settings_response_all_of.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/edgeimpulse_api/rest.py` & `edgeimpulse_api-1.49.9/edgeimpulse_api/rest.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.8/pyproject.toml` & `edgeimpulse_api-1.49.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgeimpulse-api"
-version = "1.49.8" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+version = "1.49.9" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 description = "Python bindings for the Edge Impulse API."
 authors = ["EdgeImpulse Inc. <hello@edgeimpulse.com>"]
 license = "Apache-2.0"
 homepage = "https://edgeimpulse.com"
 documentation = "https://docs.edgeimpulse.com/reference/edge-impulse-api/edge-impulse-api"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `edgeimpulse_api-1.49.8/PKG-INFO` & `edgeimpulse_api-1.49.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgeimpulse-api
-Version: 1.49.8
+Version: 1.49.9
 Summary: Python bindings for the Edge Impulse API.
 Home-page: https://edgeimpulse.com
 License: Apache-2.0
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

