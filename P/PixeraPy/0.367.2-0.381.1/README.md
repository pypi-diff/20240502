# Comparing `tmp/PixeraPy-0.367.2.tar.gz` & `tmp/PixeraPy-0.381.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PixeraPy-0.367.2.tar", last modified: Wed Dec 13 02:49:38 2023, max compression
+gzip compressed data, was "PixeraPy-0.381.1.tar", last modified: Thu May  2 15:20:09 2024, max compression
```

## Comparing `PixeraPy-0.367.2.tar` & `PixeraPy-0.381.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-12-13 02:49:38.888544 PixeraPy-0.367.2/
--rw-rw-rw-   0        0        0     1078 2023-11-24 20:54:59.000000 PixeraPy-0.367.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2260 2023-12-13 02:49:38.888048 PixeraPy-0.367.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-12-13 02:49:38.876639 PixeraPy-0.367.2/PixeraPy/
--rw-rw-rw-   0        0        0       92 2023-11-24 20:52:23.000000 PixeraPy-0.367.2/PixeraPy/__init__.py
--rw-rw-rw-   0        0        0   177319 2023-12-13 02:28:56.000000 PixeraPy-0.367.2/PixeraPy/api_functions.py
--rw-rw-rw-   0        0        0     8498 2023-12-13 02:33:46.000000 PixeraPy-0.367.2/PixeraPy/pixera.py
-drwxrwxrwx   0        0        0        0 2023-12-13 02:49:38.887551 PixeraPy-0.367.2/PixeraPy.egg-info/
--rw-rw-rw-   0        0        0     2260 2023-12-13 02:49:38.000000 PixeraPy-0.367.2/PixeraPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-12-13 02:49:38.000000 PixeraPy-0.367.2/PixeraPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-13 02:49:38.000000 PixeraPy-0.367.2/PixeraPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-12-13 02:49:38.000000 PixeraPy-0.367.2/PixeraPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-12-13 02:49:38.000000 PixeraPy-0.367.2/PixeraPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1740 2023-12-13 01:31:34.000000 PixeraPy-0.367.2/README.md
--rw-rw-rw-   0        0        0       42 2023-12-13 02:49:38.888544 PixeraPy-0.367.2/setup.cfg
--rw-rw-rw-   0        0        0      885 2023-12-13 02:49:00.000000 PixeraPy-0.367.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:20:09.062096 PixeraPy-0.381.1/
+-rw-rw-rw-   0        0        0     1078 2023-11-24 20:54:59.000000 PixeraPy-0.381.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2260 2024-05-02 15:20:09.061600 PixeraPy-0.381.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 15:20:09.051680 PixeraPy-0.381.1/PixeraPy/
+-rw-rw-rw-   0        0        0       92 2023-11-24 20:52:23.000000 PixeraPy-0.381.1/PixeraPy/__init__.py
+-rw-rw-rw-   0        0        0   177978 2024-05-02 14:47:14.000000 PixeraPy-0.381.1/PixeraPy/api_functions.py
+-rw-rw-rw-   0        0        0     8498 2023-12-13 03:05:31.000000 PixeraPy-0.381.1/PixeraPy/pixera.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:20:09.060608 PixeraPy-0.381.1/PixeraPy.egg-info/
+-rw-rw-rw-   0        0        0     2260 2024-05-02 15:20:08.000000 PixeraPy-0.381.1/PixeraPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-05-02 15:20:09.000000 PixeraPy-0.381.1/PixeraPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 15:20:08.000000 PixeraPy-0.381.1/PixeraPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 15:20:08.000000 PixeraPy-0.381.1/PixeraPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 15:20:08.000000 PixeraPy-0.381.1/PixeraPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1740 2023-12-13 01:31:34.000000 PixeraPy-0.381.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 15:20:09.062096 PixeraPy-0.381.1/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-05-02 14:55:25.000000 PixeraPy-0.381.1/setup.py
```

### Comparing `PixeraPy-0.367.2/LICENSE.txt` & `PixeraPy-0.381.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PixeraPy-0.367.2/PKG-INFO` & `PixeraPy-0.381.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PixeraPy
-Version: 0.367.2
+Version: 0.381.1
 Summary: Python package for AVStumpfl, Pixera API
 Home-page: https://github.com/Tedcharlesbrown/Pixera-TCB/tree/main/01-Custom/03-API
 Author: Ted Charles Brown
 Author-email: tedcharlesbrown@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PixeraPy-0.367.2/PixeraPy/api_functions.py` & `PixeraPy-0.381.1/PixeraPy/api_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,14 +732,20 @@
         def getInst(handle: handle, instancePath: str) -> handle:
             method = "Pixera.LiveSystems.MultiUserMember.getInst"
             params = ["handle", "instancePath"]
             return [method, params, [handle, instancePath]]
 
     class LiveSystem:
         @staticmethod
+        def ref(handle: handle) -> handle:
+            method = "Pixera.LiveSystems.LiveSystem.ref"
+            params = ["handle"]
+            return [method, params, [handle]]
+
+        @staticmethod
         def getName(handle: handle) -> str:
             method = "Pixera.LiveSystems.LiveSystem.getName"
             params = ["handle"]
             return [method, params, [handle]]
 
         @staticmethod
         def getIp(handle: handle) -> str:
@@ -3984,14 +3990,26 @@
         @staticmethod
         def setTimelineTriggerApplyCue(handle: handle, goalCueLabel: str) -> bool:
             method = "Pixera.Timelines.Cue.setTimelineTriggerApplyCue"
             params = ["handle", "goalCueLabel"]
             return [method, params, [handle, goalCueLabel]]
 
         @staticmethod
+        def isActive(handle: handle) -> bool:
+            method = "Pixera.Timelines.Cue.isActive"
+            params = ["handle"]
+            return [method, params, [handle]]
+
+        @staticmethod
+        def setActivity(handle: handle, idState: int) -> None:
+            method = "Pixera.Timelines.Cue.setActivity"
+            params = ["handle", "idState"]
+            return [method, params, [handle, idState]]
+
+        @staticmethod
         def getCountdown(handle: handle) -> float:
             method = "Pixera.Timelines.Cue.getCountdown"
             params = ["handle"]
             return [method, params, [handle]]
 
         @staticmethod
         def getCountdownHMSF(handle: handle) -> str:
```

### Comparing `PixeraPy-0.367.2/PixeraPy/pixera.py` & `PixeraPy-0.381.1/PixeraPy/pixera.py`

 * *Files identical despite different names*

### Comparing `PixeraPy-0.367.2/PixeraPy.egg-info/PKG-INFO` & `PixeraPy-0.381.1/PixeraPy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PixeraPy
-Version: 0.367.2
+Version: 0.381.1
 Summary: Python package for AVStumpfl, Pixera API
 Home-page: https://github.com/Tedcharlesbrown/Pixera-TCB/tree/main/01-Custom/03-API
 Author: Ted Charles Brown
 Author-email: tedcharlesbrown@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PixeraPy-0.367.2/README.md` & `PixeraPy-0.381.1/README.md`

 * *Files identical despite different names*

### Comparing `PixeraPy-0.367.2/setup.py` & `PixeraPy-0.381.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
 
 from setuptools import setup, find_packages
 
 setup(
     name='PixeraPy',
-    version='0.367.2',
+    version='0.381.1',
     packages=find_packages(),
     description='Python package for AVStumpfl, Pixera API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Tedcharlesbrown/Pixera-TCB/tree/main/01-Custom/03-API',
     author='Ted Charles Brown',
     author_email='tedcharlesbrown@gmail.com',
```

