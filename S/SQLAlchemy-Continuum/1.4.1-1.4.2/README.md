# Comparing `tmp/SQLAlchemy-Continuum-1.4.1.tar.gz` & `tmp/sqlalchemy_continuum-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLAlchemy-Continuum-1.4.1.tar", last modified: Thu Mar 14 02:06:48 2024, max compression
+gzip compressed data, was "sqlalchemy_continuum-1.4.2.tar", last modified: Thu May  2 20:03:14 2024, max compression
```

## Comparing `SQLAlchemy-Continuum-1.4.1.tar` & `sqlalchemy_continuum-1.4.2.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.164448 SQLAlchemy-Continuum-1.4.1/
--rw-r--r--   0 root         (0) root         (0)    17882 2024-03-14 01:59:54.000000 SQLAlchemy-Continuum-1.4.1/CHANGES.rst
--rw-r--r--   0 root         (0) root         (0)     1480 2022-01-26 18:31:39.000000 SQLAlchemy-Continuum-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      193 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1843 2024-03-14 02:06:48.164448 SQLAlchemy-Continuum-1.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4029 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.164448 SQLAlchemy-Continuum-1.4.1/SQLAlchemy_Continuum.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1843 2024-03-14 02:06:48.000000 SQLAlchemy-Continuum-1.4.1/SQLAlchemy_Continuum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4108 2024-03-14 02:06:48.000000 SQLAlchemy-Continuum-1.4.1/SQLAlchemy_Continuum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 02:06:48.000000 SQLAlchemy-Continuum-1.4.1/SQLAlchemy_Continuum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 02:06:47.000000 SQLAlchemy-Continuum-1.4.1/SQLAlchemy_Continuum.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      324 2024-03-14 02:06:48.000000 SQLAlchemy-Continuum-1.4.1/SQLAlchemy_Continuum.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-14 02:06:48.000000 SQLAlchemy-Continuum-1.4.1/SQLAlchemy_Continuum.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.134448 SQLAlchemy-Continuum-1.4.1/docs/
--rw-r--r--   0 root         (0) root         (0)     6818 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      830 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/alembic.rst
--rw-r--r--   0 root         (0) root         (0)      757 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/api.rst
--rw-r--r--   0 root         (0) root         (0)     8420 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     5375 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/configuration.rst
--rw-r--r--   0 root         (0) root         (0)      297 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     3468 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/intro.rst
--rw-r--r--   0 root         (0) root         (0)       41 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/license.rst
--rw-r--r--   0 root         (0) root         (0)     6729 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     1223 2022-08-28 14:29:19.000000 SQLAlchemy-Continuum-1.4.1/docs/native_versioning.rst
--rw-r--r--   0 root         (0) root         (0)      801 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/plugins.rst
--rw-r--r--   0 root         (0) root         (0)     1714 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/queries.rst
--rw-r--r--   0 root         (0) root         (0)     2209 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/revert.rst
--rw-r--r--   0 root         (0) root         (0)     1898 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/schema.rst
--rw-r--r--   0 root         (0) root         (0)     1877 2023-06-05 00:09:48.000000 SQLAlchemy-Continuum-1.4.1/docs/transactions.rst
--rw-r--r--   0 root         (0) root         (0)      892 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/docs/utilities.rst
--rw-r--r--   0 root         (0) root         (0)     6020 2023-06-09 21:50:46.000000 SQLAlchemy-Continuum-1.4.1/docs/version_objects.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-14 02:06:48.164448 SQLAlchemy-Continuum-1.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2315 2024-03-14 02:04:45.000000 SQLAlchemy-Continuum-1.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.144448 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/
--rw-r--r--   0 root         (0) root         (0)     3244 2024-03-14 02:05:33.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8541 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.144448 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/dialects/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/dialects/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15473 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/dialects/postgresql.py
--rw-r--r--   0 root         (0) root         (0)      152 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/exc.py
--rw-r--r--   0 root         (0) root         (0)      975 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/expression_reflector.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/factory.py
--rw-r--r--   0 root         (0) root         (0)     5839 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/fetcher.py
--rw-r--r--   0 root         (0) root         (0)    16006 2024-03-14 02:04:45.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/manager.py
--rw-r--r--   0 root         (0) root         (0)     9815 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/model_builder.py
--rw-r--r--   0 root         (0) root         (0)     2680 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/operation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.144448 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/
--rw-r--r--   0 root         (0) root         (0)      322 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10607 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/activity.py
--rw-r--r--   0 root         (0) root         (0)     1866 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/base.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-07-25 00:25:31.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/flask.py
--rw-r--r--   0 root         (0) root         (0)      987 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/null_delete.py
--rw-r--r--   0 root         (0) root         (0)     2487 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/property_mod_tracker.py
--rw-r--r--   0 root         (0) root         (0)     3239 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/transaction_changes.py
--rw-r--r--   0 root         (0) root         (0)     3175 2023-09-12 20:06:49.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/transaction_meta.py
--rw-r--r--   0 root         (0) root         (0)    12703 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/relationship_builder.py
--rw-r--r--   0 root         (0) root         (0)     4464 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/reverter.py
--rw-r--r--   0 root         (0) root         (0)     5681 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/schema.py
--rw-r--r--   0 root         (0) root         (0)     4672 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/table_builder.py
--rw-r--r--   0 root         (0) root         (0)     5800 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/transaction.py
--rw-r--r--   0 root         (0) root         (0)    10939 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/unit_of_work.py
--rw-r--r--   0 root         (0) root         (0)    12249 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/utils.py
--rw-r--r--   0 root         (0) root         (0)     2095 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.154448 SQLAlchemy-Continuum-1.4.1/tests/
--rw-r--r--   0 root         (0) root         (0)     7955 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.154448 SQLAlchemy-Continuum-1.4.1/tests/builders/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/tests/builders/__init__.py
--rw-r--r--   0 root         (0) root         (0)      259 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/tests/builders/test_model_builder.py
--rw-r--r--   0 root         (0) root         (0)     1146 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/builders/test_relationship_builder.py
--rw-r--r--   0 root         (0) root         (0)     3316 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/builders/test_table_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.154448 SQLAlchemy-Continuum-1.4.1/tests/dialects/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/tests/dialects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/dialects/test_triggers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.154448 SQLAlchemy-Continuum-1.4.1/tests/inheritance/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/tests/inheritance/__init__.py
--rw-r--r--   0 root         (0) root         (0)      940 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/inheritance/test_common_base_class.py
--rw-r--r--   0 root         (0) root         (0)     3273 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/inheritance/test_concrete_inheritance.py
--rw-r--r--   0 root         (0) root         (0)     7122 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/inheritance/test_join_table_inheritance.py
--rw-r--r--   0 root         (0) root         (0)     1646 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/inheritance/test_multi_level_inheritance.py
--rw-r--r--   0 root         (0) root         (0)     3308 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/inheritance/test_single_table_inheritance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.154448 SQLAlchemy-Continuum-1.4.1/tests/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:10:37.000000 SQLAlchemy-Continuum-1.4.1/tests/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6895 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/plugins/test_activity.py
--rw-r--r--   0 root         (0) root         (0)     8227 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/plugins/test_flask.py
--rw-r--r--   0 root         (0) root         (0)     1000 2023-06-05 00:10:37.000000 SQLAlchemy-Continuum-1.4.1/tests/plugins/test_null_delete.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-06-05 00:10:37.000000 SQLAlchemy-Continuum-1.4.1/tests/plugins/test_plugin_collection.py
--rw-r--r--   0 root         (0) root         (0)     5947 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/plugins/test_property_mod_tracker.py
--rw-r--r--   0 root         (0) root         (0)     2473 2023-06-05 00:10:37.000000 SQLAlchemy-Continuum-1.4.1/tests/plugins/test_transaction_changes.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/plugins/test_transaction_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.164448 SQLAlchemy-Continuum-1.4.1/tests/relationships/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/tests/relationships/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2336 2022-09-02 22:30:07.000000 SQLAlchemy-Continuum-1.4.1/tests/relationships/test_association_table_relations.py
--rw-r--r--   0 root         (0) root         (0)     2477 2022-09-02 22:30:07.000000 SQLAlchemy-Continuum-1.4.1/tests/relationships/test_custom_condition_relations.py
--rw-r--r--   0 root         (0) root         (0)     3029 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/relationships/test_dynamic_relationships.py
--rw-r--r--   0 root         (0) root         (0)    14738 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/relationships/test_many_to_many_relations.py
--rw-r--r--   0 root         (0) root         (0)     3291 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/relationships/test_non_versioned_classes.py
--rw-r--r--   0 root         (0) root         (0)     9182 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/relationships/test_one_to_many_relations.py
--rw-r--r--   0 root         (0) root         (0)     2882 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/relationships/test_one_to_one_relations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.164448 SQLAlchemy-Continuum-1.4.1/tests/revert/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/tests/revert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2112 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/revert/test_deep_relationships.py
--rw-r--r--   0 root         (0) root         (0)     2806 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/revert/test_many_to_many_relationships.py
--rw-r--r--   0 root         (0) root         (0)     1817 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/revert/test_one_to_one_relationship.py
--rw-r--r--   0 root         (0) root         (0)     2127 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/revert/test_one_to_one_with_secondary_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.164448 SQLAlchemy-Continuum-1.4.1/tests/schema/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/tests/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/schema/test_update_end_transaction_id.py
--rw-r--r--   0 root         (0) root         (0)     2955 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/schema/test_update_property_mod_flags.py
--rw-r--r--   0 root         (0) root         (0)     8343 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_accessors.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_changeset.py
--rw-r--r--   0 root         (0) root         (0)     1935 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.1/tests/test_column_aliases.py
--rw-r--r--   0 root         (0) root         (0)     3661 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.1/tests/test_column_inclusion_and_exclusion.py
--rw-r--r--   0 root         (0) root         (0)      440 2024-03-14 02:04:45.000000 SQLAlchemy-Continuum-1.4.1/tests/test_compatibility.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.1/tests/test_composite_primary_key.py
--rw-r--r--   0 root         (0) root         (0)     3660 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_configuration.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_custom_schema.py
--rw-r--r--   0 root         (0) root         (0)     1114 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.1/tests/test_custom_version_base_class.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.1/tests/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1068 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.1/tests/test_exotic_listener_chaining.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.1/tests/test_exotic_operation_combos.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_i18n.py
--rw-r--r--   0 root         (0) root         (0)     2647 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_insert.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.1/tests/test_mapper_args.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_raw_sql.py
--rw-r--r--   0 root         (0) root         (0)     6000 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.1/tests/test_revert.py
--rw-r--r--   0 root         (0) root         (0)     1505 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_savepoints.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_sessions.py
--rw-r--r--   0 root         (0) root         (0)     2947 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_transaction.py
--rw-r--r--   0 root         (0) root         (0)     3420 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_update.py
--rw-r--r--   0 root         (0) root         (0)     1707 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.1/tests/test_vacuum.py
--rw-r--r--   0 root         (0) root         (0)     3658 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_validity_strategy.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.1/tests/test_validity_strategy_multithreaded.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.1/tests/test_versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 02:06:48.164448 SQLAlchemy-Continuum-1.4.1/tests/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/tests/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      869 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/utils/test_changeset.py
--rw-r--r--   0 root         (0) root         (0)     1079 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/utils/test_count_versions.py
--rw-r--r--   0 root         (0) root         (0)      877 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/utils/test_is_modified.py
--rw-r--r--   0 root         (0) root         (0)      440 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.1/tests/utils/test_parent_class.py
--rw-r--r--   0 root         (0) root         (0)      477 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/utils/test_transaction_class.py
--rw-r--r--   0 root         (0) root         (0)      824 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/utils/test_tx_column_name.py
--rw-r--r--   0 root         (0) root         (0)      887 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.1/tests/utils/test_version_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.797962 sqlalchemy_continuum-1.4.2/
+-rw-r--r--   0 root         (0) root         (0)    17882 2024-03-14 01:59:54.000000 sqlalchemy_continuum-1.4.2/CHANGES.rst
+-rw-r--r--   0 root         (0) root         (0)     1480 2022-01-26 18:31:39.000000 sqlalchemy_continuum-1.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      193 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-05-02 20:03:14.797962 sqlalchemy_continuum-1.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.797962 sqlalchemy_continuum-1.4.2/SQLAlchemy_Continuum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-05-02 20:03:14.000000 sqlalchemy_continuum-1.4.2/SQLAlchemy_Continuum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4108 2024-05-02 20:03:14.000000 sqlalchemy_continuum-1.4.2/SQLAlchemy_Continuum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:03:14.000000 sqlalchemy_continuum-1.4.2/SQLAlchemy_Continuum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:03:14.000000 sqlalchemy_continuum-1.4.2/SQLAlchemy_Continuum.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-02 20:03:14.000000 sqlalchemy_continuum-1.4.2/SQLAlchemy_Continuum.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-02 20:03:14.000000 sqlalchemy_continuum-1.4.2/SQLAlchemy_Continuum.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.717965 sqlalchemy_continuum-1.4.2/docs/
+-rw-r--r--   0 root         (0) root         (0)     6818 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      830 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/alembic.rst
+-rw-r--r--   0 root         (0) root         (0)      757 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/api.rst
+-rw-r--r--   0 root         (0) root         (0)     8420 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     5375 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)      297 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     3468 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/intro.rst
+-rw-r--r--   0 root         (0) root         (0)       41 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/license.rst
+-rw-r--r--   0 root         (0) root         (0)     6729 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     1223 2022-08-28 14:29:19.000000 sqlalchemy_continuum-1.4.2/docs/native_versioning.rst
+-rw-r--r--   0 root         (0) root         (0)      801 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/plugins.rst
+-rw-r--r--   0 root         (0) root         (0)     1714 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/queries.rst
+-rw-r--r--   0 root         (0) root         (0)     2209 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/revert.rst
+-rw-r--r--   0 root         (0) root         (0)     1898 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/schema.rst
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-06-05 00:09:48.000000 sqlalchemy_continuum-1.4.2/docs/transactions.rst
+-rw-r--r--   0 root         (0) root         (0)      892 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/docs/utilities.rst
+-rw-r--r--   0 root         (0) root         (0)     6020 2023-06-09 21:50:46.000000 sqlalchemy_continuum-1.4.2/docs/version_objects.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 20:03:14.797962 sqlalchemy_continuum-1.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-05-02 20:00:10.000000 sqlalchemy_continuum-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.727964 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/
+-rw-r--r--   0 root         (0) root         (0)     3244 2024-05-02 20:00:10.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8541 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.727964 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/dialects/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/dialects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15473 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/dialects/postgresql.py
+-rw-r--r--   0 root         (0) root         (0)      152 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/exc.py
+-rw-r--r--   0 root         (0) root         (0)      975 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/expression_reflector.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/factory.py
+-rw-r--r--   0 root         (0) root         (0)     5839 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/fetcher.py
+-rw-r--r--   0 root         (0) root         (0)    16006 2024-03-14 02:04:45.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9815 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/model_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.737964 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/
+-rw-r--r--   0 root         (0) root         (0)      322 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10607 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/activity.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/base.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-07-25 00:25:31.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/flask.py
+-rw-r--r--   0 root         (0) root         (0)      987 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/null_delete.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/property_mod_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     3239 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/transaction_changes.py
+-rw-r--r--   0 root         (0) root         (0)     3175 2023-09-12 20:06:49.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/transaction_meta.py
+-rw-r--r--   0 root         (0) root         (0)    12703 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/relationship_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4464 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/reverter.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/schema.py
+-rw-r--r--   0 root         (0) root         (0)     4672 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/table_builder.py
+-rw-r--r--   0 root         (0) root         (0)     5800 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/transaction.py
+-rw-r--r--   0 root         (0) root         (0)    10939 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/unit_of_work.py
+-rw-r--r--   0 root         (0) root         (0)    12249 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.747964 sqlalchemy_continuum-1.4.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     7955 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.747964 sqlalchemy_continuum-1.4.2/tests/builders/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/tests/builders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      259 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/tests/builders/test_model_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/builders/test_relationship_builder.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/builders/test_table_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.747964 sqlalchemy_continuum-1.4.2/tests/dialects/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/tests/dialects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/dialects/test_triggers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.747964 sqlalchemy_continuum-1.4.2/tests/inheritance/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/tests/inheritance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      940 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/inheritance/test_common_base_class.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/inheritance/test_concrete_inheritance.py
+-rw-r--r--   0 root         (0) root         (0)     7122 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/inheritance/test_join_table_inheritance.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/inheritance/test_multi_level_inheritance.py
+-rw-r--r--   0 root         (0) root         (0)     3308 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/inheritance/test_single_table_inheritance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.767963 sqlalchemy_continuum-1.4.2/tests/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:10:37.000000 sqlalchemy_continuum-1.4.2/tests/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6895 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/plugins/test_activity.py
+-rw-r--r--   0 root         (0) root         (0)     8227 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/plugins/test_flask.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-06-05 00:10:37.000000 sqlalchemy_continuum-1.4.2/tests/plugins/test_null_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-06-05 00:10:37.000000 sqlalchemy_continuum-1.4.2/tests/plugins/test_plugin_collection.py
+-rw-r--r--   0 root         (0) root         (0)     5947 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/plugins/test_property_mod_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2023-06-05 00:10:37.000000 sqlalchemy_continuum-1.4.2/tests/plugins/test_transaction_changes.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/plugins/test_transaction_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.777963 sqlalchemy_continuum-1.4.2/tests/relationships/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/tests/relationships/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2336 2022-09-02 22:30:07.000000 sqlalchemy_continuum-1.4.2/tests/relationships/test_association_table_relations.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2022-09-02 22:30:07.000000 sqlalchemy_continuum-1.4.2/tests/relationships/test_custom_condition_relations.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/relationships/test_dynamic_relationships.py
+-rw-r--r--   0 root         (0) root         (0)    14738 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/relationships/test_many_to_many_relations.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/relationships/test_non_versioned_classes.py
+-rw-r--r--   0 root         (0) root         (0)     9182 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/relationships/test_one_to_many_relations.py
+-rw-r--r--   0 root         (0) root         (0)     2882 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/relationships/test_one_to_one_relations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.777963 sqlalchemy_continuum-1.4.2/tests/revert/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/tests/revert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/revert/test_deep_relationships.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/revert/test_many_to_many_relationships.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/revert/test_one_to_one_relationship.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/revert/test_one_to_one_with_secondary_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.777963 sqlalchemy_continuum-1.4.2/tests/schema/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/tests/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/schema/test_update_end_transaction_id.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/schema/test_update_property_mod_flags.py
+-rw-r--r--   0 root         (0) root         (0)     8343 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_accessors.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_changeset.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-06-05 00:10:31.000000 sqlalchemy_continuum-1.4.2/tests/test_column_aliases.py
+-rw-r--r--   0 root         (0) root         (0)     3661 2023-06-05 00:10:31.000000 sqlalchemy_continuum-1.4.2/tests/test_column_inclusion_and_exclusion.py
+-rw-r--r--   0 root         (0) root         (0)      440 2024-03-14 02:04:45.000000 sqlalchemy_continuum-1.4.2/tests/test_compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-06-05 00:10:31.000000 sqlalchemy_continuum-1.4.2/tests/test_composite_primary_key.py
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_custom_schema.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-06-05 00:10:31.000000 sqlalchemy_continuum-1.4.2/tests/test_custom_version_base_class.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-06-05 00:10:31.000000 sqlalchemy_continuum-1.4.2/tests/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-06-05 00:10:31.000000 sqlalchemy_continuum-1.4.2/tests/test_exotic_listener_chaining.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-06-05 00:10:31.000000 sqlalchemy_continuum-1.4.2/tests/test_exotic_operation_combos.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_i18n.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_insert.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-06-05 00:10:31.000000 sqlalchemy_continuum-1.4.2/tests/test_mapper_args.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_raw_sql.py
+-rw-r--r--   0 root         (0) root         (0)     6000 2023-06-05 00:10:31.000000 sqlalchemy_continuum-1.4.2/tests/test_revert.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_savepoints.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_sessions.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_transaction.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_update.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-06-05 00:10:31.000000 sqlalchemy_continuum-1.4.2/tests/test_vacuum.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_validity_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-07-12 17:09:37.000000 sqlalchemy_continuum-1.4.2/tests/test_validity_strategy_multithreaded.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-05 00:10:31.000000 sqlalchemy_continuum-1.4.2/tests/test_versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:03:14.797962 sqlalchemy_continuum-1.4.2/tests/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/tests/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      869 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/utils/test_changeset.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/utils/test_count_versions.py
+-rw-r--r--   0 root         (0) root         (0)      877 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/utils/test_is_modified.py
+-rw-r--r--   0 root         (0) root         (0)      440 2022-01-01 15:24:43.000000 sqlalchemy_continuum-1.4.2/tests/utils/test_parent_class.py
+-rw-r--r--   0 root         (0) root         (0)      477 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/utils/test_transaction_class.py
+-rw-r--r--   0 root         (0) root         (0)      824 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/utils/test_tx_column_name.py
+-rw-r--r--   0 root         (0) root         (0)      887 2022-08-28 14:42:37.000000 sqlalchemy_continuum-1.4.2/tests/utils/test_version_class.py
```

### Comparing `SQLAlchemy-Continuum-1.4.1/CHANGES.rst` & `sqlalchemy_continuum-1.4.2/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/LICENSE` & `sqlalchemy_continuum-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/PKG-INFO` & `sqlalchemy_continuum-1.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemy-Continuum
-Version: 1.4.1
+Version: 1.4.2
 Summary: Versioning and auditing extension for SQLAlchemy.
 Home-page: https://github.com/kvesteri/sqlalchemy-continuum
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
 Platform: any
 Classifier: Environment :: Web Environment
