# Comparing `tmp/galaxy-objectstore-24.0.0.tar.gz` & `tmp/galaxy_objectstore-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-objectstore-24.0.0.tar", last modified: Wed Apr  3 02:44:43 2024, max compression
+gzip compressed data, was "galaxy_objectstore-24.0.1.tar", last modified: Thu May  2 13:47:48 2024, max compression
```

## Comparing `galaxy-objectstore-24.0.0.tar` & `galaxy_objectstore-24.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:43.902832 galaxy-objectstore-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-03 02:44:43.902832 galaxy-objectstore-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:43.898832 galaxy-objectstore-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:43.898832 galaxy-objectstore-24.0.0/galaxy/objectstore/
--rw-r--r--   0 runner    (1001) docker     (127)    66165 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23700 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/azure_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/badges.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    29441 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    32881 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/irods.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/pithos.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/pulsar.py
--rw-r--r--   0 runner    (1001) docker     (127)    30757 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/s3_multipart_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:43.898832 galaxy-objectstore-24.0.0/galaxy/objectstore/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:43.902832 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-03 02:44:43.000000 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-03 02:44:43.000000 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:44:43.000000 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 02:44:43.000000 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:44:43.000000 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-03 02:44:43.902832 galaxy-objectstore-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:48.829575 galaxy_objectstore-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-05-02 13:47:48.829575 galaxy_objectstore-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:48.825575 galaxy_objectstore-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:48.829575 galaxy_objectstore-24.0.1/galaxy/objectstore/
+-rw-r--r--   0 runner    (1001) docker     (127)    66165 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/objectstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23700 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/objectstore/azure_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/objectstore/badges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/objectstore/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29441 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/objectstore/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32881 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/objectstore/irods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/objectstore/pithos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/objectstore/pulsar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30757 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/objectstore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/objectstore/s3_multipart_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:48.829575 galaxy_objectstore-24.0.1/galaxy/objectstore/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/objectstore/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:48.829575 galaxy_objectstore-24.0.1/galaxy_objectstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-05-02 13:47:48.000000 galaxy_objectstore-24.0.1/galaxy_objectstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-02 13:47:48.000000 galaxy_objectstore-24.0.1/galaxy_objectstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:47:48.000000 galaxy_objectstore-24.0.1/galaxy_objectstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 13:47:48.000000 galaxy_objectstore-24.0.1/galaxy_objectstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:47:48.000000 galaxy_objectstore-24.0.1/galaxy_objectstore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-02 13:47:48.829575 galaxy_objectstore-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_objectstore-24.0.1/test-requirements.txt
```

### Comparing `galaxy-objectstore-24.0.0/HISTORY.rst` & `galaxy_objectstore-24.0.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-objectstore-24.0.0/LICENSE` & `galaxy_objectstore-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/PKG-INFO` & `galaxy_objectstore-24.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-objectstore
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy objectstore framework and plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,14 +46,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-objectstore-24.0.0/galaxy/objectstore/__init__.py` & `galaxy_objectstore-24.0.1/galaxy/objectstore/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/galaxy/objectstore/azure_blob.py` & `galaxy_objectstore-24.0.1/galaxy/objectstore/azure_blob.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/galaxy/objectstore/badges.py` & `galaxy_objectstore-24.0.1/galaxy/objectstore/badges.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/galaxy/objectstore/caching.py` & `galaxy_objectstore-24.0.1/galaxy/objectstore/caching.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/galaxy/objectstore/cloud.py` & `galaxy_objectstore-24.0.1/galaxy/objectstore/cloud.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/galaxy/objectstore/irods.py` & `galaxy_objectstore-24.0.1/galaxy/objectstore/irods.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/galaxy/objectstore/pithos.py` & `galaxy_objectstore-24.0.1/galaxy/objectstore/pithos.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/galaxy/objectstore/pulsar.py` & `galaxy_objectstore-24.0.1/galaxy/objectstore/pulsar.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/galaxy/objectstore/s3.py` & `galaxy_objectstore-24.0.1/galaxy/objectstore/s3.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/galaxy/objectstore/s3_multipart_upload.py` & `galaxy_objectstore-24.0.1/galaxy/objectstore/s3_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/galaxy/objectstore/unittest_utils/__init__.py` & `galaxy_objectstore-24.0.1/galaxy/objectstore/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/PKG-INFO` & `galaxy_objectstore-24.0.1/galaxy_objectstore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-objectstore
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy objectstore framework and plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,14 +46,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/SOURCES.txt` & `galaxy_objectstore-24.0.1/galaxy_objectstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-24.0.0/setup.cfg` & `galaxy_objectstore-24.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-objectstore
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	pydantic>=2,!=2.6.0,!=2.6.1
 	PyYAML
```

