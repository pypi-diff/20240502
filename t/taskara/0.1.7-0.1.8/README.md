# Comparing `tmp/taskara-0.1.7.tar.gz` & `tmp/taskara-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.7.tar", max compression
+gzip compressed data, was "taskara-0.1.8.tar", max compression
```

## Comparing `taskara-0.1.7.tar` & `taskara-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.7/LICENSE
--rw-r--r--   0        0        0      753 2024-04-03 02:46:31.154602 taskara-0.1.7/README.md
--rw-r--r--   0        0        0      392 2024-04-04 17:21:39.608405 taskara-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.7/taskara/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.7/taskara/db/conn.py
--rw-r--r--   0        0        0     1352 2024-04-03 02:34:26.057465 taskara-0.1.7/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.7/taskara/env.py
--rw-r--r--   0        0        0     1513 2024-04-04 16:36:43.488474 taskara-0.1.7/taskara/models.py
--rw-r--r--   0        0        0    18410 2024-04-04 17:21:05.365064 taskara-0.1.7/taskara/task.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 taskara-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.8/LICENSE
+-rw-r--r--   0        0        0      753 2024-04-03 02:46:31.154602 taskara-0.1.8/README.md
+-rw-r--r--   0        0        0      392 2024-04-04 17:57:52.140664 taskara-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.8/taskara/__init__.py
+-rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.8/taskara/db/conn.py
+-rw-r--r--   0        0        0     1352 2024-04-03 02:34:26.057465 taskara-0.1.8/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.8/taskara/env.py
+-rw-r--r--   0        0        0     1513 2024-04-04 16:36:43.488474 taskara-0.1.8/taskara/models.py
+-rw-r--r--   0        0        0    18411 2024-04-04 17:57:44.458394 taskara-0.1.8/taskara/task.py
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 taskara-0.1.8/PKG-INFO
```

### Comparing `taskara-0.1.7/LICENSE` & `taskara-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.7/README.md` & `taskara-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.7/taskara/db/conn.py` & `taskara-0.1.8/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.7/taskara/db/models.py` & `taskara-0.1.8/taskara/db/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.7/taskara/models.py` & `taskara-0.1.8/taskara/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.7/taskara/task.py` & `taskara-0.1.8/taskara/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from dataclasses import dataclass, field
 import uuid
 import time
 from typing import List, Optional, TypeVar
 import requests
 import os
 import json
 import hashlib
@@ -443,15 +442,15 @@
         obj._output = schema.output
         obj._version = schema.version
         obj._remote = remote
 
         if schema.threads:
             obj._threads = [RoleThread.from_schema(s) for s in schema.threads]
         else:
-            obj._threads = []
+            obj._threads = [RoleThread(owner_id=owner_id, name="feed")]
 
         return obj
 
     def refresh(self, auth_token: Optional[str] = None) -> None:
         print("\n!refreshing task", self._id)
         if hasattr(self, "_remote") and self._remote:
             print("\n!refreshing remote task", self._id)
```

### Comparing `taskara-0.1.7/PKG-INFO` & `taskara-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.7
+Version: 0.1.8
 Summary: Task management for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

