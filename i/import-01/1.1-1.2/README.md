# Comparing `tmp/import_01-1.1.tar.gz` & `tmp/import_01-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "import_01-1.1.tar", last modified: Sun Mar 10 17:37:11 2024, max compression
+gzip compressed data, was "import_01-1.2.tar", last modified: Thu May  2 08:40:28 2024, max compression
```

## Comparing `import_01-1.1.tar` & `import_01-1.2.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxr-xr-x   0 pranjalchaubey   (501) staff       (20)        0 2024-03-10 17:37:11.722790 import_01-1.1/
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)        0 2023-09-03 18:34:24.000000 import_01-1.1/LICENSE
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1886 2024-03-10 17:37:11.722695 import_01-1.1/PKG-INFO
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)      103 2023-09-03 18:34:46.000000 import_01-1.1/pyproject.toml
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1403 2024-03-10 17:34:18.000000 import_01-1.1/readme.md
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)      608 2024-03-10 17:37:11.723077 import_01-1.1/setup.cfg
-drwxr-xr-x   0 pranjalchaubey   (501) staff       (20)        0 2024-03-10 17:37:11.716625 import_01-1.1/src/
-drwxr-xr-x   0 pranjalchaubey   (501) staff       (20)        0 2024-03-10 17:37:11.721608 import_01-1.1/src/import_01/
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1210 2024-01-21 18:07:25.000000 import_01-1.1/src/import_01/Q1_and_or.py
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1349 2024-01-21 18:07:33.000000 import_01-1.1/src/import_01/Q2_xor_andnot.py
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)     2251 2024-01-24 14:52:59.000000 import_01-1.1/src/import_01/Q3_hebbian_net.py
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1526 2024-01-21 18:07:51.000000 import_01-1.1/src/import_01/Q4_discrete_hopfield_net.py
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)     2590 2024-01-21 18:07:59.000000 import_01-1.1/src/import_01/Q5_Kohonen_self_organizing_maps.py
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1756 2024-03-10 17:28:41.000000 import_01-1.1/src/import_01/Q6_perceptron.py
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)     2240 2024-03-10 17:26:51.000000 import_01-1.1/src/import_01/Q7_lvq.py
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)     4461 2024-03-10 17:28:19.000000 import_01-1.1/src/import_01/Q8_bipolar_sigmoid.py
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)        0 2023-09-05 16:12:11.000000 import_01-1.1/src/import_01/__init__.py
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)      186 2024-03-10 17:25:02.000000 import_01-1.1/src/import_01/main.py
-drwxr-xr-x   0 pranjalchaubey   (501) staff       (20)        0 2024-03-10 17:37:11.722451 import_01-1.1/src/import_01.egg-info/
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1886 2024-03-10 17:37:11.000000 import_01-1.1/src/import_01.egg-info/PKG-INFO
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)      510 2024-03-10 17:37:11.000000 import_01-1.1/src/import_01.egg-info/SOURCES.txt
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)        1 2024-03-10 17:37:11.000000 import_01-1.1/src/import_01.egg-info/dependency_links.txt
--rw-r--r--   0 pranjalchaubey   (501) staff       (20)       10 2024-03-10 17:37:11.000000 import_01-1.1/src/import_01.egg-info/top_level.txt
+drwxr-xr-x   0 pranjalchaubey   (501) staff       (20)        0 2024-05-02 08:40:28.238882 import_01-1.2/
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)        0 2023-09-03 18:34:24.000000 import_01-1.2/LICENSE
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1886 2024-05-02 08:40:28.238758 import_01-1.2/PKG-INFO
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)      103 2023-09-03 18:34:46.000000 import_01-1.2/pyproject.toml
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1403 2024-03-10 17:34:18.000000 import_01-1.2/readme.md
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)      608 2024-05-02 08:40:28.239446 import_01-1.2/setup.cfg
+drwxr-xr-x   0 pranjalchaubey   (501) staff       (20)        0 2024-05-02 08:40:28.228757 import_01-1.2/src/
+drwxr-xr-x   0 pranjalchaubey   (501) staff       (20)        0 2024-05-02 08:40:28.237085 import_01-1.2/src/import_01/
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1210 2024-01-21 18:07:25.000000 import_01-1.2/src/import_01/Q1_and_or.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1349 2024-01-21 18:07:33.000000 import_01-1.2/src/import_01/Q2_xor_andnot.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     2251 2024-01-24 14:52:59.000000 import_01-1.2/src/import_01/Q3_hebbian_net.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1526 2024-01-21 18:07:51.000000 import_01-1.2/src/import_01/Q4_discrete_hopfield_net.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     2590 2024-01-21 18:07:59.000000 import_01-1.2/src/import_01/Q5_Kohonen_self_organizing_maps.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1756 2024-03-10 17:28:41.000000 import_01-1.2/src/import_01/Q6_perceptron.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     2240 2024-03-10 17:26:51.000000 import_01-1.2/src/import_01/Q7_lvq.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     4461 2024-03-10 17:28:19.000000 import_01-1.2/src/import_01/Q8_bipolar_sigmoid.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)        0 2023-09-05 16:12:11.000000 import_01-1.2/src/import_01/__init__.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     2073 2024-05-02 08:39:31.000000 import_01-1.2/src/import_01/ann.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)      925 2024-05-02 08:22:07.000000 import_01-1.2/src/import_01/clustering.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)    12824 2024-05-02 08:23:04.000000 import_01-1.2/src/import_01/code.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1343 2024-05-02 08:29:19.000000 import_01-1.2/src/import_01/lightgbm.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)      263 2024-05-02 08:37:07.000000 import_01-1.2/src/import_01/main.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1558 2024-05-02 08:32:54.000000 import_01-1.2/src/import_01/modules.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1428 2024-05-02 08:25:05.000000 import_01-1.2/src/import_01/randomforest.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     2559 2024-05-02 08:35:44.000000 import_01-1.2/src/import_01/whatsapp.py
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1412 2024-05-02 08:38:03.000000 import_01-1.2/src/import_01/xgboost.py
+drwxr-xr-x   0 pranjalchaubey   (501) staff       (20)        0 2024-05-02 08:40:28.238346 import_01-1.2/src/import_01.egg-info/
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)     1886 2024-05-02 08:40:28.000000 import_01-1.2/src/import_01.egg-info/PKG-INFO
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)      713 2024-05-02 08:40:28.000000 import_01-1.2/src/import_01.egg-info/SOURCES.txt
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)        1 2024-05-02 08:40:28.000000 import_01-1.2/src/import_01.egg-info/dependency_links.txt
+-rw-r--r--   0 pranjalchaubey   (501) staff       (20)       10 2024-05-02 08:40:28.000000 import_01-1.2/src/import_01.egg-info/top_level.txt
```

### Comparing `import_01-1.1/PKG-INFO` & `import_01-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: import_01
-Version: 1.1
+Version: 1.2
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: prnjl
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `import_01-1.1/readme.md` & `import_01-1.2/readme.md`

 * *Files identical despite different names*

