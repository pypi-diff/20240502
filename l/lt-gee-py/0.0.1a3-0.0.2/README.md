# Comparing `tmp/lt_gee_py-0.0.1a3.tar.gz` & `tmp/lt_gee_py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lt_gee_py-0.0.1a3.tar", last modified: Fri Apr 26 00:53:33 2024, max compression
+gzip compressed data, was "lt_gee_py-0.0.2.tar", last modified: Thu May  2 17:04:01 2024, max compression
```

## Comparing `lt_gee_py-0.0.1a3.tar` & `lt_gee_py-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.108868 lt_gee_py-0.0.1a3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.104868 lt_gee_py-0.0.1a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.104868 lt_gee_py-0.0.1a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-04-26 00:53:33.108868 lt_gee_py-0.0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.104868 lt_gee_py-0.0.1a3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    33927 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/examples/basic_examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 00:53:33.108868 lt_gee_py-0.0.1a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.104868 lt_gee_py-0.0.1a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.108868 lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-04-26 00:53:33.000000 lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-26 00:53:33.000000 lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 00:53:33.000000 lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 00:53:33.000000 lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:53:33.108868 lt_gee_py-0.0.1a3/src/ltgee/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/src/ltgee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/src/ltgee/gee_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    44824 2024-04-26 00:53:12.000000 lt_gee_py-0.0.1a3/src/ltgee/landtrendr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:04:01.109618 lt_gee_py-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:04:01.105618 lt_gee_py-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:04:01.105618 lt_gee_py-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-02 17:03:56.000000 lt_gee_py-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-02 17:03:56.000000 lt_gee_py-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-02 17:03:56.000000 lt_gee_py-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-02 17:03:56.000000 lt_gee_py-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20701 2024-05-02 17:04:01.109618 lt_gee_py-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-02 17:03:56.000000 lt_gee_py-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:04:01.105618 lt_gee_py-0.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    33927 2024-05-02 17:03:56.000000 lt_gee_py-0.0.2/examples/basic_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-02 17:03:56.000000 lt_gee_py-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:04:01.109618 lt_gee_py-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:04:01.105618 lt_gee_py-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:04:01.109618 lt_gee_py-0.0.2/src/lt_gee_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20701 2024-05-02 17:04:01.000000 lt_gee_py-0.0.2/src/lt_gee_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-02 17:04:01.000000 lt_gee_py-0.0.2/src/lt_gee_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:04:01.000000 lt_gee_py-0.0.2/src/lt_gee_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 17:04:01.000000 lt_gee_py-0.0.2/src/lt_gee_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:04:01.109618 lt_gee_py-0.0.2/src/ltgee/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 17:03:56.000000 lt_gee_py-0.0.2/src/ltgee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-05-02 17:03:56.000000 lt_gee_py-0.0.2/src/ltgee/gee_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44819 2024-05-02 17:03:56.000000 lt_gee_py-0.0.2/src/ltgee/landtrendr.py
```

### Comparing `lt_gee_py-0.0.1a3/.github/workflows/python-publish.yml` & `lt_gee_py-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lt_gee_py-0.0.1a3/.gitignore` & `lt_gee_py-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lt_gee_py-0.0.1a3/CONTRIBUTING.md` & `lt_gee_py-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lt_gee_py-0.0.1a3/LICENSE` & `lt_gee_py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lt_gee_py-0.0.1a3/PKG-INFO` & `lt_gee_py-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lt-gee-py
-Version: 0.0.1a3
+Version: 0.0.2
 Summary: Python interface to the Google Earth Engine implementation of the LandTrendr spectral-temporal segmentation algorithm.
 Author-email: Myscon Truong <myscontruong@gmail.com>, Robert Kennedy <robert.kennedy@oregonstate.edu>, Peter Clary <clarype@oregonstate.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -254,15 +254,15 @@
 earthengine authenticate # There are several alternatives for this. See link above.
 ```
 
 ## Basic Usage
 
 ```python
 import ee
-from ltgee import LandTrendr
+from ltgee import LandTrendr, LandsatComposite, LtCollection
 
 # Initialize access to Google's EE servers
 ee.Initialize("my_project_name")
 
 # Initialize variables for LandTrendr algorithm
 composite_params = {
     "start_date": date(1985, 6,1),
```

### Comparing `lt_gee_py-0.0.1a3/README.md` & `lt_gee_py-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 earthengine authenticate # There are several alternatives for this. See link above.
 ```
 
 ## Basic Usage
 
 ```python
 import ee
-from ltgee import LandTrendr
+from ltgee import LandTrendr, LandsatComposite, LtCollection
 
 # Initialize access to Google's EE servers
 ee.Initialize("my_project_name")
 
 # Initialize variables for LandTrendr algorithm
 composite_params = {
     "start_date": date(1985, 6,1),
```

### Comparing `lt_gee_py-0.0.1a3/examples/basic_examples.ipynb` & `lt_gee_py-0.0.2/examples/basic_examples.ipynb`

 * *Files identical despite different names*

### Comparing `lt_gee_py-0.0.1a3/pyproject.toml` & `lt_gee_py-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lt_gee_py-0.0.1a3/src/lt_gee_py.egg-info/PKG-INFO` & `lt_gee_py-0.0.2/src/lt_gee_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lt-gee-py
-Version: 0.0.1a3
+Version: 0.0.2
 Summary: Python interface to the Google Earth Engine implementation of the LandTrendr spectral-temporal segmentation algorithm.
 Author-email: Myscon Truong <myscontruong@gmail.com>, Robert Kennedy <robert.kennedy@oregonstate.edu>, Peter Clary <clarype@oregonstate.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -254,15 +254,15 @@
 earthengine authenticate # There are several alternatives for this. See link above.
 ```
 
 ## Basic Usage
 
 ```python
 import ee
-from ltgee import LandTrendr
+from ltgee import LandTrendr, LandsatComposite, LtCollection
 
 # Initialize access to Google's EE servers
 ee.Initialize("my_project_name")
 
 # Initialize variables for LandTrendr algorithm
 composite_params = {
     "start_date": date(1985, 6,1),
```

### Comparing `lt_gee_py-0.0.1a3/src/ltgee/gee_utils.py` & `lt_gee_py-0.0.2/src/ltgee/gee_utils.py`

 * *Files identical despite different names*

### Comparing `lt_gee_py-0.0.1a3/src/ltgee/landtrendr.py` & `lt_gee_py-0.0.2/src/ltgee/landtrendr.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
                 collection = collection.filter(ee.Filter.neq(
                     'system:index', image_id.split('/')[-1]))
 
         if 'slcOff' in self.exclude:
             if self.exclude['slcOff'] is True:
                 collection = collection.filter(ee.Filter.And(
                     ee.Filter.eq('SPACECRAFT_ID', 'LANDSAT_7'),
-                    ee.Filter.gt('SCENE_CENTER_TIME', '2003-06-01T00:00')
+                    ee.Filter.gt('system:time_start', 1054425600000)
                 ).Not())
         return collection
 
 
 class LtCollection(ee.ImageCollection):
     """
```

