# Comparing `tmp/astx-0.9.0.tar.gz` & `tmp/astx-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astx-0.9.0.tar", max compression
+gzip compressed data, was "astx-0.9.1.tar", max compression
```

## Comparing `astx-0.9.0.tar` & `astx-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1498 2024-03-06 20:36:58.573550 astx-0.9.0/LICENSE
--rw-r--r--   0        0        0     2574 2024-03-06 20:36:58.577550 astx-0.9.0/docs/index.md
--rw-r--r--   0        0        0     2103 2024-03-06 20:38:05.449304 astx-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2633 2024-03-06 20:38:05.445304 astx-0.9.0/src/astx/__init__.py
--rw-r--r--   0        0        0     4839 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/base.py
--rw-r--r--   0        0        0     2036 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/blocks.py
--rw-r--r--   0        0        0     4359 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/callables.py
--rw-r--r--   0        0        0     7810 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/datatypes.py
--rw-r--r--   0        0        0     4336 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/flows.py
--rw-r--r--   0        0        0      392 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/mixes.py
--rw-r--r--   0        0        0      530 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/modifiers.py
--rw-r--r--   0        0        0      130 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/operators.py
--rw-r--r--   0        0        0        0 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/py.typed
--rw-r--r--   0        0        0     4263 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/symbol_table.py
--rw-r--r--   0        0        0     5451 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/variables.py
--rw-r--r--   0        0        0     2164 2024-03-06 20:36:58.581550 astx-0.9.0/src/astx/viz.py
--rw-r--r--   0        0        0     3266 1970-01-01 00:00:00.000000 astx-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-03-23 00:36:57.777600 astx-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2574 2024-03-23 00:36:57.781600 astx-0.9.1/docs/index.md
+-rw-r--r--   0        0        0     2103 2024-03-23 00:38:07.969226 astx-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2633 2024-03-23 00:38:07.969226 astx-0.9.1/src/astx/__init__.py
+-rw-r--r--   0        0        0     4839 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/base.py
+-rw-r--r--   0        0        0     2036 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/blocks.py
+-rw-r--r--   0        0        0     4359 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/callables.py
+-rw-r--r--   0        0        0     7810 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/datatypes.py
+-rw-r--r--   0        0        0     4336 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/flows.py
+-rw-r--r--   0        0        0      392 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/mixes.py
+-rw-r--r--   0        0        0      530 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/modifiers.py
+-rw-r--r--   0        0        0      130 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/operators.py
+-rw-r--r--   0        0        0        0 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/py.typed
+-rw-r--r--   0        0        0     4263 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/symbol_table.py
+-rw-r--r--   0        0        0     5451 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/variables.py
+-rw-r--r--   0        0        0     2164 2024-03-23 00:36:57.785600 astx-0.9.1/src/astx/viz.py
+-rw-r--r--   0        0        0     3266 1970-01-01 00:00:00.000000 astx-0.9.1/PKG-INFO
```

### Comparing `astx-0.9.0/LICENSE` & `astx-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astx-0.9.0/docs/index.md` & `astx-0.9.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `astx-0.9.0/pyproject.toml` & `astx-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "astx"
-version = "0.9.0"  # semantic-release
+version = "0.9.1"  # semantic-release
 description = "ASTx is an agnostic expression structure for AST."
 readme = "docs/index.md"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD 3 Clause"
 exclude = [
   ".git/*",
   ".env*",
@@ -37,15 +37,15 @@
 mkdocs-jupyter = ">=0.24.1"
 mkdocs-literate-nav = ">=0.6.0"
 mkdocs-macros-plugin = ">=0.7.0,<1"
 mkdocs-material = ">=9.1.15"
 mkdocstrings = ">=0.21.2"
 mkdocstrings-python = ">=1.1.2"
 jupyterlab = ">=4.0.5"
-makim = "1.10.0"
+makim = "1.14.0"
 umlizer = "^0.1.0"
 nbmake = ">=1.4.6"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
```

### Comparing `astx-0.9.0/src/astx/__init__.py` & `astx-0.9.1/src/astx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 
 def get_version() -> str:
     """Return the program version."""
     try:
         return importlib_metadata.version(__name__)
     except importlib_metadata.PackageNotFoundError:  # pragma: no cover
-        return "0.9.0"  # semantic-release
+        return "0.9.1"  # semantic-release
 
 
 __all__ = [
     "Argument",
     "AST",
     "ASTKind",
     "base",
```

### Comparing `astx-0.9.0/src/astx/base.py` & `astx-0.9.1/src/astx/base.py`

 * *Files identical despite different names*

### Comparing `astx-0.9.0/src/astx/blocks.py` & `astx-0.9.1/src/astx/blocks.py`

 * *Files identical despite different names*

### Comparing `astx-0.9.0/src/astx/callables.py` & `astx-0.9.1/src/astx/callables.py`

 * *Files identical despite different names*

### Comparing `astx-0.9.0/src/astx/datatypes.py` & `astx-0.9.1/src/astx/datatypes.py`

 * *Files identical despite different names*

### Comparing `astx-0.9.0/src/astx/flows.py` & `astx-0.9.1/src/astx/flows.py`

 * *Files identical despite different names*

### Comparing `astx-0.9.0/src/astx/modifiers.py` & `astx-0.9.1/src/astx/modifiers.py`

 * *Files identical despite different names*

### Comparing `astx-0.9.0/src/astx/symbol_table.py` & `astx-0.9.1/src/astx/symbol_table.py`

 * *Files identical despite different names*

### Comparing `astx-0.9.0/src/astx/variables.py` & `astx-0.9.1/src/astx/variables.py`

 * *Files identical despite different names*

### Comparing `astx-0.9.0/src/astx/viz.py` & `astx-0.9.1/src/astx/viz.py`

 * *Files identical despite different names*

### Comparing `astx-0.9.0/PKG-INFO` & `astx-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astx
-Version: 0.9.0
+Version: 0.9.1
 Summary: ASTx is an agnostic expression structure for AST.
 License: BSD 3 Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

