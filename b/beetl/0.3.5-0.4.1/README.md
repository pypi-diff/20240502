# Comparing `tmp/beetl-0.3.5.tar.gz` & `tmp/beetl-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beetl-0.3.5.tar", last modified: Thu May  2 13:59:29 2024, max compression
+gzip compressed data, was "beetl-0.4.1.tar", last modified: Wed Mar 13 12:33:09 2024, max compression
```

## Comparing `beetl-0.3.5.tar` & `beetl-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:59:29.496742 beetl-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-02 13:59:29.496742 beetl-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-02 13:58:45.000000 beetl-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:59:29.496742 beetl-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-02 13:58:45.000000 beetl-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:59:29.492742 beetl-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:59:29.492742 beetl-0.3.5/src/beetl/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/beetl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:59:29.496742 beetl-0.3.5/src/beetl/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/sources/faker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/sources/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/sources/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/sources/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/sources/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/sources/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/sources/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/sources/sqlserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/sources/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:59:29.496742 beetl-0.3.5/src/beetl/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/transformers/frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/transformers/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/transformers/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/transformers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/transformers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/transformers/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-02 13:58:45.000000 beetl-0.3.5/src/beetl/transformers/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:59:29.496742 beetl-0.3.5/src/beetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-02 13:59:29.000000 beetl-0.3.5/src/beetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-02 13:59:29.000000 beetl-0.3.5/src/beetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:59:29.000000 beetl-0.3.5/src/beetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 13:59:29.000000 beetl-0.3.5/src/beetl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 13:59:29.000000 beetl-0.3.5/src/beetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 13:59:29.000000 beetl-0.3.5/src/beetl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:59:29.000000 beetl-0.3.5/src/beetl.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:33:09.559771 beetl-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-03-13 12:33:09.559771 beetl-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-03-13 12:32:19.000000 beetl-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 12:33:09.559771 beetl-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-13 12:32:19.000000 beetl-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:33:09.555771 beetl-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:33:09.555771 beetl-0.4.1/src/beetl/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/beetl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:33:09.559771 beetl-0.4.1/src/beetl/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/sources/faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/sources/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/sources/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/sources/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/sources/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/sources/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/sources/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/sources/sqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/sources/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:33:09.559771 beetl-0.4.1/src/beetl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/transformers/frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/transformers/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/transformers/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/transformers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/transformers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/transformers/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-13 12:32:19.000000 beetl-0.4.1/src/beetl/transformers/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:33:09.555771 beetl-0.4.1/src/beetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-03-13 12:33:09.000000 beetl-0.4.1/src/beetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-13 12:33:09.000000 beetl-0.4.1/src/beetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:33:09.000000 beetl-0.4.1/src/beetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-13 12:33:09.000000 beetl-0.4.1/src/beetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-13 12:33:09.000000 beetl-0.4.1/src/beetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-13 12:33:09.000000 beetl-0.4.1/src/beetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:33:09.000000 beetl-0.4.1/src/beetl.egg-info/zip-safe
```

### Comparing `beetl-0.3.5/PKG-INFO` & `beetl-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.3.5
+Version: 0.4.1
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <h1 style="width: 100%; text-align: center; margin-bottom: 20px; border-bottom: 0px;">BeETL: Extensible Python/Polars-based ETL Framework</h1>
-<p style="text-align: center; margin-bottom: 30px;"><img src="./images/beetl.jpg" style="max-width: 400px;" alt=" "><img src="./docs/images/beetl.jpg" style="max-width: 400px;" alt=" "><br/></p>
+<p style="text-align: center; margin-bottom: 30px;"><img src="./_static/BeETL.png" style="max-width: 400px;" alt=" "><img src="./docs/_static/BeETL.png" style="max-width: 400px;" alt=" "><br/></p>
 BeETL was born from a job as Integration Developer where a majority of the integrations we develop follow the same pattern - get here, transform a little, put there (with the middle step frequently missing altogether). 
 
 After building our 16th integration between the same two systems with another manual template, we decided to build BeETL. BeETL is currently limited to one datasource per source and destination per sync, but this will be expanded in the future. One configuration can contain multiple syncs.
 
 Note: Even though most of the configuration below is in YAML format, you can also use JSON or a python dictionary.
 
 ## Todo:
```

### Comparing `beetl-0.3.5/README.md` & `beetl-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 style="width: 100%; text-align: center; margin-bottom: 20px; border-bottom: 0px;">BeETL: Extensible Python/Polars-based ETL Framework</h1>
-<p style="text-align: center; margin-bottom: 30px;"><img src="./images/beetl.jpg" style="max-width: 400px;" alt=" "><img src="./docs/images/beetl.jpg" style="max-width: 400px;" alt=" "><br/></p>
+<p style="text-align: center; margin-bottom: 30px;"><img src="./_static/BeETL.png" style="max-width: 400px;" alt=" "><img src="./docs/_static/BeETL.png" style="max-width: 400px;" alt=" "><br/></p>
 BeETL was born from a job as Integration Developer where a majority of the integrations we develop follow the same pattern - get here, transform a little, put there (with the middle step frequently missing altogether). 
 
 After building our 16th integration between the same two systems with another manual template, we decided to build BeETL. BeETL is currently limited to one datasource per source and destination per sync, but this will be expanded in the future. One configuration can contain multiple syncs.
 
 Note: Even though most of the configuration below is in YAML format, you can also use JSON or a python dictionary.
 
 ## Todo:
