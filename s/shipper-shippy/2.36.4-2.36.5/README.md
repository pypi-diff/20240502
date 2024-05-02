# Comparing `tmp/shipper_shippy-2.36.4.tar.gz` & `tmp/shipper_shippy-2.36.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper_shippy-2.36.4.tar", last modified: Mon Apr 29 21:29:20 2024, max compression
+gzip compressed data, was "shipper_shippy-2.36.5.tar", last modified: Thu May  2 04:47:58 2024, max compression
```

## Comparing `shipper_shippy-2.36.4.tar` & `shipper_shippy-2.36.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:29:20.735770 shipper_shippy-2.36.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-29 21:29:20.735770 shipper_shippy-2.36.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 21:29:20.735770 shipper_shippy-2.36.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:29:20.731770 shipper_shippy-2.36.4/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-29 21:29:20.000000 shipper_shippy-2.36.4/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-29 21:29:20.000000 shipper_shippy-2.36.4/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:29:20.000000 shipper_shippy-2.36.4/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 21:29:20.000000 shipper_shippy-2.36.4/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 21:29:20.000000 shipper_shippy-2.36.4/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 21:29:20.000000 shipper_shippy-2.36.4/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:29:20.731770 shipper_shippy-2.36.4/shippy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/shippy/server_compat_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 21:29:10.000000 shipper_shippy-2.36.4/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:47:58.246729 shipper_shippy-2.36.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-02 04:47:58.246729 shipper_shippy-2.36.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 04:47:58.246729 shipper_shippy-2.36.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:47:58.242729 shipper_shippy-2.36.5/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-02 04:47:58.000000 shipper_shippy-2.36.5/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-02 04:47:58.000000 shipper_shippy-2.36.5/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 04:47:58.000000 shipper_shippy-2.36.5/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 04:47:58.000000 shipper_shippy-2.36.5/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 04:47:58.000000 shipper_shippy-2.36.5/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 04:47:58.000000 shipper_shippy-2.36.5/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:47:58.242729 shipper_shippy-2.36.5/shippy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 04:47:50.000000 shipper_shippy-2.36.5/shippy/version.py
```

### Comparing `shipper_shippy-2.36.4/PKG-INFO` & `shipper_shippy-2.36.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.36.4
+Version: 2.36.5
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper_shippy-2.36.4/README.md` & `shipper_shippy-2.36.5/README.md`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.4/setup.py` & `shipper_shippy-2.36.5/setup.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.4/shipper_shippy.egg-info/PKG-INFO` & `shipper_shippy-2.36.5/shipper_shippy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.36.4
+Version: 2.36.5
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper_shippy-2.36.4/shippy/__main__.py` & `shipper_shippy-2.36.5/shippy/__main__.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.4/shippy/client.py` & `shipper_shippy-2.36.5/shippy/client.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.4/shippy/config.py` & `shipper_shippy-2.36.5/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.4/shippy/constants.py` & `shipper_shippy-2.36.5/shippy/constants.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.4/shippy/helper.py` & `shipper_shippy-2.36.5/shippy/helper.py`

 * *Files identical despite different names*

