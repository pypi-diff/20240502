# Comparing `tmp/waylay_sdk_storage-0.4.2.20240430.tar.gz` & `tmp/waylay_sdk_storage-0.4.2b20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_storage-0.4.2.20240430.tar", last modified: Thu May  2 07:57:47 2024, max compression
+gzip compressed data, was "waylay_sdk_storage-0.4.2b20240423.tar", last modified: Wed Apr 24 07:48:37 2024, max compression
```

## Comparing `waylay_sdk_storage-0.4.2.20240430.tar` & `waylay_sdk_storage-0.4.2b20240423.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.617842 waylay_sdk_storage-0.4.2.20240430/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-02 07:57:47.617842 waylay_sdk_storage-0.4.2.20240430/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 07:57:47.617842 waylay_sdk_storage-0.4.2.20240430/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.609841 waylay_sdk_storage-0.4.2.20240430/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.609841 waylay_sdk_storage-0.4.2.20240430/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.609841 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.609841 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.613842 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/api/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/api/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/api/bucket_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27934 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/api/object_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    44677 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/api/subscription_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.613842 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/service/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-02 07:57:43.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.613842 waylay_sdk_storage-0.4.2.20240430/src/waylay_sdk_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-02 07:57:47.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay_sdk_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-02 07:57:47.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay_sdk_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:57:47.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay_sdk_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-02 07:57:47.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay_sdk_storage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-02 07:57:47.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay_sdk_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 07:57:47.000000 waylay_sdk_storage-0.4.2.20240430/src/waylay_sdk_storage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:37.584814 waylay_sdk_storage-0.4.2b20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-24 07:48:37.584814 waylay_sdk_storage-0.4.2b20240423/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:48:37.584814 waylay_sdk_storage-0.4.2b20240423/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:37.580814 waylay_sdk_storage-0.4.2b20240423/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:37.580814 waylay_sdk_storage-0.4.2b20240423/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:37.580814 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:37.580814 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:37.584814 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/api/about_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/api/bucket_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27934 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/api/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    44677 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/api/subscription_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:37.584814 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 07:48:33.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:37.584814 waylay_sdk_storage-0.4.2b20240423/src/waylay_sdk_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-24 07:48:37.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay_sdk_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-24 07:48:37.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay_sdk_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:48:37.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay_sdk_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 07:48:37.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay_sdk_storage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-24 07:48:37.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay_sdk_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 07:48:37.000000 waylay_sdk_storage-0.4.2b20240423/src/waylay_sdk_storage.egg-info/top_level.txt
```

### Comparing `waylay_sdk_storage-0.4.2.20240430/LICENSE.txt` & `waylay_sdk_storage-0.4.2b20240423/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.2.20240430/PKG-INFO` & `waylay_sdk_storage-0.4.2b20240423/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage
-Version: 0.4.2.20240430
+Version: 0.4.2b20240423
 Summary: Waylay Storage
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice
```

### Comparing `waylay_sdk_storage-0.4.2.20240430/README.md` & `waylay_sdk_storage-0.4.2b20240423/README.md`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.2.20240430/pyproject.toml` & `waylay_sdk_storage-0.4.2b20240423/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-storage"
-version = "0.4.2.20240430"
+version = "0.4.2b20240423"
 description = "Waylay Storage"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Storage"]
 requires-python = ">= 3.9"
 dependencies = [
```

### Comparing `waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/api/about_api.py` & `waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/api/about_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/api/bucket_api.py` & `waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/api/bucket_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/api/object_api.py` & `waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/api/object_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/api/subscription_api.py` & `waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/api/subscription_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.2.20240430/src/waylay/services/storage/service/service.py` & `waylay_sdk_storage-0.4.2b20240423/src/waylay/services/storage/service/service.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.2.20240430/src/waylay_sdk_storage.egg-info/PKG-INFO` & `waylay_sdk_storage-0.4.2b20240423/src/waylay_sdk_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage
-Version: 0.4.2.20240430
+Version: 0.4.2b20240423
 Summary: Waylay Storage
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice
```

### Comparing `waylay_sdk_storage-0.4.2.20240430/src/waylay_sdk_storage.egg-info/SOURCES.txt` & `waylay_sdk_storage-0.4.2b20240423/src/waylay_sdk_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

