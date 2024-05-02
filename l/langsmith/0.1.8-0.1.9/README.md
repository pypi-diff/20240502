# Comparing `tmp/langsmith-0.1.8.tar.gz` & `tmp/langsmith-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langsmith-0.1.8.tar", max compression
+gzip compressed data, was "langsmith-0.1.9.tar", max compression
```

## Comparing `langsmith-0.1.8.tar` & `langsmith-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    12164 2024-02-25 02:50:50.330597 langsmith-0.1.8/README.md
--rw-r--r--   0        0        0      559 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/cli/__init__.py
--rw-r--r--   0        0        0     4856 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/cli/docker-compose.yaml
--rw-r--r--   0        0        0    11931 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/cli/main.py
--rw-r--r--   0        0        0      351 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/cli/users.xml
--rw-r--r--   0        0        0   131045 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/client.py
--rw-r--r--   0        0        0      840 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/env/__init__.py
--rw-r--r--   0        0        0     1582 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/env/_git.py
--rw-r--r--   0        0        0     6548 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/env/_runtime_env.py
--rw-r--r--   0        0        0      266 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/evaluation/__init__.py
--rw-r--r--   0        0        0     6253 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/evaluation/evaluator.py
--rw-r--r--   0        0        0     1583 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/evaluation/string_evaluator.py
--rw-r--r--   0        0        0        0 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/py.typed
--rw-r--r--   0        0        0    33940 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/run_helpers.py
--rw-r--r--   0        0        0     8416 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/run_trees.py
--rw-r--r--   0        0        0    18452 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/schemas.py
--rw-r--r--   0        0        0    12511 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/utils.py
--rw-r--r--   0        0        0      157 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/wrappers/__init__.py
--rw-r--r--   0        0        0     6292 2024-02-25 02:50:50.330597 langsmith-0.1.8/langsmith/wrappers/_openai.py
--rw-r--r--   0        0        0     1838 2024-02-25 02:50:50.330597 langsmith-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    13062 1970-01-01 00:00:00.000000 langsmith-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    12164 2024-02-26 20:53:12.563147 langsmith-0.1.9/README.md
+-rw-r--r--   0        0        0      559 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/cli/__init__.py
+-rw-r--r--   0        0        0     4856 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    11931 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/cli/main.py
+-rw-r--r--   0        0        0      351 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/cli/users.xml
+-rw-r--r--   0        0        0   131750 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/client.py
+-rw-r--r--   0        0        0      840 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/env/__init__.py
+-rw-r--r--   0        0        0     1582 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/env/_git.py
+-rw-r--r--   0        0        0     6548 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/env/_runtime_env.py
+-rw-r--r--   0        0        0      266 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/evaluation/__init__.py
+-rw-r--r--   0        0        0     6253 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1583 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0        0 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/py.typed
+-rw-r--r--   0        0        0    33940 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/run_helpers.py
+-rw-r--r--   0        0        0     8416 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/run_trees.py
+-rw-r--r--   0        0        0    18452 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/schemas.py
+-rw-r--r--   0        0        0    12511 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/utils.py
+-rw-r--r--   0        0        0      157 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/wrappers/__init__.py
+-rw-r--r--   0        0        0     6292 2024-02-26 20:53:12.563147 langsmith-0.1.9/langsmith/wrappers/_openai.py
+-rw-r--r--   0        0        0     1838 2024-02-26 20:53:12.563147 langsmith-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    13062 1970-01-01 00:00:00.000000 langsmith-0.1.9/PKG-INFO
```

### Comparing `langsmith-0.1.8/README.md` & `langsmith-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/__init__.py` & `langsmith-0.1.9/langsmith/__init__.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/cli/docker-compose.yaml` & `langsmith-0.1.9/langsmith/cli/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/cli/main.py` & `langsmith-0.1.9/langsmith/cli/main.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/client.py` & `langsmith-0.1.9/langsmith/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -883,15 +883,17 @@
         result = response.json()
         # TODO: Make this more robust server-side
         if "detail" in result and "already exists" in result["detail"]:
             file_name = csv_file if isinstance(csv_file, str) else csv_file[0]
             file_name = file_name.split("/")[-1]
             raise ValueError(f"Dataset {file_name} already exists")
         return ls_schemas.Dataset(
-            **result, _host_url=self._host_url, _tenant_id=self._get_tenant_id()
+            **result,
+            _host_url=self._host_url,
+            _tenant_id=self._get_optional_tenant_id(),
         )
 
     @staticmethod
     def _run_transform(
         run: Union[ls_schemas.Run, dict, ls_schemas.RunLikeDict], update: bool = False
     ) -> dict:
         """Transform the given run object into a dictionary representation.
@@ -1754,26 +1756,37 @@
             endpoint,
             headers={**self._headers, "Content-Type": "application/json"},
             data=_dumps_json(body),
         )
         ls_utils.raise_for_status_with_text(response)
         return ls_schemas.TracerSession(**response.json(), _host_url=self._host_url)
 
-    def _get_tenant_id(self) -> uuid.UUID:
+    def _get_optional_tenant_id(self) -> Optional[uuid.UUID]:
         if self._tenant_id is not None:
             return self._tenant_id
-        response = self._get_with_retries("/sessions", params={"limit": 1})
-        result = response.json()
-        if isinstance(result, list):
-            tracer_session = ls_schemas.TracerSessionResult(
-                **result[0], _host_url=self._host_url
+        try:
+            response = self._get_with_retries("/sessions", params={"limit": 1})
+            result = response.json()
+            if isinstance(result, list) and len(result) > 0:
+                tracer_session = ls_schemas.TracerSessionResult(
+                    **result[0], _host_url=self._host_url
+                )
+                self._tenant_id = tracer_session.tenant_id
+                return self._tenant_id
+        except Exception as e:
+            logger.warning(
+                "Failed to get tenant ID from LangSmith: %s", repr(e), exc_info=True
             )
-            self._tenant_id = tracer_session.tenant_id
-            return self._tenant_id
-        raise ls_utils.LangSmithError("No projects found")
+        return None
+
+    def _get_tenant_id(self) -> uuid.UUID:
+        tenant_id = self._get_optional_tenant_id()
+        if tenant_id is None:
+            raise ls_utils.LangSmithError("No tenant ID found")
+        return tenant_id
 
     @ls_utils.xor_args(("project_id", "project_name"))
     def read_project(
         self,
         *,
         project_id: Optional[str] = None,
         project_name: Optional[str] = None,
@@ -2022,15 +2035,15 @@
             headers={**self._headers, "Content-Type": "application/json"},
             data=dataset.json(),
         )
         ls_utils.raise_for_status_with_text(response)
         return ls_schemas.Dataset(
             **response.json(),
             _host_url=self._host_url,
-            _tenant_id=self._get_tenant_id(),
+            _tenant_id=self._get_optional_tenant_id(),
         )
 
     def has_dataset(
         self, *, dataset_name: Optional[str] = None, dataset_id: Optional[str] = None
     ) -> bool:
         """Check whether a dataset exists in your tenant.
 
