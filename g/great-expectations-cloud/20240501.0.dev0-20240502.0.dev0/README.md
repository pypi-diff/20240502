# Comparing `tmp/great_expectations_cloud-20240501.0.dev0.tar.gz` & `tmp/great_expectations_cloud-20240502.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-20240501.0.dev0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240502.0.dev0.tar", max compression
```

## Comparing `great_expectations_cloud-20240501.0.dev0.tar` & `great_expectations_cloud-20240502.0.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2084 2024-05-01 18:47:23.631606 great_expectations_cloud-20240501.0.dev0/LICENSE
--rw-r--r--   0        0        0     9532 2024-05-01 18:47:23.631606 great_expectations_cloud-20240501.0.dev0/README.md
--rw-r--r--   0        0        0      150 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      244 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      733 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      763 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      316 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1503 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4279 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     4171 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2881 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     2041 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     2993 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
--rw-r--r--   0        0        0      739 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/unknown.py
--rw-r--r--   0        0        0    17221 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0      362 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/agent_warnings.py
--rw-r--r--   0        0        0     2851 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      858 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0      246 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/constants.py
--rw-r--r--   0        0        0     4663 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0     1360 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9260 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5836 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     3562 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      639 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0     1762 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/logging/README.md
--rw-r--r--   0        0        0     5918 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/logging/logging_cfg.py
--rw-r--r--   0        0        0     9533 2024-05-01 18:47:23.663606 great_expectations_cloud-20240501.0.dev0/pyproject.toml
--rw-r--r--   0        0        0    10886 1970-01-01 00:00:00.000000 great_expectations_cloud-20240501.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-05-02 18:02:54.374021 great_expectations_cloud-20240502.0.dev0/LICENSE
+-rw-r--r--   0        0        0     9760 2024-05-02 18:02:54.374021 great_expectations_cloud-20240502.0.dev0/README.md
+-rw-r--r--   0        0        0      150 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     2993 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      739 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    17221 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0      362 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/agent_warnings.py
+-rw-r--r--   0        0        0     2851 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4663 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0     1762 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     5918 2024-05-02 18:02:54.402021 great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0     9533 2024-05-02 18:02:54.406021 great_expectations_cloud-20240502.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    11114 1970-01-01 00:00:00.000000 great_expectations_cloud-20240502.0.dev0/PKG-INFO
```

### Comparing `great_expectations_cloud-20240501.0.dev0/LICENSE` & `great_expectations_cloud-20240502.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/README.md` & `great_expectations_cloud-20240502.0.dev0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -217,12 +217,15 @@
 
 ### Dependabot and Releases/Pre-releases
 GitHub's Dependabot regularly checks our dependencies for vulnerabilty-based updates and proposes PRs to update dependency version numbers accordingly.
 
 Dependabot may only update the `poetry.lock` file. If only changes to `poetry.lock` are made, this may be done in a pre-release.
 
 For changes to the `pyproject.toml` file:
-- If the version of a tool in the `[tool.poetry.group.dev.dependencies]` group is updated, this may be done in a pre-release.
+- If the version of a tool in the `[tool.poetry.group.dev.dependencies]` group is updated, this may be done without any version bump.
    -  While doing this, make sure any version references in the pre-commit config `.pre-commit-config.yaml` are kept in sync (e.g., ruff).
-- For other dependency updates, a new release should be orchestrated. This includes updates in the following sections:
+- For other dependency updates or package build metadata changes, a new release should be orchestrated. This includes updates in the following sections:
   - `[tool.poetry.dependencies]`
   - `[tool.poetry.group.*.dependencies]` where `*` is the name of the group (not including the `dev` group)
+- To stop the auto-version bump add the `no version bump` label to the PR. Use this when:
+  - Only modifying dev dependencies.
+  - Only modifying tests that do not change functionality.
```

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/actions/unknown.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/actions/unknown.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/agent.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/cli.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/config.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/config.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/event_handler.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/exceptions.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/agent/run.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/agent/run.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/logging/README.md` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/logging/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/great_expectations_cloud/logging/logging_cfg.py` & `great_expectations_cloud-20240502.0.dev0/great_expectations_cloud/logging/logging_cfg.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240501.0.dev0/pyproject.toml` & `great_expectations_cloud-20240502.0.dev0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "20240501.0.dev0"
+version = "20240502.0.dev0"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
```

### Comparing `great_expectations_cloud-20240501.0.dev0/PKG-INFO` & `great_expectations_cloud-20240502.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great_expectations_cloud
-Version: 20240501.0.dev0
+Version: 20240502.0.dev0
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -250,13 +250,16 @@
 
 ### Dependabot and Releases/Pre-releases
 GitHub's Dependabot regularly checks our dependencies for vulnerabilty-based updates and proposes PRs to update dependency version numbers accordingly.
 
 Dependabot may only update the `poetry.lock` file. If only changes to `poetry.lock` are made, this may be done in a pre-release.
 
 For changes to the `pyproject.toml` file:
-- If the version of a tool in the `[tool.poetry.group.dev.dependencies]` group is updated, this may be done in a pre-release.
+- If the version of a tool in the `[tool.poetry.group.dev.dependencies]` group is updated, this may be done without any version bump.
    -  While doing this, make sure any version references in the pre-commit config `.pre-commit-config.yaml` are kept in sync (e.g., ruff).
-- For other dependency updates, a new release should be orchestrated. This includes updates in the following sections:
+- For other dependency updates or package build metadata changes, a new release should be orchestrated. This includes updates in the following sections:
   - `[tool.poetry.dependencies]`
   - `[tool.poetry.group.*.dependencies]` where `*` is the name of the group (not including the `dev` group)
+- To stop the auto-version bump add the `no version bump` label to the PR. Use this when:
+  - Only modifying dev dependencies.
+  - Only modifying tests that do not change functionality.
```

