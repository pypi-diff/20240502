# Comparing `tmp/pqapi-5.0.0.tar.gz` & `tmp/pqapi-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqapi-5.0.0.tar", last modified: Fri Mar 29 17:14:44 2024, max compression
+gzip compressed data, was "pqapi-5.0.1.tar", last modified: Thu May  2 20:00:52 2024, max compression
```

## Comparing `pqapi-5.0.0.tar` & `pqapi-5.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:14:44.701162 pqapi-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-29 17:14:23.000000 pqapi-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-29 17:14:44.701162 pqapi-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-29 17:14:23.000000 pqapi-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:14:44.701162 pqapi-5.0.0/pqapi/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-29 17:14:23.000000 pqapi-5.0.0/pqapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-03-29 17:14:23.000000 pqapi-5.0.0/pqapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-03-29 17:14:23.000000 pqapi-5.0.0/pqapi/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-29 17:14:23.000000 pqapi-5.0.0/pqapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-29 17:14:23.000000 pqapi-5.0.0/pqapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:14:44.701162 pqapi-5.0.0/pqapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-29 17:14:44.000000 pqapi-5.0.0/pqapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-29 17:14:44.000000 pqapi-5.0.0/pqapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 17:14:44.000000 pqapi-5.0.0/pqapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-29 17:14:44.000000 pqapi-5.0.0/pqapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-29 17:14:44.000000 pqapi-5.0.0/pqapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-29 17:14:23.000000 pqapi-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 17:14:44.701162 pqapi-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-29 17:14:23.000000 pqapi-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:14:44.701162 pqapi-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-03-29 17:14:23.000000 pqapi-5.0.0/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:00:52.542230 pqapi-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 20:00:30.000000 pqapi-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-02 20:00:52.542230 pqapi-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-02 20:00:30.000000 pqapi-5.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:00:52.538231 pqapi-5.0.1/pqapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:00:52.542230 pqapi-5.0.1/pqapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-02 20:00:52.000000 pqapi-5.0.1/pqapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 20:00:52.000000 pqapi-5.0.1/pqapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:00:52.000000 pqapi-5.0.1/pqapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-02 20:00:52.000000 pqapi-5.0.1/pqapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 20:00:52.000000 pqapi-5.0.1/pqapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-02 20:00:30.000000 pqapi-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:00:52.542230 pqapi-5.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:00:52.542230 pqapi-5.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-02 20:00:30.000000 pqapi-5.0.1/tests/test_api.py
```

### Comparing `pqapi-5.0.0/LICENSE` & `pqapi-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pqapi-5.0.0/README.md` & `pqapi-5.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # peperqa-api
+
 Python client for interacting with paperqa app
 
 # Usage
 
 Make sure to set the environment variable `PQA_API_TOKEN` or `PQA_API_KEY` to your API token.
 
 ```sh
@@ -15,14 +16,15 @@
 import pqapi
 response = pqapi.agent_query(
     "Are COVID-19 vaccines effective?"
 )
 ```
 
 to query with a specific bibliography (collection of papers)
+
 ```py
 import pqapi
 response = pqapi.agent_query(
     "Are COVID-19 vaccines effective?",
     "covid"
 )
 ```
@@ -33,14 +35,15 @@
 
 ```jinja
 The effectiveness of COVID-19 is given below:
 {{ "Are COVID-19 vaccines effective?" | pqa}}
 ```
 
 Or, more complex examples can use shared bibliographies set by variables names:
+
 ```jinja
 {% with bib = "covid" %}
 ## Info
 {{ "Are COVID-19 vaccines effective?" | pqa(bib)}}
 
 ## Modality
 {{ "Has there been an AAV COVID-19 vaccine?" | pqa(bib)}}
@@ -49,18 +52,16 @@
 
 You render it via:
 
 ```sh
 pqa-render template.jinja > output.md
 ```
 
-
 ## Managing bibliographies
 
-
 To get information about a specific bibliography
 
 ```py
 import pqapi
 response = pqapi.get_bibliography(
     "default"
 )
