# Comparing `tmp/waylay_sdk-2024.4.23.tar.gz` & `tmp/waylay_sdk-2024.4.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk-2024.4.23.tar", last modified: Thu Apr 25 12:52:44 2024, max compression
+gzip compressed data, was "waylay_sdk-2024.4.30.tar", last modified: Thu May  2 08:02:20 2024, max compression
```

## Comparing `waylay_sdk-2024.4.23.tar` & `waylay_sdk-2024.4.30.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-25 12:52:44.069711 waylay_sdk-2024.4.23/
--rw-r--r--   0 thomas     (502) staff       (20)      746 2024-04-25 12:51:46.000000 waylay_sdk-2024.4.23/LICENCE.txt
--rw-r--r--   0 thomas     (502) staff       (20)     8664 2024-04-25 12:52:44.069224 waylay_sdk-2024.4.23/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)     6769 2024-04-09 11:13:26.000000 waylay_sdk-2024.4.23/README.md
--rw-r--r--   0 thomas     (502) staff       (20)     1606 2024-04-25 12:49:55.000000 waylay_sdk-2024.4.23/pyproject.toml
--rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-25 12:52:44.069757 waylay_sdk-2024.4.23/setup.cfg
-drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-25 12:52:44.068390 waylay_sdk-2024.4.23/waylay_sdk.egg-info/
--rw-r--r--   0 thomas     (502) staff       (20)     8664 2024-04-25 12:52:44.000000 waylay_sdk-2024.4.23/waylay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (502) staff       (20)      205 2024-04-25 12:52:44.000000 waylay_sdk-2024.4.23/waylay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-25 12:52:44.000000 waylay_sdk-2024.4.23/waylay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (502) staff       (20)      833 2024-04-25 12:52:44.000000 waylay_sdk-2024.4.23/waylay_sdk.egg-info/requires.txt
--rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-25 12:52:44.000000 waylay_sdk-2024.4.23/waylay_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-05-02 08:02:20.702692 waylay_sdk-2024.4.30/
+-rw-r--r--   0 thomas     (502) staff       (20)      746 2024-04-25 12:51:46.000000 waylay_sdk-2024.4.30/LICENCE.txt
+-rw-r--r--   0 thomas     (502) staff       (20)     8664 2024-05-02 08:02:20.702220 waylay_sdk-2024.4.30/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)     6769 2024-04-09 11:13:26.000000 waylay_sdk-2024.4.30/README.md
+-rw-r--r--   0 thomas     (502) staff       (20)     1606 2024-05-02 07:58:07.000000 waylay_sdk-2024.4.30/pyproject.toml
+-rw-r--r--   0 thomas     (502) staff       (20)       38 2024-05-02 08:02:20.702750 waylay_sdk-2024.4.30/setup.cfg
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-05-02 08:02:20.700979 waylay_sdk-2024.4.30/waylay_sdk.egg-info/
+-rw-r--r--   0 thomas     (502) staff       (20)     8664 2024-05-02 08:02:20.000000 waylay_sdk-2024.4.30/waylay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)      205 2024-05-02 08:02:20.000000 waylay_sdk-2024.4.30/waylay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-05-02 08:02:20.000000 waylay_sdk-2024.4.30/waylay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (502) staff       (20)      833 2024-05-02 08:02:20.000000 waylay_sdk-2024.4.30/waylay_sdk.egg-info/requires.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-05-02 08:02:20.000000 waylay_sdk-2024.4.30/waylay_sdk.egg-info/top_level.txt
```

### Comparing `waylay_sdk-2024.4.23/LICENCE.txt` & `waylay_sdk-2024.4.30/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk-2024.4.23/PKG-INFO` & `waylay_sdk-2024.4.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: waylay-sdk
-Version: 2024.4.23
+Version: 2024.4.30
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 Project-URL: Homepage, https://www.waylay.io/
 Project-URL: Documentation, https://docs.waylay.io/#/api/sdk/python
 Project-URL: Repository, https://github.com/waylayio/waylay-py-services.git
 Keywords: waylay,sdk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: waylay-sdk-core~=0.2.1
 Requires-Dist: waylay-sdk-alarms>=1.11.0.20240423
 Requires-Dist: waylay-sdk-data>=2.14.0.20240423
-Requires-Dist: waylay-sdk-registry>=2.12.4.20240423
+Requires-Dist: waylay-sdk-registry>=2.12.4.20240430
 Requires-Dist: waylay-sdk-resources>=8.1.0.20240423
 Requires-Dist: waylay-sdk-rules>=6.5.0.20240423
