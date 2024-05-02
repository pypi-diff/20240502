# Comparing `tmp/efel-5.6.8.tar.gz` & `tmp/efel-5.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efel-5.6.8.tar", last modified: Thu Apr 25 07:59:10 2024, max compression
+gzip compressed data, was "efel-5.6.9.tar", last modified: Thu Apr 25 09:18:57 2024, max compression
```

## Comparing `efel-5.6.8.tar` & `efel-5.6.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:59:10.501384 efel-5.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 07:59:09.000000 efel-5.6.8/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-04-25 07:59:09.000000 efel-5.6.8/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-25 07:59:09.000000 efel-5.6.8/COPYING.less
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-25 07:59:09.000000 efel-5.6.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-25 07:59:09.000000 efel-5.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-25 07:59:10.501384 efel-5.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-25 07:59:09.000000 efel-5.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:59:10.493384 efel-5.6.8/efel/
--rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-04-25 07:59:09.000000 efel-5.6.8/efel/DependencyV5.txt
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-25 07:59:09.000000 efel-5.6.8/efel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 07:59:10.501384 efel-5.6.8/efel/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-04-25 07:59:09.000000 efel-5.6.8/efel/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:59:10.497384 efel-5.6.8/efel/cppcore/
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/DependencyTree.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/DependencyTree.h
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/EfelExceptions.h
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/FillFptrTable.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/FillFptrTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/Global.h
--rw-r--r--   0 runner    (1001) docker     (127)    38348 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/LibV1.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/LibV1.h
--rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/LibV2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/LibV2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/LibV3.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/LibV3.h
--rw-r--r--   0 runner    (1001) docker     (127)    92113 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/LibV5.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/LibV5.h
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/Utils.h
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/cfeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/cfeature.h
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/cppcore.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/eFELLogger.h
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/mapoperations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/mapoperations.h
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore/types.h
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-25 07:59:09.000000 efel-5.6.8/efel/cppcore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-25 07:59:09.000000 efel-5.6.8/efel/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:59:10.497384 efel-5.6.8/efel/pyfeatures/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-25 07:59:09.000000 efel-5.6.8/efel/pyfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-25 07:59:09.000000 efel-5.6.8/efel/pyfeatures/cppfeature_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-04-25 07:59:09.000000 efel-5.6.8/efel/pyfeatures/isi.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-25 07:59:09.000000 efel-5.6.8/efel/pyfeatures/multitrace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-25 07:59:09.000000 efel-5.6.8/efel/pyfeatures/pyfeatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-25 07:59:09.000000 efel-5.6.8/efel/pyfeatures/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-25 07:59:09.000000 efel-5.6.8/efel/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:59:10.501384 efel-5.6.8/efel/units/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-25 07:59:09.000000 efel-5.6.8/efel/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-25 07:59:09.000000 efel-5.6.8/efel/units/units.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:59:10.493384 efel-5.6.8/efel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-25 07:59:10.000000 efel-5.6.8/efel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-25 07:59:10.000000 efel-5.6.8/efel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:59:10.000000 efel-5.6.8/efel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 07:59:10.000000 efel-5.6.8/efel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 07:59:10.000000 efel-5.6.8/efel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-25 07:59:09.000000 efel-5.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-25 07:59:10.501384 efel-5.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-25 07:59:09.000000 efel-5.6.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-25 07:59:09.000000 efel-5.6.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:18:57.988291 efel-5.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 09:18:56.000000 efel-5.6.9/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-04-25 09:18:56.000000 efel-5.6.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-25 09:18:56.000000 efel-5.6.9/COPYING.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-25 09:18:56.000000 efel-5.6.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-25 09:18:56.000000 efel-5.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-25 09:18:57.988291 efel-5.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-25 09:18:56.000000 efel-5.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:18:57.980291 efel-5.6.9/efel/
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2024-04-25 09:18:56.000000 efel-5.6.9/efel/DependencyV5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-25 09:18:56.000000 efel-5.6.9/efel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 09:18:57.988291 efel-5.6.9/efel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-04-25 09:18:56.000000 efel-5.6.9/efel/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:18:57.988291 efel-5.6.9/efel/cppcore/
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/DependencyTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/DependencyTree.h
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/EfelExceptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/FillFptrTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/FillFptrTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/Global.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38348 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/LibV1.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/LibV1.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/LibV2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/LibV2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/LibV3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/LibV3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    92113 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/LibV5.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/LibV5.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/Utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/cfeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/cfeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/cppcore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/eFELLogger.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/mapoperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/mapoperations.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore/types.h
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-25 09:18:56.000000 efel-5.6.9/efel/cppcore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-25 09:18:56.000000 efel-5.6.9/efel/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:18:57.988291 efel-5.6.9/efel/pyfeatures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-25 09:18:56.000000 efel-5.6.9/efel/pyfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-25 09:18:56.000000 efel-5.6.9/efel/pyfeatures/cppfeature_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-04-25 09:18:56.000000 efel-5.6.9/efel/pyfeatures/isi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-25 09:18:56.000000 efel-5.6.9/efel/pyfeatures/multitrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-25 09:18:56.000000 efel-5.6.9/efel/pyfeatures/pyfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-25 09:18:56.000000 efel-5.6.9/efel/pyfeatures/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-25 09:18:56.000000 efel-5.6.9/efel/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:18:57.988291 efel-5.6.9/efel/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-25 09:18:56.000000 efel-5.6.9/efel/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-25 09:18:56.000000 efel-5.6.9/efel/units/units.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:18:57.984291 efel-5.6.9/efel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-25 09:18:57.000000 efel-5.6.9/efel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-25 09:18:57.000000 efel-5.6.9/efel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:18:57.000000 efel-5.6.9/efel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 09:18:57.000000 efel-5.6.9/efel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 09:18:57.000000 efel-5.6.9/efel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-25 09:18:56.000000 efel-5.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-25 09:18:57.988291 efel-5.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-25 09:18:56.000000 efel-5.6.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-25 09:18:56.000000 efel-5.6.9/versioneer.py
```

### Comparing `efel-5.6.8/COPYING` & `efel-5.6.9/COPYING`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/COPYING.less` & `efel-5.6.9/COPYING.less`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/LICENSE.txt` & `efel-5.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/PKG-INFO` & `efel-5.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 5.6.8
+Version: 5.6.9
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-5.6.8/README.md` & `efel-5.6.9/README.md`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/DependencyV5.txt` & `efel-5.6.9/efel/DependencyV5.txt`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/__init__.py` & `efel-5.6.9/efel/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/api.py` & `efel-5.6.9/efel/api.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/DependencyTree.cpp` & `efel-5.6.9/efel/cppcore/DependencyTree.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/DependencyTree.h` & `efel-5.6.9/efel/cppcore/DependencyTree.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/EfelExceptions.h` & `efel-5.6.9/efel/cppcore/EfelExceptions.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/FillFptrTable.cpp` & `efel-5.6.9/efel/cppcore/FillFptrTable.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/FillFptrTable.h` & `efel-5.6.9/efel/cppcore/FillFptrTable.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/Global.h` & `efel-5.6.9/efel/cppcore/Global.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/LibV1.cpp` & `efel-5.6.9/efel/cppcore/LibV1.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/LibV1.h` & `efel-5.6.9/efel/cppcore/LibV1.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/LibV2.cpp` & `efel-5.6.9/efel/cppcore/LibV2.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/LibV2.h` & `efel-5.6.9/efel/cppcore/LibV2.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/LibV3.cpp` & `efel-5.6.9/efel/cppcore/LibV3.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/LibV3.h` & `efel-5.6.9/efel/cppcore/LibV3.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/LibV5.cpp` & `efel-5.6.9/efel/cppcore/LibV5.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/LibV5.h` & `efel-5.6.9/efel/cppcore/LibV5.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/Utils.cpp` & `efel-5.6.9/efel/cppcore/Utils.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/Utils.h` & `efel-5.6.9/efel/cppcore/Utils.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/cfeature.cpp` & `efel-5.6.9/efel/cppcore/cfeature.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/cfeature.h` & `efel-5.6.9/efel/cppcore/cfeature.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/cppcore.cpp` & `efel-5.6.9/efel/cppcore/cppcore.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/eFELLogger.h` & `efel-5.6.9/efel/cppcore/eFELLogger.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/mapoperations.cpp` & `efel-5.6.9/efel/cppcore/mapoperations.cpp`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/mapoperations.h` & `efel-5.6.9/efel/cppcore/mapoperations.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore/types.h` & `efel-5.6.9/efel/cppcore/types.h`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/cppcore.pyi` & `efel-5.6.9/efel/cppcore.pyi`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/io.py` & `efel-5.6.9/efel/io.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/pyfeatures/__init__.py` & `efel-5.6.9/efel/pyfeatures/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/pyfeatures/cppfeature_access.py` & `efel-5.6.9/efel/pyfeatures/cppfeature_access.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/pyfeatures/isi.py` & `efel-5.6.9/efel/pyfeatures/isi.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/pyfeatures/multitrace.py` & `efel-5.6.9/efel/pyfeatures/multitrace.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/pyfeatures/pyfeatures.py` & `efel-5.6.9/efel/pyfeatures/pyfeatures.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/pyfeatures/validation.py` & `efel-5.6.9/efel/pyfeatures/validation.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/settings.py` & `efel-5.6.9/efel/settings.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel/units/units.json` & `efel-5.6.9/efel/units/units.json`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/efel.egg-info/PKG-INFO` & `efel-5.6.9/efel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 5.6.8
+Version: 5.6.9
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-5.6.8/efel.egg-info/SOURCES.txt` & `efel-5.6.9/efel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/setup.py` & `efel-5.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `efel-5.6.8/versioneer.py` & `efel-5.6.9/versioneer.py`

 * *Files identical despite different names*

