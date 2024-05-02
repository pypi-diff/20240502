# Comparing `tmp/seaplane-0.6a8.tar.gz` & `tmp/seaplane-0.6a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplane-0.6a8.tar", max compression
+gzip compressed data, was "seaplane-0.6a9.tar", max compression
```

## Comparing `seaplane-0.6a8.tar` & `seaplane-0.6a9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1617 2024-01-10 23:00:46.682643 seaplane-0.6a8/README.md
--rw-r--r--   0        0        0     5924 2024-01-10 23:00:46.686643 seaplane-0.6a8/pyproject.toml
--rw-r--r--   0        0        0      175 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/apps/__init__.py
--rw-r--r--   0        0        0     9902 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/apps/cli.py
--rw-r--r--   0        0        0     1009 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/apps/debug_schema.py
--rw-r--r--   0        0        0     6140 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/apps/decorators.py
--rw-r--r--   0        0        0     4622 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/apps/entry_points.py
--rw-r--r--   0        0        0     3839 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/apps/status.py
--rw-r--r--   0        0        0     7152 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/config.py
--rw-r--r--   0        0        0     4759 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/deploy/__init__.py
--rw-r--r--   0        0        0     6151 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/deploy/utils.py
--rw-r--r--   0        0        0      540 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/errors.py
--rw-r--r--   0        0        0     1544 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/integrations/langchain.py
--rw-r--r--   0        0        0     5879 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/kv.py
--rw-r--r--   0        0        0     2168 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/logs.py
--rw-r--r--   0        0        0     7111 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/object.py
--rw-r--r--   0        0        0    11741 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/pipes/__init__.py
--rw-r--r--   0        0        0     8894 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/pipes/executor.py
--rw-r--r--   0        0        0      128 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/run_load_dotenv.py
--rw-r--r--   0        0        0        0 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/sdk_internal_utils/__init__.py
--rw-r--r--   0        0        0     1699 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/sdk_internal_utils/buckets.py
--rw-r--r--   0        0        0      391 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/sdk_internal_utils/http.py
--rw-r--r--   0        0        0     3371 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/sdk_internal_utils/token_api.py
--rw-r--r--   0        0        0     4402 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/sdk_internal_utils/token_auth.py
--rw-r--r--   0        0        0      766 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/sql.py
--rw-r--r--   0        0        0     8755 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/substation.py
--rw-r--r--   0        0        0     6545 2024-01-10 23:00:46.686643 seaplane-0.6a8/src/seaplane/vector.py
--rw-r--r--   0        0        0     3521 1970-01-01 00:00:00.000000 seaplane-0.6a8/PKG-INFO
+-rw-r--r--   0        0        0     1617 2024-01-10 23:57:17.969866 seaplane-0.6a9/README.md
+-rw-r--r--   0        0        0     5924 2024-01-10 23:57:17.969866 seaplane-0.6a9/pyproject.toml
+-rw-r--r--   0        0        0      175 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/apps/__init__.py
+-rw-r--r--   0        0        0     9902 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/apps/cli.py
+-rw-r--r--   0        0        0     1009 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/apps/debug_schema.py
+-rw-r--r--   0        0        0     6140 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/apps/decorators.py
+-rw-r--r--   0        0        0     4622 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/apps/entry_points.py
+-rw-r--r--   0        0        0     3839 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/apps/status.py
+-rw-r--r--   0        0        0     7152 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/config.py
+-rw-r--r--   0        0        0     4759 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/deploy/__init__.py
+-rw-r--r--   0        0        0     6407 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/deploy/utils.py
+-rw-r--r--   0        0        0      540 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/errors.py
+-rw-r--r--   0        0        0     1544 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/integrations/langchain.py
+-rw-r--r--   0        0        0     5879 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/kv.py
+-rw-r--r--   0        0        0     2168 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/logs.py
+-rw-r--r--   0        0        0     7111 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/object.py
+-rw-r--r--   0        0        0    11741 2024-01-10 23:57:17.969866 seaplane-0.6a9/src/seaplane/pipes/__init__.py
+-rw-r--r--   0        0        0     8894 2024-01-10 23:57:17.973866 seaplane-0.6a9/src/seaplane/pipes/executor.py
+-rw-r--r--   0        0        0      128 2024-01-10 23:57:17.973866 seaplane-0.6a9/src/seaplane/run_load_dotenv.py
+-rw-r--r--   0        0        0        0 2024-01-10 23:57:17.973866 seaplane-0.6a9/src/seaplane/sdk_internal_utils/__init__.py
+-rw-r--r--   0        0        0     1699 2024-01-10 23:57:17.973866 seaplane-0.6a9/src/seaplane/sdk_internal_utils/buckets.py
+-rw-r--r--   0        0        0      391 2024-01-10 23:57:17.973866 seaplane-0.6a9/src/seaplane/sdk_internal_utils/http.py
+-rw-r--r--   0        0        0     3371 2024-01-10 23:57:17.973866 seaplane-0.6a9/src/seaplane/sdk_internal_utils/token_api.py
+-rw-r--r--   0        0        0     4402 2024-01-10 23:57:17.973866 seaplane-0.6a9/src/seaplane/sdk_internal_utils/token_auth.py
+-rw-r--r--   0        0        0      766 2024-01-10 23:57:17.973866 seaplane-0.6a9/src/seaplane/sql.py
+-rw-r--r--   0        0        0     8755 2024-01-10 23:57:17.973866 seaplane-0.6a9/src/seaplane/substation.py
+-rw-r--r--   0        0        0     6545 2024-01-10 23:57:17.973866 seaplane-0.6a9/src/seaplane/vector.py
+-rw-r--r--   0        0        0     3521 1970-01-01 00:00:00.000000 seaplane-0.6a9/PKG-INFO
```

### Comparing `seaplane-0.6a8/README.md` & `seaplane-0.6a9/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/pyproject.toml` & `seaplane-0.6a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seaplane"
-version = "0.6a8"
+version = "0.6a9"
 description = "Seaplane Python SDK"
 authors = ["Seaplane IO, Inc."]
 license = "Apache License"
 readme = "README.md"
 repository = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 documentation = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
