# Comparing `tmp/galaxy-web-framework-24.0.0.tar.gz` & `tmp/galaxy_web_framework-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-web-framework-24.0.0.tar", last modified: Wed Apr  3 02:46:17 2024, max compression
+gzip compressed data, was "galaxy_web_framework-24.0.1.tar", last modified: Thu May  2 13:49:22 2024, max compression
```

## Comparing `galaxy-web-framework-24.0.0.tar` & `galaxy_web_framework-24.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.479979 galaxy-web-framework-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-03 02:46:17.479979 galaxy-web-framework-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.471979 galaxy-web-framework-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.471979 galaxy-web-framework-24.0.0/galaxy/web/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/form_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21864 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17365 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/remoteuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/request_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/sqldebug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/statsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/translogger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/xforwardedhost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/legacy_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/legacy_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38863 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/legacy_framework/grids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/proxy/
--rw-r--r--   0 runner    (1001) docker     (127)    13254 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.475979 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/mapper.js
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/proxy.js
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/proxy/js/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/galaxy/web/statsd_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:17.479979 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-03 02:46:17.000000 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-03 02:46:17.000000 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:46:17.000000 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 02:46:17.000000 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:46:17.000000 galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-03 02:46:17.479979 galaxy-web-framework-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-web-framework-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.542112 galaxy_web_framework-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-02 13:49:22.542112 galaxy_web_framework-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.534112 galaxy_web_framework-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.534112 galaxy_web_framework-24.0.1/galaxy/web/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/form_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.534112 galaxy_web_framework-24.0.1/galaxy/web/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21864 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.534112 galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.538112 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17365 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/remoteuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/sqldebug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/statsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/translogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/xforwardedhost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.538112 galaxy_web_framework-24.0.1/galaxy/web/legacy_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/legacy_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38863 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/legacy_framework/grids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.538112 galaxy_web_framework-24.0.1/galaxy/web/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13254 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.538112 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.538112 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/mapper.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/statsd_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.542112 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-02 13:49:22.000000 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-02 13:49:22.000000 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:49:22.000000 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-02 13:49:22.000000 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:49:22.000000 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-02 13:49:22.542112 galaxy_web_framework-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/test-requirements.txt
```

### Comparing `galaxy-web-framework-24.0.0/HISTORY.rst` & `galaxy_web_framework-24.0.1/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix KeyError in ``XForwardedHostMiddleware`` by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17955 <https://github.com/galaxyproject/galaxy/pull/17955>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-web-framework-24.0.0/LICENSE` & `galaxy_web_framework-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/PKG-INFO` & `galaxy_web_framework-24.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,14 +52,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix KeyError in ``XForwardedHostMiddleware`` by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17955 <https://github.com/galaxyproject/galaxy/pull/17955>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/__init__.py` & `galaxy_web_framework-24.0.1/galaxy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/__init__.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/base.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/base.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/decorators.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/decorators.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/__init__.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/grids.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/grids.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/helpers/tags.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/error.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/error.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/profile.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/profile.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/remoteuser.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/remoteuser.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/sqldebug.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/sqldebug.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/static.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/static.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/statsd.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/statsd.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/translogger.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/translogger.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/framework/middleware/xforwardedhost.py` & `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/xforwardedhost.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,18 +5,18 @@
     """
 
     def __init__(self, app, global_conf=None):
         self.app = app
 
     def __call__(self, environ, start_response):
         if x_forwarded_host := environ.get("HTTP_X_FORWARDED_HOST", None):
-            environ["ORGINAL_HTTP_HOST"] = environ["HTTP_HOST"]
+            environ["ORIGINAL_HTTP_HOST"] = environ.get("HTTP_HOST")
             environ["HTTP_HOST"] = x_forwarded_host.split(", ", 1)[0]
         if x_forwarded_for := environ.get("HTTP_X_FORWARDED_FOR", None):
-            environ["ORGINAL_REMOTE_ADDR"] = environ["REMOTE_ADDR"]
+            environ["ORIGINAL_REMOTE_ADDR"] = environ.get("REMOTE_ADDR")
             environ["REMOTE_ADDR"] = x_forwarded_for.split(",", 1)[0].strip()
         x_forwarded_proto = environ.get("HTTP_X_FORWARDED_PROTO", None)
         if x_forwarded_proto:
             x_forwarded_proto = x_forwarded_proto.split(",", 1)[0].strip()
         if x_url_scheme := environ.get("HTTP_X_URL_SCHEME", x_forwarded_proto):
             environ["original_wsgi.url_scheme"] = environ["wsgi.url_scheme"]
             environ["wsgi.url_scheme"] = x_url_scheme
```

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/legacy_framework/grids.py` & `galaxy_web_framework-24.0.1/galaxy/web/legacy_framework/grids.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/proxy/__init__.py` & `galaxy_web_framework-24.0.1/galaxy/web/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/proxy/js/Dockerfile` & `galaxy_web_framework-24.0.1/galaxy/web/proxy/js/Dockerfile`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/main.js` & `galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/main.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/mapper.js` & `galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/mapper.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/proxy/js/lib/proxy.js` & `galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/proxy.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy/web/statsd_client.py` & `galaxy_web_framework-24.0.1/galaxy/web/statsd_client.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/PKG-INFO` & `galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,14 +52,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix KeyError in ``XForwardedHostMiddleware`` by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17955 <https://github.com/galaxyproject/galaxy/pull/17955>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-web-framework-24.0.0/galaxy_web_framework.egg-info/SOURCES.txt` & `galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-24.0.0/setup.cfg` & `galaxy_web_framework-24.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-web-framework
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-util
 	babel
```

