# Comparing `tmp/py-scibec-openapi-client-1.8.5.tar.gz` & `tmp/py-scibec-openapi-client-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-scibec-openapi-client-1.8.5.tar", last modified: Tue Jan 16 13:19:48 2024, max compression
+gzip compressed data, was "py-scibec-openapi-client-1.8.6.tar", last modified: Tue Jan 16 13:23:15 2024, max compression
```

## Comparing `py-scibec-openapi-client-1.8.5.tar` & `py-scibec-openapi-client-1.8.6.tar`

### file list

```diff
@@ -1,659 +1,659 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.491363 py-scibec-openapi-client-1.8.5/
--rw-r--r--   0 root         (0) root         (0)      293 2024-01-16 13:19:48.491363 py-scibec-openapi-client-1.8.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    31635 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.450359 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    58504 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.450359 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7789 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.454359 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/access_accounts.py
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/access_accounts_count.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/access_accounts_id.py
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/access_configs.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/access_configs_count.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/access_configs_id.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/auth_callback.py
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/auth_login.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/auth_logout.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/beamlines.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/beamlines_count.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/beamlines_id.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/datasets_count.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/datasets_id.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/devices.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/devices_count.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/devices_id.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/events.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/events_count.py
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/events_id.py
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/experiment_accounts.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/experiment_accounts_count.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/experiment_accounts_id.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/experiments.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/experiments_count.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/experiments_id.py
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/functional_accounts.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/functional_accounts_count.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/functional_accounts_id.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/nxentities.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/nxentities_count.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/nxentities_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/nxentities_id.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/scans.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/scans_count.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/scans_id.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/sessions_count.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/sessions_id.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/users.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/users_login.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/users_me.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/paths/users_user_id.py
--rw-rw-rw-   0 root         (0) root         (0)     3301 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.455359 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/access_account_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/access_config_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/beamline_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1190 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/dataset_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/device_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/event_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/experiment_account_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/experiment_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/functional_account_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1475 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/nx_entity_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)      746 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/oidc_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/scan_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1190 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/session_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/user_controller_api.py
--rw-rw-rw-   0 root         (0) root         (0)    15715 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4478 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.463360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10673 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_account.py
--rw-rw-rw-   0 root         (0) root         (0)    24644 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_account_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    26497 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_account_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)    10726 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_account_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    10784 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_account_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)    11368 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config.py
--rw-rw-rw-   0 root         (0) root         (0)    28026 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    29879 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)     3760 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)    11363 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    16991 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    14045 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)     8523 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline.py
--rw-rw-rw-   0 root         (0) root         (0)    24578 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    26431 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)     3711 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)     8571 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    16983 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    11117 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)     9022 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    25520 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    27373 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)     3668 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)     9102 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    16981 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    11454 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)    17398 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device.py
--rw-rw-rw-   0 root         (0) root         (0)    35363 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    37216 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)    17369 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    16979 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    21971 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)     9548 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event.py
--rw-rw-rw-   0 root         (0) root         (0)    26461 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    28314 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)     3630 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)     9626 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    16977 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    11072 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)    13662 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment.py
--rw-rw-rw-   0 root         (0) root         (0)    11800 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account.py
--rw-rw-rw-   0 root         (0) root         (0)    26576 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    28429 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)    11857 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    17001 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    12711 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)    32162 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    34015 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)     4093 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)    13697 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    16987 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    20208 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)    11826 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account.py
--rw-rw-rw-   0 root         (0) root         (0)    26602 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    28455 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)     3599 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)    11883 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    17001 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    12772 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)     2396 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/loopback_count.py
--rw-rw-rw-   0 root         (0) root         (0)    10278 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_access_account.py
--rw-rw-rw-   0 root         (0) root         (0)    10971 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_access_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8118 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_beamline.py
--rw-rw-rw-   0 root         (0) root         (0)     8615 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    16989 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_device.py
--rw-rw-rw-   0 root         (0) root         (0)     9137 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_event.py
--rw-rw-rw-   0 root         (0) root         (0)    13261 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_experiment.py
--rw-rw-rw-   0 root         (0) root         (0)    11413 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_experiment_account.py
--rw-rw-rw-   0 root         (0) root         (0)    11439 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_functional_account.py
--rw-rw-rw-   0 root         (0) root         (0)    11022 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_nx_entity.py
--rw-rw-rw-   0 root         (0) root         (0)    12068 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_nx_entity_nested.py
--rw-rw-rw-   0 root         (0) root         (0)    15320 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_scan.py
--rw-rw-rw-   0 root         (0) root         (0)     8737 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_session.py
--rw-rw-rw-   0 root         (0) root         (0)     7466 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_user.py
--rw-rw-rw-   0 root         (0) root         (0)     7413 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11427 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity.py
--rw-rw-rw-   0 root         (0) root         (0)    28573 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    30426 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)     3848 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)    12385 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_nested.py
--rw-rw-rw-   0 root         (0) root         (0)    11508 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    16983 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    14419 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)    15733 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan.py
--rw-rw-rw-   0 root         (0) root         (0)    37302 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    39155 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)     4001 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)    15810 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    16975 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    19671 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)     9144 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session.py
--rw-rw-rw-   0 root         (0) root         (0)    25641 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    27494 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)     3846 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)     9191 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_partial.py
--rw-rw-rw-   0 root         (0) root         (0)    16981 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)    13149 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)     6799 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.463360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/models/
--rw-rw-rw-   0 root         (0) root         (0)     8484 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.463360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.464360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts/
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10904 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15611 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    12093 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.464360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_count/
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11125 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.464360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_id/
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8273 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12249 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12570 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.464360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs/
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10883 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15593 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    12072 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.464360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_count/
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11114 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.465360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_id/
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8262 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12232 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12552 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.465360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_callback/
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_callback/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6248 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_callback/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.465360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_login/
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_login/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6237 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_login/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.465360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_logout/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_logout/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6086 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_logout/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.466360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10787 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15506 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    11972 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.466360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_count/
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11060 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.466360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_id/
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8208 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12152 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12465 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.466360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets/
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10766 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15488 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    11951 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.466360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_count/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11049 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.467360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_id/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8197 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12135 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12447 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.467360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices/
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10745 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15470 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    11930 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.467360 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_count/
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11038 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.468361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_id/
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8186 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12118 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12429 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.468361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events/
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10724 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15452 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    11909 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.468361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_count/
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11027 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.469361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_id/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8175 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12101 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12411 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_id/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    12372 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.469361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts/
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10988 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15683 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    12177 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.469361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_count/
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11169 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.469361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_id/
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12642 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.470361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10829 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15542 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    12014 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.470361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_count/
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11082 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.470361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_id/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8230 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12186 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12501 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.470361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts/
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10988 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15683 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    12177 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.471361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_count/
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11169 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.471361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_id/
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12642 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.471361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities/
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10809 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15533 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    12000 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.471361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_count/
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11080 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.471361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_entry/
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_entry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12129 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_entry/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.472361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_id/
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8228 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12174 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12492 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_id/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    12453 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.472361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10703 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15434 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    11888 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.472361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_count/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11016 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.473361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_id/
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8164 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12084 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12393 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.473361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions/
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10766 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions/get.py
--rw-rw-rw-   0 root         (0) root         (0)    15488 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions/patch.py
--rw-rw-rw-   0 root         (0) root         (0)    11951 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.473361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_count/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11049 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_count/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.473361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_id/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8197 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_id/delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12135 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    12447 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.474361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11832 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.474361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_login/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_login/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15992 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_login/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.474361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_me/
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_me/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10485 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_me/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.474361 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_user_id/
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_user_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9785 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_user_id/get.py
--rw-rw-rw-   0 root         (0) root         (0)    10641 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)    97634 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.450359 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      293 2024-01-16 13:19:48.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    28077 2024-01-16 13:19:48.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-16 13:19:48.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2024-01-16 13:19:48.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-01-16 13:19:48.000000 py-scibec-openapi-client-1.8.5/py_scibec_openapi_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-01-16 13:19:48.492363 py-scibec-openapi-client-1.8.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1050 2024-01-16 13:19:35.000000 py-scibec-openapi-client-1.8.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.447358 py-scibec-openapi-client-1.8.5/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.482362 py-scibec-openapi-client-1.8.5/test/test_models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_account.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_account_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_account_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_account_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      606 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_account_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_config.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      623 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_beamline.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      606 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_device.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_device_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_device_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_device_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_device_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_device_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_device_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      519 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_event.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_event_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_event_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_event_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_event_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_event_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_event_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      597 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)      597 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account.py
--rw-rw-rw-   0 root         (0) root         (0)      593 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      597 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)      597 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_loopback_count.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_access_account.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_access_config.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_beamline.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_device.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_event.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_experiment.py
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_experiment_account.py
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_functional_account.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_nx_entity.py
--rw-rw-rw-   0 root         (0) root         (0)      570 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_nx_entity_nested.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_scan.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_session.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_user.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_new_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_nested.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_scan.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_scan_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_scan_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_scan_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_scan_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_scan_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_scan_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_session.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_session_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_session_filter1.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_session_include_filter_items.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_session_partial.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_session_scope_filter.py
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_session_with_relations.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.5/test/test_models/test_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.482362 py-scibec-openapi-client-1.8.5/test/test_paths/
--rw-rw-rw-   0 root         (0) root         (0)     1995 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.482362 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.482362 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.482362 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      817 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.483362 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.483362 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.483362 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      814 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.483362 py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_callback/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_callback/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_callback/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.483362 py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_login/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_login/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_login/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.483362 py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_logout/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_logout/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_logout/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.484362 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.484362 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.484362 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      831 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.484362 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.485362 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.485362 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.485362 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      788 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.485362 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.486362 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.486362 py-scibec-openapi-client-1.8.5/test/test_paths/test_events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_events/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_events/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      788 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_events/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.486362 py-scibec-openapi-client-1.8.5/test/test_paths/test_events_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_events_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_events_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.486362 py-scibec-openapi-client-1.8.5/test/test_paths/test_events_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_events_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_events_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_events_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_events_id/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_events_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.487362 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.487362 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      838 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.487362 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.487362 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.487362 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.488362 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.488362 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.488362 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      838 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.488362 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.489362 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.489362 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.489362 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_entry/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_entry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_entry/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.489362 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      831 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_id/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.490363 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      788 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.490363 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.490363 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      789 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.490363 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions/test_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.490363 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_count/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.491363 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_id/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_id/test_get.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.491363 py-scibec-openapi-client-1.8.5/test/test_paths/test_users/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_users/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.491363 py-scibec-openapi-client-1.8.5/test/test_paths/test_users_login/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_users_login/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_users_login/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.491363 py-scibec-openapi-client-1.8.5/test/test_paths/test_users_me/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_users_me/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      789 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_users_me/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:19:48.491363 py-scibec-openapi-client-1.8.5/test/test_paths/test_users_user_id/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:19:34.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_users_user_id/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.5/test/test_paths/test_users_user_id/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.929803 py-scibec-openapi-client-1.8.6/
+-rw-r--r--   0 root         (0) root         (0)      293 2024-01-16 13:23:15.929803 py-scibec-openapi-client-1.8.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    31635 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.887799 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    58504 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.887799 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7789 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.891800 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/access_accounts.py
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/access_accounts_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/access_accounts_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/access_configs.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/access_configs_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/access_configs_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/auth_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/auth_login.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/auth_logout.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/beamlines.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/beamlines_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/beamlines_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/datasets_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/datasets_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/devices.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/devices_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/devices_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/events.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/events_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/events_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/experiment_accounts.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/experiment_accounts_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/experiment_accounts_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/experiments.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/experiments_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/experiments_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/functional_accounts.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/functional_accounts_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/functional_accounts_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/nxentities.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/nxentities_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/nxentities_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/nxentities_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/scans.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/scans_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/scans_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/sessions_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/sessions_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/users_login.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/users_me.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/paths/users_user_id.py
+-rw-rw-rw-   0 root         (0) root         (0)     3301 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.892800 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/access_account_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/access_config_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/beamline_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1190 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/dataset_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/device_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/event_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/experiment_account_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/experiment_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/functional_account_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/nx_entity_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      746 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/oidc_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/scan_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1190 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/session_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/user_controller_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    15715 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4478 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.901800 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10673 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_account.py
+-rw-rw-rw-   0 root         (0) root         (0)    24644 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_account_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    26497 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_account_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)    10726 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_account_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    10784 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_account_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    11368 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    28026 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    29879 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3760 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)    11363 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    16991 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    14045 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)     8523 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)    24578 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    26431 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3711 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     8571 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    16983 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11117 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9022 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    25520 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    27373 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3668 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     9102 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    16981 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11454 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    17398 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device.py
+-rw-rw-rw-   0 root         (0) root         (0)    35363 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    37216 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)    17369 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    16979 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    21971 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9548 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event.py
+-rw-rw-rw-   0 root         (0) root         (0)    26461 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    28314 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3630 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     9626 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    16977 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11072 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13662 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11800 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account.py
+-rw-rw-rw-   0 root         (0) root         (0)    26576 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    28429 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)    11857 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    17001 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    12711 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    32162 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    34015 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4093 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)    13697 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    16987 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    20208 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    11826 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account.py
+-rw-rw-rw-   0 root         (0) root         (0)    26602 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    28455 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3599 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)    11883 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    17001 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    12772 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2396 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/loopback_count.py
+-rw-rw-rw-   0 root         (0) root         (0)    10278 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_access_account.py
+-rw-rw-rw-   0 root         (0) root         (0)    10971 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_access_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8118 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)     8615 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    16989 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     9137 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_event.py
+-rw-rw-rw-   0 root         (0) root         (0)    13261 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11413 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_experiment_account.py
+-rw-rw-rw-   0 root         (0) root         (0)    11439 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_functional_account.py
+-rw-rw-rw-   0 root         (0) root         (0)    11022 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_nx_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)    12068 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_nx_entity_nested.py
+-rw-rw-rw-   0 root         (0) root         (0)    15320 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_scan.py
+-rw-rw-rw-   0 root         (0) root         (0)     8737 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     7466 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     7413 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11427 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)    28573 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    30426 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3848 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)    12385 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_nested.py
+-rw-rw-rw-   0 root         (0) root         (0)    11508 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    16983 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    14419 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    15733 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan.py
+-rw-rw-rw-   0 root         (0) root         (0)    37302 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    39155 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)    15810 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    16975 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    19671 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9144 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session.py
+-rw-rw-rw-   0 root         (0) root         (0)    25641 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    27494 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3846 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     9191 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)    16981 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    13149 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6799 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.901800 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/models/
+-rw-rw-rw-   0 root         (0) root         (0)     8484 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.901800 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.901800 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts/
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10904 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15611 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    12093 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.902801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_count/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11125 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.902801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_id/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8273 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12249 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12570 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.902801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs/
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10883 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15593 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    12072 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.902801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_count/
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11114 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.903801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_id/
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8262 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12232 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12552 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.903801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_callback/
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_callback/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6248 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_callback/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.903801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_login/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_login/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6237 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_login/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.903801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_logout/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_logout/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6086 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_logout/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.903801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10787 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15506 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    11972 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.904801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_count/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11060 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.904801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_id/
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8208 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12152 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12465 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.904801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets/
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10766 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15488 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    11951 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.904801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_count/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11049 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.905801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_id/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8197 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12135 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12447 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.905801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices/
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10745 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15470 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    11930 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.905801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_count/
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11038 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.905801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_id/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8186 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12118 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12429 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.906801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events/
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10724 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15452 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    11909 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.906801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_count/
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11027 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.906801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_id/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8175 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12101 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12411 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_id/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    12372 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.907801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts/
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10988 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15683 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    12177 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.907801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_count/
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11169 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.907801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_id/
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12642 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.907801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10829 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15542 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    12014 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.907801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_count/
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11082 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.908801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_id/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8230 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12186 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12501 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.908801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts/
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10988 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15683 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    12177 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.908801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_count/
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11169 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.909801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_id/
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12642 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.909801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10809 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15533 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    12000 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.909801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_count/
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11080 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.909801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_entry/
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_entry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12129 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_entry/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.910802 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_id/
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8228 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12174 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12492 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_id/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    12453 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.910802 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10703 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15434 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    11888 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.910802 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_count/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11016 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.910802 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_id/
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8164 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12084 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12393 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.911801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions/
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10766 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    15488 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions/patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    11951 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.911801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_count/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11049 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_count/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.911801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_id/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8197 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_id/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12135 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    12447 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.911801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11832 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.911801 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_login/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_login/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15992 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_login/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.912802 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_me/
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_me/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10485 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_me/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.912802 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_user_id/
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_user_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9785 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_user_id/get.py
+-rw-rw-rw-   0 root         (0) root         (0)    10641 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)    97634 2023-12-01 17:28:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.887799 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      293 2024-01-16 13:23:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    28077 2024-01-16 13:23:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-16 13:23:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2024-01-16 13:23:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-01-16 13:23:15.000000 py-scibec-openapi-client-1.8.6/py_scibec_openapi_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-01-16 13:23:15.929803 py-scibec-openapi-client-1.8.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-01-16 13:23:03.000000 py-scibec-openapi-client-1.8.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.884799 py-scibec-openapi-client-1.8.6/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.919802 py-scibec-openapi-client-1.8.6/test/test_models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_account_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_account_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_account_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_account_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      623 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_device.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_device_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_device_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_device_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_device_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_device_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_device_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      519 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_event.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_event_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_event_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_event_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_event_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_event_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_event_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      597 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      597 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      564 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      593 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      597 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      597 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_loopback_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_access_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_access_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_device.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_event.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_experiment_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_functional_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_nx_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)      570 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_nx_entity_nested.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_scan.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_session.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_new_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_nested.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_scan.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_scan_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_scan_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_scan_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_scan_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_scan_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_scan_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_session.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_session_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_session_filter1.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_session_include_filter_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_session_partial.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_session_scope_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_session_with_relations.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-01-16 11:32:13.000000 py-scibec-openapi-client-1.8.6/test/test_models/test_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.919802 py-scibec-openapi-client-1.8.6/test/test_paths/
+-rw-rw-rw-   0 root         (0) root         (0)     1995 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.919802 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.920802 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.920802 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      817 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.920802 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.920802 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.921802 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      814 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.921802 py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_callback/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_callback/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_callback/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.921802 py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_login/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_login/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_login/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.921802 py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_logout/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_logout/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_logout/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.921802 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      794 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.921802 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.922803 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      831 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.922803 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      794 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.922803 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.922803 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.923803 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      788 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      794 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.923803 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.923803 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.923803 py-scibec-openapi-client-1.8.6/test/test_paths/test_events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_events/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_events/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      788 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_events/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.924803 py-scibec-openapi-client-1.8.6/test/test_paths/test_events_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_events_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_events_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.924803 py-scibec-openapi-client-1.8.6/test/test_paths/test_events_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_events_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_events_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_events_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_events_id/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_events_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.924803 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.924803 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      838 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.925803 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.925803 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.925803 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.925803 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.926803 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.926803 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      838 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.926803 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.926803 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.926803 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.926803 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_entry/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_entry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_entry/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.927803 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      831 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_id/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.927803 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      788 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.927803 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.927803 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      789 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.928803 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions/test_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      794 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.928803 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_count/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.928803 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_id/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_id/test_get.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.928803 py-scibec-openapi-client-1.8.6/test/test_paths/test_users/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_users/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.928803 py-scibec-openapi-client-1.8.6/test/test_paths/test_users_login/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_users_login/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_users_login/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.929803 py-scibec-openapi-client-1.8.6/test/test_paths/test_users_me/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_users_me/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      789 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_users_me/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 13:23:15.929803 py-scibec-openapi-client-1.8.6/test/test_paths/test_users_user_id/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 13:23:02.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_users_user_id/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-12-01 16:51:18.000000 py-scibec-openapi-client-1.8.6/test/test_paths/test_users_user_id/test_get.py
```

### Comparing `py-scibec-openapi-client-1.8.5/README.md` & `py-scibec-openapi-client-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/__init__.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/api_client.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/path_to_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tag_to_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/__init__.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/access_account_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/access_account_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/access_config_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/access_config_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/beamline_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/beamline_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/dataset_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/dataset_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/device_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/device_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/event_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/event_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/experiment_account_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/experiment_account_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/experiment_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/experiment_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/functional_account_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/functional_account_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/nx_entity_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/nx_entity_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/oidc_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/oidc_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/scan_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/scan_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/session_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/session_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/apis/tags/user_controller_api.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/apis/tags/user_controller_api.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/configuration.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/exceptions.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_account.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_account_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_account_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_account_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_account_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_account_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_account_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_account_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_account_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_scope_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/access_config_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/access_config_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_scope_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/beamline_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/beamline_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_scope_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/dataset_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/dataset_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_scope_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/device_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/device_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_scope_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/event_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/event_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_scope_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_account_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_account_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_scope_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/experiment_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/experiment_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_scope_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/functional_account_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/functional_account_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/loopback_count.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/loopback_count.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_access_account.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_access_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_access_config.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_access_config.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_beamline.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_beamline.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_dataset.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_dataset.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_device.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_device.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_event.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_event.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_experiment.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_experiment.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_experiment_account.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_experiment_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_functional_account.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_functional_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_nx_entity.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_nx_entity.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_nx_entity_nested.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_nx_entity_nested.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_scan.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_scan.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_session.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_session.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_user.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_user.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/new_user_request.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/new_user_request.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_nested.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_nested.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_scope_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/nx_entity_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/nx_entity_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_scope_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/scan_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/scan_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_filter1.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_partial.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_scope_filter.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/session_with_relations.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/session_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/model/user.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/model/user.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/models/__init__.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/__init__.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_accounts_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_accounts_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/access_configs_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/access_configs_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_callback/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_callback/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_login/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_login/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/auth_logout/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/auth_logout/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/beamlines_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/beamlines_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/datasets_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/datasets_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/devices_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/devices_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/events_id/put.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/events_id/put.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiment_accounts_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiment_accounts_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/experiments_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/experiments_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/functional_accounts_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/functional_accounts_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_entry/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_entry/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/nxentities_id/put.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/nxentities_id/put.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/scans_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/scans_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_count/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_count/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_id/delete.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_id/delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/sessions_id/patch.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/sessions_id/patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_login/post.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_login/post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_me/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_me/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/paths/users_user_id/get.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/paths/users_user_id/get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/rest.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client/schemas.py` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client/schemas.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/py_scibec_openapi_client.egg-info/SOURCES.txt` & `py-scibec-openapi-client-1.8.6/py_scibec_openapi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/setup.py` & `py-scibec-openapi-client-1.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: klaus.wakonig@psi.ch
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "py-scibec-openapi-client"
-VERSION = "1.8.5"
+VERSION = "1.8.6"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_account.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_account_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_account_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_account_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_account_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_account_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_account_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_account_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_account_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_config.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_config.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_scope_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_access_config_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_access_config_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_beamline.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_beamline.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_scope_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_beamline_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_beamline_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_dataset.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_dataset.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_scope_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_dataset_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_dataset_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_device.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_device.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_device_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_device_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_device_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_device_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_device_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_device_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_device_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_device_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_device_scope_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_device_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_device_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_device_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_event.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_event.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_event_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_event_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_event_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_event_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_event_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_event_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_event_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_event_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_event_scope_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_event_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_event_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_event_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_scope_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_account_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_account_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_scope_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_experiment_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_experiment_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_scope_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_functional_account_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_functional_account_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_loopback_count.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_loopback_count.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_access_account.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_access_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_access_config.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_access_config.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_beamline.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_beamline.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_dataset.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_dataset.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_device.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_device.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_event.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_event.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_experiment.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_experiment.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_experiment_account.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_experiment_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_functional_account.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_functional_account.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_nx_entity.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_nx_entity.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_nx_entity_nested.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_nx_entity_nested.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_scan.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_scan.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_session.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_session.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_user.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_user.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_new_user_request.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_new_user_request.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_nested.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_nested.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_scope_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_nx_entity_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_nx_entity_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_scan.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_scan.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_scan_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_scan_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_scan_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_scan_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_scan_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_scan_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_scan_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_scan_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_scan_scope_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_scan_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_scan_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_scan_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_session.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_session.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_session_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_session_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_session_filter1.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_session_filter1.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_session_include_filter_items.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_session_include_filter_items.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_session_partial.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_session_partial.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_session_scope_filter.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_session_scope_filter.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_session_with_relations.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_session_with_relations.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_models/test_user.py` & `py-scibec-openapi-client-1.8.6/test/test_models/test_user.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/__init__.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_accounts_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_accounts_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_access_configs_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_access_configs_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_callback/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_callback/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_login/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_login/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_auth_logout/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_auth_logout/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_beamlines_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_beamlines_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_datasets_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_datasets_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_devices/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_devices/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_devices/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_devices/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_devices/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_devices/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_devices_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_devices_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_events/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_events/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_events/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_events/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_events/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_events/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_events_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_events_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_events_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_events_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_events_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_events_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_events_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_events_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_events_id/test_put.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_events_id/test_put.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiment_accounts_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiment_accounts_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_experiments_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_experiments_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_functional_accounts_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_functional_accounts_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_entry/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_entry/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_nxentities_id/test_put.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_nxentities_id/test_put.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_scans/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_scans/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_scans/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_scans/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_scans/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_scans/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_scans_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_scans_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_count/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_count/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_id/test_delete.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_id/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_sessions_id/test_patch.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_sessions_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_users/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_users/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_users_login/test_post.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_users_login/test_post.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_users_me/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_users_me/test_get.py`

 * *Files identical despite different names*

### Comparing `py-scibec-openapi-client-1.8.5/test/test_paths/test_users_user_id/test_get.py` & `py-scibec-openapi-client-1.8.6/test/test_paths/test_users_user_id/test_get.py`

 * *Files identical despite different names*

