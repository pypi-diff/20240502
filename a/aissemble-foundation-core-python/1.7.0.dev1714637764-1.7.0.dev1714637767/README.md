# Comparing `tmp/aissemble_foundation_core_python-1.7.0.dev1714637764.tar.gz` & `tmp/aissemble_foundation_core_python-1.7.0.dev1714637767.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_core_python-1.7.0.dev1714637764.tar", max compression
+gzip compressed data, was "aissemble_foundation_core_python-1.7.0.dev1714637767.tar", max compression
```

## Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764.tar` & `aissemble_foundation_core_python-1.7.0.dev1714637767.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     9580 2024-05-02 08:15:38.878489 aissemble_foundation_core_python-1.7.0.dev1714637764/LICENSE
--rw-r--r--   0        0        0      129 2024-05-02 08:12:10.113802 aissemble_foundation_core_python-1.7.0.dev1714637764/README.md
--rw-r--r--   0        0        0     1171 2024-05-02 08:16:05.184450 aissemble_foundation_core_python-1.7.0.dev1714637764/pyproject.toml
--rw-r--r--   0        0        0      196 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_bom/__init__.py
--rw-r--r--   0        0        0     1129 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_bom/training_bom.py
--rw-r--r--   0        0        0      466 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_config/__init__.py
--rw-r--r--   0        0        0      804 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_config/messaging_config.py
--rw-r--r--   0        0        0     1740 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_config/rdbms_connection_pool.py
--rw-r--r--   0        0        0     6470 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_config/spark_elasticsearch_config.py
--rw-r--r--   0        0        0     6907 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_config/spark_neo4j_config.py
--rw-r--r--   0        0        0     1545 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_config/spark_postgres_config.py
--rw-r--r--   0        0        0      196 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_filestore/__init__.py
--rw-r--r--   0        0        0     3181 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_filestore/file_store_factory.py
--rw-r--r--   0        0        0      196 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_metadata/__init__.py
--rw-r--r--   0        0        0     1252 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_metadata/hive_metadata_api_service.py
--rw-r--r--   0        0        0     1599 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_metadata/logging_metadata_api_service.py
--rw-r--r--   0        0        0      728 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_metadata/metadata_api.py
--rw-r--r--   0        0        0      974 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_metadata/metadata_model.py
--rw-r--r--   0        0        0      196 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiopsauth/__init__.py
--rw-r--r--   0        0        0     2185 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiopsauth/auth_config.py
--rw-r--r--   0        0        0     4546 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiopsauth/json_web_token_util.py
--rw-r--r--   0        0        0      196 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/__init__.py
--rw-r--r--   0        0        0     1309 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_client.py
--rw-r--r--   0        0        0     1329 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_config.py
--rw-r--r--   0        0        0     1634 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_request.py
--rw-r--r--   0        0        0      892 2024-05-02 08:12:10.114802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_request_batch.py
--rw-r--r--   0        0        0      842 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_result.py
--rw-r--r--   0        0        0      890 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_result_batch.py
--rw-r--r--   0        0        0     2853 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/rest_inference_client.py
--rw-r--r--   0        0        0      326 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/__init__.py
--rw-r--r--   0        0        0     8799 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/abstract_policy_manager.py
--rw-r--r--   0        0        0      264 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/configuration/__init__.py
--rw-r--r--   0        0        0      756 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/configuration/policy_configuration.py
--rw-r--r--   0        0        0      901 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/default_policy_manager.py
--rw-r--r--   0        0        0      293 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/policy/__init__.py
--rw-r--r--   0        0        0      265 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/policy/json/__init__.py
--rw-r--r--   0        0        0     1611 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/policy/json/policy_input.py
--rw-r--r--   0        0        0     1962 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/policy/policy.py
--rw-r--r--   0        0        0      271 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/policy/result/__init__.py
--rw-r--r--   0        0        0      479 2024-05-02 08:12:10.115802 aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/policy/result/policy_invocation_result.py
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 aissemble_foundation_core_python-1.7.0.dev1714637764/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-02 08:15:38.583091 aissemble_foundation_core_python-1.7.0.dev1714637767/LICENSE
+-rw-r--r--   0        0        0      129 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/README.md
+-rw-r--r--   0        0        0     1171 2024-05-02 08:16:07.492283 aissemble_foundation_core_python-1.7.0.dev1714637767/pyproject.toml
+-rw-r--r--   0        0        0      196 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_bom/__init__.py
+-rw-r--r--   0        0        0     1129 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_bom/training_bom.py
+-rw-r--r--   0        0        0      466 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_config/__init__.py
+-rw-r--r--   0        0        0      804 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_config/messaging_config.py
+-rw-r--r--   0        0        0     1740 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_config/rdbms_connection_pool.py
+-rw-r--r--   0        0        0     6470 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_config/spark_elasticsearch_config.py
+-rw-r--r--   0        0        0     6907 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_config/spark_neo4j_config.py
+-rw-r--r--   0        0        0     1545 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_config/spark_postgres_config.py
+-rw-r--r--   0        0        0      196 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_filestore/__init__.py
+-rw-r--r--   0        0        0     3181 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_filestore/file_store_factory.py
+-rw-r--r--   0        0        0      196 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_metadata/__init__.py
+-rw-r--r--   0        0        0     1252 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_metadata/hive_metadata_api_service.py
+-rw-r--r--   0        0        0     1599 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_metadata/logging_metadata_api_service.py
+-rw-r--r--   0        0        0      728 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_metadata/metadata_api.py
+-rw-r--r--   0        0        0      974 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_metadata/metadata_model.py
+-rw-r--r--   0        0        0      196 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiopsauth/__init__.py
+-rw-r--r--   0        0        0     2185 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiopsauth/auth_config.py
+-rw-r--r--   0        0        0     4546 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiopsauth/json_web_token_util.py
+-rw-r--r--   0        0        0      196 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/__init__.py
+-rw-r--r--   0        0        0     1309 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_client.py
+-rw-r--r--   0        0        0     1329 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_config.py
+-rw-r--r--   0        0        0     1634 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_request.py
+-rw-r--r--   0        0        0      892 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_request_batch.py
+-rw-r--r--   0        0        0      842 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_result.py
+-rw-r--r--   0        0        0      890 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_result_batch.py
+-rw-r--r--   0        0        0     2853 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/rest_inference_client.py
+-rw-r--r--   0        0        0      326 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/__init__.py
+-rw-r--r--   0        0        0     8799 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/abstract_policy_manager.py
+-rw-r--r--   0        0        0      264 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/configuration/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/configuration/policy_configuration.py
+-rw-r--r--   0        0        0      901 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/default_policy_manager.py
+-rw-r--r--   0        0        0      293 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/policy/__init__.py
+-rw-r--r--   0        0        0      265 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/policy/json/__init__.py
+-rw-r--r--   0        0        0     1611 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/policy/json/policy_input.py
+-rw-r--r--   0        0        0     1962 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/policy/policy.py
+-rw-r--r--   0        0        0      271 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/policy/result/__init__.py
+-rw-r--r--   0        0        0      479 2024-05-02 08:12:10.918922 aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/policy/result/policy_invocation_result.py
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 aissemble_foundation_core_python-1.7.0.dev1714637767/PKG-INFO
```

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/LICENSE` & `aissemble_foundation_core_python-1.7.0.dev1714637767/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/pyproject.toml` & `aissemble_foundation_core_python-1.7.0.dev1714637767/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-core-python"
-version = "1.7.0.dev1714637764"
+version = "1.7.0.dev1714637767"
 description = "Core classes for supporting concepts (alerting, metadata, etc) that are needed across most Python-based components"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "aiops_core_bom", from = "src"},
     {include = "aiops_core_config", from = "src"},
     {include = "aiops_core_filestore", from = "src"},