@@ -17,16 +17,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
-Requires-Dist: SQLAlchemy<=2.0.21,>=1.4.0
-Requires-Dist: SQLAlchemy-Utils>=0.30.12
+Requires-Dist: SQLAlchemy>=1.4.0
+Requires-Dist: SQLAlchemy-Utils>=0.41.2
 Provides-Extra: test
 Requires-Dist: pytest>=2.3.5; extra == "test"
 Requires-Dist: psycopg2>=2.4.6; extra == "test"
 Requires-Dist: PyMySQL>=0.8.0; extra == "test"
 Requires-Dist: Flask>=0.9; extra == "test"
 Requires-Dist: Flask-Login>=0.2.9; extra == "test"
 Requires-Dist: Flask-SQLAlchemy>=1.0; extra == "test"
```

### Comparing `SQLAlchemy-Continuum-1.4.1/README.rst` & `sqlalchemy_continuum-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/SQLAlchemy_Continuum.egg-info/PKG-INFO` & `sqlalchemy_continuum-1.4.2/SQLAlchemy_Continuum.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemy-Continuum
-Version: 1.4.1
+Version: 1.4.2
 Summary: Versioning and auditing extension for SQLAlchemy.
 Home-page: https://github.com/kvesteri/sqlalchemy-continuum
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
 Platform: any
 Classifier: Environment :: Web Environment
