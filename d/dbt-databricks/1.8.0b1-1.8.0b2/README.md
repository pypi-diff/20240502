# Comparing `tmp/dbt-databricks-1.8.0b1.tar.gz` & `tmp/dbt-databricks-1.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-databricks-1.8.0b1.tar", last modified: Mon Feb 26 22:36:48 2024, max compression
+gzip compressed data, was "dbt-databricks-1.8.0b2.tar", last modified: Mon Mar 11 17:33:35 2024, max compression
```

## Comparing `dbt-databricks-1.8.0b1.tar` & `dbt-databricks-1.8.0b2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.897104 dbt-databricks-1.8.0b1/
--rw-r--r--   0 ben.cassell   (502) staff       (20)       46 2023-09-19 21:16:10.000000 dbt-databricks-1.8.0b1/MANIFEST.in
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5378 2024-02-26 22:36:48.896911 dbt-databricks-1.8.0b1/PKG-INFO
--rw-r--r--   0 ben.cassell   (502) staff       (20)     4624 2024-01-19 01:37:59.000000 dbt-databricks-1.8.0b1/README.md
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.871168 dbt-databricks-1.8.0b1/dbt/
--rw-r--r--   0 ben.cassell   (502) staff       (20)       76 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b1/dbt/__init__.py
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.865606 dbt-databricks-1.8.0b1/dbt/adapters/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.874092 dbt-databricks-1.8.0b1/dbt/adapters/databricks/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      626 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/__init__.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)       25 2024-02-26 19:46:50.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/__version__.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2732 2024-02-13 22:55:34.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/auth.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)      671 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/column.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)    62171 2024-02-26 19:45:06.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/connections.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)    33172 2024-02-26 19:45:06.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/impl.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)    19503 2024-02-26 19:45:06.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/python_submissions.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5339 2024-02-26 19:45:06.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation.py
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.877227 dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5611 2024-02-26 19:45:06.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/base.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1053 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/comment.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1584 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/materialized_view.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1457 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/partitioning.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1053 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/query.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2782 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/refresh.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1639 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/streaming_table.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2421 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/tblproperties.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2431 2024-02-22 18:57:29.000000 dbt-databricks-1.8.0b1/dbt/adapters/databricks/utils.py
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.866218 dbt-databricks-1.8.0b1/dbt/include/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.878539 dbt-databricks-1.8.0b1/dbt/include/databricks/
--rw-r--r--   0 ben.cassell   (502) staff       (20)       52 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/__init__.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)       77 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/dbt_project.yml
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.869221 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.881143 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3591 2024-02-26 19:45:06.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/catalog.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2409 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/copy_into.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      591 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/databricks_catalog.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2904 2024-02-22 18:57:29.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/metadata.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1985 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/persist_docs.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3542 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/python.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1157 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/relation.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.881448 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/etc/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      648 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/etc/statement.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.881695 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/get_custom_name/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      458 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/get_custom_name/get_custom_database.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.883754 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2802 2024-01-19 01:37:59.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/clone.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.885311 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/incremental/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     4329 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     4229 2024-02-22 18:03:27.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2066 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/incremental/validate.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3656 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/materialized_view.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.885822 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/seeds/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2683 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2476 2024-01-19 01:37:59.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/seeds/seeds.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5397 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/snapshot.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3622 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/streaming_table.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1727 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/table.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1266 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/view.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.888787 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.890318 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/components/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      130 2024-02-22 18:57:29.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/components/comment.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      216 2024-02-22 18:57:29.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/components/partitioning.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      669 2024-02-22 18:57:29.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/components/refresh_schedule.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      309 2024-02-22 18:57:29.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/components/tblproperties.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)    10574 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/constraints.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      628 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      567 2024-02-22 18:57:29.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      211 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/file_format.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.891465 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/materialized_view/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1800 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/materialized_view/alter.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      755 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/materialized_view/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      125 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/materialized_view/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      118 2024-02-22 18:57:29.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1373 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/optimize.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2273 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/replace.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.893077 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/streaming_table/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3211 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/streaming_table/alter.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      904 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/streaming_table/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      245 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/streaming_table/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      292 2024-02-22 18:57:34.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/streaming_table/refresh.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.893586 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/table/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3108 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/table/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      101 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/table/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      466 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/tblproperties.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.894248 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/view/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      642 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/view/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)       99 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/view/drop.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.894791 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/utils/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      318 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/utils/dateadd.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      338 2023-10-26 17:27:28.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/macros/utils/datediff.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      535 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b1/dbt/include/databricks/profile_template.yml
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-02-26 22:36:48.896619 dbt-databricks-1.8.0b1/dbt_databricks.egg-info/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5378 2024-02-26 22:36:48.000000 dbt-databricks-1.8.0b1/dbt_databricks.egg-info/PKG-INFO
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3872 2024-02-26 22:36:48.000000 dbt-databricks-1.8.0b1/dbt_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2024-02-26 22:36:48.000000 dbt-databricks-1.8.0b1/dbt_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2023-12-12 23:00:14.000000 dbt-databricks-1.8.0b1/dbt_databricks.egg-info/not-zip-safe
--rw-r--r--   0 ben.cassell   (502) staff       (20)      109 2024-02-26 22:36:48.000000 dbt-databricks-1.8.0b1/dbt_databricks.egg-info/requires.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)        4 2024-02-26 22:36:48.000000 dbt-databricks-1.8.0b1/dbt_databricks.egg-info/top_level.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)       38 2024-02-26 22:36:48.897217 dbt-databricks-1.8.0b1/setup.cfg
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2539 2024-02-26 19:46:50.000000 dbt-databricks-1.8.0b1/setup.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.496461 dbt-databricks-1.8.0b2/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       46 2023-09-19 21:16:10.000000 dbt-databricks-1.8.0b2/MANIFEST.in
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     6130 2024-03-11 17:33:35.496305 dbt-databricks-1.8.0b2/PKG-INFO
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     4624 2024-01-19 01:37:59.000000 dbt-databricks-1.8.0b2/README.md
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.475138 dbt-databricks-1.8.0b2/dbt/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       76 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b2/dbt/__init__.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.471857 dbt-databricks-1.8.0b2/dbt/adapters/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.477804 dbt-databricks-1.8.0b2/dbt/adapters/databricks/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      626 2024-02-27 00:26:50.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/__init__.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       25 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/__version__.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2732 2024-03-04 22:22:27.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/auth.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      671 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/column.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    64604 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/connections.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    33435 2024-03-11 17:21:51.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/impl.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    19098 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/python_submissions.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     4999 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.480009 dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5984 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/base.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1022 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/comment.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1584 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/materialized_view.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1619 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/partitioning.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1136 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/query.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2892 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/refresh.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1639 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/streaming_table.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2531 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/tblproperties.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2430 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/adapters/databricks/utils.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.472224 dbt-databricks-1.8.0b2/dbt/include/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.481043 dbt-databricks-1.8.0b2/dbt/include/databricks/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       52 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/__init__.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       77 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/dbt_project.yml
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.474151 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.483121 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3598 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/catalog.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2409 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/copy_into.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      591 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/databricks_catalog.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3351 2024-03-11 17:21:51.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/metadata.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1985 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/persist_docs.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3542 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/python.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1157 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/relation.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.483390 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/etc/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      648 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/etc/statement.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.483669 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/get_custom_name/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      458 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/get_custom_name/get_custom_database.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.485764 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2802 2024-01-19 01:37:59.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/clone.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.486827 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/incremental/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     4329 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5573 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2066 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3656 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/materialized_view.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.487334 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/seeds/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2683 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2476 2024-01-19 01:37:59.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/seeds/seeds.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5397 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/snapshot.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3622 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/streaming_table.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1727 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/table.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1266 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/view.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.489408 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.490537 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/components/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      130 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/components/comment.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      216 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/components/partitioning.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      669 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/components/refresh_schedule.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      309 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/components/tblproperties.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    10574 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/constraints.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      628 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      566 2024-03-08 21:42:25.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      211 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/file_format.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.491504 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/materialized_view/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1800 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      755 2024-03-11 17:21:51.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/materialized_view/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      125 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      118 2024-03-11 17:21:51.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1373 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/optimize.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2273 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/replace.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.492685 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/streaming_table/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3211 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/streaming_table/alter.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      904 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/streaming_table/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      245 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/streaming_table/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      292 2024-03-11 17:21:47.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/streaming_table/refresh.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.493131 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/table/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3108 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/table/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      101 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/table/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      466 2024-02-01 23:42:58.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/tblproperties.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.493743 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/view/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      642 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/view/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       99 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/view/drop.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.494202 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/utils/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      318 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/utils/dateadd.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      338 2023-10-26 17:27:28.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/macros/utils/datediff.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      535 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0b2/dbt/include/databricks/profile_template.yml
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-03-11 17:33:35.495801 dbt-databricks-1.8.0b2/dbt_databricks.egg-info/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     6130 2024-03-11 17:33:35.000000 dbt-databricks-1.8.0b2/dbt_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3872 2024-03-11 17:33:35.000000 dbt-databricks-1.8.0b2/dbt_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2024-03-11 17:33:35.000000 dbt-databricks-1.8.0b2/dbt_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2024-03-11 17:33:35.000000 dbt-databricks-1.8.0b2/dbt_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      111 2024-03-11 17:33:35.000000 dbt-databricks-1.8.0b2/dbt_databricks.egg-info/requires.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)        4 2024-03-11 17:33:35.000000 dbt-databricks-1.8.0b2/dbt_databricks.egg-info/top_level.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       38 2024-03-11 17:33:35.496528 dbt-databricks-1.8.0b2/setup.cfg
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2541 2024-03-11 17:21:51.000000 dbt-databricks-1.8.0b2/setup.py
```

### Comparing `dbt-databricks-1.8.0b1/PKG-INFO` & `dbt-databricks-1.8.0b2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,107 +1,109 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
+License: UNKNOWN
+Description: <p align="center">
+          <img src="https://bynder-public-us-west-2.s3.amazonaws.com/styleguide/ABB317701CA31CB7F29268E32B303CAE-pdf-column-1.png" alt="databricks logo" width="50%" />
+          <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="250"/>
+        </p>
+        <p align="center">
+          <a href="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml">
+            <img src="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
+          </a>
+          <a href="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml">
+            <img src="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml/badge.svg?event=push" alt="Integration Tests Badge"/>
+          </a>
+        </p>
+        
+        **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
+        
+        The **[Databricks Lakehouse](https://www.databricks.com/)** provides one simple platform to unify all your data, analytics and AI workloads.
+        
+        # dbt-databricks
+        
+        The `dbt-databricks` adapter contains all of the code enabling dbt to work with Databricks. This adapter is based off the amazing work done in [dbt-spark](https://github.com/dbt-labs/dbt-spark). Some key features include:
+        
+        - **Easy setup**. No need to install an ODBC driver as the adapter uses pure Python APIs.
+        - **Open by default**. For example, it uses the the open and performant [Delta](https://delta.io/) table format by default. This has many benefits, including letting you use `MERGE` as the the default incremental materialization strategy.
+        - **Support for Unity Catalog**. dbt-databricks>=1.1.1 supports the 3-level namespace of Unity Catalog (catalog / schema / relations) so you can organize and secure your data the way you like.
+        - **Performance**. The adapter generates SQL expressions that are automatically accelerated by the native, vectorized [Photon](https://databricks.com/product/photon) execution engine.
+        
+        ## Choosing between dbt-databricks and dbt-spark
+        If you are developing a dbt project on Databricks, we recommend using `dbt-databricks` for the reasons noted above.
+        
+        `dbt-spark` is an actively developed adapter which works with Databricks as well as Apache Spark anywhere it is hosted e.g. on AWS EMR.
+        
+        ## Getting started
+        
+        ### Installation
+        
+        Install using pip:
+        ```nofmt
+        pip install dbt-databricks
+        ```
+        
+        Upgrade to the latest version
+        ```nofmt
+        pip install --upgrade dbt-databricks
+        ```
+        
+        ### Profile Setup
+        
+        ```nofmt
+        your_profile_name:
+          target: dev
+          outputs:
+            dev:
+              type: databricks
+              catalog: [optional catalog name, if you are using Unity Catalog, only available in dbt-databricks>=1.1.1]
+              schema: [database/schema name]
+              host: [your.databrickshost.com]
+              http_path: [/sql/your/http/path]
+              token: [dapiXXXXXXXXXXXXXXXXXXXXXXX]
+        ```
+        
+        ### Quick Starts
+        
+        These following quick starts will get you up and running with the `dbt-databricks` adapter:
+        - [Developing your first dbt project](https://github.com/databricks/dbt-databricks/blob/main/docs/local-dev.md)
+        - Using dbt Cloud with Databricks ([Azure](https://docs.microsoft.com/en-us/azure/databricks/integrations/prep/dbt-cloud) | [AWS](https://docs.databricks.com/integrations/prep/dbt-cloud.html))
+        - [Running dbt production jobs on Databricks Workflows](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-workflows.md)
+        - [Using Unity Catalog with dbt-databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/uc.md)
+        - [Using GitHub Actions for dbt CI/CD on Databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/github-actions.md)
+        - [Loading data from S3 into Delta using the databricks_copy_into macro](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-copy-into-macro-aws.md)
+        - [Contribute to this repository](CONTRIBUTING.MD)
+        
+        ### Compatibility
+        
+        The `dbt-databricks` adapter has been tested:
+        
+        - with Python 3.7 or above.
+        - against `Databricks SQL` and `Databricks runtime releases 9.1 LTS` and later.
+        
+        ### Tips and Tricks
+        ## Choosing compute for a Python model
+        You can override the compute used for a specific Python model by setting the `http_path` property in model configuration. This can be useful if, for example, you want to run a Python model on an All Purpose cluster, while running SQL models on a SQL Warehouse. Note that this capability is only available for Python models.
+        
+        ```
+        def model(dbt, session):
+            dbt.config(
+              http_path="sql/protocolv1/..."
+            )
+        ```
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-
-<p align="center">
-  <img src="https://bynder-public-us-west-2.s3.amazonaws.com/styleguide/ABB317701CA31CB7F29268E32B303CAE-pdf-column-1.png" alt="databricks logo" width="50%" />
-  <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="250"/>
-</p>
-<p align="center">
-  <a href="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml">
-    <img src="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
-  </a>
-  <a href="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml">
-    <img src="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml/badge.svg?event=push" alt="Integration Tests Badge"/>
-  </a>
-</p>
-
-**[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
-
-The **[Databricks Lakehouse](https://www.databricks.com/)** provides one simple platform to unify all your data, analytics and AI workloads.
-
-# dbt-databricks
-
-The `dbt-databricks` adapter contains all of the code enabling dbt to work with Databricks. This adapter is based off the amazing work done in [dbt-spark](https://github.com/dbt-labs/dbt-spark). Some key features include:
-
-- **Easy setup**. No need to install an ODBC driver as the adapter uses pure Python APIs.
-- **Open by default**. For example, it uses the the open and performant [Delta](https://delta.io/) table format by default. This has many benefits, including letting you use `MERGE` as the the default incremental materialization strategy.
-- **Support for Unity Catalog**. dbt-databricks>=1.1.1 supports the 3-level namespace of Unity Catalog (catalog / schema / relations) so you can organize and secure your data the way you like.
-- **Performance**. The adapter generates SQL expressions that are automatically accelerated by the native, vectorized [Photon](https://databricks.com/product/photon) execution engine.
-
-## Choosing between dbt-databricks and dbt-spark
-If you are developing a dbt project on Databricks, we recommend using `dbt-databricks` for the reasons noted above.
-
-`dbt-spark` is an actively developed adapter which works with Databricks as well as Apache Spark anywhere it is hosted e.g. on AWS EMR.
-
-## Getting started
-
-### Installation
-
-Install using pip:
-```nofmt
-pip install dbt-databricks
-```
-
-Upgrade to the latest version
-```nofmt
-pip install --upgrade dbt-databricks
-```
-
-### Profile Setup
-
-```nofmt
-your_profile_name:
-  target: dev
-  outputs:
-    dev:
-      type: databricks
-      catalog: [optional catalog name, if you are using Unity Catalog, only available in dbt-databricks>=1.1.1]
-      schema: [database/schema name]
-      host: [your.databrickshost.com]
-      http_path: [/sql/your/http/path]
-      token: [dapiXXXXXXXXXXXXXXXXXXXXXXX]
-```
-
-### Quick Starts
-
-These following quick starts will get you up and running with the `dbt-databricks` adapter:
-- [Developing your first dbt project](https://github.com/databricks/dbt-databricks/blob/main/docs/local-dev.md)
-- Using dbt Cloud with Databricks ([Azure](https://docs.microsoft.com/en-us/azure/databricks/integrations/prep/dbt-cloud) | [AWS](https://docs.databricks.com/integrations/prep/dbt-cloud.html))
-- [Running dbt production jobs on Databricks Workflows](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-workflows.md)
-- [Using Unity Catalog with dbt-databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/uc.md)
-- [Using GitHub Actions for dbt CI/CD on Databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/github-actions.md)
-- [Loading data from S3 into Delta using the databricks_copy_into macro](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-copy-into-macro-aws.md)
-- [Contribute to this repository](CONTRIBUTING.MD)
-
-### Compatibility
-
-The `dbt-databricks` adapter has been tested:
-
-- with Python 3.7 or above.
-- against `Databricks SQL` and `Databricks runtime releases 9.1 LTS` and later.
-
-### Tips and Tricks
-## Choosing compute for a Python model
-You can override the compute used for a specific Python model by setting the `http_path` property in model configuration. This can be useful if, for example, you want to run a Python model on an All Purpose cluster, while running SQL models on a SQL Warehouse. Note that this capability is only available for Python models.
-
-```
-def model(dbt, session):
-    dbt.config(
-      http_path="sql/protocolv1/..."
-    )
-```
```

### Comparing `dbt-databricks-1.8.0b1/README.md` & `dbt-databricks-1.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/__init__.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/auth.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/auth.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/column.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/connections.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/connections.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
+from multiprocessing.context import SpawnContext
 import uuid
 import logging
 import warnings
 from contextlib import contextmanager
 from dataclasses import dataclass
+import decimal
 import itertools
 import os
 import re
 import sys
 import threading
 import time
 from threading import get_ident
@@ -25,42 +27,41 @@
     Union,
     Hashable,
 )
 from numbers import Number
 
 from agate import Table
 
-import dbt.exceptions
-from dbt.adapters.base import Credentials
 from dbt.adapters.base.query_headers import MacroQueryStringSetter
 from dbt.adapters.spark.connections import SparkConnectionManager
-from dbt.clients import agate_helper
-from dbt.contracts.connection import (
+from dbt_common.clients import agate_helper
+from dbt.adapters.contracts.connection import (
     AdapterResponse,
     AdapterRequiredConfig,
     Connection,
     ConnectionState,
+    Credentials,
     DEFAULT_QUERY_COMMENT,
     Identifier,
     LazyHandle,
 )
-from dbt.events.types import (
+from dbt.adapters.events.types import (
     NewConnection,
     ConnectionReused,
+    ConnectionUsed,
     ConnectionLeftOpenInCleanup,
     ConnectionClosedInCleanup,
+    SQLQuery,
+    SQLQueryStatus,
 )
 
-from dbt.contracts.graph.manifest import Manifest
-from dbt.contracts.graph.nodes import ResultNode
-from dbt.events import AdapterLogger
-from dbt.events.contextvars import get_node_info
-from dbt.events.functions import fire_event
-from dbt.events.types import ConnectionUsed, SQLQuery, SQLQueryStatus
-from dbt.utils import DECIMALS, cast_to_str
+from dbt.adapters.events.logging import AdapterLogger
+from dbt_common.events.contextvars import get_node_info
+from dbt_common.events.functions import fire_event
+from dbt_common.utils import cast_to_str
 
 import databricks.sql as dbsql
 from databricks.sql.client import (
     Connection as DatabricksSQLConnection,
     Cursor as DatabricksSQLCursor,
 )
 from databricks.sql.exc import Error
@@ -74,21 +75,27 @@
 
 from requests.auth import AuthBase
 from requests import PreparedRequest
 from databricks.sdk.core import HeaderFactory
 
 import keyring
 from requests import Session
+from dbt_common.exceptions import (
+    DbtValidationError,
+    DbtConfigError,
+    DbtRuntimeError,
+    DbtInternalError,
+)
 
-logger = AdapterLogger("Databricks")
 
 mv_refresh_regex = re.compile(r"refresh\s+materialized\s+view\s+([`\w.]+)", re.IGNORECASE)
 st_refresh_regex = re.compile(
     r"create\s+or\s+refresh\s+streaming\s+table\s+([`\w.]+)", re.IGNORECASE
 )
+logger = AdapterLogger("Databricks")
 
 
 TCredentialProvider = Union[CredentialsProvider, SessionCredentials]
 
 
 class DbtCoreHandler(logging.Handler):
     def __init__(self, level: Union[str, int], dbt_logger: AdapterLogger):
@@ -118,14 +125,15 @@
 DBT_DATABRICKS_INVOCATION_ENV_REGEX = re.compile("^[A-z0-9\\-]+$")
 EXTRACT_CLUSTER_ID_FROM_HTTP_PATH_REGEX = re.compile(r"/?sql/protocolv1/o/\d+/(.*)")
 DBT_DATABRICKS_HTTP_SESSION_HEADERS = "DBT_DATABRICKS_HTTP_SESSION_HEADERS"
 
 REDIRECT_URL = "http://localhost:8020"
 CLIENT_ID = "dbt-databricks"
 SCOPES = ["all-apis", "offline_access"]
+MAX_NT_PASSWORD_SIZE = 1280
 
 # toggle for session managements that minimizes the number of sessions opened/closed
 USE_LONG_SESSIONS = os.getenv("DBT_DATABRICKS_LONG_SESSIONS", "True").upper() == "TRUE"
 
 # Number of idle seconds before a connection is automatically closed. Only applicable if
 # USE_LONG_SESSIONS is true.
 DEFAULT_MAX_IDLE_TIME = 600
@@ -184,37 +192,35 @@
         data = super().__pre_deserialize__(data)
         if "database" not in data:
             data["database"] = None
         return data
 
     def __post_init__(self) -> None:
         if "." in (self.schema or ""):
-            raise dbt.exceptions.DbtValidationError(
+            raise DbtValidationError(
                 f"The schema should not contain '.': {self.schema}\n"
                 "If you are trying to set a catalog, please use `catalog` instead.\n"
             )
 
         session_properties = self.session_properties or {}
         if CATALOG_KEY_IN_SESSION_PROPERTIES in session_properties:
             if self.database is None:
                 self.database = session_properties[CATALOG_KEY_IN_SESSION_PROPERTIES]
                 del session_properties[CATALOG_KEY_IN_SESSION_PROPERTIES]
             else:
-                raise dbt.exceptions.DbtValidationError(
+                raise DbtValidationError(
                     f"Got duplicate keys: (`{CATALOG_KEY_IN_SESSION_PROPERTIES}` "
                     'in session_properties) all map to "database"'
                 )
         self.session_properties = session_properties
 
         if self.database is not None:
             database = self.database.strip()
             if not database:
-                raise dbt.exceptions.DbtValidationError(
-                    f"Invalid catalog name : `{self.database}`."
-                )
+                raise DbtValidationError(f"Invalid catalog name : `{self.database}`.")
             self.database = database
         else:
             self.database = "hive_metastore"
 
         connection_parameters = self.connection_parameters or {}
         for key in (
             "server_hostname",
@@ -224,60 +230,56 @@
             "client_secret",
             "session_configuration",
             "catalog",
             "schema",
             "_user_agent_entry",
         ):
             if key in connection_parameters:
-                raise dbt.exceptions.DbtValidationError(
-                    f"The connection parameter `{key}` is reserved."
-                )
+                raise DbtValidationError(f"The connection parameter `{key}` is reserved.")
         if "http_headers" in connection_parameters:
             http_headers = connection_parameters["http_headers"]
             if not isinstance(http_headers, dict) or any(
                 not isinstance(key, str) or not isinstance(value, str)
                 for key, value in http_headers.items()
             ):
-                raise dbt.exceptions.DbtValidationError(
+                raise DbtValidationError(
                     "The connection parameter `http_headers` should be dict of strings: "
                     f"{http_headers}."
                 )
         if "_socket_timeout" not in connection_parameters:
             connection_parameters["_socket_timeout"] = 180
         self.connection_parameters = connection_parameters
 
     def validate_creds(self) -> None:
         for key in ["host", "http_path"]:
             if not getattr(self, key):
-                raise dbt.exceptions.DbtProfileError(
+                raise DbtConfigError(
                     "The config '{}' is required to connect to Databricks".format(key)
                 )
         if not self.token and self.auth_type != "oauth":
-            raise dbt.exceptions.DbtProfileError(
+            raise DbtConfigError(
                 ("The config `auth_type: oauth` is required when not using access token")
             )
 
         if not self.client_id and self.client_secret:
-            raise dbt.exceptions.DbtProfileError(
+            raise DbtConfigError(
                 (
                     "The config 'client_id' is required to connect "
                     "to Databricks when 'client_secret' is present"
                 )
             )
 
     @classmethod
     def get_invocation_env(cls) -> Optional[str]:
         invocation_env = os.environ.get(DBT_DATABRICKS_INVOCATION_ENV)
         if invocation_env:
             # Thrift doesn't allow nested () so we need to ensure
             # that the passed user agent is valid.
             if not DBT_DATABRICKS_INVOCATION_ENV_REGEX.search(invocation_env):
-                raise dbt.exceptions.DbtValidationError(
-                    f"Invalid invocation environment: {invocation_env}"
-                )
+                raise DbtValidationError(f"Invalid invocation environment: {invocation_env}")
         return invocation_env
 
     @classmethod
     def get_all_http_headers(cls, user_http_session_headers: Dict[str, str]) -> Dict[str, str]:
         http_session_headers_str: Optional[str] = os.environ.get(
             DBT_DATABRICKS_HTTP_SESSION_HEADERS
         )
@@ -292,15 +294,15 @@
         )
 
         intersect_http_header_keys = (
             user_http_session_headers.keys() & http_session_headers_dict.keys()
         )
 
         if len(intersect_http_header_keys) > 0:
-            raise dbt.exceptions.DbtValidationError(
+            raise DbtValidationError(
                 f"Intersection with reserved http_headers in keys: {intersect_http_header_keys}"
             )
 
         http_session_headers_dict.update(user_http_session_headers)
 
         return http_session_headers_dict
 
@@ -386,50 +388,109 @@
                 client_secret="",
                 redirect_url=REDIRECT_URL,
                 scopes=SCOPES,
             )
             # optional branch. Try and keep going if it does not work
             try:
                 # try to get cached credentials
-                credsdict = keyring.get_password("dbt-databricks", host)
+                credsdict = self.get_sharded_password("dbt-databricks", host)
 
                 if credsdict:
                     provider = SessionCredentials.from_dict(oauth_client, json.loads(credsdict))
                     # if refresh token is expired, this will throw
                     try:
                         if provider.token().valid:
                             return provider
                     except Exception as e:
                         logger.debug(e)
                         # whatever it is, get rid of the cache
-                        keyring.delete_password("dbt-databricks", host)
+                        self.delete_sharded_password("dbt-databricks", host)
 
             # error with keyring. Maybe machine has no password persistency
             except Exception as e:
                 logger.debug(e)
                 logger.info("could not retrieved saved token")
 
             # no token, go fetch one
             consent = oauth_client.initiate_consent()
 
             provider = consent.launch_external_browser()
             # save for later
             self._credentials_provider = provider.as_dict()
             try:
-                keyring.set_password("dbt-databricks", host, json.dumps(self._credentials_provider))
+                self.set_sharded_password(
+                    "dbt-databricks", host, json.dumps(self._credentials_provider)
+                )
             # error with keyring. Maybe machine has no password persistency
             except Exception as e:
                 logger.debug(e)
                 logger.info("could not save token")
 
             return provider
 
         finally:
             self._lock.release()
 
+    def set_sharded_password(self, service_name: str, username: str, password: str) -> None:
+        max_size = MAX_NT_PASSWORD_SIZE
+
+        # if not Windows or "small" password, stick to the default
+        if os.name != "nt" or len(password) < max_size:
+            keyring.set_password(service_name, username, password)
+        else:
+            logger.debug(f"password is {len(password)} characters, sharding it.")
+
+            password_shards = [
+                password[i : i + max_size] for i in range(0, len(password), max_size)
+            ]
+            shard_info = {
+                "sharded_password": True,
+                "shard_count": len(password_shards),
+            }
+
+            # store the "shard info" as the "base" password
+            keyring.set_password(service_name, username, json.dumps(shard_info))
+            # then store all shards with the shard number as postfix
+            for i, s in enumerate(password_shards):
+                keyring.set_password(service_name, f"{username}__{i}", s)
+
+    def get_sharded_password(self, service_name: str, username: str) -> Optional[str]:
+        password = keyring.get_password(service_name, username)
+
+        # check for "shard info" stored as json
+        try:
+            password_as_dict = json.loads(str(password))
+            if password_as_dict.get("sharded_password"):
+                # if password was stored shared, reconstruct it
+                shard_count = int(password_as_dict.get("shard_count"))
+
+                password = ""
+                for i in range(shard_count):
+                    password += str(keyring.get_password(service_name, f"{username}__{i}"))
+        except ValueError:
+            pass
+
+        return password
+
+    def delete_sharded_password(self, service_name: str, username: str) -> None:
+        password = keyring.get_password(service_name, username)
+
+        # check for "shard info" stored as json. If so delete all shards
+        try:
+            password_as_dict = json.loads(str(password))
+            if password_as_dict.get("sharded_password"):
+                shard_count = int(password_as_dict.get("shard_count"))
+                for i in range(shard_count):
+                    keyring.delete_password(service_name, f"{username}__{i}")
+        except ValueError:
+            pass
+
+        # delete "base" password
+        keyring.delete_password(service_name, username)
+
     def _provider_from_dict(self) -> Optional[TCredentialProvider]:
         if self.token:
             return token_auth.from_dict(self._credentials_provider)
 
         if self.client_id and self.client_secret:
             return m2m_auth.from_dict(
                 host=self.host or "",
@@ -598,15 +659,15 @@
         session.headers = {"User-Agent": self._user_agent}
 
         pipeline_id = _get_table_view_pipeline_id(session, host, model_name)
         pipeline = _get_pipeline_state(session, host, pipeline_id)
         # get the most recently created update for the pipeline
         latest_update = _find_update(pipeline)
         if not latest_update:
-            raise dbt.exceptions.DbtRuntimeError(f"No update created for pipeline: {pipeline_id}")
+            raise DbtRuntimeError(f"No update created for pipeline: {pipeline_id}")
 
         state = latest_update.get("state")
         # we use update_id to retrieve the update in the polling loop
         update_id = latest_update.get("update_id", "")
         prev_state = state
 
         logger.info(
@@ -623,15 +684,15 @@
             # should we do exponential backoff?
             time.sleep(polling_interval)
 
             pipeline = _get_pipeline_state(session, host, pipeline_id)
             # get the update we are currently polling
             update = _find_update(pipeline, update_id)
             if not update:
-                raise dbt.exceptions.DbtRuntimeError(
+                raise DbtRuntimeError(
                     f"Error getting pipeline update info: {pipeline_id}, update: {update_id}"
                 )
 
             state = update.get("state")
             if state != prev_state:
                 logger.info(
                     f"refreshing {model_name}, pipeline: {pipeline_id}, update: {update_id} {state}"
@@ -644,32 +705,30 @@
                 if msg:
                     logger.error(msg)
 
                 # another update may have been created due to retry_on_fail settings
                 # get the latest update and see if it is a new one
                 latest_update = _find_update(pipeline)
                 if not latest_update:
-                    raise dbt.exceptions.DbtRuntimeError(
-                        f"No update created for pipeline: {pipeline_id}"
-                    )
+                    raise DbtRuntimeError(f"No update created for pipeline: {pipeline_id}")
 
                 latest_update_id = latest_update.get("update_id", "")
                 if latest_update_id != update_id:
                     update_id = latest_update_id
                     state = None
 
         if exceeded_timeout:
-            raise dbt.exceptions.DbtRuntimeError("timed out waiting for materialized view refresh")
+            raise DbtRuntimeError("timed out waiting for materialized view refresh")
 
         if state == "FAILED":
             msg = _get_update_error_msg(session, host, pipeline_id, update_id)
-            raise dbt.exceptions.DbtRuntimeError(f"error refreshing model {model_name} {msg}")
+            raise DbtRuntimeError(f"error refreshing model {model_name} {msg}")
 
         if state == "CANCELED":
-            raise dbt.exceptions.DbtRuntimeError(f"refreshing model {model_name} cancelled")
+            raise DbtRuntimeError(f"refreshing model {model_name} cancelled")
 
         return
 
     @classmethod
     def findUpdate(cls, updates: List, id: str) -> Optional[Dict]:
         matches = [x for x in updates if x.get("update_id") == id]
         if matches:
@@ -688,15 +747,15 @@
 
         return str(_as_hex)
 
     @classmethod
     def _fix_binding(cls, value: Any) -> Any:
         """Convert complex datatypes to primitives that can be loaded by
         the Spark driver"""
-        if isinstance(value, DECIMALS):
+        if isinstance(value, decimal.Decimal):
             return float(value)
         else:
             return value
 
     @property
     def description(
         self,
@@ -781,22 +840,22 @@
     # last_used_time, essentially indicating that the connection was in use while the python
     # model was running. So the session is not refreshed by idle connection cleanup and errors
     # the next time it is used.
     language: Optional[str] = None
 
     session_id: Optional[str] = None
 
-    def _acquire(self, node: Optional[ResultNode]) -> None:
+    def _acquire(self, query_header_context: Any) -> None:
         """Indicate that this connection is in use."""
-        self._log_usage(node)
+        self._log_usage(query_header_context)
         self.acquire_release_count += 1
         if self.last_used_time is None:
             self.last_used_time = time.time()
-        if node and hasattr(node, "language"):
-            self.language = node.language
+        if query_header_context and hasattr(query_header_context, "language"):
+            self.language = query_header_context.language
         else:
             self.language = None
 
         self._log_info("_acquire")
 
     def _release(self) -> None:
         """Indicate that this connection is not in use."""
@@ -826,19 +885,19 @@
             f"lang: {self.language}, thrd: {self.thread_identifier}, "
             f"cmpt: `{self.compute_name}`, lut: {self.last_used_time}"
         )
 
     def _log_info(self, caller: Optional[str]) -> None:
         logger.debug(f"conn: {id(self)}: {caller} {self._get_conn_info_str()}")
 
-    def _log_usage(self, node: Optional[ResultNode]) -> None:
-        if node:
+    def _log_usage(self, query_header_context: Any) -> None:
+        if query_header_context:
             # ResultNode *should* have relation_name attr, but we work around a core
             # issue by checking.
-            relation_name = getattr(node, "relation_name", "[unknown]")
+            relation_name = getattr(query_header_context, "relation_name", "[unknown]")
             if not self.compute_name:
                 logger.debug(
                     f"On thread {self.thread_identifier}: {relation_name} "
                     "using default compute resource."
                 )
             else:
                 logger.debug(
@@ -857,67 +916,67 @@
         self.last_used_time = None
 
 
 class DatabricksConnectionManager(SparkConnectionManager):
     TYPE: str = "databricks"
     credentials_provider: Optional[TCredentialProvider] = None
 
-    def __init__(self, profile: AdapterRequiredConfig) -> None:
-        super().__init__(profile)
+    def __init__(self, profile: AdapterRequiredConfig, mp_context: SpawnContext) -> None:
+        super().__init__(profile, mp_context)
         if USE_LONG_SESSIONS:
             self.threads_compute_connections: Dict[
                 Hashable, Dict[Hashable, DatabricksDBTConnection]
             ] = {}
 
     def compare_dbr_version(self, major: int, minor: int) -> int:
         version = (major, minor)
 
         connection: DatabricksSQLConnectionWrapper = self.get_thread_connection().handle
         dbr_version = connection.dbr_version
         return (dbr_version > version) - (dbr_version < version)
 
-    def set_query_header(self, manifest: Manifest) -> None:
-        self.query_header = DatabricksMacroQueryStringSetter(self.profile, manifest)
+    def set_query_header(self, query_header_context: Dict[str, Any]) -> None:
+        self.query_header = DatabricksMacroQueryStringSetter(self.profile, query_header_context)
 
     @contextmanager
     def exception_handler(self, sql: str) -> Iterator[None]:
         log_sql = redact_credentials(sql)
 
         try:
             yield
 
         except Error as exc:
             logger.debug(f"Error while running:\n{log_sql}")
             _log_dbsql_errors(exc)
-            raise dbt.exceptions.DbtRuntimeError(str(exc)) from exc
+            raise DbtRuntimeError(str(exc)) from exc
 
         except Exception as exc:
             logger.debug(f"Error while running:\n{log_sql}")
             logger.debug(exc)
             if len(exc.args) == 0:
                 raise
 
             thrift_resp = exc.args[0]
             if hasattr(thrift_resp, "status"):
                 msg = thrift_resp.status.errorMessage
-                raise dbt.exceptions.DbtRuntimeError(msg) from exc
+                raise DbtRuntimeError(msg) from exc
             else:
-                raise dbt.exceptions.DbtRuntimeError(str(exc)) from exc
+                raise DbtRuntimeError(str(exc)) from exc
 
     # override/overload
     def set_connection_name(
-        self, name: Optional[str] = None, node: Optional[ResultNode] = None
+        self, name: Optional[str] = None, query_header_context: Any = None
     ) -> Connection:
         """Called by 'acquire_connection' in DatabricksAdapter, which is called by
         'connection_named', called by 'connection_for(node)'.
         Creates a connection for this thread if one doesn't already
         exist, and will rename an existing connection."""
 
         if USE_LONG_SESSIONS:
-            return self._get_compute_connection(name, node)
+            return self._get_compute_connection(name, query_header_context)
 
         conn_name: str = "master" if name is None else name
 
         # Get a connection for this thread
         conn = self.get_if_exists()
 
         if conn and conn.name == conn_name and conn.state == ConnectionState.OPEN:
@@ -930,23 +989,23 @@
                 type=Identifier(self.TYPE),
                 name=conn_name,
                 state=ConnectionState.INIT,
                 transaction_open=False,
                 handle=None,
                 credentials=self.profile.credentials,
             )
-            conn.handle = LazyHandle(self.get_open_for_model(node))
+            conn.handle = LazyHandle(self.get_open_for_context(query_header_context))
             # Add the connection to thread_connections for this thread
             self.set_thread_connection(conn)
             fire_event(
                 NewConnection(conn_name=conn_name, conn_type=self.TYPE, node_info=get_node_info())
             )
         else:  # existing connection either wasn't open or didn't have the right name
             if conn.state != ConnectionState.OPEN:
-                conn.handle = LazyHandle(self.get_open_for_model(node))
+                conn.handle = LazyHandle(self.get_open_for_context(query_header_context))
             if conn.name != conn_name:
                 orig_conn_name: str = conn.name or ""
                 conn.name = conn_name
                 fire_event(ConnectionReused(orig_conn_name=orig_conn_name, conn_name=conn_name))
 
         return conn
 
@@ -994,45 +1053,42 @@
                     self.close(connection)
 
             # garbage collect these connections
             self.thread_connections.clear()
             self.threads_compute_connections.clear()
 
     def _get_compute_connection(
-        self, name: Optional[str] = None, node: Optional[ResultNode] = None
+        self, name: Optional[str] = None, query_header_context: Any = None
     ) -> Connection:
         """Called by 'set_connection_name' in DatabricksConnectionManager.
         Creates a connection for this thread/node if one doesn't already
         exist, and will rename an existing connection."""
 
         assert (
             USE_LONG_SESSIONS
         ), "This path, '_get_compute_connection', should only be reachable with USE_LONG_SESSIONS"
 
         self._cleanup_idle_connections()
 
         conn_name: str = "master" if name is None else name
 
         # Get a connection for this thread
-        conn = self._get_if_exists_compute_connection(_get_compute_name(node) or "")
+        conn = self._get_if_exists_compute_connection(_get_compute_name(query_header_context) or "")
 
         if conn is None:
-            conn = self._create_compute_connection(conn_name, node)
+            conn = self._create_compute_connection(conn_name, query_header_context)
         else:  # existing connection either wasn't open or didn't have the right name
-            conn = self._update_compute_connection(conn, conn_name, node)
+            conn = self._update_compute_connection(conn, conn_name)
 
-        conn._acquire(node)
+        conn._acquire(query_header_context)
 
         return conn
 
     def _update_compute_connection(
-        self,
-        conn: DatabricksDBTConnection,
-        new_name: str,
-        node: Optional[ResultNode] = None,
+        self, conn: DatabricksDBTConnection, new_name: str
     ) -> DatabricksDBTConnection:
         """Update a connection that is being re-used with a new name, handle, etc."""
         assert USE_LONG_SESSIONS, (
             "This path, '_update_compute_connection', should only be "
             "reachable with USE_LONG_SESSIONS"
         )
 
@@ -1054,39 +1110,39 @@
             self.set_thread_connection(conn)
 
         conn._log_info(f"reusing connection {orig_conn_name}")
 
         return conn
 
     def _create_compute_connection(
-        self, conn_name: str, node: Optional[ResultNode] = None
+        self, conn_name: str, query_header_context: Any = None
     ) -> DatabricksDBTConnection:
         """Create anew connection for the combination of current thread and compute associated
         with the given node."""
         assert USE_LONG_SESSIONS, (
             "This path, '_create_compute_connection', should only be reachable "
             "with USE_LONG_SESSIONS"
         )
 
         # Create a new connection
-        compute_name = _get_compute_name(node=node) or ""
+        compute_name = _get_compute_name(query_header_context) or ""
 
         conn = DatabricksDBTConnection(
             type=Identifier(self.TYPE),
             name=conn_name,
             state=ConnectionState.INIT,
             transaction_open=False,
             handle=None,
             credentials=self.profile.credentials,
         )
         conn.compute_name = compute_name
         creds = cast(DatabricksCredentials, self.profile.credentials)
-        conn.http_path = _get_http_path(node=node, creds=creds) or ""
+        conn.http_path = _get_http_path(query_header_context, creds=creds) or ""
         conn.thread_identifier = cast(Tuple[int, int], self.get_thread_identifier())
-        conn.max_idle_time = _get_max_idle_time(node=node, creds=creds)
+        conn.max_idle_time = _get_max_idle_time(query_header_context, creds=creds)
 
         conn.handle = LazyHandle(self._open2)
 
         conn._log_info("Creating DatabricksDBTConnection")
 
         # Add this connection to the thread/compute connection pool.
         self._add_compute_connection(conn)
@@ -1106,15 +1162,15 @@
         assert (
             USE_LONG_SESSIONS
         ), "This path, '_add_compute_connection', should only be reachable with USE_LONG_SESSIONS"
 
         with self.lock:
             thread_map = self._get_compute_connections()
             if conn.compute_name in thread_map:
-                raise dbt.exceptions.DbtInternalError(
+                raise DbtInternalError(
                     f"In set_thread_compute_connection, connection exists for `{conn.compute_name}`"
                 )
             thread_map[conn.compute_name] = conn
 
     def _get_compute_connections(
         self,
     ) -> Dict[Hashable, DatabricksDBTConnection]:
@@ -1308,36 +1364,36 @@
             f"GetTables(database={database}, schema={schema}, identifier={identifier})",
             lambda cursor: cursor.tables(
                 catalog_name=database, schema_name=schema, table_name=identifier
             ),
         )
 
     @classmethod
-    def get_open_for_model(
-        cls, node: Optional[ResultNode] = None
+    def get_open_for_context(
+        cls, query_header_context: Any = None
     ) -> Callable[[Connection], Connection]:
         # If there is no node we can simply return the exsting class method open.
         # If there is a node create a closure that will call cls._open with the node.
-        if not node:
+        if not query_header_context:
             return cls.open
 
         def open_for_model(connection: Connection) -> Connection:
-            return cls._open(connection, node)
+            return cls._open(connection, query_header_context)
 
         return open_for_model
 
     @classmethod
     def open(cls, connection: Connection) -> Connection:
         # Simply call _open with no ResultNode argument.
         # Because this is an overridden method we can't just add
         # a ResultNode parameter to open.
         return cls._open(connection)
 
     @classmethod
-    def _open(cls, connection: Connection, node: Optional[ResultNode] = None) -> Connection:
+    def _open(cls, connection: Connection, query_header_context: Any = None) -> Connection:
         if connection.state == ConnectionState.OPEN:
             logger.debug("Connection is already open, skipping open.")
             return connection
 
         creds: DatabricksCredentials = connection.credentials
         timeout = creds.connect_timeout
 
@@ -1354,15 +1410,15 @@
 
         http_headers: List[Tuple[str, str]] = list(
             creds.get_all_http_headers(connection_parameters.pop("http_headers", {})).items()
         )
 
         # If a model specifies a compute resource the http path
         # may be different than the http_path property of creds.
-        http_path = _get_http_path(node, creds)
+        http_path = _get_http_path(query_header_context, creds)
 
         def connect() -> DatabricksSQLConnectionWrapper:
             try:
                 # TODO: what is the error when a user specifies a catalog they don't have access to
                 conn: DatabricksSQLConnection = dbsql.connect(
                     server_hostname=creds.host,
                     http_path=http_path,
@@ -1519,45 +1575,41 @@
     return refresh_search is not None, name
 
 
 def _get_table_view_pipeline_id(session: Session, host: str, name: str) -> str:
     table_url = f"https://{host}/api/2.1/unity-catalog/tables/{name}"
     resp1 = session.get(table_url)
     if resp1.status_code != 200:
-        raise dbt.exceptions.DbtRuntimeError(
+        raise DbtRuntimeError(
             f"Error getting info for materialized view/streaming table {name}: {resp1.text}"
         )
 
     pipeline_id = resp1.json().get("pipeline_id", "")
     if not pipeline_id:
-        raise dbt.exceptions.DbtRuntimeError(
+        raise DbtRuntimeError(
             f"Materialized view/streaming table {name} does not have a pipeline id"
         )
 
     return pipeline_id
 
 
 def _get_pipeline_state(session: Session, host: str, pipeline_id: str) -> dict:
     pipeline_url = f"https://{host}/api/2.0/pipelines/{pipeline_id}"
 
     response = session.get(pipeline_url)
     if response.status_code != 200:
-        raise dbt.exceptions.DbtRuntimeError(
-            f"Error getting pipeline info for {pipeline_id}: {response.text}"
-        )
+        raise DbtRuntimeError(f"Error getting pipeline info for {pipeline_id}: {response.text}")
 
     return response.json()
 
 
 def _find_update(pipeline: dict, id: str = "") -> Optional[Dict]:
     updates = pipeline.get("latest_updates", [])
     if not updates:
-        raise dbt.exceptions.DbtRuntimeError(
-            f"No updates for pipeline: {pipeline.get('pipeline_id', '')}"
-        )
+        raise DbtRuntimeError(f"No updates for pipeline: {pipeline.get('pipeline_id', '')}")
 
     if not id:
         return updates[0]
 
     matches = [x for x in updates if x.get("update_id") == id]
     if matches:
         return matches[0]
@@ -1565,15 +1617,15 @@
     return None
 
 
 def _get_update_error_msg(session: Session, host: str, pipeline_id: str, update_id: str) -> str:
     events_url = f"https://{host}/api/2.0/pipelines/{pipeline_id}/events"
     response = session.get(events_url)
     if response.status_code != 200:
-        raise dbt.exceptions.DbtRuntimeError(
+        raise DbtRuntimeError(
             f"Error getting pipeline event info for {pipeline_id}: {response.text}"
         )
 
     events = response.json().get("events", [])
     update_events = [
         e
         for e in events
@@ -1590,85 +1642,89 @@
     msg = ""
     if error_events:
         msg = error_events[0].get("message", "")
 
     return msg
 
 
-def _get_compute_name(node: Optional[ResultNode]) -> Optional[str]:
+def _get_compute_name(query_header_context: Any) -> Optional[str]:
     # Get the name of the specified compute resource from the node's
     # config.
     compute_name = None
-    if node and node.config:
-        compute_name = node.config.get("databricks_compute", None)
+    if (
+        query_header_context
+        and hasattr(query_header_context, "config")
+        and query_header_context.config
+    ):
+        compute_name = query_header_context.config.get("databricks_compute", None)
     return compute_name
 
 
-def _get_http_path(node: Optional[ResultNode], creds: DatabricksCredentials) -> Optional[str]:
+def _get_http_path(query_header_context: Any, creds: DatabricksCredentials) -> Optional[str]:
     """Get the http_path for the compute specified for the node.
     If none is specified default will be used."""
 
     thread_id = (os.getpid(), get_ident())
 
     # ResultNode *should* have relation_name attr, but we work around a core
     # issue by checking.
-    relation_name = getattr(node, "relation_name", "[unknown]")
+    relation_name = getattr(query_header_context, "relation_name", "[unknown]")
 
     # If there is no node we return the http_path for the default compute.
-    if not node:
+    if not query_header_context:
         if not USE_LONG_SESSIONS:
             logger.debug(f"Thread {thread_id}: using default compute resource.")
         return creds.http_path
 
     # Get the name of the compute resource specified in the node's config.
     # If none is specified return the http_path for the default compute.
-    compute_name = _get_compute_name(node)
+    compute_name = _get_compute_name(query_header_context)
     if not compute_name:
         if not USE_LONG_SESSIONS:
             logger.debug(f"On thread {thread_id}: {relation_name} using default compute resource.")
         return creds.http_path
 
     # Get the http_path for the named compute.
     http_path = None
     if creds.compute:
         http_path = creds.compute.get(compute_name, {}).get("http_path", None)
 
     # no http_path for the named compute resource is an error condition
     if not http_path:
-        raise dbt.exceptions.DbtRuntimeError(
+        raise DbtRuntimeError(
             f"Compute resource {compute_name} does not exist or "
             f"does not specify http_path, relation: {relation_name}"
         )
 
     if not USE_LONG_SESSIONS:
         logger.debug(
             f"On thread {thread_id}: {relation_name} using compute resource '{compute_name}'."
         )
 
     return http_path
 
 
-def _get_max_idle_time(node: Optional[ResultNode], creds: DatabricksCredentials) -> int:
+def _get_max_idle_time(query_header_context: Any, creds: DatabricksCredentials) -> int:
     """Get the http_path for the compute specified for the node.
     If none is specified default will be used."""
 
     max_idle_time = (
         DEFAULT_MAX_IDLE_TIME if creds.connect_max_idle is None else creds.connect_max_idle
     )
 
-    if node:
-        compute_name = _get_compute_name(node)
+    if query_header_context:
+        compute_name = _get_compute_name(query_header_context)
         if compute_name and creds.compute:
             max_idle_time = creds.compute.get(compute_name, {}).get(
                 "connect_max_idle", max_idle_time
             )
 
     if not isinstance(max_idle_time, Number):
         if isinstance(max_idle_time, str) and max_idle_time.strip().isnumeric():
             return int(max_idle_time.strip())
         else:
-            raise dbt.exceptions.DbtRuntimeError(
+            raise DbtRuntimeError(
                 f"{max_idle_time} is not a valid value for connect_max_idle. "
                 "Must be a number of seconds."
             )
 
     return max_idle_time
```

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/impl.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dataclasses import dataclass
 import os
 import re
 from typing import (
     Any,
     ClassVar,
     Dict,
+    FrozenSet,
     Generic,
     Iterable,
     Iterator,
     List,
     Optional,
     Set,
     Tuple,
@@ -38,22 +39,19 @@
     GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME,
     KEY_TABLE_OWNER,
     KEY_TABLE_STATISTICS,
     LIST_RELATIONS_MACRO_NAME,
     LIST_SCHEMAS_MACRO_NAME,
     TABLE_OR_VIEW_NOT_FOUND_MESSAGES,
 )
-from dbt.clients.agate_helper import DEFAULT_TYPE_TESTER, empty_table
-from dbt.contracts.connection import AdapterResponse, Connection
-from dbt.contracts.graph.manifest import Manifest
-from dbt.contracts.graph.nodes import ResultNode, ModelNode
-from dbt.contracts.relation import RelationType
-import dbt.exceptions
-from dbt.events import AdapterLogger
-from dbt.utils import executor
+from dbt_common.clients.agate_helper import DEFAULT_TYPE_TESTER, empty_table
+from dbt.adapters.contracts.connection import AdapterResponse, Connection
+from dbt.adapters.contracts.relation import RelationType
+from dbt.adapters.events.logging import AdapterLogger
+from dbt_common.utils import executor
 
 from dbt.adapters.databricks.column import DatabricksColumn
 from dbt.adapters.databricks.connections import DatabricksConnectionManager
 from dbt.adapters.databricks.python_submissions import (
     DbtDatabricksAllPurposeClusterPythonJobHelper,
     DbtDatabricksJobClusterPythonJobHelper,
 )
@@ -65,15 +63,17 @@
 from dbt.adapters.databricks.relation_configs.base import (
     DatabricksRelationConfig,
     DatabricksRelationConfigBase,
 )
 from dbt.adapters.databricks.relation_configs.materialized_view import MaterializedViewConfig
 from dbt.adapters.databricks.relation_configs.streaming_table import StreamingTableConfig
 from dbt.adapters.databricks.utils import redact_credentials, undefined_proof, get_first_row
-from dbt.adapters.relation_configs.config_base import RelationResults
+from dbt.adapters.relation_configs import RelationResults
+from dbt.adapters.contracts.relation import RelationConfig
+from dbt_common.exceptions import DbtRuntimeError
 
 
 logger = AdapterLogger("Databricks")
 
 CURRENT_CATALOG_MACRO_NAME = "current_catalog"
 USE_CATALOG_MACRO_NAME = "use_catalog"
 GET_CATALOG_MACRO_NAME = "get_catalog"
@@ -136,25 +136,25 @@
             Capability.TableLastModifiedMetadata: CapabilitySupport(support=Support.Full),
             Capability.SchemaMetadataByRelations: CapabilitySupport(support=Support.Full),
         }
     )
 
     # override/overload
     def acquire_connection(
-        self, name: Optional[str] = None, node: Optional[ResultNode] = None
+        self, name: Optional[str] = None, query_header_context: Any = None
     ) -> Connection:
-        return self.connections.set_connection_name(name, node)
+        return self.connections.set_connection_name(name, query_header_context)
 
     # override
     @contextmanager
-    def connection_named(self, name: str, node: Optional[ResultNode] = None) -> Iterator[None]:
+    def connection_named(self, name: str, query_header_context: Any = None) -> Iterator[None]:
         try:
             if self.connections.query_header is not None:
-                self.connections.query_header.set(name, node)
-            self.acquire_connection(name, node)
+                self.connections.query_header.set(name, query_header_context)
+            self.acquire_connection(name, query_header_context)
             yield
         finally:
             self.release_connection()
             if self.connections.query_header is not None:
                 self.connections.query_header.reset()
 
     @available.parse(lambda *a, **k: 0)
@@ -204,15 +204,15 @@
 
     def list_relations_without_caching(  # type: ignore[override]
         self, schema_relation: DatabricksRelation
     ) -> List[DatabricksRelation]:
         kwargs = {"schema_relation": schema_relation}
         try:
             results = self.execute_macro(LIST_RELATIONS_MACRO_NAME, kwargs=kwargs)
-        except dbt.exceptions.DbtRuntimeError as e:
+        except DbtRuntimeError as e:
             errmsg = getattr(e, "msg", "")
             if check_not_found_error(errmsg):
                 return []
             else:
                 description = "Error while retrieving information about"
                 logger.debug(f"{description} {schema_relation}: {e.msg}")
                 raise e
@@ -234,27 +234,27 @@
     ) -> List[Tuple[DatabricksRelation, str]]:
         results: List[Row]
         kwargs = {"schema_relation": schema_relation}
         try:
             # The catalog for `show table extended` needs to match the current catalog.
             with self._catalog(schema_relation.database):
                 results = list(self.execute_macro(SHOW_TABLE_EXTENDED_MACRO_NAME, kwargs=kwargs))
-        except dbt.exceptions.DbtRuntimeError as e:
+        except DbtRuntimeError as e:
             errmsg = getattr(e, "msg", "")
             if check_not_found_error(errmsg):
                 results = []
             else:
                 description = "Error while retrieving information about"
                 logger.debug(f"{description} {schema_relation.without_identifier()}: {e.msg}")
                 raise e
 
         relations: List[Tuple[DatabricksRelation, str]] = []
         for row in results:
             if len(row) != 4:
-                raise dbt.exceptions.DbtRuntimeError(
+                raise DbtRuntimeError(
                     f'Invalid value from "show table extended ...", '
                     f"got {len(row)} values, expected 4"
                 )
             _schema, name, _, information = row
             rel_type = RelationType.View if "Type: VIEW" in information else RelationType.Table
             relation = self.Relation.create(
                 database=schema_relation.database,
@@ -394,15 +394,15 @@
             # it is either a table or a streaming table
             return (
                 DatabricksRelationType.StreamingTable
                 if table_names[name]
                 else DatabricksRelationType.Table
             )
         else:
-            raise dbt.exceptions.DbtRuntimeError(
+            raise DbtRuntimeError(
                 f"Unexpected relation type discovered: Database:{database}, Relation:{name}"
             )
 
     def get_relation(
         self,
         database: Optional[str],
         schema: str,
@@ -463,15 +463,15 @@
             rows: List[Row] = list(
                 self.execute_macro(
                     GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME,
                     kwargs={"relation": relation},
                 )
             )
             metadata, columns = self.parse_describe_extended(relation, rows)
-        except dbt.exceptions.DbtRuntimeError as e:
+        except DbtRuntimeError as e:
             # spark would throw error when table doesn't exist, where other
             # CDW would just return and empty list, normalizing the behavior here
             errmsg = getattr(e, "msg", "")
             found_msgs = (msg in errmsg for msg in TABLE_OR_VIEW_NOT_FOUND_MESSAGES)
             if any(found_msgs):
                 metadata = None
                 columns = []
@@ -530,16 +530,18 @@
                 column=column_name,
                 dtype=DatabricksColumn.translate_type(column_type),
                 table_stats=table_stats,
             )
             columns.append(column)
         return columns
 
-    def get_catalog(self, manifest: Manifest) -> Tuple[Table, List[Exception]]:  # type: ignore
-        schema_map = self._get_catalog_schemas(manifest)
+    def get_catalog(
+        self, relation_configs: Iterable[RelationConfig], used_schemas: FrozenSet[Tuple[str, str]]
+    ) -> Tuple[Table, List[Exception]]:  # type: ignore
+        schema_map = self._get_catalog_schemas(relation_configs)
 
         with executor(self.config) as tpe:
             futures: List[Future[Table]] = []
             for info, schemas in schema_map.items():
                 if is_hive_metastore(info.database):
                     for schema in schemas:
                         futures.append(
@@ -550,45 +552,34 @@
                                 schema,
                                 "*",
                             )
                         )
                 else:
                     name = ".".join([str(info.database), "information_schema"])
                     fut = tpe.submit_connected(
-                        self,
-                        name,
-                        self._get_one_unity_catalog,
-                        info,
-                        schemas,
-                        manifest,
+                        self, name, self._get_one_unity_catalog, info, used_schemas
                     )
                     futures.append(fut)
             catalogs, exceptions = catch_as_completed(futures)
         return catalogs, exceptions
 
     def _get_one_unity_catalog(
-        self, info: InformationSchema, schemas: Set[str], manifest: Manifest
+        self, info: InformationSchema, schemas: FrozenSet[Tuple[str, str]]
     ) -> Table:
         kwargs = {
             "information_schema": info,
             "schemas": schemas,
         }
-        table = self.execute_macro(
-            GET_CATALOG_MACRO_NAME,
-            kwargs=kwargs,
-            # pass in the full manifest, so we get any local project
-            # overrides
-            manifest=manifest,
-        )
+        table = self.execute_macro(GET_CATALOG_MACRO_NAME, kwargs=kwargs)
 
-        results = self._catalog_filter_table(table, manifest)  # type: ignore[arg-type]
+        results = self._catalog_filter_table(table, schemas)
         return results
 
     def get_catalog_by_relations(
-        self, manifest: Manifest, relations: Set[BaseRelation]
+        self, used_schemas: FrozenSet[Tuple[str, str]], relations: Set[BaseRelation]
     ) -> Tuple[Table, List[Exception]]:
         with executor(self.config) as tpe:
             relations_by_catalog = self._get_catalog_relations_by_info_schema(relations)
 
             futures: List[Future[Table]] = []
 
             for info_schema, catalog_relations in relations_by_catalog.items():
@@ -612,15 +603,15 @@
                     name = ".".join([str(info_schema.database), "information_schema"])
                     fut = tpe.submit_connected(
                         self,
                         name,
                         self._get_one_catalog_by_relations,
                         info_schema,
                         catalog_relations,
-                        manifest,
+                        used_schemas,
                     )
                     futures.append(fut)
 
             catalogs, exceptions = catch_as_completed(futures)
         return catalogs, exceptions
 
     def _get_hive_catalog(
@@ -745,26 +736,27 @@
                 return_columns[name] = columns[name]
 
         return return_columns
 
     @available.parse(lambda *a, **k: {})
     def get_relation_config(self, relation: DatabricksRelation) -> DatabricksRelationConfigBase:
         if relation.type == DatabricksRelationType.MaterializedView:
-            return MaterializedViewAPI.get_relation_config(self, relation)
+            return MaterializedViewAPI.get_from_relation(self, relation)
         elif relation.type == DatabricksRelationType.StreamingTable:
-            return StreamingTableAPI.get_relation_config(self, relation)
+            return StreamingTableAPI.get_from_relation(self, relation)
         else:
             raise NotImplementedError(f"Relation type {relation.type} is not supported.")
 
     @available.parse(lambda *a, **k: {})
-    def get_config_from_model(self, model: ModelNode) -> DatabricksRelationConfigBase:
+    def get_config_from_model(self, model: RelationConfig) -> DatabricksRelationConfigBase:
+        assert model.config, "Config was missing from relation"
         if model.config.materialized == "materialized_view":
-            return MaterializedViewAPI.get_config_from_model(model)
+            return MaterializedViewAPI.get_from_relation_config(model)
         elif model.config.materialized == "streaming_table":
-            return StreamingTableAPI.get_config_from_model(model)
+            return StreamingTableAPI.get_from_relation_config(model)
         else:
             raise NotImplementedError(
                 f"Materialization {model.config.materialized} is not supported."
             )
 
 
 @dataclass(frozen=True)
@@ -779,28 +771,28 @@
     @abstractmethod
     def config_type(cls) -> Type[DatabricksRelationConfig]:
         """Get the config class for delegating calls."""
 
         raise NotImplementedError("Must be implemented by subclass")
 
     @classmethod
-    def get_relation_config(
+    def get_from_relation(
         cls, adapter: DatabricksAdapter, relation: DatabricksRelation
     ) -> DatabricksRelationConfig:
         """Get the relation config from the relation."""
 
         assert relation.type == cls.relation_type
         results = cls._describe_relation(adapter, relation)
         return cls.config_type().from_results(results)
 
     @classmethod
-    def get_config_from_model(cls, model: ModelNode) -> DatabricksRelationConfig:
+    def get_from_relation_config(cls, relation_config: RelationConfig) -> DatabricksRelationConfig:
         """Get the relation config from the model node."""
 
-        return cls.config_type().from_model_node(model)
+        return cls.config_type().from_relation_config(relation_config)
 
     @classmethod
     @abstractmethod
     def _describe_relation(
         cls, adapter: DatabricksAdapter, relation: DatabricksRelation
     ) -> RelationResults:
         """Describe the relation and return the results."""
@@ -822,20 +814,25 @@
         kwargs = {"table_name": relation}
         results: RelationResults = dict()
         results["describe_extended"] = adapter.execute_macro(
             DESCRIBE_TABLE_EXTENDED_MACRO_NAME, kwargs=kwargs
         )
 
         kwargs = {"relation": relation}
-        results["information_schema.views"] = get_first_row(
-            adapter.execute_macro("get_view_description", kwargs=kwargs)
-        )
+        results["information_schema.views"] = cls._get_information_schema_views(adapter, kwargs)
         results["show_tblproperties"] = adapter.execute_macro("fetch_tbl_properties", kwargs=kwargs)
         return results
 
+    @staticmethod
+    def _get_information_schema_views(adapter: DatabricksAdapter, kwargs: Dict[str, Any]) -> Row:
+        row = get_first_row(adapter.execute_macro("get_view_description", kwargs=kwargs))
+        if "view_definition" in row.keys() and row["view_definition"] is not None:
+            return row
+        return get_first_row(adapter.execute_macro("get_view_description_alt", kwargs=kwargs))
+
 
 class StreamingTableAPI(RelationAPIBase[StreamingTableConfig]):
     relation_type = DatabricksRelationType.StreamingTable
 
     @classmethod
     def config_type(cls) -> Type[StreamingTableConfig]:
         return StreamingTableConfig
```

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/python_submissions.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/python_submissions.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 import base64
 import time
 import uuid
 
 from urllib3.util.retry import Retry
 
-from dbt.events import AdapterLogger
-import dbt.exceptions
+from dbt.adapters.events.logging import AdapterLogger
 from dbt.adapters.base import PythonJobHelper
 
 from requests.adapters import HTTPAdapter
 from dbt.adapters.databricks.connections import BearerAuth
+from dbt_common.exceptions import DbtRuntimeError
 
 
 logger = AdapterLogger("Databricks")
 
 DEFAULT_POLLING_INTERVAL = 10
 SUBMISSION_LANGUAGE = "python"
 DEFAULT_TIMEOUT = 60 * 60 * 24
@@ -67,15 +67,15 @@
             f"https://{self.credentials.host}/api/2.0/workspace/mkdirs",
             headers=self.extra_headers,
             json={
                 "path": path,
             },
         )
         if response.status_code != 200:
-            raise dbt.exceptions.DbtRuntimeError(
+            raise DbtRuntimeError(
                 f"Error creating work_dir for python notebooks\n {response.content!r}"
             )
 
     def _update_with_acls(self, cluster_dict: dict) -> dict:
         acl = self.parsed_model["config"].get("access_control_list", None)
         if acl:
             cluster_dict.update({"access_control_list": acl})
@@ -91,17 +91,15 @@
                 "content": b64_encoded_content,
                 "language": "PYTHON",
                 "overwrite": True,
                 "format": "SOURCE",
             },
         )
         if response.status_code != 200:
-            raise dbt.exceptions.DbtRuntimeError(
-                f"Error creating python notebook.\n {response.content!r}"
-            )
+            raise DbtRuntimeError(f"Error creating python notebook.\n {response.content!r}")
 
     def _submit_job(self, path: str, cluster_spec: dict) -> str:
         job_spec = {
             "run_name": f"{self.schema}-{self.identifier}-{uuid.uuid4()}",
             "notebook_task": {
                 "notebook_path": path,
             },
@@ -130,17 +128,15 @@
         job_spec.update({"libraries": libraries})  # type: ignore
         submit_response = self.session.post(
             f"https://{self.credentials.host}/api/2.1/jobs/runs/submit",
             headers=self.extra_headers,
             json=job_spec,
         )
         if submit_response.status_code != 200:
-            raise dbt.exceptions.DbtRuntimeError(
-                f"Error creating python run.\n {submit_response.content!r}"
-            )
+            raise DbtRuntimeError(f"Error creating python run.\n {submit_response.content!r}")
         response_json = submit_response.json()
         logger.info(f"Job submission response={response_json}")
         return response_json["run_id"]
 
     def _submit_through_notebook(self, compiled_code: str, cluster_spec: dict) -> None:
         # it is safe to call mkdirs even if dir already exists and have content inside
         work_dir = f"/Shared/dbt_python_model/{self.schema}/"
@@ -168,15 +164,15 @@
         run_output = self.session.get(
             f"https://{self.credentials.host}" f"/api/2.1/jobs/runs/get-output?run_id={run_id}",
             headers=self.extra_headers,
         )
         json_run_output = run_output.json()
         result_state = json_run_output["metadata"]["state"]["result_state"]
         if result_state != "SUCCESS":
-            raise dbt.exceptions.DbtRuntimeError(
+            raise DbtRuntimeError(
                 "Python model failed with traceback as:\n"
                 "(Note that the line number here does not "
                 "match the line number in your code due to dbt templating)\n"
                 f"{utils.remove_ansi(json_run_output['error_trace'])}"
             )
 
     def submit(self, compiled_code: str) -> None:
@@ -202,17 +198,17 @@
                 exceeded_timeout = True
                 break
             # should we do exponential backoff?
             time.sleep(self.polling_interval)
             response = status_func(**status_func_kwargs)
             state = get_state_func(response)
         if exceeded_timeout:
-            raise dbt.exceptions.DbtRuntimeError("python model run timed out")
+            raise DbtRuntimeError("python model run timed out")
         if state != expected_end_state:
-            raise dbt.exceptions.DbtRuntimeError(
+            raise DbtRuntimeError(
                 "python model run ended in state"
                 f"{state} with state_message\n{get_state_msg_func(response)}"
             )
         return response
 
 
 class JobClusterPythonJobHelper(BaseDatabricksHelper):
@@ -255,47 +251,41 @@
             headers=self.extra_headers,
             json={
                 "clusterId": self.cluster_id,
                 "language": SUBMISSION_LANGUAGE,
             },
         )
         if response.status_code != 200:
-            raise dbt.exceptions.DbtRuntimeError(
-                f"Error creating an execution context.\n {response.content!r}"
-            )
+            raise DbtRuntimeError(f"Error creating an execution context.\n {response.content!r}")
         return response.json()["id"]
 
     def destroy(self, context_id: str) -> str:
         # https://docs.databricks.com/dev-tools/api/1.2/index.html#delete-an-execution-context
         response = self.session.post(
             f"https://{self.host}/api/1.2/contexts/destroy",
             headers=self.extra_headers,
             json={
                 "clusterId": self.cluster_id,
                 "contextId": context_id,
             },
         )
         if response.status_code != 200:
-            raise dbt.exceptions.DbtRuntimeError(
-                f"Error deleting an execution context.\n {response.content!r}"
-            )
+            raise DbtRuntimeError(f"Error deleting an execution context.\n {response.content!r}")
         return response.json()["id"]
 
     def get_cluster_status(self) -> Dict:
         # https://docs.databricks.com/dev-tools/api/latest/clusters.html#get
 
         response = self.session.get(
             f"https://{self.host}/api/2.0/clusters/get",
             headers=self.extra_headers,
             json={"cluster_id": self.cluster_id},
         )
         if response.status_code != 200:
-            raise dbt.exceptions.DbtRuntimeError(
-                f"Error getting status of cluster.\n {response.content!r}"
-            )
+            raise DbtRuntimeError(f"Error getting status of cluster.\n {response.content!r}")
 
         json_response = response.json()
         return json_response
 
     def start_cluster(self) -> None:
         """Send the start command and poll for the cluster status until it shows "Running"
 
@@ -308,17 +298,15 @@
 
         response = self.session.post(
             f"https://{self.host}/api/2.0/clusters/start",
             headers=self.extra_headers,
             json={"cluster_id": self.cluster_id},
         )
         if response.status_code != 200:
-            raise dbt.exceptions.DbtRuntimeError(
-                f"Error starting terminated cluster.\n {response.content!r}"
-            )
+            raise DbtRuntimeError(f"Error starting terminated cluster.\n {response.content!r}")
 
         self._wait_for_cluster_to_start()
 
     def _wait_for_cluster_to_start(self) -> None:
         # seconds
         logger.info("Waiting for cluster to be ready")
 
@@ -331,15 +319,15 @@
         while get_elapsed() < MAX_CLUSTER_START_TIME:
             status_response = self.get_cluster_status()
             if str(status_response.get("state")).lower() == "running":
                 return
             else:
                 time.sleep(5)
 
-        raise dbt.exceptions.DbtRuntimeError(
+        raise DbtRuntimeError(
             f"Cluster {self.cluster_id} restart timed out after {MAX_CLUSTER_START_TIME} seconds"
         )
 
 
 class DBCommand:
     def __init__(
         self,
@@ -363,34 +351,30 @@
                 "contextId": context_id,
                 "language": SUBMISSION_LANGUAGE,
                 "command": command,
             },
         )
         logger.info(f"Job submission response={response.json()}")
         if response.status_code != 200:
-            raise dbt.exceptions.DbtRuntimeError(
-                f"Error creating a command.\n {response.content!r}"
-            )
+            raise DbtRuntimeError(f"Error creating a command.\n {response.content!r}")
         return response.json()["id"]
 
     def status(self, context_id: str, command_id: str) -> Dict[str, Any]:
         # https://docs.databricks.com/dev-tools/api/1.2/index.html#get-information-about-a-command
         response = self.session.get(
             f"https://{self.host}/api/1.2/commands/status",
             headers=self.extra_headers,
             params={
                 "clusterId": self.cluster_id,
                 "contextId": context_id,
                 "commandId": command_id,
             },
         )
         if response.status_code != 200:
-            raise dbt.exceptions.DbtRuntimeError(
-                f"Error getting status of command.\n {response.content!r}"
-            )
+            raise DbtRuntimeError(f"Error getting status of command.\n {response.content!r}")
         return response.json()
 
 
 class AllPurposeClusterPythonJobHelper(BaseDatabricksHelper):
     def check_credentials(self) -> None:
         if not self.cluster_id:
             raise ValueError(
@@ -427,15 +411,15 @@
                     },
                     get_state_func=lambda response: response["status"],
                     terminal_states=("Cancelled", "Error", "Finished"),
                     expected_end_state="Finished",
                     get_state_msg_func=lambda response: response.json()["results"]["data"],
                 )
                 if response["results"]["resultType"] == "error":
-                    raise dbt.exceptions.DbtRuntimeError(
+                    raise DbtRuntimeError(
                         f"Python model failed with traceback as:\n"
                         f"{utils.remove_ansi(response['results']['cause'])}"
                     )
             finally:
                 context.destroy(context_id)
```

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from dataclasses import dataclass, field
 from typing import Any, Dict, Iterable, Optional, Set, Type
-from dbt.contracts.relation import (
+from dbt.adapters.contracts.relation import (
     ComponentName,
 )
 from dbt.adapters.base.relation import BaseRelation, Policy, InformationSchema
 from dbt.adapters.spark.impl import KEY_TABLE_OWNER, KEY_TABLE_STATISTICS
-from dbt.dataclass_schema import StrEnum
+from dbt_common.dataclass_schema import StrEnum
 
 from dbt.adapters.databricks.utils import remove_undefined
-from dbt.utils import filter_null_values, classproperty
-from dbt.exceptions import DbtRuntimeError
+from dbt_common.utils import filter_null_values
+from dbt.adapters.utils import classproperty
+from dbt_common.exceptions import DbtRuntimeError
 
 KEY_TABLE_PROVIDER = "Provider"
 
 
 @dataclass
 class DatabricksQuotePolicy(Policy):
     database: bool = True
@@ -31,14 +32,15 @@
 class DatabricksRelationType(StrEnum):
     Table = "table"
     View = "view"
     CTE = "cte"
     MaterializedView = "materialized_view"
     External = "external"
     StreamingTable = "streaming_table"
+    Unknown = "unknown"
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class DatabricksInformationSchema(InformationSchema):
     quote_policy: Policy = field(default_factory=lambda: DatabricksQuotePolicy())
     include_policy: Policy = field(default_factory=lambda: DatabricksIncludePolicy())
     quote_character: str = "`"
@@ -61,30 +63,14 @@
         data = super().__pre_deserialize__(data)
         if "database" not in data["path"]:
             data["path"]["database"] = None
         else:
             data["path"]["database"] = remove_undefined(data["path"]["database"])
         return data
 
-    renameable_relations = frozenset(
-        {
-            DatabricksRelationType.View,
-            DatabricksRelationType.Table,
-        }
-    )
-
-    # list relations that can be atomically replaced (e.g. `CREATE OR REPLACE my_relation..`
-    # versus `DROP` and `CREATE`)
-    replaceable_relations = frozenset(
-        {
-            DatabricksRelationType.View,
-            DatabricksRelationType.Table,
-        }
-    )
-
     def has_information(self) -> bool:
         return self.metadata is not None
 
     @property
     def is_materialized_view(self) -> bool:
         return self.type == DatabricksRelationType.MaterializedView
```

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/base.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from pydantic import BaseModel, ConfigDict
-from typing import ClassVar, Dict, Generic, List, Optional, TypeVar
+from typing import Any, ClassVar, Dict, Generic, List, Optional, TypeVar
 from typing_extensions import Self, Type
 
 from dbt.adapters.relation_configs.config_base import RelationResults
-from dbt.contracts.graph.nodes import ModelNode
+from dbt.adapters.contracts.relation import RelationConfig
 
 
 class DatabricksComponentConfig(BaseModel):
     """Class for encapsulating a single component of a Databricks relation config.
 
     Ex: A materialized view has a `query` component, which is a string that if changed, requires a
     full refresh.
@@ -64,22 +64,22 @@
 
     # The name of the component. This is used as the key in the config dictionary of the relation
     # config.
     name: ClassVar[str]
 
     @classmethod
     @abstractmethod
-    def from_results(cls, row: RelationResults) -> Component:
+    def from_relation_results(cls, row: RelationResults) -> Component:
         """Extract the component from the results of a query against the existing relation."""
 
         raise NotImplementedError("Must be implemented by subclass")
 
     @classmethod
     @abstractmethod
-    def from_model_node(cls, model_node: ModelNode) -> Component:
+    def from_relation_config(cls, model_node: RelationConfig) -> Component:
         """Extract the component from the model node.
 
         While some components, e.g. query, can be extracted directly from the model node,
         specialized Databricks config can be found in model_node.config.extra.
         """
 
         raise NotImplementedError("Must be implemented by subclass")
@@ -96,32 +96,32 @@
     # The list of components that make up the relation config. In the base implemenation, these
     # components are applied sequentially to either the existing relation, or the model node, to
     # build up the config.
     config_components: ClassVar[List[Type[DatabricksComponentProcessor]]]
     config: Dict[str, DatabricksComponentConfig]
 
     @classmethod
-    def from_model_node(cls, model_node: ModelNode) -> Self:
+    def from_relation_config(cls, relation_config: RelationConfig) -> Self:
         """Build the relation config from a model node."""
 
         config_dict: Dict[str, DatabricksComponentConfig] = {}
         for component in cls.config_components:
-            model_component = component.from_model_node(model_node)
-            if model_component:
-                config_dict[component.name] = model_component
+            relation_component = component.from_relation_config(relation_config)
+            if relation_component:
+                config_dict[component.name] = relation_component
 
         return cls(config=config_dict)
 
     @classmethod
     def from_results(cls, results: RelationResults) -> Self:
         """Build the relation config from the results of a query against the existing relation."""
 
         config_dict: Dict[str, DatabricksComponentConfig] = {}
         for component in cls.config_components:
-            result_component = component.from_results(results)
+            result_component = component.from_relation_results(results)
             if result_component:
                 config_dict[component.name] = result_component
 
         return cls(config=config_dict)
 
     @abstractmethod
     def get_changeset(self, existing: Self) -> Optional[DatabricksRelationChangeSet]:
@@ -130,7 +130,16 @@
         None.
         """
 
         raise NotImplementedError("Must be implemented by subclass")
 
 
 DatabricksRelationConfig = TypeVar("DatabricksRelationConfig", bound=DatabricksRelationConfigBase)
+
+
+def get_config_value(config: RelationConfig, key: str) -> Any:
+    """Get a value from the config.extra dictionary, or None if it is not present."""
+
+    materialization_config = config.config
+    if materialization_config:
+        return materialization_config.extra.get(key)
+    return None
```

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/comment.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/comment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from typing import Optional, ClassVar
-from dbt.contracts.graph.nodes import ModelNode
-
 from dbt.adapters.databricks.relation_configs.base import (
     DatabricksComponentConfig,
     DatabricksComponentProcessor,
 )
 from dbt.adapters.relation_configs.config_base import RelationResults
+from dbt.adapters.contracts.relation import RelationConfig
 
 
 class CommentConfig(DatabricksComponentConfig):
     """Component encapsulating the relation-level comment."""
 
     comment: Optional[str] = None
 
 
 class CommentProcessor(DatabricksComponentProcessor[CommentConfig]):
     name: ClassVar[str] = "comment"
 
     @classmethod
-    def from_results(cls, results: RelationResults) -> CommentConfig:
+    def from_relation_results(cls, results: RelationResults) -> CommentConfig:
         table = results["describe_extended"]
         for row in table.rows:
             if row[0] == "Comment":
                 return CommentConfig(comment=row[1])
         return CommentConfig()
 
     @classmethod
-    def from_model_node(cls, model_node: ModelNode) -> CommentConfig:
-        if model_node.description is not None:
-            return CommentConfig(comment=model_node.description)
-        return CommentConfig()
+    def from_relation_config(cls, relation_config: RelationConfig) -> CommentConfig:
+        return CommentConfig(comment=getattr(relation_config, "description"))
```

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/materialized_view.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/materialized_view.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/partitioning.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/partitioning.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import itertools
-from typing import ClassVar, List
+from typing import ClassVar, List, Union
 
 from dbt.adapters.relation_configs.config_base import RelationResults
-from dbt.contracts.graph.nodes import ModelNode
+from dbt.adapters.contracts.relation import RelationConfig
+from dbt.adapters.databricks.relation_configs import base
 from dbt.adapters.databricks.relation_configs.base import (
     DatabricksComponentConfig,
     DatabricksComponentProcessor,
 )
 
 
 class PartitionedByConfig(DatabricksComponentConfig):
@@ -15,28 +16,30 @@
     partition_by: List[str]
 
 
 class PartitionedByProcessor(DatabricksComponentProcessor):
     name: ClassVar[str] = "partition_by"
 
     @classmethod
-    def from_results(cls, results: RelationResults) -> PartitionedByConfig:
+    def from_relation_results(cls, results: RelationResults) -> PartitionedByConfig:
         table = results["describe_extended"]
         cols = []
         rows = itertools.takewhile(
             lambda row: row[0],
             itertools.dropwhile(lambda row: row[0] != "# Partition Information", table.rows),
         )
         for row in rows:
             if not row[0].startswith("# "):
                 cols.append(row[0])
 
         return PartitionedByConfig(partition_by=cols)
 
     @classmethod
-    def from_model_node(cls, model_node: ModelNode) -> PartitionedByConfig:
-        partition_by = model_node.config.extra.get("partition_by")
-        if isinstance(partition_by, str):
-            return PartitionedByConfig(partition_by=[partition_by])
+    def from_relation_config(cls, relation_config: RelationConfig) -> PartitionedByConfig:
+        partition_by: Union[str, List[str], None] = base.get_config_value(
+            relation_config, "partition_by"
+        )
         if not partition_by:
             return PartitionedByConfig(partition_by=[])
+        if isinstance(partition_by, str):
+            return PartitionedByConfig(partition_by=[partition_by])
         return PartitionedByConfig(partition_by=partition_by)
```

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/query.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from typing import ClassVar
 from dbt.adapters.relation_configs.config_base import RelationResults
-from dbt.contracts.graph.nodes import ModelNode
+from dbt.adapters.contracts.relation import RelationConfig
 from dbt.adapters.databricks.relation_configs.base import (
     DatabricksComponentConfig,
     DatabricksComponentProcessor,
 )
-from dbt.exceptions import DbtRuntimeError
+from dbt_common.exceptions import DbtRuntimeError
 
 
 class QueryConfig(DatabricksComponentConfig):
     """Component encapsulating the query that defines a relation."""
 
     query: str
 
 
 class QueryProcessor(DatabricksComponentProcessor[QueryConfig]):
     name: ClassVar[str] = "query"
 
     @classmethod
-    def from_results(cls, result: RelationResults) -> QueryConfig:
+    def from_relation_results(cls, result: RelationResults) -> QueryConfig:
         row = result["information_schema.views"]
         return QueryConfig(query=row["view_definition"])
 
     @classmethod
-    def from_model_node(cls, model_node: ModelNode) -> QueryConfig:
-        query = model_node.compiled_code
+    def from_relation_config(cls, relation_config: RelationConfig) -> QueryConfig:
+        query = relation_config.compiled_code
 
         if query:
             return QueryConfig(query=query.strip())
         else:
-            raise DbtRuntimeError(f"Cannot compile model {model_node.unique_id} with no SQL query")
+            raise DbtRuntimeError(
+                f"Cannot compile model {relation_config.identifier} with no SQL query"
+            )
```

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/refresh.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/refresh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from typing import ClassVar, Optional
 
 from dbt.adapters.relation_configs.config_base import RelationResults
-from dbt.exceptions import DbtRuntimeError
-from dbt.contracts.graph.nodes import ModelNode
-
+from dbt_common.exceptions import DbtRuntimeError
+from dbt.adapters.contracts.relation import RelationConfig
+from dbt.adapters.databricks.relation_configs import base
 from dbt.adapters.databricks.relation_configs.base import (
     DatabricksComponentConfig,
     DatabricksComponentProcessor,
 )
 
 SCHEDULE_REGEX = re.compile(r"CRON '(.*)' AT TIME ZONE '(.*)'")
 
@@ -34,15 +34,15 @@
         return None
 
 
 class RefreshProcessor(DatabricksComponentProcessor[RefreshConfig]):
     name: ClassVar[str] = "refresh"
 
     @classmethod
-    def from_results(cls, results: RelationResults) -> RefreshConfig:
+    def from_relation_results(cls, results: RelationResults) -> RefreshConfig:
         table = results["describe_extended"]
         for row in table.rows:
             if row[0] == "Refresh Schedule":
                 if row[1] == "MANUAL":
                     return RefreshConfig()
 
                 match = SCHEDULE_REGEX.match(row[1])
@@ -59,16 +59,16 @@
 
         raise DbtRuntimeError(
             "Could not parse schedule for table."
             " This is most likely a bug in the dbt-databricks adapter, so please file an issue!"
         )
 
     @classmethod
-    def from_model_node(cls, model_node: ModelNode) -> RefreshConfig:
-        schedule = model_node.config.extra.get("schedule")
+    def from_relation_config(cls, relation_config: RelationConfig) -> RefreshConfig:
+        schedule = base.get_config_value(relation_config, "schedule")
         if schedule:
             if "cron" not in schedule:
                 raise DbtRuntimeError(f"Schedule config must contain a 'cron' key, got {schedule}")
             return RefreshConfig(
                 cron=schedule["cron"], time_zone_value=schedule.get("time_zone_value")
             )
         else:
```

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/streaming_table.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/streaming_table.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/relation_configs/tblproperties.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/relation_configs/tblproperties.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, ClassVar, List
-from dbt.contracts.graph.nodes import ModelNode
-
+from dbt.adapters.databricks.relation_configs import base
 from dbt.adapters.databricks.relation_configs.base import (
     DatabricksComponentConfig,
     DatabricksComponentProcessor,
 )
 from dbt.adapters.relation_configs.config_base import RelationResults
-from dbt.exceptions import DbtRuntimeError
+from dbt.adapters.contracts.relation import RelationConfig
+from dbt_common.exceptions import DbtRuntimeError
 
 
 class TblPropertiesConfig(DatabricksComponentConfig):
     """Component encapsulating the tblproperties of a relation."""
 
     tblproperties: Dict[str, str]
 
@@ -40,27 +40,27 @@
         )
 
 
 class TblPropertiesProcessor(DatabricksComponentProcessor[TblPropertiesConfig]):
     name: ClassVar[str] = "tblproperties"
 
     @classmethod
-    def from_results(cls, results: RelationResults) -> TblPropertiesConfig:
+    def from_relation_results(cls, results: RelationResults) -> TblPropertiesConfig:
         table = results.get("show_tblproperties")
         tblproperties = dict()
 
         if table:
             for row in table.rows:
                 tblproperties[str(row[0])] = str(row[1])
 
         return TblPropertiesConfig(tblproperties=tblproperties)
 
     @classmethod
-    def from_model_node(cls, model_node: ModelNode) -> TblPropertiesConfig:
-        tblproperties = model_node.config.extra.get("tblproperties")
+    def from_relation_config(cls, relation_config: RelationConfig) -> TblPropertiesConfig:
+        tblproperties = base.get_config_value(relation_config, "tblproperties")
         if not tblproperties:
             return TblPropertiesConfig(tblproperties=dict())
         if isinstance(tblproperties, Dict):
             tblproperties = {str(k): str(v) for k, v in tblproperties.items()}
             return TblPropertiesConfig(tblproperties=tblproperties)
         else:
             raise DbtRuntimeError("tblproperties must be a dictionary")
```

### Comparing `dbt-databricks-1.8.0b1/dbt/adapters/databricks/utils.py` & `dbt-databricks-1.8.0b2/dbt/adapters/databricks/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import functools
 import inspect
 import re
 from typing import Any, Callable, Type, TypeVar
-
+from agate import Table, Row
 from dbt.adapters.base import BaseAdapter
 from jinja2.runtime import Undefined
-from agate import Table, Row
 
 
 A = TypeVar("A", bound=BaseAdapter)
 
 
 CREDENTIAL_IN_COPY_INTO_REGEX = re.compile(
     r"(?<=credential)\s*?\((\s*?'\w*?'\s*?=\s*?'.*?'\s*?(?:,\s*?'\w*?'\s*?=\s*?'.*?'\s*?)*?)\)"
```

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/catalog.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/catalog.sql`

 * *Files 8% similar despite different names*

```diff
@@ -67,16 +67,16 @@
     select *
     from tables
     join columns using (table_database, table_schema, table_name)
     order by column_index
 {%- endmacro %}
 
 {% macro databricks__get_catalog_schemas_where_clause_sql(schemas) -%}
-    where ({%- for schema in schemas -%}
-        table_schema = lower('{{ schema }}'){%- if not loop.last %} or {% endif -%}
+    where ({%- for relation in schemas -%}
+        table_schema = lower('{{ relation[1] }}'){%- if not loop.last %} or {% endif -%}
     {%- endfor -%})
 {%- endmacro %}
 
 
 {% macro databricks__get_catalog_relations_where_clause_sql(relations) -%}
     where (
         {%- for relation in relations -%}
```

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/copy_into.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/copy_into.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/databricks_catalog.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/databricks_catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/metadata.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/metadata.sql`

 * *Files 14% similar despite different names*

```diff
@@ -69,12 +69,27 @@
 
   {{ return(load_result('last_modified')) }}
 
 {% endmacro %}
 
 {% macro get_view_description(relation) %}
   {% call statement('get_view_description', fetch_result=True) -%}
-    select * from {{ relation.information_schema() }}.`views` where table_schema = '{{ relation.schema }}' and table_name = '{{ relation.identifier }}'
-  {% endcall %}
+    select * 
+    from {{ relation.information_schema() }}.`views` 
+    where table_schema = '{{ relation.schema }}' 
+      and table_name = '{{ relation.identifier }}'
+  {%- endcall -%}
 
   {% do return(load_result('get_view_description').table) %}
+{% endmacro %}
+
+{% macro get_view_description_alt(relation) %}
+  {% call statement('get_view_description_alt', fetch_result=True) -%}
+    select *
+    from `system`.`information_schema`.`views`
+    where table_catalog = '{{ relation.database }}'
+      and table_schema = '{{ relation.schema }}'
+      and table_name = '{{ relation.identifier }}'
+  {% endcall %}
+
+  {% do return(load_result('get_view_description_alt').table) %}
 {% endmacro %}
```

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/persist_docs.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/python.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/adapters/relation.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/etc/statement.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/clone.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/incremental/incremental.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/incremental/strategies.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/incremental/strategies.sql`

 * *Files 20% similar despite different names*

```diff
@@ -45,34 +45,42 @@
       {% endif %}
     {% endif %}
     table {{ temp_relation }}
         
 {% endmacro %}
 
 {% macro get_insert_into_sql(source_relation, target_relation) %}
+    {%- set source_columns = adapter.get_columns_in_relation(source_relation) | map(attribute="quoted") | list -%}
+    {%- set dest_columns = adapter.get_columns_in_relation(target_relation) | map(attribute="quoted") | list -%}
+    {{ insert_into_sql_impl(target_relation, dest_columns, source_relation, source_columns) }}
+{% endmacro %}
 
+{% macro insert_into_sql_impl(target_relation, dest_columns, source_relation, source_columns) %}
     {%- set common_columns = [] -%}
-    {%- set source_columns = adapter.get_columns_in_relation(source_relation) | map(attribute="name") -%}
-    {%- for dest_col in adapter.get_columns_in_relation(target_relation) -%}
-      {% if dest_col.name in source_columns %}
-          {%- if common_columns.append(dest_col) -%}{%- endif -%}
+    {%- for dest_col in dest_columns -%}
+      {%- if dest_col in source_columns -%}
+        {%- do common_columns.append(dest_col) -%}
+      {%- else -%}
+        {%- do common_columns.append('NULL') -%}
       {%- endif -%}
     {%- endfor -%}
-    {%- set dest_cols_csv = common_columns | map(attribute='quoted') | join(', ') -%}
-    insert into table {{ target_relation }} ({{ dest_cols_csv }})
-    select {{dest_cols_csv}} from {{ source_relation }}
-
-{% endmacro %}
+    {%- set dest_cols_csv = dest_columns | join(', ') -%}
+    {%- set source_cols_csv = common_columns | join(', ') -%}
+insert into table {{ target_relation }} ({{ dest_cols_csv }})
+select {{source_cols_csv}} from {{ source_relation }}
+{%- endmacro %}
 
 {% macro databricks__get_merge_sql(target, source, unique_key, dest_columns, incremental_predicates) %}
   {# need dest_columns for merge_exclude_columns, default to use "*" #}
   {%- set predicates = [] if incremental_predicates is none else [] + incremental_predicates -%}
   {%- set dest_columns = adapter.get_columns_in_relation(target) -%}
+  {%- set source_columns = (adapter.get_columns_in_relation(source) | map(attribute='quoted') | list)-%}
   {%- set merge_update_columns = config.get('merge_update_columns') -%}
   {%- set merge_exclude_columns = config.get('merge_exclude_columns') -%}
+  {%- set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') -%}
   {%- set update_columns = get_merge_update_columns(merge_update_columns, merge_exclude_columns, dest_columns) -%}
 
   {% if unique_key %}
       {% if unique_key is sequence and unique_key is not mapping and unique_key is not string %}
           {% for key in unique_key %}
               {% set this_key_match %}
                   DBT_INTERNAL_SOURCE.{{ key }} <=> DBT_INTERNAL_DEST.{{ key }}
@@ -90,17 +98,35 @@
   {% endif %}
 
   {{ sql_header if sql_header is not none }}
 
   merge into {{ target }} as DBT_INTERNAL_DEST
       using {{ source }} as DBT_INTERNAL_SOURCE
       on {{ predicates | join(' and ') }}
+      when matched then update set {{ get_merge_update_set(update_columns, on_schema_change, source_columns) }}
+      when not matched then insert {{ get_merge_insert(on_schema_change, source_columns) }}
+{% endmacro %}
 
-      when matched then update set
-        {% if update_columns -%}{%- for column_name in update_columns %}
-            {{ column_name }} = DBT_INTERNAL_SOURCE.{{ column_name }}
-            {%- if not loop.last %}, {%- endif %}
-        {%- endfor %}
-        {%- else %} * {% endif %}
+{% macro get_merge_update_set(update_columns, on_schema_change, source_columns) %}
+  {%- if update_columns -%}
+    {%- for column_name in update_columns -%}
+      {{ column_name }} = DBT_INTERNAL_SOURCE.{{ column_name }}{%- if not loop.last %}, {% endif -%}
+    {%- endfor %}
+  {%- elif on_schema_change == 'ignore' -%}
+    *
+  {%- else -%}
+    {%- for column in source_columns -%}
+      {{ column }} = DBT_INTERNAL_SOURCE.{{ column }}{%- if not loop.last %}, {% endif -%}
+    {%- endfor %}
+  {%- endif -%}
+{% endmacro %}
 
-      when not matched then insert *
+{% macro get_merge_insert(on_schema_change, source_columns) %}
+  {%- if on_schema_change == 'ignore' -%}
+    *
+  {%- else -%}
+    ({{ source_columns | join(", ") }}) VALUES (
+    {%- for column in source_columns -%}
+      DBT_INTERNAL_SOURCE.{{ column }}{%- if not loop.last %}, {% endif -%}
+    {%- endfor %})
+  {%- endif -%}
 {% endmacro %}
```

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/incremental/validate.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/materialized_view.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/seeds/helpers.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/seeds/seeds.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/seeds/seeds.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/snapshot.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/streaming_table.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/streaming_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/table.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/materializations/view.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/components/refresh_schedule.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/components/refresh_schedule.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/constraints.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/constraints.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/create.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/drop.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/drop.sql`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-{% macro databricks__drop_relation(relation) -%}
-    {% call statement('drop_relation', auto_begin=False) -%}
-        {{ get_drop_sql(relation) }}
-    {%- endcall %}
-{% endmacro %}
-
 {% macro databricks__get_drop_sql(relation) -%}
     {%- if relation.is_materialized_view -%}
         {{ drop_materialized_view(relation) }}
     {%- elif relation.is_streaming_table-%}
         {{ drop_streaming_table(relation) }}   
     {%- elif relation.is_view -%}
         {{ drop_view(relation) }}
     {%- else -%}
         {{ drop_table(relation) }}
     {%- endif -%}
 {% endmacro %}
+
+{% macro databricks__drop_relation(relation) -%}
+    {% call statement('drop_relation', auto_begin=False) -%}
+        {{ get_drop_sql(relation) }}
+    {%- endcall %}
+{% endmacro %}
```

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/materialized_view/alter.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/materialized_view/create.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/materialized_view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/optimize.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/optimize.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/replace.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/streaming_table/alter.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/streaming_table/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/streaming_table/create.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/streaming_table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/table/create.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/macros/relations/view/create.sql` & `dbt-databricks-1.8.0b2/dbt/include/databricks/macros/relations/view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt/include/databricks/profile_template.yml` & `dbt-databricks-1.8.0b2/dbt/include/databricks/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/dbt_databricks.egg-info/PKG-INFO` & `dbt-databricks-1.8.0b2/dbt_databricks.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,107 +1,109 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
+License: UNKNOWN
+Description: <p align="center">
+          <img src="https://bynder-public-us-west-2.s3.amazonaws.com/styleguide/ABB317701CA31CB7F29268E32B303CAE-pdf-column-1.png" alt="databricks logo" width="50%" />
+          <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="250"/>
+        </p>
+        <p align="center">
+          <a href="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml">
+            <img src="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
+          </a>
+          <a href="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml">
+            <img src="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml/badge.svg?event=push" alt="Integration Tests Badge"/>
+          </a>
+        </p>
+        
+        **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
+        
+        The **[Databricks Lakehouse](https://www.databricks.com/)** provides one simple platform to unify all your data, analytics and AI workloads.
+        
+        # dbt-databricks
+        
+        The `dbt-databricks` adapter contains all of the code enabling dbt to work with Databricks. This adapter is based off the amazing work done in [dbt-spark](https://github.com/dbt-labs/dbt-spark). Some key features include:
+        
+        - **Easy setup**. No need to install an ODBC driver as the adapter uses pure Python APIs.
+        - **Open by default**. For example, it uses the the open and performant [Delta](https://delta.io/) table format by default. This has many benefits, including letting you use `MERGE` as the the default incremental materialization strategy.
+        - **Support for Unity Catalog**. dbt-databricks>=1.1.1 supports the 3-level namespace of Unity Catalog (catalog / schema / relations) so you can organize and secure your data the way you like.
+        - **Performance**. The adapter generates SQL expressions that are automatically accelerated by the native, vectorized [Photon](https://databricks.com/product/photon) execution engine.
+        
+        ## Choosing between dbt-databricks and dbt-spark
+        If you are developing a dbt project on Databricks, we recommend using `dbt-databricks` for the reasons noted above.
+        
+        `dbt-spark` is an actively developed adapter which works with Databricks as well as Apache Spark anywhere it is hosted e.g. on AWS EMR.
+        
+        ## Getting started
+        
+        ### Installation
+        
+        Install using pip:
+        ```nofmt
+        pip install dbt-databricks
+        ```
+        
+        Upgrade to the latest version
+        ```nofmt
+        pip install --upgrade dbt-databricks
+        ```
+        
+        ### Profile Setup
+        
+        ```nofmt
+        your_profile_name:
+          target: dev
+          outputs:
+            dev:
+              type: databricks
+              catalog: [optional catalog name, if you are using Unity Catalog, only available in dbt-databricks>=1.1.1]
+              schema: [database/schema name]
+              host: [your.databrickshost.com]
+              http_path: [/sql/your/http/path]
+              token: [dapiXXXXXXXXXXXXXXXXXXXXXXX]
+        ```
+        
+        ### Quick Starts
+        
+        These following quick starts will get you up and running with the `dbt-databricks` adapter:
+        - [Developing your first dbt project](https://github.com/databricks/dbt-databricks/blob/main/docs/local-dev.md)
+        - Using dbt Cloud with Databricks ([Azure](https://docs.microsoft.com/en-us/azure/databricks/integrations/prep/dbt-cloud) | [AWS](https://docs.databricks.com/integrations/prep/dbt-cloud.html))
+        - [Running dbt production jobs on Databricks Workflows](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-workflows.md)
+        - [Using Unity Catalog with dbt-databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/uc.md)
+        - [Using GitHub Actions for dbt CI/CD on Databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/github-actions.md)
+        - [Loading data from S3 into Delta using the databricks_copy_into macro](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-copy-into-macro-aws.md)
+        - [Contribute to this repository](CONTRIBUTING.MD)
+        
+        ### Compatibility
+        
+        The `dbt-databricks` adapter has been tested:
+        
+        - with Python 3.7 or above.
+        - against `Databricks SQL` and `Databricks runtime releases 9.1 LTS` and later.
+        
+        ### Tips and Tricks
+        ## Choosing compute for a Python model
+        You can override the compute used for a specific Python model by setting the `http_path` property in model configuration. This can be useful if, for example, you want to run a Python model on an All Purpose cluster, while running SQL models on a SQL Warehouse. Note that this capability is only available for Python models.
+        
+        ```
+        def model(dbt, session):
+            dbt.config(
+              http_path="sql/protocolv1/..."
+            )
+        ```
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-
-<p align="center">
-  <img src="https://bynder-public-us-west-2.s3.amazonaws.com/styleguide/ABB317701CA31CB7F29268E32B303CAE-pdf-column-1.png" alt="databricks logo" width="50%" />
-  <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="250"/>
-</p>
-<p align="center">
-  <a href="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml">
-    <img src="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
-  </a>
-  <a href="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml">
-    <img src="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml/badge.svg?event=push" alt="Integration Tests Badge"/>
-  </a>
-</p>
-
-**[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
-
-The **[Databricks Lakehouse](https://www.databricks.com/)** provides one simple platform to unify all your data, analytics and AI workloads.
-
-# dbt-databricks
-
-The `dbt-databricks` adapter contains all of the code enabling dbt to work with Databricks. This adapter is based off the amazing work done in [dbt-spark](https://github.com/dbt-labs/dbt-spark). Some key features include:
-
-- **Easy setup**. No need to install an ODBC driver as the adapter uses pure Python APIs.
-- **Open by default**. For example, it uses the the open and performant [Delta](https://delta.io/) table format by default. This has many benefits, including letting you use `MERGE` as the the default incremental materialization strategy.
-- **Support for Unity Catalog**. dbt-databricks>=1.1.1 supports the 3-level namespace of Unity Catalog (catalog / schema / relations) so you can organize and secure your data the way you like.
-- **Performance**. The adapter generates SQL expressions that are automatically accelerated by the native, vectorized [Photon](https://databricks.com/product/photon) execution engine.
-
-## Choosing between dbt-databricks and dbt-spark
-If you are developing a dbt project on Databricks, we recommend using `dbt-databricks` for the reasons noted above.
-
-`dbt-spark` is an actively developed adapter which works with Databricks as well as Apache Spark anywhere it is hosted e.g. on AWS EMR.
-
-## Getting started
-
-### Installation
-
-Install using pip:
-```nofmt
-pip install dbt-databricks
-```
-
-Upgrade to the latest version
-```nofmt
-pip install --upgrade dbt-databricks
-```
-
-### Profile Setup
-
-```nofmt
-your_profile_name:
-  target: dev
-  outputs:
-    dev:
-      type: databricks
-      catalog: [optional catalog name, if you are using Unity Catalog, only available in dbt-databricks>=1.1.1]
-      schema: [database/schema name]
-      host: [your.databrickshost.com]
-      http_path: [/sql/your/http/path]
-      token: [dapiXXXXXXXXXXXXXXXXXXXXXXX]
-```
-
-### Quick Starts
-
-These following quick starts will get you up and running with the `dbt-databricks` adapter:
-- [Developing your first dbt project](https://github.com/databricks/dbt-databricks/blob/main/docs/local-dev.md)
-- Using dbt Cloud with Databricks ([Azure](https://docs.microsoft.com/en-us/azure/databricks/integrations/prep/dbt-cloud) | [AWS](https://docs.databricks.com/integrations/prep/dbt-cloud.html))
-- [Running dbt production jobs on Databricks Workflows](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-workflows.md)
-- [Using Unity Catalog with dbt-databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/uc.md)
-- [Using GitHub Actions for dbt CI/CD on Databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/github-actions.md)
-- [Loading data from S3 into Delta using the databricks_copy_into macro](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-copy-into-macro-aws.md)
-- [Contribute to this repository](CONTRIBUTING.MD)
-
-### Compatibility
-
-The `dbt-databricks` adapter has been tested:
-
-- with Python 3.7 or above.
-- against `Databricks SQL` and `Databricks runtime releases 9.1 LTS` and later.
-
-### Tips and Tricks
-## Choosing compute for a Python model
-You can override the compute used for a specific Python model by setting the `http_path` property in model configuration. This can be useful if, for example, you want to run a Python model on an All Purpose cluster, while running SQL models on a SQL Warehouse. Note that this capability is only available for Python models.
-
-```
-def model(dbt, session):
-    dbt.config(
-      http_path="sql/protocolv1/..."
-    )
-```
```

### Comparing `dbt-databricks-1.8.0b1/dbt_databricks.egg-info/SOURCES.txt` & `dbt-databricks-1.8.0b2/dbt_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0b1/setup.py` & `dbt-databricks-1.8.0b2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     long_description_content_type="text/markdown",
     author="Databricks",
     author_email="feedback@databricks.com",
     url="https://github.com/databricks/dbt-databricks",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-spark~=1.7.1",
+        "dbt-spark~=1.8.0b1",
         "databricks-sql-connector>=3.1.0, <3.2.0",
         "databricks-sdk==0.17.0",
         "keyring>=23.13.0",
         "pandas<2.2.0",
     ],
     zip_safe=False,
     classifiers=[
```

