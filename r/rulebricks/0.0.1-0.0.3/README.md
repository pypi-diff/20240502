# Comparing `tmp/rulebricks-0.0.1.tar.gz` & `tmp/rulebricks-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rulebricks-0.0.1.tar", max compression
+gzip compressed data, was "rulebricks-0.0.3.tar", max compression
```

## Comparing `rulebricks-0.0.1.tar` & `rulebricks-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1022 2024-05-01 23:17:55.155350 rulebricks-0.0.1/README.md
--rw-r--r--   0        0        0      428 2024-05-01 23:17:55.155350 rulebricks-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      510 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/__init__.py
--rw-r--r--   0        0        0     1485 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/client.py
--rw-r--r--   0        0        0      519 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/core/api_error.py
--rw-r--r--   0        0        0      968 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      221 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/errors/bad_request_error.py
--rw-r--r--   0        0        0      252 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/errors/internal_server_error.py
--rw-r--r--   0        0        0      404 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/resources/flows/__init__.py
--rw-r--r--   0        0        0     4253 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/resources/flows/client.py
--rw-r--r--   0        0        0      351 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/resources/rules/__init__.py
--rw-r--r--   0        0        0    16686 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/resources/rules/client.py
--rw-r--r--   0        0        0      473 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/resources/rules/types/__init__.py
--rw-r--r--   0        0        0     1700 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/resources/rules/types/list_response_item.py
--rw-r--r--   0        0        0     1870 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
--rw-r--r--   0        0        0     1878 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
--rw-r--r--   0        0        0     1675 2024-05-01 23:17:55.155350 rulebricks-0.0.1/src/rulebricks/resources/rules/types/usage_response.py
--rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 rulebricks-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2430 2024-05-02 00:13:17.585411 rulebricks-0.0.3/README.md
+-rw-r--r--   0        0        0      428 2024-05-02 00:13:17.585411 rulebricks-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2038 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/client.py
+-rw-r--r--   0        0        0      519 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/api_error.py
+-rw-r--r--   0        0        0      968 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      221 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/errors/bad_request_error.py
+-rw-r--r--   0        0        0      252 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/errors/internal_server_error.py
+-rw-r--r--   0        0        0      404 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/flows/__init__.py
+-rw-r--r--   0        0        0     4115 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/flows/client.py
+-rw-r--r--   0        0        0      351 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/__init__.py
+-rw-r--r--   0        0        0    15996 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/client.py
+-rw-r--r--   0        0        0      473 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/types/__init__.py
+-rw-r--r--   0        0        0     1700 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item.py
+-rw-r--r--   0        0        0     1870 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
+-rw-r--r--   0        0        0     1878 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
+-rw-r--r--   0        0        0     1675 2024-05-02 00:13:17.585411 rulebricks-0.0.3/src/rulebricks/resources/rules/types/usage_response.py
+-rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 rulebricks-0.0.3/PKG-INFO
```

### Comparing `rulebricks-0.0.1/src/rulebricks/client.py` & `rulebricks-0.0.3/src/rulebricks/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.1/src/rulebricks/core/__init__.py` & `rulebricks-0.0.3/src/rulebricks/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.1/src/rulebricks/core/client_wrapper.py` & `rulebricks-0.0.3/src/rulebricks/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.1/src/rulebricks/core/datetime_utils.py` & `rulebricks-0.0.3/src/rulebricks/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.1/src/rulebricks/core/jsonable_encoder.py` & `rulebricks-0.0.3/src/rulebricks/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.1/src/rulebricks/resources/flows/client.py` & `rulebricks-0.0.3/src/rulebricks/resources/flows/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,21 +28,20 @@
         Execute a flow by its slug.
 
         Parameters:
             - slug: str. The unique identifier for the flow.
 
             - request: typing.Dict[str, typing.Any].
         ---
-        from rulebricks.client import RulebricksApi
+        import rulebricks as rb
 
