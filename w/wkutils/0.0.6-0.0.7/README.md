# Comparing `tmp/wkutils-0.0.6.tar.gz` & `tmp/wkutils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkutils-0.0.6.tar", last modified: Thu May  2 08:13:32 2024, max compression
+gzip compressed data, was "wkutils-0.0.7.tar", last modified: Thu May  2 08:18:31 2024, max compression
```

## Comparing `wkutils-0.0.6.tar` & `wkutils-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 08:13:32.791152 wkutils-0.0.6/
--rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 08:13:32.790841 wkutils-0.0.6/PKG-INFO
--rw-r--r--   0 wernerkruger   (501) staff       (20)       31 2024-05-02 06:08:22.000000 wkutils-0.0.6/README.md
--rw-r--r--   0 wernerkruger   (501) staff       (20)       38 2024-05-02 08:13:32.791208 wkutils-0.0.6/setup.cfg
--rw-r--r--   0 wernerkruger   (501) staff       (20)      922 2024-05-02 08:13:25.000000 wkutils-0.0.6/setup.py
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 08:13:32.788348 wkutils-0.0.6/wkutils/
--rw-r--r--   0 wernerkruger   (501) staff       (20)      864 2024-05-02 08:10:00.000000 wkutils-0.0.6/wkutils/__init__.py
-drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 08:13:32.790077 wkutils-0.0.6/wkutils.egg-info/
--rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 08:13:32.000000 wkutils-0.0.6/wkutils.egg-info/PKG-INFO
--rw-r--r--   0 wernerkruger   (501) staff       (20)      192 2024-05-02 08:13:32.000000 wkutils-0.0.6/wkutils.egg-info/SOURCES.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)        1 2024-05-02 08:13:32.000000 wkutils-0.0.6/wkutils.egg-info/dependency_links.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)       16 2024-05-02 08:13:32.000000 wkutils-0.0.6/wkutils.egg-info/requires.txt
--rw-r--r--   0 wernerkruger   (501) staff       (20)        8 2024-05-02 08:13:32.000000 wkutils-0.0.6/wkutils.egg-info/top_level.txt
+drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 08:18:31.838726 wkutils-0.0.7/
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 08:18:31.838465 wkutils-0.0.7/PKG-INFO
+-rw-r--r--   0 wernerkruger   (501) staff       (20)       31 2024-05-02 06:08:22.000000 wkutils-0.0.7/README.md
+-rw-r--r--   0 wernerkruger   (501) staff       (20)       38 2024-05-02 08:18:31.838783 wkutils-0.0.7/setup.cfg
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      922 2024-05-02 08:18:25.000000 wkutils-0.0.7/setup.py
+drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 08:18:31.836719 wkutils-0.0.7/wkutils/
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      862 2024-05-02 08:18:19.000000 wkutils-0.0.7/wkutils/__init__.py
+drwxr-xr-x   0 wernerkruger   (501) staff       (20)        0 2024-05-02 08:18:31.838111 wkutils-0.0.7/wkutils.egg-info/
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      627 2024-05-02 08:18:31.000000 wkutils-0.0.7/wkutils.egg-info/PKG-INFO
+-rw-r--r--   0 wernerkruger   (501) staff       (20)      192 2024-05-02 08:18:31.000000 wkutils-0.0.7/wkutils.egg-info/SOURCES.txt
+-rw-r--r--   0 wernerkruger   (501) staff       (20)        1 2024-05-02 08:18:31.000000 wkutils-0.0.7/wkutils.egg-info/dependency_links.txt
+-rw-r--r--   0 wernerkruger   (501) staff       (20)       16 2024-05-02 08:18:31.000000 wkutils-0.0.7/wkutils.egg-info/requires.txt
+-rw-r--r--   0 wernerkruger   (501) staff       (20)        8 2024-05-02 08:18:31.000000 wkutils-0.0.7/wkutils.egg-info/top_level.txt
```

### Comparing `wkutils-0.0.6/PKG-INFO` & `wkutils-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Useful utilities for python
 Author: Werner Kruger
 Author-email: <python@wkruger.com>
 Keywords: python,utilities,financial,calculator
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wkutils-0.0.6/setup.py` & `wkutils-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Useful utilities for python'
 LONG_DESCRIPTION = 'A package that contains a bunch of useful utilities I have collected over the years'
 
 # Setting up
 setup(
     name="wkutils",
     version=VERSION,
```

### Comparing `wkutils-0.0.6/wkutils/__init__.py` & `wkutils-0.0.7/wkutils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 def gross_payment(rate, nper, pv):
     '''
         
     '''
     return float(twoDecimalPlaces(npf.pmt(rate/(nper*12), nper*12, pv)))
 
 def net_payment(grosspayment):
-    return float(twoDecimalPlaces(grosspayment * (1-0.3693)))
+    return float(twoDecimalPlaces(grosspayment * (1-0.22)))
 
 def calculate_loan_payments(rate, nper, pv):
     gp = gross_payment(rate, nper, pv)
     np = net_payment(gp)
     print('Gross payment:', gp)
     print('Net payment:', np)
```

### Comparing `wkutils-0.0.6/wkutils.egg-info/PKG-INFO` & `wkutils-0.0.7/wkutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Useful utilities for python
 Author: Werner Kruger
 Author-email: <python@wkruger.com>
 Keywords: python,utilities,financial,calculator
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