-Requires-Dist: waylay-sdk-storage>=0.4.1.20240423
+Requires-Dist: waylay-sdk-storage>=0.4.1.20240430
 Provides-Extra: types-alarms
 Requires-Dist: waylay-sdk-alarms-types>=1.11.0.20240423; extra == "types-alarms"
 Provides-Extra: types-data
 Requires-Dist: waylay-sdk-data-types>=2.14.0.20240423; extra == "types-data"
 Provides-Extra: types-registry
-Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240423; extra == "types-registry"
+Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240430; extra == "types-registry"
 Provides-Extra: types-resources
 Requires-Dist: waylay-sdk-resources-types>=8.1.0.20240423; extra == "types-resources"
 Provides-Extra: types-rules
 Requires-Dist: waylay-sdk-rules-types>=6.5.0.20240423; extra == "types-rules"
 Provides-Extra: types-storage
-Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240423; extra == "types-storage"
+Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240430; extra == "types-storage"
 Provides-Extra: types
 Requires-Dist: waylay-sdk-alarms-types>=1.11.0.20240423; extra == "types"
 Requires-Dist: waylay-sdk-data-types>=2.14.0.20240423; extra == "types"
-Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240423; extra == "types"
+Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240430; extra == "types"
 Requires-Dist: waylay-sdk-resources-types>=8.1.0.20240423; extra == "types"
 Requires-Dist: waylay-sdk-rules-types>=6.5.0.20240423; extra == "types"
-Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240423; extra == "types"
+Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240430; extra == "types"
 
 # Waylay Python SDK
 
 Python SDK for the Waylay Platform.
 
 This `waylay-sdk` package is the main entrypoint to install the python SDK client for the [Waylay REST apis](https://docs.waylay.io/#/api/?id=openapi-docs).
```

### Comparing `waylay_sdk-2024.4.23/README.md` & `waylay_sdk-2024.4.30/README.md`

 * *Files identical despite different names*

### Comparing `waylay_sdk-2024.4.23/pyproject.toml` & `waylay_sdk-2024.4.30/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 readme = "README.md"
 authors = [{name = "Waylay", email = "info@waylay.io"}]
 license={file = "LICENSE.txt"}
 dependencies = [
     "waylay-sdk-core~=0.2.1",
     "waylay-sdk-alarms>=1.11.0.20240423",
     "waylay-sdk-data>=2.14.0.20240423",
-    "waylay-sdk-registry>=2.12.4.20240423",
+    "waylay-sdk-registry>=2.12.4.20240430",
     "waylay-sdk-resources>=8.1.0.20240423",
     "waylay-sdk-rules>=6.5.0.20240423",
-    "waylay-sdk-storage>=0.4.1.20240423",
+    "waylay-sdk-storage>=0.4.1.20240430",
 ]
 [project.optional-dependencies]
 types-alarms = [ "waylay-sdk-alarms-types>=1.11.0.20240423" ]
 types-data = [ "waylay-sdk-data-types>=2.14.0.20240423" ]
-types-registry = [ "waylay-sdk-registry-types>=2.12.4.20240423" ]
+types-registry = [ "waylay-sdk-registry-types>=2.12.4.20240430" ]
 types-resources = [ "waylay-sdk-resources-types>=8.1.0.20240423" ]
 types-rules = [ "waylay-sdk-rules-types>=6.5.0.20240423" ]
-types-storage = [ "waylay-sdk-storage-types>=0.4.1.20240423" ]
+types-storage = [ "waylay-sdk-storage-types>=0.4.1.20240430" ]
 types = [
     "waylay-sdk-alarms-types>=1.11.0.20240423",
     "waylay-sdk-data-types>=2.14.0.20240423",
-    "waylay-sdk-registry-types>=2.12.4.20240423",
+    "waylay-sdk-registry-types>=2.12.4.20240430",
     "waylay-sdk-resources-types>=8.1.0.20240423",
     "waylay-sdk-rules-types>=6.5.0.20240423",
-    "waylay-sdk-storage-types>=0.4.1.20240423",
+    "waylay-sdk-storage-types>=0.4.1.20240430",
 ]
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
 Documentation = "https://docs.waylay.io/#/api/sdk/python"
 Repository = "https://github.com/waylayio/waylay-py-services.git"
```

### Comparing `waylay_sdk-2024.4.23/waylay_sdk.egg-info/PKG-INFO` & `waylay_sdk-2024.4.30/waylay_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: waylay-sdk
-Version: 2024.4.23
+Version: 2024.4.30
 Summary: Waylay Python SDK.
 Author-email: Waylay <info@waylay.io>
 Project-URL: Homepage, https://www.waylay.io/
 Project-URL: Documentation, https://docs.waylay.io/#/api/sdk/python
 Project-URL: Repository, https://github.com/waylayio/waylay-py-services.git
 Keywords: waylay,sdk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: waylay-sdk-core~=0.2.1
 Requires-Dist: waylay-sdk-alarms>=1.11.0.20240423
 Requires-Dist: waylay-sdk-data>=2.14.0.20240423
-Requires-Dist: waylay-sdk-registry>=2.12.4.20240423
+Requires-Dist: waylay-sdk-registry>=2.12.4.20240430
 Requires-Dist: waylay-sdk-resources>=8.1.0.20240423
 Requires-Dist: waylay-sdk-rules>=6.5.0.20240423
-Requires-Dist: waylay-sdk-storage>=0.4.1.20240423
+Requires-Dist: waylay-sdk-storage>=0.4.1.20240430
 Provides-Extra: types-alarms
 Requires-Dist: waylay-sdk-alarms-types>=1.11.0.20240423; extra == "types-alarms"
 Provides-Extra: types-data
 Requires-Dist: waylay-sdk-data-types>=2.14.0.20240423; extra == "types-data"
 Provides-Extra: types-registry
-Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240423; extra == "types-registry"
+Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240430; extra == "types-registry"
 Provides-Extra: types-resources
 Requires-Dist: waylay-sdk-resources-types>=8.1.0.20240423; extra == "types-resources"
 Provides-Extra: types-rules
 Requires-Dist: waylay-sdk-rules-types>=6.5.0.20240423; extra == "types-rules"
 Provides-Extra: types-storage
-Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240423; extra == "types-storage"
+Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240430; extra == "types-storage"
 Provides-Extra: types
 Requires-Dist: waylay-sdk-alarms-types>=1.11.0.20240423; extra == "types"
 Requires-Dist: waylay-sdk-data-types>=2.14.0.20240423; extra == "types"
-Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240423; extra == "types"
+Requires-Dist: waylay-sdk-registry-types>=2.12.4.20240430; extra == "types"
 Requires-Dist: waylay-sdk-resources-types>=8.1.0.20240423; extra == "types"
 Requires-Dist: waylay-sdk-rules-types>=6.5.0.20240423; extra == "types"
-Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240423; extra == "types"
+Requires-Dist: waylay-sdk-storage-types>=0.4.1.20240430; extra == "types"
 
 # Waylay Python SDK
 
 Python SDK for the Waylay Platform.
 
 This `waylay-sdk` package is the main entrypoint to install the python SDK client for the [Waylay REST apis](https://docs.waylay.io/#/api/?id=openapi-docs).
```

### Comparing `waylay_sdk-2024.4.23/waylay_sdk.egg-info/requires.txt` & `waylay_sdk-2024.4.30/waylay_sdk.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 waylay-sdk-core~=0.2.1
 waylay-sdk-alarms>=1.11.0.20240423
 waylay-sdk-data>=2.14.0.20240423
-waylay-sdk-registry>=2.12.4.20240423
+waylay-sdk-registry>=2.12.4.20240430
 waylay-sdk-resources>=8.1.0.20240423
 waylay-sdk-rules>=6.5.0.20240423
-waylay-sdk-storage>=0.4.1.20240423
+waylay-sdk-storage>=0.4.1.20240430
 
 [types]
 waylay-sdk-alarms-types>=1.11.0.20240423
 waylay-sdk-data-types>=2.14.0.20240423
-waylay-sdk-registry-types>=2.12.4.20240423
+waylay-sdk-registry-types>=2.12.4.20240430
 waylay-sdk-resources-types>=8.1.0.20240423
 waylay-sdk-rules-types>=6.5.0.20240423
-waylay-sdk-storage-types>=0.4.1.20240423
+waylay-sdk-storage-types>=0.4.1.20240430
 
 [types-alarms]
 waylay-sdk-alarms-types>=1.11.0.20240423
 
 [types-data]
 waylay-sdk-data-types>=2.14.0.20240423
 
 [types-registry]
-waylay-sdk-registry-types>=2.12.4.20240423
+waylay-sdk-registry-types>=2.12.4.20240430
 
 [types-resources]
 waylay-sdk-resources-types>=8.1.0.20240423
 
 [types-rules]
 waylay-sdk-rules-types>=6.5.0.20240423
 
 [types-storage]
-waylay-sdk-storage-types>=0.4.1.20240423
+waylay-sdk-storage-types>=0.4.1.20240430
```

