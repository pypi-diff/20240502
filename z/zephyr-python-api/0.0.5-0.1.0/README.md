# Comparing `tmp/zephyr_python_api-0.0.5.tar.gz` & `tmp/zephyr_python_api-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephyr_python_api-0.0.5.tar", last modified: Wed Apr 17 11:29:36 2024, max compression
+gzip compressed data, was "zephyr_python_api-0.1.0.tar", last modified: Thu May  2 16:36:59 2024, max compression
```

## Comparing `zephyr_python_api-0.0.5.tar` & `zephyr_python_api-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.475239 zephyr_python_api-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-17 11:29:36.475239 zephyr_python_api-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-17 11:29:36.475239 zephyr_python_api-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.467239 zephyr_python_api-0.0.5/zephyr/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.471239 zephyr_python_api-0.0.5/zephyr/scale/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.471239 zephyr_python_api-0.0.5/zephyr/scale/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/cloud_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.471239 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/automations.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/folders.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/priorities.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_cycles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_executions.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.471239 zephyr_python_api-0.0.5/zephyr/scale/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.471239 zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15427 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/server_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/server_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/zephyr_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.475239 zephyr_python_api-0.0.5/zephyr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.475239 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-17 11:29:36.000000 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-17 11:29:36.000000 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:29:36.000000 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 11:29:36.000000 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 11:29:36.000000 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:59.878807 zephyr_python_api-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-02 16:36:59.878807 zephyr_python_api-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-02 16:36:59.878807 zephyr_python_api-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:59.874807 zephyr_python_api-0.1.0/zephyr/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:59.874807 zephyr_python_api-0.1.0/zephyr/scale/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:59.878807 zephyr_python_api-0.1.0/zephyr/scale/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/cloud/cloud_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:59.878807 zephyr_python_api-0.1.0/zephyr/scale/cloud/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/cloud/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29178 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/cloud/endpoints/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/cloud/endpoints/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:59.878807 zephyr_python_api-0.1.0/zephyr/scale/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:59.878807 zephyr_python_api-0.1.0/zephyr/scale/server/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/server/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15265 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/server/endpoints/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/server/endpoints/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/server/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/server/server_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/scale/zephyr_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:59.878807 zephyr_python_api-0.1.0/zephyr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-02 16:36:27.000000 zephyr_python_api-0.1.0/zephyr/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:36:59.878807 zephyr_python_api-0.1.0/zephyr_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-02 16:36:59.000000 zephyr_python_api-0.1.0/zephyr_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-02 16:36:59.000000 zephyr_python_api-0.1.0/zephyr_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:36:59.000000 zephyr_python_api-0.1.0/zephyr_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 16:36:59.000000 zephyr_python_api-0.1.0/zephyr_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 16:36:59.000000 zephyr_python_api-0.1.0/zephyr_python_api.egg-info/top_level.txt
```

### Comparing `zephyr_python_api-0.0.5/LICENSE` & `zephyr_python_api-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zephyr_python_api-0.0.5/PKG-INFO` & `zephyr_python_api-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyr-python-api
-Version: 0.0.5
+Version: 0.1.0
 Summary: Zephyr (TM4J) Python REST API wrapper
 Home-page: https://github.com/nassauwinter/zephyr-python-api
 Author: Petr Sharapenko
 Author-email: nassauwinter@gmail.com
 Project-URL: Bug Tracker, https://github.com/nassauwinter/zephyr-python-api/issues
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -23,15 +23,19 @@
 # Zephyr-python-api
 
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zephyr-python-api)
 ![PyPI](https://img.shields.io/pypi/v/zephyr-python-api)
 ![PyPI - License](https://img.shields.io/pypi/l/zephyr-python-api)
 ### Project description
-This is a set of wrappers for Zephyr Scale (TM4J) REST API. This means you can interact with Zephyr Scale without GUI, access it with python code and create automation scripts for your every day interactions.
+This is a set of wrappers for Zephyr Scale (TM4J) REST API. 
+This means you can interact with Zephyr Scale without GUI, access it with python code and create 
+automation scripts for your every day interactions.
+
+For more detailed information please see [the project's documentation](https://zephyr-python-api.readthedocs.io/en/main/index.html).
 
 To be done:
 * More usage examples
 * Tests, tests and tests for gods of testing
 * Convenient docs
 * Implementing higher level wrappers representing Test Case, Test Cycle, etc.
 
@@ -43,15 +47,15 @@
 
 ### Example usage
 
 Zephyr Cloud auth:
 ```python
 from zephyr import ZephyrScale
 
-zscale = ZephyrScale(token=<your_token>)
+zscale = ZephyrScale(token="<your_token>")
 ```
 
 Zephyr Server (TM4J) auth:
 ```python
 from zephyr import ZephyrScale
 
 # Auth can be made with Jira token
@@ -59,15 +63,15 @@
 
 # or with login and password (suggest using get_pass)
 auth = {"username": "<your_login>", "password": "<your_password>"}
 
 # or even session cookie dict
 auth = {"cookies": "<session_cookie_dict>"}
 
-zscale = ZephyrScale.server_api(base_url=<your_base_url>, **auth)
+zscale = ZephyrScale.server_api(base_url="<your_base_url>", **auth)
 ```
 
 Then it is possible to interact with api wrappers:
 ```python
 zapi = zscale.api
 
 # Get all test cases
@@ -76,19 +80,14 @@
 # Get a single test case by its id
 test_case = zapi.test_cases.get_test_case("<test_case_id>")
 
 # Create a test case
 creation_result = zapi.test_cases.create_test_case("<project_key>", "test_case_name")
 ```
 
-### Troubleshooting
-
-For troubleshooting see [TROUBLESHOOTING.md](TROUBLESHOOTING.md)
-
-
 ### License
 
 This library is licensed under the Apache 2.0 License.
 
 ### Links
 
 [Zephyr Scale Cloud API docs](https://support.smartbear.com/zephyr-scale-cloud/api-docs/)
```

### Comparing `zephyr_python_api-0.0.5/README.md` & `zephyr_python_api-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Zephyr-python-api
 
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zephyr-python-api)
 ![PyPI](https://img.shields.io/pypi/v/zephyr-python-api)
 ![PyPI - License](https://img.shields.io/pypi/l/zephyr-python-api)
 ### Project description
-This is a set of wrappers for Zephyr Scale (TM4J) REST API. This means you can interact with Zephyr Scale without GUI, access it with python code and create automation scripts for your every day interactions.
+This is a set of wrappers for Zephyr Scale (TM4J) REST API. 
+This means you can interact with Zephyr Scale without GUI, access it with python code and create 
+automation scripts for your every day interactions.
+
+For more detailed information please see [the project's documentation](https://zephyr-python-api.readthedocs.io/en/main/index.html).
 
 To be done:
 * More usage examples
 * Tests, tests and tests for gods of testing
 * Convenient docs
 * Implementing higher level wrappers representing Test Case, Test Cycle, etc.
 
@@ -21,15 +25,15 @@
 
 ### Example usage
 
 Zephyr Cloud auth:
 ```python
 from zephyr import ZephyrScale
 
-zscale = ZephyrScale(token=<your_token>)
+zscale = ZephyrScale(token="<your_token>")
 ```
 
 Zephyr Server (TM4J) auth:
 ```python
 from zephyr import ZephyrScale
 
 # Auth can be made with Jira token
@@ -37,15 +41,15 @@
 
 # or with login and password (suggest using get_pass)
 auth = {"username": "<your_login>", "password": "<your_password>"}
 
 # or even session cookie dict
 auth = {"cookies": "<session_cookie_dict>"}
 
-zscale = ZephyrScale.server_api(base_url=<your_base_url>, **auth)
+zscale = ZephyrScale.server_api(base_url="<your_base_url>", **auth)
 ```
 
 Then it is possible to interact with api wrappers:
 ```python
 zapi = zscale.api
 
 # Get all test cases
@@ -54,19 +58,14 @@
 # Get a single test case by its id
 test_case = zapi.test_cases.get_test_case("<test_case_id>")
 
 # Create a test case
 creation_result = zapi.test_cases.create_test_case("<project_key>", "test_case_name")
 ```
 
-### Troubleshooting
-
-For troubleshooting see [TROUBLESHOOTING.md](TROUBLESHOOTING.md)
-
-
 ### License
 
 This library is licensed under the Apache 2.0 License.
 
 ### Links
 
 [Zephyr Scale Cloud API docs](https://support.smartbear.com/zephyr-scale-cloud/api-docs/)
```

### Comparing `zephyr_python_api-0.0.5/setup.cfg` & `zephyr_python_api-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `zephyr_python_api-0.0.5/zephyr/scale/scale.py` & `zephyr_python_api-0.1.0/zephyr/scale/scale.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+A module with the Zephyr Scale base object.
+"""
+
 import logging
 
 from zephyr.scale.zephyr_session import ZephyrSession
 from zephyr.scale.cloud.cloud_api import CloudApiWrapper
 from zephyr.scale.server.server_api import ServerApiWrapper
 
 
@@ -9,20 +13,24 @@
 
 API_V2 = "v2"
 API_V1 = "v1"
 
 
 class ZephyrScale:
     """
-    Zephyr Scale base object to interact with other objects or raw api by its methods.
+    Zephyr Scale base object to interact with raw Zephyr APIs or other Zephyr entities. You should
+    define the API version of Zephyr Scale instance you are going to work with. Server is v1 and
+    Cloud is v2.
 
     NOTE: Cloud API accepts only token auth, whereas Server API works with Jira auth methods.
 
     :param base_url: base API url to connect with
     :param api_version: 'v2' for Cloud and 'v1' for Server
+
+    :raises ValueError: if api_version is not 'v1' or 'v2'
     """
     def __init__(self, base_url=None, api_version=API_V2, **kwargs):
         base_url = DEFAULT_BASE_URL if not base_url else base_url
         session = ZephyrSession(base_url=base_url, **kwargs)
 
         if api_version.lower() == API_V2:
             self.api = CloudApiWrapper(session)
@@ -30,9 +38,13 @@
             self.api = ServerApiWrapper(session)
         else:
             raise ValueError("API version should be either 'v1' (Server) or 'v2' (Cloud)")
         self.logger = logging.getLogger(__name__)
 
     @classmethod
     def server_api(cls, base_url, **kwargs):
-        """Alternative constructor for Zephyr Scale Server client"""
+        """
+        Alternative constructor for Zephyr Scale Server client.
+
+        :param base_url: base API url to connect with
+        """
         return cls(base_url=base_url, api_version=API_V1, **kwargs)
```

### Comparing `zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/__init__.py` & `zephyr_python_api-0.1.0/zephyr/scale/server/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/endpoints.py` & `zephyr_python_api-0.1.0/zephyr/scale/server/endpoints/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-from ...zephyr_session import ZephyrSession
+from ...zephyr_session import EndpointTemplate
 from .paths import ServerPaths as Paths
 
 
-class EndpointTemplate:
-    """Class with basic constructor for endpoint classes"""
-    def __init__(self, session: ZephyrSession):
-        self.session = session
-
-
 class TestCaseEndpoints(EndpointTemplate):
     """Api wrapper for "Test Case" endpoints"""
 
     def create_test_case(self, project_key, name, **kwargs):
         """Creates a new Test Case"""
         json = {"projectKey": project_key,
                 "name": name}
```

### Comparing `zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/paths.py` & `zephyr_python_api-0.1.0/zephyr/scale/server/endpoints/paths.py`

 * *Files identical despite different names*

### Comparing `zephyr_python_api-0.0.5/zephyr/scale/server/server_defaults.py` & `zephyr_python_api-0.1.0/zephyr/scale/server/server_defaults.py`

 * *Files identical despite different names*

### Comparing `zephyr_python_api-0.0.5/zephyr/scale/zephyr_session.py` & `zephyr_python_api-0.1.0/zephyr/scale/zephyr_session.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+"""
+A module for Zephyr Scale session object.
+"""
 import logging
 from urllib.parse import urlparse, parse_qs
 
 from requests import HTTPError, Session
 
 
 INIT_SESSION_MSG = "Initialize session by {}"
 
 
 class InvalidAuthData(Exception):
-    """Invalid authentication data provided"""
+    """Raised when Invalid authentication data provided."""
 
 
 class ZephyrSession:
     """
-    Zephyr Scale basic session object.
+    Zephyr Scale basic session object. The authentication and response handling logic
+    is placed here.
 
     :param base_url: url to make requests to
     :param token: auth token
     :param username: username
     :param password: password
     :param cookies: cookie dict
 
-    :keyword session_attrs: a dict with session attrs to be set as keys and their values
+    :param keyword session_attrs: a dict with session attrs to be set as keys and their values
     """
     def __init__(self, base_url, token=None, username=None, password=None, cookies=None, **kwargs):
         self.base_url = base_url
         self._session = Session()
 
         self.logger = logging.getLogger(__name__)
 
@@ -51,44 +55,89 @@
     def _modify_session(self, **kwargs):
         """Modify requests session with extra arguments"""
         self.logger.debug(f"Modify requests session object with {kwargs}")
         for session_attr, value in kwargs.items():
             setattr(self._session, session_attr, value)
 
     def _request(self, method: str, endpoint: str, return_raw: bool = False, **kwargs):
-        """General request wrapper with logging and handling response"""
+        """
+        General request wrapper with logging and handling response
+
+        :param method: request method
+        :param endpoint: endpoint to make request to
+        :param return_raw: whether to return raw response or not
+
+        :raises: HTTPError if response status code is 400 or higher
+
+        :return: response json, empty str or raw response
+        """
         self.logger.debug(f"{method.capitalize()} data: endpoint={endpoint} and {kwargs}")
         url = self._create_url(endpoint)
         response = self._session.request(method=method, url=url, **kwargs)
         if response.status_code < 400:
             if return_raw:
                 return response
             if response.text:
                 return response.json()
             return ""
         raise HTTPError(f"Error {response.status_code}. Response: {response.content}")
 
     def get(self, endpoint: str, params: dict = None, **kwargs):
-        """Get request wrapper"""
+        """
+        Get request wrapper.
+
+        :param endpoint: endpoint to make request to
+        :param params: dict with params to be passed to request
+
+        :return: response json, empty str or raw response
+        """
         return self._request("get", endpoint, params=params, **kwargs)
 
     def post(self, endpoint: str, json: dict = None, **kwargs):
-        """Post request wrapper"""
+        """
+        Post request wrapper.
+
+        :param endpoint: endpoint to make request to
+        :param json: json to be passed to request
+
+        :return: response json, empty str or raw response
+        """
         return self._request("post", endpoint, json=json, **kwargs)
 
     def put(self, endpoint: str, json: dict = None, **kwargs):
-        """Put request wrapper"""
+        """
+        Put request wrapper
+
+        :param endpoint: endpoint to make request to
+        :param json: json to be passed to request
+
+        :return: response json, empty str or raw response
+        """
         return self._request("put", endpoint, json=json, **kwargs)
 
     def delete(self, endpoint: str, **kwargs):
-        """Delete request wrapper"""
+        """
+        Delete request wrapper.
+
+        :param endpoint: endpoint to make request to
+
+        :return: response json, empty str or raw response
+        """
         return self._request("delete", endpoint, **kwargs)
 
     def get_paginated(self, endpoint, params=None):
-        """Get paginated data"""
+        """
+        Get request wrapper for getting paginated data. Yields values from multiple get requests
+        responses.
+
+        :param endpoint: endpoint to make request to
+        :param params: dict with params to be passed to request
+
+        :return: generator with values from responses
+        """
         self.logger.debug(f"Get paginated data from endpoint={endpoint} and params={params}")
         if params is None:
             params = {}
 
         while True:
             response = self.get(endpoint, params=params)
             if "values" not in response:
@@ -102,17 +151,28 @@
             params_str = urlparse(response.get("next")).query
             params.update(parse_qs(params_str))
 
         return
 
     def post_file(self, endpoint: str, file_path: str, to_files=None, **kwargs):
         """
-        Post wrapper to send a file. Handles single file opening,
-        sending its content and closing
+        Post wrapper to send a file. Handles single file opening, sending its content and closing.
+
+        :param endpoint: endpoint to make request to
+        :param file_path: path to file to be sent
+        :param to_files: dict with files to be sent along with the main file
+
+        :return: response json, empty str or raw response
         """
         with open(file_path, "rb") as file:
             files = {"file": file}
 
             if to_files:
                 files.update(to_files)
 
             return self._request("post", endpoint, files=files, **kwargs)
+
+
+class EndpointTemplate:
+    """Class with basic constructor for endpoint classes"""
+    def __init__(self, session: ZephyrSession):
+        self.session = session
```

### Comparing `zephyr_python_api-0.0.5/zephyr/utils/common.py` & `zephyr_python_api-0.1.0/zephyr/utils/common.py`

 * *Files identical despite different names*

### Comparing `zephyr_python_api-0.0.5/zephyr_python_api.egg-info/PKG-INFO` & `zephyr_python_api-0.1.0/zephyr_python_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyr-python-api
-Version: 0.0.5
+Version: 0.1.0
 Summary: Zephyr (TM4J) Python REST API wrapper
 Home-page: https://github.com/nassauwinter/zephyr-python-api
 Author: Petr Sharapenko
 Author-email: nassauwinter@gmail.com
 Project-URL: Bug Tracker, https://github.com/nassauwinter/zephyr-python-api/issues
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -23,15 +23,19 @@
 # Zephyr-python-api
 
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zephyr-python-api)
 ![PyPI](https://img.shields.io/pypi/v/zephyr-python-api)
 ![PyPI - License](https://img.shields.io/pypi/l/zephyr-python-api)
 ### Project description
-This is a set of wrappers for Zephyr Scale (TM4J) REST API. This means you can interact with Zephyr Scale without GUI, access it with python code and create automation scripts for your every day interactions.
+This is a set of wrappers for Zephyr Scale (TM4J) REST API. 
+This means you can interact with Zephyr Scale without GUI, access it with python code and create 
+automation scripts for your every day interactions.
+
+For more detailed information please see [the project's documentation](https://zephyr-python-api.readthedocs.io/en/main/index.html).
 
 To be done:
 * More usage examples
 * Tests, tests and tests for gods of testing
 * Convenient docs
 * Implementing higher level wrappers representing Test Case, Test Cycle, etc.
 
@@ -43,15 +47,15 @@
 
 ### Example usage
 
 Zephyr Cloud auth:
 ```python
 from zephyr import ZephyrScale
 
-zscale = ZephyrScale(token=<your_token>)
+zscale = ZephyrScale(token="<your_token>")
 ```
 
 Zephyr Server (TM4J) auth:
 ```python
 from zephyr import ZephyrScale
 
 # Auth can be made with Jira token
@@ -59,15 +63,15 @@
 
 # or with login and password (suggest using get_pass)
 auth = {"username": "<your_login>", "password": "<your_password>"}
 
 # or even session cookie dict
 auth = {"cookies": "<session_cookie_dict>"}
 
-zscale = ZephyrScale.server_api(base_url=<your_base_url>, **auth)
+zscale = ZephyrScale.server_api(base_url="<your_base_url>", **auth)
 ```
 
 Then it is possible to interact with api wrappers:
 ```python
 zapi = zscale.api
 
 # Get all test cases
@@ -76,19 +80,14 @@
 # Get a single test case by its id
 test_case = zapi.test_cases.get_test_case("<test_case_id>")
 
 # Create a test case
 creation_result = zapi.test_cases.create_test_case("<project_key>", "test_case_name")
 ```
 
-### Troubleshooting
-
-For troubleshooting see [TROUBLESHOOTING.md](TROUBLESHOOTING.md)
-
-
 ### License
 
 This library is licensed under the Apache 2.0 License.
 
 ### Links
 
 [Zephyr Scale Cloud API docs](https://support.smartbear.com/zephyr-scale-cloud/api-docs/)
```

