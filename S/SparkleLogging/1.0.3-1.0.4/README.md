# Comparing `tmp/SparkleLogging-1.0.3.tar.gz` & `tmp/SparkleLogging-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleLogging-1.0.3.tar", last modified: Thu May  2 12:12:19 2024, max compression
+gzip compressed data, was "SparkleLogging-1.0.4.tar", last modified: Thu May  2 17:09:03 2024, max compression
```

## Comparing `SparkleLogging-1.0.3.tar` & `SparkleLogging-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 12:12:18.920859 SparkleLogging-1.0.3/
--rw-rw-rw-   0        0        0     2838 2024-05-02 12:12:18.918864 SparkleLogging-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 12:12:18.817911 SparkleLogging-1.0.3/SparkleLogging/
--rw-rw-rw-   0        0        0        0 2024-05-01 12:32:10.000000 SparkleLogging-1.0.3/SparkleLogging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:12:18.907894 SparkleLogging-1.0.3/SparkleLogging/plugins/
--rw-rw-rw-   0        0        0      450 2024-02-21 07:45:12.000000 SparkleLogging-1.0.3/SparkleLogging/plugins/DecoratorsTools.py
--rw-rw-rw-   0        0        0     1160 2024-02-20 08:39:34.000000 SparkleLogging-1.0.3/SparkleLogging/plugins/HttpHander.py
--rw-rw-rw-   0        0        0        0 2024-02-20 09:06:56.000000 SparkleLogging-1.0.3/SparkleLogging/plugins/__init__.py
--rw-rw-rw-   0        0        0      954 2024-02-18 04:21:24.000000 SparkleLogging-1.0.3/SparkleLogging/plugins/websocketHander.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:12:18.914875 SparkleLogging-1.0.3/SparkleLogging/utils/
--rw-rw-rw-   0        0        0        0 2024-04-30 09:33:18.000000 SparkleLogging-1.0.3/SparkleLogging/utils/__init__.py
--rw-rw-rw-   0        0        0       50 2024-05-01 05:44:49.000000 SparkleLogging-1.0.3/SparkleLogging/utils/core.py
--rw-rw-rw-   0        0        0     4991 2024-05-02 12:07:21.000000 SparkleLogging-1.0.3/SparkleLogging/utils/getLog.py
--rw-rw-rw-   0        0        0      372 2024-05-01 05:44:51.000000 SparkleLogging-1.0.3/SparkleLogging/utils/plugins_for_core.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:12:18.916869 SparkleLogging-1.0.3/SparkleLogging.egg-info/
--rw-rw-rw-   0        0        0     2838 2024-05-02 12:12:16.000000 SparkleLogging-1.0.3/SparkleLogging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-05-02 12:12:16.000000 SparkleLogging-1.0.3/SparkleLogging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 12:12:16.000000 SparkleLogging-1.0.3/SparkleLogging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-02 12:12:16.000000 SparkleLogging-1.0.3/SparkleLogging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-02 12:12:16.000000 SparkleLogging-1.0.3/SparkleLogging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 12:12:18.920859 SparkleLogging-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      724 2024-05-02 12:10:40.000000 SparkleLogging-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:09:03.607595 SparkleLogging-1.0.4/
+-rw-rw-rw-   0        0        0     2897 2024-05-02 17:09:03.606598 SparkleLogging-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 17:09:03.515297 SparkleLogging-1.0.4/SparkleLogging/
+-rw-rw-rw-   0        0        0        0 2024-05-01 12:32:10.000000 SparkleLogging-1.0.4/SparkleLogging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:09:03.598622 SparkleLogging-1.0.4/SparkleLogging/plugins/
+-rw-rw-rw-   0        0        0      450 2024-02-21 07:45:12.000000 SparkleLogging-1.0.4/SparkleLogging/plugins/DecoratorsTools.py
+-rw-rw-rw-   0        0        0     1160 2024-02-20 08:39:34.000000 SparkleLogging-1.0.4/SparkleLogging/plugins/HttpHander.py
+-rw-rw-rw-   0        0        0        0 2024-02-20 09:06:56.000000 SparkleLogging-1.0.4/SparkleLogging/plugins/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-02-18 04:21:24.000000 SparkleLogging-1.0.4/SparkleLogging/plugins/websocketHander.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:09:03.603608 SparkleLogging-1.0.4/SparkleLogging/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-30 09:33:18.000000 SparkleLogging-1.0.4/SparkleLogging/utils/__init__.py
+-rw-rw-rw-   0        0        0      445 2024-05-02 17:04:22.000000 SparkleLogging-1.0.4/SparkleLogging/utils/core.py
+-rw-rw-rw-   0        0        0     4991 2024-05-02 12:07:21.000000 SparkleLogging-1.0.4/SparkleLogging/utils/getLog.py
+-rw-rw-rw-   0        0        0      372 2024-05-01 05:44:51.000000 SparkleLogging-1.0.4/SparkleLogging/utils/plugins_for_core.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:09:03.604606 SparkleLogging-1.0.4/SparkleLogging.egg-info/
+-rw-rw-rw-   0        0        0     2897 2024-05-02 17:09:02.000000 SparkleLogging-1.0.4/SparkleLogging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-05-02 17:09:02.000000 SparkleLogging-1.0.4/SparkleLogging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 17:09:02.000000 SparkleLogging-1.0.4/SparkleLogging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-02 17:09:02.000000 SparkleLogging-1.0.4/SparkleLogging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-02 17:09:02.000000 SparkleLogging-1.0.4/SparkleLogging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 17:09:03.607595 SparkleLogging-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      724 2024-05-02 17:04:39.000000 SparkleLogging-1.0.4/setup.py
```

### Comparing `SparkleLogging-1.0.3/PKG-INFO` & `SparkleLogging-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.3
+Version: 1.0.4
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -74,7 +74,11 @@
 
 - `custom_formatter`: 自定义格式化函数,默认None
 - `setConsoleLevel`: 设置控制台日志输出级别,默认DEBUG
 - `setFileLevel`: 设置文件日志输出级别,默认INFO
 - `setWebLevel`: 设置websocket日志输出级别,默认INFO
 - `setHttpLevel`: 设置http日志输出级别,默认INFO
 - `custom_fomatter`: 自定义格式化函数,默认None
