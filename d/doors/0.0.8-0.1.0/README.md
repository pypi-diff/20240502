# Comparing `tmp/doors-0.0.8.tar.gz` & `tmp/doors-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doors-0.0.8.tar", max compression
+gzip compressed data, was "doors-0.1.0.tar", max compression
```

## Comparing `doors-0.0.8.tar` & `doors-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1066 2024-02-24 22:07:41.410280 doors-0.0.8/LICENCE.txt
--rw-r--r--   0        0        0       78 2024-02-24 22:07:41.410605 doors-0.0.8/doors/__init__.py
--rw-r--r--   0        0        0     2479 2024-02-24 22:07:41.410684 doors-0.0.8/doors/bq.py
--rw-r--r--   0        0        0      258 2024-02-24 22:07:41.410755 doors-0.0.8/doors/clargs.py
--rw-r--r--   0        0        0      373 2024-04-02 08:25:43.804077 doors-0.0.8/doors/cleaning.py
--rw-r--r--   0        0        0     4260 2024-03-01 09:59:55.397515 doors-0.0.8/doors/dates.py
--rw-r--r--   0        0        0     1433 2024-04-02 08:43:34.358264 doors-0.0.8/doors/debug.py
--rw-r--r--   0        0        0      701 2024-02-24 22:07:41.410992 doors-0.0.8/doors/dicts.py
--rw-r--r--   0        0        0     1087 2024-02-24 22:07:41.411078 doors-0.0.8/doors/eda.py
--rw-r--r--   0        0        0     5019 2024-03-27 10:05:49.192587 doors-0.0.8/doors/features.py
--rw-r--r--   0        0        0     1997 2024-03-06 16:43:27.752219 doors-0.0.8/doors/inout.py
--rw-r--r--   0        0        0     1795 2024-02-24 22:07:41.411341 doors-0.0.8/doors/mem.py
--rw-r--r--   0        0        0      267 2024-02-24 22:07:41.411413 doors-0.0.8/doors/metrics.py
--rw-r--r--   0        0        0     5461 2024-02-24 22:07:41.411514 doors-0.0.8/doors/modelling.py
--rw-r--r--   0        0        0      909 2024-02-24 22:07:41.411591 doors-0.0.8/doors/models.py
--rw-r--r--   0        0        0     5968 2024-02-24 22:07:41.411691 doors-0.0.8/doors/multifeat.py
--rw-r--r--   0        0        0    10967 2024-03-01 10:16:33.543543 doors-0.0.8/doors/np.py
--rw-r--r--   0        0        0     1188 2024-02-24 22:07:41.411921 doors-0.0.8/doors/outliers.py
--rw-r--r--   0        0        0      146 2024-02-24 22:07:41.411989 doors-0.0.8/doors/paths.py
--rw-r--r--   0        0        0     3809 2024-02-24 22:07:41.412096 doors-0.0.8/doors/plots.py
--rw-r--r--   0        0        0      307 2024-02-24 22:07:41.412176 doors-0.0.8/doors/setup_logger.py
--rw-r--r--   0        0        0     1506 2024-02-24 22:07:41.412258 doors-0.0.8/doors/stats.py
--rw-r--r--   0        0        0     4406 2024-02-24 22:07:41.412347 doors-0.0.8/doors/strings.py
--rw-r--r--   0        0        0     2832 2024-02-24 22:07:41.412421 doors-0.0.8/doors/venn.py
--rw-r--r--   0        0        0      500 2024-04-02 08:45:18.386741 doors-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 doors-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-02-24 22:07:41.410280 doors-0.1.0/LICENCE.txt
+-rw-r--r--   0        0        0       78 2024-02-24 22:07:41.410605 doors-0.1.0/doors/__init__.py
+-rw-r--r--   0        0        0     2479 2024-02-24 22:07:41.410684 doors-0.1.0/doors/bq.py
+-rw-r--r--   0        0        0      258 2024-02-24 22:07:41.410755 doors-0.1.0/doors/clargs.py
+-rw-r--r--   0        0        0      373 2024-04-02 08:25:43.804077 doors-0.1.0/doors/cleaning.py
+-rw-r--r--   0        0        0     4260 2024-03-01 09:59:55.397515 doors-0.1.0/doors/dates.py
+-rw-r--r--   0        0        0     1433 2024-04-02 08:43:34.358264 doors-0.1.0/doors/debug.py
+-rw-r--r--   0        0        0      701 2024-02-24 22:07:41.410992 doors-0.1.0/doors/dicts.py
+-rw-r--r--   0        0        0     3138 2024-05-02 13:24:14.335106 doors-0.1.0/doors/download.py
+-rw-r--r--   0        0        0     1087 2024-02-24 22:07:41.411078 doors-0.1.0/doors/eda.py
+-rw-r--r--   0        0        0     5019 2024-03-27 10:05:49.192587 doors-0.1.0/doors/features.py
+-rw-r--r--   0        0        0     2760 2024-05-02 13:22:34.201982 doors-0.1.0/doors/inout.py
+-rw-r--r--   0        0        0     1795 2024-02-24 22:07:41.411341 doors-0.1.0/doors/mem.py
+-rw-r--r--   0        0        0      267 2024-02-24 22:07:41.411413 doors-0.1.0/doors/metrics.py
+-rw-r--r--   0        0        0     5461 2024-02-24 22:07:41.411514 doors-0.1.0/doors/modelling.py
+-rw-r--r--   0        0        0      909 2024-02-24 22:07:41.411591 doors-0.1.0/doors/models.py
+-rw-r--r--   0        0        0     5968 2024-02-24 22:07:41.411691 doors-0.1.0/doors/multifeat.py
+-rw-r--r--   0        0        0    10967 2024-03-01 10:16:33.543543 doors-0.1.0/doors/np.py
+-rw-r--r--   0        0        0     1188 2024-02-24 22:07:41.411921 doors-0.1.0/doors/outliers.py
+-rw-r--r--   0        0        0      146 2024-02-24 22:07:41.411989 doors-0.1.0/doors/paths.py
+-rw-r--r--   0        0        0     3809 2024-02-24 22:07:41.412096 doors-0.1.0/doors/plots.py
+-rw-r--r--   0        0        0      307 2024-02-24 22:07:41.412176 doors-0.1.0/doors/setup_logger.py
+-rw-r--r--   0        0        0     1506 2024-02-24 22:07:41.412258 doors-0.1.0/doors/stats.py
+-rw-r--r--   0        0        0     4406 2024-02-24 22:07:41.412347 doors-0.1.0/doors/strings.py
+-rw-r--r--   0        0        0     2832 2024-02-24 22:07:41.412421 doors-0.1.0/doors/venn.py
+-rw-r--r--   0        0        0      500 2024-04-29 13:53:48.093736 doors-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 doors-0.1.0/PKG-INFO
```

### Comparing `doors-0.0.8/LICENCE.txt` & `doors-0.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/bq.py` & `doors-0.1.0/doors/bq.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/dates.py` & `doors-0.1.0/doors/dates.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/debug.py` & `doors-0.1.0/doors/debug.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/dicts.py` & `doors-0.1.0/doors/dicts.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/eda.py` & `doors-0.1.0/doors/eda.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/features.py` & `doors-0.1.0/doors/features.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/inout.py` & `doors-0.1.0/doors/inout.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,40 @@
+import hashlib
 import json
 import os
 import pickle
 
 import pandas as pd
