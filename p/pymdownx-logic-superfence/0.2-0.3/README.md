# Comparing `tmp/pymdownx-logic-superfence-0.2.tar.gz` & `tmp/pymdownx-logic-superfence-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymdownx-logic-superfence-0.2.tar", last modified: Thu May  2 08:56:34 2024, max compression
+gzip compressed data, was "pymdownx-logic-superfence-0.3.tar", last modified: Thu May  2 09:36:49 2024, max compression
```

## Comparing `pymdownx-logic-superfence-0.2.tar` & `pymdownx-logic-superfence-0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 davy      (1000) davy      (1000)        0 2024-05-02 08:56:34.625136 pymdownx-logic-superfence-0.2/
--rw-rw-r--   0 davy      (1000) davy      (1000)    35150 2024-05-02 08:24:14.000000 pymdownx-logic-superfence-0.2/COPYING
--rw-rw-r--   0 davy      (1000) davy      (1000)      424 2024-05-02 08:56:34.625136 pymdownx-logic-superfence-0.2/PKG-INFO
-drwxrwxr-x   0 davy      (1000) davy      (1000)        0 2024-05-02 08:56:34.625136 pymdownx-logic-superfence-0.2/pymdownx_logic_superfence.egg-info/
--rw-rw-r--   0 davy      (1000) davy      (1000)      424 2024-05-02 08:56:34.000000 pymdownx-logic-superfence-0.2/pymdownx_logic_superfence.egg-info/PKG-INFO
--rw-rw-r--   0 davy      (1000) davy      (1000)      212 2024-05-02 08:56:34.000000 pymdownx-logic-superfence-0.2/pymdownx_logic_superfence.egg-info/SOURCES.txt
--rw-rw-r--   0 davy      (1000) davy      (1000)        1 2024-05-02 08:56:34.000000 pymdownx-logic-superfence-0.2/pymdownx_logic_superfence.egg-info/dependency_links.txt
--rw-rw-r--   0 davy      (1000) davy      (1000)        1 2024-05-02 08:56:34.000000 pymdownx-logic-superfence-0.2/pymdownx_logic_superfence.egg-info/top_level.txt
--rw-rw-r--   0 davy      (1000) davy      (1000)       38 2024-05-02 08:56:34.625136 pymdownx-logic-superfence-0.2/setup.cfg
--rw-rw-r--   0 davy      (1000) davy      (1000)      521 2024-05-02 08:56:25.000000 pymdownx-logic-superfence-0.2/setup.py
+drwxrwxr-x   0 davy      (1000) davy      (1000)        0 2024-05-02 09:36:49.733471 pymdownx-logic-superfence-0.3/
+-rw-rw-r--   0 davy      (1000) davy      (1000)    35150 2024-05-02 08:24:14.000000 pymdownx-logic-superfence-0.3/COPYING
+-rw-rw-r--   0 davy      (1000) davy      (1000)      424 2024-05-02 09:36:49.733471 pymdownx-logic-superfence-0.3/PKG-INFO
+drwxrwxr-x   0 davy      (1000) davy      (1000)        0 2024-05-02 09:36:49.733471 pymdownx-logic-superfence-0.3/pymdownx_logic_superfence.egg-info/
+-rw-rw-r--   0 davy      (1000) davy      (1000)      424 2024-05-02 09:36:49.000000 pymdownx-logic-superfence-0.3/pymdownx_logic_superfence.egg-info/PKG-INFO
+-rw-rw-r--   0 davy      (1000) davy      (1000)      212 2024-05-02 09:36:49.000000 pymdownx-logic-superfence-0.3/pymdownx_logic_superfence.egg-info/SOURCES.txt
+-rw-rw-r--   0 davy      (1000) davy      (1000)        1 2024-05-02 09:36:49.000000 pymdownx-logic-superfence-0.3/pymdownx_logic_superfence.egg-info/dependency_links.txt
+-rw-rw-r--   0 davy      (1000) davy      (1000)        1 2024-05-02 09:36:49.000000 pymdownx-logic-superfence-0.3/pymdownx_logic_superfence.egg-info/top_level.txt
+-rw-rw-r--   0 davy      (1000) davy      (1000)       38 2024-05-02 09:36:49.733471 pymdownx-logic-superfence-0.3/setup.cfg
+-rw-rw-r--   0 davy      (1000) davy      (1000)      521 2024-05-02 09:36:43.000000 pymdownx-logic-superfence-0.3/setup.py
```

### Comparing `pymdownx-logic-superfence-0.2/COPYING` & `pymdownx-logic-superfence-0.3/COPYING`

 * *Files identical despite different names*

### Comparing `pymdownx-logic-superfence-0.2/setup.py` & `pymdownx-logic-superfence-0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pymdownx-logic-superfence',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     author='Davy Cottet',
     description='A superfence pymarkdown extension for logic circuit simulator',
     url='https://gitlab.com/davy39/logic-superfence',
     license='GNU General Public License v3.0',
     platforms=['Any'],
     classifiers=[
```

