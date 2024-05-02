# Comparing `tmp/jupyverse_api-0.5.1.tar.gz` & `tmp/jupyverse_api-0.5.2.tar.gz`

## Comparing `jupyverse_api-0.5.1.tar` & `jupyverse_api-0.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/cli.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/py.typed
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/notebook/__init__.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/README.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 jupyverse_api-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/notebook/__init__.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/README.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 jupyverse_api-0.5.2/PKG-INFO
```

### Comparing `jupyverse_api-0.5.1/jupyverse_api/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict
 
 from pydantic import BaseModel
 
 from .app import App
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse_api-0.5.1/jupyverse_api/cli.py` & `jupyverse_api-0.5.2/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/app/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/auth/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/contents/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/contents/models.py` & `jupyverse_api-0.5.2/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/jupyterlab/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/kernels/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/kernels/models.py` & `jupyverse_api-0.5.2/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/lab/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/main/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/nbconvert/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/notebook/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/resource_usage/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/terminals/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/jupyverse_api/yjs/__init__.py` & `jupyverse_api-0.5.2/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/.gitignore` & `jupyverse_api-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/COPYING.md` & `jupyverse_api-0.5.2/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/pyproject.toml` & `jupyverse_api-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.5.1/PKG-INFO` & `jupyverse_api-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyverse_api
-Version: 0.5.1
+Version: 0.5.2
 Summary: The public API for Jupyverse
 Project-URL: Source, https://github.com/jupyter-server/jupyverse/jupyverse_api
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: api,jupyverse
 Classifier: Development Status :: 4 - Beta
```

