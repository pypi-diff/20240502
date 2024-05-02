# Comparing `tmp/galaxy-schema-24.0.0.tar.gz` & `tmp/galaxy_schema-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-schema-24.0.0.tar", last modified: Wed Apr  3 02:44:52 2024, max compression
+gzip compressed data, was "galaxy_schema-24.0.1.tar", last modified: Thu May  2 13:47:57 2024, max compression
```

## Comparing `galaxy-schema-24.0.0.tar` & `galaxy_schema-24.0.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.922922 galaxy-schema-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-03 02:44:52.922922 galaxy-schema-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.914922 galaxy-schema-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.918922 galaxy-schema-24.0.0/galaxy/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.918922 galaxy-schema-24.0.0/galaxy/schema/bco/
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/description_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/error_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/execution_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/io_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/parametric_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/provenance_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/usability_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/bco/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.918922 galaxy-schema-24.0.0/galaxy/schema/drs/
--rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/fetch_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    25194 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/invocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/item_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/remote_files.py
--rw-r--r--   0 runner    (1001) docker     (127)   117967 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/storage_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.918922 galaxy-schema-24.0.0/galaxy/schema/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/workflow/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/galaxy/schema/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:52.922922 galaxy-schema-24.0.0/galaxy_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-03 02:44:52.000000 galaxy-schema-24.0.0/galaxy_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-03 02:44:52.000000 galaxy-schema-24.0.0/galaxy_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:44:52.000000 galaxy-schema-24.0.0/galaxy_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 02:44:52.000000 galaxy-schema-24.0.0/galaxy_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:44:52.000000 galaxy-schema-24.0.0/galaxy_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-03 02:44:52.922922 galaxy-schema-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-schema-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.925628 galaxy_schema-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.929628 galaxy_schema-24.0.1/galaxy/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/galaxy/schema/bco/
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/description_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/error_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/execution_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/io_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/parametric_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/provenance_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/usability_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/galaxy/schema/drs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/fetch_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25194 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/invocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/item_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/remote_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118022 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/storage_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/galaxy/schema/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/workflow/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/galaxy_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-02 13:47:57.000000 galaxy_schema-24.0.1/galaxy_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-02 13:47:57.000000 galaxy_schema-24.0.1/galaxy_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:47:57.000000 galaxy_schema-24.0.1/galaxy_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 13:47:57.000000 galaxy_schema-24.0.1/galaxy_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:47:57.000000 galaxy_schema-24.0.1/galaxy_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/test-requirements.txt
```

### Comparing `galaxy-schema-24.0.0/HISTORY.rst` & `galaxy_schema-24.0.1/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,25 @@
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
+* Fix tag regex pattern by `@jdavcs <https://github.com/jdavcs>`_ in `#18025 <https://github.com/galaxyproject/galaxy/pull/18025>`_
+* Fix History Dataset Association creation so that hid is always set by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18036 <https://github.com/galaxyproject/galaxy/pull/18036>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-schema-24.0.0/LICENSE` & `galaxy_schema-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/PKG-INFO` & `galaxy_schema-24.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-schema
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,26 @@
 
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
+* Fix tag regex pattern by `@jdavcs <https://github.com/jdavcs>`_ in `#18025 <https://github.com/galaxyproject/galaxy/pull/18025>`_
+* Fix History Dataset Association creation so that hid is always set by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18036 <https://github.com/galaxyproject/galaxy/pull/18036>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-schema-24.0.0/galaxy/schema/__init__.py` & `galaxy_schema-24.0.1/galaxy/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/bco/__init__.py` & `galaxy_schema-24.0.1/galaxy/schema/bco/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/bco/description_domain.py` & `galaxy_schema-24.0.1/galaxy/schema/bco/description_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/bco/error_domain.py` & `galaxy_schema-24.0.1/galaxy/schema/bco/error_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/bco/execution_domain.py` & `galaxy_schema-24.0.1/galaxy/schema/bco/execution_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/bco/io_domain.py` & `galaxy_schema-24.0.1/galaxy/schema/bco/io_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/bco/parametric_domain.py` & `galaxy_schema-24.0.1/galaxy/schema/bco/parametric_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/bco/provenance_domain.py` & `galaxy_schema-24.0.1/galaxy/schema/bco/provenance_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/bco/usability_domain.py` & `galaxy_schema-24.0.1/galaxy/schema/bco/usability_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/bco/util.py` & `galaxy_schema-24.0.1/galaxy/schema/bco/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/cloud.py` & `galaxy_schema-24.0.1/galaxy/schema/cloud.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/drs/__init__.py` & `galaxy_schema-24.0.1/galaxy/schema/drs/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/fetch_data.py` & `galaxy_schema-24.0.1/galaxy/schema/fetch_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/fields.py` & `galaxy_schema-24.0.1/galaxy/schema/fields.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/groups.py` & `galaxy_schema-24.0.1/galaxy/schema/groups.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/help.py` & `galaxy_schema-24.0.1/galaxy/schema/help.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/history.py` & `galaxy_schema-24.0.1/galaxy/schema/history.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/invocation.py` & `galaxy_schema-24.0.1/galaxy/schema/invocation.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/item_tags.py` & `galaxy_schema-24.0.1/galaxy/schema/item_tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/jobs.py` & `galaxy_schema-24.0.1/galaxy/schema/jobs.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/notifications.py` & `galaxy_schema-24.0.1/galaxy/schema/notifications.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/remote_files.py` & `galaxy_schema-24.0.1/galaxy/schema/remote_files.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/schema.py` & `galaxy_schema-24.0.1/galaxy/schema/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 INVOCATION_MODEL_CLASS = Literal["WorkflowInvocation"]
 INVOCATION_STEP_MODEL_CLASS = Literal["WorkflowInvocationStep"]
 INVOCATION_REPORT_MODEL_CLASS = Literal["Report"]
 IMPLICIT_COLLECTION_JOBS_MODEL_CLASS = Literal["ImplicitCollectionJobs"]
 
 OptionalNumberT = Annotated[Optional[Union[int, float]], Field(None)]
 
