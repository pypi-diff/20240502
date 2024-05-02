# Comparing `tmp/spleendatads-1.0.8.tar.gz` & `tmp/spleendatads-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spleendatads-1.0.8.tar", last modified: Wed May  1 20:35:00 2024, max compression
+gzip compressed data, was "spleendatads-2.0.2.tar", last modified: Thu May  2 18:09:06 2024, max compression
```

## Comparing `spleendatads-1.0.8.tar` & `spleendatads-2.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-01 20:35:00.291669 spleendatads-1.0.8/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2024-04-22 17:46:01.000000 spleendatads-1.0.8/LICENSE
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     5639 2024-05-01 20:35:00.291669 spleendatads-1.0.8/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     5050 2024-05-01 20:34:59.000000 spleendatads-1.0.8/README.rst
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2024-05-01 20:35:00.291669 spleendatads-1.0.8/setup.cfg
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1469 2024-05-01 20:32:45.000000 spleendatads-1.0.8/setup.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-01 20:35:00.291669 spleendatads-1.0.8/spleendatads.egg-info/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     5639 2024-05-01 20:35:00.000000 spleendatads-1.0.8/spleendatads.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      283 2024-05-01 20:35:00.000000 spleendatads-1.0.8/spleendatads.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2024-05-01 20:35:00.000000 spleendatads-1.0.8/spleendatads.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       51 2024-05-01 20:35:00.000000 spleendatads-1.0.8/spleendatads.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       40 2024-05-01 20:35:00.000000 spleendatads-1.0.8/spleendatads.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       13 2024-05-01 20:35:00.000000 spleendatads-1.0.8/spleendatads.egg-info/top_level.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     4013 2024-05-01 20:34:19.000000 spleendatads-1.0.8/spleendatads.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-01 20:35:00.291669 spleendatads-1.0.8/tests/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      657 2024-04-22 17:46:01.000000 spleendatads-1.0.8/tests/test_example.py
+drwxrwxr-x   0 rudolphpienaar (2090878) domain_users (2000513)        0 2024-05-02 18:09:06.100030 spleendatads-2.0.2/
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     1069 2024-05-02 16:59:02.000000 spleendatads-2.0.2/LICENSE
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     5569 2024-05-02 18:09:06.097160 spleendatads-2.0.2/PKG-INFO
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     5051 2024-05-02 18:09:03.000000 spleendatads-2.0.2/README.rst
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)       38 2024-05-02 18:09:06.101985 spleendatads-2.0.2/setup.cfg
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     1469 2024-05-02 16:59:02.000000 spleendatads-2.0.2/setup.py
+drwxrwxr-x   0 rudolphpienaar (2090878) domain_users (2000513)        0 2024-05-02 18:09:06.075265 spleendatads-2.0.2/spleendatads.egg-info/
+-rw-r--r--   0 rudolphpienaar (2090878) domain_users (2000513)     5569 2024-05-02 18:09:05.000000 spleendatads-2.0.2/spleendatads.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)      283 2024-05-02 18:09:05.000000 spleendatads-2.0.2/spleendatads.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)        1 2024-05-02 18:09:05.000000 spleendatads-2.0.2/spleendatads.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)       51 2024-05-02 18:09:05.000000 spleendatads-2.0.2/spleendatads.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)       40 2024-05-02 18:09:05.000000 spleendatads-2.0.2/spleendatads.egg-info/requires.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)       13 2024-05-02 18:09:05.000000 spleendatads-2.0.2/spleendatads.egg-info/top_level.txt
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)     7435 2024-05-02 18:05:07.000000 spleendatads-2.0.2/spleendatads.py
+drwxrwxr-x   0 rudolphpienaar (2090878) domain_users (2000513)        0 2024-05-02 18:09:06.087186 spleendatads-2.0.2/tests/
+-rw-rw-r--   0 rudolphpienaar (2090878) domain_users (2000513)      555 2024-05-02 17:08:58.000000 spleendatads-2.0.2/tests/test_example.py
```

### Comparing `spleendatads-1.0.8/LICENSE` & `spleendatads-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spleendatads-1.0.8/PKG-INFO` & `spleendatads-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: spleendatads
-Version: 1.0.8
+Version: 2.0.2
 Summary: A ChRIS DS plugin to download a set of spleen data
 Home-page: https://github.com/FNNDSC/pl-spleendatads
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-License-File: LICENSE
-Requires-Dist: chris_plugin
 Provides-Extra: none
 Provides-Extra: dev
-Requires-Dist: pytest~=7.1; extra == "dev"
+License-File: LICENSE
 
 Spleen data downloader
 ======================
 
 |Version| |MIT License| |ci|
 
 ``pl-spleendatads`` is a `ChRIS <https://chrisproject.org/>`__ *DS*
@@ -45,16 +43,17 @@
 saving lots of space.
 
 You still need to download the whole set, however, before you can prune.
 
 Installation
 ------------
 
-``pl-spleendatads`` is a `ChRIS <https://chrisproject.org/>`__ *plugin*,
-meaning it can run from either within *ChRIS* or the command-line.
+``pl-spleendatads`` is a
+`ChRIS <https://chrisproject.org/>`__\ *plugin*, meaning it can run from
+either within *ChRIS* or the command-line.
 
 Local Usage
 -----------
 
 On the metal
 ~~~~~~~~~~~~
```

### Comparing `spleendatads-1.0.8/README.rst` & `spleendatads-2.0.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 saving lots of space.
 
 You still need to download the whole set, however, before you can prune.
 
 Installation
 ------------
 
-``pl-spleendatads`` is a `ChRIS <https://chrisproject.org/>`__ *plugin*,
-meaning it can run from either within *ChRIS* or the command-line.
+``pl-spleendatads`` is a
+`ChRIS <https://chrisproject.org/>`__\ *plugin*, meaning it can run from
+either within *ChRIS* or the command-line.
 
 Local Usage
 -----------
 
 On the metal
 ~~~~~~~~~~~~
```

### Comparing `spleendatads-1.0.8/setup.py` & `spleendatads-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `spleendatads-1.0.8/spleendatads.egg-info/PKG-INFO` & `spleendatads-2.0.2/spleendatads.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: spleendatads
-Version: 1.0.8
+Version: 2.0.2
 Summary: A ChRIS DS plugin to download a set of spleen data
 Home-page: https://github.com/FNNDSC/pl-spleendatads
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-License-File: LICENSE
-Requires-Dist: chris_plugin
 Provides-Extra: none
 Provides-Extra: dev
-Requires-Dist: pytest~=7.1; extra == "dev"
+License-File: LICENSE
 
 Spleen data downloader
 ======================
 
 |Version| |MIT License| |ci|
 
 ``pl-spleendatads`` is a `ChRIS <https://chrisproject.org/>`__ *DS*
@@ -45,16 +43,17 @@
 saving lots of space.
 
 You still need to download the whole set, however, before you can prune.
 
 Installation
 ------------
 
-``pl-spleendatads`` is a `ChRIS <https://chrisproject.org/>`__ *plugin*,
-meaning it can run from either within *ChRIS* or the command-line.
+``pl-spleendatads`` is a
+`ChRIS <https://chrisproject.org/>`__\ *plugin*, meaning it can run from
+either within *ChRIS* or the command-line.
 
 Local Usage
 -----------
 
 On the metal
 ~~~~~~~~~~~~
```

