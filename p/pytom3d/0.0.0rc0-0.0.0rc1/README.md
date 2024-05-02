# Comparing `tmp/pytom3d-0.0.0rc0.tar.gz` & `tmp/pytom3d-0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytom3d-0.0.0rc0.tar", last modified: Wed May  1 15:18:43 2024, max compression
+gzip compressed data, was "pytom3d-0.0.0rc1.tar", last modified: Thu May  2 08:19:28 2024, max compression
```

## Comparing `pytom3d-0.0.0rc0.tar` & `pytom3d-0.0.0rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-01 15:18:43.026654 pytom3d-0.0.0rc0/
--rw-rw-r--   0 ale       (1000) ale       (1000)    32473 2024-04-29 13:58:35.000000 pytom3d-0.0.0rc0/LICENSE
--rw-r--r--   0 ale       (1000) ale       (1000)    10927 2024-05-01 15:18:43.026654 pytom3d-0.0.0rc0/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     9974 2024-05-01 15:12:45.000000 pytom3d-0.0.0rc0/README.md
--rw-rw-r--   0 ale       (1000) ale       (1000)       86 2024-04-29 13:58:35.000000 pytom3d-0.0.0rc0/pyproject.toml
--rw-rw-r--   0 ale       (1000) ale       (1000)       38 2024-05-01 15:18:43.026654 pytom3d-0.0.0rc0/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1123 2024-05-01 15:17:39.000000 pytom3d-0.0.0rc0/setup.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-01 15:18:43.022654 pytom3d-0.0.0rc0/src/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-01 15:18:43.022654 pytom3d-0.0.0rc0/src/pytom3d/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2024-04-29 13:58:35.000000 pytom3d-0.0.0rc0/src/pytom3d/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    17041 2024-04-29 13:58:35.000000 pytom3d-0.0.0rc0/src/pytom3d/core.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2688 2024-05-01 14:30:14.000000 pytom3d-0.0.0rc0/src/pytom3d/scan.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2214 2024-04-30 13:39:00.000000 pytom3d-0.0.0rc0/src/pytom3d/stats.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    14028 2024-05-01 14:29:46.000000 pytom3d-0.0.0rc0/src/pytom3d/util.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    17747 2024-05-01 14:31:12.000000 pytom3d-0.0.0rc0/src/pytom3d/viewer.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-01 15:18:43.022654 pytom3d-0.0.0rc0/src/pytom3d.egg-info/
--rw-r--r--   0 ale       (1000) ale       (1000)    10927 2024-05-01 15:18:43.000000 pytom3d-0.0.0rc0/src/pytom3d.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)      342 2024-05-01 15:18:43.000000 pytom3d-0.0.0rc0/src/pytom3d.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-05-01 15:18:43.000000 pytom3d-0.0.0rc0/src/pytom3d.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      112 2024-05-01 15:18:43.000000 pytom3d-0.0.0rc0/src/pytom3d.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        8 2024-05-01 15:18:43.000000 pytom3d-0.0.0rc0/src/pytom3d.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 08:19:28.320021 pytom3d-0.0.0rc1/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    32473 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/LICENSE
+-rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-02 08:19:28.320021 pytom3d-0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)      613 2024-05-02 08:15:05.000000 pytom3d-0.0.0rc1/README.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)       86 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/pyproject.toml
+-rw-rw-r--   0 ale       (1000) ale       (1000)       38 2024-05-02 08:19:28.320021 pytom3d-0.0.0rc1/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1123 2024-05-02 08:19:09.000000 pytom3d-0.0.0rc1/setup.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 08:19:28.316021 pytom3d-0.0.0rc1/src/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 08:19:28.316021 pytom3d-0.0.0rc1/src/pytom3d/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17041 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/core.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2688 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/scan.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2214 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/stats.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    14028 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/util.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17747 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/viewer.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 08:19:28.316021 pytom3d-0.0.0rc1/src/pytom3d.egg-info/
+-rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-02 08:19:28.000000 pytom3d-0.0.0rc1/src/pytom3d.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)      342 2024-05-02 08:19:28.000000 pytom3d-0.0.0rc1/src/pytom3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-05-02 08:19:28.000000 pytom3d-0.0.0rc1/src/pytom3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      112 2024-05-02 08:19:28.000000 pytom3d-0.0.0rc1/src/pytom3d.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        8 2024-05-02 08:19:28.000000 pytom3d-0.0.0rc1/src/pytom3d.egg-info/top_level.txt
```

### Comparing `pytom3d-0.0.0rc0/LICENSE` & `pytom3d-0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc0/setup.py` & `pytom3d-0.0.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pytom3d",
-    version="0.0.0rc0",
+    version="0.0.0rc1",
     description="PyToM-3D: Python Topography Manipulator in 3D",
     long_description=long_description,
     long_description_content_type="text/markdown",
         
     author="Alessandro Tognan",
     author_email="alessandro.tognan@gmail.com",
     url="https://github.com/aletgn/pytom-3d.git",
```

### Comparing `pytom3d-0.0.0rc0/src/pytom3d/core.py` & `pytom3d-0.0.0rc1/src/pytom3d/core.py`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc0/src/pytom3d/scan.py` & `pytom3d-0.0.0rc1/src/pytom3d/scan.py`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc0/src/pytom3d/stats.py` & `pytom3d-0.0.0rc1/src/pytom3d/stats.py`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc0/src/pytom3d/util.py` & `pytom3d-0.0.0rc1/src/pytom3d/util.py`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc0/src/pytom3d/viewer.py` & `pytom3d-0.0.0rc1/src/pytom3d/viewer.py`

 * *Files identical despite different names*

