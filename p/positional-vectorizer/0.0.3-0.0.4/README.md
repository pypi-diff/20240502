# Comparing `tmp/positional_vectorizer-0.0.3.tar.gz` & `tmp/positional_vectorizer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "positional_vectorizer-0.0.3.tar", last modified: Wed May  1 22:57:48 2024, max compression
+gzip compressed data, was "positional_vectorizer-0.0.4.tar", last modified: Wed May  1 23:14:23 2024, max compression
```

## Comparing `positional_vectorizer-0.0.3.tar` & `positional_vectorizer-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.238785 positional_vectorizer-0.0.3/
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/.mypy_cache/
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/.mypy_cache/3.11/
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/.mypy_cache/3.11/positional_vectorizer/
--rw-rw-r--   0 timotta   (1000) timotta   (1000)    13459 2024-05-01 19:42:33.000000 positional_vectorizer-0.0.3/.mypy_cache/3.11/positional_vectorizer/__init__.data.json
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     1624 2024-05-01 19:42:33.000000 positional_vectorizer-0.0.3/.mypy_cache/3.11/positional_vectorizer/__init__.meta.json
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     1431 2024-05-01 22:20:12.000000 positional_vectorizer-0.0.3/LICENSE
--rw-rw-r--   0 timotta   (1000) timotta   (1000)      115 2024-05-01 22:57:25.000000 positional_vectorizer-0.0.3/MANIFEST.in
--rw-r--r--   0 timotta   (1000) timotta   (1000)     3155 2024-05-01 22:57:48.238785 positional_vectorizer-0.0.3/PKG-INFO
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     2604 2024-05-01 22:16:28.000000 positional_vectorizer-0.0.3/README.md
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/dist/
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/dist/positional_vectorizer-0.0.2/
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/dist/positional_vectorizer-0.0.2/positional_vectorizer/
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     4308 2024-05-01 19:48:05.000000 positional_vectorizer-0.0.3/dist/positional_vectorizer-0.0.2/positional_vectorizer/__init__.py
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/positional_vectorizer/
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     4308 2024-05-01 19:48:05.000000 positional_vectorizer-0.0.3/positional_vectorizer/__init__.py
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/positional_vectorizer/__pycache__/
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     6034 2024-05-01 19:47:34.000000 positional_vectorizer-0.0.3/positional_vectorizer/__pycache__/__init__.cpython-311.pyc
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.238785 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/
--rw-r--r--   0 timotta   (1000) timotta   (1000)     3155 2024-05-01 22:57:47.000000 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/PKG-INFO
--rw-rw-r--   0 timotta   (1000) timotta   (1000)      599 2024-05-01 22:57:48.000000 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/SOURCES.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)        1 2024-05-01 22:57:47.000000 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/dependency_links.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)       20 2024-05-01 22:57:47.000000 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/requires.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)       22 2024-05-01 22:57:47.000000 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/top_level.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)       19 2024-04-30 23:59:15.000000 positional_vectorizer-0.0.3/requirements.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)       38 2024-05-01 22:57:48.238785 positional_vectorizer-0.0.3/setup.cfg
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     1364 2024-05-01 22:20:55.000000 positional_vectorizer-0.0.3/setup.py
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 23:14:23.076343 positional_vectorizer-0.0.4/
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 23:14:23.072343 positional_vectorizer-0.0.4/.mypy_cache/
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 23:14:23.072343 positional_vectorizer-0.0.4/.mypy_cache/3.11/
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 23:14:23.072343 positional_vectorizer-0.0.4/.mypy_cache/3.11/positional_vectorizer/
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)    13459 2024-05-01 19:42:33.000000 positional_vectorizer-0.0.4/.mypy_cache/3.11/positional_vectorizer/__init__.data.json
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     1624 2024-05-01 19:42:33.000000 positional_vectorizer-0.0.4/.mypy_cache/3.11/positional_vectorizer/__init__.meta.json
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     1431 2024-05-01 22:20:12.000000 positional_vectorizer-0.0.4/LICENSE
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)      131 2024-05-01 23:12:56.000000 positional_vectorizer-0.0.4/MANIFEST.in
+-rw-r--r--   0 timotta   (1000) timotta   (1000)     3155 2024-05-01 23:14:23.076343 positional_vectorizer-0.0.4/PKG-INFO
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     2604 2024-05-01 22:16:28.000000 positional_vectorizer-0.0.4/README.md
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)        6 2024-05-01 23:14:18.000000 positional_vectorizer-0.0.4/VERSION
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 23:14:23.072343 positional_vectorizer-0.0.4/positional_vectorizer/
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     4308 2024-05-01 19:48:05.000000 positional_vectorizer-0.0.4/positional_vectorizer/__init__.py
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 23:14:23.072343 positional_vectorizer-0.0.4/positional_vectorizer/__pycache__/
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     6034 2024-05-01 19:47:34.000000 positional_vectorizer-0.0.4/positional_vectorizer/__pycache__/__init__.cpython-311.pyc
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 23:14:23.076343 positional_vectorizer-0.0.4/positional_vectorizer.egg-info/
+-rw-r--r--   0 timotta   (1000) timotta   (1000)     3155 2024-05-01 23:14:22.000000 positional_vectorizer-0.0.4/positional_vectorizer.egg-info/PKG-INFO
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)      538 2024-05-01 23:14:23.000000 positional_vectorizer-0.0.4/positional_vectorizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)        1 2024-05-01 23:14:22.000000 positional_vectorizer-0.0.4/positional_vectorizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)       20 2024-05-01 23:14:22.000000 positional_vectorizer-0.0.4/positional_vectorizer.egg-info/requires.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)       22 2024-05-01 23:14:22.000000 positional_vectorizer-0.0.4/positional_vectorizer.egg-info/top_level.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)       19 2024-04-30 23:59:15.000000 positional_vectorizer-0.0.4/requirements.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)       38 2024-05-01 23:14:23.076343 positional_vectorizer-0.0.4/setup.cfg
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     1303 2024-05-01 23:13:17.000000 positional_vectorizer-0.0.4/setup.py
```

### Comparing `positional_vectorizer-0.0.3/.mypy_cache/3.11/positional_vectorizer/__init__.data.json` & `positional_vectorizer-0.0.4/.mypy_cache/3.11/positional_vectorizer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `positional_vectorizer-0.0.3/.mypy_cache/3.11/positional_vectorizer/__init__.meta.json` & `positional_vectorizer-0.0.4/.mypy_cache/3.11/positional_vectorizer/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `positional_vectorizer-0.0.3/LICENSE` & `positional_vectorizer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `positional_vectorizer-0.0.3/PKG-INFO` & `positional_vectorizer-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: positional-vectorizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Positional Vectorizer is a scikit-learn transformer that converts text to bag of words vector using a positional ranking algorithm as score
 Home-page: https://github.com/timotta/positional-vectorizer
 Author: Tiago Albineli Motta
 Author-email: timotta@gmail.com
 License: new BSD
 Keywords: machine learning,embedding,vectorizer,scikit-learn,text,NLP
 Requires-Python: >=3.11, <3.12
```

