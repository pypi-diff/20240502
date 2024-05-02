# Comparing `tmp/galaxy-test-base-24.0.0.tar.gz` & `tmp/galaxy_test_base-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-test-base-24.0.0.tar", last modified: Wed Apr  3 02:45:41 2024, max compression
+gzip compressed data, was "galaxy_test_base-24.0.1.tar", last modified: Thu May  2 13:48:46 2024, max compression
```

## Comparing `galaxy-test-base-24.0.0.tar` & `galaxy_test_base-24.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:41.007406 galaxy-test-base-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-03 02:45:41.007406 galaxy-test-base-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:40.999406 galaxy-test-base-24.0.0/galaxy_test/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:41.003406 galaxy-test-base-24.0.0/galaxy_test/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/api_asserts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/api_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:41.007406 galaxy-test-base-24.0.0/galaxy_test/base/data/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/minimal_tool_no_id.json
--rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_subworkflow_with_integer_input.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_1.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_2.ga
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_batch.ga
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_map_reduce_pause.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_matching_lists.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_missing_tool.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_pause.ga
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga
--rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_topoambigouity.ga
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_two_random_lines.ga
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_validation_1.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_with_input_tags.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_with_runtime_input.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/interactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/json_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   135178 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/populators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/rules_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/uses_shed_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/base/workflow_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/galaxy_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:41.007406 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-03 02:45:40.000000 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-03 02:45:40.000000 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:40.000000 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 02:45:40.000000 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 02:45:40.000000 galaxy-test-base-24.0.0/galaxy_test_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-03 02:45:41.007406 galaxy-test-base-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-test-base-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:46.057886 galaxy_test_base-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-02 13:48:46.057886 galaxy_test_base-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:46.049886 galaxy_test_base-24.0.1/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:46.053886 galaxy_test_base-24.0.1/galaxy_test/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/api_asserts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/api_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:46.057886 galaxy_test_base-24.0.1/galaxy_test/base/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/minimal_tool_no_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_subworkflow_with_integer_input.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_1.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_2.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_batch.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_map_reduce_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_matching_lists.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_missing_tool.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga
+-rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_topoambigouity.ga
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_two_random_lines.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_validation_1.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_with_input_tags.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_with_runtime_input.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/json_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135637 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/populators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/rules_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/uses_shed_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/workflow_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:46.057886 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-02 13:48:46.000000 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-02 13:48:46.000000 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:48:46.000000 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 13:48:46.000000 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 13:48:46.000000 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-02 13:48:46.057886 galaxy_test_base-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/test-requirements.txt
```

### Comparing `galaxy-test-base-24.0.0/HISTORY.rst` & `galaxy_test_base-24.0.1/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Make `wait_for_history_jobs` look at jobs, not datasets by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17892 <https://github.com/galaxyproject/galaxy/pull/17892>`_
+* Fix missing implicit conversion for mapped over jobs by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17952 <https://github.com/galaxyproject/galaxy/pull/17952>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-test-base-24.0.0/LICENSE` & `galaxy_test_base-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/PKG-INFO` & `galaxy_test_base-24.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-base
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy testing utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,14 +51,26 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Make `wait_for_history_jobs` look at jobs, not datasets by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17892 <https://github.com/galaxyproject/galaxy/pull/17892>`_
+* Fix missing implicit conversion for mapped over jobs by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17952 <https://github.com/galaxyproject/galaxy/pull/17952>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/api.py` & `galaxy_test_base-24.0.1/galaxy_test/base/api.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/api_asserts.py` & `galaxy_test_base-24.0.1/galaxy_test/base/api_asserts.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/api_util.py` & `galaxy_test_base-24.0.1/galaxy_test/base/api_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_subworkflow_with_integer_input.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_subworkflow_with_integer_input.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_1.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_1.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_2.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_2.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_batch.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_batch.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_map_reduce_pause.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_map_reduce_pause.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_matching_lists.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_matching_lists.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_missing_tool.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_missing_tool.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_pause.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_pause.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_topoambigouity.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_topoambigouity.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_two_random_lines.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_two_random_lines.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_validation_1.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_validation_1.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_with_input_tags.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_with_input_tags.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/data/test_workflow_with_runtime_input.ga` & `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_with_runtime_input.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/decorators.py` & `galaxy_test_base-24.0.1/galaxy_test/base/decorators.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/env.py` & `galaxy_test_base-24.0.1/galaxy_test/base/env.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/interactor.py` & `galaxy_test_base-24.0.1/galaxy_test/base/interactor.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/json_schema_utils.py` & `galaxy_test_base-24.0.1/galaxy_test/base/json_schema_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/populators.py` & `galaxy_test_base-24.0.1/galaxy_test/base/populators.py`

 * *Files 0% similar despite different names*

