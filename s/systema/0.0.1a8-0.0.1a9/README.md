# Comparing `tmp/systema-0.0.1a8.tar.gz` & `tmp/systema-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systema-0.0.1a8.tar", max compression
+gzip compressed data, was "systema-0.0.1a9.tar", max compression
```

## Comparing `systema-0.0.1a8.tar` & `systema-0.0.1a9.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      389 2024-02-19 14:55:46.299732 systema-0.0.1a8/README.md
--rw-r--r--   0        0        0     1179 2024-02-20 20:39:21.296470 systema-0.0.1a8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-20 01:01:57.424523 systema-0.0.1a8/systema/__init__.py
--rw-r--r--   0        0        0       59 2024-02-16 20:05:37.769344 systema-0.0.1a8/systema/__main__.py
--rw-r--r--   0        0        0       20 2024-02-20 20:39:21.286470 systema-0.0.1a8/systema/__version__.py
--rw-r--r--   0        0        0     2371 2024-02-20 20:38:46.329624 systema-0.0.1a8/systema/cli.py
--rw-r--r--   0        0        0     1626 2024-02-20 19:55:27.634082 systema-0.0.1a8/systema/management.py
--rw-r--r--   0        0        0      151 2024-02-20 19:56:15.417575 systema-0.0.1a8/systema/security.py
--rw-r--r--   0        0        0        0 2024-02-16 17:46:15.526105 systema-0.0.1a8/systema/server/__init__.py
--rw-r--r--   0        0        0     1256 2024-02-20 01:27:57.174754 systema-0.0.1a8/systema/server/auth/endpoints.py
--rw-r--r--   0        0        0      355 2024-02-20 00:31:19.469731 systema-0.0.1a8/systema/server/auth/models.py
--rw-r--r--   0        0        0     3070 2024-02-20 19:05:54.912639 systema-0.0.1a8/systema/server/auth/utils.py
--rw-r--r--   0        0        0      259 2024-02-20 18:54:09.172521 systema-0.0.1a8/systema/server/db.py
--rw-r--r--   0        0        0      854 2024-02-20 20:19:57.067790 systema-0.0.1a8/systema/server/main.py
--rw-r--r--   0        0        0     2194 2024-02-20 19:39:12.115949 systema-0.0.1a8/systema/server/project_manager/endpoints/project.py
--rw-r--r--   0        0        0     2755 2024-02-20 20:15:02.870090 systema-0.0.1a8/systema/server/project_manager/endpoints/task.py
--rw-r--r--   0        0        0        0 2024-02-19 14:36:18.750685 systema-0.0.1a8/systema/server/project_manager/models/__init__.py
--rw-r--r--   0        0        0      464 2024-02-20 20:01:42.934707 systema-0.0.1a8/systema/server/project_manager/models/project.py
--rw-r--r--   0        0        0      712 2024-02-20 20:19:47.331080 systema-0.0.1a8/systema/server/project_manager/models/task.py
--rw-r--r--   0        0        0      455 2024-02-20 20:32:06.924371 systema-0.0.1a8/systema/tui/app.py
--rw-r--r--   0        0        0      369 2024-02-20 19:59:58.561273 systema-0.0.1a8/systema/utils.py
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 systema-0.0.1a8/PKG-INFO
+-rw-r--r--   0        0        0      389 2024-02-19 14:55:46.299732 systema-0.0.1a9/README.md
+-rw-r--r--   0        0        0     1179 2024-02-21 03:44:32.915215 systema-0.0.1a9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-20 01:01:57.424523 systema-0.0.1a9/systema/__init__.py
+-rw-r--r--   0        0        0       59 2024-02-16 20:05:37.769344 systema-0.0.1a9/systema/__main__.py
+-rw-r--r--   0        0        0       20 2024-02-21 03:44:32.905215 systema-0.0.1a9/systema/__version__.py
+-rw-r--r--   0        0        0     2408 2024-02-21 03:41:18.221102 systema-0.0.1a9/systema/cli.py
+-rw-r--r--   0        0        0     1626 2024-02-20 19:55:27.634082 systema-0.0.1a9/systema/management.py
+-rw-r--r--   0        0        0      151 2024-02-20 19:56:15.417575 systema-0.0.1a9/systema/security.py
+-rw-r--r--   0        0        0        0 2024-02-16 17:46:15.526105 systema-0.0.1a9/systema/server/__init__.py
+-rw-r--r--   0        0        0     1256 2024-02-20 01:27:57.174754 systema-0.0.1a9/systema/server/auth/endpoints.py
+-rw-r--r--   0        0        0      355 2024-02-20 00:31:19.469731 systema-0.0.1a9/systema/server/auth/models.py
+-rw-r--r--   0        0        0     3070 2024-02-20 19:05:54.912639 systema-0.0.1a9/systema/server/auth/utils.py
+-rw-r--r--   0        0        0      259 2024-02-20 18:54:09.172521 systema-0.0.1a9/systema/server/db.py
+-rw-r--r--   0        0        0      854 2024-02-20 20:19:57.067790 systema-0.0.1a9/systema/server/main.py
+-rw-r--r--   0        0        0     2194 2024-02-20 19:39:12.115949 systema-0.0.1a9/systema/server/project_manager/endpoints/project.py
+-rw-r--r--   0        0        0     2755 2024-02-20 20:15:02.870090 systema-0.0.1a9/systema/server/project_manager/endpoints/task.py
+-rw-r--r--   0        0        0        0 2024-02-19 14:36:18.750685 systema-0.0.1a9/systema/server/project_manager/models/__init__.py
+-rw-r--r--   0        0        0     1076 2024-02-21 03:41:18.221102 systema-0.0.1a9/systema/server/project_manager/models/project.py
+-rw-r--r--   0        0        0      712 2024-02-20 20:19:47.331080 systema-0.0.1a9/systema/server/project_manager/models/task.py
+-rw-r--r--   0        0        0     2818 2024-02-21 03:40:28.277569 systema-0.0.1a9/systema/tui/app.py
+-rw-r--r--   0        0        0      453 2024-02-21 03:21:11.449651 systema-0.0.1a9/systema/tui/proxy.py
+-rw-r--r--   0        0        0     1283 2024-02-21 03:40:24.387554 systema-0.0.1a9/systema/tui/screens.py
+-rw-r--r--   0        0        0      369 2024-02-20 19:59:58.561273 systema-0.0.1a9/systema/utils.py
+-rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 systema-0.0.1a9/PKG-INFO
```

### Comparing `systema-0.0.1a8/pyproject.toml` & `systema-0.0.1a9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "systema"
-version = "0.0.1a8"
+version = "0.0.1a9"
 description = ""
 authors = ["Rodrigo Eiti Kimura <rodrigoeitikimura@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.109.2"
@@ -40,15 +40,15 @@
 
 [tool.ruff.lint]
 select = ["E4", "E7", "E9", "F", "W", "C901"]
 extend-select = ["I"]
 ignore = []
 
 [tool.commitizen]
-version = "0.0.1a8"
+version = "0.0.1a9"
 tag_format = "v$version"
 version_files = [
     "systema/__version__.py",
     "pyproject.toml:version",
 ]
 
 [tool.pyright]
```

### Comparing `systema-0.0.1a8/systema/cli.py` & `systema-0.0.1a9/systema/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 def serve(dev: bool = typer.Option(False)):
     _serve(dev=dev)
 
 
 @app.command(help="Start TUI client")
 def tui(
     remote: bool = typer.Option(False, help="Enable access to remote server via HTTP"),
+    dev: bool = typer.Option(False),
 ):
     if remote:
         raise NotImplementedError("Sorry! Not available yet.")
 
     app = SystemaTUIApp()
     app.run()
```

### Comparing `systema-0.0.1a8/systema/management.py` & `systema-0.0.1a9/systema/management.py`

 * *Files identical despite different names*

### Comparing `systema-0.0.1a8/systema/server/auth/endpoints.py` & `systema-0.0.1a9/systema/server/auth/endpoints.py`

 * *Files identical despite different names*

### Comparing `systema-0.0.1a8/systema/server/auth/utils.py` & `systema-0.0.1a9/systema/server/auth/utils.py`

 * *Files identical despite different names*

### Comparing `systema-0.0.1a8/systema/server/main.py` & `systema-0.0.1a9/systema/server/main.py`

 * *Files identical despite different names*

### Comparing `systema-0.0.1a8/systema/server/project_manager/endpoints/project.py` & `systema-0.0.1a9/systema/server/project_manager/endpoints/project.py`

 * *Files identical despite different names*

### Comparing `systema-0.0.1a8/systema/server/project_manager/endpoints/task.py` & `systema-0.0.1a9/systema/server/project_manager/endpoints/task.py`

 * *Files identical despite different names*

### Comparing `systema-0.0.1a8/systema/server/project_manager/models/task.py` & `systema-0.0.1a9/systema/server/project_manager/models/task.py`

 * *Files identical despite different names*

### Comparing `systema-0.0.1a8/PKG-INFO` & `systema-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systema
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: 
 Author: Rodrigo Eiti Kimura
 Author-email: rodrigoeitikimura@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

