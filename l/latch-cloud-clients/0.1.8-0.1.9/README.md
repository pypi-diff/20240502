# Comparing `tmp/latch_cloud_clients-0.1.8.tar.gz` & `tmp/latch_cloud_clients-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_cloud_clients-0.1.8.tar", max compression
+gzip compressed data, was "latch_cloud_clients-0.1.9.tar", max compression
```

## Comparing `latch_cloud_clients-0.1.8.tar` & `latch_cloud_clients-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.8/LICENSE
--rw-r--r--   0        0        0      121 2024-04-24 21:08:53.493221 latch_cloud_clients-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.8/latch_cloud_clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.8/latch_cloud_clients/aws/__init__.py
--rw-r--r--   0        0        0    11808 2024-04-27 18:30:47.134379 latch_cloud_clients-0.1.8/latch_cloud_clients/aws/storage_client.py
--rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.8/latch_cloud_clients/gcp/__init__.py
--rw-r--r--   0        0        0     2639 2024-04-27 18:28:09.547136 latch_cloud_clients-0.1.8/latch_cloud_clients/gcp/client_pool.py
--rw-r--r--   0        0        0    17851 2024-04-27 18:40:43.543767 latch_cloud_clients-0.1.8/latch_cloud_clients/gcp/storage.py
--rw-r--r--   0        0        0     7211 2024-04-27 18:31:31.609721 latch_cloud_clients-0.1.8/latch_cloud_clients/gcp/storage_client.py
--rw-r--r--   0        0        0      809 2024-04-26 17:58:15.128561 latch_cloud_clients-0.1.8/latch_cloud_clients/get_storage_client.py
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.8/latch_cloud_clients/py.typed
--rw-r--r--   0        0        0     2901 2024-04-27 18:33:06.209679 latch_cloud_clients-0.1.8/latch_cloud_clients/utils.py
--rw-r--r--   0        0        0     1502 2024-04-27 19:42:09.511948 latch_cloud_clients-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.9/LICENSE
+-rw-r--r--   0        0        0      121 2024-04-24 21:08:53.493221 latch_cloud_clients-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.9/latch_cloud_clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.9/latch_cloud_clients/aws/__init__.py
+-rw-r--r--   0        0        0    11808 2024-04-27 18:30:47.134379 latch_cloud_clients-0.1.9/latch_cloud_clients/aws/storage_client.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.9/latch_cloud_clients/gcp/__init__.py
+-rw-r--r--   0        0        0     2639 2024-04-27 18:28:09.547136 latch_cloud_clients-0.1.9/latch_cloud_clients/gcp/client_pool.py
+-rw-r--r--   0        0        0    17879 2024-04-30 22:30:33.173896 latch_cloud_clients-0.1.9/latch_cloud_clients/gcp/storage.py
+-rw-r--r--   0        0        0     7211 2024-04-27 18:31:31.609721 latch_cloud_clients-0.1.9/latch_cloud_clients/gcp/storage_client.py
+-rw-r--r--   0        0        0      809 2024-04-26 17:58:15.128561 latch_cloud_clients-0.1.9/latch_cloud_clients/get_storage_client.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.9/latch_cloud_clients/py.typed
+-rw-r--r--   0        0        0     2901 2024-04-27 18:33:06.209679 latch_cloud_clients-0.1.9/latch_cloud_clients/utils.py
+-rw-r--r--   0        0        0     1502 2024-04-30 22:30:38.461156 latch_cloud_clients-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.9/PKG-INFO
```

### Comparing `latch_cloud_clients-0.1.8/LICENSE` & `latch_cloud_clients-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.8/latch_cloud_clients/aws/storage_client.py` & `latch_cloud_clients-0.1.9/latch_cloud_clients/aws/storage_client.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.8/latch_cloud_clients/gcp/client_pool.py` & `latch_cloud_clients-0.1.9/latch_cloud_clients/gcp/client_pool.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.8/latch_cloud_clients/gcp/storage.py` & `latch_cloud_clients-0.1.9/latch_cloud_clients/gcp/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,17 +194,17 @@
         except NotFound:
             return None
 
         return Object(
             name=res["name"],
             id=res["id"],
             bucket=res["bucket"],
-            media_link=res["mediaLink"],
-            generation=res["generation"],
-            content_type=res["contentType"],
+            media_link=res.get("mediaLink"),
+            generation=res.get("generation"),
+            content_type=res.get("contentType"),
             size=int(res["size"]),
             creation_time=datetime.fromisoformat(res["timeCreated"]),
             update_time=datetime.fromisoformat(res["updated"]),
         )
 
     def list_blobs(
         self,
@@ -303,17 +303,17 @@
             return_json=True,
         )
 
         return Object(
             id=resp["id"],
             name=resp["name"],
             bucket=resp["bucket"],
-            media_link=resp["mediaLink"],
-            generation=resp["generation"],
-            content_type=resp["contentType"],
+            media_link=resp.get("mediaLink"),
+            generation=resp.get("generation"),
+            content_type=resp.get("contentType"),
             size=int(resp["size"]),
             creation_time=datetime.fromisoformat(resp["timeCreated"]),
             update_time=datetime.fromisoformat(resp["updated"]),
         )
 
     async def copy_blob(
         self,
@@ -533,15 +533,15 @@
 
             return Object(
                 id=obj["id"],
                 name=obj["name"],
                 bucket=obj["bucket"],
                 media_link=obj.get("mediaLink"),
                 generation=obj.get("generation"),
-                content_type=obj["contentType"],
+                content_type=obj.get("contentType"),
                 size=int(obj["size"]),
                 creation_time=creation_time,
                 update_time=update_time,
             )
 
         if self.next_page_token:
             self.params["pageToken"] = self.next_page_token
```

### Comparing `latch_cloud_clients-0.1.8/latch_cloud_clients/gcp/storage_client.py` & `latch_cloud_clients-0.1.9/latch_cloud_clients/gcp/storage_client.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.8/latch_cloud_clients/get_storage_client.py` & `latch_cloud_clients-0.1.9/latch_cloud_clients/get_storage_client.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.8/latch_cloud_clients/utils.py` & `latch_cloud_clients-0.1.9/latch_cloud_clients/utils.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.8/pyproject.toml` & `latch_cloud_clients-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-cloud-clients"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Taras Priadka <taras@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_cloud_clients"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_cloud_clients-0.1.8/PKG-INFO` & `latch_cloud_clients-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-cloud-clients
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: CC0 1.0
 Author: Taras Priadka
 Author-email: taras@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

