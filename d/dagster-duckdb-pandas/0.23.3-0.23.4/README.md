# Comparing `tmp/dagster-duckdb-pandas-0.23.3.tar.gz` & `tmp/dagster-duckdb-pandas-0.23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pandas-0.23.3.tar", last modified: Thu Apr 25 20:17:34 2024, max compression
+gzip compressed data, was "dagster-duckdb-pandas-0.23.4.tar", last modified: Thu May  2 20:42:36 2024, max compression
```

## Comparing `dagster-duckdb-pandas-0.23.3.tar` & `dagster-duckdb-pandas-0.23.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:17:34.091631 dagster-duckdb-pandas-0.23.3/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagster-duckdb-pandas-0.23.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-25 20:08:31.000000 dagster-duckdb-pandas-0.23.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      671 2024-04-25 20:17:34.091631 dagster-duckdb-pandas-0.23.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      142 2024-04-25 20:08:31.000000 dagster-duckdb-pandas-0.23.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:17:34.087631 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas/
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-25 20:08:31.000000 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8658 2024-04-25 20:08:31.000000 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-25 20:08:31.000000 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-25 20:08:31.000000 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:17:34.091631 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      671 2024-04-25 20:17:33.000000 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2024-04-25 20:17:33.000000 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:17:33.000000 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:17:33.000000 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-25 20:17:33.000000 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-25 20:17:33.000000 dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-25 20:17:34.091631 dagster-duckdb-pandas-0.23.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1508 2024-04-25 20:08:31.000000 dagster-duckdb-pandas-0.23.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:42:36.863494 dagster-duckdb-pandas-0.23.4/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:41.000000 dagster-duckdb-pandas-0.23.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-02 20:31:41.000000 dagster-duckdb-pandas-0.23.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      671 2024-05-02 20:42:36.863494 dagster-duckdb-pandas-0.23.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-02 20:31:41.000000 dagster-duckdb-pandas-0.23.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:42:36.863494 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas/
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-02 20:31:41.000000 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8658 2024-05-02 20:31:41.000000 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-02 20:31:41.000000 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:41.000000 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:42:36.863494 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      671 2024-05-02 20:42:36.000000 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2024-05-02 20:42:36.000000 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:42:36.000000 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:42:36.000000 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-02 20:42:36.000000 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-02 20:42:36.000000 dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-02 20:42:36.863494 dagster-duckdb-pandas-0.23.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1508 2024-05-02 20:31:41.000000 dagster-duckdb-pandas-0.23.4/setup.py
```

### Comparing `dagster-duckdb-pandas-0.23.3/LICENSE` & `dagster-duckdb-pandas-0.23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pandas-0.23.3/PKG-INFO` & `dagster-duckdb-pandas-0.23.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.23.3
+Version: 0.23.4
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas/duckdb_pandas_type_handler.py` & `dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas/duckdb_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pandas-0.23.3/dagster_duckdb_pandas.egg-info/PKG-INFO` & `dagster-duckdb-pandas-0.23.4/dagster_duckdb_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.23.3
+Version: 0.23.4
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pandas-0.23.3/setup.py` & `dagster-duckdb-pandas-0.23.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pandas_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.3",
-        "dagster-duckdb==0.23.3",
+        "dagster==1.7.4",
+        "dagster-duckdb==0.23.4",
         # Pinned pending duckdb removal of broken pandas import. Pin can be
         # removed as soon as it produces a working build.
         "pandas<2.1",
     ],
     zip_safe=False,
 )
```

