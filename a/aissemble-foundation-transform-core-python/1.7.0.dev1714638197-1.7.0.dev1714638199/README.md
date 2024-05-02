# Comparing `tmp/aissemble_foundation_transform_core_python-1.7.0.dev1714638197.tar.gz` & `tmp/aissemble_foundation_transform_core_python-1.7.0.dev1714638199.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_transform_core_python-1.7.0.dev1714638197.tar", max compression
+gzip compressed data, was "aissemble_foundation_transform_core_python-1.7.0.dev1714638199.tar", max compression
```

## Comparing `aissemble_foundation_transform_core_python-1.7.0.dev1714638197.tar` & `aissemble_foundation_transform_core_python-1.7.0.dev1714638199.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     9580 2024-05-02 08:23:07.112887 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/LICENSE
--rw-r--r--   0        0        0        0 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/README.md
--rw-r--r--   0        0        0      656 2024-05-02 08:23:17.590874 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/pyproject.toml
--rw-r--r--   0        0        0      244 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/__init__.py
--rw-r--r--   0        0        0      342 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/data_transform_exception.py
--rw-r--r--   0        0        0      507 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/mediator/__init__.py
--rw-r--r--   0        0        0      747 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/mediator/logging_mediator.py
--rw-r--r--   0        0        0     4333 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/mediator/mediation_manager.py
--rw-r--r--   0        0        0     1726 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/mediator/mediation_objects.py
--rw-r--r--   0        0        0     1374 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/mediator/mediator.py
--rw-r--r--   0        0        0      689 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/mediator/pass_through_mediator.py
--rw-r--r--   0        0        0      308 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/policy/__init__.py
--rw-r--r--   0        0        0      514 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/policy/data_transform_policy.py
--rw-r--r--   0        0        0     3608 2024-05-02 08:12:10.185802 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/policy/data_transform_policy_manager.py
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 aissemble_foundation_transform_core_python-1.7.0.dev1714638197/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-02 08:23:07.840544 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/README.md
+-rw-r--r--   0        0        0      656 2024-05-02 08:23:19.670214 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/pyproject.toml
+-rw-r--r--   0        0        0      244 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/__init__.py
+-rw-r--r--   0        0        0      342 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/data_transform_exception.py
+-rw-r--r--   0        0        0      507 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/mediator/__init__.py
+-rw-r--r--   0        0        0      747 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/mediator/logging_mediator.py
+-rw-r--r--   0        0        0     4333 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/mediator/mediation_manager.py
+-rw-r--r--   0        0        0     1726 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/mediator/mediation_objects.py
+-rw-r--r--   0        0        0     1374 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/mediator/mediator.py
+-rw-r--r--   0        0        0      689 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/mediator/pass_through_mediator.py
+-rw-r--r--   0        0        0      308 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/policy/__init__.py
+-rw-r--r--   0        0        0      514 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/policy/data_transform_policy.py
+-rw-r--r--   0        0        0     3608 2024-05-02 08:12:10.998919 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/policy/data_transform_policy_manager.py
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 aissemble_foundation_transform_core_python-1.7.0.dev1714638199/PKG-INFO
```

### Comparing `aissemble_foundation_transform_core_python-1.7.0.dev1714638197/LICENSE` & `aissemble_foundation_transform_core_python-1.7.0.dev1714638199/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_transform_core_python-1.7.0.dev1714638197/pyproject.toml` & `aissemble_foundation_transform_core_python-1.7.0.dev1714638199/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-transform-core-python"
-version = "1.7.0.dev1714638197"
+version = "1.7.0.dev1714638199"
 description = "Contains the core Python implementation of data transform"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "data_transform_core", from="src"}
 ]
```

### Comparing `aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/mediator/logging_mediator.py` & `aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/mediator/logging_mediator.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/mediator/mediation_manager.py` & `aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/mediator/mediation_manager.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/mediator/mediation_objects.py` & `aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/mediator/mediation_objects.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/mediator/mediator.py` & `aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/mediator/mediator.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/mediator/pass_through_mediator.py` & `aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/mediator/pass_through_mediator.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/policy/data_transform_policy.py` & `aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/policy/data_transform_policy.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_transform_core_python-1.7.0.dev1714638197/src/data_transform_core/policy/data_transform_policy_manager.py` & `aissemble_foundation_transform_core_python-1.7.0.dev1714638199/src/data_transform_core/policy/data_transform_policy_manager.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_transform_core_python-1.7.0.dev1714638197/PKG-INFO` & `aissemble_foundation_transform_core_python-1.7.0.dev1714638199/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-transform-core-python
-Version: 1.7.0.dev1714638197
+Version: 1.7.0.dev1714638199
 Summary: Contains the core Python implementation of data transform
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cryptography (>=42.0.4)
```

