# Comparing `tmp/weba-0.0.8.tar.gz` & `tmp/weba-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weba-0.0.8.tar", max compression
+gzip compressed data, was "weba-0.0.9.tar", max compression
```

## Comparing `weba-0.0.8.tar` & `weba-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       80 2023-09-06 20:16:50.122418 weba-0.0.8/README.md
--rw-r--r--   0        0        0     2825 2023-09-22 19:12:36.938938 weba-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      924 2023-09-22 16:31:19.089593 weba-0.0.8/weba/__init__.py
--rw-r--r--   0        0        0     2976 2023-09-22 16:25:37.157697 weba-0.0.8/weba/app.py
--rw-r--r--   0        0        0      144 2023-09-22 16:31:19.089895 weba-0.0.8/weba/base/__init__.py
--rw-r--r--   0        0        0     1016 2023-09-22 16:31:19.090304 weba-0.0.8/weba/base/component.py
--rw-r--r--   0        0        0     2659 2023-09-22 16:31:19.090472 weba-0.0.8/weba/base/page.py
--rw-r--r--   0        0        0    12292 2023-09-22 18:54:55.803445 weba-0.0.8/weba/build.py
--rw-r--r--   0        0        0      169 2023-09-20 22:19:09.183713 weba-0.0.8/weba/cache.py
--rw-r--r--   0        0        0       72 2023-09-20 22:19:09.184115 weba-0.0.8/weba/components/__init__.py
--rw-r--r--   0        0        0      401 2023-09-22 19:10:04.096569 weba-0.0.8/weba/components/browser.py
--rw-r--r--   0        0        0     4055 2023-09-22 16:31:19.091507 weba-0.0.8/weba/document.py
--rw-r--r--   0        0        0     1590 2023-09-20 22:19:09.184901 weba-0.0.8/weba/dominate_overrides.py
--rw-r--r--   0        0        0     7158 2023-09-22 19:12:25.356506 weba-0.0.8/weba/env.py
--rw-r--r--   0        0        0      224 2023-09-20 22:19:09.185499 weba-0.0.8/weba/logger.py
--rw-r--r--   0        0        0      212 2023-09-20 22:19:09.185962 weba-0.0.8/weba/middleware/__init__.py
--rw-r--r--   0        0        0     2424 2023-09-22 16:31:19.092107 weba-0.0.8/weba/middleware/csrf.py
--rw-r--r--   0        0        0     1180 2023-09-22 17:04:46.749739 weba-0.0.8/weba/middleware/exceptions.py
--rw-r--r--   0        0        0     6313 2023-09-22 16:47:29.329101 weba-0.0.8/weba/middleware/weba.py
--rw-r--r--   0        0        0     2592 2023-09-22 18:36:45.131627 weba-0.0.8/weba/packages.py
--rw-r--r--   0        0        0      580 2023-09-22 16:31:19.092646 weba-0.0.8/weba/pages/404.py
--rw-r--r--   0        0        0      990 2023-09-22 19:09:13.322087 weba-0.0.8/weba/pages/500.py
--rw-r--r--   0        0        0     3268 2023-09-22 16:31:19.093247 weba-0.0.8/weba/tags.py
--rw-r--r--   0        0        0     2772 2023-09-22 16:20:59.969051 weba-0.0.8/weba/test.py
--rw-r--r--   0        0        0      107 2023-09-20 22:19:09.187476 weba-0.0.8/weba/ui.py
--rw-r--r--   0        0        0     7573 2023-09-22 16:31:19.093521 weba-0.0.8/weba/utils.py
--rw-r--r--   0        0        0     1767 2023-09-22 16:31:19.093795 weba-0.0.8/weba/weba.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 weba-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-09-06 20:16:50.122418 weba-0.0.9/README.md
+-rw-r--r--   0        0        0     2825 2023-09-22 19:49:23.490369 weba-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      924 2023-09-22 19:13:16.424743 weba-0.0.9/weba/__init__.py
+-rw-r--r--   0        0        0     2976 2023-09-22 19:13:16.425479 weba-0.0.9/weba/app.py
+-rw-r--r--   0        0        0      144 2023-09-22 19:13:16.425670 weba-0.0.9/weba/base/__init__.py
+-rw-r--r--   0        0        0     1016 2023-09-22 19:13:16.425835 weba-0.0.9/weba/base/component.py
+-rw-r--r--   0        0        0     2659 2023-09-22 19:13:16.425973 weba-0.0.9/weba/base/page.py
+-rw-r--r--   0        0        0    12292 2023-09-22 19:13:16.426372 weba-0.0.9/weba/build.py
+-rw-r--r--   0        0        0      169 2023-09-22 19:13:16.426989 weba-0.0.9/weba/cache.py
+-rw-r--r--   0        0        0       72 2023-09-22 19:13:16.427119 weba-0.0.9/weba/components/__init__.py
+-rw-r--r--   0        0        0      401 2023-09-22 19:13:16.427269 weba-0.0.9/weba/components/browser.py
+-rw-r--r--   0        0        0     4148 2023-09-22 19:42:40.134779 weba-0.0.9/weba/document.py
+-rw-r--r--   0        0        0     1590 2023-09-22 19:13:16.427676 weba-0.0.9/weba/dominate_overrides.py
+-rw-r--r--   0        0        0     7195 2023-09-22 19:41:10.813534 weba-0.0.9/weba/env.py
+-rw-r--r--   0        0        0      224 2023-09-22 19:13:16.428363 weba-0.0.9/weba/logger.py
+-rw-r--r--   0        0        0      212 2023-09-22 19:13:16.428858 weba-0.0.9/weba/middleware/__init__.py
+-rw-r--r--   0        0        0     2424 2023-09-22 19:13:16.428979 weba-0.0.9/weba/middleware/csrf.py
+-rw-r--r--   0        0        0     1180 2023-09-22 19:13:16.429254 weba-0.0.9/weba/middleware/exceptions.py
+-rw-r--r--   0        0        0     6313 2023-09-22 19:13:16.429751 weba-0.0.9/weba/middleware/weba.py
+-rw-r--r--   0        0        0     2592 2023-09-22 19:13:16.430143 weba-0.0.9/weba/packages.py
+-rw-r--r--   0        0        0      580 2023-09-22 19:13:16.430335 weba-0.0.9/weba/pages/404.py
+-rw-r--r--   0        0        0      990 2023-09-22 19:13:16.430505 weba-0.0.9/weba/pages/500.py
+-rw-r--r--   0        0        0     3268 2023-09-22 19:13:16.430646 weba-0.0.9/weba/tags.py
+-rw-r--r--   0        0        0     2772 2023-09-22 19:13:16.430995 weba-0.0.9/weba/test.py
+-rw-r--r--   0        0        0      107 2023-09-22 19:13:16.431212 weba-0.0.9/weba/ui.py
+-rw-r--r--   0        0        0     7573 2023-09-22 19:13:16.431377 weba-0.0.9/weba/utils.py
+-rw-r--r--   0        0        0     1767 2023-09-22 19:13:16.431551 weba-0.0.9/weba/weba.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 weba-0.0.9/PKG-INFO
```

### Comparing `weba-0.0.8/pyproject.toml` & `weba-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weba"
-version = "0.0.8"
+version = "0.0.9"
 description = "Build web applications using FastAPI, Htmx and Tailwind"
 authors = ["CJ Lazell <cjlazell@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "weba"}]
```

### Comparing `weba-0.0.8/weba/__init__.py` & `weba-0.0.9/weba/__init__.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/app.py` & `weba-0.0.9/weba/app.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/base/component.py` & `weba-0.0.9/weba/base/component.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/base/page.py` & `weba-0.0.9/weba/base/page.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/build.py` & `weba-0.0.9/weba/build.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/document.py` & `weba-0.0.9/weba/document.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from typing import Any, Optional
 
 import dominate
 import dominate.tags as t
 from dominate.util import raw  # type: ignore
 from fastapi import Request
 
@@ -85,14 +86,15 @@
     def _render_default_head(self) -> None:
         if self._weba_head_rendered:
             return
 
         with self.head:
             t.meta(charset="utf-8")
             t.meta(name="viewport", content="width=device-width, initial-scale=1")
+            t.meta(name="htmx-config", content=f"{json.dumps(env.htmx_config)}")
 
         self.head.add(load_script_tags())  # type: ignore
         self._weba_head_rendered = True
 
 
 def weba_document(request: Request) -> WebaDocument:
     return request.scope["weba_document"]
```

### Comparing `weba-0.0.8/weba/dominate_overrides.py` & `weba-0.0.9/weba/dominate_overrides.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/env.py` & `weba-0.0.9/weba/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
     In live_reload mode, these files in their own file, this results in larger files but quicker compile times.
     """
     css_files: List[str] = []
     js_files: List[str] = []
     htmx_version: str = "1.9.6"
     htmx_extentions: List[str] = ["head-support", "json-enc"]
     htmx_boost: bool = True
+    htmx_config: dict[str, Any] = {}
     ignored_folders: List[str] = [
         ".git",
         ".github",
         ".vscode",
         ".venv",
         "venv",
         "node_modules",
```

### Comparing `weba-0.0.8/weba/middleware/csrf.py` & `weba-0.0.9/weba/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/middleware/exceptions.py` & `weba-0.0.9/weba/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/middleware/weba.py` & `weba-0.0.9/weba/middleware/weba.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/packages.py` & `weba-0.0.9/weba/packages.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/pages/404.py` & `weba-0.0.9/weba/pages/404.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/pages/500.py` & `weba-0.0.9/weba/pages/500.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/tags.py` & `weba-0.0.9/weba/tags.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/test.py` & `weba-0.0.9/weba/test.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/utils.py` & `weba-0.0.9/weba/utils.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/weba/weba.py` & `weba-0.0.9/weba/weba.py`

 * *Files identical despite different names*

### Comparing `weba-0.0.8/PKG-INFO` & `weba-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weba
-Version: 0.0.8
+Version: 0.0.9
 Summary: Build web applications using FastAPI, Htmx and Tailwind
 License: MIT
 Author: CJ Lazell
 Author-email: cjlazell@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