```

### Comparing `pqapi-5.0.0/pqapi/__init__.py` & `pqapi-5.0.1/pqapi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from .version import __version__  # noqa
 from .api import (
-    upload_file,
-    upload_paper,
     agent_query,
-    get_bibliography,
-    delete_bibliography,
+    async_agent_query,
     async_delete_bibliography,
     async_get_bibliography,
-    async_agent_query,
+    async_get_feedback,
     async_query,
     async_send_feedback,
-    async_get_feedback,
     check_dois,
-)  # noqa
-from .models import QueryRequest, UploadMetadata, AnswerResponse  # noqa
-from .models import get_prompts
+    delete_bibliography,
+    get_bibliography,
+    upload_file,
+    upload_paper,
+)
+from .models import AnswerResponse, QueryRequest, UploadMetadata, get_prompts
+from .version import __version__
 
 __all__ = [
+    "__version__",
     "upload_file",
     "upload_paper",
     "agent_query",
     "get_bibliography",
     "delete_bibliography",
     "QueryRequest",
     "UploadMetadata",
```

### Comparing `pqapi-5.0.0/pqapi/api.py` & `pqapi-5.0.1/pqapi/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,256 +1,241 @@
 import json
-from logging import getLogger
-from typing import Any, BinaryIO, Dict, Optional, Union
+import logging
+from typing import Any, BinaryIO
 from uuid import UUID
 
 import aiohttp
 import requests
 import tenacity
 
 from .models import AnswerResponse, DocsStatus, QueryRequest, UploadMetadata
 from .utils import get_pqa_key, get_pqa_url
 
-logger = getLogger(__name__)
+logger = logging.getLogger(__name__)
 PQA_URL = get_pqa_url()
 
 
-def coerce_request(query: Union[str, QueryRequest]) -> QueryRequest:
+def coerce_request(query: str | QueryRequest) -> QueryRequest:
     if isinstance(query, str):
         return QueryRequest(query=query)
-    elif isinstance(query, QueryRequest):
+    if isinstance(query, QueryRequest):
         return query
-    else:
-        raise TypeError("Query must be a string or QueryRequest")
+    raise TypeError("Query must be a string or QueryRequest")
 
 
-def parse_response(data: Dict[str, Any]) -> AnswerResponse:
+def parse_response(data: dict[str, Any]) -> AnswerResponse:
     return AnswerResponse(**data)
 
 
 def upload_file(
     bibliography: str,
     file: BinaryIO,
     metadata: UploadMetadata,
     public: bool = False,
-) -> Dict[str, Any]:
-    if public:
-        if not bibliography.startswith("public:"):
-            bibliography = f"public:{bibliography}"
-    url = f"{PQA_URL}/api/docs/{bibliography}/upload"
+) -> dict[str, Any]:
+    if public and not bibliography.startswith("public:"):
+        bibliography = f"public:{bibliography}"
 
     with requests.Session() as session:
         response = session.post(
-            url,
+            f"{PQA_URL}/api/docs/{bibliography}/upload",
             files=[("file", file)],
-            data=dict(metadata=metadata.json()),
+            json={"metadata": metadata.model_dump()},
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
         )
         response.raise_for_status()
-        result: Dict[str, Any] = response.json()
-        return result
+        return response.json()
 
 
-def upload_paper(
-    paper_id: str,
-    file: BinaryIO,
-):
-    url = f"{PQA_URL}/db/upload/paper/{paper_id}"
+def upload_paper(doi: str, file: BinaryIO) -> None:
     with requests.Session() as session:
         result = session.post(
-            url,
+            f"{PQA_URL}/db/upload/paper/",
+            params={"doi": doi},
             files=[("file", file)],
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
         )
         result.raise_for_status()
 
 
-def check_dois(
-    dois: list[str],
-) -> Dict:
-    url = f"{PQA_URL}/db/docs/dois"
+def check_dois(dois: list[str]) -> dict[str, tuple[str, str]]:
     with requests.Session() as session:
         result = session.post(
-            url,
+            f"{PQA_URL}/db/docs/dois",
             json=dois,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
         )
         result.raise_for_status()
         return result.json()
 
 
 def delete_bibliography(bibliography: str, public: bool = False) -> None:
-    if public:
-        if not bibliography.startswith("public:"):
-            bibliography = f"public:{bibliography}"
+    if public and not bibliography.startswith("public:"):
+        bibliography = f"public:{bibliography}"
     url = f"{PQA_URL}/db/docs/delete/{bibliography}"
     with requests.Session() as session:
         response = session.get(
             url,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
         )
         response.raise_for_status()
 
 
 async def async_delete_bibliography(bibliography: str, public: bool = False) -> None:
