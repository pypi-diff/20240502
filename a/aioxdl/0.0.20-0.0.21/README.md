# Comparing `tmp/aioxdl-0.0.20.tar.gz` & `tmp/aioxdl-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.20.tar", last modified: Thu May  2 04:44:27 2024, max compression
+gzip compressed data, was "aioxdl-0.0.21.tar", last modified: Thu May  2 05:44:37 2024, max compression
```

## Comparing `aioxdl-0.0.20.tar` & `aioxdl-0.0.21.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.220153 aioxdl-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 04:44:21.000000 aioxdl-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 04:44:27.220153 aioxdl-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-02 04:44:21.000000 aioxdl-0.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.216153 aioxdl-0.0.20/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.216153 aioxdl-0.0.20/aioxdl/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.216153 aioxdl-0.0.20/aioxdl/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/modules/module01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.220153 aioxdl-0.0.20/aioxdl/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/scripts/en.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.220153 aioxdl-0.0.20/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 04:44:27.000000 aioxdl-0.0.20/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 04:44:27.000000 aioxdl-0.0.20/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 04:44:27.000000 aioxdl-0.0.20/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 04:44:27.000000 aioxdl-0.0.20/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 04:44:27.000000 aioxdl-0.0.20/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 04:44:27.220153 aioxdl-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 04:44:21.000000 aioxdl-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.690697 aioxdl-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 05:44:29.000000 aioxdl-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 05:44:37.690697 aioxdl-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-02 05:44:29.000000 aioxdl-0.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.686697 aioxdl-0.0.21/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.690697 aioxdl-0.0.21/aioxdl/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.690697 aioxdl-0.0.21/aioxdl/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/modules/module01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.690697 aioxdl-0.0.21/aioxdl/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/scripts/en.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.690697 aioxdl-0.0.21/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 05:44:37.000000 aioxdl-0.0.21/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 05:44:37.000000 aioxdl-0.0.21/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 05:44:37.000000 aioxdl-0.0.21/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 05:44:37.000000 aioxdl-0.0.21/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 05:44:37.000000 aioxdl-0.0.21/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 05:44:37.690697 aioxdl-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 05:44:29.000000 aioxdl-0.0.21/setup.py
```

### Comparing `aioxdl-0.0.20/LICENSE` & `aioxdl-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.20/PKG-INFO` & `aioxdl-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.20
+Version: 0.0.21
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.20 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.21 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
```

### Comparing `aioxdl-0.0.20/README.md` & `aioxdl-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.20/aioxdl/__init__.py` & `aioxdl-0.0.21/aioxdl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "aioxdl"
-version = "0.0.20"
+version = "0.0.21"
 
 install = ["aiohttp", "yt-dlp"]
 
 contact = "clintonabrahamc@gmail.com"
 
 classis = ['Natural Language :: English',
           'Intended Audience :: Developers',
```

### Comparing `aioxdl-0.0.20/aioxdl/modules/module01.py` & `aioxdl-0.0.21/aioxdl/modules/module01.py`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.20/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.21/aioxdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.20
+Version: 0.0.21
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.20 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.21 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
```

### Comparing `aioxdl-0.0.20/setup.py` & `aioxdl-0.0.21/setup.py`

 * *Files identical despite different names*

