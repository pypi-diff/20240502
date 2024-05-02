# Comparing `tmp/rulebricks-0.0.5.tar.gz` & `tmp/rulebricks-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rulebricks-0.0.5.tar", max compression
+gzip compressed data, was "rulebricks-0.0.6.tar", max compression
```

## Comparing `rulebricks-0.0.5.tar` & `rulebricks-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2526 2024-05-02 01:02:32.381071 rulebricks-0.0.5/README.md
--rw-r--r--   0        0        0      428 2024-05-02 01:02:32.381071 rulebricks-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2128 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/__init__.py
--rw-r--r--   0        0        0     1485 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/client.py
--rw-r--r--   0        0        0      519 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/core/api_error.py
--rw-r--r--   0        0        0      968 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      221 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/errors/bad_request_error.py
--rw-r--r--   0        0        0      252 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/errors/internal_server_error.py
--rw-r--r--   0        0        0      404 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/resources/flows/__init__.py
--rw-r--r--   0        0        0     4115 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/resources/flows/client.py
--rw-r--r--   0        0        0      351 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/resources/rules/__init__.py
--rw-r--r--   0        0        0    15996 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/resources/rules/client.py
--rw-r--r--   0        0        0      473 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/resources/rules/types/__init__.py
--rw-r--r--   0        0        0     1700 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/resources/rules/types/list_response_item.py
--rw-r--r--   0        0        0     1870 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
--rw-r--r--   0        0        0     1878 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
--rw-r--r--   0        0        0     1675 2024-05-02 01:02:32.381071 rulebricks-0.0.5/src/rulebricks/resources/rules/types/usage_response.py
--rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 rulebricks-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2526 2024-05-02 02:25:44.674669 rulebricks-0.0.6/README.md
+-rw-r--r--   0        0        0      428 2024-05-02 02:25:44.674669 rulebricks-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2418 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/client.py
+-rw-r--r--   0        0        0      519 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/core/api_error.py
+-rw-r--r--   0        0        0      968 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      221 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/errors/bad_request_error.py
+-rw-r--r--   0        0        0      252 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/errors/internal_server_error.py
+-rw-r--r--   0        0        0      404 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/resources/flows/__init__.py
+-rw-r--r--   0        0        0     4115 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/resources/flows/client.py
+-rw-r--r--   0        0        0      351 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/resources/rules/__init__.py
+-rw-r--r--   0        0        0    15996 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/resources/rules/client.py
+-rw-r--r--   0        0        0      473 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/resources/rules/types/__init__.py
+-rw-r--r--   0        0        0     1700 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/resources/rules/types/list_response_item.py
+-rw-r--r--   0        0        0     1870 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
+-rw-r--r--   0        0        0     1878 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
+-rw-r--r--   0        0        0     1675 2024-05-02 02:25:44.674669 rulebricks-0.0.6/src/rulebricks/resources/rules/types/usage_response.py
+-rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 rulebricks-0.0.6/PKG-INFO
```

### Comparing `rulebricks-0.0.5/README.md` & `rulebricks-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/src/rulebricks/__init__.py` & `rulebricks-0.0.6/src/rulebricks/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,21 @@
-# This file was auto-generated by Fern from our API Definition.
 from typing import Optional
 from .client import RulebricksApi, AsyncRulebricksApi
 from .errors import BadRequestError, InternalServerError
 from .resources import (
     ListResponseItem,
     ListResponseItemRequestSchemaItem,
     ListResponseItemResponseSchemaItem,
     UsageResponse
 )
 
 class Config:
     api_key: Optional[str] = None
     base_url: str = "https://rulebricks.com"
 
-def set_api_key(api_key: str) -> None:
-    Config.api_key = api_key
-
-def set_instance_url(base_url: str) -> None:
-    Config.base_url = base_url
-
 class APIManager:
     _instance: Optional[RulebricksApi] = None
     _async_instance: Optional[AsyncRulebricksApi] = None
 
     @staticmethod
     def get_api() -> RulebricksApi:
         if APIManager._instance is None:
@@ -35,25 +28,32 @@
     async def get_async_api() -> AsyncRulebricksApi:
         if APIManager._async_instance is None:
             if Config.api_key is None:
                 raise ValueError("API key not set. Please set the API key first.")
             APIManager._async_instance = AsyncRulebricksApi(base_url=Config.base_url, api_key=Config.api_key)
         return APIManager._async_instance
 
-# Asynchronous API access
-class AsyncAPI:
-    def __getattr__(self, name):
-        async def async_method(*args, **kwargs):
-            api = await APIManager.get_async_api()
-            func = getattr(api, name)
-            return await func(*args, **kwargs)
-        return async_method
-
 sync_api = APIManager.get_api()
-async_api = AsyncAPI()
+async_api = APIManager.get_async_api()
+
+def set_api_key(api_key: str) -> None:
+    Config.api_key = api_key
+    if Config.api_key is not None:
+        APIManager._instance = RulebricksApi(base_url=Config.base_url, api_key=Config.api_key)
+        APIManager._async_instance = AsyncRulebricksApi(base_url=Config.base_url, api_key=Config.api_key)
+    else:
+        raise ValueError("An API key must be provided.")
+
+def set_instance_url(base_url: str) -> None:
+    Config.base_url = base_url
+    if Config.api_key is not None:
+        APIManager._instance = RulebricksApi(base_url=Config.base_url, api_key=Config.api_key)
+        APIManager._async_instance = AsyncRulebricksApi(base_url=Config.base_url, api_key=Config.api_key)
+    else:
+        raise ValueError("You must set the API key using set_api_key first.")
 
 flows = sync_api.flows
 rules = sync_api.rules
 
 __all__ = [
     "BadRequestError",
     "InternalServerError",
```

### Comparing `rulebricks-0.0.5/src/rulebricks/client.py` & `rulebricks-0.0.6/src/rulebricks/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/src/rulebricks/core/__init__.py` & `rulebricks-0.0.6/src/rulebricks/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/src/rulebricks/core/client_wrapper.py` & `rulebricks-0.0.6/src/rulebricks/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/src/rulebricks/core/datetime_utils.py` & `rulebricks-0.0.6/src/rulebricks/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/src/rulebricks/core/jsonable_encoder.py` & `rulebricks-0.0.6/src/rulebricks/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/src/rulebricks/resources/flows/client.py` & `rulebricks-0.0.6/src/rulebricks/resources/flows/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/src/rulebricks/resources/rules/client.py` & `rulebricks-0.0.6/src/rulebricks/resources/rules/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/src/rulebricks/resources/rules/types/list_response_item.py` & `rulebricks-0.0.6/src/rulebricks/resources/rules/types/list_response_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py` & `rulebricks-0.0.6/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py` & `rulebricks-0.0.6/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/src/rulebricks/resources/rules/types/usage_response.py` & `rulebricks-0.0.6/src/rulebricks/resources/rules/types/usage_response.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.5/PKG-INFO` & `rulebricks-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rulebricks
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

