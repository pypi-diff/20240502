# Comparing `tmp/wkutils-0.0.4.tar.gz` & `tmp/wkutils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkutils-0.0.4.tar", last modified: Thu May  2 06:37:50 2024, max compression
+gzip compressed data, was "wkutils-0.0.5.tar", last modified: Thu May  2 06:42:02 2024, max compression
```

## Comparing `wkutils-0.0.4.tar` & `wkutils-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:37:50.866064 wkutils-0.0.4/
--rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 06:37:50.865716 wkutils-0.0.4/PKG-INFO
--rw-r--r--   0 wernerkruger   (501) staff       (20)       31 2024-05-02 06:08:22.000000 wkutils-0.0.4/README.md
--rw-r--r--   0 wernerkruger   (501) staff       (20)       38 2024-05-02 06:37:50.866131 wkutils-0.0.4/setup.cfg
--rw-r--r--   0 wernerkruger   (501) staff       (20)      922 2024-05-02 06:37:42.000000 wkutils-0.0.4/setup.py
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:37:50.864267 wkutils-0.0.4/wkutils/
--rw-r--r--   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:37:35.000000 wkutils-0.0.4/wkutils/__init__.py
--rw-r--r--   0 wernerkruger   (501) staff       (20)      565 2024-05-02 06:37:30.000000 wkutils-0.0.4/wkutils/my_utilities.py
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:37:50.865278 wkutils-0.0.4/wkutils.egg-info/
--rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 06:37:50.000000 wkutils-0.0.4/wkutils.egg-info/PKG-INFO
--rw-r--r--   0 wernerkruger   (501) staff       (20)      216 2024-05-02 06:37:50.000000 wkutils-0.0.4/wkutils.egg-info/SOURCES.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)        1 2024-05-02 06:37:50.000000 wkutils-0.0.4/wkutils.egg-info/dependency_links.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)       16 2024-05-02 06:37:50.000000 wkutils-0.0.4/wkutils.egg-info/requires.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)        8 2024-05-02 06:37:50.000000 wkutils-0.0.4/wkutils.egg-info/top_level.txt
+drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:42:02.169472 wkutils-0.0.5/
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 06:42:02.169224 wkutils-0.0.5/PKG-INFO
+-rw-r--r--   0 wernerkruger   (501) staff       (20)       31 2024-05-02 06:08:22.000000 wkutils-0.0.5/README.md
+-rw-r--r--   0 wernerkruger   (501) staff       (20)       38 2024-05-02 06:42:02.169564 wkutils-0.0.5/setup.cfg
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      922 2024-05-02 06:41:55.000000 wkutils-0.0.5/setup.py
+drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:42:02.168037 wkutils-0.0.5/wkutils/
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      565 2024-05-02 06:41:47.000000 wkutils-0.0.5/wkutils/__init__.py
+drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 06:42:02.168897 wkutils-0.0.5/wkutils.egg-info/
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 06:42:02.000000 wkutils-0.0.5/wkutils.egg-info/PKG-INFO
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      192 2024-05-02 06:42:02.000000 wkutils-0.0.5/wkutils.egg-info/SOURCES.txt
+-rw-r--r--   0 wernerkruger   (501) staff       (20)        1 2024-05-02 06:42:02.000000 wkutils-0.0.5/wkutils.egg-info/dependency_links.txt
+-rw-r--r--   0 wernerkruger   (501) staff       (20)       16 2024-05-02 06:42:02.000000 wkutils-0.0.5/wkutils.egg-info/requires.txt
+-rw-r--r--   0 wernerkruger   (501) staff       (20)        8 2024-05-02 06:42:02.000000 wkutils-0.0.5/wkutils.egg-info/top_level.txt
```

### Comparing `wkutils-0.0.4/PKG-INFO` & `wkutils-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkutils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Useful utilities for python
 Author: Werner Kruger
 Author-email: <python@wkruger.com>
 Keywords: python,utilities,financial,calculator
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wkutils-0.0.4/setup.py` & `wkutils-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Useful utilities for python'
 LONG_DESCRIPTION = 'A package that contains a bunch of useful utilities I have collected over the years'
 
 # Setting up
 setup(
     name="wkutils",
     version=VERSION,
```

### Comparing `wkutils-0.0.4/wkutils/my_utilities.py` & `wkutils-0.0.5/wkutils/__init__.py`

 * *Files identical despite different names*

### Comparing `wkutils-0.0.4/wkutils.egg-info/PKG-INFO` & `wkutils-0.0.5/wkutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkutils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Useful utilities for python
 Author: Werner Kruger
 Author-email: <python@wkruger.com>
 Keywords: python,utilities,financial,calculator
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

