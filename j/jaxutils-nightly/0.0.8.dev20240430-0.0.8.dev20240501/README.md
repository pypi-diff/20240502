# Comparing `tmp/jaxutils-nightly-0.0.8.dev20240430.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20240430.tar", last modified: Tue Apr 30 00:06:18 2024, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20240501.tar", last modified: Wed May  1 00:06:41 2024, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20240430.tar` & `jaxutils-nightly-0.0.8.dev20240501.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-30 00:06:18.332570 jaxutils-nightly-0.0.8.dev20240430/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-04-30 00:06:18.332570 jaxutils-nightly-0.0.8.dev20240430/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2024-04-30 00:06:10.000000 jaxutils-nightly-0.0.8.dev20240430/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-30 00:06:18.336570 jaxutils-nightly-0.0.8.dev20240430/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2024-04-30 00:06:10.000000 jaxutils-nightly-0.0.8.dev20240430/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2024-04-30 00:06:18.336570 jaxutils-nightly-0.0.8.dev20240430/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2024-04-30 00:06:10.000000 jaxutils-nightly-0.0.8.dev20240430/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2024-04-30 00:06:10.000000 jaxutils-nightly-0.0.8.dev20240430/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2024-04-30 00:06:10.000000 jaxutils-nightly-0.0.8.dev20240430/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2024-04-30 00:06:10.000000 jaxutils-nightly-0.0.8.dev20240430/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2024-04-30 00:06:10.000000 jaxutils-nightly-0.0.8.dev20240430/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-30 00:06:18.332570 jaxutils-nightly-0.0.8.dev20240430/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-04-30 00:06:18.000000 jaxutils-nightly-0.0.8.dev20240430/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2024-04-30 00:06:18.000000 jaxutils-nightly-0.0.8.dev20240430/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-30 00:06:18.000000 jaxutils-nightly-0.0.8.dev20240430/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2024-04-30 00:06:18.000000 jaxutils-nightly-0.0.8.dev20240430/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2024-04-30 00:06:18.000000 jaxutils-nightly-0.0.8.dev20240430/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2024-04-30 00:06:18.336570 jaxutils-nightly-0.0.8.dev20240430/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2024-04-30 00:06:10.000000 jaxutils-nightly-0.0.8.dev20240430/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2024-04-30 00:06:10.000000 jaxutils-nightly-0.0.8.dev20240430/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-01 00:06:41.678343 jaxutils-nightly-0.0.8.dev20240501/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-05-01 00:06:41.678343 jaxutils-nightly-0.0.8.dev20240501/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2024-05-01 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240501/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-01 00:06:41.682343 jaxutils-nightly-0.0.8.dev20240501/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2024-05-01 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240501/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2024-05-01 00:06:41.682343 jaxutils-nightly-0.0.8.dev20240501/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2024-05-01 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240501/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2024-05-01 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240501/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2024-05-01 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240501/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2024-05-01 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240501/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2024-05-01 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240501/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-01 00:06:41.678343 jaxutils-nightly-0.0.8.dev20240501/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-05-01 00:06:41.000000 jaxutils-nightly-0.0.8.dev20240501/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2024-05-01 00:06:41.000000 jaxutils-nightly-0.0.8.dev20240501/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-01 00:06:41.000000 jaxutils-nightly-0.0.8.dev20240501/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2024-05-01 00:06:41.000000 jaxutils-nightly-0.0.8.dev20240501/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2024-05-01 00:06:41.000000 jaxutils-nightly-0.0.8.dev20240501/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2024-05-01 00:06:41.678343 jaxutils-nightly-0.0.8.dev20240501/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2024-05-01 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240501/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2024-05-01 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240501/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20240430/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20240501/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20240430
+Version: 0.0.8.dev20240501
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20240430/README.md` & `jaxutils-nightly-0.0.8.dev20240501/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240430/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20240501/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240430/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20240501/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240430/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20240501/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240430/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20240501/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240430/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20240501/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240430/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20240501/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240430/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20240501/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20240430
+Version: 0.0.8.dev20240501
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20240430/setup.py` & `jaxutils-nightly-0.0.8.dev20240501/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240430/versioneer.py` & `jaxutils-nightly-0.0.8.dev20240501/versioneer.py`

 * *Files identical despite different names*

