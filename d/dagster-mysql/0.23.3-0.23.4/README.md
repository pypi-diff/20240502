# Comparing `tmp/dagster-mysql-0.23.3.tar.gz` & `tmp/dagster-mysql-0.23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mysql-0.23.3.tar", last modified: Thu Apr 25 20:20:15 2024, max compression
+gzip compressed data, was "dagster-mysql-0.23.4.tar", last modified: Thu May  2 20:41:52 2024, max compression
```

## Comparing `dagster-mysql-0.23.3.tar` & `dagster-mysql-0.23.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:15.030190 dagster-mysql-0.23.3/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      126 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-25 20:20:15.030190 dagster-mysql-0.23.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      125 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:15.026190 dagster-mysql-0.23.3/dagster_mysql/
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:15.030190 dagster-mysql-0.23.3/dagster_mysql/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/alembic/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:15.030190 dagster-mysql-0.23.3/dagster_mysql/event_log/
--rw-r--r--   0 root         (0) root         (0)       68 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8490 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/event_log/event_log.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:15.030190 dagster-mysql-0.23.3/dagster_mysql/run_storage/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/run_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7307 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/run_storage/run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:15.030190 dagster-mysql-0.23.3/dagster_mysql/schedule_storage/
--rw-r--r--   0 root         (0) root         (0)       75 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/schedule_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7590 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/schedule_storage/schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     3742 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/storage.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/dagster_mysql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:15.030190 dagster-mysql-0.23.3/dagster_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-25 20:20:14.000000 dagster-mysql-0.23.3/dagster_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      704 2024-04-25 20:20:14.000000 dagster-mysql-0.23.3/dagster_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:20:14.000000 dagster-mysql-0.23.3/dagster_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:20:14.000000 dagster-mysql-0.23.3/dagster_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 20:20:14.000000 dagster-mysql-0.23.3/dagster_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-25 20:20:14.000000 dagster-mysql-0.23.3/dagster_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-25 20:20:15.030190 dagster-mysql-0.23.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1286 2024-04-25 20:08:31.000000 dagster-mysql-0.23.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:41:52.439896 dagster-mysql-0.23.4/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      126 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      588 2024-05-02 20:41:52.439896 dagster-mysql-0.23.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:41:52.435896 dagster-mysql-0.23.4/dagster_mysql/
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:41:52.435896 dagster-mysql-0.23.4/dagster_mysql/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/alembic/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:41:52.435896 dagster-mysql-0.23.4/dagster_mysql/event_log/
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8490 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/event_log/event_log.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:41:52.439896 dagster-mysql-0.23.4/dagster_mysql/run_storage/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/run_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7307 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/run_storage/run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:41:52.439896 dagster-mysql-0.23.4/dagster_mysql/schedule_storage/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/schedule_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/schedule_storage/schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3742 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/storage.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/dagster_mysql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:41:52.435896 dagster-mysql-0.23.4/dagster_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      588 2024-05-02 20:41:52.000000 dagster-mysql-0.23.4/dagster_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      704 2024-05-02 20:41:52.000000 dagster-mysql-0.23.4/dagster_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:41:52.000000 dagster-mysql-0.23.4/dagster_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:41:52.000000 dagster-mysql-0.23.4/dagster_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 20:41:52.000000 dagster-mysql-0.23.4/dagster_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-02 20:41:52.000000 dagster-mysql-0.23.4/dagster_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2024-05-02 20:41:52.443896 dagster-mysql-0.23.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-05-02 20:31:41.000000 dagster-mysql-0.23.4/setup.py
```

### Comparing `dagster-mysql-0.23.3/LICENSE` & `dagster-mysql-0.23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.3/PKG-INFO` & `dagster-mysql-0.23.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.23.3
+Version: 0.23.4
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mysql-0.23.3/dagster_mysql/alembic/alembic.ini` & `dagster-mysql-0.23.4/dagster_mysql/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.3/dagster_mysql/event_log/event_log.py` & `dagster-mysql-0.23.4/dagster_mysql/event_log/event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.3/dagster_mysql/run_storage/run_storage.py` & `dagster-mysql-0.23.4/dagster_mysql/run_storage/run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.3/dagster_mysql/schedule_storage/schedule_storage.py` & `dagster-mysql-0.23.4/dagster_mysql/schedule_storage/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.3/dagster_mysql/storage.py` & `dagster-mysql-0.23.4/dagster_mysql/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.3/dagster_mysql/utils.py` & `dagster-mysql-0.23.4/dagster_mysql/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.3/dagster_mysql.egg-info/PKG-INFO` & `dagster-mysql-0.23.4/dagster_mysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.23.3
+Version: 0.23.4
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mysql-0.23.3/dagster_mysql.egg-info/SOURCES.txt` & `dagster-mysql-0.23.4/dagster_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.23.3/setup.py` & `dagster-mysql-0.23.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,10 +33,10 @@
     package_data={
         "dagster-mysql": [
             "dagster_mysql/alembic/*",
         ]
     },
     include_package_data=True,
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.3", "mysql-connector-python"],
+    install_requires=["dagster==1.7.4", "mysql-connector-python"],
     zip_safe=False,
 )
```

