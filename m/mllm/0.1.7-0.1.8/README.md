# Comparing `tmp/mllm-0.1.7.tar.gz` & `tmp/mllm-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mllm-0.1.7.tar", max compression
+gzip compressed data, was "mllm-0.1.8.tar", max compression
```

## Comparing `mllm-0.1.7.tar` & `mllm-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-04-27 16:19:02.140835 mllm-0.1.7/LICENSE
--rw-r--r--   0        0        0     2221 2024-04-29 21:12:11.290383 mllm-0.1.7/README.md
--rw-r--r--   0        0        0      149 2024-04-29 21:17:19.261017 mllm-0.1.7/mllm/__init__.py
--rw-r--r--   0        0        0     2249 2024-04-30 02:56:14.276096 mllm-0.1.7/mllm/db/conn.py
--rw-r--r--   0        0        0      541 2024-04-27 16:19:02.141445 mllm-0.1.7/mllm/db/models.py
--rw-r--r--   0        0        0      846 2024-04-29 21:16:16.874384 mllm-0.1.7/mllm/models.py
--rw-r--r--   0        0        0     5605 2024-04-30 21:03:51.206117 mllm-0.1.7/mllm/prompt.py
--rw-r--r--   0        0        0     8299 2024-04-29 21:17:12.773037 mllm-0.1.7/mllm/router.py
--rw-r--r--   0        0        0      793 2024-04-29 21:17:15.851578 mllm-0.1.7/mllm/util.py
--rw-r--r--   0        0        0      390 2024-04-30 21:37:42.022957 mllm-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 mllm-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-27 16:19:02.140835 mllm-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2221 2024-04-29 21:12:11.290383 mllm-0.1.8/README.md
+-rw-r--r--   0        0        0      202 2024-04-30 21:47:38.359510 mllm-0.1.8/mllm/__init__.py
+-rw-r--r--   0        0        0     2249 2024-04-30 02:56:14.276096 mllm-0.1.8/mllm/db/conn.py
+-rw-r--r--   0        0        0      541 2024-04-27 16:19:02.141445 mllm-0.1.8/mllm/db/models.py
+-rw-r--r--   0        0        0      834 2024-04-30 21:47:46.059972 mllm-0.1.8/mllm/models.py
+-rw-r--r--   0        0        0     5565 2024-04-30 21:46:42.203231 mllm-0.1.8/mllm/prompt.py
+-rw-r--r--   0        0        0     8299 2024-04-30 21:47:47.547719 mllm-0.1.8/mllm/router.py
+-rw-r--r--   0        0        0      793 2024-04-29 21:17:15.851578 mllm-0.1.8/mllm/util.py
+-rw-r--r--   0        0        0      390 2024-04-30 21:47:53.908729 mllm-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 mllm-0.1.8/PKG-INFO
```

### Comparing `mllm-0.1.7/LICENSE` & `mllm-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mllm-0.1.7/README.md` & `mllm-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `mllm-0.1.7/mllm/db/conn.py` & `mllm-0.1.8/mllm/db/conn.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.7/mllm/db/models.py` & `mllm-0.1.8/mllm/db/models.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.7/mllm/prompt.py` & `mllm-0.1.8/mllm/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import uuid
 import time
 import logging
 import json
 from typing import Dict, Any, List, Optional
 
 from threadmem import RoleThread, RoleMessage
-from threadmem.server.models import RoleMessageModel, RoleThreadModel
+from threadmem.server.models import V1RoleMessage, V1RoleThread
 
 from .db.models import PromptRecord
 from .db.conn import WithDB
 from .models import V1Prompt
 
 logger = logging.getLogger(__name__)
 
@@ -111,29 +111,29 @@
         # Serialize the response using RoleMessageModel's json() method
         if not self.metadata:
             self.metadata = {}
 
         return PromptRecord(
             id=self._id,
             namespace=self._namespace,
-            thread=self._thread.to_schema().model_dump_json(),
-            response=self._response.to_schema().model_dump_json(),
+            thread=self._thread.to_v1().model_dump_json(),
+            response=self._response.to_v1().model_dump_json(),
             metadata_=json.dumps(self._metadata),
             created=self._created,
             approved=self._approved,
             flagged=self._flagged,
         )
 
     @classmethod
     def from_record(cls, record: PromptRecord) -> "Prompt":
         # Deserialize thread_id into a RoleThreadModel using a suitable method or lookup
-        thread_model = RoleThreadModel.model_validate_json(str(record.thread))
-        thread = RoleThread.from_schema(thread_model)
+        thread_model = V1RoleThread.model_validate_json(str(record.thread))
+        thread = RoleThread.from_v1(thread_model)
 
-        response = RoleMessageModel.model_validate_json(str(record.response))
+        response = V1RoleMessage.model_validate_json(str(record.response))
         metadata = json.loads(record.metadata_) if record.metadata_ else {}  # type: ignore
 
         obj = cls.__new__(cls)
         obj._id = record.id
         obj._namespace = record.namespace
         obj._thread = thread
         obj._response = response
@@ -144,30 +144,30 @@
 
         return obj
 
     def to_v1(self) -> V1Prompt:
         return V1Prompt(
             id=self._id,
             namespace=self._namespace,
-            thread=self._thread.to_schema(),
-            response=self._response.to_schema(),
+            thread=self._thread.to_v1(),
+            response=self._response.to_v1(),
             metadata=self._metadata,
             created=self._created,
             approved=self._approved,
             flagged=self._flagged,
         )
 
     @classmethod
     def from_v1(cls, v1: V1Prompt) -> "Prompt":
         obj = cls.__new__(cls)
 
         obj._id = v1.id
         obj._namespace = v1.namespace
-        obj._thread = RoleThread.from_schema(v1.thread)
-        obj._response = RoleMessage.from_schema(v1.response)
+        obj._thread = RoleThread.from_v1(v1.thread)
+        obj._response = RoleMessage.from_v1(v1.response)
         obj._metadata = v1.metadata
         obj._created = v1.created
         obj._approved = v1.approved
         obj._flagged = v1.flagged
 
         return obj
```

### Comparing `mllm-0.1.7/mllm/router.py` & `mllm-0.1.8/mllm/router.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.7/mllm/util.py` & `mllm-0.1.8/mllm/util.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.7/PKG-INFO` & `mllm-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mllm
-Version: 0.1.7
+Version: 0.1.8
 Summary: Multimodal Large Language Models
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

