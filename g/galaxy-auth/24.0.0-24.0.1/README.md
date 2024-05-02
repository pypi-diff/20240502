# Comparing `tmp/galaxy-auth-24.0.0.tar.gz` & `tmp/galaxy_auth-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-auth-24.0.0.tar", last modified: Wed Apr  3 02:45:50 2024, max compression
+gzip compressed data, was "galaxy_auth-24.0.1.tar", last modified: Thu May  2 13:48:55 2024, max compression
```

## Comparing `galaxy-auth-24.0.0.tar` & `galaxy_auth-24.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/galaxy/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/galaxy/auth/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/providers/alwaysreject.py
--rw-r--r--   0 runner    (1001) docker     (127)    18512 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/providers/ldap_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/providers/localdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/providers/pam_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/galaxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-03 02:45:50.000000 galaxy-auth-24.0.0/galaxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-03 02:45:50.000000 galaxy-auth-24.0.0/galaxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:50.000000 galaxy-auth-24.0.0/galaxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 02:45:50.000000 galaxy-auth-24.0.0/galaxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:45:50.000000 galaxy-auth-24.0.0/galaxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-03 02:45:50.035499 galaxy-auth-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:55.085936 galaxy_auth-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-02 13:48:55.085936 galaxy_auth-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:55.081936 galaxy_auth-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:55.081936 galaxy_auth-24.0.1/galaxy/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:55.085936 galaxy_auth-24.0.1/galaxy/auth/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/providers/alwaysreject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18512 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/providers/ldap_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/providers/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/providers/pam_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:55.085936 galaxy_auth-24.0.1/galaxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-02 13:48:55.000000 galaxy_auth-24.0.1/galaxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-02 13:48:55.000000 galaxy_auth-24.0.1/galaxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:48:55.000000 galaxy_auth-24.0.1/galaxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 13:48:55.000000 galaxy_auth-24.0.1/galaxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:48:55.000000 galaxy_auth-24.0.1/galaxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-02 13:48:55.085936 galaxy_auth-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_auth-24.0.1/test-requirements.txt
```

### Comparing `galaxy-auth-24.0.0/HISTORY.rst` & `galaxy_auth-24.0.1/HISTORY.rst`

 * *Files 11% similar despite different names*

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
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-auth-24.0.0/LICENSE` & `galaxy_auth-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-auth-24.0.0/PKG-INFO` & `galaxy_auth-24.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-auth
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,20 @@
 
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
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-auth-24.0.0/galaxy/auth/__init__.py` & `galaxy_auth-24.0.1/galaxy/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-24.0.0/galaxy/auth/providers/__init__.py` & `galaxy_auth-24.0.1/galaxy/auth/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-24.0.0/galaxy/auth/providers/alwaysreject.py` & `galaxy_auth-24.0.1/galaxy/auth/providers/alwaysreject.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-24.0.0/galaxy/auth/providers/ldap_ad.py` & `galaxy_auth-24.0.1/galaxy/auth/providers/ldap_ad.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-24.0.0/galaxy/auth/providers/localdb.py` & `galaxy_auth-24.0.1/galaxy/auth/providers/localdb.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-24.0.0/galaxy/auth/providers/pam_auth.py` & `galaxy_auth-24.0.1/galaxy/auth/providers/pam_auth.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-24.0.0/galaxy/auth/util.py` & `galaxy_auth-24.0.1/galaxy/auth/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-24.0.0/galaxy_auth.egg-info/PKG-INFO` & `galaxy_auth-24.0.1/galaxy_auth.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-auth
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,20 @@
 
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
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-auth-24.0.0/galaxy_auth.egg-info/SOURCES.txt` & `galaxy_auth-24.0.1/galaxy_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-auth-24.0.0/setup.cfg` & `galaxy_auth-24.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-auth
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-util
 packages = find:
```

