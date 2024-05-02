# Comparing `tmp/galaxy-test-driver-24.0.0.tar.gz` & `tmp/galaxy_test_driver-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-test-driver-24.0.0.tar", last modified: Wed Apr  3 02:47:00 2024, max compression
+gzip compressed data, was "galaxy_test_driver-24.0.1.tar", last modified: Thu May  2 13:50:05 2024, max compression
```

## Comparing `galaxy-test-driver-24.0.0.tar` & `galaxy_test_driver-24.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:00.396629 galaxy-test-driver-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-03 02:47:00.396629 galaxy-test-driver-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:00.392629 galaxy-test-driver-24.0.0/galaxy_test/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:00.396629 galaxy-test-driver-24.0.0/galaxy_test/driver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41199 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/driver_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/integration_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/integration_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/uses_shed.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:00.396629 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-03 02:47:00.000000 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 02:47:00.000000 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:47:00.000000 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 02:47:00.000000 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 02:47:00.000000 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-03 02:47:00.396629 galaxy-test-driver-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:05.554349 galaxy_test_driver-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-02 13:50:05.554349 galaxy_test_driver-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:05.550349 galaxy_test_driver-24.0.1/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:05.554349 galaxy_test_driver-24.0.1/galaxy_test/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/galaxy_test/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41199 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/galaxy_test/driver/driver_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/galaxy_test/driver/integration_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/galaxy_test/driver/integration_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/galaxy_test/driver/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/galaxy_test/driver/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/galaxy_test/driver/uses_shed.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:50:05.554349 galaxy_test_driver-24.0.1/galaxy_test_driver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-02 13:50:05.000000 galaxy_test_driver-24.0.1/galaxy_test_driver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-02 13:50:05.000000 galaxy_test_driver-24.0.1/galaxy_test_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:50:05.000000 galaxy_test_driver-24.0.1/galaxy_test_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 13:50:05.000000 galaxy_test_driver-24.0.1/galaxy_test_driver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 13:50:05.000000 galaxy_test_driver-24.0.1/galaxy_test_driver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-02 13:50:05.554349 galaxy_test_driver-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_test_driver-24.0.1/test-requirements.txt
```

### Comparing `galaxy-test-driver-24.0.0/HISTORY.rst` & `galaxy_test_driver-24.0.1/HISTORY.rst`

 * *Files 4% similar despite different names*

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

### Comparing `galaxy-test-driver-24.0.0/LICENSE` & `galaxy_test_driver-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-24.0.0/PKG-INFO` & `galaxy_test_driver-24.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-driver
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy test driver
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -53,14 +53,20 @@
 
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

### Comparing `galaxy-test-driver-24.0.0/galaxy_test/driver/driver_util.py` & `galaxy_test_driver-24.0.1/galaxy_test/driver/driver_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-24.0.0/galaxy_test/driver/integration_setup.py` & `galaxy_test_driver-24.0.1/galaxy_test/driver/integration_setup.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-24.0.0/galaxy_test/driver/integration_util.py` & `galaxy_test_driver-24.0.1/galaxy_test/driver/integration_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-24.0.0/galaxy_test/driver/uses_shed.py` & `galaxy_test_driver-24.0.1/galaxy_test/driver/uses_shed.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/PKG-INFO` & `galaxy_test_driver-24.0.1/galaxy_test_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-driver
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy test driver
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -53,14 +53,20 @@
 
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

### Comparing `galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/SOURCES.txt` & `galaxy_test_driver-24.0.1/galaxy_test_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-24.0.0/setup.cfg` & `galaxy_test_driver-24.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-test-driver
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-app
 	galaxy-config
 	galaxy-data
```

