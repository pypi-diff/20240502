# Comparing `tmp/mnist_separator-1.0.2.tar.gz` & `tmp/mnist_separator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnist_separator-1.0.2.tar", max compression
+gzip compressed data, was "mnist_separator-1.0.3.tar", max compression
```

## Comparing `mnist_separator-1.0.2.tar` & `mnist_separator-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      227 2024-04-12 10:18:12.545299 mnist_separator-1.0.2/README.md
--rw-r--r--   0        0        0     6148 2024-05-02 14:50:49.508177 mnist_separator-1.0.2/mnist_separator/.DS_Store
--rw-r--r--   0        0        0      177 2024-05-02 14:31:44.020164 mnist_separator-1.0.2/mnist_separator/__init__.py
--rw-r--r--   0        0        0     6148 2024-05-02 14:58:00.574752 mnist_separator-1.0.2/mnist_separator/src/.DS_Store
--rw-r--r--   0        0        0      553 2024-05-02 03:22:36.857384 mnist_separator-1.0.2/mnist_separator/src/clean_all.py
--rw-r--r--   0        0        0     2820 2024-05-02 03:22:36.842248 mnist_separator-1.0.2/mnist_separator/src/convert_data.py
--rw-r--r--   0        0        0     2076 2024-05-02 03:22:36.911146 mnist_separator-1.0.2/mnist_separator/src/create_dirs.py
--rw-r--r--   0        0        0      722 2024-05-02 03:22:36.863875 mnist_separator-1.0.2/mnist_separator/src/get_similarity.py
--rw-r--r--   0        0        0     1263 2024-05-02 03:22:36.903410 mnist_separator-1.0.2/mnist_separator/src/get_similarity_group.py
--rw-r--r--   0        0        0      690 2024-05-02 03:22:36.899832 mnist_separator-1.0.2/mnist_separator/src/glbl.py
--rw-r--r--   0        0        0     3103 2024-05-02 03:22:36.887208 mnist_separator-1.0.2/mnist_separator/src/go.py
--rw-r--r--   0        0        0      181 2024-05-02 03:22:36.821442 mnist_separator-1.0.2/mnist_separator/src/init.py
--rw-r--r--   0        0        0      970 2024-05-02 14:35:43.534234 mnist_separator-1.0.2/mnist_separator/src/load_data.py
--rw-r--r--   0        0        0     1012 2024-05-02 03:22:36.836421 mnist_separator-1.0.2/mnist_separator/src/load_samples.py
--rw-r--r--   0        0        0     1386 2024-05-02 03:22:36.848610 mnist_separator-1.0.2/mnist_separator/src/save_result.py
--rw-r--r--   0        0        0      825 2024-05-02 03:22:36.833593 mnist_separator-1.0.2/mnist_separator/src/timer.py
--rw-r--r--   0        0        0     4104 2024-05-02 03:22:36.896651 mnist_separator-1.0.2/mnist_separator/src/to_canonical.py
--rw-r--r--   0        0        0      663 2024-05-02 14:27:33.572174 mnist_separator-1.0.2/mnist_separator/src/utils_directory.py
--rw-r--r--   0        0        0      600 2024-05-02 03:22:36.907332 mnist_separator-1.0.2/mnist_separator/src/utils_list.py
--rw-r--r--   0        0        0      497 2024-05-02 15:08:13.003138 mnist_separator-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 mnist_separator-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-04-12 10:18:12.545299 mnist_separator-1.0.3/README.md
+-rw-r--r--   0        0        0     6148 2024-05-02 14:50:49.508177 mnist_separator-1.0.3/mnist_separator/.DS_Store
+-rw-r--r--   0        0        0      177 2024-05-02 14:31:44.020164 mnist_separator-1.0.3/mnist_separator/__init__.py
+-rw-r--r--   0        0        0     6148 2024-05-02 14:58:00.574752 mnist_separator-1.0.3/mnist_separator/src/.DS_Store
+-rw-r--r--   0        0        0      553 2024-05-02 03:22:36.857384 mnist_separator-1.0.3/mnist_separator/src/clean_all.py
+-rw-r--r--   0        0        0     2820 2024-05-02 03:22:36.842248 mnist_separator-1.0.3/mnist_separator/src/convert_data.py
+-rw-r--r--   0        0        0     2076 2024-05-02 03:22:36.911146 mnist_separator-1.0.3/mnist_separator/src/create_dirs.py
+-rw-r--r--   0        0        0      722 2024-05-02 03:22:36.863875 mnist_separator-1.0.3/mnist_separator/src/get_similarity.py
+-rw-r--r--   0        0        0     1243 2024-05-02 15:38:53.247769 mnist_separator-1.0.3/mnist_separator/src/get_similarity_group.py
+-rw-r--r--   0        0        0      690 2024-05-02 03:22:36.899832 mnist_separator-1.0.3/mnist_separator/src/glbl.py
+-rw-r--r--   0        0        0     3103 2024-05-02 03:22:36.887208 mnist_separator-1.0.3/mnist_separator/src/go.py
+-rw-r--r--   0        0        0      181 2024-05-02 03:22:36.821442 mnist_separator-1.0.3/mnist_separator/src/init.py
+-rw-r--r--   0        0        0      970 2024-05-02 14:35:43.534234 mnist_separator-1.0.3/mnist_separator/src/load_data.py
+-rw-r--r--   0        0        0     1012 2024-05-02 03:22:36.836421 mnist_separator-1.0.3/mnist_separator/src/load_samples.py
+-rw-r--r--   0        0        0     1386 2024-05-02 03:22:36.848610 mnist_separator-1.0.3/mnist_separator/src/save_result.py
+-rw-r--r--   0        0        0      825 2024-05-02 03:22:36.833593 mnist_separator-1.0.3/mnist_separator/src/timer.py
+-rw-r--r--   0        0        0     4104 2024-05-02 03:22:36.896651 mnist_separator-1.0.3/mnist_separator/src/to_canonical.py
+-rw-r--r--   0        0        0      663 2024-05-02 14:27:33.572174 mnist_separator-1.0.3/mnist_separator/src/utils_directory.py
+-rw-r--r--   0        0        0      600 2024-05-02 03:22:36.907332 mnist_separator-1.0.3/mnist_separator/src/utils_list.py
+-rw-r--r--   0        0        0      497 2024-05-02 18:20:32.158611 mnist_separator-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 mnist_separator-1.0.3/PKG-INFO
```

### Comparing `mnist_separator-1.0.2/mnist_separator/.DS_Store` & `mnist_separator-1.0.3/mnist_separator/.DS_Store`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/.DS_Store` & `mnist_separator-1.0.3/mnist_separator/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/clean_all.py` & `mnist_separator-1.0.3/mnist_separator/src/clean_all.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/convert_data.py` & `mnist_separator-1.0.3/mnist_separator/src/convert_data.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/create_dirs.py` & `mnist_separator-1.0.3/mnist_separator/src/create_dirs.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/get_similarity.py` & `mnist_separator-1.0.3/mnist_separator/src/get_similarity.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/get_similarity_group.py` & `mnist_separator-1.0.3/mnist_separator/src/get_similarity_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # May-02-2024
 # get_similarity_group.py
 
 import os
 import cv2 as cv
 import numpy as np
 
-from one_with_another.src.calc_similarity import calc_similarity
+from one_with_another import calc_similarity
 
 
 def get_similarity_group(path_image_test: str, path_train: str) -> float:
     """
     Нахождение максимального значения степени сходства между
     заданным каноническим изображением и всеми каноническими
     изображениями группы.
```

### Comparing `mnist_separator-1.0.2/mnist_separator/src/glbl.py` & `mnist_separator-1.0.3/mnist_separator/src/glbl.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/go.py` & `mnist_separator-1.0.3/mnist_separator/src/go.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/load_data.py` & `mnist_separator-1.0.3/mnist_separator/src/load_data.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/load_samples.py` & `mnist_separator-1.0.3/mnist_separator/src/load_samples.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/save_result.py` & `mnist_separator-1.0.3/mnist_separator/src/save_result.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/timer.py` & `mnist_separator-1.0.3/mnist_separator/src/timer.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/to_canonical.py` & `mnist_separator-1.0.3/mnist_separator/src/to_canonical.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/utils_directory.py` & `mnist_separator-1.0.3/mnist_separator/src/utils_directory.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/mnist_separator/src/utils_list.py` & `mnist_separator-1.0.3/mnist_separator/src/utils_list.py`

 * *Files identical despite different names*

### Comparing `mnist_separator-1.0.2/PKG-INFO` & `mnist_separator-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnist-separator
-Version: 1.0.2
+Version: 1.0.3
 Summary: mnist-separator is a new technology for recognizing handwritten numbers from the MNIST dataset
 License: MIT
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

