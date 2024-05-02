# Comparing `tmp/datewise-0.2.2.tar.gz` & `tmp/datewise-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datewise-0.2.2.tar", last modified: Thu Apr 18 20:31:11 2024, max compression
+gzip compressed data, was "datewise-1.0.0.tar", last modified: Thu May  2 17:40:39 2024, max compression
```

## Comparing `datewise-0.2.2.tar` & `datewise-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:11.683951 datewise-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-18 20:31:11.683951 datewise-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 20:30:52.000000 datewise-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:11.679951 datewise-0.2.2/datewise/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-18 20:30:52.000000 datewise-0.2.2/datewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-04-18 20:30:52.000000 datewise-0.2.2/datewise/datewise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:11.683951 datewise-0.2.2/datewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-18 20:31:11.000000 datewise-0.2.2/datewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-18 20:31:11.000000 datewise-0.2.2/datewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:31:11.000000 datewise-0.2.2/datewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 20:31:11.000000 datewise-0.2.2/datewise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:31:11.000000 datewise-0.2.2/datewise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:31:11.683951 datewise-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-18 20:30:52.000000 datewise-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:11.683951 datewise-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-04-18 20:30:52.000000 datewise-0.2.2/tests/test_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:40:39.036864 datewise-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-02 17:40:39.036864 datewise-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 17:40:20.000000 datewise-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:40:39.032864 datewise-1.0.0/datewise/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-02 17:40:20.000000 datewise-1.0.0/datewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-05-02 17:40:20.000000 datewise-1.0.0/datewise/datewise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:40:39.036864 datewise-1.0.0/datewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-02 17:40:39.000000 datewise-1.0.0/datewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-02 17:40:39.000000 datewise-1.0.0/datewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:40:39.000000 datewise-1.0.0/datewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 17:40:39.000000 datewise-1.0.0/datewise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 17:40:39.000000 datewise-1.0.0/datewise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:40:39.036864 datewise-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 17:40:20.000000 datewise-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:40:39.036864 datewise-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-05-02 17:40:20.000000 datewise-1.0.0/tests/test_functionality.py
```

### Comparing `datewise-0.2.2/PKG-INFO` & `datewise-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datewise
-Version: 0.2.2
+Version: 1.0.0
 Summary: Thesis Library
 Home-page: https://datewise.readthedocs.io/
 Author: Sebastian Gontkovic
 Author-email: sebascngont@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datewise-0.2.2/datewise/datewise.py` & `datewise-1.0.0/datewise/datewise.py`

 * *Files identical despite different names*

### Comparing `datewise-0.2.2/datewise.egg-info/PKG-INFO` & `datewise-1.0.0/datewise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datewise
-Version: 0.2.2
+Version: 1.0.0
 Summary: Thesis Library
 Home-page: https://datewise.readthedocs.io/
 Author: Sebastian Gontkovic
 Author-email: sebascngont@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datewise-0.2.2/setup.py` & `datewise-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-from setuptools import setup, find_packages
-from codecs import open
 from os import path
+from codecs import open
+from setuptools import setup, find_packages
 
-# The directory containing this file
-HERE = path.abspath(path.dirname(__file__))
+current_path = path.abspath(path.dirname(__file__))
 
-# Get the long description from the README file
-with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
+with open(path.join(current_path, 'README.md'), encoding='utf-8') as f:
+    desc = f.read()
 
-# This call to setup() does all the work
 setup(
     name="datewise",
-    version="0.2.2",
+    version="1.0.0",
     description="Thesis Library",
-    long_description=long_description,
+    long_description=desc,
     long_description_content_type="text/markdown",
     url="https://datewise.readthedocs.io/",
     author="Sebastian Gontkovic",
     author_email="sebascngont@gmail.com",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
```

### Comparing `datewise-0.2.2/tests/test_functionality.py` & `datewise-1.0.0/tests/test_functionality.py`

 * *Files identical despite different names*

