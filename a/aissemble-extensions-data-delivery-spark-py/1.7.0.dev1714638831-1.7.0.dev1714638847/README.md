# Comparing `tmp/aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831.tar.gz` & `tmp/aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831.tar", max compression
+gzip compressed data, was "aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847.tar", max compression
```

## Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831.tar` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9580 2024-05-02 08:33:31.404257 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831/LICENSE
--rw-r--r--   0        0        0      118 2024-05-02 08:12:10.077802 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831/README.md
--rw-r--r--   0        0        0      650 2024-05-02 08:33:51.744239 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831/pyproject.toml
--rw-r--r--   0        0        0      205 2024-05-02 08:12:10.078802 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831/src/data_delivery_spark_py/__init__.py
--rw-r--r--   0        0        0      205 2024-05-02 08:12:10.078802 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831/src/data_delivery_spark_py/test_utils/__init__.py
--rw-r--r--   0        0        0     2822 2024-05-02 08:12:10.078802 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831/src/data_delivery_spark_py/test_utils/spark_session_manager.py
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-02 08:33:46.962726 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847/LICENSE
+-rw-r--r--   0        0        0      118 2024-05-02 08:12:10.878923 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847/README.md
+-rw-r--r--   0        0        0      650 2024-05-02 08:34:07.792143 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847/pyproject.toml
+-rw-r--r--   0        0        0      205 2024-05-02 08:12:10.878923 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847/src/data_delivery_spark_py/__init__.py
+-rw-r--r--   0        0        0      205 2024-05-02 08:12:10.878923 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847/src/data_delivery_spark_py/test_utils/__init__.py
+-rw-r--r--   0        0        0     2822 2024-05-02 08:12:10.878923 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847/src/data_delivery_spark_py/test_utils/spark_session_manager.py
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847/PKG-INFO
```

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831/LICENSE` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831/pyproject.toml` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-extensions-data-delivery-spark-py"
-version = "1.7.0.dev1714638831"
+version = "1.7.0.dev1714638847"
 description = "Contains the core Python functionality of data delivery for Spark"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "data_delivery_spark_py", from="src"},
 ]
```

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831/src/data_delivery_spark_py/test_utils/spark_session_manager.py` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847/src/data_delivery_spark_py/test_utils/spark_session_manager.py`

 * *Files identical despite different names*

### Comparing `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638831/PKG-INFO` & `aissemble_extensions_data_delivery_spark_py-1.7.0.dev1714638847/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-extensions-data-delivery-spark-py
-Version: 1.7.0.dev1714638831
+Version: 1.7.0.dev1714638847
 Summary: Contains the core Python functionality of data delivery for Spark
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: krausening (>=19)
```

