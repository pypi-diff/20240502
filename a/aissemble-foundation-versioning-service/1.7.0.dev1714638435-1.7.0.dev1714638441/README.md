# Comparing `tmp/aissemble_foundation_versioning_service-1.7.0.dev1714638435.tar.gz` & `tmp/aissemble_foundation_versioning_service-1.7.0.dev1714638441.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_versioning_service-1.7.0.dev1714638435.tar", max compression
+gzip compressed data, was "aissemble_foundation_versioning_service-1.7.0.dev1714638441.tar", max compression
```

## Comparing `aissemble_foundation_versioning_service-1.7.0.dev1714638435.tar` & `aissemble_foundation_versioning_service-1.7.0.dev1714638441.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9580 2024-05-02 08:26:47.633651 aissemble_foundation_versioning_service-1.7.0.dev1714638435/LICENSE
--rw-r--r--   0        0        0     2933 2024-05-02 08:12:10.116802 aissemble_foundation_versioning_service-1.7.0.dev1714638435/README.md
--rw-r--r--   0        0        0     1042 2024-05-02 08:27:15.957620 aissemble_foundation_versioning_service-1.7.0.dev1714638435/pyproject.toml
--rw-r--r--   0        0        0     2697 2024-05-02 08:12:10.116802 aissemble_foundation_versioning_service-1.7.0.dev1714638435/src/model_versioning/version.py
--rw-r--r--   0        0        0     2811 2024-05-02 08:12:10.116802 aissemble_foundation_versioning_service-1.7.0.dev1714638435/src/model_versioning/versioning_api.py
--rw-r--r--   0        0        0     1810 2024-05-02 08:12:10.117802 aissemble_foundation_versioning_service-1.7.0.dev1714638435/src/util/maven_util.py
--rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 aissemble_foundation_versioning_service-1.7.0.dev1714638435/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-02 08:26:53.004258 aissemble_foundation_versioning_service-1.7.0.dev1714638441/LICENSE
+-rw-r--r--   0        0        0     2933 2024-05-02 08:12:10.918922 aissemble_foundation_versioning_service-1.7.0.dev1714638441/README.md
+-rw-r--r--   0        0        0     1042 2024-05-02 08:27:22.053449 aissemble_foundation_versioning_service-1.7.0.dev1714638441/pyproject.toml
+-rw-r--r--   0        0        0     2697 2024-05-02 08:12:10.918922 aissemble_foundation_versioning_service-1.7.0.dev1714638441/src/model_versioning/version.py
+-rw-r--r--   0        0        0     2811 2024-05-02 08:12:10.918922 aissemble_foundation_versioning_service-1.7.0.dev1714638441/src/model_versioning/versioning_api.py
+-rw-r--r--   0        0        0     1810 2024-05-02 08:12:10.918922 aissemble_foundation_versioning_service-1.7.0.dev1714638441/src/util/maven_util.py
+-rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 aissemble_foundation_versioning_service-1.7.0.dev1714638441/PKG-INFO
```

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1714638435/LICENSE` & `aissemble_foundation_versioning_service-1.7.0.dev1714638441/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1714638435/README.md` & `aissemble_foundation_versioning_service-1.7.0.dev1714638441/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1714638435/pyproject.toml` & `aissemble_foundation_versioning_service-1.7.0.dev1714638441/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-versioning-service"
-version = "1.7.0.dev1714638435"
+version = "1.7.0.dev1714638441"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "model_versioning", from = "src"},
     {include = "util", from = "src"}
 ]
```

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1714638435/src/model_versioning/version.py` & `aissemble_foundation_versioning_service-1.7.0.dev1714638441/src/model_versioning/version.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1714638435/src/model_versioning/versioning_api.py` & `aissemble_foundation_versioning_service-1.7.0.dev1714638441/src/model_versioning/versioning_api.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1714638435/src/util/maven_util.py` & `aissemble_foundation_versioning_service-1.7.0.dev1714638441/src/util/maven_util.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_versioning_service-1.7.0.dev1714638435/PKG-INFO` & `aissemble_foundation_versioning_service-1.7.0.dev1714638441/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-versioning-service
-Version: 1.7.0.dev1714638435
+Version: 1.7.0.dev1714638441
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: fastapi (>=0.95.0)
 Requires-Dist: mlflow (>=2.3.1,<3.0.0)
```