-    if public:
-        if not bibliography.startswith("public:"):
-            bibliography = f"public:{bibliography}"
+    if public and not bibliography.startswith("public:"):
+        bibliography = f"public:{bibliography}"
     url = f"{PQA_URL}/db/docs/delete/{bibliography}"
-    async with aiohttp.ClientSession() as session:
-        async with session.get(
+    async with (
+        aiohttp.ClientSession() as session,
+        session.get(
             url,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
-        ) as response:
-            response.raise_for_status()
+        ) as response,
+    ):
+        response.raise_for_status()
 
 
 def get_bibliography(bibliography: str, public: bool = False) -> DocsStatus:
-    if public:
-        if not bibliography.startswith("public:"):
-            bibliography = f"public:{bibliography}"
+    if public and not bibliography.startswith("public:"):
+        bibliography = f"public:{bibliography}"
     url = f"{PQA_URL}/api/docs/status/{bibliography}"
     with requests.Session() as session:
         response = session.get(
             url,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
         )
         response.raise_for_status()
-        result = DocsStatus(**response.json())
-        return result
+        return DocsStatus(**response.json())
 
 
 async def async_get_bibliography(bibliography: str, public: bool = False) -> DocsStatus:
-    if public:
-        if not bibliography.startswith("public:"):
-            bibliography = f"public:{bibliography}"
+    if public and not bibliography.startswith("public:"):
+        bibliography = f"public:{bibliography}"
     url = f"{PQA_URL}/api/docs/status/{bibliography}"
-    async with aiohttp.ClientSession() as session:
-        async with session.get(
+    async with (
+        aiohttp.ClientSession() as session,
+        session.get(
             url,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
-        ) as response:
-            data = await response.json()
-            result = DocsStatus(**data)
-            return result
+        ) as response,
+    ):
+        data = await response.json()
+        return DocsStatus(**data)
 
 
 @tenacity.retry(
     wait=tenacity.wait_random_exponential(multiplier=1, max=30),
     stop=tenacity.stop_after_attempt(3),
 )
-def agent_query(
-    query: Union[QueryRequest, str], bibliography: str = "tmp"
-) -> AnswerResponse:
+def agent_query(query: QueryRequest | str, bibliography: str = "tmp") -> AnswerResponse:
     query_request = coerce_request(query)
     url = f"{PQA_URL}/api/agent/{bibliography if bibliography else 'tmp'}"
     with requests.Session() as session:
-        qd = query_request.dict()
         response = session.post(
             url,
-            json={"query": qd},
+            json={"query": query_request.model_dump()},
             headers={
                 "Authorization": f"Bearer {get_pqa_key()}",
                 "Content-Type": "application/json; charset=utf-8",
             },
         )
         response.raise_for_status()
-        result = parse_response(response.json())
-    return result
+        return parse_response(response.json())
 
 
 @tenacity.retry(
     wait=tenacity.wait_random_exponential(multiplier=1, max=10),
     stop=tenacity.stop_after_attempt(2),
 )
 async def async_agent_query(
-    query: Union[QueryRequest, str],
+    query: QueryRequest | str,
     bibliography: str = "tmp",
 ) -> AnswerResponse:
     query_request = coerce_request(query)
-    url = f"{PQA_URL}/api/agent/{bibliography if bibliography else 'tmp'}"
-    async with aiohttp.ClientSession() as session:
-        qd = query_request.dict()
-        async with session.post(
-            url,
+    qd = query_request.model_dump()
+    async with (
+        aiohttp.ClientSession() as session,
+        session.post(
+            f"{PQA_URL}/api/agent/{bibliography if bibliography else 'tmp'}",
             json={"query": qd},
             timeout=1200,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
-        ) as response:
-            try:
-                data = await response.json()
-            except Exception:
-                text = await response.text()
-                logger.warning("Failed Request: \n" + json.dumps(qd, indent=2))
-                logger.warning("\n\nResponse:\n\n" + text)
-            response.raise_for_status()
-            result = parse_response(data)
-    return result
+        ) as response,
+    ):
+        try:
+            data = await response.json()
+        except Exception:
+            text = await response.text()
+            logger.warning(f"Failed Request: \n{json.dumps(qd, indent=2)}")
+            logger.warning(f"\n\nResponse:\n\n{text}")
+        response.raise_for_status()
+        return parse_response(data)
 
 
 @tenacity.retry(
     wait=tenacity.wait_random_exponential(multiplier=1, max=10),
     stop=tenacity.stop_after_attempt(3),
 )
