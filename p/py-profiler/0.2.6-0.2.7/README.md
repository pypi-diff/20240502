# Comparing `tmp/py_profiler-0.2.6.tar.gz` & `tmp/py_profiler-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_profiler-0.2.6.tar", last modified: Fri Mar 15 15:56:16 2024, max compression
+gzip compressed data, was "py_profiler-0.2.7.tar", last modified: Thu May  2 10:59:53 2024, max compression
```

## Comparing `py_profiler-0.2.6.tar` & `py_profiler-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-03-15 15:56:16.512001 py_profiler-0.2.6/
--rw-r--r--   0 andy       (501) staff       (20)     1073 2023-02-02 15:54:28.000000 py_profiler-0.2.6/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)       50 2023-02-02 15:54:28.000000 py_profiler-0.2.6/MANIFEST.in
--rw-r--r--   0 andy       (501) staff       (20)     3702 2024-03-15 15:56:16.511748 py_profiler-0.2.6/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     3120 2024-03-14 09:41:54.000000 py_profiler-0.2.6/README.md
--rw-r--r--   0 andy       (501) staff       (20)      126 2023-02-02 15:54:28.000000 py_profiler-0.2.6/pyproject.toml
--rw-r--r--   0 andy       (501) staff       (20)       38 2024-03-15 15:56:16.512055 py_profiler-0.2.6/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)      911 2024-03-15 15:56:03.000000 py_profiler-0.2.6/setup.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-03-15 15:56:16.507237 py_profiler-0.2.6/src/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-03-15 15:56:16.510067 py_profiler-0.2.6/src/py_profiler/
--rw-r--r--   0 andy       (501) staff       (20)       79 2023-02-02 15:54:28.000000 py_profiler-0.2.6/src/py_profiler/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1026 2023-02-02 15:54:28.000000 py_profiler-0.2.6/src/py_profiler/decorator.py
--rw-r--r--   0 andy       (501) staff       (20)      330 2024-03-15 15:55:53.000000 py_profiler-0.2.6/src/py_profiler/fastapi_profiler_controller.py
--rw-r--r--   0 andy       (501) staff       (20)      522 2023-02-02 15:54:28.000000 py_profiler-0.2.6/src/py_profiler/long_adder.py
--rw-r--r--   0 andy       (501) staff       (20)     5555 2024-03-14 09:41:54.000000 py_profiler-0.2.6/src/py_profiler/measure_service.py
--rw-r--r--   0 andy       (501) staff       (20)      260 2024-03-14 09:41:54.000000 py_profiler-0.2.6/src/py_profiler/profiler_controller.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-03-15 15:56:16.510993 py_profiler-0.2.6/src/py_profiler/templates/
--rw-r--r--   0 andy       (501) staff       (20)     3308 2024-03-14 09:35:36.000000 py_profiler-0.2.6/src/py_profiler/templates/profiler.html
--rw-r--r--   0 andy       (501) staff       (20)      743 2023-02-02 15:54:28.000000 py_profiler-0.2.6/src/py_profiler/utils.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-03-15 15:56:16.511476 py_profiler-0.2.6/src/py_profiler.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)     3702 2024-03-15 15:56:16.000000 py_profiler-0.2.6/src/py_profiler.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      520 2024-03-15 15:56:16.000000 py_profiler-0.2.6/src/py_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-03-15 15:56:16.000000 py_profiler-0.2.6/src/py_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       22 2024-03-15 15:56:16.000000 py_profiler-0.2.6/src/py_profiler.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)       12 2024-03-15 15:56:16.000000 py_profiler-0.2.6/src/py_profiler.egg-info/top_level.txt
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 10:59:53.651219 py_profiler-0.2.7/
+-rw-r--r--   0 andy       (501) staff       (20)     1073 2023-02-02 15:54:28.000000 py_profiler-0.2.7/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)       50 2023-02-02 15:54:28.000000 py_profiler-0.2.7/MANIFEST.in
+-rw-r--r--   0 andy       (501) staff       (20)     3702 2024-05-02 10:59:53.650935 py_profiler-0.2.7/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     3120 2024-03-14 09:41:54.000000 py_profiler-0.2.7/README.md
+-rw-r--r--   0 andy       (501) staff       (20)      126 2023-02-02 15:54:28.000000 py_profiler-0.2.7/pyproject.toml
+-rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-02 10:59:53.651274 py_profiler-0.2.7/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)      911 2024-05-02 05:32:12.000000 py_profiler-0.2.7/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 10:59:53.645250 py_profiler-0.2.7/src/
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 10:59:53.649043 py_profiler-0.2.7/src/py_profiler/
+-rw-r--r--   0 andy       (501) staff       (20)       79 2023-02-02 15:54:28.000000 py_profiler-0.2.7/src/py_profiler/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     1026 2023-02-02 15:54:28.000000 py_profiler-0.2.7/src/py_profiler/decorator.py
+-rw-r--r--   0 andy       (501) staff       (20)      330 2024-03-15 15:55:53.000000 py_profiler-0.2.7/src/py_profiler/fastapi_profiler_controller.py
+-rw-r--r--   0 andy       (501) staff       (20)      522 2023-02-02 15:54:28.000000 py_profiler-0.2.7/src/py_profiler/long_adder.py
+-rw-r--r--   0 andy       (501) staff       (20)     5555 2024-03-14 09:41:54.000000 py_profiler-0.2.7/src/py_profiler/measure_service.py
+-rw-r--r--   0 andy       (501) staff       (20)      260 2024-03-14 09:41:54.000000 py_profiler-0.2.7/src/py_profiler/profiler_controller.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 10:59:53.650158 py_profiler-0.2.7/src/py_profiler/templates/
+-rw-r--r--   0 andy       (501) staff       (20)     3308 2024-03-14 09:35:36.000000 py_profiler-0.2.7/src/py_profiler/templates/profiler.html
+-rw-r--r--   0 andy       (501) staff       (20)      743 2023-02-02 15:54:28.000000 py_profiler-0.2.7/src/py_profiler/utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 10:59:53.650624 py_profiler-0.2.7/src/py_profiler.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)     3702 2024-05-02 10:59:53.000000 py_profiler-0.2.7/src/py_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      520 2024-05-02 10:59:53.000000 py_profiler-0.2.7/src/py_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-02 10:59:53.000000 py_profiler-0.2.7/src/py_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       22 2024-05-02 10:59:53.000000 py_profiler-0.2.7/src/py_profiler.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)       12 2024-05-02 10:59:53.000000 py_profiler-0.2.7/src/py_profiler.egg-info/top_level.txt
```

### Comparing `py_profiler-0.2.6/LICENSE` & `py_profiler-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.6/PKG-INFO` & `py_profiler-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_profiler
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library to measure your method, function execution time.
 Home-page: https://github.com/andy1xx8/py-profiler
 Author: Andy Le
 Author-email: tauit.dnmd@gmail.com
 Project-URL: Bug Tracker, https://github.com/andy1xx8/py-profiler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py_profiler-0.2.6/README.md` & `py_profiler-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.6/setup.py` & `py_profiler-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_profiler",
