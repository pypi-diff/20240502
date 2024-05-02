# Comparing `tmp/aioxdl-0.0.24.tar.gz` & `tmp/aioxdl-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.24.tar", last modified: Thu May  2 18:10:18 2024, max compression
+gzip compressed data, was "aioxdl-0.0.25.tar", last modified: Thu May  2 18:16:06 2024, max compression
```

## Comparing `aioxdl-0.0.24.tar` & `aioxdl-0.0.25.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.792386 aioxdl-0.0.24/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 18:10:08.000000 aioxdl-0.0.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-02 18:10:18.788386 aioxdl-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-02 18:10:08.000000 aioxdl-0.0.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.788386 aioxdl-0.0.24/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.788386 aioxdl-0.0.24/aioxdl/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.788386 aioxdl-0.0.24/aioxdl/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/modules/module01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.788386 aioxdl-0.0.24/aioxdl/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/scripts/en.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.788386 aioxdl-0.0.24/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-02 18:10:18.000000 aioxdl-0.0.24/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 18:10:18.000000 aioxdl-0.0.24/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:10:18.000000 aioxdl-0.0.24/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 18:10:18.000000 aioxdl-0.0.24/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 18:10:18.000000 aioxdl-0.0.24/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:10:18.792386 aioxdl-0.0.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 18:10:08.000000 aioxdl-0.0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:16:06.849547 aioxdl-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 18:15:59.000000 aioxdl-0.0.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-02 18:16:06.849547 aioxdl-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-02 18:15:59.000000 aioxdl-0.0.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:16:06.845546 aioxdl-0.0.25/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 18:15:59.000000 aioxdl-0.0.25/aioxdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:16:06.849547 aioxdl-0.0.25/aioxdl/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 18:15:59.000000 aioxdl-0.0.25/aioxdl/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 18:15:59.000000 aioxdl-0.0.25/aioxdl/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:16:06.849547 aioxdl-0.0.25/aioxdl/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 18:15:59.000000 aioxdl-0.0.25/aioxdl/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-02 18:15:59.000000 aioxdl-0.0.25/aioxdl/modules/module01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:16:06.849547 aioxdl-0.0.25/aioxdl/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 18:15:59.000000 aioxdl-0.0.25/aioxdl/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 18:15:59.000000 aioxdl-0.0.25/aioxdl/scripts/en.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:16:06.849547 aioxdl-0.0.25/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-02 18:16:06.000000 aioxdl-0.0.25/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 18:16:06.000000 aioxdl-0.0.25/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:16:06.000000 aioxdl-0.0.25/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 18:16:06.000000 aioxdl-0.0.25/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 18:16:06.000000 aioxdl-0.0.25/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:16:06.849547 aioxdl-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 18:15:59.000000 aioxdl-0.0.25/setup.py
```

### Comparing `aioxdl-0.0.24/LICENSE` & `aioxdl-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.24/PKG-INFO` & `aioxdl-0.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.24
+Version: 0.0.25
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
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.24 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.25 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
```

### Comparing `aioxdl-0.0.24/README.md` & `aioxdl-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.24/aioxdl/__init__.py` & `aioxdl-0.0.25/aioxdl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "aioxdl"
-version = "0.0.24"
+version = "0.0.25"
 
 install = ["aiohttp", "yt-dlp"]
 
 contact = "clintonabrahamc@gmail.com"
 
 classis = ['Natural Language :: English',
           'Intended Audience :: Developers',
```

### Comparing `aioxdl-0.0.24/aioxdl/modules/module01.py` & `aioxdl-0.0.25/aioxdl/modules/module01.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             await progress(self.stimes, self.tsizes, self.dsizes)
         else: pass
 
 #=========================================================================================================
 
     async def start(self, url, location, progress=None, **kwargs):
         try:
-            location = await self.download(url, location, self.otimes, cancelid, progress, kwargs)
+            location = await self.download(url, location, self.otimes, progress, kwargs)
         except aiohttp.ClientConnectorError as errors:
             self.errors = errors
         except asyncio.TimeoutError:
             self.errors = Scripted.DATA01
         except Exception as errors:
             self.errors = errors
```

### Comparing `aioxdl-0.0.24/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.25/aioxdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.24
+Version: 0.0.25
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
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.24 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.25 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
```

### Comparing `aioxdl-0.0.24/setup.py` & `aioxdl-0.0.25/setup.py`

 * *Files identical despite different names*