### Comparing `positional_vectorizer-0.0.3/README.md` & `positional_vectorizer-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `positional_vectorizer-0.0.3/dist/positional_vectorizer-0.0.2/positional_vectorizer/__init__.py` & `positional_vectorizer-0.0.4/positional_vectorizer/__init__.py`

 * *Files identical despite different names*

### Comparing `positional_vectorizer-0.0.3/positional_vectorizer/__pycache__/__init__.cpython-311.pyc` & `positional_vectorizer-0.0.4/positional_vectorizer/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `positional_vectorizer-0.0.3/positional_vectorizer.egg-info/PKG-INFO` & `positional_vectorizer-0.0.4/positional_vectorizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: positional-vectorizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Positional Vectorizer is a scikit-learn transformer that converts text to bag of words vector using a positional ranking algorithm as score
 Home-page: https://github.com/timotta/positional-vectorizer
 Author: Tiago Albineli Motta
 Author-email: timotta@gmail.com
 License: new BSD
 Keywords: machine learning,embedding,vectorizer,scikit-learn,text,NLP
 Requires-Python: >=3.11, <3.12
```

### Comparing `positional_vectorizer-0.0.3/setup.py` & `positional_vectorizer-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from os import environ
 from typing import List
 import setuptools
 
 
 def read_multiline_as_list(file_path: str) -> List[str]:
     with open(file_path) as fh:
         contents = fh.read().split("\n")
@@ -12,22 +11,19 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = read_multiline_as_list("requirements.txt")
 
-
-version = environ["POSITIONAL_VECTORIZER_VERSION"]
-
 setuptools.setup(
     name="positional-vectorizer",
-    version=version,
     author="Tiago Albineli Motta",
     author_email="timotta@gmail.com",
+    version=open("VERSION").read(),
     description="Positional Vectorizer is a scikit-learn transformer that converts text to bag of words vector using a positional ranking algorithm as score",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/timotta/positional-vectorizer",
     packages=setuptools.find_packages(
         include=["positional_vectorizer", "positional_vectorizer.*"]
     ),
```

