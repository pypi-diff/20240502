# Comparing `tmp/airbyte_source_s3-4.5.9.dev202403072308.tar.gz` & `tmp/airbyte_source_s3-4.5.9.dev202403082230.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_s3-4.5.9.dev202403072308.tar", max compression
+gzip compressed data, was "airbyte_source_s3-4.5.9.dev202403082230.tar", max compression
```

## Comparing `airbyte_source_s3-4.5.9.dev202403072308.tar` & `airbyte_source_s3-4.5.9.dev202403082230.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     4424 2024-03-07 23:05:30.456383 airbyte_source_s3-4.5.9.dev202403072308/README.md
--rw-r--r--   0        0        0     1015 2024-03-07 23:08:36.430144 airbyte_source_s3-4.5.9.dev202403072308/pyproject.toml
--rw-r--r--   0        0        0       61 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/__init__.py
--rw-r--r--   0        0        0     1226 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/exceptions.py
--rw-r--r--   0        0        0     1673 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/run.py
--rw-r--r--   0        0        0     3270 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/source.py
--rw-r--r--   0        0        0       61 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/__init__.py
--rw-r--r--   0        0        0       61 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/formats/__init__.py
--rw-r--r--   0        0        0      373 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/formats/avro_spec.py
--rw-r--r--   0        0        0     3956 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/formats/csv_spec.py
--rw-r--r--   0        0        0     1678 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/formats/jsonl_spec.py
--rw-r--r--   0        0        0     1463 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/formats/parquet_spec.py
--rw-r--r--   0        0        0     5261 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/source.py
--rw-r--r--   0        0        0     5313 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/spec.py
--rw-r--r--   0        0        0     4251 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/stream.py
--rw-r--r--   0        0        0     2327 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/utils.py
--rw-r--r--   0        0        0      351 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/__init__.py
--rw-r--r--   0        0        0     3923 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/config.py
--rw-r--r--   0        0        0     7297 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/cursor.py
--rw-r--r--   0        0        0     7839 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/legacy_config_transformer.py
--rw-r--r--   0        0        0     4778 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/source.py
--rw-r--r--   0        0        0    11567 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/stream_reader.py
--rw-r--r--   0        0        0    14606 2024-03-07 23:05:30.460384 airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/zip_reader.py
--rw-r--r--   0        0        0     5312 1970-01-01 00:00:00.000000 airbyte_source_s3-4.5.9.dev202403072308/PKG-INFO
+-rw-r--r--   0        0        0     4424 2024-03-08 22:28:26.124543 airbyte_source_s3-4.5.9.dev202403082230/README.md
+-rw-r--r--   0        0        0     1015 2024-03-08 22:30:57.675038 airbyte_source_s3-4.5.9.dev202403082230/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/__init__.py
+-rw-r--r--   0        0        0     1226 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/exceptions.py
+-rw-r--r--   0        0        0     1673 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/run.py
+-rw-r--r--   0        0        0     3270 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/source.py
+-rw-r--r--   0        0        0       61 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/__init__.py
+-rw-r--r--   0        0        0       61 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/formats/__init__.py
+-rw-r--r--   0        0        0      373 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/formats/avro_spec.py
+-rw-r--r--   0        0        0     3956 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/formats/csv_spec.py
+-rw-r--r--   0        0        0     1678 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/formats/jsonl_spec.py
+-rw-r--r--   0        0        0     1463 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/formats/parquet_spec.py
+-rw-r--r--   0        0        0     5261 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/source.py
+-rw-r--r--   0        0        0     5313 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/spec.py
+-rw-r--r--   0        0        0     4251 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/stream.py
+-rw-r--r--   0        0        0     2327 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/utils.py
+-rw-r--r--   0        0        0      351 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/__init__.py
+-rw-r--r--   0        0        0     3923 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/config.py
+-rw-r--r--   0        0        0     7297 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/cursor.py
+-rw-r--r--   0        0        0     7839 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/legacy_config_transformer.py
+-rw-r--r--   0        0        0     4778 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/source.py
+-rw-r--r--   0        0        0    11567 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/stream_reader.py
+-rw-r--r--   0        0        0    14606 2024-03-08 22:28:26.128543 airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/zip_reader.py
+-rw-r--r--   0        0        0     5312 1970-01-01 00:00:00.000000 airbyte_source_s3-4.5.9.dev202403082230/PKG-INFO
```

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/README.md` & `airbyte_source_s3-4.5.9.dev202403082230/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/pyproject.toml` & `airbyte_source_s3-4.5.9.dev202403082230/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "4.5.9.dev202403072308"
+version = "4.5.9.dev202403082230"
 name = "airbyte-source-s3"
 description = "Source implementation for S3."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/exceptions.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/run.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/source.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/formats/csv_spec.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/formats/csv_spec.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/formats/jsonl_spec.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/formats/jsonl_spec.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/formats/parquet_spec.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/formats/parquet_spec.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/source.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/source_files_abstract/spec.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/source_files_abstract/spec.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/stream.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/stream.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/utils.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/config.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/config.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/cursor.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/legacy_config_transformer.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/legacy_config_transformer.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/source.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/stream_reader.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/stream_reader.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/source_s3/v4/zip_reader.py` & `airbyte_source_s3-4.5.9.dev202403082230/source_s3/v4/zip_reader.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_s3-4.5.9.dev202403072308/PKG-INFO` & `airbyte_source_s3-4.5.9.dev202403082230/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-s3
-Version: 4.5.9.dev202403072308
+Version: 4.5.9.dev202403082230
 Summary: Source implementation for S3.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

