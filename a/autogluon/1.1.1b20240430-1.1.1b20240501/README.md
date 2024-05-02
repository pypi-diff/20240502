# Comparing `tmp/autogluon-1.1.1b20240430.tar.gz` & `tmp/autogluon-1.1.1b20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.1.1b20240430.tar", last modified: Tue Apr 30 09:05:42 2024, max compression
+gzip compressed data, was "autogluon-1.1.1b20240501.tar", last modified: Wed May  1 09:05:20 2024, max compression
```

## Comparing `autogluon-1.1.1b20240430.tar` & `autogluon-1.1.1b20240501.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:42.146494 autogluon-1.1.1b20240430/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-30 09:05:42.146494 autogluon-1.1.1b20240430/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:05:42.146494 autogluon-1.1.1b20240430/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-30 09:03:50.000000 autogluon-1.1.1b20240430/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:42.146494 autogluon-1.1.1b20240430/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:42.146494 autogluon-1.1.1b20240430/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:42.146494 autogluon-1.1.1b20240430/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:03:50.000000 autogluon-1.1.1b20240430/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:42.146494 autogluon-1.1.1b20240430/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-30 09:05:42.000000 autogluon-1.1.1b20240430/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-30 09:05:42.000000 autogluon-1.1.1b20240430/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:05:42.000000 autogluon-1.1.1b20240430/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 09:05:42.000000 autogluon-1.1.1b20240430/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-30 09:05:42.000000 autogluon-1.1.1b20240430/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 09:05:42.000000 autogluon-1.1.1b20240430/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:05:42.000000 autogluon-1.1.1b20240430/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:20.253454 autogluon-1.1.1b20240501/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-01 09:05:20.253454 autogluon-1.1.1b20240501/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 09:05:20.253454 autogluon-1.1.1b20240501/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-01 09:03:44.000000 autogluon-1.1.1b20240501/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:20.249454 autogluon-1.1.1b20240501/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:20.249454 autogluon-1.1.1b20240501/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:20.253454 autogluon-1.1.1b20240501/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 09:03:44.000000 autogluon-1.1.1b20240501/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:20.253454 autogluon-1.1.1b20240501/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-01 09:05:20.000000 autogluon-1.1.1b20240501/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-01 09:05:20.000000 autogluon-1.1.1b20240501/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:05:20.000000 autogluon-1.1.1b20240501/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 09:05:20.000000 autogluon-1.1.1b20240501/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 09:05:20.000000 autogluon-1.1.1b20240501/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 09:05:20.000000 autogluon-1.1.1b20240501/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:05:20.000000 autogluon-1.1.1b20240501/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.1.1b20240430/PKG-INFO` & `autogluon-1.1.1b20240501/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240430
+Version: 1.1.1b20240501
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-1.1.1b20240430/setup.py` & `autogluon-1.1.1b20240501/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.1.1b20240430/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.1.1b20240501/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240430
+Version: 1.1.1b20240501
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

