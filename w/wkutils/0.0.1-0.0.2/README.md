# Comparing `tmp/wkutils-0.0.1.tar.gz` & `tmp/wkutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkutils-0.0.1.tar", last modified: Thu May  2 06:22:18 2024, max compression
+gzip compressed data, was "wkutils-0.0.2.tar", last modified: Thu May  2 06:31:50 2024, max compression
```

## Comparing `wkutils-0.0.1.tar` & `wkutils-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:22:18.809733 wkutils-0.0.1/
--rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 06:22:18.809489 wkutils-0.0.1/PKG-INFO
--rw-r--r--   0 wernerkruger   (501) staff       (20)       31 2024-05-02 06:08:22.000000 wkutils-0.0.1/README.md
--rw-r--r--   0 wernerkruger   (501) staff       (20)       38 2024-05-02 06:22:18.809777 wkutils-0.0.1/setup.cfg
--rw-r--r--   0 wernerkruger   (501) staff       (20)      922 2024-05-02 06:22:05.000000 wkutils-0.0.1/setup.py
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:22:18.808156 wkutils-0.0.1/wkutils/
--rw-r--r--   0 wernerkruger   (501) staff       (20)      147 2024-05-02 06:15:46.000000 wkutils-0.0.1/wkutils/__init__.py
--rw-r--r--   0 wernerkruger   (501) staff       (20)      566 2024-05-02 06:15:37.000000 wkutils-0.0.1/wkutils/wkutils.py
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:22:18.809179 wkutils-0.0.1/wkutils.egg-info/
--rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 06:22:18.000000 wkutils-0.0.1/wkutils.egg-info/PKG-INFO
--rw-r--r--   0 wernerkruger   (501) staff       (20)      211 2024-05-02 06:22:18.000000 wkutils-0.0.1/wkutils.egg-info/SOURCES.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)        1 2024-05-02 06:22:18.000000 wkutils-0.0.1/wkutils.egg-info/dependency_links.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)       16 2024-05-02 06:22:18.000000 wkutils-0.0.1/wkutils.egg-info/requires.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)        8 2024-05-02 06:22:18.000000 wkutils-0.0.1/wkutils.egg-info/top_level.txt
+drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:31:50.705635 wkutils-0.0.2/
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 06:31:50.705359 wkutils-0.0.2/PKG-INFO
+-rw-r--r--   0 wernerkruger   (501) staff       (20)       31 2024-05-02 06:08:22.000000 wkutils-0.0.2/README.md
+-rw-r--r--   0 wernerkruger   (501) staff       (20)       38 2024-05-02 06:31:50.705686 wkutils-0.0.2/setup.cfg
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      922 2024-05-02 06:31:45.000000 wkutils-0.0.2/setup.py
+drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:31:50.703919 wkutils-0.0.2/wkutils/
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      110 2024-05-02 06:30:35.000000 wkutils-0.0.2/wkutils/__init__.py
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      566 2024-05-02 06:15:37.000000 wkutils-0.0.2/wkutils/wkutils.py
+drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:31:50.704980 wkutils-0.0.2/wkutils.egg-info/
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 06:31:50.000000 wkutils-0.0.2/wkutils.egg-info/PKG-INFO
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      211 2024-05-02 06:31:50.000000 wkutils-0.0.2/wkutils.egg-info/SOURCES.txt
+-rw-r--r--   0 wernerkruger   (501) staff       (20)        1 2024-05-02 06:31:50.000000 wkutils-0.0.2/wkutils.egg-info/dependency_links.txt
+-rw-r--r--   0 wernerkruger   (501) staff       (20)       16 2024-05-02 06:31:50.000000 wkutils-0.0.2/wkutils.egg-info/requires.txt
+-rw-r--r--   0 wernerkruger   (501) staff       (20)        8 2024-05-02 06:31:50.000000 wkutils-0.0.2/wkutils.egg-info/top_level.txt
```

### Comparing `wkutils-0.0.1/PKG-INFO` & `wkutils-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Useful utilities for python
 Author: Werner Kruger
 Author-email: <python@wkruger.com>
 Keywords: python,utilities,financial,calculator
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wkutils-0.0.1/setup.py` & `wkutils-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Useful utilities for python'
 LONG_DESCRIPTION = 'A package that contains a bunch of useful utilities I have collected over the years'
 
 # Setting up
 setup(
     name="wkutils",
     version=VERSION,
```

### Comparing `wkutils-0.0.1/wkutils/wkutils.py` & `wkutils-0.0.2/wkutils/wkutils.py`

 * *Files identical despite different names*

### Comparing `wkutils-0.0.1/wkutils.egg-info/PKG-INFO` & `wkutils-0.0.2/wkutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Useful utilities for python
 Author: Werner Kruger
 Author-email: <python@wkruger.com>
 Keywords: python,utilities,financial,calculator
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

