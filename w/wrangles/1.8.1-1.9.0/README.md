# Comparing `tmp/wrangles-1.8.1.tar.gz` & `tmp/wrangles-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrangles-1.8.1.tar", last modified: Thu Feb  1 19:22:36 2024, max compression
+gzip compressed data, was "wrangles-1.9.0.tar", last modified: Mon Mar 25 16:23:39 2024, max compression
```

## Comparing `wrangles-1.8.1.tar` & `wrangles-1.9.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:22:36.734143 wrangles-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-02-01 19:22:36.734143 wrangles-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-02-01 19:22:29.000000 wrangles-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-01 19:22:36.734143 wrangles-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-01 19:22:29.000000 wrangles-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:22:36.722143 wrangles-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-02-01 19:22:29.000000 wrangles-1.8.1/tests/test_back_ processes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-02-01 19:22:29.000000 wrangles-1.8.1/tests/test_wrangles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:22:36.726143 wrangles-1.8.1/wrangles/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:22:36.730143 wrangles-1.8.1/wrangles/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/akeneo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/ckan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    15724 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/pricefx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/sftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/connectors/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    35385 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/recipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:22:36.734143 wrangles-1.8.1/wrangles/recipe_wrangles/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/recipe_wrangles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/recipe_wrangles/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/recipe_wrangles/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    27133 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/recipe_wrangles/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/recipe_wrangles/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    34017 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/recipe_wrangles/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/recipe_wrangles/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/recipe_wrangles/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    19389 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/recipe_wrangles/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/recipe_wrangles/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/standardize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-02-01 19:22:29.000000 wrangles-1.8.1/wrangles/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:22:36.734143 wrangles-1.8.1/wrangles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-02-01 19:22:36.000000 wrangles-1.8.1/wrangles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-01 19:22:36.000000 wrangles-1.8.1/wrangles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 19:22:36.000000 wrangles-1.8.1/wrangles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-01 19:22:36.000000 wrangles-1.8.1/wrangles.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-01 19:22:36.000000 wrangles-1.8.1/wrangles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-01 19:22:36.000000 wrangles-1.8.1/wrangles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:23:39.747118 wrangles-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-25 16:23:39.747118 wrangles-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-03-25 16:23:36.000000 wrangles-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-25 16:23:39.747118 wrangles-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-25 16:23:36.000000 wrangles-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:23:39.735118 wrangles-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-25 16:23:36.000000 wrangles-1.9.0/tests/test_back_ processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-03-25 16:23:36.000000 wrangles-1.9.0/tests/test_wrangles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:23:39.739118 wrangles-1.9.0/wrangles/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:23:39.743118 wrangles-1.9.0/wrangles/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/akeneo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/ckan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15724 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/pricefx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/connectors/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35385 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/recipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:23:39.747118 wrangles-1.9.0/wrangles/recipe_wrangles/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/recipe_wrangles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/recipe_wrangles/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/recipe_wrangles/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27427 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/recipe_wrangles/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/recipe_wrangles/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34017 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/recipe_wrangles/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/recipe_wrangles/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/recipe_wrangles/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19389 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/recipe_wrangles/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/recipe_wrangles/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/standardize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-03-25 16:23:36.000000 wrangles-1.9.0/wrangles/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:23:39.747118 wrangles-1.9.0/wrangles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-25 16:23:39.000000 wrangles-1.9.0/wrangles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-25 16:23:39.000000 wrangles-1.9.0/wrangles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 16:23:39.000000 wrangles-1.9.0/wrangles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-25 16:23:39.000000 wrangles-1.9.0/wrangles.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-25 16:23:39.000000 wrangles-1.9.0/wrangles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 16:23:39.000000 wrangles-1.9.0/wrangles.egg-info/top_level.txt
```

### Comparing `wrangles-1.8.1/PKG-INFO` & `wrangles-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrangles
-Version: 1.8.1
+Version: 1.9.0
 Summary: Wrangle your data into shape with AI
 Home-page: https://github.com/wrangleworks/WranglesPy
 Author: WrangleWorks
 Author-email: chris@wrangleworks.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/wrangleworks/WranglesPy/issues
 Project-URL: Documentation, https://wrangles.io/python