```

### Comparing `seaplane-0.6a8/src/seaplane/apps/cli.py` & `seaplane-0.6a9/src/seaplane/apps/cli.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/apps/debug_schema.py` & `seaplane-0.6a9/src/seaplane/apps/debug_schema.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/apps/decorators.py` & `seaplane-0.6a9/src/seaplane/apps/decorators.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/apps/entry_points.py` & `seaplane-0.6a9/src/seaplane/apps/entry_points.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/apps/status.py` & `seaplane-0.6a9/src/seaplane/apps/status.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/config.py` & `seaplane-0.6a9/src/seaplane/config.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/deploy/__init__.py` & `seaplane-0.6a9/src/seaplane/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/deploy/utils.py` & `seaplane-0.6a9/src/seaplane/deploy/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,22 +48,29 @@
         headers=headers(token),
     )
     resp.raise_for_status()
 
 
 @with_token
 def delete_store(token: str, name: str) -> None:
-    log.logger.debug(f"deleting store: {name}")
-    url = f"{config.carrier_endpoint}/kv/{name}"
-
-    resp = requests.delete(
+    url = f"{config.carrier_endpoint}/kv"
+    stores = requests.get(
         url,
         headers=headers(token),
     )
-    resp.raise_for_status()
+    stores.raise_for_status()
+    store_list = eval(stores.content.decode())
+    if name in set(store_list):
+        log.logger.debug(f"deleting store: {name}")
+        url = f"{config.carrier_endpoint}/kv/{name}"
+        resp = requests.delete(
+            url,
+            headers=headers(token),
+        )
+        resp.raise_for_status()
 
 
 @with_token
 def create_stream(token: str, name: str) -> None:
     log.logger.debug(f"creating stream: {name}")
     url = f"{config.carrier_endpoint}/stream/{name}"
```

### Comparing `seaplane-0.6a8/src/seaplane/errors.py` & `seaplane-0.6a9/src/seaplane/errors.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/integrations/langchain.py` & `seaplane-0.6a9/src/seaplane/integrations/langchain.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/kv.py` & `seaplane-0.6a9/src/seaplane/kv.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/logs.py` & `seaplane-0.6a9/src/seaplane/logs.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/object.py` & `seaplane-0.6a9/src/seaplane/object.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/pipes/__init__.py` & `seaplane-0.6a9/src/seaplane/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/pipes/executor.py` & `seaplane-0.6a9/src/seaplane/pipes/executor.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/sdk_internal_utils/buckets.py` & `seaplane-0.6a9/src/seaplane/sdk_internal_utils/buckets.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/sdk_internal_utils/token_api.py` & `seaplane-0.6a9/src/seaplane/sdk_internal_utils/token_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/sdk_internal_utils/token_auth.py` & `seaplane-0.6a9/src/seaplane/sdk_internal_utils/token_auth.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/sql.py` & `seaplane-0.6a9/src/seaplane/sql.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/substation.py` & `seaplane-0.6a9/src/seaplane/substation.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/src/seaplane/vector.py` & `seaplane-0.6a9/src/seaplane/vector.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.6a8/PKG-INFO` & `seaplane-0.6a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplane
-Version: 0.6a8
+Version: 0.6a9
 Summary: Seaplane Python SDK
 Home-page: https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 License: Apache License
 Author: Seaplane IO, Inc.
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

