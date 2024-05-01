# Comparing `tmp/pm2-0.0.4.1.tar.gz` & `tmp/pm2-0.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm2-0.0.4.1.tar", last modified: Wed May  1 14:20:00 2024, max compression
+gzip compressed data, was "pm2-0.0.4.2.tar", last modified: Wed May  1 18:20:56 2024, max compression
```

## Comparing `pm2-0.0.4.1.tar` & `pm2-0.0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 14:20:00.008778 pm2-0.0.4.1/
--rw-rw-rw-   0        0        0    35803 2024-04-30 09:18:53.000000 pm2-0.0.4.1/LICENSE
--rw-rw-rw-   0        0        0     4842 2024-05-01 14:19:59.905794 pm2-0.0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3318 2024-04-30 09:18:53.000000 pm2-0.0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 14:19:59.718485 pm2-0.0.4.1/pm2/
--rw-rw-rw-   0        0        0    10004 2024-05-01 14:19:13.000000 pm2-0.0.4.1/pm2/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-30 09:18:53.000000 pm2-0.0.4.1/pm2/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 14:19:59.889637 pm2-0.0.4.1/pm2.egg-info/
--rw-rw-rw-   0        0        0     4842 2024-05-01 14:19:58.000000 pm2-0.0.4.1/pm2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-01 14:19:59.000000 pm2-0.0.4.1/pm2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 14:19:58.000000 pm2-0.0.4.1/pm2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-01 14:19:58.000000 pm2-0.0.4.1/pm2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2024-05-01 14:19:58.000000 pm2-0.0.4.1/pm2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-01 14:19:58.000000 pm2-0.0.4.1/pm2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 14:20:00.030134 pm2-0.0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2052 2024-04-30 09:22:44.000000 pm2-0.0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 18:20:56.493099 pm2-0.0.4.2/
+-rw-rw-rw-   0        0        0    35803 2024-04-30 09:18:53.000000 pm2-0.0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     4842 2024-05-01 18:20:56.412107 pm2-0.0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3318 2024-04-30 09:18:53.000000 pm2-0.0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 18:20:56.293089 pm2-0.0.4.2/pm2/
+-rw-rw-rw-   0        0        0    10340 2024-05-01 18:20:48.000000 pm2-0.0.4.2/pm2/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 09:18:53.000000 pm2-0.0.4.2/pm2/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 18:20:56.403092 pm2-0.0.4.2/pm2.egg-info/
+-rw-rw-rw-   0        0        0     4842 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       22 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 18:20:56.494097 pm2-0.0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     2052 2024-04-30 09:22:44.000000 pm2-0.0.4.2/setup.py
```

### Comparing `pm2-0.0.4.1/LICENSE` & `pm2-0.0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pm2-0.0.4.1/PKG-INFO` & `pm2-0.0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm2
-Version: 0.0.4.1
+Version: 0.0.4.2
 Summary: Python wrapper for PM2
 Home-page: https://github.com/y4kupkaya/pm2
 Author: y4kupkaya
 Author-email: contact@yakupkaya.net.tr
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Keywords: process-manager,pm2,pm2-py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pm2-0.0.4.1/README.md` & `pm2-0.0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pm2-0.0.4.1/pm2/__init__.py` & `pm2-0.0.4.2/pm2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from typing import Any, List, Optional
 
 import aiofiles
 from aylak.rich.console import Console
 
 console = Console()
 
-__version__ = "0.0.4.1"
+__version__ = "0.0.4.2"
 
 
 class PathIsFolderError(Exception):
     pass
 
 
 class PM2Process:
@@ -189,22 +189,32 @@
 
     async def logs(
         self,
         lines: int = 500,
         pid: int = None,
         pm_id: int = None,
         name: str = None,
-        errors: bool = False,
+        out_log: bool = True,
+        err_log: bool = False,
     ) -> str:
         process = await self.get(pid=pid, pm_id=pm_id, name=name)
-        async with aiofiles.open(process.out_log, "r", encoding="utf-8") as f:
-            out_log = "\n".join(await f.readlines()[-lines:])
-        async with aiofiles.open(process.err_log, "r", encoding="utf-8") as f:
-            err_log = "\n".join(await f.readlines()[-lines:])
-        return (out_log, err_log) if errors else out_log
+        if not process:
+            return None, None
+
+        out_log, err_log = "", ""
+
+        if out_log:
+            async with aiofiles.open(process.out_log, "r", encoding="utf-8") as f:
+                out_log += "\n".join(await f.readlines()[-lines:])
+
+        if err_log:
+            async with aiofiles.open(process.err_log, "r", encoding="utf-8") as f:
+                err_log += "\n".join(await f.readlines()[-lines:])
+
+        return (out_log, err_log)
 
 
 # sync PM2
 class PM2:
     def __init__(self, command_path: str = "pm2") -> None:
         self.COMMAND = [command_path]
         pass
@@ -281,15 +291,25 @@
 
     def logs(
         self,
         lines: int = 500,
         pid: int = None,
         pm_id: int = None,
         name: str = None,
-        errors: bool = False,
+        out_log: bool = True,
+        err_log: bool = False,
     ) -> str:
         process = self.get(pid=pid, pm_id=pm_id, name=name)
-        with open(process.out_log, "r", encoding="utf-8") as f:
-            out_log = "\n".join(f.readlines()[-lines:])
-        with open(process.err_log, "r", encoding="utf-8") as f:
-            err_log = "\n".join(f.readlines()[-lines:])
-        return (out_log, err_log) if errors else out_log
+        if not process:
+            return None, None
+
+        out_log, err_log = "", ""
+
+        if out_log:
+            with open(process.out_log, "r", encoding="utf-8") as f:
+                out_log += "\n".join(f.readlines()[-lines:])
+
+        if err_log:
+            with open(process.err_log, "r", encoding="utf-8") as f:
+                err_log += "\n".join(f.readlines()[-lines:])
+
+        return (out_log, err_log)
```

### Comparing `pm2-0.0.4.1/pm2.egg-info/PKG-INFO` & `pm2-0.0.4.2/pm2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm2
-Version: 0.0.4.1
+Version: 0.0.4.2
 Summary: Python wrapper for PM2
 Home-page: https://github.com/y4kupkaya/pm2
 Author: y4kupkaya
 Author-email: contact@yakupkaya.net.tr
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Keywords: process-manager,pm2,pm2-py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pm2-0.0.4.1/setup.py` & `pm2-0.0.4.2/setup.py`

 * *Files identical despite different names*