-        client = RulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        client.flows.execute(
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        rb.flows.execute(
             slug="slug",
             request={"name": "John Doe", "age": 30, "email": "jdoe@acme.co"},
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/flow/{slug}"),
@@ -72,21 +71,20 @@
         Execute a flow by its slug.
 
         Parameters:
             - slug: str. The unique identifier for the flow.
 
             - request: typing.Dict[str, typing.Any].
         ---
-        from rulebricks.client import AsyncRulebricksApi
+        import rulebricks as rb
 
-        client = AsyncRulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        await client.flows.execute(
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        await rb.async_api.flows.execute(
             slug="slug",
             request={"name": "John Doe", "age": 30, "email": "jdoe@acme.co"},
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/flow/{slug}"),
```

### Comparing `rulebricks-0.0.1/src/rulebricks/resources/rules/client.py` & `rulebricks-0.0.3/src/rulebricks/resources/rules/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,21 +30,20 @@
         Executes a single rule identified by a unique slug. The request and response formats are dynamic, dependent on the rule configuration.
 
         Parameters:
             - slug: str. The unique identifier for the rule.
 
             - request: typing.Dict[str, typing.Any].
         ---
-        from rulebricks.client import RulebricksApi
+        import rulebricks as rb
 
-        client = RulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        client.rules.solve(
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        rb.rules.solve(
             slug="slug",
             request={"name": "John Doe", "age": 30, "email": "jdoe@acme.co"},
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/solve/{slug}"),
@@ -71,21 +70,20 @@
         Executes a particular rule against multiple request data payloads provided in a list.
 
         Parameters:
             - slug: str. The unique identifier of the rule to execute against all payloads.
 
             - request: typing.List[typing.Dict[str, typing.Any]].
         ---
-        from rulebricks.client import RulebricksApi
+        import rulebricks as rb
 
-        client = RulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        client.rules.bulk_solve(
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        rb.rules.bulk_solve(
             slug="slug",
             request=[
                 {"name": "John Doe", "age": 30, "email": "jdoe@acme.co"},
                 {"name": "Jane Doe", "age": 28, "email": "jane@example.com"},
             ],
         )
         """
@@ -111,21 +109,20 @@
     def parallel_solve(self, *, request: typing.Dict[str, typing.Any]) -> typing.Dict[str, typing.Any]:
         """
         Executes multiple rules in parallel based on a provided mapping of rule slugs to payloads.
 
         Parameters:
             - request: typing.Dict[str, typing.Any].
         ---
-        from rulebricks.client import RulebricksApi
+        import rulebricks as rb
 
-        client = RulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        client.rules.parallel_solve(
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        rb.rules.parallel_solve(
             request={
                 "eligibility": {
                     "rule": "1ef03ms",
                     "name": "John Doe",
                     "age": 30,
                     "email": "jdoe@acme.co",
                 },
@@ -158,21 +155,20 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list(self) -> typing.List[ListResponseItem]:
         """
         List all rules in the organization.
 
         ---
-        from rulebricks.client import RulebricksApi
+        import rulebricks as rb
 
-        client = RulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        client.rules.list()
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        rb.rules.list()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/list"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -185,21 +181,20 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def usage(self) -> UsageResponse:
         """
         Get the rule execution usage of your organization.
 
         ---
-        from rulebricks.client import RulebricksApi
+        import rulebricks as rb
 
-        client = RulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        client.rules.usage()
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        rb.rules.usage()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/usage"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -221,21 +216,20 @@
         Executes a single rule identified by a unique slug. The request and response formats are dynamic, dependent on the rule configuration.
 
         Parameters:
             - slug: str. The unique identifier for the rule.
 
             - request: typing.Dict[str, typing.Any].
         ---
-        from rulebricks.client import AsyncRulebricksApi
+        import rulebricks as rb
 
-        client = AsyncRulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        await client.rules.solve(
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        await rb.async_api.rules.solve(
             slug="slug",
             request={"name": "John Doe", "age": 30, "email": "jdoe@acme.co"},
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/v1/solve/{slug}"),
@@ -262,21 +256,20 @@
         Executes a particular rule against multiple request data payloads provided in a list.
 
         Parameters:
             - slug: str. The unique identifier of the rule to execute against all payloads.
 
             - request: typing.List[typing.Dict[str, typing.Any]].
         ---
-        from rulebricks.client import AsyncRulebricksApi
+        import rulebricks as rb
 
-        client = AsyncRulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        await client.rules.bulk_solve(
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        await rb.async_api.rules.bulk_solve(
             slug="slug",
             request=[
                 {"name": "John Doe", "age": 30, "email": "jdoe@acme.co"},
                 {"name": "Jane Doe", "age": 28, "email": "jane@example.com"},
             ],
         )
         """
@@ -302,21 +295,20 @@
     async def parallel_solve(self, *, request: typing.Dict[str, typing.Any]) -> typing.Dict[str, typing.Any]:
         """
         Executes multiple rules in parallel based on a provided mapping of rule slugs to payloads.
 
         Parameters:
             - request: typing.Dict[str, typing.Any].
         ---
-        from rulebricks.client import AsyncRulebricksApi
+        import rulebricks as rb
 
-        client = AsyncRulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        await client.rules.parallel_solve(
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        await rb.async_api.rules.parallel_solve(
             request={
                 "eligibility": {
                     "rule": "1ef03ms",
                     "name": "John Doe",
                     "age": 30,
                     "email": "jdoe@acme.co",
                 },
@@ -349,21 +341,20 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list(self) -> typing.List[ListResponseItem]:
         """
         List all rules in the organization.
 
         ---
-        from rulebricks.client import AsyncRulebricksApi
+        import rulebricks as rb
 
-        client = AsyncRulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        await client.rules.list()
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        await rb.async_api.rules.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/list"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -376,21 +367,20 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def usage(self) -> UsageResponse:
         """
         Get the rule execution usage of your organization.
 
         ---
-        from rulebricks.client import AsyncRulebricksApi
+        import rulebricks as rb
 
-        client = AsyncRulebricksApi(
-            api_key="YOUR_API_KEY",
-            base_url="https://yourhost.com/path/to/api",
-        )
-        await client.rules.usage()
+        # Set the API key
+        rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
+
+        await rb.async_api.rules.usage()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v1/usage"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
```

### Comparing `rulebricks-0.0.1/src/rulebricks/resources/rules/types/list_response_item.py` & `rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.1/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py` & `rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.1/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py` & `rulebricks-0.0.3/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.0.1/src/rulebricks/resources/rules/types/usage_response.py` & `rulebricks-0.0.3/src/rulebricks/resources/rules/types/usage_response.py`

 * *Files identical despite different names*

