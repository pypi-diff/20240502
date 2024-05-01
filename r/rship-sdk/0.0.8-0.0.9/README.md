# Comparing `tmp/rship-sdk-0.0.8.tar.gz` & `tmp/rship-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rship-sdk-0.0.8.tar", last modified: Mon Mar 25 23:02:28 2024, max compression
+gzip compressed data, was "rship-sdk-0.0.9.tar", last modified: Mon Mar 25 23:20:03 2024, max compression
```

## Comparing `rship-sdk-0.0.8.tar` & `rship-sdk-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2024-03-25 23:02:28.138424 rship-sdk-0.0.8/
--rw-r--r--   0 max        (501) staff       (20)     1074 2024-03-25 20:56:17.000000 rship-sdk-0.0.8/LICENSE
--rw-r--r--   0 max        (501) staff       (20)      523 2024-03-25 23:02:28.138160 rship-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)       15 2024-03-25 20:50:27.000000 rship-sdk-0.0.8/README.md
--rw-r--r--   0 max        (501) staff       (20)      586 2024-03-25 23:02:20.000000 rship-sdk-0.0.8/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)       38 2024-03-25 23:02:28.138471 rship-sdk-0.0.8/setup.cfg
-drwxr-xr-x   0 max        (501) staff       (20)        0 2024-03-25 23:02:28.134839 rship-sdk-0.0.8/src/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2024-03-25 23:02:28.136850 rship-sdk-0.0.8/src/rship_sdk/
--rw-r--r--   0 max        (501) staff       (20)      112 2024-03-25 22:57:25.000000 rship-sdk-0.0.8/src/rship_sdk/__init__.py
--rw-r--r--   0 max        (501) staff       (20)     6468 2024-03-25 23:02:10.000000 rship-sdk-0.0.8/src/rship_sdk/client.py
--rw-r--r--   0 max        (501) staff       (20)     2687 2024-03-25 22:56:01.000000 rship-sdk-0.0.8/src/rship_sdk/models.py
--rw-r--r--   0 max        (501) staff       (20)      576 2024-03-25 22:57:10.000000 rship-sdk-0.0.8/src/rship_sdk/utils.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2024-03-25 23:02:28.137892 rship-sdk-0.0.8/src/rship_sdk.egg-info/
--rw-r--r--   0 max        (501) staff       (20)      523 2024-03-25 23:02:28.000000 rship-sdk-0.0.8/src/rship_sdk.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      313 2024-03-25 23:02:28.000000 rship-sdk-0.0.8/src/rship_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2024-03-25 23:02:28.000000 rship-sdk-0.0.8/src/rship_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)        5 2024-03-25 23:02:28.000000 rship-sdk-0.0.8/src/rship_sdk.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)       10 2024-03-25 23:02:28.000000 rship-sdk-0.0.8/src/rship_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-03-25 23:20:03.918390 rship-sdk-0.0.9/
+-rw-r--r--   0 max        (501) staff       (20)     1074 2024-03-25 20:56:17.000000 rship-sdk-0.0.9/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)      523 2024-03-25 23:20:03.918145 rship-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)       15 2024-03-25 20:50:27.000000 rship-sdk-0.0.9/README.md
+-rw-r--r--   0 max        (501) staff       (20)      586 2024-03-25 23:19:58.000000 rship-sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)       38 2024-03-25 23:20:03.918439 rship-sdk-0.0.9/setup.cfg
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-03-25 23:20:03.914723 rship-sdk-0.0.9/src/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-03-25 23:20:03.916927 rship-sdk-0.0.9/src/rship_sdk/
+-rw-r--r--   0 max        (501) staff       (20)      171 2024-03-25 23:19:43.000000 rship-sdk-0.0.9/src/rship_sdk/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)     6501 2024-03-25 23:19:03.000000 rship-sdk-0.0.9/src/rship_sdk/client.py
+-rw-r--r--   0 max        (501) staff       (20)     3150 2024-03-25 23:18:31.000000 rship-sdk-0.0.9/src/rship_sdk/models.py
+-rw-r--r--   0 max        (501) staff       (20)      576 2024-03-25 22:57:10.000000 rship-sdk-0.0.9/src/rship_sdk/utils.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-03-25 23:20:03.917934 rship-sdk-0.0.9/src/rship_sdk.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)      523 2024-03-25 23:20:03.000000 rship-sdk-0.0.9/src/rship_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      313 2024-03-25 23:20:03.000000 rship-sdk-0.0.9/src/rship_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2024-03-25 23:20:03.000000 rship-sdk-0.0.9/src/rship_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)        5 2024-03-25 23:20:03.000000 rship-sdk-0.0.9/src/rship_sdk.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)       10 2024-03-25 23:20:03.000000 rship-sdk-0.0.9/src/rship_sdk.egg-info/top_level.txt
```

### Comparing `rship-sdk-0.0.8/LICENSE` & `rship-sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rship-sdk-0.0.8/PKG-INFO` & `rship-sdk-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rship-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Rship SDK in python
 Author-email: Max Fletcher <max@lucid.rocks>
 Project-URL: Homepage, https://github.com/lucid-rocks/rship
 Project-URL: Issues, https://github.com/lucid-rocks/rship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rship-sdk-0.0.8/pyproject.toml` & `rship-sdk-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rship-sdk"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Max Fletcher", email="max@lucid.rocks" },
 ]
 description = "The Rship SDK in python"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `rship-sdk-0.0.8/src/rship_sdk/client.py` & `rship-sdk-0.0.9/src/rship_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import json
 import websockets
 from typing import Any, Callable, Dict
 from myko import MEvent, MEventType, MCommand, WSMEvent, WSMCommand
-from .models import Target, Action, Emitter, Pulse, Instance, Machine, Alert
+from .models import Target, Action, Emitter, Pulse, Instance, Machine, Alert, InstanceStatus, TargetStatus, AlertEntityType, AlertLevel
 from .utils import generate_id, get_current_timestamp, make_instance_id
 
 class RshipExecClient:
     def __init__(self, rship_host: str, rship_port: int, on_connect: Callable[[], None] = None,
                  on_disconnect: Callable[[], None] = None, on_pulse: Callable[[Pulse], None] = None):
         self.rship_host = rship_host
         self.rship_port = rship_port
@@ -116,29 +116,29 @@
 
     async def pulse_emitter(self, emitter_id: str, data: Any):
         pulse = Pulse(id=generate_id(), name="", emitter_id=emitter_id, data=data)
         await self.set_data(pulse)
 
 
     
-    # async def set_instance_offline(self, instance_id: str):
-    #     instance = self.instances.get(instance_id)
-    #     if instance:
-    #         instance.status = InstanceStatus.UNAVAILABLE
-    #         await self.set_data(instance)
-
-    # async def set_target_offline(self, target_id: str, instance_id: str):
-    #     target = self.targets.get(target_id)
-    #     if target:
-    #         await self.set_target_status(target_id, instance_id, TargetStatus.OFFLINE)
-
-    # async def set_target_status(self, target_id: str, instance_id: str, status: TargetStatus):
-    #     target_status = TargetStatus(id=f"{instance_id}:{target_id}", target_id=target_id,
-    #                                  instance_id=instance_id, status=status)
-    #     await self.set_data(target_status)
+    async def set_instance_offline(self, instance_id: str):
+        instance = self.instances.get(instance_id)
+        if instance:
+            instance.status = InstanceStatus.UNAVAILABLE
+            await self.set_data(instance)
+
+    async def set_target_offline(self, target_id: str, instance_id: str):
+        target = self.targets.get(target_id)
+        if target:
+            await self.set_target_status(target_id, instance_id, TargetStatus.OFFLINE)
+
+    async def set_target_status(self, target_id: str, instance_id: str, status: TargetStatus):
+        target_status = TargetStatus(id=f"{instance_id}:{target_id}", target_id=target_id,
+                                     instance_id=instance_id, status=status)
+        await self.set_data(target_status)
 
     async def save_target(self, target: Target):
         self.targets[target.id] = target
         await self.set_data(target)
 
     async def save_action(self, action: Action):
         self.actions[action.id] = action
```

