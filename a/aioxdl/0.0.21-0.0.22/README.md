# Comparing `tmp/aioxdl-0.0.21.tar.gz` & `tmp/aioxdl-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.21.tar", last modified: Thu May  2 05:44:37 2024, max compression
+gzip compressed data, was "aioxdl-0.0.22.tar", last modified: Thu May  2 07:21:25 2024, max compression
```

## Comparing `aioxdl-0.0.21.tar` & `aioxdl-0.0.22.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.690697 aioxdl-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 05:44:29.000000 aioxdl-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 05:44:37.690697 aioxdl-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-02 05:44:29.000000 aioxdl-0.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.686697 aioxdl-0.0.21/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.690697 aioxdl-0.0.21/aioxdl/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.690697 aioxdl-0.0.21/aioxdl/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/modules/module01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.690697 aioxdl-0.0.21/aioxdl/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 05:44:29.000000 aioxdl-0.0.21/aioxdl/scripts/en.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:44:37.690697 aioxdl-0.0.21/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 05:44:37.000000 aioxdl-0.0.21/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 05:44:37.000000 aioxdl-0.0.21/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 05:44:37.000000 aioxdl-0.0.21/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 05:44:37.000000 aioxdl-0.0.21/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 05:44:37.000000 aioxdl-0.0.21/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 05:44:37.690697 aioxdl-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 05:44:29.000000 aioxdl-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:21:25.317962 aioxdl-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 07:21:18.000000 aioxdl-0.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 07:21:25.317962 aioxdl-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-02 07:21:18.000000 aioxdl-0.0.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:21:25.313962 aioxdl-0.0.22/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 07:21:18.000000 aioxdl-0.0.22/aioxdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:21:25.317962 aioxdl-0.0.22/aioxdl/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 07:21:18.000000 aioxdl-0.0.22/aioxdl/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 07:21:18.000000 aioxdl-0.0.22/aioxdl/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:21:25.317962 aioxdl-0.0.22/aioxdl/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 07:21:18.000000 aioxdl-0.0.22/aioxdl/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-02 07:21:18.000000 aioxdl-0.0.22/aioxdl/modules/module01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:21:25.317962 aioxdl-0.0.22/aioxdl/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 07:21:18.000000 aioxdl-0.0.22/aioxdl/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 07:21:18.000000 aioxdl-0.0.22/aioxdl/scripts/en.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:21:25.317962 aioxdl-0.0.22/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 07:21:25.000000 aioxdl-0.0.22/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 07:21:25.000000 aioxdl-0.0.22/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:21:25.000000 aioxdl-0.0.22/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 07:21:25.000000 aioxdl-0.0.22/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 07:21:25.000000 aioxdl-0.0.22/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 07:21:25.317962 aioxdl-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 07:21:18.000000 aioxdl-0.0.22/setup.py
```

### Comparing `aioxdl-0.0.21/LICENSE` & `aioxdl-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.21/PKG-INFO` & `aioxdl-0.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.21
+Version: 0.0.22
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
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.21 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.22 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
```

### Comparing `aioxdl-0.0.21/README.md` & `aioxdl-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.21/aioxdl/__init__.py` & `aioxdl-0.0.22/aioxdl/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "aioxdl"
-version = "0.0.21"
+version = "0.0.22"
 
 install = ["aiohttp", "yt-dlp"]
 
 contact = "clintonabrahamc@gmail.com"
 
 classis = ['Natural Language :: English',
           'Intended Audience :: Developers',
```

### Comparing `aioxdl-0.0.21/aioxdl/modules/module01.py` & `aioxdl-0.0.22/aioxdl/modules/module01.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 return 200 if response.status == 200 else response.status
 
 #====================================================================================================
 
     async def download(self, url, location, timeout, progress, kwargs):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
-                self.tsize += await self.getsizes(response)
+                self.tsizes += await self.getsizes(response)
                 with open(location, "wb") as handlexo:
                     while True:
                         chunks = await response.content.read(self.chunks)
                         if not chunks:
                             break
                         handlexo.write(chunks)
                         self.dsizes += self.chunks
```

### Comparing `aioxdl-0.0.21/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.22/aioxdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.21
+Version: 0.0.22
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
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.21 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.22 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
```

### Comparing `aioxdl-0.0.21/setup.py` & `aioxdl-0.0.22/setup.py`

 * *Files identical despite different names*

