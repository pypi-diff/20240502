# Comparing `tmp/rutificador-0.0.1.tar.gz` & `tmp/rutificador-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.0.1.tar", max compression
+gzip compressed data, was "rutificador-0.0.2.tar", max compression
```

## Comparing `rutificador-0.0.1.tar` & `rutificador-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-02 20:04:31.149923 rutificador-0.0.1/LICENSE
--rw-r--r--   0        0        0     4232 2024-05-02 20:04:31.149923 rutificador-0.0.1/README.md
--rw-r--r--   0        0        0     1071 2024-05-02 20:04:31.149923 rutificador-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-02 20:04:31.149923 rutificador-0.0.1/rutificador/__init__.py
--rw-r--r--   0        0        0     9113 2024-05-02 20:04:31.149923 rutificador-0.0.1/rutificador/rutificador.py
--rw-r--r--   0        0        0     5143 1970-01-01 00:00:00.000000 rutificador-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-02 20:31:15.457230 rutificador-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4232 2024-05-02 20:31:15.461230 rutificador-0.0.2/README.md
+-rw-r--r--   0        0        0     1130 2024-05-02 20:31:15.461230 rutificador-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-02 20:31:15.461230 rutificador-0.0.2/rutificador/__init__.py
+-rw-r--r--   0        0        0     9113 2024-05-02 20:31:15.461230 rutificador-0.0.2/rutificador/rutificador.py
+-rw-r--r--   0        0        0     5143 1970-01-01 00:00:00.000000 rutificador-0.0.2/PKG-INFO
```

### Comparing `rutificador-0.0.1/LICENSE` & `rutificador-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.0.1/README.md` & `rutificador-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rutificador-0.0.1/pyproject.toml` & `rutificador-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Rutificador"
-version = "0.0.1"
+version = "0.0.2"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo"]
 classifiers = [
@@ -29,7 +29,12 @@
 testpaths = ["tests"]
 addopts = "--import-mode=importlib"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+[project]
+packages = [
+    { include = 'rutificador' },
+]
+
```

### Comparing `rutificador-0.0.1/rutificador/rutificador.py` & `rutificador-0.0.2/rutificador/rutificador.py`

 * *Files identical despite different names*

### Comparing `rutificador-0.0.1/PKG-INFO` & `rutificador-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Rutificador
-Version: 0.0.1
+Version: 0.0.2
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://
 License: MIT
 Keywords: RUT,Chile,validación,formateo
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
```