-async def async_query(
-    query: Union[QueryRequest, str], bibliography: str
-) -> AnswerResponse:
+async def async_query(query: QueryRequest | str, bibliography: str) -> AnswerResponse:
     query_request = coerce_request(query)
     url = f"{PQA_URL}/api/query/{bibliography}"
-    async with aiohttp.ClientSession() as session:
-        qd = query_request.dict()
-        async with session.post(
+    async with (
+        aiohttp.ClientSession() as session,
+        session.post(
             url,
-            json=qd,
+            json=query_request.model_dump(),
             timeout=600,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
-        ) as response:
-            data = await response.json()
-            response.raise_for_status()
-            result = parse_response(data)
-    return result
+        ) as response,
+    ):
+        data = await response.json()
+        response.raise_for_status()
+        return parse_response(data)
 
 
 async def async_send_feedback(
-    queries: list[UUID], feedback: list[dict], group: Optional[str] = None
+    queries: list[UUID], feedback: list[dict], group: str | None = None
 ) -> bool:
     url = f"{PQA_URL}/api/feedback"
     # default JSON serializer in python cannot handle UUID
     queries_as_str = [str(q) for q in queries]
-    async with aiohttp.ClientSession() as session:
-        async with session.post(
+    async with (
+        aiohttp.ClientSession() as session,
+        session.post(
             url,
             json={
                 "queries": queries_as_str,
                 "feedback": feedback,
                 "feedback_group": group,
             },
             timeout=600,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
-        ) as response:
-            response.raise_for_status()
+        ) as response,
+    ):
+        response.raise_for_status()
     return True
 
 
 async def async_get_feedback(
-    query: Optional[UUID] = None, group: Optional[str] = None
-) -> Dict[str, Any]:
+    query: UUID | None = None, group: str | None = None
+) -> dict[str, Any]:
     # add as query parameters
     body = {"query": str(query), "feedback_group": group}
     if query is None and group is None:
         raise ValueError("At least one of query or group must be provided")
     if query is None:
         del body["query"]
     if group is None:
         del body["feedback_group"]
     url = f"{PQA_URL}/db/feedback"
 
-    async with aiohttp.ClientSession() as session:
-        async with session.get(
+    async with (
+        aiohttp.ClientSession() as session,
+        session.get(
             url,
             json=body,
             timeout=600,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
-        ) as response:
-            response.raise_for_status()
-            result = await response.json()
-    return result
+        ) as response,
+    ):
+        response.raise_for_status()
+        return await response.json()
```

### Comparing `pqapi-5.0.0/pqapi/models.py` & `pqapi-5.0.1/pqapi/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import re
 from functools import lru_cache
-from typing import Dict, List, Optional, Tuple
 
 import paperqa
 import requests
 from paperqa.types import Answer, PromptCollection
 from pydantic import BaseModel, Field, ValidationInfo, field_validator, validator
 
 from .utils import get_pqa_key, get_pqa_url
@@ -14,78 +13,78 @@
     agent_prompt: str = ""
     agent_search_tool: str = ""
     search_count: int = 8
     wipe_context_on_answer_failure: bool = True
     timeout: float = 500  # seconds
 
 
-def _extract_doi(citation: str) -> Optional[str]:
+def _extract_doi(citation: str) -> str | None:
     doi = re.findall(r"10\.\d{4}/\S+", citation, re.IGNORECASE)
     if len(doi) > 0:
         return doi[-1]
     return None
 
 
 # we have to put it here to avoid circular imports
 # because we use this in the default factory of the QueryRequest
 @lru_cache(maxsize=100)
-def get_prompts() -> Tuple[Dict[str, PromptCollection], AgentPromptCollection]:
+def get_prompts() -> tuple[dict[str, PromptCollection], AgentPromptCollection]:
     url = f"{get_pqa_url()}/api/prompts/all"
     with requests.Session() as session:
         response = session.get(
             url,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
         )
         response.raise_for_status()
         result = response.json()
     return (
         {
-            k: PromptCollection.parse_obj(v["prompt-collection"])
+            k: PromptCollection.model_validate(v["prompt-collection"])
             for k, v in result.items()
         },
-        AgentPromptCollection.parse_obj(result["default"]["agent-prompt"]),
+        AgentPromptCollection.model_validate(result["default"]["agent-prompt"]),
     )
 
 
 class UploadMetadata(BaseModel):
     filename: str
     citation: str