+TAG_ITEM_PATTERN = r"^([^\s.:])+(\.[^\s.:]+)*(:\S+)?$"
+
 
 class DatasetState(str, Enum):
     NEW = "new"
     UPLOAD = "upload"
     QUEUED = "queued"
     RUNNING = "running"
     OK = "ok"
@@ -523,15 +525,15 @@
     library_folder = "library_folder"
     new_collection = "new_collection"
 
 
 DatasetCollectionInstanceType = Literal["history", "library"]
 
 
-TagItem = Annotated[str, Field(..., pattern=r"^([^\s.:])+(.[^\s.:]+)*(:[^\s.:]+)?$")]
+TagItem = Annotated[str, Field(..., pattern=TAG_ITEM_PATTERN)]
 
 
 class TagCollection(RootModel):
     """Represents the collection of tags associated with an item."""
 
     root: List[TagItem] = Field(
         default=...,
@@ -965,21 +967,21 @@
         description="The position index of this element inside the collection.",
     )
     element_identifier: str = Field(
         ...,
         title="Element Identifier",
         description="The actual name of this element.",
     )
-    element_type: DCEType = Field(
-        ...,
+    element_type: Optional[DCEType] = Field(
+        None,
         title="Element Type",
         description="The type of the element. Used to interpret the `object` field.",
     )
-    object: Union[HDAObject, HDADetailed, DCObject] = Field(
-        ...,
+    object: Optional[Union[HDAObject, HDADetailed, DCObject]] = Field(
+        None,
         title="Object",
         description="The element's specific data depending on the value of `element_type`.",
     )
 
 
 DCObject.model_rebuild()
```

### Comparing `galaxy-schema-24.0.0/galaxy/schema/storage_cleaner.py` & `galaxy_schema-24.0.1/galaxy/schema/storage_cleaner.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/tasks.py` & `galaxy_schema-24.0.1/galaxy/schema/tasks.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/types.py` & `galaxy_schema-24.0.1/galaxy/schema/types.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/visualization.py` & `galaxy_schema-24.0.1/galaxy/schema/visualization.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/workflow/comments.py` & `galaxy_schema-24.0.1/galaxy/schema/workflow/comments.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy/schema/workflows.py` & `galaxy_schema-24.0.1/galaxy/schema/workflows.py`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/galaxy_schema.egg-info/PKG-INFO` & `galaxy_schema-24.0.1/galaxy_schema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-schema
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,26 @@
 
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
+* Fix tag regex pattern by `@jdavcs <https://github.com/jdavcs>`_ in `#18025 <https://github.com/galaxyproject/galaxy/pull/18025>`_
+* Fix History Dataset Association creation so that hid is always set by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18036 <https://github.com/galaxyproject/galaxy/pull/18036>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-schema-24.0.0/galaxy_schema.egg-info/SOURCES.txt` & `galaxy_schema-24.0.1/galaxy_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-schema-24.0.0/setup.cfg` & `galaxy_schema-24.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-schema
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	pydantic[email]>=2,!=2.6.0,!=2.6.1
 packages = find:
```

