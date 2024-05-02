# Comparing `tmp/aioxdl-0.0.23.tar.gz` & `tmp/aioxdl-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.23.tar", last modified: Thu May  2 07:36:24 2024, max compression
+gzip compressed data, was "aioxdl-0.0.24.tar", last modified: Thu May  2 18:10:18 2024, max compression
```

## Comparing `aioxdl-0.0.23.tar` & `aioxdl-0.0.24.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:36:24.106531 aioxdl-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 07:36:18.000000 aioxdl-0.0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 07:36:24.106531 aioxdl-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-02 07:36:18.000000 aioxdl-0.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:36:24.102530 aioxdl-0.0.23/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 07:36:18.000000 aioxdl-0.0.23/aioxdl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:36:24.106531 aioxdl-0.0.23/aioxdl/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 07:36:18.000000 aioxdl-0.0.23/aioxdl/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 07:36:18.000000 aioxdl-0.0.23/aioxdl/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:36:24.106531 aioxdl-0.0.23/aioxdl/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 07:36:18.000000 aioxdl-0.0.23/aioxdl/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-02 07:36:18.000000 aioxdl-0.0.23/aioxdl/modules/module01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:36:24.106531 aioxdl-0.0.23/aioxdl/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 07:36:18.000000 aioxdl-0.0.23/aioxdl/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 07:36:18.000000 aioxdl-0.0.23/aioxdl/scripts/en.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:36:24.106531 aioxdl-0.0.23/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-02 07:36:24.000000 aioxdl-0.0.23/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 07:36:24.000000 aioxdl-0.0.23/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:36:24.000000 aioxdl-0.0.23/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 07:36:24.000000 aioxdl-0.0.23/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 07:36:24.000000 aioxdl-0.0.23/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 07:36:24.106531 aioxdl-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 07:36:18.000000 aioxdl-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.792386 aioxdl-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 18:10:08.000000 aioxdl-0.0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-02 18:10:18.788386 aioxdl-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-02 18:10:08.000000 aioxdl-0.0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.788386 aioxdl-0.0.24/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.788386 aioxdl-0.0.24/aioxdl/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.788386 aioxdl-0.0.24/aioxdl/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/modules/module01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.788386 aioxdl-0.0.24/aioxdl/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 18:10:08.000000 aioxdl-0.0.24/aioxdl/scripts/en.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:10:18.788386 aioxdl-0.0.24/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-02 18:10:18.000000 aioxdl-0.0.24/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 18:10:18.000000 aioxdl-0.0.24/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:10:18.000000 aioxdl-0.0.24/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 18:10:18.000000 aioxdl-0.0.24/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 18:10:18.000000 aioxdl-0.0.24/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:10:18.792386 aioxdl-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 18:10:08.000000 aioxdl-0.0.24/setup.py
```

### Comparing `aioxdl-0.0.23/LICENSE` & `aioxdl-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.23/PKG-INFO` & `aioxdl-0.0.24/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.23
+Version: 0.0.24
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Natural Language :: English
@@ -37,40 +37,40 @@
 pip install aioxdl
 ```
 
 ## USAGE
 
 ```python
 import asyncio
-from aioxdl.modules import Downloader
+from aioxdl.modules import Aioxdl
 
 async def progress(stime, tsize, dsize):
     # stime = start_time
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
 
 async def main():
-    core = Downloader()
+    core = Aioxdl(timeout=2000)
     link = "https://example.link/file.txt"
     loca = await core.filename(link)
     file = await core.start(link, loca, progress=progress)
     fine = file if core.errors == None else core.errors
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
-from aioxdl.modules import Downloader
+from aioxdl.modules import Aioxdl
 
 async def main():
-    core = Downloader()
+    core = Aioxdl()
     link = "https://example.link/file.txt"
     name = await core.filename(link)
     print(name)
 
 asyncio.run(main())
 ```
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.23 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.24 Summary: Python fast
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
-asyncio from aioxdl.modules import Downloader async def progress(stime, tsize,
+asyncio from aioxdl.modules import Aioxdl async def progress(stime, tsize,
 dsize): # stime = start_time # tsize = total_size # dsize = download_size
 percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
-(percentage), end="", flush=True) async def main(): core = Downloader() link =
-"https://example.link/file.txt" loca = await core.filename(link) file = await
-core.start(link, loca, progress=progress) fine = file if core.errors == None
-else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python
-from aioxdl.modules import Downloader async def main(): core = Downloader()
+(percentage), end="", flush=True) async def main(): core = Aioxdl(timeout=2000)
+link = "https://example.link/file.txt" loca = await core.filename(link) file =
+await core.start(link, loca, progress=progress) fine = file if core.errors ==
+None else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME
+```python from aioxdl.modules import Aioxdl async def main(): core = Aioxdl()
 link = "https://example.link/file.txt" name = await core.filename(link) print
 (name) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.23/README.md` & `aioxdl-0.0.24/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -13,40 +13,40 @@
 pip install aioxdl
 ```
 
 ## USAGE
 
 ```python
 import asyncio
