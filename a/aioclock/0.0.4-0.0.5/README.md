# Comparing `tmp/aioclock-0.0.4.tar.gz` & `tmp/aioclock-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioclock-0.0.4.tar", max compression
+gzip compressed data, was "aioclock-0.0.5.tar", max compression
```

## Comparing `aioclock-0.0.4.tar` & `aioclock-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-05-02 16:48:08.901821 aioclock-0.0.4/LICENSE
--rw-r--r--   0        0        0     3674 2024-05-02 16:48:08.901821 aioclock-0.0.4/README.md
--rw-r--r--   0        0        0      299 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/__init__.py
--rw-r--r--   0        0        0     2495 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/app.py
--rw-r--r--   0        0        0     1182 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/group.py
--rw-r--r--   0        0        0       55 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/logger.py
--rw-r--r--   0        0        0      122 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/provider.py
--rw-r--r--   0        0        0      779 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/task.py
--rw-r--r--   0        0        0     7706 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/triggers.py
--rw-r--r--   0        0        0     1042 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/types.py
--rw-r--r--   0        0        0      862 2024-05-02 16:48:08.901821 aioclock-0.0.4/aioclock/utils.py
--rw-r--r--   0        0        0     1966 2024-05-02 16:48:35.150003 aioclock-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4617 1970-01-01 00:00:00.000000 aioclock-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-02 16:52:15.471454 aioclock-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3674 2024-05-02 16:52:15.471454 aioclock-0.0.5/README.md
+-rw-r--r--   0        0        0      299 2024-05-02 16:52:15.471454 aioclock-0.0.5/aioclock/__init__.py
+-rw-r--r--   0        0        0     2495 2024-05-02 16:52:15.471454 aioclock-0.0.5/aioclock/app.py
+-rw-r--r--   0        0        0     1182 2024-05-02 16:52:15.471454 aioclock-0.0.5/aioclock/group.py
+-rw-r--r--   0        0        0       55 2024-05-02 16:52:15.471454 aioclock-0.0.5/aioclock/logger.py
+-rw-r--r--   0        0        0      122 2024-05-02 16:52:15.471454 aioclock-0.0.5/aioclock/provider.py
+-rw-r--r--   0        0        0      779 2024-05-02 16:52:15.471454 aioclock-0.0.5/aioclock/task.py
+-rw-r--r--   0        0        0     7712 2024-05-02 16:52:15.475454 aioclock-0.0.5/aioclock/triggers.py
+-rw-r--r--   0        0        0     1042 2024-05-02 16:52:15.475454 aioclock-0.0.5/aioclock/types.py
+-rw-r--r--   0        0        0      862 2024-05-02 16:52:15.475454 aioclock-0.0.5/aioclock/utils.py
+-rw-r--r--   0        0        0     1966 2024-05-02 16:52:37.123337 aioclock-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4617 1970-01-01 00:00:00.000000 aioclock-0.0.5/PKG-INFO
```

### Comparing `aioclock-0.0.4/LICENSE` & `aioclock-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.4/README.md` & `aioclock-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.4/aioclock/app.py` & `aioclock-0.0.5/aioclock/app.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.4/aioclock/group.py` & `aioclock-0.0.5/aioclock/group.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.4/aioclock/task.py` & `aioclock-0.0.5/aioclock/task.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.4/aioclock/triggers.py` & `aioclock-0.0.5/aioclock/triggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def should_trigger(self) -> bool:
         """
         `should_trigger` checks if the event should be triggered or not.
         """
         return True
 
     @abstractmethod
-    async def get_waiting_time_till_next_trigger(self) -> float | None:
+    async def get_waiting_time_till_next_trigger(self) -> Union[float, None]:
         """
         `get_waiting_time_till_next_trigger` returns the time in seconds, after which the event should be triggered.
         Returns None, if the event should not trigger anymore.
         """
         ...
```

### Comparing `aioclock-0.0.4/aioclock/types.py` & `aioclock-0.0.5/aioclock/types.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.4/aioclock/utils.py` & `aioclock-0.0.5/aioclock/utils.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.4/pyproject.toml` & `aioclock-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioclock"
-version = "0.0.4"
+version = "0.0.5"
 description = "An asyncio-based scheduling framework designed for execution of periodic task with integrated support for dependency injection, enabling efficient and flexiable task management"
 authors = ["Mani Mozaffar <fmani.mozaffar@gmail.com>"]
 repository = "https://github.com/ManiMozaffar/aioclock"
 documentation = "https://ManiMozaffar.github.io/aioclock/"
 readme = "README.md"
 packages = [{ include = "aioclock" }]
```

### Comparing `aioclock-0.0.4/PKG-INFO` & `aioclock-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioclock
-Version: 0.0.4
+Version: 0.0.5
 Summary: An asyncio-based scheduling framework designed for execution of periodic task with integrated support for dependency injection, enabling efficient and flexiable task management
 Home-page: https://github.com/ManiMozaffar/aioclock
 Author: Mani Mozaffar
 Author-email: fmani.mozaffar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