@@ -2088,18 +2101,22 @@
         result = response.json()
         if isinstance(result, list):
             if len(result) == 0:
                 raise ls_utils.LangSmithNotFoundError(
                     f"Dataset {dataset_name} not found"
                 )
             return ls_schemas.Dataset(
-                **result[0], _host_url=self._host_url, _tenant_id=self._get_tenant_id()
+                **result[0],
+                _host_url=self._host_url,
+                _tenant_id=self._get_optional_tenant_id(),
             )
         return ls_schemas.Dataset(
-            **result, _host_url=self._host_url, _tenant_id=self._get_tenant_id()
+            **result,
+            _host_url=self._host_url,
+            _tenant_id=self._get_optional_tenant_id(),
         )
 
     def read_dataset_openai_finetuning(
         self, dataset_id: Optional[str] = None, *, dataset_name: Optional[str] = None
     ) -> list:
         """Download a dataset in OpenAI Jsonl format and load it as a list of dicts.
 
@@ -2151,15 +2168,17 @@
         if dataset_name is not None:
             params["name"] = dataset_name
         if dataset_name_contains is not None:
             params["name_contains"] = dataset_name_contains
 
         yield from (
             ls_schemas.Dataset(
-                **dataset, _host_url=self._host_url, _tenant_id=self._get_tenant_id()
+                **dataset,
+                _host_url=self._host_url,
+                _tenant_id=self._get_optional_tenant_id(),
             )
             for dataset in self._get_paginated_list("/datasets", params=params)
         )
 
     @ls_utils.xor_args(("dataset_id", "dataset_name"))
     def delete_dataset(
         self,
@@ -2494,15 +2513,17 @@
             f"{self.api_url}/examples",
             headers={**self._headers, "Content-Type": "application/json"},
             data=example.json(),
         )
         ls_utils.raise_for_status_with_text(response)
         result = response.json()
         return ls_schemas.Example(
-            **result, _host_url=self._host_url, _tenant_id=self._get_tenant_id()
+            **result,
+            _host_url=self._host_url,
+            _tenant_id=self._get_optional_tenant_id(),
         )
 
     def read_example(self, example_id: ID_TYPE) -> ls_schemas.Example:
         """Read an example from the LangSmith API.
 
         Args:
             example_id (UUID): The ID of the example to read.
