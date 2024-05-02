# Comparing `tmp/templated_setup-0.952.tar.gz` & `tmp/templated_setup-0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.952.tar", last modified: Thu May  2 04:58:04 2024, max compression
+gzip compressed data, was "templated_setup-0.953.tar", last modified: Thu May  2 05:06:01 2024, max compression
```

## Comparing `templated_setup-0.952.tar` & `templated_setup-0.953.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:58:04.573497 templated_setup-0.952/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.952/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 04:58:04.572864 templated_setup-0.952/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.952/README.md
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 04:58:04.573606 templated_setup-0.952/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.952/setup.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:58:04.569085 templated_setup-0.952/templated_setup/
--rw-r--r--   0 joel-watson   (501) staff       (20)    19827 2024-05-02 04:57:16.000000 templated_setup-0.952/templated_setup/__init__.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 04:58:04.572147 templated_setup-0.952/templated_setup.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 04:58:04.000000 templated_setup-0.952/templated_setup.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 04:58:04.000000 templated_setup-0.952/templated_setup.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 04:58:04.000000 templated_setup-0.952/templated_setup.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 04:58:04.000000 templated_setup-0.952/templated_setup.egg-info/top_level.txt
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 05:06:01.260096 templated_setup-0.953/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-05-02 00:01:08.000000 templated_setup-0.953/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 05:06:01.259525 templated_setup-0.953/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2111 2024-05-02 00:01:08.000000 templated_setup-0.953/README.md
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 05:06:01.260198 templated_setup-0.953/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      362 2024-05-02 04:50:07.000000 templated_setup-0.953/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 05:06:01.257178 templated_setup-0.953/templated_setup/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    20042 2024-05-02 05:05:37.000000 templated_setup-0.953/templated_setup/__init__.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 05:06:01.259056 templated_setup-0.953/templated_setup.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2467 2024-05-02 05:06:01.000000 templated_setup-0.953/templated_setup.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      210 2024-05-02 05:06:01.000000 templated_setup-0.953/templated_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 05:06:01.000000 templated_setup-0.953/templated_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       16 2024-05-02 05:06:01.000000 templated_setup-0.953/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.952/LICENCE` & `templated_setup-0.953/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.952/PKG-INFO` & `templated_setup-0.953/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.952
+Version: 0.953
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Standardized `setup.py`
@@ -65,9 +65,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.952 released on 2nd/5/2024
+## V0.953 released on 2nd/5/2024
 god please kill me. ;(
```

### Comparing `templated_setup-0.952/README.md` & `templated_setup-0.953/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.952/templated_setup/__init__.py` & `templated_setup-0.953/templated_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from dataclasses import dataclass as dataclass_x_dataclass
 from json import load as json_x_load, dump as json_x_dump, loads as json_x_loads, dumps as json_x_dumps
 from datetime import date as datetime_x_date
-from time import sleep as time_x_sleep
+#from time import sleep as time_x_sleep
 from typing import Callable, overload
 from setuptools import setup
 import shutil
 import sys
 import os
 
+def time_x_sleep(x):
+	pass
 
 
 
 
 
 
 CACHE_FILE_PATH = ""
@@ -591,15 +593,19 @@
 
 
 
 	@classmethod
 	def _load_from_hardcoded(cls):
 
 		cls._is_using_pip = False
+		if os.path.exists(os.path.join(cls._base_dir, "IS_USING_PIP.txt")):
+			cls._is_using_pip = True
 		if "PIP_BUILD_TRACKER" in " ".join(os.environ.keys()):
+			with open(os.path.join(cls._base_dir, "IS_USING_PIP.txt"), "w") as f:
+				f.write("")
 			cls._is_using_pip = True
 
 		try:
 			__ = cls._json_data
 		except AttributeError:
 			cls._json_data = None
 		cls.__inner_reload_cached_data()
```

### Comparing `templated_setup-0.952/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.953/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.952
+Version: 0.953
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Standardized `setup.py`
@@ -65,9 +65,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.952 released on 2nd/5/2024
+## V0.953 released on 2nd/5/2024
 god please kill me. ;(
```

