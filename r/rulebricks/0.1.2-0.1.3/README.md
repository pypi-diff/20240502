# Comparing `tmp/rulebricks-0.1.2.tar.gz` & `tmp/rulebricks-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rulebricks-0.1.2.tar", max compression
+gzip compressed data, was "rulebricks-0.1.3.tar", max compression
```

## Comparing `rulebricks-0.1.2.tar` & `rulebricks-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2535 2024-05-02 03:51:49.144162 rulebricks-0.1.2/README.md
--rw-r--r--   0        0        0      428 2024-05-02 03:51:49.144162 rulebricks-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3150 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/__init__.py
--rw-r--r--   0        0        0     1485 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/client.py
--rw-r--r--   0        0        0      519 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/api_error.py
--rw-r--r--   0        0        0      968 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      221 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/errors/bad_request_error.py
--rw-r--r--   0        0        0      252 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/errors/internal_server_error.py
--rw-r--r--   0        0        0      404 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/flows/__init__.py
--rw-r--r--   0        0        0     4115 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/flows/client.py
--rw-r--r--   0        0        0      351 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/__init__.py
--rw-r--r--   0        0        0    15996 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/client.py
--rw-r--r--   0        0        0      473 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/types/__init__.py
--rw-r--r--   0        0        0     1700 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item.py
--rw-r--r--   0        0        0     1870 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
--rw-r--r--   0        0        0     1878 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
--rw-r--r--   0        0        0     1675 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/types/usage_response.py
--rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 rulebricks-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2535 2024-05-02 04:00:57.910000 rulebricks-0.1.3/README.md
+-rw-r--r--   0        0        0      428 2024-05-02 04:00:57.910000 rulebricks-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3116 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/client.py
+-rw-r--r--   0        0        0      519 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/core/api_error.py
+-rw-r--r--   0        0        0      968 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      221 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/errors/bad_request_error.py
+-rw-r--r--   0        0        0      252 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/errors/internal_server_error.py
+-rw-r--r--   0        0        0      351 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/resources/flows/__init__.py
+-rw-r--r--   0        0        0     4124 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/resources/flows/client.py
+-rw-r--r--   0        0        0      351 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/resources/rules/__init__.py
+-rw-r--r--   0        0        0    16041 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/resources/rules/client.py
+-rw-r--r--   0        0        0      473 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/resources/rules/types/__init__.py
+-rw-r--r--   0        0        0     1700 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/resources/rules/types/list_response_item.py
+-rw-r--r--   0        0        0     1870 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
+-rw-r--r--   0        0        0     1878 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
+-rw-r--r--   0        0        0     1675 2024-05-02 04:00:57.914000 rulebricks-0.1.3/src/rulebricks/resources/rules/types/usage_response.py
+-rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 rulebricks-0.1.3/PKG-INFO
```

### Comparing `rulebricks-0.1.2/README.md` & `rulebricks-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.2/src/rulebricks/__init__.py` & `rulebricks-0.1.3/src/rulebricks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 base_url=Config.base_url,
                 api_key=Config.api_key,
                 timeout=Config.timeout
             )
         return APIManager._instance
 
     @staticmethod
-    async def get_async_api() -> AsyncRulebricksApi:
+    def get_async_api() -> AsyncRulebricksApi:
         if APIManager._async_instance is None:
             if Config.api_key is None:
                 raise ValueError("API key not set. Please set the API key first.")
             APIManager._async_instance = AsyncRulebricksApi(
                 base_url=Config.base_url,
                 api_key=Config.api_key,
                 timeout=Config.timeout
@@ -74,20 +74,20 @@
         return APIManager.get_api().flows
 
 sync_api = SyncAPI()
 
 # Asynchronous API with type hints and lazy loading
 class AsyncAPI:
     @property
-    async def rules(self) -> AsyncRulesClient:
-        return (await APIManager.get_async_api()).rules
+    def rules(self) -> AsyncRulesClient:
+        return APIManager.get_async_api().rules
 
     @property
-    async def flows(self) -> AsyncFlowsClient:
-        return (await APIManager.get_async_api()).flows
+    def flows(self) -> AsyncFlowsClient:
+        return APIManager.get_async_api().flows
 
 async_api = AsyncAPI()
 
 __all__ = [
     "BadRequestError",
     "InternalServerError",
     "async_api",
```

### Comparing `rulebricks-0.1.2/src/rulebricks/client.py` & `rulebricks-0.1.3/src/rulebricks/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.2/src/rulebricks/core/__init__.py` & `rulebricks-0.1.3/src/rulebricks/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.2/src/rulebricks/core/client_wrapper.py` & `rulebricks-0.1.3/src/rulebricks/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.2/src/rulebricks/core/datetime_utils.py` & `rulebricks-0.1.3/src/rulebricks/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.2/src/rulebricks/core/jsonable_encoder.py` & `rulebricks-0.1.3/src/rulebricks/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.2/src/rulebricks/resources/flows/client.py` & `rulebricks-0.1.3/src/rulebricks/resources/flows/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             - request: typing.Dict[str, typing.Any].
         ---
         import rulebricks as rb
 
         # Set the API key
         rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
 
-        rb.flows.execute(
+        rb.sync_api.flows.execute(
             slug="slug",
             request={"name": "John Doe", "age": 30, "email": "jdoe@acme.co"},
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/flow/{slug}"),
```

### Comparing `rulebricks-0.1.2/src/rulebricks/resources/rules/client.py` & `rulebricks-0.1.3/src/rulebricks/resources/rules/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             - request: typing.Dict[str, typing.Any].
         ---
         import rulebricks as rb
 
         # Set the API key
         rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
 
-        rb.rules.solve(
+        rb.sync_api.rules.solve(
             slug="slug",
             request={"name": "John Doe", "age": 30, "email": "jdoe@acme.co"},
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/solve/{slug}"),
@@ -75,15 +75,15 @@
             - request: typing.List[typing.Dict[str, typing.Any]].
         ---
         import rulebricks as rb
 
         # Set the API key
         rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
 
-        rb.rules.bulk_solve(
+        rb.sync_api.rules.bulk_solve(
             slug="slug",
             request=[
                 {"name": "John Doe", "age": 30, "email": "jdoe@acme.co"},
                 {"name": "Jane Doe", "age": 28, "email": "jane@example.com"},
             ],
         )
         """
@@ -114,15 +114,15 @@
             - request: typing.Dict[str, typing.Any].
         ---
         import rulebricks as rb
 
         # Set the API key
         rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
 
-        rb.rules.parallel_solve(
+        rb.sync_api.rules.parallel_solve(
             request={
                 "eligibility": {
                     "rule": "1ef03ms",
                     "name": "John Doe",
                     "age": 30,
                     "email": "jdoe@acme.co",
                 },
@@ -160,15 +160,15 @@
 
         ---
         import rulebricks as rb
 
         # Set the API key
         rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
 
-        rb.rules.list()
+        rb.sync_api.rules.list()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/list"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -186,15 +186,15 @@
 
         ---
         import rulebricks as rb
 
         # Set the API key
         rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
 
-        rb.rules.usage()
+        rb.sync_api.rules.usage()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/usage"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
```

### Comparing `rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item.py` & `rulebricks-0.1.3/src/rulebricks/resources/rules/types/list_response_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py` & `rulebricks-0.1.3/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py` & `rulebricks-0.1.3/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.2/src/rulebricks/resources/rules/types/usage_response.py` & `rulebricks-0.1.3/src/rulebricks/resources/rules/types/usage_response.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.2/PKG-INFO` & `rulebricks-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rulebricks
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