-    version="0.2.6",
+    version="0.2.7",
     author="Andy Le",
     author_email="tauit.dnmd@gmail.com",
     description="A library to measure your method, function execution time.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andy1xx8/py-profiler",
     project_urls={
```

### Comparing `py_profiler-0.2.6/src/py_profiler/decorator.py` & `py_profiler-0.2.7/src/py_profiler/decorator.py`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.6/src/py_profiler/long_adder.py` & `py_profiler-0.2.7/src/py_profiler/long_adder.py`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.6/src/py_profiler/measure_service.py` & `py_profiler-0.2.7/src/py_profiler/measure_service.py`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.6/src/py_profiler/templates/profiler.html` & `py_profiler-0.2.7/src/py_profiler/templates/profiler.html`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.6/src/py_profiler/utils.py` & `py_profiler-0.2.7/src/py_profiler/utils.py`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.6/src/py_profiler.egg-info/PKG-INFO` & `py_profiler-0.2.7/src/py_profiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_profiler
-Version: 0.2.6
+Version: 0.2.7
 Summary: A library to measure your method, function execution time.
 Home-page: https://github.com/andy1xx8/py-profiler
 Author: Andy Le
 Author-email: tauit.dnmd@gmail.com
 Project-URL: Bug Tracker, https://github.com/andy1xx8/py-profiler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py_profiler-0.2.6/src/py_profiler.egg-info/SOURCES.txt` & `py_profiler-0.2.7/src/py_profiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