```

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_bom/training_bom.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_bom/training_bom.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_config/messaging_config.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_config/messaging_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_config/rdbms_connection_pool.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_config/rdbms_connection_pool.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_config/spark_elasticsearch_config.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_config/spark_elasticsearch_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_config/spark_neo4j_config.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_config/spark_neo4j_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_config/spark_postgres_config.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_config/spark_postgres_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_filestore/file_store_factory.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_filestore/file_store_factory.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_metadata/hive_metadata_api_service.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_metadata/hive_metadata_api_service.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_metadata/logging_metadata_api_service.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_metadata/logging_metadata_api_service.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_metadata/metadata_api.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_metadata/metadata_api.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiops_core_metadata/metadata_model.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiops_core_metadata/metadata_model.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiopsauth/auth_config.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiopsauth/auth_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/aiopsauth/json_web_token_util.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/aiopsauth/json_web_token_util.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_client.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_client.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_config.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_request.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_request.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_request_batch.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_request_batch.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_result.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_result.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/inference_result_batch.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/inference_result_batch.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/inference/rest_inference_client.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/inference/rest_inference_client.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/abstract_policy_manager.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/abstract_policy_manager.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/configuration/policy_configuration.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/configuration/policy_configuration.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/default_policy_manager.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/default_policy_manager.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/policy/json/policy_input.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/policy/json/policy_input.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/src/policy_manager/policy/policy.py` & `aissemble_foundation_core_python-1.7.0.dev1714637767/src/policy_manager/policy/policy.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_core_python-1.7.0.dev1714637764/PKG-INFO` & `aissemble_foundation_core_python-1.7.0.dev1714637767/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-core-python
-Version: 1.7.0.dev1714637764
+Version: 1.7.0.dev1714637767
 Summary: Core classes for supporting concepts (alerting, metadata, etc) that are needed across most Python-based components
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.8.0)
```

