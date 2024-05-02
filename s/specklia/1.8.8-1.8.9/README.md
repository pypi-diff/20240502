# Comparing `tmp/specklia-1.8.8.tar.gz` & `tmp/specklia-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.8.8.tar", last modified: Tue Feb 27 11:34:35 2024, max compression
+gzip compressed data, was "specklia-1.8.9.tar", last modified: Wed Feb 28 15:11:11 2024, max compression
```

## Comparing `specklia-1.8.8.tar` & `specklia-1.8.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:34:35.770891 specklia-1.8.8/
--rw-r--r--   0 root         (0) root         (0)     1061 2024-02-27 04:18:01.000000 specklia-1.8.8/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2897 2024-02-27 11:34:35.770891 specklia-1.8.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1611 2024-02-27 04:18:01.000000 specklia-1.8.8/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2024-02-27 11:34:35.770891 specklia-1.8.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2366 2024-02-27 04:18:01.000000 specklia-1.8.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:34:35.770891 specklia-1.8.8/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2024-02-27 04:18:01.000000 specklia-1.8.8/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14715 2024-02-27 04:18:01.000000 specklia-1.8.8/specklia/_websocket_helpers.py
--rw-r--r--   0 root         (0) root         (0)    39737 2024-02-27 11:07:11.000000 specklia-1.8.8/specklia/client.py
--rw-r--r--   0 root         (0) root         (0)     3790 2024-02-27 04:18:01.000000 specklia-1.8.8/specklia/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:34:35.770891 specklia-1.8.8/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2897 2024-02-27 11:34:35.000000 specklia-1.8.8/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      365 2024-02-27 11:34:35.000000 specklia-1.8.8/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 11:34:35.000000 specklia-1.8.8/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-02-27 11:34:35.000000 specklia-1.8.8/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-02-27 11:34:35.000000 specklia-1.8.8/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 11:34:35.770891 specklia-1.8.8/tests/
--rw-r--r--   0 root         (0) root         (0)    14649 2024-02-27 11:07:11.000000 specklia-1.8.8/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     2654 2024-02-27 04:18:01.000000 specklia-1.8.8/tests/test_utilities.py
--rw-r--r--   0 root         (0) root         (0)    11629 2024-02-27 04:18:01.000000 specklia-1.8.8/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 15:11:11.329601 specklia-1.8.9/
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-02-27 11:34:21.000000 specklia-1.8.9/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2897 2024-02-28 15:11:11.329601 specklia-1.8.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-02-27 11:34:21.000000 specklia-1.8.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2024-02-28 15:11:11.333601 specklia-1.8.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2366 2024-02-27 11:34:21.000000 specklia-1.8.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 15:11:11.325601 specklia-1.8.9/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-02-27 11:34:21.000000 specklia-1.8.9/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14715 2024-02-27 11:34:21.000000 specklia-1.8.9/specklia/_websocket_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    39737 2024-02-27 11:34:21.000000 specklia-1.8.9/specklia/client.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-02-27 11:34:21.000000 specklia-1.8.9/specklia/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 15:11:11.329601 specklia-1.8.9/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2897 2024-02-28 15:11:11.000000 specklia-1.8.9/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      365 2024-02-28 15:11:11.000000 specklia-1.8.9/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 15:11:11.000000 specklia-1.8.9/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-02-28 15:11:11.000000 specklia-1.8.9/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-02-28 15:11:11.000000 specklia-1.8.9/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 15:11:11.329601 specklia-1.8.9/tests/
+-rw-r--r--   0 root         (0) root         (0)    14649 2024-02-27 11:34:21.000000 specklia-1.8.9/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2024-02-27 11:34:21.000000 specklia-1.8.9/tests/test_utilities.py
+-rw-r--r--   0 root         (0) root         (0)    11629 2024-02-27 11:34:21.000000 specklia-1.8.9/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.8.8/LICENCE` & `specklia-1.8.9/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.8.8/PKG-INFO` & `specklia-1.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.8.8
+Version: 1.8.9
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/
 Project-URL: Changelog, https://specklia.earthwave.co.uk/generated_docs/change_log.html
```

### Comparing `specklia-1.8.8/README.md` & `specklia-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.8.8/setup.py` & `specklia-1.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.8/specklia/_websocket_helpers.py` & `specklia-1.8.9/specklia/_websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.8/specklia/client.py` & `specklia-1.8.9/specklia/client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.8/specklia/utilities.py` & `specklia-1.8.9/specklia/utilities.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.8/specklia.egg-info/PKG-INFO` & `specklia-1.8.9/specklia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.8.8
+Version: 1.8.9
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/
 Project-URL: Changelog, https://specklia.earthwave.co.uk/generated_docs/change_log.html
```

### Comparing `specklia-1.8.8/tests/test_client.py` & `specklia-1.8.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.8/tests/test_utilities.py` & `specklia-1.8.9/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.8/tests/test_websocket_helpers.py` & `specklia-1.8.9/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

