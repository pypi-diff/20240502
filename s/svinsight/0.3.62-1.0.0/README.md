# Comparing `tmp/svinsight-0.3.62.tar.gz` & `tmp/svinsight-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svinsight-0.3.62.tar", max compression
+gzip compressed data, was "svinsight-1.0.0.tar", max compression
```

## Comparing `svinsight-0.3.62.tar` & `svinsight-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2024-05-01 17:05:45.110819 svinsight-0.3.62/LICENSE
--rw-r--r--   0        0        0      111 2024-05-01 17:05:45.310820 svinsight-0.3.62/long_desc.md
--rw-r--r--   0        0        0      547 2024-05-01 17:05:45.310820 svinsight-0.3.62/pyproject.toml
--rw-r--r--   0        0        0       58 2024-05-01 17:05:45.310820 svinsight-0.3.62/svinsight/__init__.py
--rw-r--r--   0        0        0    17061 2024-05-01 17:05:45.310820 svinsight-0.3.62/svinsight/census_variables.py
--rw-r--r--   0        0        0    77547 2024-05-01 17:05:45.310820 svinsight-0.3.62/svinsight/svi.py
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 svinsight-0.3.62/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-02 14:56:16.392909 svinsight-1.0.0/LICENSE
+-rw-r--r--   0        0        0      111 2024-05-02 14:56:16.592907 svinsight-1.0.0/long_desc.md
+-rw-r--r--   0        0        0      546 2024-05-02 14:56:16.592907 svinsight-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       57 2024-05-02 14:56:16.592907 svinsight-1.0.0/svinsight/__init__.py
+-rw-r--r--   0        0        0    17061 2024-05-02 14:56:16.592907 svinsight-1.0.0/svinsight/census_variables.py
+-rw-r--r--   0        0        0    77547 2024-05-02 14:56:16.596907 svinsight-1.0.0/svinsight/svi.py
+-rw-r--r--   0        0        0      875 1970-01-01 00:00:00.000000 svinsight-1.0.0/PKG-INFO
```

### Comparing `svinsight-0.3.62/LICENSE` & `svinsight-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svinsight-0.3.62/pyproject.toml` & `svinsight-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "svinsight"
-version = "0.3.62"
+version = "1.0.0"
 description = "Create social vulnerability index"
 authors = ["Matthew Preisser <mattpreisser@gmail.com>"]
 license = "MIT"
 readme = "long_desc.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `svinsight-0.3.62/svinsight/census_variables.py` & `svinsight-1.0.0/svinsight/census_variables.py`

 * *Files identical despite different names*

### Comparing `svinsight-0.3.62/svinsight/svi.py` & `svinsight-1.0.0/svinsight/svi.py`

 * *Files identical despite different names*

### Comparing `svinsight-0.3.62/PKG-INFO` & `svinsight-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svinsight
-Version: 0.3.62
+Version: 1.0.0
 Summary: Create social vulnerability index
 License: MIT
 Author: Matthew Preisser
 Author-email: mattpreisser@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

