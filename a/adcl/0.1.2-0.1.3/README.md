# Comparing `tmp/adcl-0.1.2.tar.gz` & `tmp/adcl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\adcl-0.1.2.tar", last modified: Thu May  2 06:46:32 2024, max compression
+gzip compressed data, was "dist\adcl-0.1.3.tar", last modified: Thu May  2 06:51:28 2024, max compression
```

## Comparing `adcl-0.1.2.tar` & `adcl-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 06:46:32.000000 adcl-0.1.2/
--rw-rw-rw-   0        0        0     1091 2024-05-01 20:17:28.000000 adcl-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4292 2024-05-02 06:46:32.000000 adcl-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3754 2024-05-01 20:17:28.000000 adcl-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 06:46:32.000000 adcl-0.1.2/adcl/
--rw-rw-rw-   0        0        0       35 2024-05-01 20:17:28.000000 adcl-0.1.2/adcl/__init__.py
--rw-rw-rw-   0        0        0    53906 2024-05-01 20:17:28.000000 adcl-0.1.2/adcl/data_preprocessing.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:46:32.000000 adcl-0.1.2/adcl.egg-info/
--rw-rw-rw-   0        0        0     4292 2024-05-02 06:46:32.000000 adcl-0.1.2/adcl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-05-02 06:46:32.000000 adcl-0.1.2/adcl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 06:46:32.000000 adcl-0.1.2/adcl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      226 2024-05-02 06:46:32.000000 adcl-0.1.2/adcl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-02 06:46:32.000000 adcl-0.1.2/adcl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 06:46:32.000000 adcl-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1020 2024-05-02 06:46:14.000000 adcl-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:51:28.000000 adcl-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2024-05-01 20:17:28.000000 adcl-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4292 2024-05-02 06:51:28.000000 adcl-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3754 2024-05-01 20:17:28.000000 adcl-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 06:51:28.000000 adcl-0.1.3/adcl/
+-rw-rw-rw-   0        0        0       35 2024-05-01 20:17:28.000000 adcl-0.1.3/adcl/__init__.py
+-rw-rw-rw-   0        0        0    53906 2024-05-01 20:17:28.000000 adcl-0.1.3/adcl/data_preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:51:28.000000 adcl-0.1.3/adcl.egg-info/
+-rw-rw-rw-   0        0        0     4292 2024-05-02 06:51:28.000000 adcl-0.1.3/adcl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-02 06:51:28.000000 adcl-0.1.3/adcl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 06:51:28.000000 adcl-0.1.3/adcl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      234 2024-05-02 06:51:28.000000 adcl-0.1.3/adcl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-02 06:51:28.000000 adcl-0.1.3/adcl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 06:51:28.000000 adcl-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1029 2024-05-02 06:51:06.000000 adcl-0.1.3/setup.py
```

### Comparing `adcl-0.1.2/LICENSE` & `adcl-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adcl-0.1.2/PKG-INFO` & `adcl-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adcl
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data preprocessing and cleaning tools for data science projects
 Home-page: https://github.com/maykov-stepan/ADCL-Automatic-Data-Cleaning
 Author: Maykov Stepan
 Author-email: steve19992@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adcl-0.1.2/README.md` & `adcl-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `adcl-0.1.2/adcl/data_preprocessing.py` & `adcl-0.1.3/adcl/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `adcl-0.1.2/adcl.egg-info/PKG-INFO` & `adcl-0.1.3/adcl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adcl
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data preprocessing and cleaning tools for data science projects
 Home-page: https://github.com/maykov-stepan/ADCL-Automatic-Data-Cleaning
 Author: Maykov Stepan
 Author-email: steve19992@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adcl-0.1.2/setup.py` & `adcl-0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='adcl',
-    version='0.1.2',
+    version='0.1.3',
     author='Maykov Stepan',
     author_email='steve19992@mail.ru',
     description='Data preprocessing and cleaning tools for data science projects',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/maykov-stepan/ADCL-Automatic-Data-Cleaning',
     packages=find_packages(),
     install_requires=[
-    'numpy>=1.21.6',
+    'numpy>=1.15.0, <1.17.0',
     'pandas>=1.0.5,<=1.3.5',
     'tensorflow>=2.11.0',
     'mxnet>=1.4.0',
     'openml>=0.14.1',
     'scipy>=1.5.4',
     'dtaidistance>=2.3.11',
     'matrixprofile>=1.1.10',
```

