# Comparing `tmp/dagster-duckdb-polars-0.23.3.tar.gz` & `tmp/dagster-duckdb-polars-0.23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-polars-0.23.3.tar", last modified: Thu Apr 25 20:20:57 2024, max compression
+gzip compressed data, was "dagster-duckdb-polars-0.23.4.tar", last modified: Thu May  2 20:39:40 2024, max compression
```

## Comparing `dagster-duckdb-polars-0.23.3.tar` & `dagster-duckdb-polars-0.23.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:57.809806 dagster-duckdb-polars-0.23.3/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagster-duckdb-polars-0.23.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-25 20:08:31.000000 dagster-duckdb-polars-0.23.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      672 2024-04-25 20:20:57.809806 dagster-duckdb-polars-0.23.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      149 2024-04-25 20:08:31.000000 dagster-duckdb-polars-0.23.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:57.805806 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars/
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-25 20:08:31.000000 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8910 2024-04-25 20:08:31.000000 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars/duckdb_polars_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-25 20:08:31.000000 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-25 20:08:31.000000 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:57.809806 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars.egg-info/
--rw-r--r--   0 root         (0) root         (0)      672 2024-04-25 20:20:57.000000 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2024-04-25 20:20:57.000000 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:20:57.000000 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:20:57.000000 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       54 2024-04-25 20:20:57.000000 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-25 20:20:57.000000 dagster-duckdb-polars-0.23.3/dagster_duckdb_polars.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-25 20:20:57.809806 dagster-duckdb-polars-0.23.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1380 2024-04-25 20:08:31.000000 dagster-duckdb-polars-0.23.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:39:40.029102 dagster-duckdb-polars-0.23.4/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:41.000000 dagster-duckdb-polars-0.23.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-02 20:31:41.000000 dagster-duckdb-polars-0.23.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      672 2024-05-02 20:39:40.029102 dagster-duckdb-polars-0.23.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      149 2024-05-02 20:31:41.000000 dagster-duckdb-polars-0.23.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:39:40.029102 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars/
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-02 20:31:41.000000 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8910 2024-05-02 20:31:41.000000 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars/duckdb_polars_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-02 20:31:41.000000 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:41.000000 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:39:40.029102 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      672 2024-05-02 20:39:39.000000 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2024-05-02 20:39:39.000000 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:39:39.000000 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:39:39.000000 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-02 20:39:39.000000 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-02 20:39:39.000000 dagster-duckdb-polars-0.23.4/dagster_duckdb_polars.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-02 20:39:40.033102 dagster-duckdb-polars-0.23.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1380 2024-05-02 20:31:41.000000 dagster-duckdb-polars-0.23.4/setup.py
```

### Comparing `dagster-duckdb-polars-0.23.3/LICENSE` & `dagster-duckdb-polars-0.23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.23.3/PKG-INFO` & `dagster-duckdb-polars-0.23.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.23.3
+Version: 0.23.4
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckdb-polars
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-polars-0.23.3/dagster_duckdb_polars/duckdb_polars_type_handler.py` & `dagster-duckdb-polars-0.23.4/dagster_duckdb_polars/duckdb_polars_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.23.3/dagster_duckdb_polars.egg-info/PKG-INFO` & `dagster-duckdb-polars-0.23.4/dagster_duckdb_polars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.23.3
+Version: 0.23.4
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckdb-polars
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-polars-0.23.3/setup.py` & `dagster-duckdb-polars-0.23.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_polars_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.3",
-        "dagster-duckdb==0.23.3",
+        "dagster==1.7.4",
+        "dagster-duckdb==0.23.4",
         "polars[pyarrow]",
     ],
     zip_safe=False,
 )
```

