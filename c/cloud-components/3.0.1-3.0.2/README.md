# Comparing `tmp/cloud_components-3.0.1.tar.gz` & `tmp/cloud_components-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_components-3.0.1.tar", max compression
+gzip compressed data, was "cloud_components-3.0.2.tar", max compression
```

## Comparing `cloud_components-3.0.1.tar` & `cloud_components-3.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1080 2024-01-25 21:09:51.070206 cloud_components-3.0.1/LICENSE
--rw-r--r--   0        0        0      870 2024-01-25 21:09:51.070206 cloud_components-3.0.1/README.md
--rw-r--r--   0        0        0      777 2024-01-25 21:09:51.070206 cloud_components-3.0.1/cloud_components/application/interface/infra/builder.py
--rwxr-xr-x   0        0        0      444 2024-01-25 21:09:51.070206 cloud_components-3.0.1/cloud_components/application/interface/infra/event.py
--rwxr-xr-x   0        0        0      246 2024-01-25 21:09:51.070206 cloud_components-3.0.1/cloud_components/application/interface/infra/function.py
--rwxr-xr-x   0        0        0      480 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/application/interface/infra/queue.py
--rw-r--r--   0        0        0      601 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/application/interface/infra/storage.py
--rw-r--r--   0        0        0      456 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/application/interface/services/env/enviroment.py
--rw-r--r--   0        0        0      456 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/application/interface/services/enviroment/enviroment.py
--rw-r--r--   0        0        0      235 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/application/interface/services/log/builder.py
--rw-r--r--   0        0        0      695 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/application/interface/services/log/logger.py
--rw-r--r--   0        0        0       94 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/application/types/aws.py
--rw-r--r--   0        0        0     2729 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/infra/aws/builder.py
--rw-r--r--   0        0        0      861 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/infra/aws/connection/connector_factory.py
--rw-r--r--   0        0        0     2457 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/infra/aws/connection/resource_connector.py
--rwxr-xr-x   0        0        0      740 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/infra/aws/resources/lambda_function.py
--rw-r--r--   0        0        0     3127 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/infra/aws/resources/s3.py
--rwxr-xr-x   0        0        0     1513 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/infra/aws/resources/sns.py
--rwxr-xr-x   0        0        0     1258 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/infra/aws/resources/sqs.py
--rw-r--r--   0        0        0     1471 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/infra/factory.py
--rw-r--r--   0        0        0      996 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/services/env/dotenv.py
--rw-r--r--   0        0        0      418 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/services/env/factory.py
--rw-r--r--   0        0        0      259 2024-01-25 21:09:51.074206 cloud_components-3.0.1/cloud_components/services/log/builder.py
--rw-r--r--   0        0        0      529 2024-01-25 21:09:51.074206 cloud_components-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 cloud_components-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-02 21:23:33.252525 cloud_components-3.0.2/LICENSE
+-rw-r--r--   0        0        0      870 2024-05-02 21:23:33.252525 cloud_components-3.0.2/README.md
+-rw-r--r--   0        0        0      777 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/application/interface/infra/builder.py
+-rwxr-xr-x   0        0        0      444 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/application/interface/infra/event.py
+-rwxr-xr-x   0        0        0      246 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/application/interface/infra/function.py
+-rwxr-xr-x   0        0        0      480 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/application/interface/infra/queue.py
+-rw-r--r--   0        0        0      824 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/application/interface/infra/storage.py
+-rw-r--r--   0        0        0      456 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/application/interface/services/env/enviroment.py
+-rw-r--r--   0        0        0      456 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/application/interface/services/enviroment/enviroment.py
+-rw-r--r--   0        0        0      235 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/application/interface/services/log/builder.py
+-rw-r--r--   0        0        0      695 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/application/interface/services/log/logger.py
+-rw-r--r--   0        0        0       94 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/application/types/aws.py
+-rw-r--r--   0        0        0     2729 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/infra/aws/builder.py
+-rw-r--r--   0        0        0      861 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/infra/aws/connection/connector_factory.py
+-rw-r--r--   0        0        0     2457 2024-05-02 21:23:33.252525 cloud_components-3.0.2/cloud_components/infra/aws/connection/resource_connector.py
+-rwxr-xr-x   0        0        0      740 2024-05-02 21:23:33.256525 cloud_components-3.0.2/cloud_components/infra/aws/resources/lambda_function.py
+-rw-r--r--   0        0        0     3556 2024-05-02 21:23:33.256525 cloud_components-3.0.2/cloud_components/infra/aws/resources/s3.py
+-rwxr-xr-x   0        0        0     1513 2024-05-02 21:23:33.256525 cloud_components-3.0.2/cloud_components/infra/aws/resources/sns.py
+-rwxr-xr-x   0        0        0     1258 2024-05-02 21:23:33.256525 cloud_components-3.0.2/cloud_components/infra/aws/resources/sqs.py
+-rw-r--r--   0        0        0     1471 2024-05-02 21:23:33.256525 cloud_components-3.0.2/cloud_components/infra/factory.py
+-rw-r--r--   0        0        0      996 2024-05-02 21:23:33.256525 cloud_components-3.0.2/cloud_components/services/env/dotenv.py
+-rw-r--r--   0        0        0      418 2024-05-02 21:23:33.256525 cloud_components-3.0.2/cloud_components/services/env/factory.py
+-rw-r--r--   0        0        0      259 2024-05-02 21:23:33.256525 cloud_components-3.0.2/cloud_components/services/log/builder.py
+-rw-r--r--   0        0        0      529 2024-05-02 21:23:33.256525 cloud_components-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 cloud_components-3.0.2/PKG-INFO
```

### Comparing `cloud_components-3.0.1/LICENSE` & `cloud_components-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/README.md` & `cloud_components-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/cloud_components/application/interface/infra/builder.py` & `cloud_components-3.0.2/cloud_components/application/interface/infra/builder.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/cloud_components/application/interface/infra/storage.py` & `cloud_components-3.0.2/cloud_components/application/interface/infra/storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,7 +22,15 @@
     def bucket(self) -> Any:
         raise NotImplementedError
 
     @bucket.setter
     @abstractmethod
     def bucket(self, name: str):
         raise NotImplementedError
