# Comparing `tmp/aanalyticsact_1-0.0.1.50.tar.gz` & `tmp/aanalyticsact_1-0.0.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aanalyticsact_1-0.0.1.50.tar", last modified: Wed Apr 24 05:08:48 2024, max compression
+gzip compressed data, was "aanalyticsact_1-0.0.1.51.tar", last modified: Thu May  2 08:43:33 2024, max compression
```

## Comparing `aanalyticsact_1-0.0.1.50.tar` & `aanalyticsact_1-0.0.1.51.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 05:08:48.716898 aanalyticsact_1-0.0.1.50/
--rw-rw-rw-   0        0        0      191 2024-04-24 05:08:48.715936 aanalyticsact_1-0.0.1.50/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 05:08:48.710581 aanalyticsact_1-0.0.1.50/aanalyticsact_1/
--rw-rw-rw-   0        0        0      151 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1/__init__.py
--rw-rw-rw-   0        0        0       24 2024-04-24 05:06:20.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1/__version__.py
--rw-rw-rw-   0        0        0     7109 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1/actExecute.py
--rw-rw-rw-   0        0        0    18036 2024-04-24 05:03:50.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1/actModuler.py
--rw-rw-rw-   0        0        0     9139 2024-04-18 06:51:22.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1/actRunner.py
-drwxrwxrwx   0        0        0        0 2024-04-24 05:08:48.714903 aanalyticsact_1-0.0.1.50/aanalyticsact_1.egg-info/
--rw-rw-rw-   0        0        0      191 2024-04-24 05:08:48.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-04-24 05:08:48.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 05:08:48.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-24 05:08:48.000000 aanalyticsact_1-0.0.1.50/aanalyticsact_1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 05:08:48.716898 aanalyticsact_1-0.0.1.50/setup.cfg
--rw-rw-rw-   0        0        0      732 2024-04-24 05:08:44.000000 aanalyticsact_1-0.0.1.50/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 08:43:33.956910 aanalyticsact_1-0.0.1.51/
+-rw-rw-rw-   0        0        0      191 2024-05-02 08:43:33.955913 aanalyticsact_1-0.0.1.51/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 08:43:33.951026 aanalyticsact_1-0.0.1.51/aanalyticsact_1/
+-rw-rw-rw-   0        0        0      151 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1/__init__.py
+-rw-rw-rw-   0        0        0       24 2024-04-24 05:06:20.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1/__version__.py
+-rw-rw-rw-   0        0        0     7109 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1/actExecute.py
+-rw-rw-rw-   0        0        0    18036 2024-04-24 05:03:50.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1/actModuler.py
+-rw-rw-rw-   0        0        0     9139 2024-04-18 06:51:22.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1/actRunner.py
+drwxrwxrwx   0        0        0        0 2024-05-02 08:43:33.954916 aanalyticsact_1-0.0.1.51/aanalyticsact_1.egg-info/
+-rw-rw-rw-   0        0        0      191 2024-05-02 08:43:33.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-05-02 08:43:33.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 08:43:33.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-02 08:43:33.000000 aanalyticsact_1-0.0.1.51/aanalyticsact_1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 08:43:33.956910 aanalyticsact_1-0.0.1.51/setup.cfg
+-rw-rw-rw-   0        0        0      732 2024-05-02 08:42:51.000000 aanalyticsact_1-0.0.1.51/setup.py
```

### Comparing `aanalyticsact_1-0.0.1.50/aanalyticsact_1/actExecute.py` & `aanalyticsact_1-0.0.1.51/aanalyticsact_1/actExecute.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact_1-0.0.1.50/aanalyticsact_1/actModuler.py` & `aanalyticsact_1-0.0.1.51/aanalyticsact_1/actModuler.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact_1-0.0.1.50/aanalyticsact_1/actRunner.py` & `aanalyticsact_1-0.0.1.51/aanalyticsact_1/actRunner.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact_1-0.0.1.50/setup.py` & `aanalyticsact_1-0.0.1.51/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 
 from setuptools import find_packages, setup
 
 # Package meta-data.
 NAME = 'aanalyticsact_1'
-Version= '0.0.1.50'
+Version= '0.0.1.51'
 URL = 'https://github.com/Glory-Cho/aanalyticsact)1'
 Summary= 'adobe analytics library for Team ACT'
 EMAIL = 'youngkwang.cho@concentrix.com'
 AUTHOR = 'Youngkwang Cho'
 
 here = os.path.abspath(os.path.dirname(__file__))
```

