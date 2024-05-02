# Comparing `tmp/aioxdl-0.0.18.tar.gz` & `tmp/aioxdl-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.18.tar", last modified: Sat Apr 13 08:58:58 2024, max compression
+gzip compressed data, was "aioxdl-0.0.19.tar", last modified: Thu May  2 03:36:46 2024, max compression
```

## Comparing `aioxdl-0.0.18.tar` & `aioxdl-0.0.19.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:58:58.290857 aioxdl-0.0.18/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 08:58:52.000000 aioxdl-0.0.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-13 08:58:58.290857 aioxdl-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-13 08:58:52.000000 aioxdl-0.0.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:58:58.286857 aioxdl-0.0.18/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-13 08:58:52.000000 aioxdl-0.0.18/aioxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-13 08:58:52.000000 aioxdl-0.0.18/aioxdl/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-13 08:58:52.000000 aioxdl-0.0.18/aioxdl/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-13 08:58:52.000000 aioxdl-0.0.18/aioxdl/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:58:58.290857 aioxdl-0.0.18/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-13 08:58:58.000000 aioxdl-0.0.18/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-13 08:58:58.000000 aioxdl-0.0.18/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 08:58:58.000000 aioxdl-0.0.18/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 08:58:58.000000 aioxdl-0.0.18/aioxdl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 08:58:58.000000 aioxdl-0.0.18/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 08:58:58.000000 aioxdl-0.0.18/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 08:58:58.290857 aioxdl-0.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-13 08:58:52.000000 aioxdl-0.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:36:46.342809 aioxdl-0.0.19/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 03:36:40.000000 aioxdl-0.0.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-02 03:36:46.338809 aioxdl-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-02 03:36:40.000000 aioxdl-0.0.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:36:46.338809 aioxdl-0.0.19/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 03:36:40.000000 aioxdl-0.0.19/aioxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-02 03:36:40.000000 aioxdl-0.0.19/aioxdl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-02 03:36:40.000000 aioxdl-0.0.19/aioxdl/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 03:36:40.000000 aioxdl-0.0.19/aioxdl/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:36:46.338809 aioxdl-0.0.19/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-02 03:36:46.000000 aioxdl-0.0.19/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-02 03:36:46.000000 aioxdl-0.0.19/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 03:36:46.000000 aioxdl-0.0.19/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 03:36:46.000000 aioxdl-0.0.19/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 03:36:46.000000 aioxdl-0.0.19/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 03:36:46.342809 aioxdl-0.0.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 03:36:40.000000 aioxdl-0.0.19/setup.py
```

### Comparing `aioxdl-0.0.18/LICENSE` & `aioxdl-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.18/PKG-INFO` & `aioxdl-0.0.19/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.18
+Version: 0.0.19
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: ~=3.9
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: yt-dlp
 
 <p align="center">
     📦 <a href="https://pypi.org/project/aioxdl" style="text-decoration:none;">AIO DOWNLOADER</a>
@@ -43,27 +39,27 @@
 
 ## USAGE
 
 ```python
 import asyncio
 from aioxdl import Downloader
 
-async def progress(_, stime, tsize, dsize):
+async def progress(stime, tsize, dsize):
     # stime = start_time
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
 
 async def main():
     core = Downloader()
     link = "https://example.link/file.txt"
     loca = await core.filename(link)
     file = await core.start(link, loca, progress=progress)
-    fine = file if core.error == None else core.error
+    fine = file if core.errors == None else core.errors
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
```

#### html2text {}

```diff
@@ -1,28 +1,25 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.18 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.19 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
-python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
-:: English Classifier: License :: OSI Approved :: GNU Lesser General Public
-License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: ~=3.9 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: aiohttp Requires-Dist: yt-
-dlp
+python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: License :: OSI
+Approved :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python:
+~=3.10 Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: aiohttp Requires-Dist: yt-dlp
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
-asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
-dsize): # stime = start_time # tsize = total_size # dsize = download_size
-percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
-(percentage), end="", flush=True) async def main(): core = Downloader() link =
-"https://example.link/file.txt" loca = await core.filename(link) file = await
-core.start(link, loca, progress=progress) fine = file if core.error == None
-else core.error print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python
-from aioxdl import Downloader async def main(): core = Downloader() link =
-"https://example.link/file.txt" name = await core.filename(link) print(name)
-asyncio.run(main()) ```
+asyncio from aioxdl import Downloader async def progress(stime, tsize, dsize):
+# stime = start_time # tsize = total_size # dsize = download_size percentage =
+round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format(percentage),
+end="", flush=True) async def main(): core = Downloader() link = "https://
+example.link/file.txt" loca = await core.filename(link) file = await core.start
+(link, loca, progress=progress) fine = file if core.errors == None else
+core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python from
+aioxdl import Downloader async def main(): core = Downloader() link = "https://
+example.link/file.txt" name = await core.filename(link) print(name) asyncio.run
+(main()) ```
```

