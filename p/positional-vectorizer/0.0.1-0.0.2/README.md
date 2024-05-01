# Comparing `tmp/positional-vectorizer-0.0.1.tar.gz` & `tmp/positional_vectorizer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "positional-vectorizer-0.0.1.tar", last modified: Wed May  1 22:39:50 2024, max compression
+gzip compressed data, was "positional_vectorizer-0.0.2.tar", last modified: Wed May  1 22:51:19 2024, max compression
```

## Comparing `positional-vectorizer-0.0.1.tar` & `positional_vectorizer-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:39:50.108057 positional-vectorizer-0.0.1/
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     1431 2024-05-01 22:20:12.000000 positional-vectorizer-0.0.1/LICENSE
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     3140 2024-05-01 22:39:50.108057 positional-vectorizer-0.0.1/PKG-INFO
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     2604 2024-05-01 22:16:28.000000 positional-vectorizer-0.0.1/README.md
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:39:50.108057 positional-vectorizer-0.0.1/positional_vectorizer/
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     4308 2024-05-01 19:48:05.000000 positional-vectorizer-0.0.1/positional_vectorizer/__init__.py
-drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:39:50.108057 positional-vectorizer-0.0.1/positional_vectorizer.egg-info/
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     3140 2024-05-01 22:39:50.000000 positional-vectorizer-0.0.1/positional_vectorizer.egg-info/PKG-INFO
--rw-rw-r--   0 timotta   (1000) timotta   (1000)      332 2024-05-01 22:39:50.000000 positional-vectorizer-0.0.1/positional_vectorizer.egg-info/SOURCES.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)        1 2024-05-01 22:39:50.000000 positional-vectorizer-0.0.1/positional_vectorizer.egg-info/dependency_links.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)       20 2024-05-01 22:39:50.000000 positional-vectorizer-0.0.1/positional_vectorizer.egg-info/entry_points.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)       20 2024-05-01 22:39:50.000000 positional-vectorizer-0.0.1/positional_vectorizer.egg-info/requires.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)       22 2024-05-01 22:39:50.000000 positional-vectorizer-0.0.1/positional_vectorizer.egg-info/top_level.txt
--rw-rw-r--   0 timotta   (1000) timotta   (1000)       38 2024-05-01 22:39:50.108057 positional-vectorizer-0.0.1/setup.cfg
--rw-rw-r--   0 timotta   (1000) timotta   (1000)     1364 2024-05-01 22:20:55.000000 positional-vectorizer-0.0.1/setup.py
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:51:19.134105 positional_vectorizer-0.0.2/
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     1431 2024-05-01 22:20:12.000000 positional_vectorizer-0.0.2/LICENSE
+-rw-r--r--   0 timotta   (1000) timotta   (1000)     3155 2024-05-01 22:51:19.134105 positional_vectorizer-0.0.2/PKG-INFO
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     2604 2024-05-01 22:16:28.000000 positional_vectorizer-0.0.2/README.md
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:51:19.134105 positional_vectorizer-0.0.2/positional_vectorizer/
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     4308 2024-05-01 19:48:05.000000 positional_vectorizer-0.0.2/positional_vectorizer/__init__.py
+drwxrwxr-x   0 timotta   (1000) timotta   (1000)        0 2024-05-01 22:51:19.134105 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/
+-rw-r--r--   0 timotta   (1000) timotta   (1000)     3155 2024-05-01 22:51:19.000000 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/PKG-INFO
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)      284 2024-05-01 22:51:19.000000 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)        1 2024-05-01 22:51:19.000000 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)       20 2024-05-01 22:51:19.000000 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/requires.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)       22 2024-05-01 22:51:19.000000 positional_vectorizer-0.0.2/positional_vectorizer.egg-info/top_level.txt
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)       38 2024-05-01 22:51:19.134105 positional_vectorizer-0.0.2/setup.cfg
+-rw-rw-r--   0 timotta   (1000) timotta   (1000)     1364 2024-05-01 22:20:55.000000 positional_vectorizer-0.0.2/setup.py
```

### Comparing `positional-vectorizer-0.0.1/LICENSE` & `positional_vectorizer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `positional-vectorizer-0.0.1/PKG-INFO` & `positional_vectorizer-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: positional-vectorizer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Positional Vectorizer is a scikit-learn transformer that converts text to bag of words vector using a positional ranking algorithm as score
 Home-page: https://github.com/timotta/positional-vectorizer
 Author: Tiago Albineli Motta
 Author-email: timotta@gmail.com
 License: new BSD
 Keywords: machine learning,embedding,vectorizer,scikit-learn,text,NLP
-Platform: UNKNOWN
 Requires-Python: >=3.11, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scikit-learn>=1.4.2
 
 # Positional Vectorizer
 
 The Positional Vectorizer is a transformer in scikit-learn designed to transform text into a bag of words vector using a positional ranking algorithm to assign scores. Similar to scikit-learn's CountVectorizer and TFIDFVectorizer, it assigns a value to each dimension based on the term's position in the original text.
 
 ## How to use
 
@@ -70,9 +70,7 @@
 If a term appears multiple times in the text, only its lowest rank is taken into account.
 
 ## TODO
 
 * Test the common parameters of _VectorizerMixin to identify potential issues when upgrading scikit-learn. Currently, only the `ngrams_range` and `analyzer` parameters are automatically tested.
 * Implement the max_features parameter.
 
-
-
```

### Comparing `positional-vectorizer-0.0.1/README.md` & `positional_vectorizer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `positional-vectorizer-0.0.1/positional_vectorizer/__init__.py` & `positional_vectorizer-0.0.2/positional_vectorizer/__init__.py`

 * *Files identical despite different names*

### Comparing `positional-vectorizer-0.0.1/positional_vectorizer.egg-info/PKG-INFO` & `positional_vectorizer-0.0.2/positional_vectorizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: positional-vectorizer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Positional Vectorizer is a scikit-learn transformer that converts text to bag of words vector using a positional ranking algorithm as score
 Home-page: https://github.com/timotta/positional-vectorizer
 Author: Tiago Albineli Motta
 Author-email: timotta@gmail.com
 License: new BSD
 Keywords: machine learning,embedding,vectorizer,scikit-learn,text,NLP
-Platform: UNKNOWN
 Requires-Python: >=3.11, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scikit-learn>=1.4.2
 
 # Positional Vectorizer
 
 The Positional Vectorizer is a transformer in scikit-learn designed to transform text into a bag of words vector using a positional ranking algorithm to assign scores. Similar to scikit-learn's CountVectorizer and TFIDFVectorizer, it assigns a value to each dimension based on the term's position in the original text.
 
 ## How to use
 
@@ -70,9 +70,7 @@
 If a term appears multiple times in the text, only its lowest rank is taken into account.
 
 ## TODO
 
 * Test the common parameters of _VectorizerMixin to identify potential issues when upgrading scikit-learn. Currently, only the `ngrams_range` and `analyzer` parameters are automatically tested.
 * Implement the max_features parameter.
 
-
-
```

### Comparing `positional-vectorizer-0.0.1/setup.py` & `positional_vectorizer-0.0.2/setup.py`

 * *Files identical despite different names*

