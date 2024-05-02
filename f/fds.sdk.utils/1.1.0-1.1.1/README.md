# Comparing `tmp/fds_sdk_utils-1.1.0.tar.gz` & `tmp/fds_sdk_utils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fds_sdk_utils-1.1.0.tar", max compression
+gzip compressed data, was "fds_sdk_utils-1.1.1.tar", max compression
```

## Comparing `fds_sdk_utils-1.1.0.tar` & `fds_sdk_utils-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/LICENSE
--rw-r--r--   0        0        0     6461 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/README.md
--rw-r--r--   0        0        0      796 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/__init__.py
--rw-r--r--   0        0        0      253 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/__init__.py
--rw-r--r--   0        0        0      273 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/__init__.py
--rw-r--r--   0        0        0    12392 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/confidential.py
--rw-r--r--   0        0        0      722 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/constants.py
--rw-r--r--   0        0        0      724 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/exceptions.py
--rw-r--r--   0        0        0      332 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/oauth2client.py
--rw-r--r--   0        0        0     7357 1970-01-01 00:00:00.000000 fds_sdk_utils-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/LICENSE
+-rw-r--r--   0        0        0     6461 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/README.md
+-rw-r--r--   0        0        0      853 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/__init__.py
+-rw-r--r--   0        0        0      253 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/__init__.py
+-rw-r--r--   0        0        0    12392 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/confidential.py
+-rw-r--r--   0        0        0      722 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/constants.py
+-rw-r--r--   0        0        0      724 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/exceptions.py
+-rw-r--r--   0        0        0      332 2024-05-02 12:53:38.399939 fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/oauth2client.py
+-rw-r--r--   0        0        0     7371 1970-01-01 00:00:00.000000 fds_sdk_utils-1.1.1/PKG-INFO
```

### Comparing `fds_sdk_utils-1.1.0/LICENSE` & `fds_sdk_utils-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fds_sdk_utils-1.1.0/README.md` & `fds_sdk_utils-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fds_sdk_utils-1.1.0/pyproject.toml` & `fds_sdk_utils-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [tool.poetry]
 name = "fds.sdk.utils"
-version = "1.1.0"
+version = "1.1.1"
 description = "Utilities for interacting with FactSet APIs."
-authors=["FactSet Research Systems"]
-license="Apache-2.0"
-readme="README.md"
-homepage="https://developer.factset.com"
-keywords=[
+authors = ["FactSet Research Systems"]
+license = "Apache-2.0"
+readme = "README.md"
+homepage = "https://developer.factset.com"
+keywords = [
   "FactSet",
   "API",
   "SDK"
 ]
-packages=[
+packages = [
   { include = "fds", from = "src" }
 ]
-exclude=["tests"]
+exclude = ["tests"]
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
-python-jose = "^3.3.0"
+python-jose = { extras = ["cryptography"], version = "^3.3.0" }
 requests-oauthlib = "^1.3.0"
 requests = "^2.28.2"
 oauthlib = "^3.2.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4"
-black = {version = "^23.3", allow-prereleases = true}
+black = { version = "^23.3", allow-prereleases = true }
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.11.1"
 tox = "^4.8.0"
 tox-gh-actions = "^3.2.0"
 
 [tool.black]
 line-length = 120
```

### Comparing `fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/confidential.py` & `fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/confidential.py`

 * *Files identical despite different names*

### Comparing `fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/constants.py` & `fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/constants.py`

 * *Files identical despite different names*

### Comparing `fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/exceptions.py` & `fds_sdk_utils-1.1.1/src/fds/sdk/utils/authentication/exceptions.py`

 * *Files identical despite different names*

### Comparing `fds_sdk_utils-1.1.0/PKG-INFO` & `fds_sdk_utils-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fds.sdk.utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: Utilities for interacting with FactSet APIs.
 Home-page: https://developer.factset.com
 License: Apache-2.0
 Keywords: FactSet,API,SDK
 Author: FactSet Research Systems
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
-Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 <img alt="FactSet" src="https://www.factset.com/hubfs/Assets/images/factset-logo.svg" height="56" width="290">
 
 # FactSet SDK Utilities for Python
```