@@ -17,16 +17,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
-Requires-Dist: SQLAlchemy<=2.0.21,>=1.4.0
-Requires-Dist: SQLAlchemy-Utils>=0.30.12
+Requires-Dist: SQLAlchemy>=1.4.0
+Requires-Dist: SQLAlchemy-Utils>=0.41.2
 Provides-Extra: test
 Requires-Dist: pytest>=2.3.5; extra == "test"
 Requires-Dist: psycopg2>=2.4.6; extra == "test"
 Requires-Dist: PyMySQL>=0.8.0; extra == "test"
 Requires-Dist: Flask>=0.9; extra == "test"
 Requires-Dist: Flask-Login>=0.2.9; extra == "test"
 Requires-Dist: Flask-SQLAlchemy>=1.0; extra == "test"
```

### Comparing `SQLAlchemy-Continuum-1.4.1/SQLAlchemy_Continuum.egg-info/SOURCES.txt` & `sqlalchemy_continuum-1.4.2/SQLAlchemy_Continuum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/Makefile` & `sqlalchemy_continuum-1.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/alembic.rst` & `sqlalchemy_continuum-1.4.2/docs/alembic.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/api.rst` & `sqlalchemy_continuum-1.4.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/conf.py` & `sqlalchemy_continuum-1.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/configuration.rst` & `sqlalchemy_continuum-1.4.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/intro.rst` & `sqlalchemy_continuum-1.4.2/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/make.bat` & `sqlalchemy_continuum-1.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/native_versioning.rst` & `sqlalchemy_continuum-1.4.2/docs/native_versioning.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/plugins.rst` & `sqlalchemy_continuum-1.4.2/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/queries.rst` & `sqlalchemy_continuum-1.4.2/docs/queries.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/revert.rst` & `sqlalchemy_continuum-1.4.2/docs/revert.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/schema.rst` & `sqlalchemy_continuum-1.4.2/docs/schema.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/transactions.rst` & `sqlalchemy_continuum-1.4.2/docs/transactions.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/utilities.rst` & `sqlalchemy_continuum-1.4.2/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/docs/version_objects.rst` & `sqlalchemy_continuum-1.4.2/docs/version_objects.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/setup.py` & `sqlalchemy_continuum-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,16 +56,16 @@
         'sqlalchemy_continuum.plugins',
         'sqlalchemy_continuum.dialects'
     ],
     zip_safe=False,
     include_package_data=True,
     platforms='any',
     install_requires=[
-        'SQLAlchemy>=1.4.0,<=2.0.21',
-        'SQLAlchemy-Utils>=0.30.12',
+        'SQLAlchemy>=1.4.0',
+        'SQLAlchemy-Utils>=0.41.2',
     ],
     extras_require=extras_require,
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
```

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/__init__.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     transaction_class,
     tx_column_name,
     vacuum,
     version_class,
 )
 
 
-__version__ = '1.4.1'
+__version__ = '1.4.2'
 
 
 versioning_manager = VersioningManager()
 
 
 def make_versioned(
     mapper=sa.orm.Mapper,
```

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/builder.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/dialects/postgresql.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/dialects/postgresql.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/expression_reflector.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/expression_reflector.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/fetcher.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/fetcher.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/manager.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/manager.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/model_builder.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/model_builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/operation.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/operation.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/activity.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/activity.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/base.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/base.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/flask.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/flask.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/null_delete.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/null_delete.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/property_mod_tracker.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/property_mod_tracker.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/transaction_changes.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/transaction_changes.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/plugins/transaction_meta.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/plugins/transaction_meta.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/relationship_builder.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/relationship_builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/reverter.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/reverter.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/schema.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/schema.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/table_builder.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/table_builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/transaction.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/transaction.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/unit_of_work.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/utils.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/utils.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/sqlalchemy_continuum/version.py` & `sqlalchemy_continuum-1.4.2/sqlalchemy_continuum/version.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/__init__.py` & `sqlalchemy_continuum-1.4.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/builders/test_relationship_builder.py` & `sqlalchemy_continuum-1.4.2/tests/builders/test_relationship_builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/builders/test_table_builder.py` & `sqlalchemy_continuum-1.4.2/tests/builders/test_table_builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/dialects/test_triggers.py` & `sqlalchemy_continuum-1.4.2/tests/dialects/test_triggers.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/inheritance/test_common_base_class.py` & `sqlalchemy_continuum-1.4.2/tests/inheritance/test_common_base_class.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/inheritance/test_concrete_inheritance.py` & `sqlalchemy_continuum-1.4.2/tests/inheritance/test_concrete_inheritance.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/inheritance/test_join_table_inheritance.py` & `sqlalchemy_continuum-1.4.2/tests/inheritance/test_join_table_inheritance.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/inheritance/test_multi_level_inheritance.py` & `sqlalchemy_continuum-1.4.2/tests/inheritance/test_multi_level_inheritance.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/inheritance/test_single_table_inheritance.py` & `sqlalchemy_continuum-1.4.2/tests/inheritance/test_single_table_inheritance.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/plugins/test_activity.py` & `sqlalchemy_continuum-1.4.2/tests/plugins/test_activity.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/plugins/test_flask.py` & `sqlalchemy_continuum-1.4.2/tests/plugins/test_flask.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/plugins/test_null_delete.py` & `sqlalchemy_continuum-1.4.2/tests/plugins/test_null_delete.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/plugins/test_plugin_collection.py` & `sqlalchemy_continuum-1.4.2/tests/plugins/test_plugin_collection.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/plugins/test_property_mod_tracker.py` & `sqlalchemy_continuum-1.4.2/tests/plugins/test_property_mod_tracker.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/plugins/test_transaction_changes.py` & `sqlalchemy_continuum-1.4.2/tests/plugins/test_transaction_changes.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/plugins/test_transaction_meta.py` & `sqlalchemy_continuum-1.4.2/tests/plugins/test_transaction_meta.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/relationships/test_association_table_relations.py` & `sqlalchemy_continuum-1.4.2/tests/relationships/test_association_table_relations.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/relationships/test_custom_condition_relations.py` & `sqlalchemy_continuum-1.4.2/tests/relationships/test_custom_condition_relations.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/relationships/test_dynamic_relationships.py` & `sqlalchemy_continuum-1.4.2/tests/relationships/test_dynamic_relationships.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/relationships/test_many_to_many_relations.py` & `sqlalchemy_continuum-1.4.2/tests/relationships/test_many_to_many_relations.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/relationships/test_non_versioned_classes.py` & `sqlalchemy_continuum-1.4.2/tests/relationships/test_non_versioned_classes.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/relationships/test_one_to_many_relations.py` & `sqlalchemy_continuum-1.4.2/tests/relationships/test_one_to_many_relations.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/relationships/test_one_to_one_relations.py` & `sqlalchemy_continuum-1.4.2/tests/relationships/test_one_to_one_relations.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/revert/test_deep_relationships.py` & `sqlalchemy_continuum-1.4.2/tests/revert/test_deep_relationships.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/revert/test_many_to_many_relationships.py` & `sqlalchemy_continuum-1.4.2/tests/revert/test_many_to_many_relationships.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/revert/test_one_to_one_relationship.py` & `sqlalchemy_continuum-1.4.2/tests/revert/test_one_to_one_relationship.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/revert/test_one_to_one_with_secondary_table.py` & `sqlalchemy_continuum-1.4.2/tests/revert/test_one_to_one_with_secondary_table.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/schema/test_update_end_transaction_id.py` & `sqlalchemy_continuum-1.4.2/tests/schema/test_update_end_transaction_id.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/schema/test_update_property_mod_flags.py` & `sqlalchemy_continuum-1.4.2/tests/schema/test_update_property_mod_flags.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_accessors.py` & `sqlalchemy_continuum-1.4.2/tests/test_accessors.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_changeset.py` & `sqlalchemy_continuum-1.4.2/tests/test_changeset.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_column_aliases.py` & `sqlalchemy_continuum-1.4.2/tests/test_column_aliases.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_column_inclusion_and_exclusion.py` & `sqlalchemy_continuum-1.4.2/tests/test_column_inclusion_and_exclusion.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_composite_primary_key.py` & `sqlalchemy_continuum-1.4.2/tests/test_composite_primary_key.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_configuration.py` & `sqlalchemy_continuum-1.4.2/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_custom_schema.py` & `sqlalchemy_continuum-1.4.2/tests/test_custom_schema.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_custom_version_base_class.py` & `sqlalchemy_continuum-1.4.2/tests/test_custom_version_base_class.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_delete.py` & `sqlalchemy_continuum-1.4.2/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_exotic_listener_chaining.py` & `sqlalchemy_continuum-1.4.2/tests/test_exotic_listener_chaining.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_exotic_operation_combos.py` & `sqlalchemy_continuum-1.4.2/tests/test_exotic_operation_combos.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_i18n.py` & `sqlalchemy_continuum-1.4.2/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_insert.py` & `sqlalchemy_continuum-1.4.2/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_mapper_args.py` & `sqlalchemy_continuum-1.4.2/tests/test_mapper_args.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_raw_sql.py` & `sqlalchemy_continuum-1.4.2/tests/test_raw_sql.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_revert.py` & `sqlalchemy_continuum-1.4.2/tests/test_revert.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_savepoints.py` & `sqlalchemy_continuum-1.4.2/tests/test_savepoints.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_sessions.py` & `sqlalchemy_continuum-1.4.2/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_transaction.py` & `sqlalchemy_continuum-1.4.2/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_update.py` & `sqlalchemy_continuum-1.4.2/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_vacuum.py` & `sqlalchemy_continuum-1.4.2/tests/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_validity_strategy.py` & `sqlalchemy_continuum-1.4.2/tests/test_validity_strategy.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_validity_strategy_multithreaded.py` & `sqlalchemy_continuum-1.4.2/tests/test_validity_strategy_multithreaded.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/test_versions.py` & `sqlalchemy_continuum-1.4.2/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/utils/test_changeset.py` & `sqlalchemy_continuum-1.4.2/tests/utils/test_changeset.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/utils/test_count_versions.py` & `sqlalchemy_continuum-1.4.2/tests/utils/test_count_versions.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/utils/test_is_modified.py` & `sqlalchemy_continuum-1.4.2/tests/utils/test_is_modified.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/utils/test_tx_column_name.py` & `sqlalchemy_continuum-1.4.2/tests/utils/test_tx_column_name.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.4.1/tests/utils/test_version_class.py` & `sqlalchemy_continuum-1.4.2/tests/utils/test_version_class.py`

 * *Files identical despite different names*

