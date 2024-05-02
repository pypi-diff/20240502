# Comparing `tmp/spand-0.1.0.tar.gz` & `tmp/spand-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spand-0.1.0.tar", max compression
+gzip compressed data, was "spand-0.1.1.tar", max compression
```

## Comparing `spand-0.1.0.tar` & `spand-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-04-05 14:25:44.496174 spand-0.1.0/LICENSE
--rw-r--r--   0        0        0       15 2024-04-05 14:25:44.496174 spand-0.1.0/README.md
--rw-r--r--   0        0        0      201 2024-04-05 14:25:44.496174 spand-0.1.0/bucket_utils/__init__.py
--rw-r--r--   0        0        0      224 2024-04-05 14:25:44.500174 spand-0.1.0/bucket_utils/exceptions.py
--rw-r--r--   0        0        0    10147 2024-04-05 14:25:44.500174 spand-0.1.0/bucket_utils/google.py
--rw-r--r--   0        0        0     3493 2024-04-05 14:25:44.500174 spand-0.1.0/bucket_utils/interface.py
--rw-r--r--   0        0        0     6388 2024-04-05 14:25:44.500174 spand-0.1.0/bucket_utils/local.py
--rw-r--r--   0        0        0      383 2024-04-05 14:25:44.500174 spand-0.1.0/bucket_utils/resumable_upload_session.py
--rw-r--r--   0        0        0      482 2024-04-05 14:25:44.500174 spand-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 spand-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-02 06:47:16.175940 spand-0.1.1/LICENSE
+-rw-r--r--   0        0        0       15 2024-05-02 06:47:16.175940 spand-0.1.1/README.md
+-rw-r--r--   0        0        0      178 2024-05-02 06:47:16.175940 spand-0.1.1/bucket_utils/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-02 06:47:16.175940 spand-0.1.1/bucket_utils/exceptions.py
+-rw-r--r--   0        0        0    10147 2024-05-02 06:47:16.175940 spand-0.1.1/bucket_utils/google.py
+-rw-r--r--   0        0        0     3493 2024-05-02 06:47:16.175940 spand-0.1.1/bucket_utils/interface.py
+-rw-r--r--   0        0        0     6388 2024-05-02 06:47:16.175940 spand-0.1.1/bucket_utils/local.py
+-rw-r--r--   0        0        0      383 2024-05-02 06:47:16.175940 spand-0.1.1/bucket_utils/resumable_upload_session.py
+-rw-r--r--   0        0        0      482 2024-05-02 06:47:16.175940 spand-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 spand-0.1.1/PKG-INFO
```

### Comparing `spand-0.1.0/LICENSE` & `spand-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spand-0.1.0/bucket_utils/google.py` & `spand-0.1.1/bucket_utils/google.py`

 * *Files identical despite different names*

### Comparing `spand-0.1.0/bucket_utils/interface.py` & `spand-0.1.1/bucket_utils/interface.py`

 * *Files identical despite different names*

### Comparing `spand-0.1.0/bucket_utils/local.py` & `spand-0.1.1/bucket_utils/local.py`

 * *Files identical despite different names*

### Comparing `spand-0.1.0/PKG-INFO` & `spand-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spand
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utility classes for interacting with cloud buckets
 Author: Magnus Hansen
 Author-email: maha@mapspeople.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

