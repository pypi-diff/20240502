# Comparing `tmp/rbfmeshgen-1.0.3.tar.gz` & `tmp/rbfmeshgen-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbfmeshgen-1.0.3.tar", last modified: Mon Apr 29 17:13:53 2024, max compression
+gzip compressed data, was "rbfmeshgen-1.0.4.tar", last modified: Thu May  2 06:18:16 2024, max compression
```

## Comparing `rbfmeshgen-1.0.3.tar` & `rbfmeshgen-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:13:53.322396 rbfmeshgen-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-29 17:13:53.322396 rbfmeshgen-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:13:53.318396 rbfmeshgen-1.0.3/RBFMeshGen/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/RBFMeshGen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/RBFMeshGen/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/RBFMeshGen/mesh_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/RBFMeshGen/visualization_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:13:53.322396 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-29 17:13:53.000000 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 17:13:53.000000 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:13:53.000000 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 17:13:53.000000 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 17:13:53.000000 rbfmeshgen-1.0.3/RBFMeshGen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:13:53.322396 rbfmeshgen-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-29 17:13:44.000000 rbfmeshgen-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:18:16.254033 rbfmeshgen-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-02 06:18:16.254033 rbfmeshgen-1.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:18:16.250033 rbfmeshgen-1.0.4/RBFMeshGen/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-02 06:18:08.000000 rbfmeshgen-1.0.4/RBFMeshGen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-05-02 06:18:08.000000 rbfmeshgen-1.0.4/RBFMeshGen/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-05-02 06:18:08.000000 rbfmeshgen-1.0.4/RBFMeshGen/mesh_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-02 06:18:08.000000 rbfmeshgen-1.0.4/RBFMeshGen/visualization_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:18:16.254033 rbfmeshgen-1.0.4/RBFMeshGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-02 06:18:16.000000 rbfmeshgen-1.0.4/RBFMeshGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-02 06:18:16.000000 rbfmeshgen-1.0.4/RBFMeshGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:18:16.000000 rbfmeshgen-1.0.4/RBFMeshGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 06:18:16.000000 rbfmeshgen-1.0.4/RBFMeshGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 06:18:16.000000 rbfmeshgen-1.0.4/RBFMeshGen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-02 06:18:08.000000 rbfmeshgen-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:18:16.254033 rbfmeshgen-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-02 06:18:08.000000 rbfmeshgen-1.0.4/setup.py
```

### Comparing `rbfmeshgen-1.0.3/PKG-INFO` & `rbfmeshgen-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RBFMeshGen
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python package for generating random meshes based on radial basis functions.
 Home-page: https://github.com/LDBreton/RBFMeshGen
 Author: Louis Breton
 Author-email: louis.breton@ciencias.unam.mx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rbfmeshgen-1.0.3/RBFMeshGen/geometry_utils.py` & `rbfmeshgen-1.0.4/RBFMeshGen/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `rbfmeshgen-1.0.3/RBFMeshGen/visualization_tools.py` & `rbfmeshgen-1.0.4/RBFMeshGen/visualization_tools.py`

 * *Files identical despite different names*

### Comparing `rbfmeshgen-1.0.3/RBFMeshGen.egg-info/PKG-INFO` & `rbfmeshgen-1.0.4/RBFMeshGen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RBFMeshGen
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python package for generating random meshes based on radial basis functions.
 Home-page: https://github.com/LDBreton/RBFMeshGen
 Author: Louis Breton
 Author-email: louis.breton@ciencias.unam.mx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rbfmeshgen-1.0.3/README.md` & `rbfmeshgen-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rbfmeshgen-1.0.3/setup.py` & `rbfmeshgen-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="RBFMeshGen",
-    version="1.0.3",
+    version="1.0.4",
     author="Louis Breton",
     author_email="louis.breton@ciencias.unam.mx",
     description="A Python package for generating random meshes based on radial basis functions.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/LDBreton/RBFMeshGen",
     packages=find_packages(),
```

