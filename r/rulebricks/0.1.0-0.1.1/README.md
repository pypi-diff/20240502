# Comparing `tmp/rulebricks-0.1.0.tar.gz` & `tmp/rulebricks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rulebricks-0.1.0.tar", max compression
+gzip compressed data, was "rulebricks-0.1.1.tar", max compression
```

## Comparing `rulebricks-0.1.0.tar` & `rulebricks-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2526 2024-05-02 03:18:54.857723 rulebricks-0.1.0/README.md
--rw-r--r--   0        0        0      428 2024-05-02 03:18:54.857723 rulebricks-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3366 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/__init__.py
--rw-r--r--   0        0        0     1485 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/client.py
--rw-r--r--   0        0        0      519 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/core/api_error.py
--rw-r--r--   0        0        0      968 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      221 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/errors/bad_request_error.py
--rw-r--r--   0        0        0      252 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/errors/internal_server_error.py
--rw-r--r--   0        0        0      404 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/resources/flows/__init__.py
--rw-r--r--   0        0        0     4115 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/resources/flows/client.py
--rw-r--r--   0        0        0      351 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/resources/rules/__init__.py
--rw-r--r--   0        0        0    15996 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/resources/rules/client.py
--rw-r--r--   0        0        0      473 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/resources/rules/types/__init__.py
--rw-r--r--   0        0        0     1700 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/resources/rules/types/list_response_item.py
--rw-r--r--   0        0        0     1870 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
--rw-r--r--   0        0        0     1878 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
--rw-r--r--   0        0        0     1675 2024-05-02 03:18:54.857723 rulebricks-0.1.0/src/rulebricks/resources/rules/types/usage_response.py
--rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 rulebricks-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2526 2024-05-02 03:28:43.536439 rulebricks-0.1.1/README.md
+-rw-r--r--   0        0        0      428 2024-05-02 03:28:43.536439 rulebricks-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2759 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/client.py
+-rw-r--r--   0        0        0      519 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/api_error.py
+-rw-r--r--   0        0        0      968 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      221 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/errors/bad_request_error.py
+-rw-r--r--   0        0        0      252 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/errors/internal_server_error.py
+-rw-r--r--   0        0        0      404 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/flows/__init__.py
+-rw-r--r--   0        0        0     4115 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/flows/client.py
+-rw-r--r--   0        0        0      351 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/__init__.py
+-rw-r--r--   0        0        0    15996 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/client.py
+-rw-r--r--   0        0        0      473 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/types/__init__.py
+-rw-r--r--   0        0        0     1700 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item.py
+-rw-r--r--   0        0        0     1870 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
+-rw-r--r--   0        0        0     1878 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
+-rw-r--r--   0        0        0     1675 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/types/usage_response.py
+-rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 rulebricks-0.1.1/PKG-INFO
```

### Comparing `rulebricks-0.1.0/README.md` & `rulebricks-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/src/rulebricks/__init__.py` & `rulebricks-0.1.1/src/rulebricks/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,15 @@
 from typing import Optional
 from .client import RulebricksApi, AsyncRulebricksApi
 from .errors import BadRequestError, InternalServerError
-from .resources import (
-    ListResponseItem,
-    ListResponseItemRequestSchemaItem,
-    ListResponseItemResponseSchemaItem,
-    UsageResponse
-)
-
-# rulebricks/__init__.py
-
-import typing
-from .client import RulebricksApi, AsyncRulebricksApi
 from .resources.rules.client import RulesClient, AsyncRulesClient
 from .resources.flows.client import FlowsClient, AsyncFlowsClient
 
-# Configuration to hold API details
 class Config:
-    api_key: typing.Optional[str] = None
+    api_key: Optional[str] = None
     base_url: str = "https://rulebricks.com"
     timeout: float = 60
 
 def set_api_key(api_key: str) -> None:
     Config.api_key = api_key
     APIManager.reset_instances()
 
@@ -29,18 +17,17 @@
     Config.base_url = base_url
     APIManager.reset_instances()
 
 def set_timeout(timeout: float) -> None:
     Config.timeout = timeout
     APIManager.reset_instances()
 
