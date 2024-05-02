# Comparing `tmp/nbdevAuto-0.0.93.tar.gz` & `tmp/nbdevAuto-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdevAuto-0.0.93.tar", last modified: Fri Dec 15 12:13:09 2023, max compression
+gzip compressed data, was "nbdevAuto-0.0.95.tar", last modified: Fri Dec 15 12:15:45 2023, max compression
```

## Comparing `nbdevAuto-0.0.93.tar` & `nbdevAuto-0.0.95.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-12-15 12:13:09.411989 nbdevAuto-0.0.93/
--rw-r--r--   0 ben       (1000) ben       (1000)    11337 2023-12-15 11:13:41.000000 nbdevAuto-0.0.93/LICENSE
--rw-r--r--   0 ben       (1000) ben       (1000)      111 2023-12-15 11:13:41.000000 nbdevAuto-0.0.93/MANIFEST.in
--rw-r--r--   0 ben       (1000) ben       (1000)     1063 2023-12-15 12:13:09.411989 nbdevAuto-0.0.93/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)      303 2023-12-15 11:15:45.000000 nbdevAuto-0.0.93/README.md
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-12-15 12:13:09.411989 nbdevAuto-0.0.93/nbdevAuto/
--rw-r--r--   0 ben       (1000) ben       (1000)       23 2023-12-15 12:13:01.000000 nbdevAuto-0.0.93/nbdevAuto/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)     3795 2023-12-15 12:13:01.000000 nbdevAuto-0.0.93/nbdevAuto/_modidx.py
--rw-r--r--   0 ben       (1000) ben       (1000)     3222 2023-12-15 12:13:01.000000 nbdevAuto-0.0.93/nbdevAuto/automate.py
--rw-r--r--   0 ben       (1000) ben       (1000)      142 2023-12-15 11:13:41.000000 nbdevAuto-0.0.93/nbdevAuto/core.py
--rw-r--r--   0 ben       (1000) ben       (1000)     7612 2023-12-15 12:13:01.000000 nbdevAuto-0.0.93/nbdevAuto/functions.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-12-15 12:13:09.411989 nbdevAuto-0.0.93/nbdevAuto.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)     1063 2023-12-15 12:13:09.000000 nbdevAuto-0.0.93/nbdevAuto.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)      389 2023-12-15 12:13:09.000000 nbdevAuto-0.0.93/nbdevAuto.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-12-15 12:13:09.000000 nbdevAuto-0.0.93/nbdevAuto.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) ben       (1000)      483 2023-12-15 12:13:09.000000 nbdevAuto-0.0.93/nbdevAuto.egg-info/entry_points.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-12-15 11:15:58.000000 nbdevAuto-0.0.93/nbdevAuto.egg-info/not-zip-safe
--rw-r--r--   0 ben       (1000) ben       (1000)        7 2023-12-15 12:13:09.000000 nbdevAuto-0.0.93/nbdevAuto.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       10 2023-12-15 12:13:09.000000 nbdevAuto-0.0.93/nbdevAuto.egg-info/top_level.txt
--rw-r--r--   0 ben       (1000) ben       (1000)     1281 2023-12-15 12:13:01.000000 nbdevAuto-0.0.93/settings.ini
--rw-r--r--   0 ben       (1000) ben       (1000)       38 2023-12-15 12:13:09.411989 nbdevAuto-0.0.93/setup.cfg
--rw-r--r--   0 ben       (1000) ben       (1000)     2596 2023-12-15 11:13:41.000000 nbdevAuto-0.0.93/setup.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-12-15 12:15:45.161981 nbdevAuto-0.0.95/
+-rw-r--r--   0 ben       (1000) ben       (1000)    11337 2023-12-15 11:13:41.000000 nbdevAuto-0.0.95/LICENSE
+-rw-r--r--   0 ben       (1000) ben       (1000)      111 2023-12-15 11:13:41.000000 nbdevAuto-0.0.95/MANIFEST.in
+-rw-r--r--   0 ben       (1000) ben       (1000)     1063 2023-12-15 12:15:45.161981 nbdevAuto-0.0.95/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)      303 2023-12-15 11:15:45.000000 nbdevAuto-0.0.95/README.md
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-12-15 12:15:45.161981 nbdevAuto-0.0.95/nbdevAuto/
+-rw-r--r--   0 ben       (1000) ben       (1000)       23 2023-12-15 12:15:38.000000 nbdevAuto-0.0.95/nbdevAuto/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3795 2023-12-15 12:15:38.000000 nbdevAuto-0.0.95/nbdevAuto/_modidx.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3222 2023-12-15 12:15:38.000000 nbdevAuto-0.0.95/nbdevAuto/automate.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      142 2023-12-15 11:13:41.000000 nbdevAuto-0.0.95/nbdevAuto/core.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     7612 2023-12-15 12:15:38.000000 nbdevAuto-0.0.95/nbdevAuto/functions.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-12-15 12:15:45.161981 nbdevAuto-0.0.95/nbdevAuto.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1063 2023-12-15 12:15:45.000000 nbdevAuto-0.0.95/nbdevAuto.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)      389 2023-12-15 12:15:45.000000 nbdevAuto-0.0.95/nbdevAuto.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-12-15 12:15:45.000000 nbdevAuto-0.0.95/nbdevAuto.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)      483 2023-12-15 12:15:45.000000 nbdevAuto-0.0.95/nbdevAuto.egg-info/entry_points.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-12-15 11:15:58.000000 nbdevAuto-0.0.95/nbdevAuto.egg-info/not-zip-safe
+-rw-r--r--   0 ben       (1000) ben       (1000)        7 2023-12-15 12:15:45.000000 nbdevAuto-0.0.95/nbdevAuto.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       10 2023-12-15 12:15:45.000000 nbdevAuto-0.0.95/nbdevAuto.egg-info/top_level.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)     1281 2023-12-15 12:15:38.000000 nbdevAuto-0.0.95/settings.ini
+-rw-r--r--   0 ben       (1000) ben       (1000)       38 2023-12-15 12:15:45.161981 nbdevAuto-0.0.95/setup.cfg
+-rw-r--r--   0 ben       (1000) ben       (1000)     2596 2023-12-15 11:13:41.000000 nbdevAuto-0.0.95/setup.py
```

### Comparing `nbdevAuto-0.0.93/LICENSE` & `nbdevAuto-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdevAuto-0.0.93/PKG-INFO` & `nbdevAuto-0.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdevAuto
-Version: 0.0.93
+Version: 0.0.95
 Summary: automating nbdev
 Home-page: https://github.com/bthek1/nbdevAuto
 Author: Benedict Thekkel
 Author-email: bthekkel1@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nbdevAuto-0.0.93/nbdevAuto/_modidx.py` & `nbdevAuto-0.0.95/nbdevAuto/_modidx.py`

 * *Files identical despite different names*

### Comparing `nbdevAuto-0.0.93/nbdevAuto/automate.py` & `nbdevAuto-0.0.95/nbdevAuto/automate.py`

 * *Files identical despite different names*

### Comparing `nbdevAuto-0.0.93/nbdevAuto/functions.py` & `nbdevAuto-0.0.95/nbdevAuto/functions.py`

 * *Files identical despite different names*

### Comparing `nbdevAuto-0.0.93/nbdevAuto.egg-info/PKG-INFO` & `nbdevAuto-0.0.95/nbdevAuto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdevAuto
-Version: 0.0.93
+Version: 0.0.95
 Summary: automating nbdev
 Home-page: https://github.com/bthek1/nbdevAuto
 Author: Benedict Thekkel
 Author-email: bthekkel1@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nbdevAuto-0.0.93/settings.ini` & `nbdevAuto-0.0.95/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = nbdevAuto
 lib_name = nbdevAuto
-version = 0.0.93
+version = 0.0.95
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = nbdevAuto
 nbs_path = nbs
 recursive = True
```

### Comparing `nbdevAuto-0.0.93/setup.py` & `nbdevAuto-0.0.95/setup.py`

 * *Files identical despite different names*

