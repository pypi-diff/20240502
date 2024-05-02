# Comparing `tmp/dagster_polars-0.3.1.tar.gz` & `tmp/dagster_polars-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_polars-0.3.1.tar", max compression
+gzip compressed data, was "dagster_polars-0.3.1a0.tar", max compression
```

## Comparing `dagster_polars-0.3.1.tar` & `dagster_polars-0.3.1a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11344 2024-01-30 22:13:59.154172 dagster_polars-0.3.1/LICENSE
--rw-r--r--   0        0        0     9069 2024-01-30 22:13:59.154172 dagster_polars-0.3.1/README.md
--rw-r--r--   0        0        0     1274 2024-01-30 22:13:59.154172 dagster_polars-0.3.1/dagster_polars/__init__.py
--rw-r--r--   0        0        0       64 2024-01-30 22:13:59.154172 dagster_polars-0.3.1/dagster_polars/constants.py
--rw-r--r--   0        0        0      718 2024-01-30 22:13:59.154172 dagster_polars-0.3.1/dagster_polars/io_managers/__init__.py
--rw-r--r--   0        0        0    17236 2024-01-30 22:13:59.154172 dagster_polars-0.3.1/dagster_polars/io_managers/base.py
--rw-r--r--   0        0        0     8022 2024-01-30 22:13:59.154172 dagster_polars-0.3.1/dagster_polars/io_managers/bigquery.py
--rw-r--r--   0        0        0    15515 2024-01-30 22:13:59.158172 dagster_polars-0.3.1/dagster_polars/io_managers/delta.py
--rw-r--r--   0        0        0    12144 2024-01-30 22:13:59.158172 dagster_polars-0.3.1/dagster_polars/io_managers/parquet.py
--rw-r--r--   0        0        0     5466 2024-01-30 22:13:59.158172 dagster_polars-0.3.1/dagster_polars/io_managers/utils.py
--rw-r--r--   0        0        0        0 2024-01-30 22:13:59.158172 dagster_polars-0.3.1/dagster_polars/py.typed
--rw-r--r--   0        0        0      870 2024-01-30 22:13:59.158172 dagster_polars-0.3.1/dagster_polars/types.py
--rw-r--r--   0        0        0       22 2024-01-30 22:14:22.518292 dagster_polars-0.3.1/dagster_polars/version.py
--rw-r--r--   0        0        0     3174 2024-01-30 22:14:22.518292 dagster_polars-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    10525 1970-01-01 00:00:00.000000 dagster_polars-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/LICENSE
+-rw-r--r--   0        0        0     9069 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/README.md
+-rw-r--r--   0        0        0     1274 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/dagster_polars/__init__.py
+-rw-r--r--   0        0        0       64 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/dagster_polars/constants.py
+-rw-r--r--   0        0        0      718 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/dagster_polars/io_managers/__init__.py
+-rw-r--r--   0        0        0    17236 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/dagster_polars/io_managers/base.py
+-rw-r--r--   0        0        0     8022 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/dagster_polars/io_managers/bigquery.py
+-rw-r--r--   0        0        0    15515 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/dagster_polars/io_managers/delta.py
+-rw-r--r--   0        0        0    12144 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/dagster_polars/io_managers/parquet.py
+-rw-r--r--   0        0        0     5466 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/dagster_polars/io_managers/utils.py
+-rw-r--r--   0        0        0        0 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/dagster_polars/py.typed
+-rw-r--r--   0        0        0      870 2024-01-30 18:30:41.138959 dagster_polars-0.3.1a0/dagster_polars/types.py
+-rw-r--r--   0        0        0       24 2024-01-30 18:31:05.942860 dagster_polars-0.3.1a0/dagster_polars/version.py
+-rw-r--r--   0        0        0     3176 2024-01-30 18:31:05.942860 dagster_polars-0.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0    10527 1970-01-01 00:00:00.000000 dagster_polars-0.3.1a0/PKG-INFO
```

### Comparing `dagster_polars-0.3.1/LICENSE` & `dagster_polars-0.3.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.3.1/README.md` & `dagster_polars-0.3.1a0/README.md`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.3.1/dagster_polars/__init__.py` & `dagster_polars-0.3.1a0/dagster_polars/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.3.1/dagster_polars/io_managers/__init__.py` & `dagster_polars-0.3.1a0/dagster_polars/io_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.3.1/dagster_polars/io_managers/base.py` & `dagster_polars-0.3.1a0/dagster_polars/io_managers/base.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.3.1/dagster_polars/io_managers/bigquery.py` & `dagster_polars-0.3.1a0/dagster_polars/io_managers/bigquery.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.3.1/dagster_polars/io_managers/delta.py` & `dagster_polars-0.3.1a0/dagster_polars/io_managers/delta.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.3.1/dagster_polars/io_managers/parquet.py` & `dagster_polars-0.3.1a0/dagster_polars/io_managers/parquet.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.3.1/dagster_polars/io_managers/utils.py` & `dagster_polars-0.3.1a0/dagster_polars/io_managers/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.3.1/dagster_polars/types.py` & `dagster_polars-0.3.1a0/dagster_polars/types.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.3.1/pyproject.toml` & `dagster_polars-0.3.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagster-polars"
-version = "0.3.1"
+version = "0.3.1a0"
 description = "Dagster integration library for Polars"
 authors = [
     "Daniel Gafni <danielgafni16@gmail.com>"
 ]
 readme = "README.md"
 packages = [{include = "dagster_polars"}]
 repository = "https://github.com/danielgafni/dagster-polars"
```

### Comparing `dagster_polars-0.3.1/PKG-INFO` & `dagster_polars-0.3.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-polars
-Version: 0.3.1
+Version: 0.3.1a0
 Summary: Dagster integration library for Polars
 Home-page: https://github.com/danielgafni/dagster-polars
 License: Apache-2.0
 Keywords: dagster,polars,ETL,dataframe
 Author: Daniel Gafni
 Author-email: danielgafni16@gmail.com
 Requires-Python: >=3.8,<4.0
```

