# Comparing `tmp/scikit-duplo-0.1.8.tar.gz` & `tmp/scikit-duplo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-duplo-0.1.8.tar", last modified: Thu Apr 18 03:20:54 2024, max compression
+gzip compressed data, was "scikit-duplo-0.1.9.tar", last modified: Thu Apr 18 22:10:14 2024, max compression
```

## Comparing `scikit-duplo-0.1.8.tar` & `scikit-duplo-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2024-04-18 03:20:54.665270 scikit-duplo-0.1.8/
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1082 2023-04-06 00:11:51.000000 scikit-duplo-0.1.8/LICENSE
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1869 2024-04-18 03:20:54.664923 scikit-duplo-0.1.8/PKG-INFO
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1329 2024-04-18 03:17:01.000000 scikit-duplo-0.1.8/README.md
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2024-04-18 03:20:54.660152 scikit-duplo-0.1.8/scikit_duplo.egg-info/
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1869 2024-04-18 03:20:54.000000 scikit-duplo-0.1.8/scikit_duplo.egg-info/PKG-INFO
--rw-r--r--   0 johnhawkins   (501) staff       (20)      537 2024-04-18 03:20:54.000000 scikit-duplo-0.1.8/scikit_duplo.egg-info/SOURCES.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)        1 2024-04-18 03:20:54.000000 scikit-duplo-0.1.8/scikit_duplo.egg-info/dependency_links.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)       26 2024-04-18 03:20:54.000000 scikit-duplo-0.1.8/scikit_duplo.egg-info/requires.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)        8 2024-04-18 03:20:54.000000 scikit-duplo-0.1.8/scikit_duplo.egg-info/top_level.txt
--rw-r--r--   0 johnhawkins   (501) staff       (20)       38 2024-04-18 03:20:54.665381 scikit-duplo-0.1.8/setup.cfg
--rwxr-xr-x   0 johnhawkins   (501) staff       (20)     1163 2023-04-10 21:57:03.000000 scikit-duplo-0.1.8/setup.py
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2024-04-18 03:20:54.660769 scikit-duplo-0.1.8/skduplo/
--rw-r--r--   0 johnhawkins   (501) staff       (20)       22 2024-04-18 03:15:50.000000 scikit-duplo-0.1.8/skduplo/__init__.py
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2024-04-18 03:20:54.662622 scikit-duplo-0.1.8/skduplo/meta/
--rw-r--r--   0 johnhawkins   (501) staff       (20)      282 2023-05-17 03:58:33.000000 scikit-duplo-0.1.8/skduplo/meta/__init__.py
--rw-r--r--   0 johnhawkins   (501) staff       (20)     4436 2023-05-17 06:07:36.000000 scikit-duplo-0.1.8/skduplo/meta/baseline_proportional_regressor.py
--rw-r--r--   0 johnhawkins   (501) staff       (20)     5862 2023-04-06 22:04:15.000000 scikit-duplo-0.1.8/skduplo/meta/quantile_stack_regressor.py
--rw-r--r--   0 johnhawkins   (501) staff       (20)     4869 2023-04-10 22:56:04.000000 scikit-duplo-0.1.8/skduplo/meta/regressor_stack.py
-drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2024-04-18 03:20:54.664409 scikit-duplo-0.1.8/skduplo/preprocessing/
--rw-r--r--   0 johnhawkins   (501) staff       (20)      172 2023-04-06 21:55:06.000000 scikit-duplo-0.1.8/skduplo/preprocessing/__init__.py
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1155 2023-04-06 00:24:35.000000 scikit-duplo-0.1.8/skduplo/preprocessing/column_concatenator.py
--rw-r--r--   0 johnhawkins   (501) staff       (20)      565 2024-04-18 03:15:20.000000 scikit-duplo-0.1.8/skduplo/preprocessing/lookup_encoder.py
--rw-r--r--   0 johnhawkins   (501) staff       (20)     1217 2023-04-06 00:20:02.000000 scikit-duplo-0.1.8/skduplo/preprocessing/two_column_ratio_diff.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2024-04-18 22:10:14.230449 scikit-duplo-0.1.9/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1082 2023-04-06 00:11:51.000000 scikit-duplo-0.1.9/LICENSE
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1869 2024-04-18 22:10:14.229939 scikit-duplo-0.1.9/PKG-INFO
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1329 2024-04-18 03:17:01.000000 scikit-duplo-0.1.9/README.md
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2024-04-18 22:10:14.219211 scikit-duplo-0.1.9/scikit_duplo.egg-info/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1869 2024-04-18 22:10:14.000000 scikit-duplo-0.1.9/scikit_duplo.egg-info/PKG-INFO
+-rw-r--r--   0 johnhawkins   (501) staff       (20)      537 2024-04-18 22:10:14.000000 scikit-duplo-0.1.9/scikit_duplo.egg-info/SOURCES.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)        1 2024-04-18 22:10:14.000000 scikit-duplo-0.1.9/scikit_duplo.egg-info/dependency_links.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       26 2024-04-18 22:10:14.000000 scikit-duplo-0.1.9/scikit_duplo.egg-info/requires.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)        8 2024-04-18 22:10:14.000000 scikit-duplo-0.1.9/scikit_duplo.egg-info/top_level.txt
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       38 2024-04-18 22:10:14.230622 scikit-duplo-0.1.9/setup.cfg
+-rwxr-xr-x   0 johnhawkins   (501) staff       (20)     1163 2023-04-10 21:57:03.000000 scikit-duplo-0.1.9/setup.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2024-04-18 22:10:14.220294 scikit-duplo-0.1.9/skduplo/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)       22 2024-04-18 22:09:39.000000 scikit-duplo-0.1.9/skduplo/__init__.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2024-04-18 22:10:14.224204 scikit-duplo-0.1.9/skduplo/meta/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)      282 2023-05-17 03:58:33.000000 scikit-duplo-0.1.9/skduplo/meta/__init__.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     4436 2023-05-17 06:07:36.000000 scikit-duplo-0.1.9/skduplo/meta/baseline_proportional_regressor.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     5862 2023-04-06 22:04:15.000000 scikit-duplo-0.1.9/skduplo/meta/quantile_stack_regressor.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     4869 2023-04-10 22:56:04.000000 scikit-duplo-0.1.9/skduplo/meta/regressor_stack.py
+drwxr-xr-x   0 johnhawkins   (501) staff       (20)        0 2024-04-18 22:10:14.228800 scikit-duplo-0.1.9/skduplo/preprocessing/
+-rw-r--r--   0 johnhawkins   (501) staff       (20)      235 2024-04-18 22:09:23.000000 scikit-duplo-0.1.9/skduplo/preprocessing/__init__.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1155 2023-04-06 00:24:35.000000 scikit-duplo-0.1.9/skduplo/preprocessing/column_concatenator.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)      565 2024-04-18 03:15:20.000000 scikit-duplo-0.1.9/skduplo/preprocessing/lookup_encoder.py
+-rw-r--r--   0 johnhawkins   (501) staff       (20)     1217 2023-04-06 00:20:02.000000 scikit-duplo-0.1.9/skduplo/preprocessing/two_column_ratio_diff.py
```

### Comparing `scikit-duplo-0.1.8/LICENSE` & `scikit-duplo-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.8/PKG-INFO` & `scikit-duplo-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-duplo
-Version: 0.1.8
+Version: 0.1.9
 Summary: Sci-kit learn tools for machine learning pipelines
 Home-page: http://getting-data-science-done.com
 Author: John Hawkins
 Author-email: johnc@getting-data-science-done.com
 License: MIT
 Project-URL: Documentation, http://scikit-duplo.readthedocs.io
 Project-URL: Source, https://github.com/getting-data-science-done/scikit-duplo
