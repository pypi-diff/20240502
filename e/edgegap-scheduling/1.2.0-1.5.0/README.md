# Comparing `tmp/edgegap_scheduling-1.2.0.tar.gz` & `tmp/edgegap_scheduling-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_scheduling-1.2.0.tar", max compression
+gzip compressed data, was "edgegap_scheduling-1.5.0.tar", max compression
```

## Comparing `edgegap_scheduling-1.2.0.tar` & `edgegap_scheduling-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/LICENSE
--rw-r--r--   0        0        0     2164 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/README.md
--rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/BUILD
--rw-r--r--   0        0        0      281 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/__init__.py
--rw-r--r--   0        0        0      128 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_depends.py
--rw-r--r--   0        0        0     4269 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_runner.py
--rw-r--r--   0        0        0     4436 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_scheduler.py
--rw-r--r--   0        0        0     1303 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_signature.py
--rw-r--r--   0        0        0      482 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_singleton.py
--rw-r--r--   0        0        0     1233 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_sleep.py
--rw-r--r--   0        0        0      188 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_state.py
--rw-r--r--   0        0        0     4221 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_task.py
--rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/errors/BUILD
--rw-r--r--   0        0        0      133 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/errors/__init__.py
--rw-r--r--   0        0        0      103 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/errors/_errors.py
--rw-r--r--   0        0        0      702 2024-05-01 17:52:46.827698 edgegap_scheduling-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 edgegap_scheduling-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2164 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/BUILD
+-rw-r--r--   0        0        0      330 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/__init__.py
+-rw-r--r--   0        0        0      128 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_depends.py
+-rw-r--r--   0        0        0     4269 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_runner.py
+-rw-r--r--   0        0        0     4436 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_scheduler.py
+-rw-r--r--   0        0        0     1303 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_signature.py
+-rw-r--r--   0        0        0      482 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_singleton.py
+-rw-r--r--   0        0        0     1468 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_sleep.py
+-rw-r--r--   0        0        0      550 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_state.py
+-rw-r--r--   0        0        0     4291 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_task.py
+-rw-r--r--   0        0        0       17 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/errors/BUILD
+-rw-r--r--   0        0        0      133 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/errors/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/errors/_errors.py
+-rw-r--r--   0        0        0      691 2024-05-02 18:20:32.343986 edgegap_scheduling-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 edgegap_scheduling-1.5.0/PKG-INFO
```

### Comparing `edgegap_scheduling-1.2.0/LICENSE` & `edgegap_scheduling-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.2.0/README.md` & `edgegap_scheduling-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.2.0/edgegap_scheduling/_runner.py` & `edgegap_scheduling-1.5.0/edgegap_scheduling/_runner.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.2.0/edgegap_scheduling/_scheduler.py` & `edgegap_scheduling-1.5.0/edgegap_scheduling/_scheduler.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.2.0/edgegap_scheduling/_signature.py` & `edgegap_scheduling-1.5.0/edgegap_scheduling/_signature.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.2.0/edgegap_scheduling/_sleep.py` & `edgegap_scheduling-1.5.0/edgegap_scheduling/_sleep.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 import asyncio
+from asyncio import Task
 
 
 class AsyncSleep:
     def __init__(self):
         self.tasks = {}
 
-    async def sleep(self, identifier: str, delay, result=None):
+    async def sleep(self, identifier: str, delay: float | int, result=None):
         coro = asyncio.sleep(delay, result=result)
         task = asyncio.ensure_future(coro)
         self.tasks[identifier] = task
 
         try:
             return await task
         except asyncio.CancelledError:
             return result
         finally:
             self.tasks.pop(task, None)
 
-    def __cancel_one_helper(self, identifier: str):
+    def __cancel_one_helper(self, identifier: str) -> Task | None:
         task = self.tasks.get(identifier)
-        task.cancel()
 
-        return task
+        if task:
+            task.cancel()
 
-    async def cancel_one(self, identifier: str):
+            return task
+
+    async def cancel_one(self, identifier: str) -> bool:
         task = self.__cancel_one_helper(identifier)
 