```

### Comparing `beetl-0.3.5/setup.py` & `beetl-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/__version__.py` & `beetl-0.4.1/src/beetl/__version__.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/beetl.py` & `beetl-0.4.1/src/beetl/beetl.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,36 +69,22 @@
 
         if isinstance(destination, Union[list, set, tuple]):
             destination = pl.DataFrame(destination)
         
         # Get all columns from destination if none are specified
         columns = destination.columns if len(columns) == 0 else columns
 
-        for column in columns:
-            
-            if column not in source.columns and column not in destination.columns:
-                raise Exception(f"Column {column} does not exist in any of the datasets")
-            
-            if column not in source.columns:
-                source = source.with_columns(pl.lit(None).alias(column).cast(source[column].dtype))
-            
-            if column not in destination.columns:
-                destination = destination.with_columns(pl.lit(None).alias(column).cast(source[column].dtype))
-
         # If source is empty, delete all in destination
         if len(source) == 0:
             return source.select(keys + columns), source.select(keys + columns), destination.select(keys)
 
         # If destination is empty, create all from source
         if len(destination) == 0:
-            return (
-                source.select(keys + columns if keys != columns else keys),
-                destination.select(keys + columns if keys != columns else keys), 
-                destination
-            )
+            return source.select(keys + columns), destination.select(keys + columns), destination
+
        
         try:
             # Get rows that only exist in source (Creates)
             create = source.join(destination, on=keys, how="anti")
 
             # Get rows that exist in both and have differing values (Updates)
             update = source.join(destination, on=keys, how="semi").join(
@@ -112,19 +98,15 @@
             raise ValueError(
                 "One or more comparison columns do not exist \n"
                 f"Source columns: {','.join(source.columns)} \n"
                 f"Destination columns: {','.join(destination.columns)} \n"
                 f"Comparison columns: {','.join(columns)} \n"
             ) from e
 
-        return (
-                create.select(keys + columns if keys != columns else keys),
-                update.select(keys + columns if keys != columns else keys), 
-                delete.select(keys)
-            )
+        return (create.select(keys + columns), update.select(keys + columns), delete.select(keys))
 
     def benchmark(self, text: str) -> None:
         """Inserts a benchmark into the log"""
         BENCHMARK.append({"text": text, "perf": perf_counter()})
 
         if len(BENCHMARK) > 1:
             print(
```

### Comparing `beetl-0.3.5/src/beetl/config.py` & `beetl-0.4.1/src/beetl/config.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/sources/faker.py` & `beetl-0.4.1/src/beetl/sources/faker.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/sources/interface.py` & `beetl-0.4.1/src/beetl/sources/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/sources/itop.py` & `beetl-0.4.1/src/beetl/sources/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/sources/mongodb.py` & `beetl-0.4.1/src/beetl/sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/sources/mysql.py` & `beetl-0.4.1/src/beetl/sources/mysql.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/sources/postgres.py` & `beetl-0.4.1/src/beetl/sources/postgres.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/sources/sqlserver.py` & `beetl-0.4.1/src/beetl/sources/sqlserver.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/sources/static.py` & `beetl-0.4.1/src/beetl/sources/static.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/transformers/interface.py` & `beetl-0.4.1/src/beetl/transformers/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         try:
             return Transformers.transformers[transformer](data, **kwargs)
         except TypeError as e:
             raise TypeError(
                 f"The wrong arguments supplied for transformer {transformer}: {str(e)}"
             ) from e
         except KeyError as e:
-            raise KeyError(f"The transformer {transformer} does not exist or an error occured in the transformer") from e
+            raise KeyError(f"The transformer {transformer} does not exist") from e
         except Exception as e:
             raise Exception(
                 f"An error occurred while running transformer {transformer}: {str(e)}"
             ) from e
 
 
 class TransformerConfiguration:
```

### Comparing `beetl-0.3.5/src/beetl/transformers/itop.py` & `beetl-0.4.1/src/beetl/transformers/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/transformers/misc.py` & `beetl-0.4.1/src/beetl/transformers/misc.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,25 +29,7 @@
             .struct.unnest()["field_0"]
             .str.splitn("=", 2)
             .struct.unnest()["field_1"]
             .alias(outField if outField is not None else inField)
         )
 
         return data
-
-    @staticmethod
-    def divide(data: pl.DataFrame, inField: str, outField: str, factor: int) -> pl.DataFrame:
-        """Divide the numbers in a given column with the given factor
-
-        Args:
-            data (pl.DataFrame): The dataFrame to modify
-            inField (str): The field to process
-            outField (str): The field to put the output into
-            factor (int): The field to divide by
-
-        Returns:
-            pl.DataFrame: The resulting DataFrame
-        """
-        
-        data = data.with_columns((data[inField].cast(pl.Int64) / factor).alias(outField))
-        
-        return data
```

### Comparing `beetl-0.3.5/src/beetl/transformers/regex.py` & `beetl-0.4.1/src/beetl/transformers/regex.py`

 * *Files identical despite different names*

### Comparing `beetl-0.3.5/src/beetl/transformers/structs.py` & `beetl-0.4.1/src/beetl/transformers/frames.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,50 @@
 from typing import List
 import polars as pl
 from .interface import TransformerInterface, register_transformer_class
-import json
 
-@register_transformer_class("structs")
-class StructTransformers(TransformerInterface):
+
+@register_transformer_class("frames")
+class FrameTransformer(TransformerInterface):
     @staticmethod
-    def staticfield(data: pl.DataFrame, field: str, value):
-        """Add a struct field to the DataFrame
+    def rename_columns(data: pl.DataFrame, columns: List[dict]):
+        """Rename columns in the dataset
 
         Args:
-            data (pl.DataFrame): The dataFrame to modify
-            field (str): The field to add
-            value (str): The value of the field to add
+            data (pl.DataFrame): The dataset
+            columns (List[dict]): A list of dicts (from: col1, to: col2)
 
         Returns:
-            pl.DataFrame: The resulting DataFrame
+            pl.DataFrame: DataFrame with renamed columns
         """
-        data = data.with_columns(pl.Series(field, [value] * len(data)))
+        for column in columns:
+            data = data.rename({column["from"]: column["to"]})
         return data
 
     @staticmethod
-    def jsonpath(data: pl.DataFrame, inField: str, outField: str, jsonPath: str, defaultValue: str = ""):
-        """
-        Retrieve a value from a jsonpath inside of a column and add it to a new column
-        
+    def copy_columns(data: pl.DataFrame, columns: List[dict]):
+        """Copies a given column to another column
+
         Args:
-            data (pl.DataFrame): The dataFrame to modify
-            field (str): The field to extract the jsonpath from
-            outField (str): The field to add the extracted value to
-            jsonPath (str): The jsonpath to extract
+            data (pl.DataFrame): The dataset
+            columns (List[dict]): A list of dicts (from: col1, to: col2)
+
+        Returns:
+            pl.DataFrame: DataFrame with renamed columns
         """
-        split_jsonpath = jsonPath.split(".")
-                
-        def jsonpathFunction(fData):
-            if isinstance(fData, str):
-                fData = json.loads(fData)
-
-            try:
-                for i in split_jsonpath:
-                    try:
-                        ix = int(i)
-                        fData = fData[ix]
-                    except:
-                        fData = fData[i]
-                return fData
-            except:
-                return defaultValue
-            
-
-            return "OK"
-        
-        dCol = data[inField]
-        outCol = []
-        for i in range(len(dCol)):
-            outCol.append(jsonpathFunction(dCol[i]))
-        
-        data = data.with_columns(pl.Series(outField, outCol))
-        
+        for column in columns:
+            data[column["to"]] = data[column["from"]]
+
         return data
+
+    @staticmethod
+    def drop_columns(data: pl.DataFrame, columns: List[str]) -> pl.DataFrame:
+        """Drop columns from a DataFrame
+
+        Args:
+            data (pl.DataFrame): Drop columns from this dataframe
+            columns (List[str]): The columns to dr op
+
+        Returns:
+            pl.DataFrame: The dataframe without the columns
+        """
+        return data.drop(columns)
```

### Comparing `beetl-0.3.5/src/beetl.egg-info/PKG-INFO` & `beetl-0.4.1/src/beetl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.3.5
+Version: 0.4.1
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <h1 style="width: 100%; text-align: center; margin-bottom: 20px; border-bottom: 0px;">BeETL: Extensible Python/Polars-based ETL Framework</h1>
-<p style="text-align: center; margin-bottom: 30px;"><img src="./images/beetl.jpg" style="max-width: 400px;" alt=" "><img src="./docs/images/beetl.jpg" style="max-width: 400px;" alt=" "><br/></p>
+<p style="text-align: center; margin-bottom: 30px;"><img src="./_static/BeETL.png" style="max-width: 400px;" alt=" "><img src="./docs/_static/BeETL.png" style="max-width: 400px;" alt=" "><br/></p>
 BeETL was born from a job as Integration Developer where a majority of the integrations we develop follow the same pattern - get here, transform a little, put there (with the middle step frequently missing altogether). 
 
 After building our 16th integration between the same two systems with another manual template, we decided to build BeETL. BeETL is currently limited to one datasource per source and destination per sync, but this will be expanded in the future. One configuration can contain multiple syncs.
 
 Note: Even though most of the configuration below is in YAML format, you can also use JSON or a python dictionary.
 
 ## Todo:
```

### Comparing `beetl-0.3.5/src/beetl.egg-info/SOURCES.txt` & `beetl-0.4.1/src/beetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