-from aioxdl.modules import Downloader
+from aioxdl.modules import Aioxdl
 
 async def progress(stime, tsize, dsize):
     # stime = start_time
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
 
 async def main():
-    core = Downloader()
+    core = Aioxdl(timeout=2000)
     link = "https://example.link/file.txt"
     loca = await core.filename(link)
     file = await core.start(link, loca, progress=progress)
     fine = file if core.errors == None else core.errors
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
-from aioxdl.modules import Downloader
+from aioxdl.modules import Aioxdl
 
 async def main():
-    core = Downloader()
+    core = Aioxdl()
     link = "https://example.link/file.txt"
     name = await core.filename(link)
     print(name)
 
 asyncio.run(main())
 ```
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
-asyncio from aioxdl.modules import Downloader async def progress(stime, tsize,
+asyncio from aioxdl.modules import Aioxdl async def progress(stime, tsize,
 dsize): # stime = start_time # tsize = total_size # dsize = download_size
 percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
-(percentage), end="", flush=True) async def main(): core = Downloader() link =
-"https://example.link/file.txt" loca = await core.filename(link) file = await
-core.start(link, loca, progress=progress) fine = file if core.errors == None
-else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python
-from aioxdl.modules import Downloader async def main(): core = Downloader()
+(percentage), end="", flush=True) async def main(): core = Aioxdl(timeout=2000)
+link = "https://example.link/file.txt" loca = await core.filename(link) file =
+await core.start(link, loca, progress=progress) fine = file if core.errors ==
+None else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME
+```python from aioxdl.modules import Aioxdl async def main(): core = Aioxdl()
 link = "https://example.link/file.txt" name = await core.filename(link) print
 (name) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.23/aioxdl/__init__.py` & `aioxdl-0.0.24/aioxdl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "aioxdl"
-version = "0.0.23"
+version = "0.0.24"
 
 install = ["aiohttp", "yt-dlp"]
 
 contact = "clintonabrahamc@gmail.com"
 
 classis = ['Natural Language :: English',
           'Intended Audience :: Developers',
```

### Comparing `aioxdl-0.0.23/aioxdl/modules/module01.py` & `aioxdl-0.0.24/aioxdl/modules/module01.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,80 @@
 import time, aiohttp, asyncio
 from ..functions import Hkeys
 from ..scripts import Scripted
 from yt_dlp import YoutubeDL, DownloadError
-#====================================================================================================
+#=========================================================================================================
 
-class Downloader:
+class Aioxdl:
 
     def __init__(self, **kwargs):
         self.dsizes = 0
         self.tsizes = 0
         self.stimes = time.time()
         self.comand = Hkeys.DATA01
         self.fnames = Hkeys.DATA02
         self.chunks = kwargs.get("chunk", 1024)
-        self.result = kwargs.get("result", None)
         self.errors = kwargs.get("errors", None)
+        self.otimes = kwargs.get("timeout", 1000)
 
-#====================================================================================================
-    
-    async def filename(self, filelink):
-        with YoutubeDL(self.comand) as ydl:
-            try:
-                resultse = ydl.extract_info(filelink, download=False)
-                filename = ydl.prepare_filename(resultse, outtmpl=self.fnames)
-            except DownloadError:
-                filename = Scripted.DATA02
-            except Exception:
-                filename = Scripted.DATA02
+#=========================================================================================================
 
-            return filename
-
-#====================================================================================================
-    
-    async def getsizes(self, response):
-        return int(response.headers.get("Content-Length", 0)) or 0
-
-    async def checkurl(self, url, timeout=20):
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url, timeout=timeout) as response:
-                return 200 if response.status == 200 else response.status
-
-#====================================================================================================
-
-    async def download(self, url, location, timeout, progress, **kwargs):
+    async def download(self, url, location, timeout, progress, kwargs):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
                 self.tsizes += await self.getsizes(response)
                 with open(location, "wb") as handlexo:
                     while True:
                         chunks = await response.content.read(self.chunks)
                         if not chunks:
                             break
                         handlexo.write(chunks)
                         self.dsizes += self.chunks
