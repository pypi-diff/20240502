# Comparing `tmp/zodchy_fastapi-0.2.4.tar.gz` & `tmp/zodchy_fastapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_fastapi-0.2.4.tar", max compression
+gzip compressed data, was "zodchy_fastapi-0.3.0.tar", max compression
```

## Comparing `zodchy_fastapi-0.2.4.tar` & `zodchy_fastapi-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0       16 2024-04-13 13:32:10.912348 zodchy_fastapi-0.2.4/README.md
--rw-r--r--   0        0        0      467 2024-04-30 09:47:52.491302 zodchy_fastapi-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       72 2024-04-29 11:12:28.828914 zodchy_fastapi-0.2.4/zodchy_fastapi/__init__.py
--rw-r--r--   0        0        0       40 2024-04-29 15:35:10.919519 zodchy_fastapi-0.2.4/zodchy_fastapi/adapters/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-29 11:12:28.953487 zodchy_fastapi-0.2.4/zodchy_fastapi/adapters/query.py
--rw-r--r--   0        0        0      293 2024-04-29 11:12:28.838554 zodchy_fastapi-0.2.4/zodchy_fastapi/contracts/__init__.py
--rw-r--r--   0        0        0      618 2024-04-28 15:36:57.385697 zodchy_fastapi-0.2.4/zodchy_fastapi/contracts/request.py
--rw-r--r--   0        0        0     1316 2024-04-30 09:47:26.103903 zodchy_fastapi-0.2.4/zodchy_fastapi/contracts/response.py
--rw-r--r--   0        0        0      173 2024-04-29 11:12:28.960486 zodchy_fastapi-0.2.4/zodchy_fastapi/contracts/tools.py
--rw-r--r--   0        0        0     1209 2024-04-11 07:57:07.719841 zodchy_fastapi-0.2.4/zodchy_fastapi/handlers.py
--rw-r--r--   0        0        0      784 2024-04-11 07:57:07.719982 zodchy_fastapi-0.2.4/zodchy_fastapi/router.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 zodchy_fastapi-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-13 13:32:10.912348 zodchy_fastapi-0.3.0/README.md
+-rw-r--r--   0        0        0      466 2024-05-02 14:57:10.853001 zodchy_fastapi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      129 2024-05-02 14:57:10.856896 zodchy_fastapi-0.3.0/zodchy_fastapi/__init__.py
+-rw-r--r--   0        0        0      232 2024-05-02 13:34:11.382181 zodchy_fastapi-0.3.0/zodchy_fastapi/contracts.py
+-rw-r--r--   0        0        0       90 2024-05-02 13:34:11.371712 zodchy_fastapi-0.3.0/zodchy_fastapi/middleware/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-02 13:34:11.364678 zodchy_fastapi-0.3.0/zodchy_fastapi/middleware/handlers.py
+-rw-r--r--   0        0        0       84 2024-05-02 13:34:11.310855 zodchy_fastapi-0.3.0/zodchy_fastapi/request/__init__.py
+-rw-r--r--   0        0        0     2061 2024-05-02 14:57:10.836323 zodchy_fastapi-0.3.0/zodchy_fastapi/request/adapter.py
+-rw-r--r--   0        0        0      553 2024-05-02 13:10:41.930229 zodchy_fastapi-0.3.0/zodchy_fastapi/request/schema.py
+-rw-r--r--   0        0        0       79 2024-05-02 13:34:11.354249 zodchy_fastapi-0.3.0/zodchy_fastapi/response/__init__.py
+-rw-r--r--   0        0        0     1399 2024-05-02 13:34:11.421798 zodchy_fastapi-0.3.0/zodchy_fastapi/response/adapter.py
+-rw-r--r--   0        0        0      577 2024-05-02 13:10:41.934281 zodchy_fastapi-0.3.0/zodchy_fastapi/response/schema.py
+-rw-r--r--   0        0        0       61 2024-05-02 13:34:11.359388 zodchy_fastapi-0.3.0/zodchy_fastapi/routing/__init__.py
+-rw-r--r--   0        0        0      766 2024-05-02 13:34:11.357096 zodchy_fastapi-0.3.0/zodchy_fastapi/routing/schema.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 zodchy_fastapi-0.3.0/PKG-INFO
```

### Comparing `zodchy_fastapi-0.2.4/zodchy_fastapi/adapters/query.py` & `zodchy_fastapi-0.3.0/zodchy_fastapi/request/adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,69 @@
+import dataclasses
+import typing
+import collections.abc
+
 from zodchy import codex
 
