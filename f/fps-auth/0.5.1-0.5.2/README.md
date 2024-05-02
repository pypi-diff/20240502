# Comparing `tmp/fps_auth-0.5.1.tar.gz` & `tmp/fps_auth-0.5.2.tar.gz`

## Comparing `fps_auth-0.5.1.tar` & `fps_auth-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.5.1/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/__init__.py
--rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/config.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/main.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/py.typed
--rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 fps_auth-0.5.1/fps_auth/routes.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_auth-0.5.1/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.5.1/COPYING.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.5.1/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 fps_auth-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fps_auth-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.5.2/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.5.2/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 fps_auth-0.5.2/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_auth-0.5.2/fps_auth/config.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 fps_auth-0.5.2/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.5.2/fps_auth/main.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fps_auth-0.5.2/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.5.2/fps_auth/py.typed
+-rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 fps_auth-0.5.2/fps_auth/routes.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_auth-0.5.2/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.5.2/COPYING.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.5.2/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 fps_auth-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fps_auth-0.5.2/PKG-INFO
```

### Comparing `fps_auth-0.5.1/fps_auth/backends.py` & `fps_auth-0.5.2/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.1/fps_auth/config.py` & `fps_auth-0.5.2/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.1/fps_auth/db.py` & `fps_auth-0.5.2/fps_auth/db.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.1/fps_auth/main.py` & `fps_auth-0.5.2/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.1/fps_auth/routes.py` & `fps_auth-0.5.2/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.1/.gitignore` & `fps_auth-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.1/COPYING.md` & `fps_auth-0.5.2/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.1/pyproject.toml` & `fps_auth-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_auth-0.5.1/PKG-INFO` & `fps_auth-0.5.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fps_auth
-Version: 0.5.1
+Version: 0.5.2
 Summary: An FPS plugin for the authentication API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

