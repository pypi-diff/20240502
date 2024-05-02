# Comparing `tmp/botocore-a-la-carte-kinesis-1.34.94.tar.gz` & `tmp/botocore-a-la-carte-kinesis-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-kinesis-1.34.94.tar", last modified: Tue Apr 30 01:01:33 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-kinesis-1.34.95.tar", last modified: Wed May  1 01:06:26 2024, max compression
```

## Comparing `botocore-a-la-carte-kinesis-1.34.94.tar` & `botocore-a-la-carte-kinesis-1.34.95.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:33.623284 botocore-a-la-carte-kinesis-1.34.94/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-30 01:01:33.000000 botocore-a-la-carte-kinesis-1.34.94/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-30 01:01:33.623284 botocore-a-la-carte-kinesis-1.34.94/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:33.619284 botocore-a-la-carte-kinesis-1.34.94/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:33.619284 botocore-a-la-carte-kinesis-1.34.94/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:33.619284 botocore-a-la-carte-kinesis-1.34.94/botocore/data/kinesis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:33.623284 botocore-a-la-carte-kinesis-1.34.94/botocore/data/kinesis/2013-12-02/
--rw-r--r--   0 runner    (1001) docker     (127)   129294 2024-04-30 01:01:14.000000 botocore-a-la-carte-kinesis-1.34.94/botocore/data/kinesis/2013-12-02/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 01:01:14.000000 botocore-a-la-carte-kinesis-1.34.94/botocore/data/kinesis/2013-12-02/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-30 01:01:14.000000 botocore-a-la-carte-kinesis-1.34.94/botocore/data/kinesis/2013-12-02/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   159464 2024-04-30 01:01:14.000000 botocore-a-la-carte-kinesis-1.34.94/botocore/data/kinesis/2013-12-02/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-30 01:01:14.000000 botocore-a-la-carte-kinesis-1.34.94/botocore/data/kinesis/2013-12-02/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:01:33.623284 botocore-a-la-carte-kinesis-1.34.94/botocore_a_la_carte_kinesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-30 01:01:33.000000 botocore-a-la-carte-kinesis-1.34.94/botocore_a_la_carte_kinesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-30 01:01:33.000000 botocore-a-la-carte-kinesis-1.34.94/botocore_a_la_carte_kinesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 01:01:33.000000 botocore-a-la-carte-kinesis-1.34.94/botocore_a_la_carte_kinesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 01:01:33.000000 botocore-a-la-carte-kinesis-1.34.94/botocore_a_la_carte_kinesis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 01:01:33.623284 botocore-a-la-carte-kinesis-1.34.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-30 01:01:33.000000 botocore-a-la-carte-kinesis-1.34.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:26.708772 botocore-a-la-carte-kinesis-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-01 01:06:26.000000 botocore-a-la-carte-kinesis-1.34.95/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-01 01:06:26.708772 botocore-a-la-carte-kinesis-1.34.95/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:26.704772 botocore-a-la-carte-kinesis-1.34.95/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:26.704772 botocore-a-la-carte-kinesis-1.34.95/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:26.704772 botocore-a-la-carte-kinesis-1.34.95/botocore/data/kinesis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:26.708772 botocore-a-la-carte-kinesis-1.34.95/botocore/data/kinesis/2013-12-02/
+-rw-r--r--   0 runner    (1001) docker     (127)   129294 2024-05-01 01:06:02.000000 botocore-a-la-carte-kinesis-1.34.95/botocore/data/kinesis/2013-12-02/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 01:06:02.000000 botocore-a-la-carte-kinesis-1.34.95/botocore/data/kinesis/2013-12-02/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-01 01:06:02.000000 botocore-a-la-carte-kinesis-1.34.95/botocore/data/kinesis/2013-12-02/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   159464 2024-05-01 01:06:02.000000 botocore-a-la-carte-kinesis-1.34.95/botocore/data/kinesis/2013-12-02/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-01 01:06:02.000000 botocore-a-la-carte-kinesis-1.34.95/botocore/data/kinesis/2013-12-02/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:26.708772 botocore-a-la-carte-kinesis-1.34.95/botocore_a_la_carte_kinesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-01 01:06:26.000000 botocore-a-la-carte-kinesis-1.34.95/botocore_a_la_carte_kinesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-01 01:06:26.000000 botocore-a-la-carte-kinesis-1.34.95/botocore_a_la_carte_kinesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:06:26.000000 botocore-a-la-carte-kinesis-1.34.95/botocore_a_la_carte_kinesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 01:06:26.000000 botocore-a-la-carte-kinesis-1.34.95/botocore_a_la_carte_kinesis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 01:06:26.708772 botocore-a-la-carte-kinesis-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-01 01:06:26.000000 botocore-a-la-carte-kinesis-1.34.95/setup.py
```

### Comparing `botocore-a-la-carte-kinesis-1.34.94/LICENSE.txt` & `botocore-a-la-carte-kinesis-1.34.95/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-kinesis-1.34.94/PKG-INFO` & `botocore-a-la-carte-kinesis-1.34.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-kinesis
-Version: 1.34.94
+Version: 1.34.95
 Summary: kinesis data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-kinesis-1.34.94/botocore/data/kinesis/2013-12-02/endpoint-rule-set-1.json` & `botocore-a-la-carte-kinesis-1.34.95/botocore/data/kinesis/2013-12-02/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-kinesis-1.34.94/botocore/data/kinesis/2013-12-02/paginators-1.json` & `botocore-a-la-carte-kinesis-1.34.95/botocore/data/kinesis/2013-12-02/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-kinesis-1.34.94/botocore/data/kinesis/2013-12-02/service-2.json` & `botocore-a-la-carte-kinesis-1.34.95/botocore/data/kinesis/2013-12-02/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-kinesis-1.34.94/botocore/data/kinesis/2013-12-02/waiters-2.json` & `botocore-a-la-carte-kinesis-1.34.95/botocore/data/kinesis/2013-12-02/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-kinesis-1.34.94/botocore_a_la_carte_kinesis.egg-info/PKG-INFO` & `botocore-a-la-carte-kinesis-1.34.95/botocore_a_la_carte_kinesis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-kinesis
-Version: 1.34.94
+Version: 1.34.95
 Summary: kinesis data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-kinesis-1.34.94/setup.py` & `botocore-a-la-carte-kinesis-1.34.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-kinesis',
-    version="1.34.94",
+    version="1.34.95",
     description='kinesis data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/kinesis/*/*.json'],
```

