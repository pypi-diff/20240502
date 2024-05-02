# Comparing `tmp/fc_pruning-0.0.4.tar.gz` & `tmp/fc_pruning-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fc_pruning-0.0.4.tar", last modified: Tue Apr 30 18:23:33 2024, max compression
+gzip compressed data, was "fc_pruning-0.0.5.tar", last modified: Thu May  2 10:57:32 2024, max compression
```

## Comparing `fc_pruning-0.0.4.tar` & `fc_pruning-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:23:33.778725 fc_pruning-0.0.4/
--rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-04-30 18:18:40.000000 fc_pruning-0.0.4/LICENSE
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-04-30 18:23:33.778622 fc_pruning-0.0.4/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-30 18:18:40.000000 fc_pruning-0.0.4/README.md
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:23:33.776973 fc_pruning-0.0.4/fc_pruning/
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:23:33.778347 fc_pruning-0.0.4/fc_pruning/Compress/
--rw-r--r--   0 aidamehammed   (501) staff       (20)       49 2024-04-30 18:22:57.000000 fc_pruning-0.0.4/fc_pruning/Compress/__init__.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     5655 2024-04-30 18:22:57.000000 fc_pruning-0.0.4/fc_pruning/Compress/compress.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     4983 2024-04-30 18:22:57.000000 fc_pruning-0.0.4/fc_pruning/Compress/utils.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:22:57.000000 fc_pruning-0.0.4/fc_pruning/__init__.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     4112 2024-04-30 18:22:57.000000 fc_pruning-0.0.4/fc_pruning/utils.py
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:23:33.777733 fc_pruning-0.0.4/fc_pruning.egg-info/
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-04-30 18:23:33.000000 fc_pruning-0.0.4/fc_pruning.egg-info/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      331 2024-04-30 18:23:33.000000 fc_pruning-0.0.4/fc_pruning.egg-info/SOURCES.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-04-30 18:23:33.000000 fc_pruning-0.0.4/fc_pruning.egg-info/dependency_links.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-04-30 18:23:33.000000 fc_pruning-0.0.4/fc_pruning.egg-info/requires.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       11 2024-04-30 18:23:33.000000 fc_pruning-0.0.4/fc_pruning.egg-info/top_level.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-04-30 18:23:33.778771 fc_pruning-0.0.4/setup.cfg
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1202 2024-04-30 18:22:57.000000 fc_pruning-0.0.4/setup.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-02 10:57:32.341402 fc_pruning-0.0.5/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-04-30 18:18:40.000000 fc_pruning-0.0.5/LICENSE
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-02 10:57:32.341262 fc_pruning-0.0.5/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-30 18:18:40.000000 fc_pruning-0.0.5/README.md
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-02 10:57:32.339312 fc_pruning-0.0.5/fc_pruning/
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-02 10:57:32.340916 fc_pruning-0.0.5/fc_pruning/Compress/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       49 2024-04-30 18:22:57.000000 fc_pruning-0.0.5/fc_pruning/Compress/__init__.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     5689 2024-04-30 18:40:51.000000 fc_pruning-0.0.5/fc_pruning/Compress/compress.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     4983 2024-04-30 18:22:57.000000 fc_pruning-0.0.5/fc_pruning/Compress/utils.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:22:57.000000 fc_pruning-0.0.5/fc_pruning/__init__.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     4112 2024-04-30 18:22:57.000000 fc_pruning-0.0.5/fc_pruning/utils.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-02 10:57:32.340250 fc_pruning-0.0.5/fc_pruning.egg-info/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-02 10:57:32.000000 fc_pruning-0.0.5/fc_pruning.egg-info/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      331 2024-05-02 10:57:32.000000 fc_pruning-0.0.5/fc_pruning.egg-info/SOURCES.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-05-02 10:57:32.000000 fc_pruning-0.0.5/fc_pruning.egg-info/dependency_links.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-05-02 10:57:32.000000 fc_pruning-0.0.5/fc_pruning.egg-info/requires.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       11 2024-05-02 10:57:32.000000 fc_pruning-0.0.5/fc_pruning.egg-info/top_level.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-05-02 10:57:32.341458 fc_pruning-0.0.5/setup.cfg
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1202 2024-05-02 10:54:24.000000 fc_pruning-0.0.5/setup.py
```

### Comparing `fc_pruning-0.0.4/LICENSE` & `fc_pruning-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.4/PKG-INFO` & `fc_pruning-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc_pruning
-Version: 0.0.4
+Version: 0.0.5
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning/issues
 Platform: UNKNOWN
```

### Comparing `fc_pruning-0.0.4/README.md` & `fc_pruning-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.4/fc_pruning/Compress/compress.py` & `fc_pruning-0.0.5/fc_pruning/Compress/compress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from FeatureCloud.app.engine.app import AppState
 from typing import TypedDict, Union, List, Type
 import torch
 import torch_pruning as tp
+import sys
+print(sys.executable)
+
 import fc_pruning.Compress.utils as pf
 
 print('running')
 
 class PruningType(TypedDict):
     model: torch.nn.Module
     reference_model: Union[List[torch.nn.Module], None]
```

### Comparing `fc_pruning-0.0.4/fc_pruning/Compress/utils.py` & `fc_pruning-0.0.5/fc_pruning/Compress/utils.py`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.4/fc_pruning/utils.py` & `fc_pruning-0.0.5/fc_pruning/utils.py`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.4/fc_pruning.egg-info/PKG-INFO` & `fc_pruning-0.0.5/fc_pruning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-pruning
-Version: 0.0.4
+Version: 0.0.5
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning/issues
 Platform: UNKNOWN
```

### Comparing `fc_pruning-0.0.4/setup.py` & `fc_pruning-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name="fc_pruning",
-                 version="0.0.4",
+                 version="0.0.5",
                  author="Aida Mehammed",
                  author_email="aida.mehammed@studium.uni-hamburg.de",
                  description="FC Pruning",
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url="https://github.com/AidaMehammed/fc_pruning",
                  project_urls={
```

