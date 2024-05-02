# Comparing `tmp/rulebricks-0.0.3.tar.gz` & `tmp/rulebricks-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rulebricks-0.0.3.tar", max compression
+gzip compressed data, was "rulebricks-0.0.4.tar", max compression
```

## Comparing `rulebricks-0.0.3.tar` & `rulebricks-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2430 2024-05-02 00:13:17.585411 rulebricks-0.0.3/README.md
--rw-r--r--   0        0        0      428 2024-05-02 00:13:17.585411 rulebricks-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2038 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/__init__.py
--rw-r--r--   0        0        0     1485 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/client.py
--rw-r--r--   0        0        0      519 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/api_error.py
--rw-r--r--   0        0        0      968 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      221 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/errors/bad_request_error.py
--rw-r--r--   0        0        0      252 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/errors/internal_server_error.py
--rw-r--r--   0        0        0      404 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/flows/__init__.py
--rw-r--r--   0        0        0     4115 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/flows/client.py
--rw-r--r--   0        0        0      351 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/__init__.py
--rw-r--r--   0        0        0    15996 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/client.py
--rw-r--r--   0        0        0      473 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/types/__init__.py
--rw-r--r--   0        0        0     1700 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item.py
--rw-r--r--   0        0        0     1870 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
--rw-r--r--   0        0        0     1878 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
--rw-r--r--   0        0        0     1675 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/types/usage_response.py
--rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 rulebricks-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2526 2024-05-02 00:38:29.086518 rulebricks-0.0.4/README.md
+-rw-r--r--   0        0        0      428 2024-05-02 00:38:29.086518 rulebricks-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2073 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/client.py
+-rw-r--r--   0        0        0      519 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/core/api_error.py
+-rw-r--r--   0        0        0      968 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      221 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/errors/bad_request_error.py
+-rw-r--r--   0        0        0      252 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/errors/internal_server_error.py
+-rw-r--r--   0        0        0      404 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/resources/flows/__init__.py
+-rw-r--r--   0        0        0     4115 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/resources/flows/client.py
+-rw-r--r--   0        0        0      351 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/resources/rules/__init__.py
+-rw-r--r--   0        0        0    15996 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/resources/rules/client.py
+-rw-r--r--   0        0        0      473 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/resources/rules/types/__init__.py
+-rw-r--r--   0        0        0     1700 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/resources/rules/types/list_response_item.py
+-rw-r--r--   0        0        0     1870 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
+-rw-r--r--   0        0        0     1878 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
+-rw-r--r--   0        0        0     1675 2024-05-02 00:38:29.086518 rulebricks-0.0.4/src/rulebricks/resources/rules/types/usage_response.py
+-rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 rulebricks-0.0.4/PKG-INFO
```

### Comparing `rulebricks-0.0.3/README.md` & `rulebricks-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Rulebricks – Python SDK
+[![pypi](https://img.shields.io/pypi/v/flatfile.svg)](https://pypi.python.org/pypi/rulebricks)
+
 
 ## Documentation
 
 API reference documentation is available [here](https://rulebricks.com/docs).
 
 ## Installation
```

### Comparing `rulebricks-0.0.3/src/rulebricks/__init__.py` & `rulebricks-0.0.4/src/rulebricks/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 # This file was auto-generated by Fern from our API Definition.
+from typing import Optional
 from .client import RulebricksApi, AsyncRulebricksApi
 from .errors import BadRequestError, InternalServerError
 from .resources import (
     ListResponseItem,
     ListResponseItemRequestSchemaItem,
     ListResponseItemResponseSchemaItem,
     UsageResponse,
     flows,
     rules,
 )
 
-# Configuration to store API key and URL
 class Config:
-    api_key = None
-    base_url = "https://rulebricks.com"
+    api_key: Optional[str] = None
+    base_url: str = "https://rulebricks.com"
 
-def set_api_key(api_key):
+def set_api_key(api_key: str) -> None:
     Config.api_key = api_key
 
-def set_instance_url(base_url):
+def set_instance_url(base_url: str) -> None:
     Config.base_url = base_url
 
-# Synchronous API access setup
-_api_instance = None
-def get_api_instance():
-    global _api_instance
-    if _api_instance is None:
-        if Config.api_key is None:
-            raise ValueError("API key not set. Use set_api_key() to initialize.")
-        _api_instance = RulebricksApi(base_url=Config.base_url, api_key=Config.api_key)
-    return _api_instance
-
-def __getattr__(name):
-    return getattr(get_api_instance(), name)
-
-# Asynchronous API access setup
-_async_api_instance = None
-async def get_async_api_instance():
-    global _async_api_instance
-    if _async_api_instance is None:
-        if Config.api_key is None:
-            raise ValueError("API key not set. Use set_api_key() to initialize.")
-        _async_api_instance = AsyncRulebricksApi(base_url=Config.base_url, api_key=Config.api_key)
-    return _async_api_instance
+class APIManager:
+    _instance: Optional[RulebricksApi] = None
+    _async_instance: Optional[AsyncRulebricksApi] = None
+
+    @staticmethod
+    def get_api() -> RulebricksApi:
+        if APIManager._instance is None:
+            if Config.api_key is None:
+                raise ValueError("API key not set. Please set the API key first.")
+            APIManager._instance = RulebricksApi(base_url=Config.base_url, api_key=Config.api_key)
+        return APIManager._instance
+
+    @staticmethod
+    async def get_async_api() -> AsyncRulebricksApi:
+        if APIManager._async_instance is None:
+            if Config.api_key is None:
+                raise ValueError("API key not set. Please set the API key first.")
+            APIManager._async_instance = AsyncRulebricksApi(base_url=Config.base_url, api_key=Config.api_key)
+        return APIManager._async_instance
 
+# Asynchronous API access
 class AsyncAPI:
     def __getattr__(self, name):
         async def async_method(*args, **kwargs):
-            instance = await get_async_api_instance()
-            func = getattr(instance, name)
+            api = await APIManager.get_async_api()
+            func = getattr(api, name)
             return await func(*args, **kwargs)
         return async_method
 
-# Create a single instance for async access
 async_api = AsyncAPI()
 
+
 __all__ = [
     "BadRequestError",
     "InternalServerError",
     "ListResponseItem",
     "ListResponseItemRequestSchemaItem",
     "ListResponseItemResponseSchemaItem",
     "UsageResponse",
```

### Comparing `rulebricks-0.0.3/src/rulebricks/client.py` & `rulebricks-0.0.4/src/rulebricks/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.3/src/rulebricks/core/__init__.py` & `rulebricks-0.0.4/src/rulebricks/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.3/src/rulebricks/core/client_wrapper.py` & `rulebricks-0.0.4/src/rulebricks/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.3/src/rulebricks/core/datetime_utils.py` & `rulebricks-0.0.4/src/rulebricks/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.3/src/rulebricks/core/jsonable_encoder.py` & `rulebricks-0.0.4/src/rulebricks/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.3/src/rulebricks/resources/flows/client.py` & `rulebricks-0.0.4/src/rulebricks/resources/flows/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.3/src/rulebricks/resources/rules/client.py` & `rulebricks-0.0.4/src/rulebricks/resources/rules/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item.py` & `rulebricks-0.0.4/src/rulebricks/resources/rules/types/list_response_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py` & `rulebricks-0.0.4/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py` & `rulebricks-0.0.4/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.3/src/rulebricks/resources/rules/types/usage_response.py` & `rulebricks-0.0.4/src/rulebricks/resources/rules/types/usage_response.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.3/PKG-INFO` & `rulebricks-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: rulebricks
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.21.2)
 Requires-Dist: pydantic (>=1.9.2)
 Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # Rulebricks – Python SDK
+[![pypi](https://img.shields.io/pypi/v/flatfile.svg)](https://pypi.python.org/pypi/rulebricks)
+
 
 ## Documentation
 
 API reference documentation is available [here](https://rulebricks.com/docs).
 
 ## Installation
```

