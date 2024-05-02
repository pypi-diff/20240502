# Comparing `tmp/data-place-0.2.1.tar.gz` & `tmp/data-place-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-place-0.2.1.tar", last modified: Sat Apr 27 12:41:23 2024, max compression
+gzip compressed data, was "data-place-0.2.2.tar", last modified: Thu May  2 20:31:18 2024, max compression
```

## Comparing `data-place-0.2.1.tar` & `data-place-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 12:41:23.158195 data-place-0.2.1/
--rw-rw-rw-   0        0        0       44 2024-04-27 12:41:23.000000 data-place-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6073 2024-04-27 12:41:23.157158 data-place-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.2.1/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.2.1/build.py
-drwxrwxrwx   0        0        0        0 2024-04-27 12:41:23.157158 data-place-0.2.1/data_place.egg-info/
--rw-rw-rw-   0        0        0     6073 2024-04-27 12:41:23.000000 data-place-0.2.1/data_place.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2024-04-27 12:41:23.000000 data-place-0.2.1/data_place.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 12:41:23.000000 data-place-0.2.1/data_place.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-27 12:41:23.000000 data-place-0.2.1/data_place.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-27 12:41:23.000000 data-place-0.2.1/data_place.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 12:41:23.155830 data-place-0.2.1/dataplace/
--rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.2.1/dataplace/__init__.py
--rw-rw-rw-   0        0        0     1611 2024-01-24 19:26:19.000000 data-place-0.2.1/dataplace/base.py
--rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.2.1/dataplace/callback.py
--rw-rw-rw-   0        0        0     2251 2024-01-27 16:19:43.000000 data-place-0.2.1/dataplace/control.py
--rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.2.1/dataplace/handler.py
--rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.2.1/dataplace/io.py
--rw-rw-rw-   0        0        0     8302 2024-01-26 07:10:39.000000 data-place-0.2.1/dataplace/receive.py
--rw-rw-rw-   0        0        0    10585 2024-01-26 07:23:18.000000 data-place-0.2.1/dataplace/send.py
--rw-rw-rw-   0        0        0     7260 2024-04-27 12:38:35.000000 data-place-0.2.1/dataplace/store.py
--rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 12:41:23.158195 data-place-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1615 2024-04-27 12:41:20.000000 data-place-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:31:18.841719 data-place-0.2.2/
+-rw-rw-rw-   0        0        0       44 2024-05-02 20:31:18.000000 data-place-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6073 2024-05-02 20:31:18.840721 data-place-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.2.2/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.2.2/build.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:31:18.839713 data-place-0.2.2/data_place.egg-info/
+-rw-rw-rw-   0        0        0     6073 2024-05-02 20:31:18.000000 data-place-0.2.2/data_place.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-05-02 20:31:18.000000 data-place-0.2.2/data_place.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 20:31:18.000000 data-place-0.2.2/data_place.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-02 20:31:18.000000 data-place-0.2.2/data_place.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-02 20:31:18.000000 data-place-0.2.2/data_place.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 20:31:18.838643 data-place-0.2.2/dataplace/
+-rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.2.2/dataplace/__init__.py
+-rw-rw-rw-   0        0        0     1611 2024-01-24 19:26:19.000000 data-place-0.2.2/dataplace/base.py
+-rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.2.2/dataplace/callback.py
+-rw-rw-rw-   0        0        0     3157 2024-05-02 20:31:15.000000 data-place-0.2.2/dataplace/control.py
+-rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.2.2/dataplace/handler.py
+-rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.2.2/dataplace/io.py
+-rw-rw-rw-   0        0        0     8302 2024-01-26 07:10:39.000000 data-place-0.2.2/dataplace/receive.py
+-rw-rw-rw-   0        0        0    10585 2024-01-26 07:23:18.000000 data-place-0.2.2/dataplace/send.py
+-rw-rw-rw-   0        0        0     7260 2024-04-27 12:38:35.000000 data-place-0.2.2/dataplace/store.py
+-rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 20:31:18.841719 data-place-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2024-05-02 20:31:15.000000 data-place-0.2.2/setup.py
```

### Comparing `data-place-0.2.1/PKG-INFO` & `data-place-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.2.1
+Version: 0.2.2
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.2.1/README.md` & `data-place-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `data-place-0.2.1/build.py` & `data-place-0.2.2/build.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.1/data_place.egg-info/PKG-INFO` & `data-place-0.2.2/data_place.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.2.1
+Version: 0.2.2
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.2.1/dataplace/base.py` & `data-place-0.2.2/dataplace/base.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.1/dataplace/callback.py` & `data-place-0.2.2/dataplace/callback.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.1/dataplace/control.py` & `data-place-0.2.2/dataplace/control.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # control.py
 
 import time
 from dataclasses import dataclass, field
 import asyncio
+from typing import Callable, Awaitable, Iterable
 
 from dataplace.io import ModelIO
 from dataplace.callback import Callback
 from dataplace.handler import Handler
 
 __all__ = [
-    "Controller"
+    "Controller",
+    "loop",
+    "async_loop"
 ]
 
 Data = ModelIO | object
 
 @dataclass
 class Controller:
 
@@ -92,7 +95,43 @@
         while self.paused:
             await asyncio.sleep(self.delay)
 
     def hold(self) -> None:
 
         while self.paused:
             time.sleep(self.delay)
+
+async def async_loop[T](
+        controller: Controller,
+        target: Callable[..., Awaitable[T]],
+        args: Iterable = None,
+        kwargs: dict[str, ...] = None,
+        results: list[T] = None
+) -> list[T]:
+
+    if results is None:
+        results = []
+
+    while controller.running:
+        results.append(await target(*args, **kwargs))
+
+        await controller.async_hold()
+
+    return results
+
+def loop[T](
+        controller: Controller,
+        target: Callable[..., Awaitable[T]],
+        args: Iterable = None,
+        kwargs: dict[str, ...] = None,
+        results: list[T] = None
+) -> list[T]:
+
+    if results is None:
+        results = []
+
+    while controller.running:
+        results.append(target(*args, **kwargs))
+
+        controller.hold()
+
+    return results
```

### Comparing `data-place-0.2.1/dataplace/handler.py` & `data-place-0.2.2/dataplace/handler.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.1/dataplace/io.py` & `data-place-0.2.2/dataplace/io.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.1/dataplace/receive.py` & `data-place-0.2.2/dataplace/receive.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.1/dataplace/send.py` & `data-place-0.2.2/dataplace/send.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.1/dataplace/store.py` & `data-place-0.2.2/dataplace/store.py`

 * *Files identical despite different names*

### Comparing `data-place-0.2.1/setup.py` & `data-place-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='data-place',
-        version='0.2.1',
+        version='0.2.2',
         description=(
             "A powerfull and flexible framework for designing async "
             "socket based data streaming and distribution systems, "
             "with automated parsing, dynamic data store and "
             "high-level control hooks."
         ),
         license='MIT',
```