### Comparing `import_01-1.1/setup.cfg` & `import_01-1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = import_01
-version = 1.1
+version = 1.2
 author = prnjl
 author_email = author@example.com
 description = A small example package
 long_description = file: readme.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `import_01-1.1/src/import_01/Q1_and_or.py` & `import_01-1.2/src/import_01/Q1_and_or.py`

 * *Files identical despite different names*

### Comparing `import_01-1.1/src/import_01/Q2_xor_andnot.py` & `import_01-1.2/src/import_01/Q2_xor_andnot.py`

 * *Files identical despite different names*

### Comparing `import_01-1.1/src/import_01/Q3_hebbian_net.py` & `import_01-1.2/src/import_01/Q3_hebbian_net.py`

 * *Files identical despite different names*

### Comparing `import_01-1.1/src/import_01/Q4_discrete_hopfield_net.py` & `import_01-1.2/src/import_01/Q4_discrete_hopfield_net.py`

 * *Files identical despite different names*

### Comparing `import_01-1.1/src/import_01/Q5_Kohonen_self_organizing_maps.py` & `import_01-1.2/src/import_01/Q5_Kohonen_self_organizing_maps.py`

 * *Files identical despite different names*

### Comparing `import_01-1.1/src/import_01/Q6_perceptron.py` & `import_01-1.2/src/import_01/Q6_perceptron.py`

 * *Files identical despite different names*

### Comparing `import_01-1.1/src/import_01/Q7_lvq.py` & `import_01-1.2/src/import_01/Q7_lvq.py`

 * *Files identical despite different names*

### Comparing `import_01-1.1/src/import_01/Q8_bipolar_sigmoid.py` & `import_01-1.2/src/import_01/Q8_bipolar_sigmoid.py`

 * *Files identical despite different names*

### Comparing `import_01-1.1/src/import_01.egg-info/PKG-INFO` & `import_01-1.2/src/import_01.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: import_01
-Version: 1.1
+Version: 1.2
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: prnjl
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

