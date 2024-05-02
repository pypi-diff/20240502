# Comparing `tmp/rinch_sql-8.5.0.tar.gz` & `tmp/rinch_sql-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rinch_sql-8.5.0.tar", last modified: Thu Feb 29 09:59:59 2024, max compression
+gzip compressed data, was "rinch_sql-9.0.0.tar", last modified: Fri Mar  1 01:19:43 2024, max compression
```

## Comparing `rinch_sql-8.5.0.tar` & `rinch_sql-9.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:59:59.026573 rinch_sql-8.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:59:59.018573 rinch_sql-8.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:59:59.022573 rinch_sql-8.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-02-29 09:59:59.026573 rinch_sql-8.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:59:59.022573 rinch_sql-8.5.0/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:59:59.022573 rinch_sql-8.5.0/example/example1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:59:59.022573 rinch_sql-8.5.0/example/example1/table/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/example/example1/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/example/example1/table/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/example/example1/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:59:59.022573 rinch_sql-8.5.0/example/example2/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/example/example2/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:59:59.022573 rinch_sql-8.5.0/example/example2/table/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/example/example2/table/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/example/example2/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/push.sh
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/push_with_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:59:59.022573 rinch_sql-8.5.0/rinch_sql/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/rinch_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/rinch_sql/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/rinch_sql/creator.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/rinch_sql/db_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/rinch_sql/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/rinch_sql/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/rinch_sql/sql_static.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/rinch_sql/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-29 09:59:46.000000 rinch_sql-8.5.0/rinch_sql/use_var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:59:59.026573 rinch_sql-8.5.0/rinch_sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-02-29 09:59:58.000000 rinch_sql-8.5.0/rinch_sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-29 09:59:59.000000 rinch_sql-8.5.0/rinch_sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 09:59:58.000000 rinch_sql-8.5.0/rinch_sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-29 09:59:58.000000 rinch_sql-8.5.0/rinch_sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-29 09:59:58.000000 rinch_sql-8.5.0/rinch_sql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 09:59:59.026573 rinch_sql-8.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 01:19:43.063122 rinch_sql-9.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 01:19:43.055122 rinch_sql-9.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 01:19:43.059122 rinch_sql-9.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-01 01:19:43.063122 rinch_sql-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 01:19:43.055122 rinch_sql-9.0.0/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 01:19:43.059122 rinch_sql-9.0.0/example/example1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 01:19:43.059122 rinch_sql-9.0.0/example/example1/table/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/example/example1/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/example/example1/table/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/example/example1/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 01:19:43.059122 rinch_sql-9.0.0/example/example2/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/example/example2/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 01:19:43.059122 rinch_sql-9.0.0/example/example2/table/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/example/example2/table/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/example/example2/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/push.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/push_with_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 01:19:43.059122 rinch_sql-9.0.0/rinch_sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/rinch_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/rinch_sql/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/rinch_sql/creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/rinch_sql/db_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/rinch_sql/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/rinch_sql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/rinch_sql/sql_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/rinch_sql/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-01 01:19:35.000000 rinch_sql-9.0.0/rinch_sql/use_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 01:19:43.063122 rinch_sql-9.0.0/rinch_sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-01 01:19:43.000000 rinch_sql-9.0.0/rinch_sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-01 01:19:43.000000 rinch_sql-9.0.0/rinch_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 01:19:43.000000 rinch_sql-9.0.0/rinch_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-01 01:19:43.000000 rinch_sql-9.0.0/rinch_sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-01 01:19:43.000000 rinch_sql-9.0.0/rinch_sql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 01:19:43.063122 rinch_sql-9.0.0/setup.cfg
```

### Comparing `rinch_sql-8.5.0/.github/workflows/publish.yml` & `rinch_sql-9.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `rinch_sql-8.5.0/.gitignore` & `rinch_sql-9.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rinch_sql-8.5.0/PKG-INFO` & `rinch_sql-9.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rinch_sql
-Version: 8.5.0
+Version: 9.0.0
 Summary: a simple orm in python based on [mysql,dataclass].
 Author-email: rinch wu <rinch.wu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/rinch-wu/rinch_sql
 Project-URL: Documentation, https://github.com/rinch-wu/rinch_sql
 Project-URL: Repository, https://github.com/rinch-wu/rinch_sql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rinch_sql-8.5.0/README.md` & `rinch_sql-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `rinch_sql-8.5.0/example/example1/task.py` & `rinch_sql-9.0.0/example/example1/task.py`

 * *Files identical despite different names*

### Comparing `rinch_sql-8.5.0/example/example2/task.py` & `rinch_sql-9.0.0/example/example2/task.py`

 * *Files identical despite different names*

### Comparing `rinch_sql-8.5.0/pyproject.toml` & `rinch_sql-9.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rinch_sql-8.5.0/rinch_sql/creator.py` & `rinch_sql-9.0.0/rinch_sql/creator.py`

 * *Files identical despite different names*

### Comparing `rinch_sql-8.5.0/rinch_sql/db_config.py` & `rinch_sql-9.0.0/rinch_sql/db_config.py`

 * *Files identical despite different names*

### Comparing `rinch_sql-8.5.0/rinch_sql/mysql.py` & `rinch_sql-9.0.0/rinch_sql/mysql.py`

 * *Files identical despite different names*

### Comparing `rinch_sql-8.5.0/rinch_sql/sql.py` & `rinch_sql-9.0.0/rinch_sql/sql.py`

 * *Files identical despite different names*

### Comparing `rinch_sql-8.5.0/rinch_sql/sql_static.py` & `rinch_sql-9.0.0/rinch_sql/sql_static.py`

 * *Files identical despite different names*

### Comparing `rinch_sql-8.5.0/rinch_sql.egg-info/PKG-INFO` & `rinch_sql-9.0.0/rinch_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rinch_sql
-Version: 8.5.0
+Version: 9.0.0
 Summary: a simple orm in python based on [mysql,dataclass].
 Author-email: rinch wu <rinch.wu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/rinch-wu/rinch_sql
 Project-URL: Documentation, https://github.com/rinch-wu/rinch_sql
 Project-URL: Repository, https://github.com/rinch-wu/rinch_sql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rinch_sql-8.5.0/rinch_sql.egg-info/SOURCES.txt` & `rinch_sql-9.0.0/rinch_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