-    key: Optional[str] = None
+    key: str | None = None
 
 
 class Doc(paperqa.Doc):
-    doi: Optional[str] = None
+    doi: str | None = None
 
     @validator("doi", pre=True)
-    def citation_to_doi(cls, v: Optional[str], values: Dict) -> Optional[str]:
+    def citation_to_doi(cls, v: str | None, values: dict) -> str | None:  # noqa: N805
         if v is None and "citation" in values:
             return _extract_doi(values["citation"])
         return v
 
 
 class DocsStatus(BaseModel):
     name: str
     llm: str
     summary_llm: str
-    docs: List[Doc]
+    docs: list[Doc]
     doc_count: int
     writeable: bool = False
 
 
-# COPIED FROM paperqa-sverer!
+# COPIED FROM paperqa-server!
 class QueryRequest(BaseModel):
     query: str
-    group: Optional[str] = None
+    group: str | None = None
     llm: str = "gpt-4-0613"
     summary_llm: str = "gpt-3.5-turbo-0125"
     length: str = "about 200 words, but can be longer if necessary"
     summary_length: str = "about 100 words"
     max_sources: int = 7
     consider_sources: int = 12
-    named_prompt: Optional[str] = None
+    named_prompt: str | None = None
     # if you change this to something other than default
     # modify code below in update_prompts
     prompts: PromptCollection = Field(
         default_factory=lambda: get_prompts()[0]["json"], validate_default=True
     )
     agent_tools: AgentPromptCollection = Field(default_factory=lambda: get_prompts()[1])
     texts_index_mmr_lambda: float = 0.9
@@ -93,21 +92,23 @@
     embedding: str = "hybrid-text-embedding-3-small"
     # concurrent number of summary calls to use inside Doc object
     max_concurrent: int = 12
     temperature: float = 0.0
     summary_temperature: float = 0.0
 
     @field_validator("max_sources")
+    @classmethod
     def max_sources_for_gpt(cls, v: int, info: ValidationInfo) -> int:
         values = info.data
-        if "gpt" in values["llm"] and v > 10:
+        if "gpt" in values["llm"] and v > 10:  # noqa: PLR2004
             raise ValueError("Max sources for GPT models is 10")
         return v
 
     @field_validator("prompts")
+    @classmethod
     def update_prompts(
         cls,
         v: PromptCollection,
         info: ValidationInfo,
     ) -> PromptCollection:
         STATIC_PROMPTS, _ = get_prompts()
         values = info.data
@@ -123,12 +124,12 @@
             # so that Docs doesn't break when we don't have a summary_llm
             values["summary_llm"] = "gpt-3.5-turbo"
         return v
 
 
 class AnswerResponse(BaseModel):
     answer: Answer
-    usage: Dict[str, List[int]]
-    bibtex: Dict[str, str]
+    usage: dict[str, list[int]]
+    bibtex: dict[str, str]
     status: str
     timing_info: dict[str, dict[str, float]] | None = None
     duration: float = 0
```

### Comparing `pqapi-5.0.0/tests/test_api.py` & `pqapi-5.0.1/tests/test_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     get_bibliography,
     get_prompts,
     upload_file,
     upload_paper,
 )
 
 
-def test_get_prompts():
+def test_get_prompts() -> None:
     prompts, agent_prompts = get_prompts()
     some_prompt = prompts["default"]
     assert isinstance(some_prompt, paperqa.PromptCollection)
     assert agent_prompts.timeout > 0
     assert len(agent_prompts.agent_search_tool) > 25
 
 
@@ -51,120 +51,123 @@
 def test_query_obj():
     prompt_collection = paperqa.PromptCollection()
     prompt_collection.post = (
         "This answer below was generated for {cost}. "
         "Provide a critique of this answer that could be used to improve it.\n\n"
         "{question}\n\n{answer}"
     )
-    print(prompt_collection.json())
     request = QueryRequest(
         query="How are bispecific antibodies engineered?",
         prompts=prompt_collection,
         max_sources=2,
         consider_sources=5,
     )
     agent_query(request)
 
 
