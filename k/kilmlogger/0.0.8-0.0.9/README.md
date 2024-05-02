# Comparing `tmp/kilmlogger-0.0.8.tar.gz` & `tmp/kilmlogger-0.0.9.tar.gz`

## Comparing `kilmlogger-0.0.8.tar` & `kilmlogger-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/__init__.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/config.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/constants.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/correlation.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/envs.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/handler.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/processor.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/styles.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/utils.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/services/scribe/client.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/services/scribe/grpc/scribelog.proto
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/services/scribe/grpc/scribelog_pb2.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/services/scribe/grpc/scribelog_pb2.pyi
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/kilmlogger/services/scribe/grpc/scribelog_pb2_grpc.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/README.md
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 kilmlogger-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/__init__.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/config.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/constants.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/correlation.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/envs.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/handler.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/processor.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/styles.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/utils.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/services/scribe/client.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog.proto
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2.pyi
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2_grpc.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/README.md
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 kilmlogger-0.0.9/PKG-INFO
```

### Comparing `kilmlogger-0.0.8/kilmlogger/config.py` & `kilmlogger-0.0.9/kilmlogger/config.py`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.8/kilmlogger/correlation.py` & `kilmlogger-0.0.9/kilmlogger/correlation.py`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.8/kilmlogger/handler.py` & `kilmlogger-0.0.9/kilmlogger/handler.py`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.8/kilmlogger/processor.py` & `kilmlogger-0.0.9/kilmlogger/processor.py`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.8/kilmlogger/styles.py` & `kilmlogger-0.0.9/kilmlogger/styles.py`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.8/kilmlogger/services/scribe/client.py` & `kilmlogger-0.0.9/kilmlogger/services/scribe/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
         return {
             "log_time": msg["time"],
             "app_name": self.app_name,
             "app_mode": self.app_prop,
             "event_category": msg["level"],
             "correlation_id": msg["correlation_id"],
             "params": {
+                "time": msg["time"],
                 "msg": msg["msg"],
             },
         }
 
     def log(self, msg: dict):
         self.grpc_stub.sendMultiLogV2(
             self._build_request(
```

### Comparing `kilmlogger-0.0.8/kilmlogger/services/scribe/grpc/scribelog.proto` & `kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog.proto`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.8/kilmlogger/services/scribe/grpc/scribelog_pb2.py` & `kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2.py`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.8/kilmlogger/services/scribe/grpc/scribelog_pb2.pyi` & `kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.8/kilmlogger/services/scribe/grpc/scribelog_pb2_grpc.py` & `kilmlogger-0.0.9/kilmlogger/services/scribe/grpc/scribelog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.8/pyproject.toml` & `kilmlogger-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kilmlogger-0.0.8/PKG-INFO` & `kilmlogger-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilmlogger
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Python Logger for all ZLB's Project
 Project-URL: Documentation, https://github.com/unknown/kilmlogger#readme
 Project-URL: Issues, https://github.com/unknown/kilmlogger/issues
 Project-URL: Source, https://github.com/unknown/kilmlogger
 Author-email: vietnh8 <vietnh8@vng.com.vn>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