-from .. import contracts
+from .schema import RequestModel, FilterParam
+
+T = typing.TypeVar('T')
 
+AdapterContract = collections.abc.Callable[[RequestModel, type[T]], T]
 
-class QueryAdapter:
+
+class Adapter:
     def __init__(
         self,
-        notation_parser: codex.query.NotationParser
+        query_notation_parser: codex.query.NotationParser
     ):
-        self._notation_parser = notation_parser
+        self._query_notation_parser = query_notation_parser
 
     def __call__(
         self,
-        request_model: contracts.RequestModel,
-        target_model: type[codex.cqea.Query]
+        request_model: RequestModel,
+        target_model: type[codex.cqea.Query] | type[codex.cqea.Command]
     ) -> codex.cqea.Query:
+        if codex.cqea.Query in target_model.__mro__:
+            return self._fill_query_model(request_model, target_model)
+        elif codex.cqea.Command in target_model.__mro__:
+            return self._fill_command_model(request_model, target_model)
+        else:
+            raise TypeError("Invalid target model type")
+
+    def _fill_query_model(
+        self,
+        request_model: RequestModel,
+        target_model: type[codex.cqea.Query]
+    ):
         return target_model(
             **{
-                t[0]: t[1] for t in self._notation_parser(
+                t[0]: t[1] for t in self._query_notation_parser(
                     request_model.model_dump(exclude_none=True, exclude_unset=True),
                     self._types_map(request_model)
                 )
             }
         )
 
     @staticmethod
-    def _types_map(payload_model: contracts.RequestModel):
+    def _fill_command_model(
+        request_model: RequestModel,
+        target_model: type[codex.cqea.Command]
+    ):
+        return target_model(
+            **{
+                k: v
+                for k, v
+                in request_model.model_dump(exclude_unset=True).items()
+                if k in {f.name for f in dataclasses.fields(target_model)}
+            }
+        )
+
+    @staticmethod
+    def _types_map(payload_model: RequestModel):
         result = {}
         for field_name, field_info in payload_model.model_fields.items():
             for e in field_info.metadata:
-                if isinstance(contracts.request.FilterParam, e):
+                if isinstance(e, FilterParam):
                     result[field_name] = e.type
                     break
         return result
```

### Comparing `zodchy_fastapi-0.2.4/zodchy_fastapi/handlers.py` & `zodchy_fastapi-0.3.0/zodchy_fastapi/middleware/handlers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 import collections.abc
 
 import fastapi
 
+from .. import contracts
+
 
 def generic_exception_handler(
-    request: fastapi.Request,
+    request: contracts.Request,
     exc: Exception
 ):
-    return fastapi.responses.ORJSONResponse(
-        status_code=500,
-        content={
-            "data": {
-                "code": 500,
-                "message": "Unknown exception",
-                "details": str(exc)
+    return request.app.response_adapter(
+        dict(
+            status_code=500,
+            content={
+                "data": {
+                    "code": 500,
+                    "message": "Unknown exception",
+                    "details": str(exc)
+                }
             }
-        }
+        )
     )
 
 
 def validation_exception_handler(
-    request: fastapi.Request,
+    request: contracts.Request,
     exc: fastapi.exceptions.ValidationException
 ):
     details = {}
     for e in exc.errors():
         details = _merge(details, _nestify(e['loc'], e['msg']))
-    return fastapi.responses.ORJSONResponse(
-        status_code=422,
-        content={
-            "data": {
-                "code": 422,
-                "message": "Validation error",
-                "details": details
+    return request.app.response_adapter(
+        dict(
+            status_code=422,
+            content={
+                "data": {
+                    "code": 422,
+                    "message": "Validation error",
+                    "details": details
+                }
             }
-        }
+        )
     )
 
 
 def _nestify(data: collections.abc.Sequence[str] | str, value: str):
     if len(data) > 1:
         value = _nestify(data[1:], value)
     return {
```

### Comparing `zodchy_fastapi-0.2.4/PKG-INFO` & `zodchy_fastapi-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zodchy-fastapi
-Version: 0.2.4
+Version: 0.3.0
 Summary: Collection of tools to integrate fastapi to zodchy architecture
 Home-page: https://github.com/smairon/zodchy-fastapi
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