-                        try: await self.display(progress, **kwargs)
+                        try: await self.display(progress, kwargs)
                         except ZeroDivisionError: pass
 
                 await response.release()
                 return location if location else None
 
-#====================================================================================================
+#=========================================================================================================
 
-    async def start(self, url, flocations, **kwargs):
+    async def filename(self, filelink):
+        with YoutubeDL(self.comand) as ydl:
+            try:
+                resultse = ydl.extract_info(filelink, download=False)
+                filename = ydl.prepare_filename(resultse, outtmpl=self.fnames)
+            except DownloadError:
+                filename = Scripted.DATA02
+            except Exception:
+                filename = Scripted.DATA02
+
+            return filename
+
+#=========================================================================================================
+
+    async def getsizes(self, response):
+        return int(response.headers.get("Content-Length", 0))
+
+#=========================================================================================================
+
+    async def display(self, progress, kwargs):
+        if progress and kwargs:
+            await progress(self.stimes, self.tsizes, self.dsizes, kwargs)
+        elif progress:
+            await progress(self.stimes, self.tsizes, self.dsizes)
+        else: pass
+
+#=========================================================================================================
+
+    async def start(self, url, location, progress=None, **kwargs):
         try:
-            timeouts = kwargs.get("timeout", 1000)
-            progress = kwargs.get("progress", None)
-            flocations = await self.download(url, flocations, timeouts, progress, **kwargs)
+            location = await self.download(url, location, self.otimes, cancelid, progress, kwargs)
         except aiohttp.ClientConnectorError as errors:
             self.errors = errors
         except asyncio.TimeoutError:
             self.errors = Scripted.DATA01
         except Exception as errors:
             self.errors = errors
 
-        return flocations
-
-#====================================================================================================
-
-    async def display(self, progress, **kwargs):
-        await progress(self.stimes, self.tsizes, self.dsizes, **kwargs) if progress else None
+        return location
 
-#====================================================================================================
+#=========================================================================================================
```

### Comparing `aioxdl-0.0.23/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.24/aioxdl.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.23
+Version: 0.0.24
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Natural Language :: English
@@ -37,40 +37,40 @@
 pip install aioxdl
 ```
 
 ## USAGE
 
 ```python
 import asyncio
-from aioxdl.modules import Downloader
+from aioxdl.modules import Aioxdl
 
 async def progress(stime, tsize, dsize):
     # stime = start_time
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
 
 async def main():
-    core = Downloader()
+    core = Aioxdl(timeout=2000)
     link = "https://example.link/file.txt"
     loca = await core.filename(link)
     file = await core.start(link, loca, progress=progress)
     fine = file if core.errors == None else core.errors
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
-from aioxdl.modules import Downloader
+from aioxdl.modules import Aioxdl
 
 async def main():
-    core = Downloader()
+    core = Aioxdl()
     link = "https://example.link/file.txt"
     name = await core.filename(link)
     print(name)
 
 asyncio.run(main())
 ```
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.23 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.24 Summary: Python fast
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
-asyncio from aioxdl.modules import Downloader async def progress(stime, tsize,
+asyncio from aioxdl.modules import Aioxdl async def progress(stime, tsize,
 dsize): # stime = start_time # tsize = total_size # dsize = download_size
 percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
-(percentage), end="", flush=True) async def main(): core = Downloader() link =
-"https://example.link/file.txt" loca = await core.filename(link) file = await
-core.start(link, loca, progress=progress) fine = file if core.errors == None
-else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python
-from aioxdl.modules import Downloader async def main(): core = Downloader()
+(percentage), end="", flush=True) async def main(): core = Aioxdl(timeout=2000)
+link = "https://example.link/file.txt" loca = await core.filename(link) file =
+await core.start(link, loca, progress=progress) fine = file if core.errors ==
+None else core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME
+```python from aioxdl.modules import Aioxdl async def main(): core = Aioxdl()
 link = "https://example.link/file.txt" name = await core.filename(link) print
 (name) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.23/setup.py` & `aioxdl-0.0.24/setup.py`

 * *Files identical despite different names*