```

### Comparing `scikit-duplo-0.1.8/README.md` & `scikit-duplo-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.8/scikit_duplo.egg-info/PKG-INFO` & `scikit-duplo-0.1.9/scikit_duplo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-duplo
-Version: 0.1.8
+Version: 0.1.9
 Summary: Sci-kit learn tools for machine learning pipelines
 Home-page: http://getting-data-science-done.com
 Author: John Hawkins
 Author-email: johnc@getting-data-science-done.com
 License: MIT
 Project-URL: Documentation, http://scikit-duplo.readthedocs.io
 Project-URL: Source, https://github.com/getting-data-science-done/scikit-duplo
```

### Comparing `scikit-duplo-0.1.8/scikit_duplo.egg-info/SOURCES.txt` & `scikit-duplo-0.1.9/scikit_duplo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.8/setup.py` & `scikit-duplo-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.8/skduplo/meta/baseline_proportional_regressor.py` & `scikit-duplo-0.1.9/skduplo/meta/baseline_proportional_regressor.py`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.8/skduplo/meta/quantile_stack_regressor.py` & `scikit-duplo-0.1.9/skduplo/meta/quantile_stack_regressor.py`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.8/skduplo/meta/regressor_stack.py` & `scikit-duplo-0.1.9/skduplo/meta/regressor_stack.py`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.8/skduplo/preprocessing/column_concatenator.py` & `scikit-duplo-0.1.9/skduplo/preprocessing/column_concatenator.py`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.8/skduplo/preprocessing/lookup_encoder.py` & `scikit-duplo-0.1.9/skduplo/preprocessing/lookup_encoder.py`

 * *Files identical despite different names*

### Comparing `scikit-duplo-0.1.8/skduplo/preprocessing/two_column_ratio_diff.py` & `scikit-duplo-0.1.9/skduplo/preprocessing/two_column_ratio_diff.py`

 * *Files identical despite different names*