+        if task is None:
+            raise KeyError(f'Task {identifier} not found')
+
         await asyncio.wait([task])
 
-        return self.tasks.pop(task, None)
+        self.tasks.pop(task, None)
+        return True
 
     def __cancel_all_helper(self) -> dict:
         cancelled = {}
 
         for identifier, task in self.tasks.items():
             if task.cancel():
                 cancelled[identifier] = task
 
         return cancelled
 
-    async def cancel_all(self):
+    async def cancel_all(self) -> int:
         cancelled = self.__cancel_all_helper()
 
-        await asyncio.wait(self.tasks.values())
+        if len(cancelled) > 0:
+            await asyncio.wait(self.tasks.values())
 
-        for identifier, _ in cancelled.items():
-            self.tasks.pop(identifier)
+            for identifier, _ in cancelled.items():
+                self.tasks.pop(identifier)
 
         return len(cancelled)
```

### Comparing `edgegap_scheduling-1.2.0/edgegap_scheduling/_task.py` & `edgegap_scheduling-1.5.0/edgegap_scheduling/_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,23 @@
     )
 
     def __str__(self):
         return (
             f'Task {Format.squared(self.name, Color.GREEN)} - '
             f'Every {Format.squared(self.every, Color.GREEN)} - '
             f'Delay {Format.squared(self.delay, Color.GREEN)} - '
-            f'{self.state}'
+            f'State {Format.squared(self.state.value, self.state.color)}'
         )
 
     @property
-    def every_in_seconds(self) -> float | None:
+    def every_in_seconds(self) -> float | int | None:
         return parse(self.every) if isinstance(self.every, str) else None
 
     @property
-    def delay_in_seconds(self) -> float | None:
+    def delay_in_seconds(self) -> float | int | None:
         return parse(self.delay) if isinstance(self.delay, str) else None
 
     @property
     def should_delay(self) -> bool:
         return isinstance(self.delay_in_seconds, (float, int))
 
     @property
@@ -56,15 +56,15 @@
     @computed_field(description='If the Task is safe to start')
     @property
     def safe_to_start(self) -> bool:
         return self.state in [TaskState.PENDING, TaskState.COMPLETED, TaskState.STOPPED, TaskState.ERROR]
 
     @computed_field(description='For how long the task did the processing before sleeping')
     @property
-    def last_processing_duration(self) -> float | None:
+    def last_processing_duration(self) -> float | int | None:
         if self.begin_at and self.sleep_at:
             if self.begin_at < self.sleep_at:
                 return (self.sleep_at - self.begin_at).total_seconds()
 
     @computed_field(description='If the task is currently processing or sleeping')
     @property
     def is_processing(self) -> bool:
@@ -85,13 +85,13 @@
         if self.begin_at and self.sleep_at:
             is_sleeping = self.sleep_at > self.begin_at
 
         return is_sleeping
 
     @computed_field(description='The Time to sleep remaining')
     @property
-    def next_sleep_duration(self) -> float | None:
+    def next_sleep_duration(self) -> float | int | None:
         if self.is_processing:
             time_since_start = (datetime.now(tz=timezone.utc) - self.begin_at).total_seconds()
             diff = max(self.every_in_seconds - time_since_start, 0)
 
             return self.every_in_seconds if not self.remove_running_time else diff
```

### Comparing `edgegap_scheduling-1.2.0/pyproject.toml` & `edgegap_scheduling-1.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "edgegap-scheduling"
-version = "1.2.0"
-description = "The Edgegap Scheduling library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization."
+version = "1.5.0"
+description = "The Edgegap library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.7.1"
 pytimeparse = "^1.1.8"
```

### Comparing `edgegap_scheduling-1.2.0/PKG-INFO` & `edgegap_scheduling-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: edgegap-scheduling
-Version: 1.2.0
-Summary: The Edgegap Scheduling library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization.
+Version: 1.5.0
+Summary: The Edgegap library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: edgegap-logging (>=1.0.0,<2.0.0)
```