### Comparing `aioxdl-0.0.18/README.md` & `aioxdl-0.0.19/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 
 ## USAGE
 
 ```python
 import asyncio
 from aioxdl import Downloader
 
-async def progress(_, stime, tsize, dsize):
+async def progress(stime, tsize, dsize):
     # stime = start_time
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
 
 async def main():
     core = Downloader()
     link = "https://example.link/file.txt"
     loca = await core.filename(link)
     file = await core.start(link, loca, progress=progress)
-    fine = file if core.error == None else core.error
+    fine = file if core.errors == None else core.errors
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
-asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
-dsize): # stime = start_time # tsize = total_size # dsize = download_size
-percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
-(percentage), end="", flush=True) async def main(): core = Downloader() link =
-"https://example.link/file.txt" loca = await core.filename(link) file = await
-core.start(link, loca, progress=progress) fine = file if core.error == None
-else core.error print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python
-from aioxdl import Downloader async def main(): core = Downloader() link =
-"https://example.link/file.txt" name = await core.filename(link) print(name)
-asyncio.run(main()) ```
+asyncio from aioxdl import Downloader async def progress(stime, tsize, dsize):
+# stime = start_time # tsize = total_size # dsize = download_size percentage =
+round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format(percentage),
+end="", flush=True) async def main(): core = Downloader() link = "https://
+example.link/file.txt" loca = await core.filename(link) file = await core.start
+(link, loca, progress=progress) fine = file if core.errors == None else
+core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python from
+aioxdl import Downloader async def main(): core = Downloader() link = "https://
+example.link/file.txt" name = await core.filename(link) print(name) asyncio.run
+(main()) ```
```

### Comparing `aioxdl-0.0.18/aioxdl/modules.py` & `aioxdl-0.0.19/aioxdl/modules.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,83 @@
 import time, aiohttp, asyncio
+from aioxdl.functions import Hkeys
 from aioxdl.scripts import Scripted
 from yt_dlp import YoutubeDL, DownloadError
-from aioxdl.functions import Hkeys, EXlogger
-#=================================================================================================
+#====================================================================================================
 
 class Downloader:
 
-    def __init__(self, message=None):
-        self.tsize = 0
-        self.dsize = 0
-        self.error = None
-        self.chunk = 1024
-        self.imssg = message
-        self.stime = time.time()
-        self.etime = Scripted.DATA01
-        self.comnd = {"quiet": True,  "no_warnings": True, "logger": EXlogger()}
-
-#=================================================================================================
+    def __init__(self, **kwargs):
+        self.dsizes = 0
+        self.tsizes = 0
+        self.stimes = time.time()
+        self.comand = Hkeys.DATA01
+        self.fnames = Hkeys.DATA02
+        self.chunks = kwargs.get("chunk", 1024)
+        self.result = kwargs.get("result", None)
+        self.errors = kwargs.get("errors", None)
 
+#====================================================================================================
+    
     async def filename(self, filelink):
-        with YoutubeDL(self.comnd) as ydl:
+        with YoutubeDL(self.comand) as ydl:
             try:
                 resultse = ydl.extract_info(filelink, download=False)
-                filename = ydl.prepare_filename(resultse, outtmpl=Hkeys.DATA01)
+                filename = ydl.prepare_filename(resultse, outtmpl=self.fnames)
             except DownloadError:
-                filename = None
+                filename = Scripted.DATA02
             except Exception:
-                filename = None
+                filename = Scripted.DATA02
 
             return filename
 
-#=================================================================================================
+#====================================================================================================
     
     async def getsizes(self, response):
         return int(response.headers.get("Content-Length", 0)) or 0
 
     async def checkurl(self, url, timeout=20):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
                 return 200 if response.status == 200 else response.status
 
