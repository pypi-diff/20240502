# Comparing `tmp/aioclock-0.0.3.tar.gz` & `tmp/aioclock-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioclock-0.0.3.tar", max compression
+gzip compressed data, was "aioclock-0.0.4.tar", max compression
```

## Comparing `aioclock-0.0.3.tar` & `aioclock-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-04-13 06:08:52.101327 aioclock-0.0.3/LICENSE
--rw-r--r--   0        0        0     3674 2024-04-13 06:08:52.101327 aioclock-0.0.3/README.md
--rw-r--r--   0        0        0      299 2024-04-13 06:08:52.101327 aioclock-0.0.3/aioclock/__init__.py
--rw-r--r--   0        0        0     2495 2024-04-13 06:08:52.101327 aioclock-0.0.3/aioclock/app.py
--rw-r--r--   0        0        0     1182 2024-04-13 06:08:52.101327 aioclock-0.0.3/aioclock/group.py
--rw-r--r--   0        0        0       55 2024-04-13 06:08:52.101327 aioclock-0.0.3/aioclock/logger.py
--rw-r--r--   0        0        0      122 2024-04-13 06:08:52.101327 aioclock-0.0.3/aioclock/provider.py
--rw-r--r--   0        0        0      584 2024-04-13 06:08:52.101327 aioclock-0.0.3/aioclock/task.py
--rw-r--r--   0        0        0     6452 2024-04-13 06:08:52.101327 aioclock-0.0.3/aioclock/triggers.py
--rw-r--r--   0        0        0     1042 2024-04-13 06:08:52.101327 aioclock-0.0.3/aioclock/types.py
--rw-r--r--   0        0        0      862 2024-04-13 06:08:52.101327 aioclock-0.0.3/aioclock/utils.py
--rw-r--r--   0        0        0     1966 2024-04-13 06:09:16.045426 aioclock-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4617 1970-01-01 00:00:00.000000 aioclock-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-02 16:48:08.901821 aioclock-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3674 2024-05-02 16:48:08.901821 aioclock-0.0.4/README.md
+-rw-r--r--   0        0        0      299 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/__init__.py
+-rw-r--r--   0        0        0     2495 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/app.py
+-rw-r--r--   0        0        0     1182 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/group.py
+-rw-r--r--   0        0        0       55 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/logger.py
+-rw-r--r--   0        0        0      122 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/provider.py
+-rw-r--r--   0        0        0      779 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/task.py
+-rw-r--r--   0        0        0     7706 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/triggers.py
+-rw-r--r--   0        0        0     1042 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/types.py
+-rw-r--r--   0        0        0      862 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/utils.py
+-rw-r--r--   0        0        0     1966 2024-05-02 16:48:35.150003 aioclock-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4617 1970-01-01 00:00:00.000000 aioclock-0.0.4/PKG-INFO
```

### Comparing `aioclock-0.0.3/LICENSE` & `aioclock-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.3/README.md` & `aioclock-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.3/aioclock/app.py` & `aioclock-0.0.4/aioclock/app.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.3/aioclock/group.py` & `aioclock-0.0.4/aioclock/group.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.3/aioclock/task.py` & `aioclock-0.0.4/aioclock/task.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,12 +9,15 @@
 class Task:
     func: Callable[..., Any]
     trigger: BaseTrigger
 
     async def run(self):
         while self.trigger.should_trigger():
             try:
+                next_trigger = await self.trigger.get_waiting_time_till_next_trigger()
+                if next_trigger:
+                    logger.info(f"Triggering next task in {next_trigger}")
                 await self.trigger.trigger_next()
                 logger.debug(f"Running task {self.func.__name__}")
                 await self.func()
             except Exception as error:
                 logger.error(f"Error running task {self.func.__name__}: {error}")
```

### Comparing `aioclock-0.0.3/aioclock/types.py` & `aioclock-0.0.4/aioclock/types.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.3/aioclock/utils.py` & `aioclock-0.0.4/aioclock/utils.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.3/pyproject.toml` & `aioclock-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioclock"
-version = "0.0.3"
+version = "0.0.4"
 description = "An asyncio-based scheduling framework designed for execution of periodic task with integrated support for dependency injection, enabling efficient and flexiable task management"
 authors = ["Mani Mozaffar <fmani.mozaffar@gmail.com>"]
 repository = "https://github.com/ManiMozaffar/aioclock"
 documentation = "https://ManiMozaffar.github.io/aioclock/"
 readme = "README.md"
 packages = [{ include = "aioclock" }]
```

### Comparing `aioclock-0.0.3/PKG-INFO` & `aioclock-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioclock
-Version: 0.0.3
+Version: 0.0.4
 Summary: An asyncio-based scheduling framework designed for execution of periodic task with integrated support for dependency injection, enabling efficient and flexiable task management
 Home-page: https://github.com/ManiMozaffar/aioclock
 Author: Mani Mozaffar
 Author-email: fmani.mozaffar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

