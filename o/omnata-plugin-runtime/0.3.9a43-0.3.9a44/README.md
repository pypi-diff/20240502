# Comparing `tmp/omnata_plugin_runtime-0.3.9a43.tar.gz` & `tmp/omnata_plugin_runtime-0.3.9a44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_plugin_runtime-0.3.9a43.tar", max compression
+gzip compressed data, was "omnata_plugin_runtime-0.3.9a44.tar", max compression
```

## Comparing `omnata_plugin_runtime-0.3.9a43.tar` & `omnata_plugin_runtime-0.3.9a44.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    26526 2024-02-29 05:14:21.737287 omnata_plugin_runtime-0.3.9a43/LICENSE
--rw-r--r--   0        0        0      433 2024-02-29 05:14:21.737287 omnata_plugin_runtime-0.3.9a43/README.md
--rw-r--r--   0        0        0     2007 2024-02-29 05:14:37.893874 omnata_plugin_runtime-0.3.9a43/pyproject.toml
--rw-r--r--   0        0        0     1214 2024-02-29 05:14:21.741287 omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/__init__.py
--rw-r--r--   0        0        0     6217 2024-02-29 05:14:21.741287 omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/api.py
--rw-r--r--   0        0        0    34742 2024-02-29 05:14:21.741287 omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/configuration.py
--rw-r--r--   0        0        0    18371 2024-02-29 05:14:21.741287 omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/forms.py
--rw-r--r--   0        0        0     3272 2024-02-29 05:14:21.741287 omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/logging.py
--rw-r--r--   0        0        0    89661 2024-02-29 05:14:21.741287 omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/omnata_plugin.py
--rw-r--r--   0        0        0    27670 2024-02-29 05:14:21.741287 omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/plugin_entrypoints.py
--rw-r--r--   0        0        0    16562 2024-02-29 05:14:21.741287 omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/rate_limiting.py
--rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.3.9a43/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-02-29 05:16:40.397442 omnata_plugin_runtime-0.3.9a44/LICENSE
+-rw-r--r--   0        0        0      433 2024-02-29 05:16:40.397442 omnata_plugin_runtime-0.3.9a44/README.md
+-rw-r--r--   0        0        0     2007 2024-02-29 05:17:02.549499 omnata_plugin_runtime-0.3.9a44/pyproject.toml
+-rw-r--r--   0        0        0     1214 2024-02-29 05:16:40.397442 omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/__init__.py
+-rw-r--r--   0        0        0     6217 2024-02-29 05:16:40.401442 omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/api.py
+-rw-r--r--   0        0        0    34742 2024-02-29 05:16:40.401442 omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/configuration.py
+-rw-r--r--   0        0        0    18371 2024-02-29 05:16:40.401442 omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/forms.py
+-rw-r--r--   0        0        0     3272 2024-02-29 05:16:40.401442 omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/logging.py
+-rw-r--r--   0        0        0    89661 2024-02-29 05:16:40.401442 omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/omnata_plugin.py
+-rw-r--r--   0        0        0    27670 2024-02-29 05:16:40.401442 omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/plugin_entrypoints.py
+-rw-r--r--   0        0        0    16562 2024-02-29 05:16:40.401442 omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/rate_limiting.py
+-rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 omnata_plugin_runtime-0.3.9a44/PKG-INFO
```

### Comparing `omnata_plugin_runtime-0.3.9a43/LICENSE` & `omnata_plugin_runtime-0.3.9a44/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.3.9a43/pyproject.toml` & `omnata_plugin_runtime-0.3.9a44/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omnata-plugin-runtime"
-version = "0.3.9-a43"
+version = "0.3.9-a44"
 description = "Classes and common runtime components for building and running Omnata Plugins"
 authors = ["James Weakley <james.weakley@omnata.com>"]
 readme = "README.md"
 packages = [{include = "omnata_plugin_runtime", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
```

### Comparing `omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/__init__.py` & `omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/api.py` & `omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/api.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/configuration.py` & `omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/configuration.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/forms.py` & `omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/forms.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/logging.py` & `omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/logging.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/omnata_plugin.py` & `omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/omnata_plugin.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/plugin_entrypoints.py` & `omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/plugin_entrypoints.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.3.9a43/src/omnata_plugin_runtime/rate_limiting.py` & `omnata_plugin_runtime-0.3.9a44/src/omnata_plugin_runtime/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `omnata_plugin_runtime-0.3.9a43/PKG-INFO` & `omnata_plugin_runtime-0.3.9a44/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnata-plugin-runtime
-Version: 0.3.9a43
+Version: 0.3.9a44
 Summary: Classes and common runtime components for building and running Omnata Plugins
 Author: James Weakley
 Author-email: james.weakley@omnata.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

