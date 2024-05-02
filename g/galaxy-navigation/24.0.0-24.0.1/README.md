# Comparing `tmp/galaxy-navigation-24.0.0.tar.gz` & `tmp/galaxy_navigation-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-navigation-24.0.0.tar", last modified: Wed Apr  3 02:44:34 2024, max compression
+gzip compressed data, was "galaxy_navigation-24.0.1.tar", last modified: Thu May  2 13:47:39 2024, max compression
```

## Comparing `galaxy-navigation-24.0.0.tar` & `galaxy_navigation-24.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:34.934742 galaxy-navigation-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-03 02:44:34.934742 galaxy-navigation-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:34.930742 galaxy-navigation-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:34.930742 galaxy-navigation-24.0.0/galaxy/navigation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/navigation/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/navigation/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44962 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/navigation/navigation.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:34.934742 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-03 02:44:34.000000 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-03 02:44:34.000000 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:44:34.000000 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 02:44:34.000000 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:44:34.000000 galaxy-navigation-24.0.0/galaxy_navigation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-03 02:44:34.934742 galaxy-navigation-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-navigation-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:39.857523 galaxy_navigation-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-02 13:47:39.857523 galaxy_navigation-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:39.857523 galaxy_navigation-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:39.857523 galaxy_navigation-24.0.1/galaxy/navigation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/galaxy/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/galaxy/navigation/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/galaxy/navigation/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44962 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/galaxy/navigation/navigation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:39.857523 galaxy_navigation-24.0.1/galaxy_navigation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-02 13:47:39.000000 galaxy_navigation-24.0.1/galaxy_navigation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-02 13:47:39.000000 galaxy_navigation-24.0.1/galaxy_navigation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:47:39.000000 galaxy_navigation-24.0.1/galaxy_navigation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 13:47:39.000000 galaxy_navigation-24.0.1/galaxy_navigation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:47:39.000000 galaxy_navigation-24.0.1/galaxy_navigation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-02 13:47:39.857523 galaxy_navigation-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_navigation-24.0.1/test-requirements.txt
```

### Comparing `galaxy-navigation-24.0.0/HISTORY.rst` & `galaxy_navigation-24.0.1/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-navigation-24.0.0/LICENSE.txt` & `galaxy_navigation-24.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-navigation-24.0.0/PKG-INFO` & `galaxy_navigation-24.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-navigation
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy client DOM navigation framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,14 +46,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-navigation-24.0.0/galaxy/navigation/components.py` & `galaxy_navigation-24.0.1/galaxy/navigation/components.py`

 * *Files identical despite different names*

### Comparing `galaxy-navigation-24.0.0/galaxy/navigation/navigation.yml` & `galaxy_navigation-24.0.1/galaxy/navigation/navigation.yml`

 * *Files identical despite different names*

### Comparing `galaxy-navigation-24.0.0/galaxy_navigation.egg-info/PKG-INFO` & `galaxy_navigation-24.0.1/galaxy_navigation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-navigation
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy client DOM navigation framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,14 +46,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-navigation-24.0.0/setup.cfg` & `galaxy_navigation-24.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-navigation
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	PyYAML
 packages = find:
```

