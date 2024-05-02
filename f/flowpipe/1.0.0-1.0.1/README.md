# Comparing `tmp/flowpipe-1.0.0.tar.gz` & `tmp/flowpipe-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowpipe-1.0.0.tar", max compression
+gzip compressed data, was "flowpipe-1.0.1.tar", max compression
```

## Comparing `flowpipe-1.0.0.tar` & `flowpipe-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2023-12-20 09:25:06.975041 flowpipe-1.0.0/LICENSE
--rw-r--r--   0        0        0    10696 2023-12-20 09:25:06.975041 flowpipe-1.0.0/README.md
--rw-r--r--   0        0        0      245 2023-12-20 09:25:06.979041 flowpipe-1.0.0/flowpipe/__init__.py
--rw-r--r--   0        0        0      281 2023-12-20 09:25:06.979041 flowpipe-1.0.0/flowpipe/errors.py
--rw-r--r--   0        0        0    10700 2023-12-20 09:25:06.979041 flowpipe-1.0.0/flowpipe/evaluator.py
--rw-r--r--   0        0        0     1644 2023-12-20 09:25:06.979041 flowpipe-1.0.0/flowpipe/event.py
--rw-r--r--   0        0        0    17956 2023-12-20 09:25:06.979041 flowpipe-1.0.0/flowpipe/graph.py
--rw-r--r--   0        0        0    25097 2023-12-20 09:25:06.979041 flowpipe-1.0.0/flowpipe/node.py
--rw-r--r--   0        0        0    15375 2023-12-20 09:25:06.979041 flowpipe-1.0.0/flowpipe/plug.py
--rw-r--r--   0        0        0     4533 2023-12-20 09:25:06.979041 flowpipe-1.0.0/flowpipe/utilities.py
--rw-r--r--   0        0        0     1340 2023-12-20 09:25:06.979041 flowpipe-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    11579 1970-01-01 00:00:00.000000 flowpipe-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-02 11:54:29.173445 flowpipe-1.0.1/LICENSE
+-rw-r--r--   0        0        0    10696 2024-05-02 11:54:29.173445 flowpipe-1.0.1/README.md
+-rw-r--r--   0        0        0      245 2024-05-02 11:54:29.173445 flowpipe-1.0.1/flowpipe/__init__.py
+-rw-r--r--   0        0        0      281 2024-05-02 11:54:29.173445 flowpipe-1.0.1/flowpipe/errors.py
+-rw-r--r--   0        0        0    10700 2024-05-02 11:54:29.173445 flowpipe-1.0.1/flowpipe/evaluator.py
+-rw-r--r--   0        0        0     1644 2024-05-02 11:54:29.173445 flowpipe-1.0.1/flowpipe/event.py
+-rw-r--r--   0        0        0    17956 2024-05-02 11:54:29.173445 flowpipe-1.0.1/flowpipe/graph.py
+-rw-r--r--   0        0        0    25097 2024-05-02 11:54:29.173445 flowpipe-1.0.1/flowpipe/node.py
+-rw-r--r--   0        0        0    15375 2024-05-02 11:54:29.173445 flowpipe-1.0.1/flowpipe/plug.py
+-rw-r--r--   0        0        0     4568 2024-05-02 11:54:29.173445 flowpipe-1.0.1/flowpipe/utilities.py
+-rw-r--r--   0        0        0     1340 2024-05-02 11:54:29.173445 flowpipe-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11579 1970-01-01 00:00:00.000000 flowpipe-1.0.1/PKG-INFO
```

### Comparing `flowpipe-1.0.0/LICENSE` & `flowpipe-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flowpipe-1.0.0/README.md` & `flowpipe-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `flowpipe-1.0.0/flowpipe/evaluator.py` & `flowpipe-1.0.1/flowpipe/evaluator.py`

 * *Files identical despite different names*

### Comparing `flowpipe-1.0.0/flowpipe/event.py` & `flowpipe-1.0.1/flowpipe/event.py`

 * *Files identical despite different names*

### Comparing `flowpipe-1.0.0/flowpipe/graph.py` & `flowpipe-1.0.1/flowpipe/graph.py`

 * *Files identical despite different names*

### Comparing `flowpipe-1.0.0/flowpipe/node.py` & `flowpipe-1.0.1/flowpipe/node.py`

 * *Files identical despite different names*

### Comparing `flowpipe-1.0.0/flowpipe/plug.py` & `flowpipe-1.0.1/flowpipe/plug.py`

 * *Files identical despite different names*

### Comparing `flowpipe-1.0.0/flowpipe/utilities.py` & `flowpipe-1.0.1/flowpipe/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         cls = getattr(module, cls_name)
     except AttributeError:  # pragma: no cover
         loader = importlib.machinery.SourceFileLoader("module", file_location)
         spec = importlib.machinery.ModuleSpec(
             "module", loader, origin=file_location
         )
         module = importlib.util.module_from_spec(spec)
+        loader.exec_module(module)
         cls = getattr(module, cls_name)
     return cls
 
 
 def deserialize_node(data):
     """De-serialize a node from the given json data."""
     node = import_class(data["module"], data["cls"], data["file_location"])(
```

### Comparing `flowpipe-1.0.0/pyproject.toml` & `flowpipe-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "too-few-public-methods",
     "too-many-instance-attributes",
     "too-many-public-methods",
 ]
 
 [tool.poetry]
 name = "Flowpipe"
-version = "1.0.0"
+version = "1.0.1"
 description = "A lightweight framework for flow-based programming in python."
 authors = ["Paul Schweizer <paulschweizer@gmx.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/PaulSchweizer/flowpipe"
 documentation = "https://flowpipe.readthedocs.io/en/latest/"
 classifiers = [
```

### Comparing `flowpipe-1.0.0/PKG-INFO` & `flowpipe-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowpipe
-Version: 1.0.0
+Version: 1.0.1
 Summary: A lightweight framework for flow-based programming in python.
 Home-page: https://github.com/PaulSchweizer/flowpipe
 License: MIT
 Author: Paul Schweizer
 Author-email: paulschweizer@gmx.net
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
```