-def test_upload_file():
+def test_upload_file() -> None:
     script_dir = os.path.dirname(__file__)
-    file = open(os.path.join(script_dir, "paper.pdf"), "rb")
+    file = open(os.path.join(script_dir, "paper.pdf"), "rb")  # noqa: SIM115
     response = upload_file(
         "default",
         file,
         UploadMetadata(filename="paper.pdf", citation="Test Citation"),
     )
+    assert response["success"], f"Expected success in response {response}."
 
-    assert response["success"] is True
 
-
-def test_upload_public():
+def test_upload_public() -> None:
     # create a public bibliography
     script_dir = os.path.dirname(__file__)
-    file = open(os.path.join(script_dir, "paper.pdf"), "rb")
+    file = open(os.path.join(script_dir, "paper.pdf"), "rb")  # noqa: SIM115
     response = upload_file(
         "api-test-public",
         file,
         UploadMetadata(filename="paper.pdf", citation="Test Citation"),
         public=True,
     )
-
-    assert response["success"] is True
+    assert response["success"], f"Expected success in response {response}."
 
     # get status of public bibliography
     status = get_bibliography("api-test-public", public=True)
 
-    assert status.writeable is True
+    assert status.writeable
     assert status.doc_count == 1
 
     # delete public bibliography
     delete_bibliography("api-test-public", public=True)
 
 
 # now test async
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_async_query_str():
     response = await async_agent_query(
         "How are bispecific antibodies engineered?", "default"
     )
     assert isinstance(response, AnswerResponse)
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_async_query_model():
     response = await async_agent_query(
         QueryRequest(query="How are bispecific antibodies engineered?"), "default"
     )
     assert isinstance(response, AnswerResponse)
 
 
-@pytest.mark.asyncio
-async def test_feedback_model():
+@pytest.mark.asyncio()
+async def test_feedback_model() -> None:
     response = await async_agent_query(
         QueryRequest(query="How are bispecific antibodies engineered?"), "default"
     )
     assert isinstance(response, AnswerResponse)
-    feedback = dict(test_feedback="great!")
-    response = await async_send_feedback([response.answer.id], [feedback], "default")
-    assert response
+    feedback = {"test_feedback": "great!"}
+    assert await async_send_feedback([response.answer.id], [feedback], "default")
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_async_tmp():
     response = await async_agent_query(
         QueryRequest(query="How are bispecific antibodies engineered?"),
     )
     assert isinstance(response, AnswerResponse)
 
 
-def test_async_upload_paper():
+def test_upload_paper() -> None:
     script_dir = os.path.dirname(__file__)
-    file = open(os.path.join(script_dir, "paper.pdf"), "rb")
-    response = upload_paper(
-        "1db1bde653658ec9b30858ae14650b8f9c9d438b",
-        file,
-    )
-    print(response)
-    assert response.status_code == 200
+    file = open(os.path.join(script_dir, "paper.pdf"), "rb")  # noqa: SIM115
+    upload_paper("10.1021/acs.jctc.2c01235", file)
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_async_query_noagent():
     response = await async_query("Why is KRAS studied?", "public:pqa-bench")
     assert isinstance(response, AnswerResponse)
 
 
-def test_check_dois():
-    dois = ["10.1126/science.1240517", "10.1126/science.1240517"]
-    response = check_dois(dois)
-    assert response
-
-
-def test_main():
-    from pqapi.main import main
+def test_check_dois() -> None:
+    response = check_dois(
+        dois=[
+            "10.1126/science.1240517",
+            "10.1126/science.1240517",  # NOTE: duplicate input DOI
+            "10.1016/j.febslet.2014.11.036",
+        ]
+    )
+    assert response == {
+        "10.1016/j.febslet.2014.11.036": [
+            "4f81e5a9ba561b9431b5919252ca677e34d1315a",
+            "cached",
+        ],
+        "10.1126/science.1240517": ["", "DOI not found"],
+    }
+
+
+@pytest.mark.skip(reason="This test is broken since it imports nonexistent module.")
+def test_main() -> None:
+    from pqapi.main import main  # type: ignore[import-not-found,unused-ignore]
 
     runner = click.testing.CliRunner()
     with runner.isolated_filesystem():
         with open("test.jinja2", "w") as f:
             f.write(
                 """
 {% with bib = "covid" %}
```