```

### Comparing `wrangles-1.8.1/README.md` & `wrangles-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/setup.py` & `wrangles-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     license_files = ('LICENSE.txt',),
     license = 'Apache License 2.0',
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent'
     ],
-    version = '1.8.1',
+    version = '1.9.0',
     url = 'https://github.com/wrangleworks/WranglesPy',
     author = 'WrangleWorks',
     author_email = 'chris@wrangleworks.com',
     keywords = ['data','wrangling'],
     install_requires = requirements,
     entry_points ={
         'console_scripts': ['wrangles.recipe = wrangles.console:recipe']
```

### Comparing `wrangles-1.8.1/tests/test_back_ processes.py` & `wrangles-1.9.0/tests/test_back_ processes.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/tests/test_wrangles.py` & `wrangles-1.9.0/tests/test_wrangles.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/__init__.py` & `wrangles-1.9.0/wrangles/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/auth.py` & `wrangles-1.9.0/wrangles/auth.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/batching.py` & `wrangles-1.9.0/wrangles/batching.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/classify.py` & `wrangles-1.9.0/wrangles/classify.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/config.py` & `wrangles-1.9.0/wrangles/config.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/akeneo.py` & `wrangles-1.9.0/wrangles/connectors/akeneo.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/ckan.py` & `wrangles-1.9.0/wrangles/connectors/ckan.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/excel.py` & `wrangles-1.9.0/wrangles/connectors/excel.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/file.py` & `wrangles-1.9.0/wrangles/connectors/file.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/http.py` & `wrangles-1.9.0/wrangles/connectors/http.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/jinja.py` & `wrangles-1.9.0/wrangles/connectors/jinja.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/matrix.py` & `wrangles-1.9.0/wrangles/connectors/matrix.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/memory.py` & `wrangles-1.9.0/wrangles/connectors/memory.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/mongodb.py` & `wrangles-1.9.0/wrangles/connectors/mongodb.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/mssql.py` & `wrangles-1.9.0/wrangles/connectors/mssql.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/mysql.py` & `wrangles-1.9.0/wrangles/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/notification.py` & `wrangles-1.9.0/wrangles/connectors/notification.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/postgres.py` & `wrangles-1.9.0/wrangles/connectors/postgres.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/pricefx.py` & `wrangles-1.9.0/wrangles/connectors/pricefx.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/recipe.py` & `wrangles-1.9.0/wrangles/connectors/recipe.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/s3.py` & `wrangles-1.9.0/wrangles/connectors/s3.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/salesforce.py` & `wrangles-1.9.0/wrangles/connectors/salesforce.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/ssh.py` & `wrangles-1.9.0/wrangles/connectors/ssh.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/test.py` & `wrangles-1.9.0/wrangles/connectors/test.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/connectors/train.py` & `wrangles-1.9.0/wrangles/connectors/train.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/console.py` & `wrangles-1.9.0/wrangles/console.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/data.py` & `wrangles-1.9.0/wrangles/data.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/extract.py` & `wrangles-1.9.0/wrangles/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 
 def custom(
     input: _Union[str, list],
     model_id: str,
     first_element: bool = False,
     use_labels: bool = False,
     case_sensitive: bool = False,
+    extract_raw: bool = False,
     use_spellcheck: bool = False
 ) -> list:
     """
     Extract entities using a custom model.
     Requires WrangleWorks Account and Subscription.
 
     :param input: A string or list of strings to searched for information.
@@ -131,15 +132,16 @@
 
     url = f'{_config.api_host}/wrangles/extract/custom'
     params = {
         'responseFormat': 'array',
         'model_id': model_id,
         'use_labels': use_labels,
         'caseSensitive': case_sensitive,
-        'useSpellcheck': use_spellcheck
+        'extract_raw': extract_raw,
+        'use_spellcheck': use_spellcheck
     }
     model_properties = _data.model(model_id)
     # If model_id format is correct but no mode_id exists
     if model_properties.get('message', None) == 'error': raise ValueError('Incorrect model_id.\nmodel_id may be wrong or does not exists')
     batch_size = model_properties['batch_size'] or 10000
     
     # Using model_id in wrong function
```

### Comparing `wrangles-1.8.1/wrangles/format.py` & `wrangles-1.9.0/wrangles/format.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,38 +18,47 @@
     else:
         return [
             concat_char.join([str(x) for x in row])
             for row in data_list
         ]
 
 
-# Super Mario Function
-def split_re(input_list, split_char, output):
-    # split char is a list of characters -> Joining them
-    if isinstance(split_char, list):
-        split_char = '|'.join(split_char)
-    
-    results = [_re.split(split_char, x) for x in input_list]
-    return results
+def split(input_list, split_char, output, pad=False, inclusive=False):
+    if split_char[:6] == 'regex:':
+            split_char = split_char[6:].strip()
+            results = [_re.split(split_char, x) for x in input_list]
+    else:
+        results = [x.split(split_char) for x in input_list]
 
+    if inclusive:
+        # Get the split stuff
+        inclusive_results = [_re.findall(split_char, x) for x in input_list]
+
+        # 'zip' together
+        merged_results = []
+        for i in range(len(results)):
+            temp = [None]*(len(results[i]) + len(inclusive_results[i]))
+            temp[::2] = results[i]
+            temp[1::2] = inclusive_results[i]
+            merged_results.append(temp)
+        
+        results = merged_results
 
-def split(input_list, split_char, output, pad=False):
     if pad:
         # Pad to be as long as the longest result
-        max_len = max([len(x.split(split_char)) for x in input_list])
-        results = [x.split(split_char) + [''] * (max_len - len(x.split(split_char))) for x in input_list]
+        max_len = max([len(x) for x in results])
+        results = [x + [''] * (max_len - len(x)) for x in results]
         
         # trimming list to appropriate output columns number
         if len(output) <= max_len and isinstance(output, list):
             results = [x[:len(output)] for x in results]
         # if more columns than number of splits, then add '' in extra columns
         elif len(output) >= max_len and isinstance(output, list):
             results = [x + [''] * (len(output) - len(x)) for x in results] 
-    else:
-        results = [x.split(split_char) for x in input_list]
+            
     return results
     
 
 def coalesce(input_list: list) -> list:
     """
     Return the first not empty result for each row
     where each row has a list of possibilities
```

### Comparing `wrangles-1.8.1/wrangles/openai.py` & `wrangles-1.9.0/wrangles/openai.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/recipe.py` & `wrangles-1.9.0/wrangles/recipe.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/recipe_wrangles/__init__.py` & `wrangles-1.9.0/wrangles/recipe_wrangles/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/recipe_wrangles/convert.py` & `wrangles-1.9.0/wrangles/recipe_wrangles/convert.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/recipe_wrangles/create.py` & `wrangles-1.9.0/wrangles/recipe_wrangles/create.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/recipe_wrangles/extract.py` & `wrangles-1.9.0/wrangles/recipe_wrangles/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,14 +427,15 @@
     df: _pd.DataFrame,
     input: _Union[str, list],
     model_id: _Union[str, list],
     output: _Union[str, list] = None,
     use_labels: bool = False,
     first_element: bool = False,
     case_sensitive: bool = False,
+    extract_raw: bool = False,
     use_spellcheck: bool = False
 ) -> _pd.DataFrame:
     """
     type: object
     description: Extract data from the input using a DIY or bespoke extraction wrangle. Requires WrangleWorks Account and Subscription.
     additionalProperties: true
     required:
@@ -461,17 +462,20 @@
         description: "Use Labels in the extract output {label: value}"
       first_element:
         type: boolean
         description: Get the first element from results
       case_sensitive:
         type: boolean
         description: Allows the wrangle to be case sensitive if set to True, default is False.
+      extract_raw:
+        type: boolean
+        description: Extract the raw data from the wrangle
       use_spellcheck:
         type: boolean
-        description: Use spellcheck to correct spelling mistakes in the input
+        description: Use spellcheck to also find minor mispellings compared to the reference data
     """
     if output is None: output = input
     
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
     if not isinstance(model_id, list): model_id = [model_id]
