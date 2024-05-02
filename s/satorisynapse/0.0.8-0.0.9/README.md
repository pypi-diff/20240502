# Comparing `tmp/satorisynapse-0.0.8.tar.gz` & `tmp/satorisynapse-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satorisynapse-0.0.8.tar", last modified: Thu Apr 18 21:40:39 2024, max compression
+gzip compressed data, was "satorisynapse-0.0.9.tar", last modified: Thu Apr 18 21:52:42 2024, max compression
```

## Comparing `satorisynapse-0.0.8.tar` & `satorisynapse-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:40:39.026631 satorisynapse-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 21:40:39.026631 satorisynapse-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:40:39.022631 satorisynapse-0.0.8/satorisynapse/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/satorisynapse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:40:39.026631 satorisynapse-0.0.8/satorisynapse/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/satorisynapse/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/satorisynapse/lib/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/satorisynapse/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/satorisynapse/lib/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/satorisynapse/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/satorisynapse/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:40:39.026631 satorisynapse-0.0.8/satorisynapse/synapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/satorisynapse/synapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/satorisynapse/synapse/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/satorisynapse/synapse/threaded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:40:39.022631 satorisynapse-0.0.8/satorisynapse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 21:40:38.000000 satorisynapse-0.0.8/satorisynapse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-18 21:40:38.000000 satorisynapse-0.0.8/satorisynapse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 21:40:38.000000 satorisynapse-0.0.8/satorisynapse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 21:40:38.000000 satorisynapse-0.0.8/satorisynapse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 21:40:38.000000 satorisynapse-0.0.8/satorisynapse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 21:40:39.026631 satorisynapse-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-18 21:40:31.000000 satorisynapse-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:42.318185 satorisynapse-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 21:52:42.314185 satorisynapse-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:42.314185 satorisynapse-0.0.9/satorisynapse/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:42.314185 satorisynapse-0.0.9/satorisynapse/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/lib/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/lib/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:42.314185 satorisynapse-0.0.9/satorisynapse/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/synapse/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/synapse/threaded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:42.314185 satorisynapse-0.0.9/satorisynapse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 21:52:42.000000 satorisynapse-0.0.9/satorisynapse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-18 21:52:42.000000 satorisynapse-0.0.9/satorisynapse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 21:52:42.000000 satorisynapse-0.0.9/satorisynapse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 21:52:42.000000 satorisynapse-0.0.9/satorisynapse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 21:52:42.000000 satorisynapse-0.0.9/satorisynapse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 21:52:42.318185 satorisynapse-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/setup.py
```

### Comparing `satorisynapse-0.0.8/LICENSE` & `satorisynapse-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.8/PKG-INFO` & `satorisynapse-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.8
+Version: 0.0.9
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.0.8/satorisynapse/lib/domain.py` & `satorisynapse-0.0.9/satorisynapse/lib/domain.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.8/satorisynapse/lib/requests.py` & `satorisynapse-0.0.9/satorisynapse/lib/requests.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.8/satorisynapse/synapse/asynchronous.py` & `satorisynapse-0.0.9/satorisynapse/synapse/asynchronous.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.8/satorisynapse/synapse/threaded.py` & `satorisynapse-0.0.9/satorisynapse/synapse/threaded.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.8/satorisynapse.egg-info/PKG-INFO` & `satorisynapse-0.0.9/satorisynapse.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.8
+Version: 0.0.9
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.0.8/setup.py` & `satorisynapse-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def get_name():
     return 'satorisynapse'
 
 
 def get_version():
-    return '0.0.8'
+    return '0.0.9'
 
 
 def get_requirements():
     requirements = get_here('requirements.txt')
     if os.path.isfile(requirements):
         with open(requirements, 'r') as f:
             return f.read().splitlines()
```

