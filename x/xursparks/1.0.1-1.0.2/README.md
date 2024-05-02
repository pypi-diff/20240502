# Comparing `tmp/xursparks-1.0.1.tar.gz` & `tmp/xursparks-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xursparks-1.0.1.tar", last modified: Mon Apr 15 03:32:33 2024, max compression
+gzip compressed data, was "xursparks-1.0.2.tar", last modified: Thu May  2 07:05:52 2024, max compression
```

## Comparing `xursparks-1.0.1.tar` & `xursparks-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-04-15 03:32:33.069271 xursparks-1.0.1/
--rw-rw-r--   0 doods     (1000) doods     (1000)     5835 2024-04-15 03:32:33.069271 xursparks-1.0.1/PKG-INFO
--rw-rw-r--   0 doods     (1000) doods     (1000)     5345 2024-04-03 04:21:12.000000 xursparks-1.0.1/README.md
--rw-rw-r--   0 doods     (1000) doods     (1000)       89 2024-04-05 01:26:52.000000 xursparks-1.0.1/pyproject.toml
--rw-rw-r--   0 doods     (1000) doods     (1000)       38 2024-04-15 03:32:33.069271 xursparks-1.0.1/setup.cfg
--rw-rw-r--   0 doods     (1000) doods     (1000)      650 2024-04-15 03:28:38.000000 xursparks-1.0.1/setup.py
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-04-15 03:32:33.069271 xursparks-1.0.1/xursparks.egg-info/
--rw-rw-r--   0 doods     (1000) doods     (1000)     5835 2024-04-15 03:32:33.000000 xursparks-1.0.1/xursparks.egg-info/PKG-INFO
--rw-rw-r--   0 doods     (1000) doods     (1000)      165 2024-04-15 03:32:33.000000 xursparks-1.0.1/xursparks.egg-info/SOURCES.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-04-15 03:32:33.000000 xursparks-1.0.1/xursparks.egg-info/dependency_links.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-04-15 03:32:33.000000 xursparks-1.0.1/xursparks.egg-info/top_level.txt
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-02 07:05:52.227546 xursparks-1.0.2/
+-rw-rw-r--   0 doods     (1000) doods     (1000)     5835 2024-05-02 07:05:52.227546 xursparks-1.0.2/PKG-INFO
+-rw-rw-r--   0 doods     (1000) doods     (1000)     5345 2024-04-03 04:21:12.000000 xursparks-1.0.2/README.md
+-rw-rw-r--   0 doods     (1000) doods     (1000)       89 2024-04-05 01:26:52.000000 xursparks-1.0.2/pyproject.toml
+-rw-rw-r--   0 doods     (1000) doods     (1000)       38 2024-05-02 07:05:52.227546 xursparks-1.0.2/setup.cfg
+-rw-rw-r--   0 doods     (1000) doods     (1000)      650 2024-05-02 07:04:54.000000 xursparks-1.0.2/setup.py
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-02 07:05:52.227546 xursparks-1.0.2/xursparks.egg-info/
+-rw-rw-r--   0 doods     (1000) doods     (1000)     5835 2024-05-02 07:05:52.000000 xursparks-1.0.2/xursparks.egg-info/PKG-INFO
+-rw-rw-r--   0 doods     (1000) doods     (1000)      165 2024-05-02 07:05:52.000000 xursparks-1.0.2/xursparks.egg-info/SOURCES.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-05-02 07:05:52.000000 xursparks-1.0.2/xursparks.egg-info/dependency_links.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-05-02 07:05:52.000000 xursparks-1.0.2/xursparks.egg-info/top_level.txt
```

### Comparing `xursparks-1.0.1/PKG-INFO` & `xursparks-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xursparks
-Version: 1.0.1
+Version: 1.0.2
 Summary: Encapsulating Apache Spark for easy usage
 Home-page: https://github.com/dev-doods687/xursparks
 Author: Randell Gabriel Santos
 Author-email: randellsantos@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xursparks-1.0.1/README.md` & `xursparks-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xursparks-1.0.1/setup.py` & `xursparks-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xursparks',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     author='Randell Gabriel Santos',
     author_email='randellsantos@gmail.com',
     description='Encapsulating Apache Spark for easy usage',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dev-doods687/xursparks',
```

### Comparing `xursparks-1.0.1/xursparks.egg-info/PKG-INFO` & `xursparks-1.0.2/xursparks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xursparks
-Version: 1.0.1
+Version: 1.0.2
 Summary: Encapsulating Apache Spark for easy usage
 Home-page: https://github.com/dev-doods687/xursparks
 Author: Randell Gabriel Santos
 Author-email: randellsantos@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

