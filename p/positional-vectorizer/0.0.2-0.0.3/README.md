# Comparing `tmp/positional_vectorizer-0.0.2.tar.gz` & `tmp/positional_vectorizer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "positional_vectorizer-0.0.2.tar", last modified: Wed May  1 22:51:19 2024, max compression
+gzip compressed data, was "positional_vectorizer-0.0.3.tar", last modified: Wed May  1 22:57:48 2024, max compression
```

## Comparing `positional_vectorizer-0.0.2.tar` & `positional_vectorizer-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,27 @@
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:51:19.134105 positional_vectorizer-0.0.2/
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     1431 2024-05-01 22:20:12.000000 positional_vectorizer-0.0.2/LICENSE
--rw-r--r--   0 timotta   (1000) timotta   (1000)     3155 2024-05-01 22:51:19.134105 positional_vectorizer-0.0.2/PKG-INFO
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     2604 2024-05-01 22:16:28.000000 positional_vectorizer-0.0.2/README.md
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:51:19.134105 positional_vectorizer-0.0.2/positional_vectorizer/
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     4308 2024-05-01 19:48:05.000000 positional_vectorizer-0.0.2/positional_vectorizer/__init__.py
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:51:19.134105 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/
--rw-r--r--   0 timotta   (1000) timotta   (1000)     3155 2024-05-01 22:51:19.000000 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/PKG-INFO
--rw-rw-r--   0 timotta   (1000) timotta   (1000)      284 2024-05-01 22:51:19.000000 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/SOURCES.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)        1 2024-05-01 22:51:19.000000 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/dependency_links.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)       20 2024-05-01 22:51:19.000000 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/requires.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)       22 2024-05-01 22:51:19.000000 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/top_level.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)       38 2024-05-01 22:51:19.134105 positional_vectorizer-0.0.2/setup.cfg
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     1364 2024-05-01 22:20:55.000000 positional_vectorizer-0.0.2/setup.py
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.238785 positional_vectorizer-0.0.3/
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/.mypy_cache/
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/.mypy_cache/3.11/
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/.mypy_cache/3.11/positional_vectorizer/
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)    13459 2024-05-01 19:42:33.000000 positional_vectorizer-0.0.3/.mypy_cache/3.11/positional_vectorizer/__init__.data.json
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     1624 2024-05-01 19:42:33.000000 positional_vectorizer-0.0.3/.mypy_cache/3.11/positional_vectorizer/__init__.meta.json
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     1431 2024-05-01 22:20:12.000000 positional_vectorizer-0.0.3/LICENSE
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)      115 2024-05-01 22:57:25.000000 positional_vectorizer-0.0.3/MANIFEST.in
+-rw-r--r--   0 timotta   (1000) timotta   (1000)     3155 2024-05-01 22:57:48.238785 positional_vectorizer-0.0.3/PKG-INFO
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     2604 2024-05-01 22:16:28.000000 positional_vectorizer-0.0.3/README.md
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/dist/
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/dist/positional_vectorizer-0.0.2/
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/dist/positional_vectorizer-0.0.2/positional_vectorizer/
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     4308 2024-05-01 19:48:05.000000 positional_vectorizer-0.0.3/dist/positional_vectorizer-0.0.2/positional_vectorizer/__init__.py
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/positional_vectorizer/
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     4308 2024-05-01 19:48:05.000000 positional_vectorizer-0.0.3/positional_vectorizer/__init__.py
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.234785 positional_vectorizer-0.0.3/positional_vectorizer/__pycache__/
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     6034 2024-05-01 19:47:34.000000 positional_vectorizer-0.0.3/positional_vectorizer/__pycache__/__init__.cpython-311.pyc
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:57:48.238785 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/
+-rw-r--r--   0 timotta   (1000) timotta   (1000)     3155 2024-05-01 22:57:47.000000 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/PKG-INFO
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)      599 2024-05-01 22:57:48.000000 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)        1 2024-05-01 22:57:47.000000 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)       20 2024-05-01 22:57:47.000000 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/requires.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)       22 2024-05-01 22:57:47.000000 positional_vectorizer-0.0.3/positional_vectorizer.egg-info/top_level.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)       19 2024-04-30 23:59:15.000000 positional_vectorizer-0.0.3/requirements.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)       38 2024-05-01 22:57:48.238785 positional_vectorizer-0.0.3/setup.cfg
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     1364 2024-05-01 22:20:55.000000 positional_vectorizer-0.0.3/setup.py
```

### Comparing `positional_vectorizer-0.0.2/LICENSE` & `positional_vectorizer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `positional_vectorizer-0.0.2/PKG-INFO` & `positional_vectorizer-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: positional-vectorizer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Positional Vectorizer is a scikit-learn transformer that converts text to bag of words vector using a positional ranking algorithm as score
 Home-page: https://github.com/timotta/positional-vectorizer
 Author: Tiago Albineli Motta
 Author-email: timotta@gmail.com
 License: new BSD
 Keywords: machine learning,embedding,vectorizer,scikit-learn,text,NLP
 Requires-Python: >=3.11, <3.12
```

### Comparing `positional_vectorizer-0.0.2/README.md` & `positional_vectorizer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `positional_vectorizer-0.0.2/positional_vectorizer/__init__.py` & `positional_vectorizer-0.0.3/dist/positional_vectorizer-0.0.2/positional_vectorizer/__init__.py`

 * *Files identical despite different names*

### Comparing `positional_vectorizer-0.0.2/positional_vectorizer.egg-info/PKG-INFO` & `positional_vectorizer-0.0.3/positional_vectorizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: positional-vectorizer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Positional Vectorizer is a scikit-learn transformer that converts text to bag of words vector using a positional ranking algorithm as score
 Home-page: https://github.com/timotta/positional-vectorizer
 Author: Tiago Albineli Motta
 Author-email: timotta@gmail.com
 License: new BSD
 Keywords: machine learning,embedding,vectorizer,scikit-learn,text,NLP
 Requires-Python: >=3.11, <3.12
```

### Comparing `positional_vectorizer-0.0.2/setup.py` & `positional_vectorizer-0.0.3/setup.py`

 * *Files identical despite different names*

