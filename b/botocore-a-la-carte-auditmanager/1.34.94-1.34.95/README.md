# Comparing `tmp/botocore-a-la-carte-auditmanager-1.34.94.tar.gz` & `tmp/botocore-a-la-carte-auditmanager-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-auditmanager-1.34.94.tar", last modified: Tue Apr 30 01:01:18 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-auditmanager-1.34.95.tar", last modified: Wed May  1 01:06:11 2024, max compression
```

## Comparing `botocore-a-la-carte-auditmanager-1.34.94.tar` & `botocore-a-la-carte-auditmanager-1.34.95.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:18.367239 botocore-a-la-carte-auditmanager-1.34.94/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-30 01:01:18.000000 botocore-a-la-carte-auditmanager-1.34.94/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-30 01:01:18.367239 botocore-a-la-carte-auditmanager-1.34.94/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:18.363239 botocore-a-la-carte-auditmanager-1.34.94/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:18.363239 botocore-a-la-carte-auditmanager-1.34.94/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:18.363239 botocore-a-la-carte-auditmanager-1.34.94/botocore/data/auditmanager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:18.363239 botocore-a-la-carte-auditmanager-1.34.94/botocore/data/auditmanager/2017-07-25/
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-30 01:01:13.000000 botocore-a-la-carte-auditmanager-1.34.94/botocore/data/auditmanager/2017-07-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 01:01:13.000000 botocore-a-la-carte-auditmanager-1.34.94/botocore/data/auditmanager/2017-07-25/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 01:01:13.000000 botocore-a-la-carte-auditmanager-1.34.94/botocore/data/auditmanager/2017-07-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   216805 2024-04-30 01:01:13.000000 botocore-a-la-carte-auditmanager-1.34.94/botocore/data/auditmanager/2017-07-25/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:18.367239 botocore-a-la-carte-auditmanager-1.34.94/botocore_a_la_carte_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-30 01:01:18.000000 botocore-a-la-carte-auditmanager-1.34.94/botocore_a_la_carte_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-30 01:01:18.000000 botocore-a-la-carte-auditmanager-1.34.94/botocore_a_la_carte_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 01:01:18.000000 botocore-a-la-carte-auditmanager-1.34.94/botocore_a_la_carte_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 01:01:18.000000 botocore-a-la-carte-auditmanager-1.34.94/botocore_a_la_carte_auditmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 01:01:18.367239 botocore-a-la-carte-auditmanager-1.34.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-30 01:01:18.000000 botocore-a-la-carte-auditmanager-1.34.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:11.268787 botocore-a-la-carte-auditmanager-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-01 01:06:11.000000 botocore-a-la-carte-auditmanager-1.34.95/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-01 01:06:11.268787 botocore-a-la-carte-auditmanager-1.34.95/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:11.264787 botocore-a-la-carte-auditmanager-1.34.95/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:11.264787 botocore-a-la-carte-auditmanager-1.34.95/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:11.264787 botocore-a-la-carte-auditmanager-1.34.95/botocore/data/auditmanager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:11.264787 botocore-a-la-carte-auditmanager-1.34.95/botocore/data/auditmanager/2017-07-25/
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-05-01 01:06:02.000000 botocore-a-la-carte-auditmanager-1.34.95/botocore/data/auditmanager/2017-07-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 01:06:02.000000 botocore-a-la-carte-auditmanager-1.34.95/botocore/data/auditmanager/2017-07-25/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 01:06:02.000000 botocore-a-la-carte-auditmanager-1.34.95/botocore/data/auditmanager/2017-07-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   216805 2024-05-01 01:06:02.000000 botocore-a-la-carte-auditmanager-1.34.95/botocore/data/auditmanager/2017-07-25/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:11.268787 botocore-a-la-carte-auditmanager-1.34.95/botocore_a_la_carte_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-01 01:06:11.000000 botocore-a-la-carte-auditmanager-1.34.95/botocore_a_la_carte_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-01 01:06:11.000000 botocore-a-la-carte-auditmanager-1.34.95/botocore_a_la_carte_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:06:11.000000 botocore-a-la-carte-auditmanager-1.34.95/botocore_a_la_carte_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 01:06:11.000000 botocore-a-la-carte-auditmanager-1.34.95/botocore_a_la_carte_auditmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 01:06:11.268787 botocore-a-la-carte-auditmanager-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-01 01:06:11.000000 botocore-a-la-carte-auditmanager-1.34.95/setup.py
```

### Comparing `botocore-a-la-carte-auditmanager-1.34.94/LICENSE.txt` & `botocore-a-la-carte-auditmanager-1.34.95/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-auditmanager-1.34.94/PKG-INFO` & `botocore-a-la-carte-auditmanager-1.34.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-auditmanager
-Version: 1.34.94
+Version: 1.34.95
 Summary: auditmanager data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-auditmanager-1.34.94/botocore/data/auditmanager/2017-07-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-auditmanager-1.34.95/botocore/data/auditmanager/2017-07-25/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-auditmanager-1.34.94/botocore/data/auditmanager/2017-07-25/service-2.json` & `botocore-a-la-carte-auditmanager-1.34.95/botocore/data/auditmanager/2017-07-25/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-auditmanager-1.34.94/botocore_a_la_carte_auditmanager.egg-info/PKG-INFO` & `botocore-a-la-carte-auditmanager-1.34.95/botocore_a_la_carte_auditmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-auditmanager
-Version: 1.34.94
+Version: 1.34.95
 Summary: auditmanager data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-auditmanager-1.34.94/setup.py` & `botocore-a-la-carte-auditmanager-1.34.95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-auditmanager',
-    version="1.34.94",
+    version="1.34.95",
     description='auditmanager data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/auditmanager/*/*.json'],
```