```diff
@@ -626,15 +626,16 @@
             wait_on(has_active_jobs, "active jobs", timeout=timeout)
         except TimeoutAssertionError as e:
             jobs = self.history_jobs(history_id)
             message = f"Failed waiting on active jobs to complete, current jobs are [{jobs}]. {e}"
             raise TimeoutAssertionError(message)
 
         if assert_ok:
-            self.wait_for_history(history_id, assert_ok=True, timeout=timeout)
+            for job in self.history_jobs(history_id=history_id):
+                assert job["state"] in ("ok", "skipped"), f"Job {job} not in expected state"
 
     def wait_for_jobs(
         self,
         jobs: Union[List[dict], List[str]],
         assert_ok: bool = False,
         timeout: timeout_type = DEFAULT_TIMEOUT,
         ok_states=None,
@@ -2867,14 +2868,16 @@
                 "name": name,
             }
         ]
         payload = dict(
             history_id=history_id,
             targets=targets,
         )
+        if "__files" in kwds:
+            payload["__files"] = kwds.pop("__files")
         return payload
 
     def wait_for_fetched_collection(self, fetch_response: Union[Dict[str, Any], Response]):
         fetch_response_dict: Dict[str, Any]
         if isinstance(fetch_response, Response):
             fetch_response_dict = fetch_response.json()
         else:
@@ -3002,30 +3005,34 @@
     has_uploads = False
 
     for key, value in test_data.items():
         is_dict = isinstance(value, dict)
         if is_dict and ("elements" in value or value.get("collection_type")):
             elements_data = value.get("elements", [])
             elements = []
-            for element_data in elements_data:
+            new_collection_kwds: Dict[str, Any] = {}
+            for i, element_data in enumerate(elements_data):
                 # Adapt differences between test_data dict and fetch API description.
                 if "name" not in element_data:
                     identifier = element_data.pop("identifier")
                     element_data["name"] = identifier
                 input_type = element_data.pop("type", "raw")
                 content = None
                 if input_type == "File":
-                    content = read_test_data(element_data)
+                    content = open_test_data(element_data)
+                    element_data["src"] = "files"
+                    if "__files" not in new_collection_kwds:
+                        new_collection_kwds["__files"] = {}
+                    new_collection_kwds["__files"][f"file_{i}|file_data"] = content
                 else:
                     content = element_data.pop("content")
-                if content is not None:
-                    element_data["src"] = "pasted"
-                    element_data["paste_content"] = content
+                    if content is not None:
+                        element_data["src"] = "pasted"
+                        element_data["paste_content"] = content
                 elements.append(element_data)
-            new_collection_kwds = {}
             if "name" in value:
                 new_collection_kwds["name"] = value["name"]
             collection_type = value.get("collection_type", "")
             if collection_type == "list:paired":
                 fetch_response = dataset_collection_populator.create_list_of_pairs_in_history(
                     history_id, contents=elements, wait=True, **new_collection_kwds
                 ).json()
```

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/rules_test_data.py` & `galaxy_test_base-24.0.1/galaxy_test/base/rules_test_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/testcase.py` & `galaxy_test_base-24.0.1/galaxy_test/base/testcase.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/uses_shed_api.py` & `galaxy_test_base-24.0.1/galaxy_test/base/uses_shed_api.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test/base/workflow_fixtures.py` & `galaxy_test_base-24.0.1/galaxy_test/base/workflow_fixtures.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/galaxy_test_base.egg-info/PKG-INFO` & `galaxy_test_base-24.0.1/galaxy_test_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-base
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy testing utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,14 +51,26 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Make `wait_for_history_jobs` look at jobs, not datasets by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17892 <https://github.com/galaxyproject/galaxy/pull/17892>`_
+* Fix missing implicit conversion for mapped over jobs by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17952 <https://github.com/galaxyproject/galaxy/pull/17952>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-test-base-24.0.0/galaxy_test_base.egg-info/SOURCES.txt` & `galaxy_test_base-24.0.1/galaxy_test_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-24.0.0/setup.cfg` & `galaxy_test_base-24.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-test-base
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-tool-util
 	galaxy-util
 	bioblend
```

