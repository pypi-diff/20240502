# Comparing `tmp/confidential-2.6.0.tar.gz` & `tmp/confidential-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confidential-2.6.0.tar", max compression
+gzip compressed data, was "confidential-2.6.1.tar", max compression
```

## Comparing `confidential-2.6.0.tar` & `confidential-2.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-03-15 15:21:34.874207 confidential-2.6.0/LICENSE
--rw-r--r--   0        0        0      108 2023-03-15 15:21:34.878207 confidential-2.6.0/confidential/__init__.py
--rw-r--r--   0        0        0       47 2023-03-15 15:21:34.878207 confidential-2.6.0/confidential/exceptions.py
--rw-r--r--   0        0        0     1491 2023-03-15 15:21:34.878207 confidential-2.6.0/confidential/parameter_store_decrypter.py
--rw-r--r--   0        0        0     4485 2023-03-15 15:21:34.878207 confidential-2.6.0/confidential/secrets_manager.py
--rw-r--r--   0        0        0     1502 2023-03-15 15:21:34.878207 confidential-2.6.0/confidential/secrets_manager_decrypter.py
--rw-r--r--   0        0        0      514 2023-03-15 15:21:34.878207 confidential-2.6.0/confidential/utils.py
--rw-r--r--   0        0        0     1074 2023-03-15 15:21:34.878207 confidential-2.6.0/pyproject.toml
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 confidential-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-02 16:59:49.942250 confidential-2.6.1/LICENSE
+-rw-r--r--   0        0        0      108 2024-05-02 16:59:49.942250 confidential-2.6.1/confidential/__init__.py
+-rw-r--r--   0        0        0       47 2024-05-02 16:59:49.942250 confidential-2.6.1/confidential/exceptions.py
+-rw-r--r--   0        0        0     1491 2024-05-02 16:59:49.942250 confidential-2.6.1/confidential/parameter_store_decrypter.py
+-rw-r--r--   0        0        0     4485 2024-05-02 16:59:49.942250 confidential-2.6.1/confidential/secrets_manager.py
+-rw-r--r--   0        0        0     1502 2024-05-02 16:59:49.946250 confidential-2.6.1/confidential/secrets_manager_decrypter.py
+-rw-r--r--   0        0        0      514 2024-05-02 16:59:49.946250 confidential-2.6.1/confidential/utils.py
+-rw-r--r--   0        0        0     1082 2024-05-02 16:59:49.946250 confidential-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 confidential-2.6.1/PKG-INFO
```

### Comparing `confidential-2.6.0/LICENSE` & `confidential-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `confidential-2.6.0/confidential/parameter_store_decrypter.py` & `confidential-2.6.1/confidential/parameter_store_decrypter.py`

 * *Files identical despite different names*

### Comparing `confidential-2.6.0/confidential/secrets_manager.py` & `confidential-2.6.1/confidential/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `confidential-2.6.0/confidential/secrets_manager_decrypter.py` & `confidential-2.6.1/confidential/secrets_manager_decrypter.py`

 * *Files identical despite different names*

### Comparing `confidential-2.6.0/confidential/utils.py` & `confidential-2.6.1/confidential/utils.py`

 * *Files identical despite different names*

### Comparing `confidential-2.6.0/pyproject.toml` & `confidential-2.6.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "confidential"
-version = "2.6.0"
+version = "2.6.1"
 description = "Manage secrets in your projects using AWS Secrets Manager"
 authors = [
     "Daniel van Flymen <dvf@candidco.com>",
     "Elliott Chartock <elliott.chartock@candidco.com>",
     "Vageli Mouzakitis <vageli.mouzakitis@candidco.com>",
     "Diaphel Thompson <diaphel@candidco.com>",
     "Tacio Rocha <tacio.rocha@candidco.com>"
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = ">=3.7,<3.12"
 boto3 = "^1.7"
-click = "8.0.3"
+click = "8.1.7"
 
 [tool.poetry.dev-dependencies]
 black = {version = "^18.3-alpha.0", allow-prereleases = true}
-pytest = "^3.0"
+pytest = "6.2.5"
 pytest-mock = "^1.10"
 moto = "^3.1.18"
 PyYAML = "^6.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `confidential-2.6.0/PKG-INFO` & `confidential-2.6.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: confidential
-Version: 2.6.0
+Version: 2.6.1
 Summary: Manage secrets in your projects using AWS Secrets Manager
 License: MIT
 Author: Daniel van Flymen
 Author-email: dvf@candidco.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.7,<2.0)
-Requires-Dist: click (==8.0.3)
+Requires-Dist: click (==8.1.7)
```

