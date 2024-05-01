# Comparing `tmp/awsync-0.1.0.tar.gz` & `tmp/awsync-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsync-0.1.0.tar", max compression
+gzip compressed data, was "awsync-0.1.1.tar", max compression
```

## Comparing `awsync-0.1.0.tar` & `awsync-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-05-01 04:32:50.769212 awsync-0.1.0/LICENSE
--rw-r--r--   0        0        0     2395 2024-05-01 06:49:57.239651 awsync-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-01 04:07:11.855130 awsync-0.1.0/awsync/__init__.py
--rw-r--r--   0        0        0     1291 2024-05-01 04:07:11.858130 awsync-0.1.0/awsync/__main__.py
--rw-r--r--   0        0        0     7403 2024-05-01 04:07:11.857129 awsync-0.1.0/awsync/client.py
--rw-r--r--   0        0        0        0 2024-05-01 04:07:11.852130 awsync-0.1.0/awsync/models/__init__.py
--rw-r--r--   0        0        0     2258 2024-05-01 04:07:11.853129 awsync-0.1.0/awsync/models/aws.py
--rw-r--r--   0        0        0     1416 2024-05-01 04:07:11.851129 awsync-0.1.0/awsync/models/http.py
--rw-r--r--   0        0        0     9239 2024-05-01 04:07:11.856130 awsync-0.1.0/awsync/request.py
--rw-r--r--   0        0        0     1049 2024-05-01 06:48:21.343646 awsync-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 awsync-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 04:32:50.769212 awsync-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2395 2024-05-01 06:49:57.239651 awsync-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-01 04:07:11.855130 awsync-0.1.1/awsync/__init__.py
+-rw-r--r--   0        0        0     1291 2024-05-01 04:07:11.858130 awsync-0.1.1/awsync/__main__.py
+-rw-r--r--   0        0        0     7403 2024-05-01 04:07:11.857129 awsync-0.1.1/awsync/client.py
+-rw-r--r--   0        0        0        0 2024-05-01 04:07:11.852130 awsync-0.1.1/awsync/models/__init__.py
+-rw-r--r--   0        0        0     2275 2024-05-01 19:57:14.549055 awsync-0.1.1/awsync/models/aws.py
+-rw-r--r--   0        0        0     1433 2024-05-01 19:56:43.825054 awsync-0.1.1/awsync/models/http.py
+-rw-r--r--   0        0        0      283 2024-05-01 19:56:06.559052 awsync-0.1.1/awsync/models/strenum.py
+-rw-r--r--   0        0        0     9239 2024-05-01 04:07:11.856130 awsync-0.1.1/awsync/request.py
+-rw-r--r--   0        0        0     1048 2024-05-01 19:58:04.098058 awsync-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 awsync-0.1.1/PKG-INFO
```

### Comparing `awsync-0.1.0/LICENSE` & `awsync-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `awsync-0.1.0/README.md` & `awsync-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `awsync-0.1.0/awsync/__main__.py` & `awsync-0.1.1/awsync/__main__.py`

 * *Files identical despite different names*

### Comparing `awsync-0.1.0/awsync/client.py` & `awsync-0.1.1/awsync/client.py`

 * *Files identical despite different names*

### Comparing `awsync-0.1.0/awsync/models/aws.py` & `awsync-0.1.1/awsync/models/aws.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 "AWS type models."
-from enum import StrEnum
+from awsync.models.strenum import StrEnum
 from dataclasses import dataclass
 from typing import Optional
 
 
 @dataclass(frozen=True)
 class Credentials:
     "AWS Credentials."
```

### Comparing `awsync-0.1.0/awsync/models/http.py` & `awsync-0.1.1/awsync/models/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 "HTTP type models."
-from enum import StrEnum
+from awsync.models.strenum import StrEnum
 
 
 class Method(StrEnum):
     """
     A HTTP request method.
     See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods
     """
```

### Comparing `awsync-0.1.0/awsync/request.py` & `awsync-0.1.1/awsync/request.py`

 * *Files identical despite different names*

### Comparing `awsync-0.1.0/pyproject.toml` & `awsync-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awsync"
-version = "0.1.0"
+version = "0.1.1"
 description = "An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable."
 license = "Apache-2.0"
 authors = ["JKCT <jkct@visceralfx.com>"]
 readme = "README.md"
 packages = [{include = "awsync"}]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -13,15 +13,15 @@
     "Typing :: Typed",
     "Development Status :: 4 - Beta",
 ]
 keywords = ["aws", "async", "boto", "request", "sdk", "typed"]
 repository = "https://github.com/JKCT/awsync"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.8"
 httpx = "^0.27.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.0"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
```

### Comparing `awsync-0.1.0/PKG-INFO` & `awsync-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: awsync
-Version: 0.1.0
+Version: 0.1.1
 Summary: An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable.
 Home-page: https://github.com/JKCT/awsync
 License: Apache-2.0
 Keywords: aws,async,boto,request,sdk,typed
 Author: JKCT
 Author-email: jkct@visceralfx.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Project-URL: Repository, https://github.com/JKCT/awsync
 Description-Content-Type: text/markdown
 
 # awsync
```

