# Comparing `tmp/dbt-singlestore-1.6.0.tar.gz` & `tmp/dbt-singlestore-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-singlestore-1.6.0.tar", last modified: Thu Dec 21 16:08:53 2023, max compression
+gzip compressed data, was "dbt-singlestore-1.6.1.tar", last modified: Thu May  2 13:26:44 2024, max compression
```

## Comparing `dbt-singlestore-1.6.0.tar` & `dbt-singlestore-1.6.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:53.005215 dbt-singlestore-1.6.0/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)    11356 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.0/LICENSE
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       46 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.0/MANIFEST.in
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      321 2023-12-21 16:08:53.005215 dbt-singlestore-1.6.0/PKG-INFO
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     3304 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/README.md
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:52.989215 dbt-singlestore-1.6.0/dbt/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        2 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/__init__.py
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:52.981215 dbt-singlestore-1.6.0/dbt/adapters/
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:52.989215 dbt-singlestore-1.6.0/dbt/adapters/singlestore/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      433 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.0/dbt/adapters/singlestore/__init__.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       18 2023-12-21 15:31:45.000000 dbt-singlestore-1.6.0/dbt/adapters/singlestore/__version__.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      751 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.0/dbt/adapters/singlestore/column.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4563 2023-10-30 13:53:32.000000 dbt-singlestore-1.6.0/dbt/adapters/singlestore/connections.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     9879 2023-12-21 15:31:45.000000 dbt-singlestore-1.6.0/dbt/adapters/singlestore/impl.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      985 2023-07-14 10:44:45.000000 dbt-singlestore-1.6.0/dbt/adapters/singlestore/relation.py
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:52.981215 dbt-singlestore-1.6.0/dbt/include/
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:52.993215 dbt-singlestore-1.6.0/dbt/include/singlestore/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       51 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/__init__.py
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       79 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/dbt_project.yml
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:52.993215 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     1554 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/catalog.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     2202 2023-12-21 15:31:45.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/columns.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)    10691 2023-12-18 12:53:16.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/common.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      606 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/grants.sql
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:52.985215 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/materializations/
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:52.993215 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/materializations/incremental/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      441 2023-12-21 15:31:45.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/materializations/incremental/incremental.sql
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:52.997215 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/materializations/snapshot/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4231 2023-07-14 10:44:45.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4373 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      916 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      224 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:53.005215 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       90 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/bool_or.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      135 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-10-30 13:53:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/data_types.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      203 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/dateadd.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      193 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/datediff.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      122 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/hash.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      624 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/listagg.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       94 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/safe_cast.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      389 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/split_part.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      361 2023-07-14 10:44:45.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/timestamps.sql
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      482 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/profile_template.yml
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      420 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.0/dbt/include/singlestore/sample_profiles.yml
-drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-12-21 16:08:53.005215 dbt-singlestore-1.6.0/dbt_singlestore.egg-info/
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      321 2023-12-21 16:08:52.000000 dbt-singlestore-1.6.0/dbt_singlestore.egg-info/PKG-INFO
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     1677 2023-12-21 16:08:52.000000 dbt-singlestore-1.6.0/dbt_singlestore.egg-info/SOURCES.txt
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        1 2023-12-21 16:08:52.000000 dbt-singlestore-1.6.0/dbt_singlestore.egg-info/dependency_links.txt
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       61 2023-12-21 16:08:52.000000 dbt-singlestore-1.6.0/dbt_singlestore.egg-info/requires.txt
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        4 2023-12-21 16:08:52.000000 dbt-singlestore-1.6.0/dbt_singlestore.egg-info/top_level.txt
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       38 2023-12-21 16:08:53.005215 dbt-singlestore-1.6.0/setup.cfg
--rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      771 2023-12-21 15:31:45.000000 dbt-singlestore-1.6.0/setup.py
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.639098 dbt-singlestore-1.6.1/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)    11356 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.1/LICENSE
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       46 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.1/MANIFEST.in
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      419 2024-05-02 13:26:44.639098 dbt-singlestore-1.6.1/PKG-INFO
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4532 2024-05-02 13:14:45.000000 dbt-singlestore-1.6.1/README.md
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.635098 dbt-singlestore-1.6.1/dbt/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        2 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/__init__.py
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.635098 dbt-singlestore-1.6.1/dbt/adapters/
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.635098 dbt-singlestore-1.6.1/dbt/adapters/singlestore/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      433 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.1/dbt/adapters/singlestore/__init__.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       18 2024-05-02 13:14:45.000000 dbt-singlestore-1.6.1/dbt/adapters/singlestore/__version__.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      751 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.1/dbt/adapters/singlestore/column.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4563 2024-04-30 14:34:36.000000 dbt-singlestore-1.6.1/dbt/adapters/singlestore/connections.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     9879 2024-04-30 14:52:18.000000 dbt-singlestore-1.6.1/dbt/adapters/singlestore/impl.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      985 2023-07-14 10:44:45.000000 dbt-singlestore-1.6.1/dbt/adapters/singlestore/relation.py
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.635098 dbt-singlestore-1.6.1/dbt/include/
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.635098 dbt-singlestore-1.6.1/dbt/include/singlestore/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       51 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/__init__.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       79 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/dbt_project.yml
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.635098 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     1554 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/catalog.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     2202 2023-12-21 15:31:45.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/columns.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)    10691 2024-04-15 23:31:46.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/common.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      606 2024-05-02 12:37:04.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/grants.sql
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.635098 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/materializations/
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.635098 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/materializations/incremental/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      441 2023-12-21 15:31:45.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/materializations/incremental/incremental.sql
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.639098 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/materializations/snapshot/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4231 2023-07-14 10:44:45.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4373 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      916 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      224 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.639098 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       90 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/bool_or.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      135 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-10-30 13:53:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/data_types.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      203 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/dateadd.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      193 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/datediff.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      122 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/hash.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      624 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/listagg.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       94 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/safe_cast.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      389 2023-06-29 14:15:32.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/split_part.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      361 2023-07-14 10:44:45.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/timestamps.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      482 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/profile_template.yml
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      420 2023-05-19 09:49:48.000000 dbt-singlestore-1.6.1/dbt/include/singlestore/sample_profiles.yml
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2024-05-02 13:26:44.639098 dbt-singlestore-1.6.1/dbt_singlestore.egg-info/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      419 2024-05-02 13:26:44.000000 dbt-singlestore-1.6.1/dbt_singlestore.egg-info/PKG-INFO
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     1677 2024-05-02 13:26:44.000000 dbt-singlestore-1.6.1/dbt_singlestore.egg-info/SOURCES.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        1 2024-05-02 13:26:44.000000 dbt-singlestore-1.6.1/dbt_singlestore.egg-info/dependency_links.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       61 2024-05-02 13:26:44.000000 dbt-singlestore-1.6.1/dbt_singlestore.egg-info/requires.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        4 2024-05-02 13:26:44.000000 dbt-singlestore-1.6.1/dbt_singlestore.egg-info/top_level.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       38 2024-05-02 13:26:44.639098 dbt-singlestore-1.6.1/setup.cfg
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      771 2024-05-02 13:14:45.000000 dbt-singlestore-1.6.1/setup.py
```

### Comparing `dbt-singlestore-1.6.0/LICENSE` & `dbt-singlestore-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/adapters/singlestore/column.py` & `dbt-singlestore-1.6.1/dbt/adapters/singlestore/column.py`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/adapters/singlestore/connections.py` & `dbt-singlestore-1.6.1/dbt/adapters/singlestore/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/adapters/singlestore/impl.py` & `dbt-singlestore-1.6.1/dbt/adapters/singlestore/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/adapters/singlestore/relation.py` & `dbt-singlestore-1.6.1/dbt/adapters/singlestore/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/include/singlestore/macros/catalog.sql` & `dbt-singlestore-1.6.1/dbt/include/singlestore/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/include/singlestore/macros/columns.sql` & `dbt-singlestore-1.6.1/dbt/include/singlestore/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/include/singlestore/macros/common.sql` & `dbt-singlestore-1.6.1/dbt/include/singlestore/macros/common.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/include/singlestore/macros/grants.sql` & `dbt-singlestore-1.6.1/dbt/include/singlestore/macros/grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql` & `dbt-singlestore-1.6.1/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql` & `dbt-singlestore-1.6.1/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-singlestore-1.6.1/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt/include/singlestore/macros/utils/listagg.sql` & `dbt-singlestore-1.6.1/dbt/include/singlestore/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/dbt_singlestore.egg-info/SOURCES.txt` & `dbt-singlestore-1.6.1/dbt_singlestore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.6.0/setup.py` & `dbt-singlestore-1.6.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_namespace_packages, setup
 
 package_name = "dbt-singlestore"
 # make sure this always matches dbt/adapters/singlestore/__version__.py
-package_version = "1.6.0"
+package_version = "1.6.1"
 description = """The singlestore adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=description,
@@ -15,11 +15,11 @@
     author_email="support@singlestore.com",
     url="https://github.com/memsql/dbt-singlestore",
     license="Apache License 2.0",
     packages=find_namespace_packages(include=['dbt', 'dbt.*']),
     include_package_data=True,
     install_requires=[
         "dbt-core>=1.0.0",
-        "singlestoredb==0.8.1",
+        "singlestoredb==1.2.0",
         "dataclasses_json>=0.5.6"
     ]
 )
```

