# Comparing `tmp/automizor-0.4.0.tar.gz` & `tmp/automizor-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automizor-0.4.0.tar", last modified: Sat Mar 30 09:20:33 2024, max compression
+gzip compressed data, was "automizor-0.4.1.tar", last modified: Thu May  2 12:17:02 2024, max compression
```

## Comparing `automizor-0.4.0.tar` & `automizor-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:20:33.909047 automizor-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-30 09:20:25.000000 automizor-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-30 09:20:25.000000 automizor-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-30 09:20:33.909047 automizor-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-30 09:20:25.000000 automizor-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:20:33.909047 automizor-0.4.0/automizor/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-30 09:20:25.000000 automizor-0.4.0/automizor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-30 09:20:25.000000 automizor-0.4.0/automizor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:20:33.909047 automizor-0.4.0/automizor/job/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-30 09:20:25.000000 automizor-0.4.0/automizor/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-03-30 09:20:25.000000 automizor-0.4.0/automizor/job/_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:20:33.909047 automizor-0.4.0/automizor/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-03-30 09:20:25.000000 automizor-0.4.0/automizor/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11021 2024-03-30 09:20:25.000000 automizor-0.4.0/automizor/storage/_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:20:33.909047 automizor-0.4.0/automizor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-30 09:20:25.000000 automizor-0.4.0/automizor/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:20:33.909047 automizor-0.4.0/automizor/vault/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-30 09:20:25.000000 automizor-0.4.0/automizor/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-30 09:20:25.000000 automizor-0.4.0/automizor/vault/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-03-30 09:20:25.000000 automizor-0.4.0/automizor/vault/_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:20:33.909047 automizor-0.4.0/automizor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-30 09:20:33.000000 automizor-0.4.0/automizor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-30 09:20:33.000000 automizor-0.4.0/automizor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 09:20:33.000000 automizor-0.4.0/automizor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-30 09:20:33.000000 automizor-0.4.0/automizor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-30 09:20:33.000000 automizor-0.4.0/automizor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-30 09:20:33.909047 automizor-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-30 09:20:25.000000 automizor-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.728154 automizor-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-02 12:16:45.000000 automizor-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 12:16:45.000000 automizor-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 12:17:02.728154 automizor-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 12:16:45.000000 automizor-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.724154 automizor-0.4.1/automizor/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.724154 automizor-0.4.1/automizor/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/job/_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.724154 automizor-0.4.1/automizor/log/
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/log/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.724154 automizor-0.4.1/automizor/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/storage/_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.724154 automizor-0.4.1/automizor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.728154 automizor-0.4.1/automizor/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/vault/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-02 12:16:45.000000 automizor-0.4.1/automizor/vault/_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:17:02.728154 automizor-0.4.1/automizor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 12:17:02.000000 automizor-0.4.1/automizor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 12:17:02.000000 automizor-0.4.1/automizor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:17:02.000000 automizor-0.4.1/automizor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 12:17:02.000000 automizor-0.4.1/automizor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 12:17:02.000000 automizor-0.4.1/automizor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 12:17:02.728154 automizor-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 12:16:45.000000 automizor-0.4.1/setup.py
```

### Comparing `automizor-0.4.0/LICENSE` & `automizor-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `automizor-0.4.0/PKG-INFO` & `automizor-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: automizor
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python Automizor framework
-Home-page: https://github.com/automizor/automizor
+Home-page: https://github.com/automizor/automizor-python
 Author: Christian Fischer
 Author-email: christian@automizor.io
 License: Apache License
 Keywords: automizor framework
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `automizor-0.4.0/automizor/exceptions.py` & `automizor-0.4.1/automizor/exceptions.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.0/automizor/job/__init__.py` & `automizor-0.4.1/automizor/job/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.0/automizor/job/_job.py` & `automizor-0.4.1/automizor/job/_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                     data = json.load(file)
         except json.JSONDecodeError:
             pass
 
         data[name] = value
 
         with open(file_path, "w", encoding="utf-8") as file:
-            json.dump(data, file, ensure_ascii=False, indent=4)
+            json.dump(data, file, ensure_ascii=False)
 
     def _read_file_context(self) -> dict:
         with open(self._context_file, "r", encoding="utf-8") as file:
             return json.load(file)
 
     def _read_job_context(self) -> dict:
         url = f"https://{self.url}/api/v1/rpa/job/{self._job_id}/"
```

### Comparing `automizor-0.4.0/automizor/storage/__init__.py` & `automizor-0.4.1/automizor/storage/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import json
 import mimetypes
 from functools import lru_cache
 from pathlib import Path
+from typing import List
 
 from ._storage import JSON
 
 
 @lru_cache
 def _get_storage():
     from ._storage import Storage
 
     return Storage()
 
 
-def list_assets() -> list[str]:
+def list_assets() -> List[str]:
     """
     Retrieves a list of all asset names.
 
     Returns:
         A list of all asset names.
     """
 
     storage = _get_storage()
     return storage.list_assets()
 
 
-def delete_asset(name: str) -> None:
+def delete_asset(name: str):
     """
     Deletes the specified asset.
 
     Parameters:
         name: The name identifier of the asset to delete.
     """
 
