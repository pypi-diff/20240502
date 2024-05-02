# Comparing `tmp/botocore-a-la-carte-opsworks-1.34.95.tar.gz` & `tmp/botocore-a-la-carte-opsworks-1.34.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-opsworks-1.34.95.tar", last modified: Wed May  1 01:06:33 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-opsworks-1.34.96.tar", last modified: Thu May  2 01:01:34 2024, max compression
```

## Comparing `botocore-a-la-carte-opsworks-1.34.95.tar` & `botocore-a-la-carte-opsworks-1.34.96.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.748764 botocore-a-la-carte-opsworks-1.34.95/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-01 01:06:33.000000 botocore-a-la-carte-opsworks-1.34.95/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-01 01:06:33.748764 botocore-a-la-carte-opsworks-1.34.95/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.744764 botocore-a-la-carte-opsworks-1.34.95/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.744764 botocore-a-la-carte-opsworks-1.34.95/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.744764 botocore-a-la-carte-opsworks-1.34.95/botocore/data/opsworks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.748764 botocore-a-la-carte-opsworks-1.34.95/botocore/data/opsworks/2013-02-18/
--rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-05-01 01:06:02.000000 botocore-a-la-carte-opsworks-1.34.95/botocore/data/opsworks/2013-02-18/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 01:06:02.000000 botocore-a-la-carte-opsworks-1.34.95/botocore/data/opsworks/2013-02-18/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-01 01:06:02.000000 botocore-a-la-carte-opsworks-1.34.95/botocore/data/opsworks/2013-02-18/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   273984 2024-05-01 01:06:02.000000 botocore-a-la-carte-opsworks-1.34.95/botocore/data/opsworks/2013-02-18/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-01 01:06:02.000000 botocore-a-la-carte-opsworks-1.34.95/botocore/data/opsworks/2013-02-18/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:06:33.748764 botocore-a-la-carte-opsworks-1.34.95/botocore_a_la_carte_opsworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-01 01:06:33.000000 botocore-a-la-carte-opsworks-1.34.95/botocore_a_la_carte_opsworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-01 01:06:33.000000 botocore-a-la-carte-opsworks-1.34.95/botocore_a_la_carte_opsworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:06:33.000000 botocore-a-la-carte-opsworks-1.34.95/botocore_a_la_carte_opsworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 01:06:33.000000 botocore-a-la-carte-opsworks-1.34.95/botocore_a_la_carte_opsworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 01:06:33.748764 botocore-a-la-carte-opsworks-1.34.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-01 01:06:33.000000 botocore-a-la-carte-opsworks-1.34.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:34.245051 botocore-a-la-carte-opsworks-1.34.96/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-02 01:01:33.000000 botocore-a-la-carte-opsworks-1.34.96/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-02 01:01:34.241051 botocore-a-la-carte-opsworks-1.34.96/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:34.241051 botocore-a-la-carte-opsworks-1.34.96/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:34.241051 botocore-a-la-carte-opsworks-1.34.96/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:34.241051 botocore-a-la-carte-opsworks-1.34.96/botocore/data/opsworks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:34.241051 botocore-a-la-carte-opsworks-1.34.96/botocore/data/opsworks/2013-02-18/
+-rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-05-02 01:01:05.000000 botocore-a-la-carte-opsworks-1.34.96/botocore/data/opsworks/2013-02-18/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 01:01:05.000000 botocore-a-la-carte-opsworks-1.34.96/botocore/data/opsworks/2013-02-18/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 01:01:05.000000 botocore-a-la-carte-opsworks-1.34.96/botocore/data/opsworks/2013-02-18/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   273984 2024-05-02 01:01:05.000000 botocore-a-la-carte-opsworks-1.34.96/botocore/data/opsworks/2013-02-18/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-02 01:01:05.000000 botocore-a-la-carte-opsworks-1.34.96/botocore/data/opsworks/2013-02-18/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:01:34.241051 botocore-a-la-carte-opsworks-1.34.96/botocore_a_la_carte_opsworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-02 01:01:34.000000 botocore-a-la-carte-opsworks-1.34.96/botocore_a_la_carte_opsworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-02 01:01:34.000000 botocore-a-la-carte-opsworks-1.34.96/botocore_a_la_carte_opsworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:01:34.000000 botocore-a-la-carte-opsworks-1.34.96/botocore_a_la_carte_opsworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 01:01:34.000000 botocore-a-la-carte-opsworks-1.34.96/botocore_a_la_carte_opsworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:01:34.245051 botocore-a-la-carte-opsworks-1.34.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-02 01:01:33.000000 botocore-a-la-carte-opsworks-1.34.96/setup.py
```

### Comparing `botocore-a-la-carte-opsworks-1.34.95/LICENSE.txt` & `botocore-a-la-carte-opsworks-1.34.96/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-opsworks-1.34.95/PKG-INFO` & `botocore-a-la-carte-opsworks-1.34.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-opsworks
-Version: 1.34.95
+Version: 1.34.96
 Summary: opsworks data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-opsworks-1.34.95/botocore/data/opsworks/2013-02-18/endpoint-rule-set-1.json` & `botocore-a-la-carte-opsworks-1.34.96/botocore/data/opsworks/2013-02-18/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-opsworks-1.34.95/botocore/data/opsworks/2013-02-18/service-2.json` & `botocore-a-la-carte-opsworks-1.34.96/botocore/data/opsworks/2013-02-18/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-opsworks-1.34.95/botocore/data/opsworks/2013-02-18/waiters-2.json` & `botocore-a-la-carte-opsworks-1.34.96/botocore/data/opsworks/2013-02-18/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-opsworks-1.34.95/botocore_a_la_carte_opsworks.egg-info/PKG-INFO` & `botocore-a-la-carte-opsworks-1.34.96/botocore_a_la_carte_opsworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-opsworks
-Version: 1.34.95
+Version: 1.34.96
 Summary: opsworks data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-opsworks-1.34.95/setup.py` & `botocore-a-la-carte-opsworks-1.34.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-opsworks',
-    version="1.34.95",
+    version="1.34.96",
     description='opsworks data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/opsworks/*/*.json'],
```