@@ -482,37 +486,40 @@
         for in_col, out_col, model in zip(input, output, model_id):
             df[out_col] = _extract.custom(
                 df[in_col].astype(str).tolist(),
                 model_id=model,
                 first_element=first_element,
                 use_labels=use_labels,
                 case_sensitive=case_sensitive,
+                extract_raw=extract_raw,
                 use_spellcheck=use_spellcheck
             )
     
     elif len(input) > 1 and len(output) == 1 and len(model_id) == 1:
         # if there are multiple inputs and one output and one model_id. concatenate the inputs
         df[output[0]] = _extract.custom(
             _format.concatenate(df[input].astype(str).values.tolist(), ' '),
             model_id=model_id[0],
             first_element=first_element,
             use_labels=use_labels,
             case_sensitive=case_sensitive,
+            extract_raw=extract_raw,
             use_spellcheck=use_spellcheck
         )
     
     else:
         # Iterate through the inputs, outputs and model_ids
         for in_col, out_col, model in zip(input, output, model_id):
             df[out_col] = _extract.custom(
                 df[in_col].astype(str).tolist(),
                 model_id=model,
                 first_element=first_element,
                 use_labels=use_labels,
                 case_sensitive=case_sensitive,
+                extract_raw=extract_raw,
                 use_spellcheck=use_spellcheck
             )
 
     return df
 
 
 def date_properties(df: _pd.DataFrame, input: _pd.Timestamp, property: str, output: str = None) -> _pd.DataFrame:
@@ -800,27 +807,28 @@
     """
     type: object
     description: Extract single values using regex
     additionalProperties: false
     required:
       - input
       - output
+      - find
     properties:
       input:
         type: 
           - string
           - array
-        description: Name of the input column.
-    output:
-      type: string
-      description: Name of the output column.
-      find:
-        type: 
+        description: Name of the input column(s).
+      output:
+        type:
           - string
           - array
+        description: Name of the output column(s).
+      find:
+        type: string
         description: Pattern to find using regex
     """
     # If output is not specified, overwrite input columns in place
     if output is None: output = input
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
```

### Comparing `wrangles-1.8.1/wrangles/recipe_wrangles/format.py` & `wrangles-1.9.0/wrangles/recipe_wrangles/format.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/recipe_wrangles/main.py` & `wrangles-1.9.0/wrangles/recipe_wrangles/main.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/recipe_wrangles/merge.py` & `wrangles-1.9.0/wrangles/recipe_wrangles/merge.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/recipe_wrangles/pandas.py` & `wrangles-1.9.0/wrangles/recipe_wrangles/pandas.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,22 @@
           - string
           - array
         description: Name of the output columns or columns
     """
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
+
+    # If input is a single column and output is multiple columns, repeat input
+    if len(input) == 1 and len(output) > 1:
+        input = input * len(output)
+
+    # If input is not the same length as output, raise error
+    if len(input) != len(output):
+        raise ValueError("Input and output must be the same length")
     
     for input_column, output_column in zip(input, output):
         df[output_column] = df[input_column].copy()
         
     return df
```

### Comparing `wrangles-1.8.1/wrangles/recipe_wrangles/select.py` & `wrangles-1.9.0/wrangles/recipe_wrangles/select.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/recipe_wrangles/split.py` & `wrangles-1.9.0/wrangles/recipe_wrangles/split.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,15 +87,23 @@
     else:
         # Else they should have provided a list for all the output columns
         df[output] = results
 
     return df
 
 
-def text(df: _pd.DataFrame, input: str, output: _Union[str, _list], char: str = ',', pad: bool = False, element: _Union[str, int] = None) -> _pd.DataFrame:
+def text(
+    df: _pd.DataFrame,
+    input: str,
+    output: _Union[str, _list],
+    char: str = ',',
+    pad: bool = False,
+    element: _Union[int, str] = None,
+    inclusive: bool = False
+) -> _pd.DataFrame:
     """
     type: object
     description: Split a string to multiple columns or a list.
     additionalProperties: false
     required:
       - input
       - output
