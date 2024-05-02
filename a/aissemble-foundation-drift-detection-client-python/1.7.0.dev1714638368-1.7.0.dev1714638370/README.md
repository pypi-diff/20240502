# Comparing `tmp/aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368.tar.gz` & `tmp/aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368.tar", max compression
+gzip compressed data, was "aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370.tar", max compression
```

## Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368.tar` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     9580 2024-05-02 08:25:54.534702 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/LICENSE
--rw-r--r--   0        0        0        0 2024-05-02 08:12:10.125802 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/README.md
--rw-r--r--   0        0        0      661 2024-05-02 08:26:08.941686 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/pyproject.toml
--rw-r--r--   0        0        0      194 2024-05-02 08:12:10.125802 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/src/config/__init__.py
--rw-r--r--   0        0        0      672 2024-05-02 08:12:10.125802 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/src/config/rest_config.py
--rw-r--r--   0        0        0      194 2024-05-02 08:12:10.125802 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/src/drift/__init__.py
--rw-r--r--   0        0        0      194 2024-05-02 08:12:10.126802 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/src/drift/detection/__init__.py
--rw-r--r--   0        0        0      194 2024-05-02 08:12:10.126802 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/src/drift/detection/rest/__init__.py
--rw-r--r--   0        0        0      194 2024-05-02 08:12:10.126802 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/src/drift/detection/rest/client/__init__.py
--rw-r--r--   0        0        0     1755 2024-05-02 08:12:10.126802 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/src/drift/detection/rest/client/drift_rest_client.py
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-02 08:25:54.995875 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-02 08:12:10.928921 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/README.md
+-rw-r--r--   0        0        0      661 2024-05-02 08:26:11.205423 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/pyproject.toml
+-rw-r--r--   0        0        0      194 2024-05-02 08:12:10.938921 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/src/config/__init__.py
+-rw-r--r--   0        0        0      672 2024-05-02 08:12:10.938921 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/src/config/rest_config.py
+-rw-r--r--   0        0        0      194 2024-05-02 08:12:10.938921 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/src/drift/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-02 08:12:10.938921 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/src/drift/detection/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-02 08:12:10.938921 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/src/drift/detection/rest/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-02 08:12:10.938921 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/src/drift/detection/rest/client/__init__.py
+-rw-r--r--   0        0        0     1755 2024-05-02 08:12:10.938921 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/src/drift/detection/rest/client/drift_rest_client.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/PKG-INFO
```

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/LICENSE` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/pyproject.toml` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-drift-detection-client-python"
-version = "1.7.0.dev1714638368"
+version = "1.7.0.dev1714638370"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "config", from = "src"},
     {include = "drift", from = "src"}
 ]
```

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/src/config/rest_config.py` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/src/config/rest_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/src/drift/detection/rest/client/drift_rest_client.py` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/src/drift/detection/rest/client/drift_rest_client.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638368/PKG-INFO` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714638370/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-drift-detection-client-python
-Version: 1.7.0.dev1714638368
+Version: 1.7.0.dev1714638370
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cryptography (>=42.0.4)
```

