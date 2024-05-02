# Comparing `tmp/shipyard_s3-0.1.4.tar.gz` & `tmp/shipyard_s3-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_s3-0.1.4.tar", max compression
+gzip compressed data, was "shipyard_s3-0.1.5a0.tar", max compression
```

## Comparing `shipyard_s3-0.1.4.tar` & `shipyard_s3-0.1.5a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-08-14 16:50:02.445112 shipyard_s3-0.1.4/README.md
--rw-r--r--   0        0        0      627 2024-03-07 16:13:45.942177 shipyard_s3-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       25 2024-02-22 17:47:27.269473 shipyard_s3-0.1.4/shipyard_s3/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 23:00:58.542212 shipyard_s3-0.1.4/shipyard_s3/cli/__init__.py
--rw-r--r--   0        0        0      608 2024-03-05 23:00:58.542801 shipyard_s3-0.1.4/shipyard_s3/cli/authtest.py
--rw-r--r--   0        0        0     4894 2024-03-07 16:13:45.943012 shipyard_s3-0.1.4/shipyard_s3/cli/download.py
--rw-r--r--   0        0        0     5197 2024-03-05 23:00:58.549349 shipyard_s3-0.1.4/shipyard_s3/cli/move.py
--rw-r--r--   0        0        0     3308 2024-03-05 23:00:58.554081 shipyard_s3-0.1.4/shipyard_s3/cli/remove.py
--rw-r--r--   0        0        0     5792 2024-03-07 16:13:45.943628 shipyard_s3-0.1.4/shipyard_s3/cli/upload.py
--rw-r--r--   0        0        0     8721 2024-03-07 16:13:45.944227 shipyard_s3-0.1.4/shipyard_s3/s3.py
--rw-r--r--   0        0        0     2386 2024-03-07 16:13:45.944697 shipyard_s3-0.1.4/shipyard_s3/utils/exceptions.py
--rw-r--r--   0        0        0      781 2024-03-05 23:00:58.565403 shipyard_s3-0.1.4/shipyard_s3/utils/utils.py
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 shipyard_s3-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.839785 shipyard_s3-0.1.5a0/README.md
+-rw-r--r--   0        0        0      629 2024-05-02 20:31:07.798494 shipyard_s3-0.1.5a0/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-05-12 18:48:21.840305 shipyard_s3-0.1.5a0/shipyard_s3/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.447197 shipyard_s3-0.1.5a0/shipyard_s3/cli/__init__.py
+-rw-r--r--   0        0        0      433 2024-05-02 20:30:30.260693 shipyard_s3-0.1.5a0/shipyard_s3/cli/authtest.py
+-rw-r--r--   0        0        0     4894 2024-03-08 15:17:28.225079 shipyard_s3-0.1.5a0/shipyard_s3/cli/download.py
+-rw-r--r--   0        0        0     5197 2024-02-27 15:08:25.023699 shipyard_s3-0.1.5a0/shipyard_s3/cli/move.py
+-rw-r--r--   0        0        0     3308 2024-03-06 13:42:18.655104 shipyard_s3-0.1.5a0/shipyard_s3/cli/remove.py
+-rw-r--r--   0        0        0     5792 2024-03-08 15:17:28.225579 shipyard_s3-0.1.5a0/shipyard_s3/cli/upload.py
+-rw-r--r--   0        0        0     9351 2024-05-02 20:30:30.316826 shipyard_s3-0.1.5a0/shipyard_s3/s3.py
+-rw-r--r--   0        0        0     2386 2024-03-08 15:17:28.226639 shipyard_s3-0.1.5a0/shipyard_s3/utils/exceptions.py
+-rw-r--r--   0        0        0      781 2024-02-27 15:08:25.119517 shipyard_s3-0.1.5a0/shipyard_s3/utils/utils.py
+-rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 shipyard_s3-0.1.5a0/PKG-INFO
```

### Comparing `shipyard_s3-0.1.4/pyproject.toml` & `shipyard_s3-0.1.5a0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-s3"
-version = "0.1.4"
+version = "0.1.5a0"
 description = "A local client for connecting and working with AWS S3"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_s3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_s3-0.1.4/shipyard_s3/cli/download.py` & `shipyard_s3-0.1.5a0/shipyard_s3/cli/download.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.4/shipyard_s3/cli/move.py` & `shipyard_s3-0.1.5a0/shipyard_s3/cli/move.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.4/shipyard_s3/cli/remove.py` & `shipyard_s3-0.1.5a0/shipyard_s3/cli/remove.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.4/shipyard_s3/cli/upload.py` & `shipyard_s3-0.1.5a0/shipyard_s3/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.4/shipyard_s3/s3.py` & `shipyard_s3-0.1.5a0/shipyard_s3/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-import boto3
 import os
-from shipyard_templates import CloudStorage, ExitCodeException, ShipyardLogger
-from boto3.exceptions import S3UploadFailedError
 from typing import Optional, Dict, Any, List
+
+import boto3
+from boto3.exceptions import S3UploadFailedError
+from shipyard_templates import CloudStorage, ExitCodeException, ShipyardLogger
+
+from shipyard_s3.utils import utils
 from shipyard_s3.utils.exceptions import (
     BucketDoesNotExist,
     DownloadError,
     InvalidBucketAccess,
     InvalidCredentials,
     InvalidRegion,
     ListObjectsError,
     MoveError,
     RemoveError,
     UploadError,
 )
-from shipyard_s3.utils import utils
-
 
 logger = ShipyardLogger.get_logger()
 
 
 class S3Client(CloudStorage):
     def __init__(
         self,
@@ -31,20 +32,38 @@
         self.aws_secret_access_key = aws_secret_access_key
         self.region = region
         self._s3_conn = None
 
     @property
     def s3_conn(self):
         if not self._s3_conn:
-            self._s3_conn = self.connect()
+            self._s3_conn = self.get_connection()
         return self._s3_conn
 
     def connect(self):
+        try:
+            boto3.client(
+                "sts",
+                region_name=self.region,
+                aws_access_key_id=self.aws_access_key,
+                aws_secret_access_key=self.aws_secret_access_key,
+            ).get_caller_identity()
+        except Exception as e:
+            logger.authtest(
+                f"Could not validate credentials to S3 with the provided credentials. Response from the "
+                f"server: {str(e)}"
+            )
+            return 1
+        else:
+            logger.authtest("Successfully connected to S3")
+            return 0
+
+    def get_connection(self):
         if self._s3_conn:
-            return self._s3_conn  # resuse existing connection
+            return self._s3_conn  # reuse existing connection
         try:
             logger.debug("Establishing connection with S3")
             client = boto3.client(
                 "s3",
                 region_name=self.region,
                 aws_access_key_id=self.aws_access_key,
                 aws_secret_access_key=self.aws_secret_access_key,
```

### Comparing `shipyard_s3-0.1.4/shipyard_s3/utils/exceptions.py` & `shipyard_s3-0.1.5a0/shipyard_s3/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.4/shipyard_s3/utils/utils.py` & `shipyard_s3-0.1.5a0/shipyard_s3/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_s3-0.1.4/PKG-INFO` & `shipyard_s3-0.1.5a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-s3
-Version: 0.1.4
+Version: 0.1.5a0
 Summary: A local client for connecting and working with AWS S3
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