@@ -105,61 +113,46 @@
         description: Name of the column to be split
       output:
         type:
           - string
           - array
         description: Name of the output column
       char:
-        type: 
-          - string
-          - array
+        type: string
         description: (Optional) Set the character(s) to split on. Default comma (,)
       pad:
         type: boolean
         description: (Optional) If outputting to a list, choose whether to pad to a consistent length. Default False
       element:
         type: 
           - integer
           - string
         description: (Optional) Select a specific element or range after splitting
+      inclusive:
+        type: boolean
+        description: (Optional) Include the split character in the output. Default False
     """
-    # If char is a list -> split on multiple chars using regex
-    if isinstance(char, _list) and '*' not in output:
-      df[output] = _format.split_re(df[input].astype(str).tolist(), char, output)
-      return df
-      
-    # Wildcard with multiple split and multiple char
-    if isinstance(output, str) and '*' in output and isinstance(char, _list):
-        # If user has entered a wildcard in the output column name
-        # then add results to that with an incrementing index for each column
-        # column * -> column 1, column 2, column 3...
-        results = _format.split_re(df[input].astype(str).tolist(), char, output)
-        output_headers = []
-        for i in range(1, len(results[0]) + 1):
-            output_headers.append(output.replace('*', str(i)))
-        df[output_headers] = results
-        return df
-        
-    # Wildcard with multiple splits 
+    # If output is a list, then pad to a consistent length
+    if isinstance(output, str) and '*' in output or isinstance(output, _list):
+        pad = True
+
+    results = _format.split(df[input].astype(str).tolist(), char, output, pad, inclusive)
+
     if isinstance(output, str) and '*' in output:
         # If user has entered a wildcard in the output column name
         # then add results to that with an incrementing index for each column
         # column * -> column 1, column 2, column 3...
-        results = _format.split(df[input].astype(str).tolist(), char, output, pad=True)
         output_headers = []
         for i in range(1, len(results[0]) + 1):
             output_headers.append(output.replace('*', str(i)))
         df[output_headers] = results
 
-    elif isinstance(output, str) and not pad:
+    else:
         # User has given a single column - return as a list within that column
-        df[output] = _format.split(df[input].astype(str).tolist(), char, output)
-
-    elif isinstance(output, _list) or pad:
-        df[output] = _format.split(df[input].astype(str).tolist(), char, output, pad=True)
+        df[output] = results
         
     # Specific element of the output list
     if isinstance(element, int):
         element_list = []
         for x in df[output]:
             try:
                 element_list.append(x[element])
```

### Comparing `wrangles-1.8.1/wrangles/select.py` & `wrangles-1.9.0/wrangles/select.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/standardize.py` & `wrangles-1.9.0/wrangles/standardize.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/train.py` & `wrangles-1.9.0/wrangles/train.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles/translate.py` & `wrangles-1.9.0/wrangles/translate.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.8.1/wrangles.egg-info/PKG-INFO` & `wrangles-1.9.0/wrangles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrangles
-Version: 1.8.1
+Version: 1.9.0
 Summary: Wrangle your data into shape with AI
 Home-page: https://github.com/wrangleworks/WranglesPy
 Author: WrangleWorks
 Author-email: chris@wrangleworks.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/wrangleworks/WranglesPy/issues
 Project-URL: Documentation, https://wrangles.io/python
```

### Comparing `wrangles-1.8.1/wrangles.egg-info/SOURCES.txt` & `wrangles-1.9.0/wrangles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