+import yaml
+
+
+def get_md5_hash(file_path):
+    """
+    Calculate the MD5 hash of a file given its file path.
+
+    :param file_path: Path to the file
+    :return: The MD5 hash of the file as a hex string
+    """
+    hash_md5 = hashlib.md5()
+    try:
+        with open(file_path, "rb") as f:
+            for chunk in iter(lambda: f.read(4096), b""):
+                hash_md5.update(chunk)
+        return hash_md5.hexdigest()
+    except FileNotFoundError:
+        return "File not found."
+    except Exception as e:
+        return f"An error occurred: {e}"
+
+
+def read_yaml(filepath: str) -> dict:
+    """parse a yaml file and returns a dictionary with the data"""
+    with open(filepath) as file:
+        ans = yaml.safe_load(file)
+        return ans
 
 
 def append_csv(data, path):
     """append to a csv"""
     assert path.endswith(".csv")
     to_log = data if isinstance(data, pd.DataFrame) else pd.DataFrame(data)
     if "~" in path:
```

### Comparing `doors-0.0.8/doors/mem.py` & `doors-0.1.0/doors/mem.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/modelling.py` & `doors-0.1.0/doors/modelling.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/models.py` & `doors-0.1.0/doors/models.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/multifeat.py` & `doors-0.1.0/doors/multifeat.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/np.py` & `doors-0.1.0/doors/np.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/outliers.py` & `doors-0.1.0/doors/outliers.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/plots.py` & `doors-0.1.0/doors/plots.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/stats.py` & `doors-0.1.0/doors/stats.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/strings.py` & `doors-0.1.0/doors/strings.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/doors/venn.py` & `doors-0.1.0/doors/venn.py`

 * *Files identical despite different names*

### Comparing `doors-0.0.8/PKG-INFO` & `doors-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doors
-Version: 0.0.8
+Version: 0.1.0
 Summary: General tools for machine learning and data processing
 License: MIT
 Author: Matias Thayer
 Author-email: matias.thayer@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

