# Comparing `tmp/aioxdl-0.0.19.tar.gz` & `tmp/aioxdl-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.19.tar", last modified: Thu May  2 03:36:46 2024, max compression
+gzip compressed data, was "aioxdl-0.0.20.tar", last modified: Thu May  2 04:44:27 2024, max compression
```

## Comparing `aioxdl-0.0.19.tar` & `aioxdl-0.0.20.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:36:46.342809 aioxdl-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 03:36:40.000000 aioxdl-0.0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-02 03:36:46.338809 aioxdl-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-02 03:36:40.000000 aioxdl-0.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:36:46.338809 aioxdl-0.0.19/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 03:36:40.000000 aioxdl-0.0.19/aioxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-02 03:36:40.000000 aioxdl-0.0.19/aioxdl/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-02 03:36:40.000000 aioxdl-0.0.19/aioxdl/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 03:36:40.000000 aioxdl-0.0.19/aioxdl/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:36:46.338809 aioxdl-0.0.19/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-02 03:36:46.000000 aioxdl-0.0.19/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-02 03:36:46.000000 aioxdl-0.0.19/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 03:36:46.000000 aioxdl-0.0.19/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 03:36:46.000000 aioxdl-0.0.19/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 03:36:46.000000 aioxdl-0.0.19/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 03:36:46.342809 aioxdl-0.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 03:36:40.000000 aioxdl-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.220153 aioxdl-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 04:44:21.000000 aioxdl-0.0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 04:44:27.220153 aioxdl-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-02 04:44:21.000000 aioxdl-0.0.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.216153 aioxdl-0.0.20/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.216153 aioxdl-0.0.20/aioxdl/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.216153 aioxdl-0.0.20/aioxdl/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/modules/module01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.220153 aioxdl-0.0.20/aioxdl/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 04:44:21.000000 aioxdl-0.0.20/aioxdl/scripts/en.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 04:44:27.220153 aioxdl-0.0.20/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 04:44:27.000000 aioxdl-0.0.20/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 04:44:27.000000 aioxdl-0.0.20/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 04:44:27.000000 aioxdl-0.0.20/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 04:44:27.000000 aioxdl-0.0.20/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 04:44:27.000000 aioxdl-0.0.20/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 04:44:27.220153 aioxdl-0.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 04:44:21.000000 aioxdl-0.0.20/setup.py
```

### Comparing `aioxdl-0.0.19/LICENSE` & `aioxdl-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.19/PKG-INFO` & `aioxdl-0.0.20/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.19
+Version: 0.0.20
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Natural Language :: English
@@ -37,15 +37,15 @@
 pip install aioxdl
 ```
 
 ## USAGE
 
 ```python
 import asyncio
