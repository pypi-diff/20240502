# Comparing `tmp/pm2-0.0.4.2.tar.gz` & `tmp/pm2-0.0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm2-0.0.4.2.tar", last modified: Wed May  1 18:20:56 2024, max compression
+gzip compressed data, was "pm2-0.0.4.3.tar", last modified: Wed May  1 23:04:54 2024, max compression
```

## Comparing `pm2-0.0.4.2.tar` & `pm2-0.0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 18:20:56.493099 pm2-0.0.4.2/
--rw-rw-rw-   0        0        0    35803 2024-04-30 09:18:53.000000 pm2-0.0.4.2/LICENSE
--rw-rw-rw-   0        0        0     4842 2024-05-01 18:20:56.412107 pm2-0.0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3318 2024-04-30 09:18:53.000000 pm2-0.0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 18:20:56.293089 pm2-0.0.4.2/pm2/
--rw-rw-rw-   0        0        0    10340 2024-05-01 18:20:48.000000 pm2-0.0.4.2/pm2/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-30 09:18:53.000000 pm2-0.0.4.2/pm2/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 18:20:56.403092 pm2-0.0.4.2/pm2.egg-info/
--rw-rw-rw-   0        0        0     4842 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-01 18:20:55.000000 pm2-0.0.4.2/pm2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 18:20:56.494097 pm2-0.0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     2052 2024-04-30 09:22:44.000000 pm2-0.0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:04:53.985823 pm2-0.0.4.3/
+-rw-rw-rw-   0        0        0    35803 2024-04-30 09:18:53.000000 pm2-0.0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     4842 2024-05-01 23:04:53.920836 pm2-0.0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3318 2024-04-30 09:18:53.000000 pm2-0.0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 23:04:53.682816 pm2-0.0.4.3/pm2/
+-rw-rw-rw-   0        0        0    11068 2024-05-01 23:04:17.000000 pm2-0.0.4.3/pm2/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 09:18:53.000000 pm2-0.0.4.3/pm2/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:04:53.914831 pm2-0.0.4.3/pm2.egg-info/
+-rw-rw-rw-   0        0        0     4842 2024-05-01 23:04:52.000000 pm2-0.0.4.3/pm2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-01 23:04:53.000000 pm2-0.0.4.3/pm2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 23:04:52.000000 pm2-0.0.4.3/pm2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-01 23:04:52.000000 pm2-0.0.4.3/pm2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       22 2024-05-01 23:04:52.000000 pm2-0.0.4.3/pm2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-01 23:04:52.000000 pm2-0.0.4.3/pm2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 23:04:53.986827 pm2-0.0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     2052 2024-04-30 09:22:44.000000 pm2-0.0.4.3/setup.py
```

### Comparing `pm2-0.0.4.2/LICENSE` & `pm2-0.0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pm2-0.0.4.2/PKG-INFO` & `pm2-0.0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm2
-Version: 0.0.4.2
+Version: 0.0.4.3
 Summary: Python wrapper for PM2
 Home-page: https://github.com/y4kupkaya/pm2
 Author: y4kupkaya
 Author-email: contact@yakupkaya.net.tr
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Keywords: process-manager,pm2,pm2-py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pm2-0.0.4.2/README.md` & `pm2-0.0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pm2-0.0.4.2/pm2/__init__.py` & `pm2-0.0.4.3/pm2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from typing import Any, List, Optional
 
 import aiofiles
 from aylak.rich.console import Console
 
 console = Console()
 
-__version__ = "0.0.4.2"
+__version__ = "0.0.4.3"
 
 
 class PathIsFolderError(Exception):
     pass
 
 
 class PM2Process:
@@ -136,29 +136,41 @@
                 or (pm_id is not None and process.pm_id == pm_id)
                 or (name is not None and process.name == name)
             ):
                 return process
         return None
 
     async def start(
-        self, path: str, name: str = None, extra_args: List[str] = None
+        self,
+        path: str,
+        name: str = None,
+        extra_args: List[str] = None,
+        pm_id: int = None,
     ) -> Optional[PM2Process]:
-        extra_args = extra_args or []
-        if os.path.isdir(path):
-            raise PathIsFolderError("Path is a folder; a file is expected.")
-        cmd = (
-            self.COMMAND
-            + ["start", path]
-            + (["--name", name] if name else [])
-            + extra_args
-        )
-        await self.execute_command(cmd)
-        return await self.get(
-            pm_id=max([process.pm_id for process in await self.list()])
-        )
+        if pm_id is None:
+            extra_args = extra_args or []
+            if os.path.isdir(path):
+                raise PathIsFolderError("Path is a folder; a file is expected.")
+            cmd = (
+                self.COMMAND
+                + ["start", path]
+                + (["--name", name] if name else [])
+                + extra_args
+            )
+            await self.execute_command(cmd)
+            return await self.get(
+                pm_id=max([process.pm_id for process in await self.list()])
+            )
+
+        else:
+            process = await self.get(pm_id=pm_id)
+            if process:
+                await self.execute_command(self.COMMAND + ["start", str(process.pm_id)])
+                return process
+            return None
 
     async def modify_process(
         self,
         action: str,
         pid: int = None,
         pm_id: int = None,
         name: str = None,
@@ -245,28 +257,39 @@
                 or (pm_id is not None and process.pm_id == pm_id)
                 or (name is not None and process.name == name)
             ):
                 return process
         return None
 
     def start(
-        self, path: str, name: str = None, extra_args: List[str] = None
+        self,
+        path: str,
+        name: str = None,
+        extra_args: List[str] = None,
+        pm_id: int = None,
     ) -> Optional[PM2Process]:
-        extra_args = extra_args or []
-        if os.path.isdir(path):
-
-            raise PathIsFolderError("Path is a folder; a file is expected.")
-        cmd = (
-            self.COMMAND
-            + ["start", path]
-            + (["--name", name] if name else [])
-            + extra_args
-        )
-        self.execute_command(cmd)
-        return self.get(pm_id=max([process.pm_id for process in self.list()]))
+        if pm_id is None:
+            extra_args = extra_args or []
+            if os.path.isdir(path):
+
+                raise PathIsFolderError("Path is a folder; a file is expected.")
+            cmd = (
+                self.COMMAND
+                + ["start", path]
+                + (["--name", name] if name else [])
+                + extra_args
+            )
+            self.execute_command(cmd)
+            return self.get(pm_id=max([process.pm_id for process in self.list()]))
+        else:
+            process = self.get(pm_id=pm_id)
+            if process:
+                self.execute_command(self.COMMAND + ["start", str(process.pm_id)])
+                return process
+            return None
 
     def modify_process(
         self,
         action: str,
         pid: int = None,
         pm_id: int = None,
         name: str = None,
```

### Comparing `pm2-0.0.4.2/pm2.egg-info/PKG-INFO` & `pm2-0.0.4.3/pm2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm2
-Version: 0.0.4.2
+Version: 0.0.4.3
 Summary: Python wrapper for PM2
 Home-page: https://github.com/y4kupkaya/pm2
 Author: y4kupkaya
 Author-email: contact@yakupkaya.net.tr
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Keywords: process-manager,pm2,pm2-py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pm2-0.0.4.2/setup.py` & `pm2-0.0.4.3/setup.py`

 * *Files identical despite different names*

