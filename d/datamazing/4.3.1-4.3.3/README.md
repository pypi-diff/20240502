# Comparing `tmp/datamazing-4.3.1.tar.gz` & `tmp/datamazing-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-4.3.1.tar", max compression
+gzip compressed data, was "datamazing-4.3.3.tar", max compression
```

## Comparing `datamazing-4.3.1.tar` & `datamazing-4.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/__init__.py
--rw-r--r--   0        0        0      277 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/_conform.py
--rw-r--r--   0        0        0      645 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0      309 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/datacollection/__init__.py
--rw-r--r--   0        0        0     2450 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/io.py
--rw-r--r--   0        0        0      140 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      766 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     2814 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0     2384 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     8044 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0     2633 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/merging.py
--rw-r--r--   0        0        0     2145 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/reindexing.py
--rw-r--r--   0        0        0     6674 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      695 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pandas/types.py
--rw-r--r--   0        0        0      184 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/__init__.py
--rw-r--r--   0        0        0       92 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/testing/__init__.py
--rw-r--r--   0        0        0      295 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/testing/assertions.py
--rw-r--r--   0        0        0     2363 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/testing/data.py
--rw-r--r--   0        0        0        0 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/transformations/__init__.py
--rw-r--r--   0        0        0     3487 2024-04-30 12:27:29.490855 datamazing-4.3.1/datamazing/pyspark/transformations/grouping.py
--rw-r--r--   0        0        0      734 2024-04-30 12:27:29.490855 datamazing-4.3.1/pyproject.toml
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 datamazing-4.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/_conform.py
+-rw-r--r--   0        0        0      645 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0     2487 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/io.py
+-rw-r--r--   0        0        0      140 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      766 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     2814 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0     2384 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     8044 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0     2633 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/transformations/merging.py
+-rw-r--r--   0        0        0     2145 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/transformations/reindexing.py
+-rw-r--r--   0        0        0     6674 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      695 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      184 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pyspark/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pyspark/testing/__init__.py
+-rw-r--r--   0        0        0      295 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pyspark/testing/assertions.py
+-rw-r--r--   0        0        0     2363 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pyspark/testing/data.py
+-rw-r--r--   0        0        0        0 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pyspark/transformations/__init__.py
+-rw-r--r--   0        0        0     3487 2024-05-02 13:06:12.353129 datamazing-4.3.3/datamazing/pyspark/transformations/grouping.py
+-rw-r--r--   0        0        0      734 2024-05-02 13:06:12.353129 datamazing-4.3.3/pyproject.toml
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 datamazing-4.3.3/PKG-INFO
```

### Comparing `datamazing-4.3.1/datamazing/pandas/__init__.py` & `datamazing-4.3.3/datamazing/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.1/datamazing/pandas/io.py` & `datamazing-4.3.3/datamazing/pandas/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     try:
         converted_values = pd.to_timedelta(values)
     except (ValueError, TypeError):
         # if not possible to parse as time delta, return original values
         return values
     try:
         values_isoformat = converted_values.apply(pd.Timedelta.isoformat)
-    except TypeError:
+    except (TypeError, AttributeError):
         return values
     if not (values_isoformat == values).all():
         # if original values is not in ISO 8601 format, return original values
         return values
     return converted_values
 
 
@@ -45,15 +45,15 @@
     Some conversions are invalid and the will cause the reading to fail.
     Example of invalid conversions:
     - converting a string to a float
 
     Args:
         filepath (str): Filepath of the CSV file
     """
-    df = pd.read_csv(filepath, keep_default_na=False)
+    df = pd.read_csv(filepath, keep_default_na=False, na_values=["nan"])
 
     # Auto cast types based on type hint in column name
     # type hints are on the form <column_name>:<type_hint>
     renames = {}
     for column_name in df.columns:
         if ":" in column_name:
             name, type_hint = column_name.split(":")
```

### Comparing `datamazing-4.3.1/datamazing/pandas/testing/assertions.py` & `datamazing-4.3.3/datamazing/pandas/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.1/datamazing/pandas/testing/data.py` & `datamazing-4.3.3/datamazing/pandas/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.1/datamazing/pandas/transformations/basic.py` & `datamazing-4.3.3/datamazing/pandas/transformations/basic.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.1/datamazing/pandas/transformations/grouping.py` & `datamazing-4.3.3/datamazing/pandas/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.1/datamazing/pandas/transformations/merging.py` & `datamazing-4.3.3/datamazing/pandas/transformations/merging.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.1/datamazing/pandas/transformations/reindexing.py` & `datamazing-4.3.3/datamazing/pandas/transformations/reindexing.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.1/datamazing/pandas/transformations/resampling.py` & `datamazing-4.3.3/datamazing/pandas/transformations/resampling.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.1/datamazing/pandas/types.py` & `datamazing-4.3.3/datamazing/pandas/types.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.1/datamazing/pyspark/testing/data.py` & `datamazing-4.3.3/datamazing/pyspark/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.1/datamazing/pyspark/transformations/grouping.py` & `datamazing-4.3.3/datamazing/pyspark/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-4.3.1/pyproject.toml` & `datamazing-4.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "4.3.1"
+version = "4.3.3"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

