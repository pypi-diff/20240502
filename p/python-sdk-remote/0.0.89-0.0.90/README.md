# Comparing `tmp/python-sdk-remote-0.0.89.tar.gz` & `tmp/python_sdk_remote-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sdk-remote-0.0.89.tar", last modified: Fri Apr 12 14:49:44 2024, max compression
+gzip compressed data, was "python_sdk_remote-0.0.90.tar", last modified: Wed May  1 07:16:07 2024, max compression
```

## Comparing `python-sdk-remote-0.0.89.tar` & `python_sdk_remote-0.0.90.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:49:44.498249 python-sdk-remote-0.0.89/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 14:49:44.498249 python-sdk-remote-0.0.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:49:44.494249 python-sdk-remote-0.0.89/python_sdk_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:49:44.498249 python-sdk-remote-0.0.89/python_sdk_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/python_sdk_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/python_sdk_remote/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/python_sdk_remote/src/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/python_sdk_remote/src/mini_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/python_sdk_remote/src/our_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/python_sdk_remote/src/unified_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/python_sdk_remote/src/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/python_sdk_remote/src/valid_json_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/python_sdk_remote/src/validate_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:49:44.498249 python-sdk-remote-0.0.89/python_sdk_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 14:49:44.000000 python-sdk-remote-0.0.89/python_sdk_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 14:49:44.000000 python-sdk-remote-0.0.89/python_sdk_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:49:44.000000 python-sdk-remote-0.0.89/python_sdk_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 14:49:44.000000 python-sdk-remote-0.0.89/python_sdk_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 14:49:44.000000 python-sdk-remote-0.0.89/python_sdk_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:49:44.498249 python-sdk-remote-0.0.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-12 14:49:29.000000 python-sdk-remote-0.0.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:16:07.507834 python_sdk_remote-0.0.90/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-01 07:16:07.507834 python_sdk_remote-0.0.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:16:07.503834 python_sdk_remote-0.0.90/python_sdk_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:16:07.507834 python_sdk_remote-0.0.90/python_sdk_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/python_sdk_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/python_sdk_remote/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/python_sdk_remote/src/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/python_sdk_remote/src/mini_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/python_sdk_remote/src/our_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/python_sdk_remote/src/unified_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/python_sdk_remote/src/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/python_sdk_remote/src/valid_json_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/python_sdk_remote/src/validate_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 07:16:07.507834 python_sdk_remote-0.0.90/python_sdk_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-01 07:16:07.000000 python_sdk_remote-0.0.90/python_sdk_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-01 07:16:07.000000 python_sdk_remote-0.0.90/python_sdk_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 07:16:07.000000 python_sdk_remote-0.0.90/python_sdk_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-01 07:16:07.000000 python_sdk_remote-0.0.90/python_sdk_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 07:16:07.000000 python_sdk_remote-0.0.90/python_sdk_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 07:16:07.507834 python_sdk_remote-0.0.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-01 07:15:53.000000 python_sdk_remote-0.0.90/setup.py
```

### Comparing `python-sdk-remote-0.0.89/PKG-INFO` & `python_sdk_remote-0.0.90/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.89
+Version: 0.0.90
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-sdk-remote-0.0.89/README.md` & `python_sdk_remote-0.0.90/README.md`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.89/python_sdk_remote/src/constants.py` & `python_sdk_remote-0.0.90/python_sdk_remote/src/constants.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.89/python_sdk_remote/src/mini_logger.py` & `python_sdk_remote-0.0.90/python_sdk_remote/src/mini_logger.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.89/python_sdk_remote/src/our_object.py` & `python_sdk_remote-0.0.90/python_sdk_remote/src/our_object.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.89/python_sdk_remote/src/unified_json.py` & `python_sdk_remote-0.0.90/python_sdk_remote/src/unified_json.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.89/python_sdk_remote/src/utilities.py` & `python_sdk_remote-0.0.90/python_sdk_remote/src/utilities.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.89/python_sdk_remote/src/validate_environment.py` & `python_sdk_remote-0.0.90/python_sdk_remote/src/validate_environment.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.89/python_sdk_remote.egg-info/PKG-INFO` & `python_sdk_remote-0.0.90/python_sdk_remote.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.89
+Version: 0.0.90
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-sdk-remote-0.0.89/python_sdk_remote.egg-info/SOURCES.txt` & `python_sdk_remote-0.0.90/python_sdk_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.89/setup.py` & `python_sdk_remote-0.0.90/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 PACKAGE_NAME = "python-sdk-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.89',  # https://pypi.org/project/python-sdk-remote/
+    version='0.0.90',  # https://pypi.org/project/python-sdk-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Python SDK Local Python",
     long_description="This is a package for sharing common functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