+
+# 2024/5/3 1:05
+
+更新了一个默认日志记录器
```

### Comparing `SparkleLogging-1.0.3/SparkleLogging/plugins/HttpHander.py` & `SparkleLogging-1.0.4/SparkleLogging/plugins/HttpHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.3/SparkleLogging/plugins/websocketHander.py` & `SparkleLogging-1.0.4/SparkleLogging/plugins/websocketHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.3/SparkleLogging/utils/getLog.py` & `SparkleLogging-1.0.4/SparkleLogging/utils/getLog.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.3/SparkleLogging.egg-info/PKG-INFO` & `SparkleLogging-1.0.4/SparkleLogging.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.3
+Version: 1.0.4
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -74,7 +74,11 @@
 
 - `custom_formatter`: 自定义格式化函数,默认None
 - `setConsoleLevel`: 设置控制台日志输出级别,默认DEBUG
 - `setFileLevel`: 设置文件日志输出级别,默认INFO
 - `setWebLevel`: 设置websocket日志输出级别,默认INFO
 - `setHttpLevel`: 设置http日志输出级别,默认INFO
 - `custom_fomatter`: 自定义格式化函数,默认None
+
+# 2024/5/3 1:05
+
+更新了一个默认日志记录器
```

### Comparing `SparkleLogging-1.0.3/SparkleLogging.egg-info/SOURCES.txt` & `SparkleLogging-1.0.4/SparkleLogging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.3/setup.py` & `SparkleLogging-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SparkleLogging',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     author='花火official',
     author_email='3072252442@qq.com',
     description='A logging library for Python',
     long_description=open('Readme.md','r',encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KOKOMI12345/SparkleLogging',
```

