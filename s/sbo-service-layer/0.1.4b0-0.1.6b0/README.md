# Comparing `tmp/sbo_service_layer-0.1.4b0.tar.gz` & `tmp/sbo_service_layer-0.1.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbo_service_layer-0.1.4b0.tar", last modified: Thu May  2 15:12:01 2024, max compression
+gzip compressed data, was "sbo_service_layer-0.1.6b0.tar", last modified: Thu May  2 15:59:49 2024, max compression
```

## Comparing `sbo_service_layer-0.1.4b0.tar` & `sbo_service_layer-0.1.6b0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:12:01.813276 sbo_service_layer-0.1.4b0/
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)       49 2023-05-03 20:35:42.000000 sbo_service_layer-0.1.4b0/MANIFEST.in
--rw-r--r--   0 jaydm     (1000) jaydm     (1000)      664 2024-05-02 15:12:01.813276 sbo_service_layer-0.1.4b0/PKG-INFO
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)      236 2024-05-02 15:08:01.000000 sbo_service_layer-0.1.4b0/README.md
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)      157 2023-05-03 20:35:42.000000 sbo_service_layer-0.1.4b0/pyproject.toml
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)      619 2024-05-02 15:12:01.813276 sbo_service_layer-0.1.4b0/setup.cfg
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)       69 2023-05-03 20:39:40.000000 sbo_service_layer-0.1.4b0/setup.py
-drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:12:01.809276 sbo_service_layer-0.1.4b0/src/
-drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:12:01.809276 sbo_service_layer-0.1.4b0/src/sbo_service/
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)        0 2023-05-03 20:35:42.000000 sbo_service_layer-0.1.4b0/src/sbo_service/__init__.py
-drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:12:01.809276 sbo_service_layer-0.1.4b0/src/sbo_service/__pycache__/
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)      153 2023-07-18 19:35:18.000000 sbo_service_layer-0.1.4b0/src/sbo_service/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)    18565 2023-10-18 01:46:37.000000 sbo_service_layer-0.1.4b0/src/sbo_service/__pycache__/service.cpython-310.pyc
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)    29543 2023-10-18 01:46:36.000000 sbo_service_layer-0.1.4b0/src/sbo_service/service.py
-drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:12:01.813276 sbo_service_layer-0.1.4b0/src/sbo_service_layer.egg-info/
--rw-r--r--   0 jaydm     (1000) jaydm     (1000)      664 2024-05-02 15:12:01.000000 sbo_service_layer-0.1.4b0/src/sbo_service_layer.egg-info/PKG-INFO
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)      553 2024-05-02 15:12:01.000000 sbo_service_layer-0.1.4b0/src/sbo_service_layer.egg-info/SOURCES.txt
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)        1 2024-05-02 15:12:01.000000 sbo_service_layer-0.1.4b0/src/sbo_service_layer.egg-info/dependency_links.txt
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)       46 2024-05-02 15:12:01.000000 sbo_service_layer-0.1.4b0/src/sbo_service_layer.egg-info/requires.txt
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)       12 2024-05-02 15:12:01.000000 sbo_service_layer-0.1.4b0/src/sbo_service_layer.egg-info/top_level.txt
-drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:12:01.813276 sbo_service_layer-0.1.4b0/tests/
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)     1909 2023-07-26 17:00:41.000000 sbo_service_layer-0.1.4b0/tests/test_00_connect.py
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)     2504 2023-07-26 17:08:37.000000 sbo_service_layer-0.1.4b0/tests/test_10_create_entity.py
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)     2015 2023-07-26 17:09:34.000000 sbo_service_layer-0.1.4b0/tests/test_20_update_entity.py
--rw-rw-r--   0 jaydm     (1000) jaydm     (1000)     3299 2023-07-26 17:11:00.000000 sbo_service_layer-0.1.4b0/tests/test_30_documents.py
+drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:59:49.757839 sbo_service_layer-0.1.6b0/
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)       49 2023-05-03 20:35:42.000000 sbo_service_layer-0.1.6b0/MANIFEST.in
+-rw-r--r--   0 jaydm     (1000) jaydm     (1000)      601 2024-05-02 15:59:49.757839 sbo_service_layer-0.1.6b0/PKG-INFO
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)      236 2024-05-02 15:08:01.000000 sbo_service_layer-0.1.6b0/README.md
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)      252 2024-05-02 15:52:51.000000 sbo_service_layer-0.1.6b0/pyproject.toml
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)      554 2024-05-02 15:59:49.757839 sbo_service_layer-0.1.6b0/setup.cfg
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)       69 2023-05-03 20:39:40.000000 sbo_service_layer-0.1.6b0/setup.py
+drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:59:49.749838 sbo_service_layer-0.1.6b0/src/
+drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:59:49.753838 sbo_service_layer-0.1.6b0/src/sbo_service/
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)        0 2023-05-03 20:35:42.000000 sbo_service_layer-0.1.6b0/src/sbo_service/__init__.py
+drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:59:49.753838 sbo_service_layer-0.1.6b0/src/sbo_service/__pycache__/
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)      153 2023-07-18 19:35:18.000000 sbo_service_layer-0.1.6b0/src/sbo_service/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)    18565 2023-10-18 01:46:37.000000 sbo_service_layer-0.1.6b0/src/sbo_service/__pycache__/service.cpython-310.pyc
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)    29543 2023-10-18 01:46:36.000000 sbo_service_layer-0.1.6b0/src/sbo_service/service.py
+drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:59:49.757839 sbo_service_layer-0.1.6b0/src/sbo_service_layer.egg-info/
+-rw-r--r--   0 jaydm     (1000) jaydm     (1000)      601 2024-05-02 15:59:49.000000 sbo_service_layer-0.1.6b0/src/sbo_service_layer.egg-info/PKG-INFO
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)      553 2024-05-02 15:59:49.000000 sbo_service_layer-0.1.6b0/src/sbo_service_layer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)        1 2024-05-02 15:59:49.000000 sbo_service_layer-0.1.6b0/src/sbo_service_layer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)       46 2024-05-02 15:59:49.000000 sbo_service_layer-0.1.6b0/src/sbo_service_layer.egg-info/requires.txt
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)       12 2024-05-02 15:59:49.000000 sbo_service_layer-0.1.6b0/src/sbo_service_layer.egg-info/top_level.txt
+drwxrwxr-x   0 jaydm     (1000) jaydm     (1000)        0 2024-05-02 15:59:49.757839 sbo_service_layer-0.1.6b0/tests/
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)     1909 2023-07-26 17:00:41.000000 sbo_service_layer-0.1.6b0/tests/test_00_connect.py
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)     2504 2023-07-26 17:08:37.000000 sbo_service_layer-0.1.6b0/tests/test_10_create_entity.py
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)     2015 2023-07-26 17:09:34.000000 sbo_service_layer-0.1.6b0/tests/test_20_update_entity.py
+-rw-rw-r--   0 jaydm     (1000) jaydm     (1000)     3299 2023-07-26 17:11:00.000000 sbo_service_layer-0.1.6b0/tests/test_30_documents.py
```

### Comparing `sbo_service_layer-0.1.4b0/src/sbo_service/__pycache__/service.cpython-310.pyc` & `sbo_service_layer-0.1.6b0/src/sbo_service/__pycache__/service.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `sbo_service_layer-0.1.4b0/src/sbo_service/service.py` & `sbo_service_layer-0.1.6b0/src/sbo_service/service.py`

 * *Files identical despite different names*

### Comparing `sbo_service_layer-0.1.4b0/src/sbo_service_layer.egg-info/SOURCES.txt` & `sbo_service_layer-0.1.6b0/src/sbo_service_layer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sbo_service_layer-0.1.4b0/tests/test_00_connect.py` & `sbo_service_layer-0.1.6b0/tests/test_00_connect.py`

 * *Files identical despite different names*

### Comparing `sbo_service_layer-0.1.4b0/tests/test_10_create_entity.py` & `sbo_service_layer-0.1.6b0/tests/test_10_create_entity.py`

 * *Files identical despite different names*

### Comparing `sbo_service_layer-0.1.4b0/tests/test_20_update_entity.py` & `sbo_service_layer-0.1.6b0/tests/test_20_update_entity.py`

 * *Files identical despite different names*

### Comparing `sbo_service_layer-0.1.4b0/tests/test_30_documents.py` & `sbo_service_layer-0.1.6b0/tests/test_30_documents.py`

 * *Files identical despite different names*

