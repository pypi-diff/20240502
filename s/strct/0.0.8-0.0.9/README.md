# Comparing `tmp/strct-0.0.8.tar.gz` & `tmp/strct-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/strct-0.0.8.tar", last modified: Tue Oct 31 09:59:23 2017, max compression
+gzip compressed data, was "dist/strct-0.0.9.tar", last modified: Sat Nov  4 17:52:40 2017, max compression
```

## Comparing `strct-0.0.8.tar` & `strct-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2017-10-31 09:59:23.000000 strct-0.0.8/
--rw-r--r--   0 shaypalachy   (501) staff       (20)       48 2017-10-09 09:39:18.000000 strct-0.0.8/MANIFEST.in
--rw-r--r--   0 shaypalachy   (501) staff       (20)     4430 2017-10-31 09:59:23.000000 strct-0.0.8/PKG-INFO
--rw-r--r--   0 shaypalachy   (501) staff       (20)     2714 2017-10-09 12:07:54.000000 strct-0.0.8/README.rst
--rw-r--r--   0 shaypalachy   (501) staff       (20)      245 2017-10-31 09:59:23.000000 strct-0.0.8/setup.cfg
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1551 2017-10-09 12:23:35.000000 strct-0.0.8/setup.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2017-10-31 09:59:23.000000 strct-0.0.8/strct/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      276 2017-10-09 09:39:23.000000 strct-0.0.8/strct/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      497 2017-10-31 09:59:23.000000 strct-0.0.8/strct/_version.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2017-10-31 09:59:23.000000 strct-0.0.8/strct.egg-info/
--rw-r--r--   0 shaypalachy   (501) staff       (20)        1 2017-10-31 09:59:23.000000 strct-0.0.8/strct.egg-info/dependency_links.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)     4430 2017-10-31 09:59:23.000000 strct-0.0.8/strct.egg-info/PKG-INFO
--rw-r--r--   0 shaypalachy   (501) staff       (20)       52 2017-10-31 09:59:23.000000 strct-0.0.8/strct.egg-info/requires.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)      235 2017-10-31 09:59:23.000000 strct-0.0.8/strct.egg-info/SOURCES.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)        6 2017-10-31 09:59:23.000000 strct-0.0.8/strct.egg-info/top_level.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)    68611 2017-10-09 09:06:06.000000 strct-0.0.8/versioneer.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2017-11-04 17:52:40.000000 strct-0.0.9/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       48 2017-10-09 09:39:18.000000 strct-0.0.9/MANIFEST.in
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     4430 2017-11-04 17:52:40.000000 strct-0.0.9/PKG-INFO
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     2714 2017-10-09 12:07:54.000000 strct-0.0.9/README.rst
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      245 2017-11-04 17:52:40.000000 strct-0.0.9/setup.cfg
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1551 2017-11-01 12:04:22.000000 strct-0.0.9/setup.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2017-11-04 17:52:40.000000 strct-0.0.9/strct/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      410 2017-11-04 17:50:07.000000 strct-0.0.9/strct/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      497 2017-11-04 17:52:40.000000 strct-0.0.9/strct/_version.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2017-11-04 17:52:40.000000 strct-0.0.9/strct.egg-info/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        1 2017-11-04 17:52:40.000000 strct-0.0.9/strct.egg-info/dependency_links.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     4430 2017-11-04 17:52:40.000000 strct-0.0.9/strct.egg-info/PKG-INFO
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       52 2017-11-04 17:52:40.000000 strct-0.0.9/strct.egg-info/requires.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      235 2017-11-04 17:52:40.000000 strct-0.0.9/strct.egg-info/SOURCES.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        6 2017-11-04 17:52:40.000000 strct-0.0.9/strct.egg-info/top_level.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    68611 2017-10-09 09:06:06.000000 strct-0.0.9/versioneer.py
```

### Comparing `strct-0.0.8/PKG-INFO` & `strct-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: strct
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small pure-python package for data structure relatedutility functions.
 Home-page: https://github.com/shaypal5/strct
 Author: Shay Palachy
 Author-email: shaypal5@gmail.com
 License: MIT
 Description: strct
         #########
```

### Comparing `strct-0.0.8/README.rst` & `strct-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `strct-0.0.8/setup.py` & `strct-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `strct-0.0.8/strct.egg-info/PKG-INFO` & `strct-0.0.9/strct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: strct
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small pure-python package for data structure relatedutility functions.
 Home-page: https://github.com/shaypal5/strct
 Author: Shay Palachy
 Author-email: shaypal5@gmail.com
 License: MIT
 Description: strct
         #########
```

### Comparing `strct-0.0.8/versioneer.py` & `strct-0.0.9/versioneer.py`

 * *Files identical despite different names*