+
+    @abstractmethod
+    def ls(self, path: str) -> list[str]:  # pylint: disable=C0103
+        raise NotImplementedError
+
+    @abstractmethod
+    def delete(self, file_path: str) -> bool:
+        raise NotImplementedError
```

### Comparing `cloud_components-3.0.1/cloud_components/application/interface/services/log/logger.py` & `cloud_components-3.0.2/cloud_components/application/interface/services/log/logger.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/cloud_components/infra/aws/builder.py` & `cloud_components-3.0.2/cloud_components/infra/aws/builder.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/cloud_components/infra/aws/connection/connector_factory.py` & `cloud_components-3.0.2/cloud_components/infra/aws/connection/connector_factory.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/cloud_components/infra/aws/connection/resource_connector.py` & `cloud_components-3.0.2/cloud_components/infra/aws/connection/resource_connector.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/cloud_components/infra/aws/resources/lambda_function.py` & `cloud_components-3.0.2/cloud_components/infra/aws/resources/lambda_function.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/cloud_components/infra/aws/resources/s3.py` & `cloud_components-3.0.2/cloud_components/infra/aws/resources/s3.py`

 * *Files 19% similar despite different names*

```diff
@@ -100,7 +100,18 @@
             content = content.get()["Body"].read()
         except ClientError as err:
             self.logger.error(
                 f"An error occurred when try to get a file in S3. Error detail: {err}"
             )
             return None
         return content
+
+    def ls(self, path: str) -> list[str]:  # pylint: disable=C0103
+        self.logger.info(f"Listing objects from {path}")
+        return [_object.key for _object in self.bucket.objects.filter(Prefix=path)]
+
+    def delete(self, file_path: str) -> bool:
+        try:
+            self.bucket.Object(file_path).delete()
+        except Exception as err:  # pylint: disable=W0612,W0718
+            return False
+        return True
```

### Comparing `cloud_components-3.0.1/cloud_components/infra/aws/resources/sns.py` & `cloud_components-3.0.2/cloud_components/infra/aws/resources/sns.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/cloud_components/infra/aws/resources/sqs.py` & `cloud_components-3.0.2/cloud_components/infra/aws/resources/sqs.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/cloud_components/infra/factory.py` & `cloud_components-3.0.2/cloud_components/infra/factory.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/cloud_components/services/env/dotenv.py` & `cloud_components-3.0.2/cloud_components/services/env/dotenv.py`

 * *Files identical despite different names*

### Comparing `cloud_components-3.0.1/pyproject.toml` & `cloud_components-3.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-components"
-version = "3.0.1"
+version = "3.0.2"
 description = ""
 authors = ["Giovani Liskoski Zanini <giovanilzanini@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cloud_components"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cloud_components-3.0.1/PKG-INFO` & `cloud_components-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-components
-Version: 3.0.1
+Version: 3.0.2
 Summary: 
 License: MIT
 Author: Giovani Liskoski Zanini
 Author-email: giovanilzanini@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

