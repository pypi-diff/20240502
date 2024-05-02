# Comparing `tmp/fps_auth_jupyterhub-0.5.1.tar.gz` & `tmp/fps_auth_jupyterhub-0.5.2.tar.gz`

## Comparing `fps_auth_jupyterhub-0.5.1.tar` & `fps_auth_jupyterhub-0.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/fps_auth_jupyterhub/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/fps_auth_jupyterhub/config.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/fps_auth_jupyterhub/db.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/fps_auth_jupyterhub/launch.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/fps_auth_jupyterhub/main.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/fps_auth_jupyterhub/models.py
--rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/fps_auth_jupyterhub/routes.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/COPYING.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/README.md
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/fps_auth_jupyterhub/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/fps_auth_jupyterhub/config.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/fps_auth_jupyterhub/db.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/fps_auth_jupyterhub/launch.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/fps_auth_jupyterhub/main.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/fps_auth_jupyterhub/models.py
+-rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/fps_auth_jupyterhub/routes.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/COPYING.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/README.md
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fps_auth_jupyterhub-0.5.2/PKG-INFO
```

### Comparing `fps_auth_jupyterhub-0.5.1/fps_auth_jupyterhub/db.py` & `fps_auth_jupyterhub-0.5.2/fps_auth_jupyterhub/db.py`

 * *Files identical despite different names*

### Comparing `fps_auth_jupyterhub-0.5.1/fps_auth_jupyterhub/main.py` & `fps_auth_jupyterhub-0.5.2/fps_auth_jupyterhub/main.py`

 * *Files identical despite different names*

### Comparing `fps_auth_jupyterhub-0.5.1/fps_auth_jupyterhub/routes.py` & `fps_auth_jupyterhub-0.5.2/fps_auth_jupyterhub/routes.py`

 * *Files identical despite different names*

### Comparing `fps_auth_jupyterhub-0.5.1/.gitignore` & `fps_auth_jupyterhub-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_auth_jupyterhub-0.5.1/COPYING.md` & `fps_auth_jupyterhub-0.5.2/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_auth_jupyterhub-0.5.1/pyproject.toml` & `fps_auth_jupyterhub-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_auth_jupyterhub-0.5.1/PKG-INFO` & `fps_auth_jupyterhub-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fps_auth_jupyterhub
-Version: 0.5.1
+Version: 0.5.2
 Summary: An FPS plugin for the authentication API, using JupyterHbu
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