-# API Manager for handling API instances
 class APIManager:
-    _instance: typing.Optional[RulebricksApi] = None
-    _async_instance: typing.Optional[AsyncRulebricksApi] = None
+    _instance: Optional[RulebricksApi] = None
+    _async_instance: Optional[AsyncRulebricksApi] = None
 
     @staticmethod
     def reset_instances():
         APIManager._instance = None
         APIManager._async_instance = None
 
     @staticmethod
@@ -49,15 +36,15 @@
             if Config.api_key is None:
                 raise ValueError("API key not set. Please set the API key first.")
             APIManager._instance = RulebricksApi(
                 base_url=Config.base_url,
                 api_key=Config.api_key,
                 timeout=Config.timeout
             )
-        assert APIManager._instance is not None, "Instance of RulebricksApi should not be None"
+        assert APIManager._instance is not None, "Instance of AsyncRulebricksApi should not be None"
         return APIManager._instance
 
     @staticmethod
     async def get_async_api() -> AsyncRulebricksApi:
         if APIManager._async_instance is None:
             if Config.api_key is None:
                 raise ValueError("API key not set. Please set the API key first.")
@@ -65,38 +52,37 @@
                 base_url=Config.base_url,
                 api_key=Config.api_key,
                 timeout=Config.timeout
             )
         assert APIManager._async_instance is not None, "Instance of AsyncRulebricksApi should not be None"
         return APIManager._async_instance
 
-# Default API access through the root of the module
-def __getattr__(name: str):
-    api = APIManager.get_api()
-    if hasattr(api, name):
-        return getattr(api, name)
-    raise AttributeError(f"'RulebricksApi' object has no attribute '{name}'")
+# Synchronous API
+rules = APIManager.get_api().rules
+flows = APIManager.get_api().flows
 
-# Asynchronous API access
+# Asynchronous API
 class AsyncAPI:
-    def __getattr__(self, name: str):
-        async def async_method(*args, **kwargs):
-            api = await APIManager.get_async_api()
-            if hasattr(api, name):
-                func = getattr(api, name)
-                return await func(*args, **kwargs)
-            raise AttributeError(f"'AsyncRulebricksApi' object has no attribute '{name}'")
-        return async_method
+    @property
+    async def rules(self) -> AsyncRulesClient:
+        return (await APIManager.get_async_api()).rules
+
+    @property
+    async def flows(self) -> AsyncFlowsClient:
+        return (await APIManager.get_async_api()).flows
 
 async_api = AsyncAPI()
 
 __all__ = [
     "BadRequestError",
     "InternalServerError",
     "ListResponseItem",
     "ListResponseItemRequestSchemaItem",
     "ListResponseItemResponseSchemaItem",
     "UsageResponse",
     "async_api",
     "set_api_key",
     "set_instance_url",
-]
+    "set_timeout",
+    "rules",
+    "flows",
+]
```

### Comparing `rulebricks-0.1.0/src/rulebricks/client.py` & `rulebricks-0.1.1/src/rulebricks/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/src/rulebricks/core/__init__.py` & `rulebricks-0.1.1/src/rulebricks/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/src/rulebricks/core/client_wrapper.py` & `rulebricks-0.1.1/src/rulebricks/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/src/rulebricks/core/datetime_utils.py` & `rulebricks-0.1.1/src/rulebricks/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/src/rulebricks/core/jsonable_encoder.py` & `rulebricks-0.1.1/src/rulebricks/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/src/rulebricks/resources/flows/client.py` & `rulebricks-0.1.1/src/rulebricks/resources/flows/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/src/rulebricks/resources/rules/client.py` & `rulebricks-0.1.1/src/rulebricks/resources/rules/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/src/rulebricks/resources/rules/types/list_response_item.py` & `rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py` & `rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py` & `rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/src/rulebricks/resources/rules/types/usage_response.py` & `rulebricks-0.1.1/src/rulebricks/resources/rules/types/usage_response.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.0/PKG-INFO` & `rulebricks-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rulebricks
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

