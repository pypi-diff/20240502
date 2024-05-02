# Comparing `tmp/galaxy-job-execution-24.0.0.tar.gz` & `tmp/galaxy_job_execution-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-job-execution-24.0.0.tar", last modified: Wed Apr  3 02:45:58 2024, max compression
+gzip compressed data, was "galaxy_job_execution-24.0.1.tar", last modified: Thu May  2 13:49:04 2024, max compression
```

## Comparing `galaxy-job-execution-24.0.0.tar` & `galaxy_job_execution-24.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.979687 galaxy-job-execution-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-03 02:45:58.979687 galaxy-job-execution-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.975687 galaxy-job-execution-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.975687 galaxy-job-execution-24.0.0/galaxy/job_execution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.975687 galaxy-job-execution-24.0.0/galaxy/job_execution/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25642 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/actions/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/compute_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/container_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    33276 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/output_collect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.975687 galaxy-job-execution-24.0.0/galaxy/job_execution/ports/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/ports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/ports/view.py
--rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.975687 galaxy-job-execution-24.0.0/galaxy/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    14491 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28288 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/metadata/set_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.979687 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-03 02:45:58.979687 galaxy-job-execution-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:04.073993 galaxy_job_execution-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-02 13:49:04.073993 galaxy_job_execution-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:04.069993 galaxy_job_execution-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:04.069993 galaxy_job_execution-24.0.1/galaxy/job_execution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/job_execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:04.069993 galaxy_job_execution-24.0.1/galaxy/job_execution/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/job_execution/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25642 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/job_execution/actions/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/job_execution/compute_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/job_execution/container_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/job_execution/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33276 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/job_execution/output_collect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:04.069993 galaxy_job_execution-24.0.1/galaxy/job_execution/ports/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/job_execution/ports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/job_execution/ports/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/job_execution/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:04.069993 galaxy_job_execution-24.0.1/galaxy/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    14491 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28288 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/metadata/set_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:04.073993 galaxy_job_execution-24.0.1/galaxy_job_execution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-02 13:49:04.000000 galaxy_job_execution-24.0.1/galaxy_job_execution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-02 13:49:04.000000 galaxy_job_execution-24.0.1/galaxy_job_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:49:04.000000 galaxy_job_execution-24.0.1/galaxy_job_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-02 13:49:04.000000 galaxy_job_execution-24.0.1/galaxy_job_execution.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 13:49:04.000000 galaxy_job_execution-24.0.1/galaxy_job_execution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:49:04.000000 galaxy_job_execution-24.0.1/galaxy_job_execution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-02 13:49:04.073993 galaxy_job_execution-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_job_execution-24.0.1/test-requirements.txt
```

### Comparing `galaxy-job-execution-24.0.0/HISTORY.rst` & `galaxy_job_execution-24.0.1/HISTORY.rst`

 * *Files 1% similar despite different names*

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

### Comparing `galaxy-job-execution-24.0.0/LICENSE` & `galaxy_job_execution-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-24.0.0/PKG-INFO` & `galaxy_job_execution-24.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-job-execution
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy job execution runtime utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -49,14 +49,20 @@
 
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

### Comparing `galaxy-job-execution-24.0.0/galaxy/job_execution/actions/post.py` & `galaxy_job_execution-24.0.1/galaxy/job_execution/actions/post.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-24.0.0/galaxy/job_execution/compute_environment.py` & `galaxy_job_execution-24.0.1/galaxy/job_execution/compute_environment.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-24.0.0/galaxy/job_execution/container_monitor.py` & `galaxy_job_execution-24.0.1/galaxy/job_execution/container_monitor.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-24.0.0/galaxy/job_execution/datasets.py` & `galaxy_job_execution-24.0.1/galaxy/job_execution/datasets.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-24.0.0/galaxy/job_execution/output_collect.py` & `galaxy_job_execution-24.0.1/galaxy/job_execution/output_collect.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-24.0.0/galaxy/job_execution/ports/view.py` & `galaxy_job_execution-24.0.1/galaxy/job_execution/ports/view.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-24.0.0/galaxy/job_execution/setup.py` & `galaxy_job_execution-24.0.1/galaxy/job_execution/setup.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-24.0.0/galaxy/metadata/__init__.py` & `galaxy_job_execution-24.0.1/galaxy/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-24.0.0/galaxy/metadata/set_metadata.py` & `galaxy_job_execution-24.0.1/galaxy/metadata/set_metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/PKG-INFO` & `galaxy_job_execution-24.0.1/galaxy_job_execution.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-job-execution
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy job execution runtime utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -49,14 +49,20 @@
 
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

### Comparing `galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/SOURCES.txt` & `galaxy_job_execution-24.0.1/galaxy_job_execution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-24.0.0/setup.cfg` & `galaxy_job_execution-24.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-job-execution
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-files
 	galaxy-objectstore
```

