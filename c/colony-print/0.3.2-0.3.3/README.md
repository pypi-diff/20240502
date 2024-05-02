# Comparing `tmp/colony-print-0.3.2.tar.gz` & `tmp/colony-print-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/colony-print-0.3.2.tar", last modified: Wed May  1 13:26:31 2024, max compression
+gzip compressed data, was "dist/colony-print-0.3.3.tar", last modified: Thu May  2 08:33:03 2024, max compression
```

## Comparing `colony-print-0.3.2.tar` & `colony-print-0.3.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/
--rw-r--r--   0 root         (0) root         (0)     1979 2024-05-01 13:26:01.000000 colony-print-0.3.2/setup.py
--rw-r--r--   0 root         (0) root         (0)     2971 2024-05-01 13:26:01.000000 colony-print-0.3.2/README.md
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-01 13:26:31.000000 colony-print-0.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4677 2024-05-01 13:26:31.000000 colony-print-0.3.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1463 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4677 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       45 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 13:26:27.000000 colony-print-0.3.2/src/colony_print.egg-info/not-zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print/printing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print/printing/binie/
--rw-r--r--   0 root         (0) root         (0)      875 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/binie/system.py
--rw-r--r--   0 root         (0) root         (0)      263 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/binie/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20906 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/binie/visitor.py
--rw-r--r--   0 root         (0) root         (0)      870 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/binie/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print/printing/manager/
--rw-r--r--   0 root         (0) root         (0)     4311 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/manager/system.py
--rw-r--r--   0 root         (0) root         (0)     2312 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/manager/ast.py
--rw-r--r--   0 root         (0) root         (0)      488 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7810 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/manager/parser.py
--rw-r--r--   0 root         (0) root         (0)     2787 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/manager/visitor.py
--rw-r--r--   0 root         (0) root         (0)      874 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/manager/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      222 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print/printing/common/
--rw-r--r--   0 root         (0) root         (0)     2712 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/common/base.py
--rw-r--r--   0 root         (0) root         (0)      111 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print/printing/pdf/
--rw-r--r--   0 root         (0) root         (0)      969 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/pdf/system.py
--rw-r--r--   0 root         (0) root         (0)      272 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/pdf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33965 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/pdf/visitor.py
--rw-r--r--   0 root         (0) root         (0)     1462 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/printing/pdf/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print/static/example/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print/static/example/js/
--rw-r--r--   0 root         (0) root         (0)     3555 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/static/example/js/main.js
--rw-r--r--   0 root         (0) root         (0)      594 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/static/example/print.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print/static/example/xml/
--rw-r--r--   0 root         (0) root         (0)      251 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/static/example/xml/hello.xml
--rw-r--r--   0 root         (0) root         (0)    26876 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/static/example/xml/money_sale_slip.xml
--rw-r--r--   0 root         (0) root         (0)     6371 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/node.py
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/__init__.py
--rw-r--r--   0 root         (0) root         (0)      461 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:26:31.000000 colony-print-0.3.2/src/colony_print/controllers/
--rw-r--r--   0 root         (0) root         (0)      117 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/controllers/base.py
--rw-r--r--   0 root         (0) root         (0)      981 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/controllers/printer.py
--rw-r--r--   0 root         (0) root         (0)     5618 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/controllers/node.py
--rw-r--r--   0 root         (0) root         (0)      285 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2790 2024-05-01 13:26:01.000000 colony-print-0.3.2/src/colony_print/controllers/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/
+-rw-r--r--   0 root         (0) root         (0)     1979 2024-05-02 08:32:35.000000 colony-print-0.3.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2024-05-02 08:32:35.000000 colony-print-0.3.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-02 08:33:03.000000 colony-print-0.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4677 2024-05-02 08:33:03.000000 colony-print-0.3.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4677 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 08:32:59.000000 colony-print-0.3.3/src/colony_print.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print/printing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print/printing/binie/
+-rw-r--r--   0 root         (0) root         (0)      875 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/binie/system.py
+-rw-r--r--   0 root         (0) root         (0)      263 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/binie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20906 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/binie/visitor.py
+-rw-r--r--   0 root         (0) root         (0)      870 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/binie/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print/printing/manager/
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/manager/system.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/manager/ast.py
+-rw-r--r--   0 root         (0) root         (0)      488 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7810 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/manager/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/manager/visitor.py
+-rw-r--r--   0 root         (0) root         (0)      874 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/manager/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      222 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print/printing/common/
+-rw-r--r--   0 root         (0) root         (0)     2712 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/common/base.py
+-rw-r--r--   0 root         (0) root         (0)      111 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print/printing/pdf/
+-rw-r--r--   0 root         (0) root         (0)      969 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/pdf/system.py
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/pdf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33965 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/pdf/visitor.py
+-rw-r--r--   0 root         (0) root         (0)     1462 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/printing/pdf/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print/static/example/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print/static/example/js/
+-rw-r--r--   0 root         (0) root         (0)     3555 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/static/example/js/main.js
+-rw-r--r--   0 root         (0) root         (0)      594 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/static/example/print.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print/static/example/xml/
+-rw-r--r--   0 root         (0) root         (0)      251 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/static/example/xml/hello.xml
+-rw-r--r--   0 root         (0) root         (0)    26876 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/static/example/xml/money_sale_slip.xml
+-rw-r--r--   0 root         (0) root         (0)     6891 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/node.py
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      461 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:33:03.000000 colony-print-0.3.3/src/colony_print/controllers/
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/controllers/base.py
+-rw-r--r--   0 root         (0) root         (0)      981 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/controllers/printer.py
+-rw-r--r--   0 root         (0) root         (0)     5618 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/controllers/node.py
+-rw-r--r--   0 root         (0) root         (0)      285 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-05-02 08:32:35.000000 colony-print-0.3.3/src/colony_print/controllers/document.py
```

### Comparing `colony-print-0.3.2/setup.py` & `colony-print-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import setuptools
 
 setuptools.setup(
     name="colony-print",
-    version="0.3.2",
+    version="0.3.3",
     author="Hive Solutions Lda.",
     author_email="development@hive.pt",
     description="Colony Print Infra-structure",
     license="Apache License, Version 2.0",
     keywords="colony print native",
     url="http://colony-print.hive.pt",
     zip_safe=False,
```

### Comparing `colony-print-0.3.2/README.md` & `colony-print-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/PKG-INFO` & `colony-print-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colony-print
-Version: 0.3.2
+Version: 0.3.3
 Summary: Colony Print Infra-structure
 Home-page: http://colony-print.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Colony Print Infra-structure](http://colony-print.hive.pt)
```

### Comparing `colony-print-0.3.2/src/colony_print.egg-info/SOURCES.txt` & `colony-print-0.3.3/src/colony_print.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print.egg-info/PKG-INFO` & `colony-print-0.3.3/src/colony_print.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colony-print
-Version: 0.3.2
+Version: 0.3.3
 Summary: Colony Print Infra-structure
 Home-page: http://colony-print.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Colony Print Infra-structure](http://colony-print.hive.pt)
```

### Comparing `colony-print-0.3.2/src/colony_print/printing/binie/system.py` & `colony-print-0.3.3/src/colony_print/printing/binie/system.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/printing/binie/visitor.py` & `colony-print-0.3.3/src/colony_print/printing/binie/visitor.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/printing/binie/exceptions.py` & `colony-print-0.3.3/src/colony_print/printing/binie/exceptions.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/printing/manager/system.py` & `colony-print-0.3.3/src/colony_print/printing/manager/system.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/printing/manager/ast.py` & `colony-print-0.3.3/src/colony_print/printing/manager/ast.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/printing/manager/parser.py` & `colony-print-0.3.3/src/colony_print/printing/manager/parser.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/printing/manager/visitor.py` & `colony-print-0.3.3/src/colony_print/printing/manager/visitor.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/printing/manager/exceptions.py` & `colony-print-0.3.3/src/colony_print/printing/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/printing/common/base.py` & `colony-print-0.3.3/src/colony_print/printing/common/base.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/printing/pdf/system.py` & `colony-print-0.3.3/src/colony_print/printing/pdf/system.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/printing/pdf/visitor.py` & `colony-print-0.3.3/src/colony_print/printing/pdf/visitor.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/printing/pdf/exceptions.py` & `colony-print-0.3.3/src/colony_print/printing/pdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/static/example/js/main.js` & `colony-print-0.3.3/src/colony_print/static/example/js/main.js`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/static/example/print.html` & `colony-print-0.3.3/src/colony_print/static/example/print.html`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/static/example/xml/money_sale_slip.xml` & `colony-print-0.3.3/src/colony_print/static/example/xml/money_sale_slip.xml`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/node.py` & `colony-print-0.3.3/src/colony_print/node.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,29 +25,32 @@
 
 
 class ColonyPrintNode(object):
     def __init__(self, sleep_time=SLEEP_TIME):
         self.sleep_time = sleep_time
         self.node_mode = None
         self.node_printer = None
-        self.node_email_address = None
+        self.node_email_receivers = None
 
     def loop(self):
         logging.basicConfig(
             format="%(asctime)s [%(levelname)s] %(message)s", level=logging.DEBUG
         )
 
         base_url = appier.conf("BASE_URL", BASE_URL)
         secret_key = appier.conf("SECRET_KEY", None)
         node_id = appier.conf("NODE_ID", "node")
         node_name = appier.conf("NODE_NAME", "node")
         node_location = appier.conf("NODE_LOCATION", "undefined")
         self.node_mode = appier.conf("NODE_MODE", "normal")
         self.node_printer = appier.conf("NODE_PRINTER", "default")
-        self.node_email_address = appier.conf("NODE_EMAIL_ADDRESS", "normal")
+        self.node_email_receivers = appier.conf("NODE_EMAIL_RECEIVER", [], cast=list)
+        self.node_email_receivers = appier.conf(
+            "NODE_EMAIL_RECEIVERS", self.node_email_receivers, cast=list
+        )
 
         headers = dict()
         if secret_key:
             headers["X-Secret-Key"] = secret_key
 
         while True:
             try:
@@ -117,33 +120,41 @@
             )
 
             self.npcolony.print_printer_base64(printer, data_b64, options=options)
 
             # does some busy waiting for the output file to be created
             # the process handling the PDF printing is asynchronous
             for _ in range(10):
-                if os.path.exists(output_path): break
+                if os.path.exists(output_path):
+                    break
                 time.sleep(0.5)
 
             file = open(output_path, "rb")
             try:
                 data = file.read()
             finally:
                 file.close()
 
-            receivers = [options.get("email_address", self.node_email_address)]
+            # computes the complete list of email receivers using the
+            # base instance value and the ones provided via options
+            email_receivers = list(self.node_email_receivers)
+            email_receiver = options.get("email_receiver", None)
+            if email_receiver:
+                email_receivers += [email_receiver]
+            email_receivers += options.get("email_receivers", [])
+
             logging.info(
                 "Sending email to %s for job '%s' with '%s' printer"
-                % (",".join(receivers), name, printer_s)
+                % (",".join(email_receivers), name, printer_s)
             )
 
             api = mailme.API()
             api.send(
                 mailme.MessagePayload(
-                    receivers=receivers,
+                    receivers=email_receivers,
                     subject="Print job '%s'" % name,
                     attachments=[
                         mailme.AttachmentPayload(
                             name="%s.pdf" % name,
                             data=base64.b64encode(data).decode(),
                             mime="application/pdf",
                         )
```

### Comparing `colony-print-0.3.2/src/colony_print/controllers/printer.py` & `colony-print-0.3.3/src/colony_print/controllers/printer.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/controllers/node.py` & `colony-print-0.3.3/src/colony_print/controllers/node.py`

 * *Files identical despite different names*

### Comparing `colony-print-0.3.2/src/colony_print/controllers/document.py` & `colony-print-0.3.3/src/colony_print/controllers/document.py`

 * *Files identical despite different names*

