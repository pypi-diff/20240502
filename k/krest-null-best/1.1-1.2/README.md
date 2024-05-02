# Comparing `tmp/krest_null_best-1.1.tar.gz` & `tmp/krest_null_best-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krest_null_best-1.1.tar", last modified: Wed May  1 17:52:31 2024, max compression
+gzip compressed data, was "krest_null_best-1.2.tar", last modified: Wed May  1 18:21:15 2024, max compression
```

## Comparing `krest_null_best-1.1.tar` & `krest_null_best-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 17:52:31.334349 krest_null_best-1.1/
--rw-rw-rw-   0        0        0     1091 2024-05-01 15:18:02.000000 krest_null_best-1.1/LICENSE
--rw-rw-rw-   0        0        0      553 2024-05-01 17:52:31.334349 krest_null_best-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-05-01 17:51:00.000000 krest_null_best-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 17:52:31.334349 krest_null_best-1.1/krest_null_best.egg-info/
--rw-rw-rw-   0        0        0      553 2024-05-01 17:52:30.000000 krest_null_best-1.1/krest_null_best.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2024-05-01 17:52:31.000000 krest_null_best-1.1/krest_null_best.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 17:52:30.000000 krest_null_best-1.1/krest_null_best.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-01 17:52:30.000000 krest_null_best-1.1/krest_null_best.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-01 17:52:30.000000 krest_null_best-1.1/krest_null_best.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 17:52:31.325333 krest_null_best-1.1/package/
--rw-rw-rw-   0        0        0        0 2024-05-01 15:10:27.000000 krest_null_best-1.1/package/__init__.py
--rw-rw-rw-   0        0        0     2196 2024-05-01 17:44:53.000000 krest_null_best-1.1/package/example.py
--rw-rw-rw-   0        0        0       42 2024-05-01 17:52:31.334349 krest_null_best-1.1/setup.cfg
--rw-rw-rw-   0        0        0      737 2024-05-01 17:51:57.000000 krest_null_best-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 18:21:15.986801 krest_null_best-1.2/
+-rw-rw-rw-   0        0        0     1091 2024-05-01 15:18:02.000000 krest_null_best-1.2/LICENSE
+-rw-rw-rw-   0        0        0      553 2024-05-01 18:21:15.986801 krest_null_best-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-05-01 17:51:00.000000 krest_null_best-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 18:21:15.986801 krest_null_best-1.2/krest_null_best.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-05-01 18:21:15.000000 krest_null_best-1.2/krest_null_best.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-05-01 18:21:15.000000 krest_null_best-1.2/krest_null_best.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 18:21:15.000000 krest_null_best-1.2/krest_null_best.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-01 18:21:15.000000 krest_null_best-1.2/krest_null_best.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-01 18:21:15.000000 krest_null_best-1.2/krest_null_best.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 18:21:15.986801 krest_null_best-1.2/package/
+-rw-rw-rw-   0        0        0        0 2024-05-01 15:10:27.000000 krest_null_best-1.2/package/__init__.py
+-rw-rw-rw-   0        0        0     2196 2024-05-01 17:44:53.000000 krest_null_best-1.2/package/example.py
+-rw-rw-rw-   0        0        0       42 2024-05-01 18:21:15.986801 krest_null_best-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      737 2024-05-01 18:20:49.000000 krest_null_best-1.2/setup.py
```

### Comparing `krest_null_best-1.1/LICENSE` & `krest_null_best-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `krest_null_best-1.1/PKG-INFO` & `krest_null_best-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krest_null_best
-Version: 1.1
+Version: 1.2
 Summary: BEST
 Home-page: https://pypi.org/krest_null_best
 Author: Python_Palma
 Author-email: admin@gmail.com
 Project-URL: Documentation, https://pypi.org/
 Keywords: Snake,python
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `krest_null_best-1.1/krest_null_best.egg-info/PKG-INFO` & `krest_null_best-1.2/krest_null_best.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krest_null_best
-Version: 1.1
+Version: 1.2
 Summary: BEST
 Home-page: https://pypi.org/krest_null_best
 Author: Python_Palma
 Author-email: admin@gmail.com
 Project-URL: Documentation, https://pypi.org/
 Keywords: Snake,python
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `krest_null_best-1.1/package/example.py` & `krest_null_best-1.2/package/example.py`

 * *Files identical despite different names*

### Comparing `krest_null_best-1.1/setup.py` & `krest_null_best-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='krest_null_best',
-  version='1.1',
+  version='1.2',
   author='Python_Palma',
   author_email='admin@gmail.com',
   description='BEST',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://pypi.org/krest_null_best',
   packages=find_packages(),
```

