# Comparing `tmp/finbourne_insights_sdk-2.1.4.tar.gz` & `tmp/finbourne_insights_sdk-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_insights_sdk-2.1.4.tar", max compression
+gzip compressed data, was "finbourne_insights_sdk-2.1.5.tar", max compression
```

## Comparing `finbourne_insights_sdk-2.1.4.tar` & `finbourne_insights_sdk-2.1.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    10554 2024-04-24 17:52:42.797784 finbourne_insights_sdk-2.1.4/README.md
--rw-r--r--   0        0        0     5228 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/__init__.py
--rw-r--r--   0        0        0      526 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/api/__init__.py
--rw-r--r--   0        0        0    24459 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/api/access_evaluations_api.py
--rw-r--r--   0        0        0     7520 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/api/application_metadata_api.py
--rw-r--r--   0        0        0    24169 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/api/auditing_api.py
--rw-r--r--   0        0        0    35828 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/api/requests_api.py
--rw-r--r--   0        0        0    36148 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/api/vendor_logs_api.py
--rw-r--r--   0        0        0    30813 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/api_client.py
--rw-r--r--   0        0        0      852 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/api_response.py
--rw-r--r--   0        0        0    14459 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/configuration.py
--rw-r--r--   0        0        0     5339 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/exceptions.py
--rw-r--r--   0        0        0      599 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/__init__.py
--rw-r--r--   0        0        0    30684 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/api_client.py
--rw-r--r--   0        0        0     9902 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8117 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/api_configuration.py
--rw-r--r--   0        0        0     6812 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12711 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/rest.py
--rw-r--r--   0        0        0    11577 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3890 2024-04-24 17:52:42.795784 finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     3641 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/__init__.py
--rw-r--r--   0        0        0     3915 2024-04-24 17:52:42.790784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/access_controlled_action.py
--rw-r--r--   0        0        0     4858 2024-04-24 17:52:42.791784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/access_controlled_resource.py
--rw-r--r--   0        0        0    11915 2024-04-24 17:52:42.791784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/access_evaluation_log.py
--rw-r--r--   0        0        0     2070 2024-04-24 17:52:42.791784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/action_id.py
--rw-r--r--   0        0        0     3756 2024-04-24 17:52:42.791784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_data.py
--rw-r--r--   0        0        0     2219 2024-04-24 17:52:42.791784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_data_summary.py
--rw-r--r--   0        0        0     3451 2024-04-24 17:52:42.791784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_entry.py
--rw-r--r--   0        0        0     2096 2024-04-24 17:52:42.791784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_entry_note.py
--rw-r--r--   0        0        0     2779 2024-04-24 17:52:42.791784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_process.py
--rw-r--r--   0        0        0     3039 2024-04-24 17:52:42.791784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_process_summary.py
--rw-r--r--   0        0        0     2119 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/bucket.py
--rw-r--r--   0        0        0     2519 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/create_audit_entry.py
--rw-r--r--   0        0        0     2597 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/histogram.py
--rw-r--r--   0        0        0     3184 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/id_selector_definition.py
--rw-r--r--   0        0        0     3109 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2262 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/link.py
--rw-r--r--   0        0        0     3857 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4693 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3212 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/problem_details.py
--rw-r--r--   0        0        0     5510 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/request.py
--rw-r--r--   0        0        0     8268 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/request_log.py
--rw-r--r--   0        0        0     2374 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource.py
--rw-r--r--   0        0        0     4263 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4203 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource_list_of_audit_process_summary.py
--rw-r--r--   0        0        0     4738 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py
--rw-r--r--   0        0        0     4638 2024-04-24 17:52:42.792784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource_list_with_histogram_of_request_log.py
--rw-r--r--   0        0        0     4627 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py
--rw-r--r--   0        0        0     5048 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/response.py
--rw-r--r--   0        0        0     2913 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/scrollable_collection_of_audit_entry.py
--rw-r--r--   0        0        0     4520 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/vendor_log.py
--rw-r--r--   0        0        0     2797 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/vendor_request.py
--rw-r--r--   0        0        0     2823 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/models/vendor_response.py
--rw-r--r--   0        0        0        0 2024-04-24 17:52:42.793784 finbourne_insights_sdk-2.1.4/finbourne_insights/py.typed
--rw-r--r--   0        0        0    10164 2024-04-24 17:52:42.794784 finbourne_insights_sdk-2.1.4/finbourne_insights/rest.py
--rw-r--r--   0        0        0      871 2024-04-24 17:52:42.797784 finbourne_insights_sdk-2.1.4/pyproject.toml
--rw-r--r--   0        0        0    11607 1970-01-01 00:00:00.000000 finbourne_insights_sdk-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10554 2024-05-02 08:40:08.834751 finbourne_insights_sdk-2.1.5/README.md
+-rw-r--r--   0        0        0     5228 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/__init__.py
+-rw-r--r--   0        0        0      526 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/api/__init__.py
+-rw-r--r--   0        0        0    24459 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/api/access_evaluations_api.py
+-rw-r--r--   0        0        0     7520 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/api/application_metadata_api.py
+-rw-r--r--   0        0        0    24169 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/api/auditing_api.py
+-rw-r--r--   0        0        0    35828 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/api/requests_api.py
+-rw-r--r--   0        0        0    36148 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/api/vendor_logs_api.py
+-rw-r--r--   0        0        0    30813 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/api_response.py
+-rw-r--r--   0        0        0    14459 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/configuration.py
+-rw-r--r--   0        0        0     5339 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/exceptions.py
+-rw-r--r--   0        0        0      599 2024-05-02 08:40:08.832751 finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/__init__.py
+-rw-r--r--   0        0        0    30684 2024-05-02 08:40:08.832751 finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/api_client.py
+-rw-r--r--   0        0        0     9902 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8117 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6812 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-05-02 08:40:08.832751 finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-05-02 08:40:08.832751 finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12711 2024-05-02 08:40:08.832751 finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/rest.py
+-rw-r--r--   0        0        0    11577 2024-05-02 08:40:08.832751 finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-05-02 08:40:08.832751 finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3890 2024-05-02 08:40:08.832751 finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     3641 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/__init__.py
+-rw-r--r--   0        0        0     3915 2024-05-02 08:40:08.828751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4858 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/access_controlled_resource.py
+-rw-r--r--   0        0        0    11915 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/access_evaluation_log.py
+-rw-r--r--   0        0        0     2070 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/action_id.py
+-rw-r--r--   0        0        0     3756 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_data.py
+-rw-r--r--   0        0        0     2219 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_data_summary.py
+-rw-r--r--   0        0        0     3451 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_entry.py
+-rw-r--r--   0        0        0     2096 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_entry_note.py
+-rw-r--r--   0        0        0     2779 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_process.py
+-rw-r--r--   0        0        0     3039 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_process_summary.py
+-rw-r--r--   0        0        0     2119 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/bucket.py
+-rw-r--r--   0        0        0     2519 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/create_audit_entry.py
+-rw-r--r--   0        0        0     2597 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/histogram.py
+-rw-r--r--   0        0        0     3184 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3109 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2262 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/link.py
+-rw-r--r--   0        0        0     3857 2024-05-02 08:40:08.829751 finbourne_insights_sdk-2.1.5/finbourne_insights/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4693 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3212 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/problem_details.py
+-rw-r--r--   0        0        0     5510 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/request.py
+-rw-r--r--   0        0        0     8268 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/request_log.py
+-rw-r--r--   0        0        0     2374 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource.py
+-rw-r--r--   0        0        0     4263 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4203 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource_list_of_audit_process_summary.py
+-rw-r--r--   0        0        0     4738 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py
+-rw-r--r--   0        0        0     4638 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource_list_with_histogram_of_request_log.py
+-rw-r--r--   0        0        0     4627 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py
+-rw-r--r--   0        0        0     5048 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/response.py
+-rw-r--r--   0        0        0     2913 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/scrollable_collection_of_audit_entry.py
+-rw-r--r--   0        0        0     4520 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/vendor_log.py
+-rw-r--r--   0        0        0     2797 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/vendor_request.py
+-rw-r--r--   0        0        0     2823 2024-05-02 08:40:08.830752 finbourne_insights_sdk-2.1.5/finbourne_insights/models/vendor_response.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/py.typed
+-rw-r--r--   0        0        0    10164 2024-05-02 08:40:08.831751 finbourne_insights_sdk-2.1.5/finbourne_insights/rest.py
+-rw-r--r--   0        0        0      871 2024-05-02 08:40:08.834751 finbourne_insights_sdk-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0    11607 1970-01-01 00:00:00.000000 finbourne_insights_sdk-2.1.5/PKG-INFO
```

### Comparing `finbourne_insights_sdk-2.1.4/README.md` & `finbourne_insights_sdk-2.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-insights-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.772
-- Package version: 2.1.4
+- API version: 0.0.774
+- Package version: 2.1.5
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/__init__.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/api/__init__.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/api/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/api/access_evaluations_api.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/api/access_evaluations_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/api/application_metadata_api.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/api/auditing_api.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/api/auditing_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/api/requests_api.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/api/requests_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/api/vendor_logs_api.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/api/vendor_logs_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/api_client.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/api_response.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/configuration.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_insights-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.772\n"\
+               "Version of the API: 0.0.774\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/exceptions.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/__init__.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/api_client.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/api_client_factory.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/api_configuration.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/configuration_loaders.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/proxy_config.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/refreshing_token.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/rest.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/retry.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/socket_keep_alive.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/extensions/tcp_keep_alive_connector.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/__init__.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/access_controlled_action.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/access_controlled_resource.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/access_evaluation_log.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/access_evaluation_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/action_id.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/action_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_data.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_data.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_data_summary.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_data_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_entry.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_entry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_entry_note.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_entry_note.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_process.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_process.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/audit_process_summary.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/audit_process_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/bucket.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/bucket.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/create_audit_entry.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/create_audit_entry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/histogram.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/histogram.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/id_selector_definition.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/identifier_part_schema.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/link.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/link.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/lusid_problem_details.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/lusid_validation_problem_details.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/problem_details.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/request.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/request.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/request_log.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/request_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource_list_of_access_controlled_resource.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource_list_of_audit_process_summary.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource_list_of_audit_process_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource_list_with_histogram_of_request_log.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource_list_with_histogram_of_request_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/response.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/response.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/scrollable_collection_of_audit_entry.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/scrollable_collection_of_audit_entry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/vendor_log.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/vendor_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/vendor_request.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/vendor_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/models/vendor_response.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/models/vendor_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/finbourne_insights/rest.py` & `finbourne_insights_sdk-2.1.5/finbourne_insights/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.1.4/pyproject.toml` & `finbourne_insights_sdk-2.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-insights-sdk"
-version = "2.1.4"
+version = "2.1.5"
 description = "FINBOURNE Insights API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/insights-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Insights API", "finbourne-insights-sdk"]
 packages = [
```

### Comparing `finbourne_insights_sdk-2.1.4/PKG-INFO` & `finbourne_insights_sdk-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-insights-sdk
-Version: 2.1.4
+Version: 2.1.5
 Summary: FINBOURNE Insights API
 Home-page: https://github.com/finbourne/insights-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Insights API,finbourne-insights-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # finbourne-insights-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.772
-- Package version: 2.1.4
+- API version: 0.0.774
+- Package version: 2.1.5
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

