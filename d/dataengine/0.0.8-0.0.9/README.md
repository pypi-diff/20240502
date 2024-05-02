# Comparing `tmp/dataengine-0.0.8.tar.gz` & `tmp/dataengine-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataengine-0.0.8.tar", last modified: Thu Oct  5 01:10:58 2023, max compression
+gzip compressed data, was "dataengine-0.0.9.tar", last modified: Thu Oct  5 12:25:49 2023, max compression
```

## Comparing `dataengine-0.0.8.tar` & `dataengine-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:10:58.610580 dataengine-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-05 01:10:48.000000 dataengine-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-10-05 01:10:58.610580 dataengine-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-10-05 01:10:48.000000 dataengine-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:10:58.606580 dataengine-0.0.8/dataengine/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7967 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/query_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:10:58.610580 dataengine-0.0.8/dataengine/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/databricks_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/datadog_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/general_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/github_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/mysql_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/postgresql_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24521 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/redact_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12341 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/slack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/utilities/spark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-10-05 01:10:48.000000 dataengine-0.0.8/dataengine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:10:58.606580 dataengine-0.0.8/dataengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-10-05 01:10:58.000000 dataengine-0.0.8/dataengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-10-05 01:10:58.000000 dataengine-0.0.8/dataengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 01:10:58.000000 dataengine-0.0.8/dataengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-10-05 01:10:58.000000 dataengine-0.0.8/dataengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-05 01:10:58.000000 dataengine-0.0.8/dataengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-05 01:10:48.000000 dataengine-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 01:10:58.610580 dataengine-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2023-10-05 01:10:48.000000 dataengine-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:10:58.606580 dataengine-0.0.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 01:10:58.610580 dataengine-0.0.8/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-05 01:10:48.000000 dataengine-0.0.8/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2023-10-05 01:10:48.000000 dataengine-0.0.8/tests/utilities/test_general_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2023-10-05 01:10:48.000000 dataengine-0.0.8/tests/utilities/test_mysql_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2023-10-05 01:10:48.000000 dataengine-0.0.8/tests/utilities/test_pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14296 2023-10-05 01:10:48.000000 dataengine-0.0.8/tests/utilities/test_redact_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9554 2023-10-05 01:10:48.000000 dataengine-0.0.8/tests/utilities/test_s3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:25:49.283791 dataengine-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-05 12:25:40.000000 dataengine-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2023-10-05 12:25:49.283791 dataengine-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2023-10-05 12:25:40.000000 dataengine-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:25:49.279791 dataengine-0.0.9/dataengine/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7967 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/query_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:25:49.283791 dataengine-0.0.9/dataengine/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/databricks_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/datadog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/github_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/mysql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/postgresql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/redact_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12341 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/slack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/utilities/spark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2023-10-05 12:25:40.000000 dataengine-0.0.9/dataengine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:25:49.279791 dataengine-0.0.9/dataengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2023-10-05 12:25:49.000000 dataengine-0.0.9/dataengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2023-10-05 12:25:49.000000 dataengine-0.0.9/dataengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 12:25:49.000000 dataengine-0.0.9/dataengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2023-10-05 12:25:49.000000 dataengine-0.0.9/dataengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-05 12:25:49.000000 dataengine-0.0.9/dataengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-05 12:25:40.000000 dataengine-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 12:25:49.283791 dataengine-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2023-10-05 12:25:40.000000 dataengine-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:25:49.279791 dataengine-0.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:25:49.283791 dataengine-0.0.9/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-05 12:25:40.000000 dataengine-0.0.9/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2023-10-05 12:25:40.000000 dataengine-0.0.9/tests/utilities/test_general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2023-10-05 12:25:40.000000 dataengine-0.0.9/tests/utilities/test_mysql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2023-10-05 12:25:40.000000 dataengine-0.0.9/tests/utilities/test_pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14296 2023-10-05 12:25:40.000000 dataengine-0.0.9/tests/utilities/test_redact_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9554 2023-10-05 12:25:40.000000 dataengine-0.0.9/tests/utilities/test_s3_utils.py
```

### Comparing `dataengine-0.0.8/LICENSE` & `dataengine-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/PKG-INFO` & `dataengine-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataengine
-Version: 0.0.8
+Version: 0.0.9
 Summary: General purpose data engineering python package.
 Home-page: https://github.com/leealessandrini/dataengine
 Author: Daniel Lee Alessandrini
 Author-email: alessandrinil@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
```

### Comparing `dataengine-0.0.8/dataengine/assets.py` & `dataengine-0.0.9/dataengine/assets.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/dataset.py` & `dataengine-0.0.9/dataengine/dataset.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/query_driver.py` & `dataengine-0.0.9/dataengine/query_driver.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/utilities/databricks_utils.py` & `dataengine-0.0.9/dataengine/utilities/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/utilities/datadog_utils.py` & `dataengine-0.0.9/dataengine/utilities/datadog_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/utilities/general_utils.py` & `dataengine-0.0.9/dataengine/utilities/general_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/utilities/github_utils.py` & `dataengine-0.0.9/dataengine/utilities/github_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/utilities/mysql_utils.py` & `dataengine-0.0.9/dataengine/utilities/mysql_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/utilities/pandas_utils.py` & `dataengine-0.0.9/dataengine/utilities/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/utilities/postgresql_utils.py` & `dataengine-0.0.9/dataengine/utilities/postgresql_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/utilities/redact_utils.py` & `dataengine-0.0.9/dataengine/utilities/redact_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,16 +623,15 @@
     Returns:
         str: The redacted text.    
     """
     # Make a copy of the original text
     redacted_text = text
     # Redact all full matches from the redaction map
     for redaction_string, values in redact_map.items():
-        redacted_text = re.sub(
-            values["regex"], redaction_string, redacted_text)
+        redacted_text = values["regex"].sub(redaction_string, redacted_text)
     
     return redacted_text
 
 
 def pooled_find(find_function, text_list, max_workers=16):
     """
     Execute a find function in parallel on a list of texts.
```

### Comparing `dataengine-0.0.8/dataengine/utilities/s3_utils.py` & `dataengine-0.0.9/dataengine/utilities/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/utilities/slack_utils.py` & `dataengine-0.0.9/dataengine/utilities/slack_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine/utilities/spark_utils.py` & `dataengine-0.0.9/dataengine/utilities/spark_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/dataengine.egg-info/PKG-INFO` & `dataengine-0.0.9/dataengine.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataengine
-Version: 0.0.8
+Version: 0.0.9
 Summary: General purpose data engineering python package.
 Home-page: https://github.com/leealessandrini/dataengine
 Author: Daniel Lee Alessandrini
 Author-email: alessandrinil@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
```

### Comparing `dataengine-0.0.8/dataengine.egg-info/SOURCES.txt` & `dataengine-0.0.9/dataengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/setup.py` & `dataengine-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/tests/utilities/test_general_utils.py` & `dataengine-0.0.9/tests/utilities/test_general_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/tests/utilities/test_mysql_utils.py` & `dataengine-0.0.9/tests/utilities/test_mysql_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/tests/utilities/test_pandas_utils.py` & `dataengine-0.0.9/tests/utilities/test_pandas_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/tests/utilities/test_redact_utils.py` & `dataengine-0.0.9/tests/utilities/test_redact_utils.py`

 * *Files identical despite different names*

### Comparing `dataengine-0.0.8/tests/utilities/test_s3_utils.py` & `dataengine-0.0.9/tests/utilities/test_s3_utils.py`

 * *Files identical despite different names*