### Comparing `rship-sdk-0.0.8/src/rship_sdk/models.py` & `rship-sdk-0.0.9/src/rship_sdk/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from enum import Enum
 from typing import List, Optional, Any, Callable
 from myko import MItem, Schema, AlertLevel, AlertEntityType, InstanceStatus
 
 class Target(MItem):
     def __init__(self, id: str, name: str, action_ids: List[str], emitter_ids: List[str],
                  sub_targets: List[str], parent_targets: List[str], service_id: str,
                  bg_color: str, fg_color: str, last_updated: str, category: str, root_level: bool):
@@ -67,7 +68,32 @@
         super().__init__(id, f"{entity_id}:{code}")
         self.entity_id = entity_id
         self.entity_type = entity_type.value
         self.instance_id = instance_id
         self.level = level.value
         self.message = message
         self.code = code
+
+class AlertLevel(Enum):
+    INFO = 'info'
+    WARN = 'warn'
+    ERROR = 'error'
+
+
+class AlertEntityType(Enum):
+    TARGET = 'Target'
+    ACTION = 'Action'
+    PAYLOAD = 'Payload'
+    INSTANCE = 'Instance'
+
+
+class InstanceStatus(Enum):
+    STARTING = 'Starting'
+    AVAILABLE = 'Available'
+    STOPPING = 'Stopping'
+    UNAVAILABLE = 'Unavailable'
+    ERROR = 'Error'
+
+
+class TargetStatus(Enum):
+    ONLINE = 'online'
+    OFFLINE = 'offline'
```

### Comparing `rship-sdk-0.0.8/src/rship_sdk/utils.py` & `rship-sdk-0.0.9/src/rship_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `rship-sdk-0.0.8/src/rship_sdk.egg-info/PKG-INFO` & `rship-sdk-0.0.9/src/rship_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rship-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Rship SDK in python
 Author-email: Max Fletcher <max@lucid.rocks>
 Project-URL: Homepage, https://github.com/lucid-rocks/rship
 Project-URL: Issues, https://github.com/lucid-rocks/rship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