-    async def display(self, progress):
-        await progress(self.imssg, self.stime, self.tsize, self.dsize) if progress else None
-
-#=================================================================================================
+#====================================================================================================
 
-    async def download(self, url, location, timeout, progress):
+    async def download(self, url, location, timeout, progress, kwargs):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
                 self.tsize += await self.getsizes(response)
                 with open(location, "wb") as handlexo:
                     while True:
-                        chunks = await response.content.read(self.chunk)
+                        chunks = await response.content.read(self.chunks)
                         if not chunks:
                             break
                         handlexo.write(chunks)
-                        self.dsize += self.chunk
-                        try: await self.display(progress)
+                        self.dsizes += self.chunks
+                        try: await self.display(progress, kwargs)
                         except ZeroDivisionError: pass
 
                 await response.release()
                 return location if location else None
 
-#=================================================================================================
+#====================================================================================================
 
-    async def start(self, url, flocations, timeout=1000, progress=None):
+    async def start(self, url, flocations, **kwargs):
         try:
-            flocations = await self.download(url, flocations, timeout, progress)
+            timeouts = kwargs.get("timeout", 1000)
+            progress = kwargs.get("progress", None)
+            flocations = await self.download(url, flocations, timeouts, progress, kwargs)
         except aiohttp.ClientConnectorError as errors:
-            self.error = errors
+            self.errors = errors
         except asyncio.TimeoutError:
-            self.error = self.etime
+            self.errors = Scripted.DATA01
         except Exception as errors:
-            self.error = errors
+            self.errors = errors
 
         return flocations
 
-#=================================================================================================
-                       
+#====================================================================================================
+
+    async def display(self, progress, kwargs):
+        await progress(self.stimes, self.tsizes, self.dsizes, kwargs) if progress else None
+
+#====================================================================================================
```

### Comparing `aioxdl-0.0.18/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.19/aioxdl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.18
+Version: 0.0.19
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: ~=3.9
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: yt-dlp
 
 <p align="center">
     📦 <a href="https://pypi.org/project/aioxdl" style="text-decoration:none;">AIO DOWNLOADER</a>
@@ -43,27 +39,27 @@
 
 ## USAGE
 
 ```python
 import asyncio
 from aioxdl import Downloader
 
-async def progress(_, stime, tsize, dsize):
+async def progress(stime, tsize, dsize):
     # stime = start_time
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("\rCOMPLETED : {}%".format(percentage), end="", flush=True)
 
 async def main():
     core = Downloader()
     link = "https://example.link/file.txt"
     loca = await core.filename(link)
     file = await core.start(link, loca, progress=progress)
-    fine = file if core.error == None else core.error
+    fine = file if core.errors == None else core.errors
     print(fine)
 
 asyncio.run(main())
 ```
 
 ## GET FILENAME
 ```python
```

#### html2text {}

```diff
@@ -1,28 +1,25 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.18 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.19 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
-python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
-:: English Classifier: License :: OSI Approved :: GNU Lesser General Public
-License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: ~=3.9 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: aiohttp Requires-Dist: yt-
-dlp
+python,downloader,aiohttp Classifier: Natural Language :: English Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: License :: OSI
+Approved :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python:
+~=3.10 Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: aiohttp Requires-Dist: yt-dlp
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
-asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
-dsize): # stime = start_time # tsize = total_size # dsize = download_size
-percentage = round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format
-(percentage), end="", flush=True) async def main(): core = Downloader() link =
-"https://example.link/file.txt" loca = await core.filename(link) file = await
-core.start(link, loca, progress=progress) fine = file if core.error == None
-else core.error print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python
-from aioxdl import Downloader async def main(): core = Downloader() link =
-"https://example.link/file.txt" name = await core.filename(link) print(name)
-asyncio.run(main()) ```
+asyncio from aioxdl import Downloader async def progress(stime, tsize, dsize):
+# stime = start_time # tsize = total_size # dsize = download_size percentage =
+round((dsize / tsize) * 100, 2) print("\rCOMPLETED : {}%".format(percentage),
+end="", flush=True) async def main(): core = Downloader() link = "https://
+example.link/file.txt" loca = await core.filename(link) file = await core.start
+(link, loca, progress=progress) fine = file if core.errors == None else
+core.errors print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python from
+aioxdl import Downloader async def main(): core = Downloader() link = "https://
+example.link/file.txt" name = await core.filename(link) print(name) asyncio.run
+(main()) ```
```