-from aioxdl import Downloader
+from aioxdl.modules import Downloader
 
 async def progress(stime, tsize, dsize):
     # stime = start_time
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
@@ -59,15 +59,15 @@
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
-from aioxdl import Downloader
+from aioxdl.modules import Downloader
 
 async def main():
     core = Downloader()
     link = "https://example.link/file.txt"
     name = await core.filename(link)
     print(name)
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.19 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.20 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: License :: OSI
 Approved :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python:
 ~=3.10 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: aiohttp Requires-Dist: yt-dlp
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
-asyncio from aioxdl import Downloader async def progress(stime, tsize, dsize):
-# stime = start_time # tsize = total_size # dsize = download_size percentage =
-round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format(percentage),
-end="", flush=True) async def main(): core = Downloader() link = "https://
-example.link/file.txt" loca = await core.filename(link) file = await core.start
-(link, loca, progress=progress) fine = file if core.errors == None else
-core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python from
-aioxdl import Downloader async def main(): core = Downloader() link = "https://
-example.link/file.txt" name = await core.filename(link) print(name) asyncio.run
-(main()) ```
+asyncio from aioxdl.modules import Downloader async def progress(stime, tsize,
+dsize): # stime = start_time # tsize = total_size # dsize = download_size
+percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
+(percentage), end="", flush=True) async def main(): core = Downloader() link =
+"https://example.link/file.txt" loca = await core.filename(link) file = await
+core.start(link, loca, progress=progress) fine = file if core.errors == None
+else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python
+from aioxdl.modules import Downloader async def main(): core = Downloader()
+link = "https://example.link/file.txt" name = await core.filename(link) print
+(name) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.19/README.md` & `aioxdl-0.0.20/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 pip install aioxdl
 ```
 
 ## USAGE
 
 ```python
 import asyncio
-from aioxdl import Downloader
+from aioxdl.modules import Downloader
 
 async def progress(stime, tsize, dsize):
     # stime = start_time
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
@@ -35,15 +35,15 @@
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
-from aioxdl import Downloader
+from aioxdl.modules import Downloader
 
 async def main():
     core = Downloader()
     link = "https://example.link/file.txt"
     name = await core.filename(link)
     print(name)
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
-asyncio from aioxdl import Downloader async def progress(stime, tsize, dsize):
-# stime = start_time # tsize = total_size # dsize = download_size percentage =
-round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format(percentage),
-end="", flush=True) async def main(): core = Downloader() link = "https://
-example.link/file.txt" loca = await core.filename(link) file = await core.start
-(link, loca, progress=progress) fine = file if core.errors == None else
-core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python from
-aioxdl import Downloader async def main(): core = Downloader() link = "https://
-example.link/file.txt" name = await core.filename(link) print(name) asyncio.run
-(main()) ```
+asyncio from aioxdl.modules import Downloader async def progress(stime, tsize,
+dsize): # stime = start_time # tsize = total_size # dsize = download_size
+percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
+(percentage), end="", flush=True) async def main(): core = Downloader() link =
+"https://example.link/file.txt" loca = await core.filename(link) file = await
+core.start(link, loca, progress=progress) fine = file if core.errors == None
+else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python
+from aioxdl.modules import Downloader async def main(): core = Downloader()
+link = "https://example.link/file.txt" name = await core.filename(link) print
+(name) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.19/aioxdl/__init__.py` & `aioxdl-0.0.20/aioxdl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "aioxdl"
-version = "0.0.19"
+version = "0.0.20"
 
 install = ["aiohttp", "yt-dlp"]
 
 contact = "clintonabrahamc@gmail.com"
 
 classis = ['Natural Language :: English',
           'Intended Audience :: Developers',
```

### Comparing `aioxdl-0.0.19/aioxdl/modules.py` & `aioxdl-0.0.20/aioxdl/modules/module01.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time, aiohttp, asyncio
-from aioxdl.functions import Hkeys
-from aioxdl.scripts import Scripted
+from ..functions import Hkeys
+from ..scripts import Scripted
 from yt_dlp import YoutubeDL, DownloadError
 #====================================================================================================
 
 class Downloader:
 
     def __init__(self, **kwargs):
         self.dsizes = 0
```

### Comparing `aioxdl-0.0.19/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.20/aioxdl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.19
+Version: 0.0.20
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Natural Language :: English
@@ -37,15 +37,15 @@
 pip install aioxdl
 ```
 
 ## USAGE
 
 ```python
 import asyncio
-from aioxdl import Downloader
+from aioxdl.modules import Downloader
 
 async def progress(stime, tsize, dsize):
     # stime = start_time
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
@@ -59,15 +59,15 @@
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
-from aioxdl import Downloader
+from aioxdl.modules import Downloader
 
 async def main():
     core = Downloader()
     link = "https://example.link/file.txt"
     name = await core.filename(link)
     print(name)
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.19 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.20 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: License :: OSI
 Approved :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python:
 ~=3.10 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: aiohttp Requires-Dist: yt-dlp
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
-asyncio from aioxdl import Downloader async def progress(stime, tsize, dsize):
-# stime = start_time # tsize = total_size # dsize = download_size percentage =
-round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format(percentage),
-end="", flush=True) async def main(): core = Downloader() link = "https://
-example.link/file.txt" loca = await core.filename(link) file = await core.start
-(link, loca, progress=progress) fine = file if core.errors == None else
-core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python from
-aioxdl import Downloader async def main(): core = Downloader() link = "https://
-example.link/file.txt" name = await core.filename(link) print(name) asyncio.run
-(main()) ```
+asyncio from aioxdl.modules import Downloader async def progress(stime, tsize,
+dsize): # stime = start_time # tsize = total_size # dsize = download_size
+percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
+(percentage), end="", flush=True) async def main(): core = Downloader() link =
+"https://example.link/file.txt" loca = await core.filename(link) file = await
+core.start(link, loca, progress=progress) fine = file if core.errors == None
+else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python
+from aioxdl.modules import Downloader async def main(): core = Downloader()
+link = "https://example.link/file.txt" name = await core.filename(link) print
+(name) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.19/setup.py` & `aioxdl-0.0.20/setup.py`

 * *Files identical despite different names*

