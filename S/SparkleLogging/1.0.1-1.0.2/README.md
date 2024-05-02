# Comparing `tmp/SparkleLogging-1.0.1.tar.gz` & `tmp/SparkleLogging-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleLogging-1.0.1.tar", last modified: Wed May  1 06:02:19 2024, max compression
+gzip compressed data, was "SparkleLogging-1.0.2.tar", last modified: Wed May  1 12:15:56 2024, max compression
```

## Comparing `SparkleLogging-1.0.1.tar` & `SparkleLogging-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 06:02:19.144002 SparkleLogging-1.0.1/
--rw-rw-rw-   0        0        0     2136 2024-05-01 06:02:19.143005 SparkleLogging-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 06:02:19.142008 SparkleLogging-1.0.1/SparkleLogging.egg-info/
--rw-rw-rw-   0        0        0     2136 2024-05-01 06:02:18.000000 SparkleLogging-1.0.1/SparkleLogging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2024-05-01 06:02:18.000000 SparkleLogging-1.0.1/SparkleLogging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 06:02:18.000000 SparkleLogging-1.0.1/SparkleLogging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-01 06:02:18.000000 SparkleLogging-1.0.1/SparkleLogging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-01 06:02:18.000000 SparkleLogging-1.0.1/SparkleLogging.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 06:02:19.113927 SparkleLogging-1.0.1/plugins/
--rw-rw-rw-   0        0        0      450 2024-02-21 07:45:12.000000 SparkleLogging-1.0.1/plugins/DecoratorsTools.py
--rw-rw-rw-   0        0        0     1160 2024-02-20 08:39:34.000000 SparkleLogging-1.0.1/plugins/HttpHander.py
--rw-rw-rw-   0        0        0        0 2024-02-20 09:06:56.000000 SparkleLogging-1.0.1/plugins/__init__.py
--rw-rw-rw-   0        0        0      954 2024-02-18 04:21:24.000000 SparkleLogging-1.0.1/plugins/websocketHander.py
--rw-rw-rw-   0        0        0       42 2024-05-01 06:02:19.144002 SparkleLogging-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      724 2024-05-01 06:02:05.000000 SparkleLogging-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:02:19.140014 SparkleLogging-1.0.1/utils/
--rw-rw-rw-   0        0        0        0 2024-04-30 09:33:18.000000 SparkleLogging-1.0.1/utils/__init__.py
--rw-rw-rw-   0        0        0       50 2024-05-01 05:44:49.000000 SparkleLogging-1.0.1/utils/core.py
--rw-rw-rw-   0        0        0     4761 2024-05-01 05:44:46.000000 SparkleLogging-1.0.1/utils/getLog.py
--rw-rw-rw-   0        0        0      372 2024-05-01 05:44:51.000000 SparkleLogging-1.0.1/utils/plugins_for_core.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:15:56.673143 SparkleLogging-1.0.2/
+-rw-rw-rw-   0        0        0     2136 2024-05-01 12:15:56.672172 SparkleLogging-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 12:15:56.647211 SparkleLogging-1.0.2/SparkleLogging/
+-rw-rw-rw-   0        0        0       21 2024-04-17 12:31:27.000000 SparkleLogging-1.0.2/SparkleLogging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:15:56.664165 SparkleLogging-1.0.2/SparkleLogging/plugins/
+-rw-rw-rw-   0        0        0      450 2024-02-21 07:45:12.000000 SparkleLogging-1.0.2/SparkleLogging/plugins/DecoratorsTools.py
+-rw-rw-rw-   0        0        0     1160 2024-02-20 08:39:34.000000 SparkleLogging-1.0.2/SparkleLogging/plugins/HttpHander.py
+-rw-rw-rw-   0        0        0        0 2024-02-20 09:06:56.000000 SparkleLogging-1.0.2/SparkleLogging/plugins/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-02-18 04:21:24.000000 SparkleLogging-1.0.2/SparkleLogging/plugins/websocketHander.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:15:56.669155 SparkleLogging-1.0.2/SparkleLogging/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-30 09:33:18.000000 SparkleLogging-1.0.2/SparkleLogging/utils/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-05-01 05:44:49.000000 SparkleLogging-1.0.2/SparkleLogging/utils/core.py
+-rw-rw-rw-   0        0        0     4761 2024-05-01 05:44:46.000000 SparkleLogging-1.0.2/SparkleLogging/utils/getLog.py
+-rw-rw-rw-   0        0        0      372 2024-05-01 05:44:51.000000 SparkleLogging-1.0.2/SparkleLogging/utils/plugins_for_core.py
+drwxrwxrwx   0        0        0        0 2024-05-01 12:15:56.670151 SparkleLogging-1.0.2/SparkleLogging.egg-info/
+-rw-rw-rw-   0        0        0     2136 2024-05-01 12:15:56.000000 SparkleLogging-1.0.2/SparkleLogging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-05-01 12:15:56.000000 SparkleLogging-1.0.2/SparkleLogging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 12:15:56.000000 SparkleLogging-1.0.2/SparkleLogging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-01 12:15:56.000000 SparkleLogging-1.0.2/SparkleLogging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-01 12:15:56.000000 SparkleLogging-1.0.2/SparkleLogging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 12:15:56.673143 SparkleLogging-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      724 2024-05-01 12:15:53.000000 SparkleLogging-1.0.2/setup.py
```

### Comparing `SparkleLogging-1.0.1/PKG-INFO` & `SparkleLogging-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.1
+Version: 1.0.2
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SparkleLogging-1.0.1/SparkleLogging.egg-info/PKG-INFO` & `SparkleLogging-1.0.2/SparkleLogging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.1
+Version: 1.0.2
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SparkleLogging-1.0.1/plugins/HttpHander.py` & `SparkleLogging-1.0.2/SparkleLogging/plugins/HttpHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.1/plugins/websocketHander.py` & `SparkleLogging-1.0.2/SparkleLogging/plugins/websocketHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.1/setup.py` & `SparkleLogging-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SparkleLogging',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     author='花火official',
     author_email='3072252442@qq.com',
     description='A logging library for Python',
     long_description=open('Readme.md','r',encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KOKOMI12345/SparkleLogging',
```

### Comparing `SparkleLogging-1.0.1/utils/getLog.py` & `SparkleLogging-1.0.2/SparkleLogging/utils/getLog.py`

 * *Files identical despite different names*

