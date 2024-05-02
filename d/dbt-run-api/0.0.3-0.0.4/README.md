# Comparing `tmp/dbt_run_api-0.0.3.tar.gz` & `tmp/dbt_run_api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_run_api-0.0.3.tar", last modified: Wed May  1 09:40:08 2024, max compression
+gzip compressed data, was "dbt_run_api-0.0.4.tar", last modified: Thu May  2 13:19:22 2024, max compression
```

## Comparing `dbt_run_api-0.0.3.tar` & `dbt_run_api-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 09:40:08.854694 dbt_run_api-0.0.3/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 09:40:08.850694 dbt_run_api-0.0.3/.github/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 09:40:08.850694 dbt_run_api-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1000) runner    (1000)     1095 2024-05-01 09:39:47.000000 dbt_run_api-0.0.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1000) runner    (1000)      673 2024-05-01 09:39:47.000000 dbt_run_api-0.0.3/.github/workflows/generate_tag.yml
--rw-r--r--   0 runner    (1000) runner    (1000)     3084 2024-05-01 09:39:47.000000 dbt_run_api-0.0.3/.gitignore
--rw-r--r--   0 runner    (1000) runner    (1000)      787 2024-05-01 09:39:47.000000 dbt_run_api-0.0.3/Dockerfile
--rw-r--r--   0 runner    (1000) runner    (1000)     1060 2024-05-01 09:39:47.000000 dbt_run_api-0.0.3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1458 2024-05-01 09:40:08.854694 dbt_run_api-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      989 2024-05-01 09:39:47.000000 dbt_run_api-0.0.3/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 09:40:08.854694 dbt_run_api-0.0.3/dbt_run_api/
--rw-r--r--   0 runner    (1000) runner    (1000)     1530 2024-05-01 09:39:47.000000 dbt_run_api-0.0.3/dbt_run_api/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 09:40:08.854694 dbt_run_api-0.0.3/dbt_run_api.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1458 2024-05-01 09:40:08.000000 dbt_run_api-0.0.3/dbt_run_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      372 2024-05-01 09:40:08.000000 dbt_run_api-0.0.3/dbt_run_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-01 09:40:08.000000 dbt_run_api-0.0.3/dbt_run_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       50 2024-05-01 09:40:08.000000 dbt_run_api-0.0.3/dbt_run_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-05-01 09:40:08.000000 dbt_run_api-0.0.3/dbt_run_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      601 2024-05-01 09:39:47.000000 dbt_run_api-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       76 2024-05-01 09:39:47.000000 dbt_run_api-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-01 09:40:08.854694 dbt_run_api-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-01 09:40:08.854694 dbt_run_api-0.0.3/test/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-05-01 09:39:47.000000 dbt_run_api-0.0.3/test/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      739 2024-05-01 09:39:47.000000 dbt_run_api-0.0.3/test/test_dbtrunner.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-02 13:19:22.276463 dbt_run_api-0.0.4/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-02 13:19:22.272463 dbt_run_api-0.0.4/.github/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-02 13:19:22.272463 dbt_run_api-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1095 2024-05-02 13:18:57.000000 dbt_run_api-0.0.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1000) runner    (1000)      673 2024-05-02 13:18:57.000000 dbt_run_api-0.0.4/.github/workflows/generate_tag.yml
+-rw-r--r--   0 runner    (1000) runner    (1000)     3084 2024-05-02 13:18:57.000000 dbt_run_api-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1000) runner    (1000)      787 2024-05-02 13:18:57.000000 dbt_run_api-0.0.4/Dockerfile
+-rw-r--r--   0 runner    (1000) runner    (1000)     1060 2024-05-02 13:18:57.000000 dbt_run_api-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1458 2024-05-02 13:19:22.276463 dbt_run_api-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      989 2024-05-02 13:18:57.000000 dbt_run_api-0.0.4/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-02 13:19:22.272463 dbt_run_api-0.0.4/dbt_run_api/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2372 2024-05-02 13:18:57.000000 dbt_run_api-0.0.4/dbt_run_api/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-02 13:19:22.276463 dbt_run_api-0.0.4/dbt_run_api.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1458 2024-05-02 13:19:22.000000 dbt_run_api-0.0.4/dbt_run_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      372 2024-05-02 13:19:22.000000 dbt_run_api-0.0.4/dbt_run_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-02 13:19:22.000000 dbt_run_api-0.0.4/dbt_run_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       50 2024-05-02 13:19:22.000000 dbt_run_api-0.0.4/dbt_run_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-05-02 13:19:22.000000 dbt_run_api-0.0.4/dbt_run_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      601 2024-05-02 13:18:57.000000 dbt_run_api-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       76 2024-05-02 13:18:57.000000 dbt_run_api-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-02 13:19:22.276463 dbt_run_api-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-02 13:19:22.276463 dbt_run_api-0.0.4/test/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-05-02 13:18:57.000000 dbt_run_api-0.0.4/test/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      739 2024-05-02 13:18:57.000000 dbt_run_api-0.0.4/test/test_dbtrunner.py
```

### Comparing `dbt_run_api-0.0.3/.github/workflows/build.yml` & `dbt_run_api-0.0.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `dbt_run_api-0.0.3/.github/workflows/generate_tag.yml` & `dbt_run_api-0.0.4/.github/workflows/generate_tag.yml`

 * *Files identical despite different names*

### Comparing `dbt_run_api-0.0.3/.gitignore` & `dbt_run_api-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_run_api-0.0.3/Dockerfile` & `dbt_run_api-0.0.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `dbt_run_api-0.0.3/LICENSE` & `dbt_run_api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_run_api-0.0.3/PKG-INFO` & `dbt_run_api-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-run-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `dbt_run_api-0.0.3/README.md` & `dbt_run_api-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_run_api-0.0.3/dbt_run_api.egg-info/PKG-INFO` & `dbt_run_api-0.0.4/dbt_run_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-run-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `dbt_run_api-0.0.3/pyproject.toml` & `dbt_run_api-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_run_api-0.0.3/test/test_dbtrunner.py` & `dbt_run_api-0.0.4/test/test_dbtrunner.py`

 * *Files identical despite different names*