@@ -2512,15 +2533,15 @@
         """
         response = self._get_with_retries(
             f"/examples/{_as_uuid(example_id, 'example_id')}",
         )
         return ls_schemas.Example(
             **response.json(),
             _host_url=self._host_url,
-            _tenant_id=self._get_tenant_id(),
+            _tenant_id=self._get_optional_tenant_id(),
         )
 
     def list_examples(
         self,
         dataset_id: Optional[ID_TYPE] = None,
         dataset_name: Optional[str] = None,
         example_ids: Optional[Sequence[ID_TYPE]] = None,
@@ -2550,15 +2571,17 @@
         else:
             pass
         if example_ids is not None:
             params["id"] = example_ids
         params["inline_s3_urls"] = inline_s3_urls
         yield from (
             ls_schemas.Example(
-                **example, _host_url=self._host_url, _tenant_id=self._get_tenant_id()
+                **example,
+                _host_url=self._host_url,
+                _tenant_id=self._get_optional_tenant_id(),
             )
             for example in self._get_paginated_list("/examples", params=params)
         )
 
     def update_example(
         self,
         example_id: str,
@@ -2663,15 +2686,17 @@
         """
         if isinstance(example, (str, uuid.UUID)):
             reference_example_ = self.read_example(example)
         elif isinstance(example, ls_schemas.Example):
             reference_example_ = example
         elif isinstance(example, dict):
             reference_example_ = ls_schemas.Example(
-                **example, _host_url=self._host_url, _tenant_id=self._get_tenant_id()
+                **example,
+                _host_url=self._host_url,
+                _tenant_id=self._get_optional_tenant_id(),
             )
         elif run.reference_example_id is not None:
             reference_example_ = self.read_example(run.reference_example_id)
         else:
             reference_example_ = None
         return reference_example_
```

### Comparing `langsmith-0.1.8/langsmith/env/__init__.py` & `langsmith-0.1.9/langsmith/env/__init__.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/env/_git.py` & `langsmith-0.1.9/langsmith/env/_git.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/env/_runtime_env.py` & `langsmith-0.1.9/langsmith/env/_runtime_env.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/evaluation/evaluator.py` & `langsmith-0.1.9/langsmith/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/evaluation/string_evaluator.py` & `langsmith-0.1.9/langsmith/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/run_helpers.py` & `langsmith-0.1.9/langsmith/run_helpers.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/run_trees.py` & `langsmith-0.1.9/langsmith/run_trees.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/schemas.py` & `langsmith-0.1.9/langsmith/schemas.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/utils.py` & `langsmith-0.1.9/langsmith/utils.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/langsmith/wrappers/_openai.py` & `langsmith-0.1.9/langsmith/wrappers/_openai.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.1.8/pyproject.toml` & `langsmith-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langsmith"
-version = "0.1.8"
+version = "0.1.9"
 description = "Client library to connect to the LangSmith LLM Tracing and Evaluation Platform."
 authors = ["LangChain <support@langchain.dev>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langsmith-sdk"
 homepage = "https://smith.langchain.com/"
 documentation = "https://docs.smith.langchain.com/"
```

### Comparing `langsmith-0.1.8/PKG-INFO` & `langsmith-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langsmith
-Version: 0.1.8
+Version: 0.1.9
 Summary: Client library to connect to the LangSmith LLM Tracing and Evaluation Platform.
 Home-page: https://smith.langchain.com/
 License: MIT
 Keywords: langsmith,langchain,llm,nlp,language,translation,evaluation,tracing,platform
 Author: LangChain
 Author-email: support@langchain.dev
 Requires-Python: >=3.8.1,<4.0
```