@@ -94,29 +95,29 @@
         The content of the asset as a text string.
     """
 
     storage = _get_storage()
     return storage.get_text(name)
 
 
-def set_bytes(name: str, data: bytes, content_type="application/octet-stream") -> None:
+def set_bytes(name: str, data: bytes, content_type="application/octet-stream"):
     """
     Uploads raw bytes as an asset.
 
     Parameters:
         name: The name identifier of the asset to upload.
         data: The raw byte content to upload.
         content_type: The MIME type of the asset.
     """
 
     storage = _get_storage()
     storage.set_bytes(name, data, content_type)
 
 
-def set_file(name: str, path: str, content_type: str = None) -> None:
+def set_file(name: str, path: str, content_type: str = None):
     """
     Uploads a file as an asset.
 
     Parameters:
         name: The name identifier of the asset to upload.
         path: The filesystem path of the file to upload.
         content_type: The MIME type of the asset.
@@ -128,15 +129,15 @@
         if content_type is None:
             content_type = "application/octet-stream"
 
     storage = _get_storage()
     storage.set_bytes(name, content, content_type)
 
 
-def set_json(name: str, value: JSON, **kwargs) -> None:
+def set_json(name: str, value: JSON, **kwargs):
     """
     Uploads JSON data as an asset.
 
     Parameters:
         name: The name identifier of the asset to upload.
         value: The JSON data to upload.
         kwargs: Additional keyword arguments to pass to json.dumps.
@@ -145,15 +146,15 @@
     content = json.dumps(value, **kwargs).encode("utf-8")
     content_type = "application/json"
 
     storage = _get_storage()
     storage.set_bytes(name, content, content_type)
 
 
-def set_text(name: str, text: str) -> None:
+def set_text(name: str, text: str):
     """
     Uploads text content as an asset.
 
     Parameters:
         name: The name identifier of the asset to upload.
         text: The text content to upload.
     """
```

### Comparing `automizor-0.4.0/automizor/storage/_storage.py` & `automizor-0.4.1/automizor/storage/_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             raise AutomizorError.from_response(
                 exc.response, "Failed to list assets"
             ) from exc
         except Exception as exc:
             raise AutomizorError("Failed to list assets") from exc
         return asset_names
 
-    def delete_asset(self, name: str) -> None:
+    def delete_asset(self, name: str):
         """
         Deletes the specified asset.
 
         This function deletes the asset identified by `name` from the storage service.
         It is useful for removing assets that are no longer needed or should be cleaned
         up to free up storage space.
 
@@ -177,15 +177,15 @@
 
         Returns:
             The content of the asset as a text string.
         """
 
         return self._download_file(name, mode="text")
 
-    def set_bytes(self, name: str, content: bytes, content_type: str) -> None:
+    def set_bytes(self, name: str, content: bytes, content_type: str):
         """
         Uploads the specified content as a new asset.
 
         This function uploads the provided `content` as a new asset with the specified
         `name`. It is useful for creating new assets or updating existing ones with
         fresh content.
 
@@ -196,15 +196,15 @@
         """
 
         try:
             self._update_asset(name, content, content_type)
         except NotFound:
             self._create_asset(name, content, content_type)
 
-    def _create_asset(self, name: str, content: bytes, content_type: str) -> None:
+    def _create_asset(self, name: str, content: bytes, content_type: str):
         """
         Creates a new asset with the specified content.
 
         This function creates a new asset with the specified `name` and `content` in the
         storage service. It is useful for uploading new assets or updating existing ones
         with fresh content.
 
@@ -265,15 +265,15 @@
         except requests.HTTPError as exc:
             raise AutomizorError.from_response(
                 exc.response, "Failed to get asset URL"
             ) from exc
         except Exception as exc:
             raise AutomizorError("Failed to get asset URL") from exc
 
-    def _update_asset(self, name: str, content: bytes, content_type: str) -> None:
+    def _update_asset(self, name: str, content: bytes, content_type: str):
         """
         Updates the specified asset with new content.
 
         This function updates the asset identified by `name` with fresh content
         provided as `content`. It is useful for modifying existing assets without
         creating a new asset, ensuring that the asset's content is up-to-date.
```

### Comparing `automizor-0.4.0/automizor/utils/__init__.py` & `automizor-0.4.1/automizor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.0/automizor/vault/__init__.py` & `automizor-0.4.1/automizor/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.0/automizor/vault/_container.py` & `automizor-0.4.1/automizor/vault/_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         """Secret.items() -> a set-like object providing a view on secret's items."""
         return self.value.items()
 
     def keys(self):
         """Secret.keys() -> a set-like object providing a view on secret's keys."""
         return self.value.keys()
 
-    def update(self, pairs: Dict[str, Any]) -> None:
+    def update(self, pairs: Dict[str, Any]):
         """Update the secret's dictionary with the key-value pairs from pairs."""
         self.value.update(pairs)
 
     def __getitem__(self, key):
         return self.value[key]
 
     def __setitem__(self, key, value):
```

### Comparing `automizor-0.4.0/automizor/vault/_vault.py` & `automizor-0.4.1/automizor/vault/_vault.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.0/automizor.egg-info/PKG-INFO` & `automizor-0.4.1/automizor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: automizor
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python Automizor framework
-Home-page: https://github.com/automizor/automizor
+Home-page: https://github.com/automizor/automizor-python
 Author: Christian Fischer
 Author-email: christian@automizor.io
 License: Apache License
 Keywords: automizor framework
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `automizor-0.4.0/setup.py` & `automizor-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from automizor import version
 
 setup(
     name="automizor",
     version=version,
     description="Python Automizor framework",
-    url="https://github.com/automizor/automizor",
+    url="https://github.com/automizor/automizor-python",
     author="Christian Fischer",
     author_email="christian@automizor.io",
     license="Apache License",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Other Audience",
         "License :: OSI Approved :: Apache Software License",
```

