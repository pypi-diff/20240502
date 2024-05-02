# Comparing `tmp/digitalhub_core-0.4.0b2.tar.gz` & `tmp/digitalhub_core-0.4.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_core-0.4.0b2.tar", last modified: Wed Apr 24 07:50:41 2024, max compression
+gzip compressed data, was "digitalhub_core-0.4.0b3.tar", last modified: Thu May  2 13:37:20 2024, max compression
```

## Comparing `digitalhub_core-0.4.0b2.tar` & `digitalhub_core-0.4.0b3.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.826710 digitalhub_core-0.4.0b2/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.4.0b2/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-04-24 07:50:41.826710 digitalhub_core-0.4.0b2/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      499 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.810709 digitalhub_core-0.4.0b2/digitalhub_core/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.810709 digitalhub_core-0.4.0b2/digitalhub_core/client/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/client/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2352 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/client/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.810709 digitalhub_core-0.4.0b2/digitalhub_core/client/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.4.0b2/digitalhub_core/client/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1166 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/client/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8684 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/client/objects/dhcore.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15648 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/client/objects/local.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.814709 digitalhub_core-0.4.0b2/digitalhub_core/context/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/context/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.4.0b2/digitalhub_core/context/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2926 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/context/context.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.814709 digitalhub_core-0.4.0b2/digitalhub_core/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.814709 digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2982 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2485 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1567 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.814709 digitalhub_core-0.4.0b2/digitalhub_core/entities/_builders/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/_builders/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1801 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/_builders/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1442 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/_builders/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1755 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/_builders/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.814709 digitalhub_core-0.4.0b2/digitalhub_core/entities/artifacts/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/artifacts/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6563 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/artifacts/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    13509 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/artifacts/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/artifacts/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/artifacts/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/artifacts/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.814709 digitalhub_core-0.4.0b2/digitalhub_core/entities/functions/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/functions/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6220 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/functions/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16136 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/functions/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/functions/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/functions/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/functions/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.818709 digitalhub_core-0.4.0b2/digitalhub_core/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8627 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    21748 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/projects/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/projects/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1894 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.818709 digitalhub_core-0.4.0b2/digitalhub_core/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4819 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/runs/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14144 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/runs/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/runs/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3620 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2692 2024-03-20 12:21:43.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.818709 digitalhub_core-0.4.0b2/digitalhub_core/entities/secrets/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/secrets/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6082 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/secrets/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8227 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/secrets/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/secrets/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/secrets/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/secrets/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.818709 digitalhub_core-0.4.0b2/digitalhub_core/entities/services/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:49:32.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/services/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6043 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/services/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6884 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/services/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/services/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      368 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/services/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:37.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/services/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.822709 digitalhub_core-0.4.0b2/digitalhub_core/entities/tasks/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/tasks/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5472 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/tasks/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10135 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/tasks/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/tasks/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/tasks/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/tasks/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/tasks/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.822709 digitalhub_core-0.4.0b2/digitalhub_core/entities/workflows/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/workflows/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6280 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/workflows/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15395 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/workflows/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/workflows/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/workflows/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.4.0b2/digitalhub_core/entities/workflows/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.822709 digitalhub_core-0.4.0b2/digitalhub_core/registry/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/registry/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2543 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/registry/import_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1468 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/registry/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1866 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/registry/registry.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.822709 digitalhub_core-0.4.0b2/digitalhub_core/runtimes/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/runtimes/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3931 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/runtimes/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1012 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/runtimes/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.822709 digitalhub_core-0.4.0b2/digitalhub_core/stores/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/stores/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-04-19 08:14:48.000000 digitalhub_core-0.4.0b2/digitalhub_core/stores/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.822709 digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/local.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/remote.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/s3.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/sql.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.826710 digitalhub_core-0.4.0b2/digitalhub_core/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b2/digitalhub_core/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.4.0b2/digitalhub_core/utils/api.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/utils/env_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.4.0b2/digitalhub_core/utils/exceptions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.4.0b2/digitalhub_core/utils/file_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4237 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/utils/generic_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3054 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/utils/git_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.4.0b2/digitalhub_core/utils/io_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.4.0b2/digitalhub_core/utils/logger.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b2/digitalhub_core/utils/uri_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:41.826710 digitalhub_core-0.4.0b2/digitalhub_core.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-04-24 07:50:41.000000 digitalhub_core-0.4.0b2/digitalhub_core.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4131 2024-04-24 07:50:41.000000 digitalhub_core-0.4.0b2/digitalhub_core.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-24 07:50:41.000000 digitalhub_core-0.4.0b2/digitalhub_core.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-04-24 07:50:41.000000 digitalhub_core-0.4.0b2/digitalhub_core.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-24 07:50:41.000000 digitalhub_core-0.4.0b2/digitalhub_core.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1731 2024-04-23 13:34:39.000000 digitalhub_core-0.4.0b2/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-24 07:50:41.826710 digitalhub_core-0.4.0b2/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.181095 digitalhub_core-0.4.0b3/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.4.0b3/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-02 13:37:20.181095 digitalhub_core-0.4.0b3/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      499 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.165095 digitalhub_core-0.4.0b3/digitalhub_core/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-05-02 13:22:47.000000 digitalhub_core-0.4.0b3/digitalhub_core/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.165095 digitalhub_core-0.4.0b3/digitalhub_core/client/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/client/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2352 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/client/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.165095 digitalhub_core-0.4.0b3/digitalhub_core/client/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.4.0b3/digitalhub_core/client/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1166 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/client/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8892 2024-05-02 13:03:59.000000 digitalhub_core-0.4.0b3/digitalhub_core/client/objects/dhcore.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15662 2024-04-24 12:58:10.000000 digitalhub_core-0.4.0b3/digitalhub_core/client/objects/local.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.169095 digitalhub_core-0.4.0b3/digitalhub_core/context/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/context/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.4.0b3/digitalhub_core/context/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2926 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/context/context.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.169095 digitalhub_core-0.4.0b3/digitalhub_core/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.169095 digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3172 2024-05-02 12:54:20.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2485 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1567 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.169095 digitalhub_core-0.4.0b3/digitalhub_core/entities/_builders/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/_builders/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1801 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/_builders/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1442 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/_builders/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1755 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/_builders/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.169095 digitalhub_core-0.4.0b3/digitalhub_core/entities/artifacts/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/artifacts/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6563 2024-05-02 13:22:47.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/artifacts/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    13877 2024-05-02 13:22:47.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/artifacts/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/artifacts/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/artifacts/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/artifacts/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.169095 digitalhub_core-0.4.0b3/digitalhub_core/entities/functions/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/functions/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6220 2024-05-02 13:22:48.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/functions/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16504 2024-05-02 13:22:48.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/functions/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/functions/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/functions/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/functions/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.173095 digitalhub_core-0.4.0b3/digitalhub_core/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8627 2024-05-02 13:22:48.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    21749 2024-05-02 13:22:48.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/projects/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/projects/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1894 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.173095 digitalhub_core-0.4.0b3/digitalhub_core/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4819 2024-05-02 13:22:47.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/runs/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14158 2024-05-02 13:22:48.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/runs/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/runs/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3620 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2692 2024-03-20 12:21:43.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.173095 digitalhub_core-0.4.0b3/digitalhub_core/entities/secrets/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/secrets/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6082 2024-05-02 13:22:47.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/secrets/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8589 2024-05-02 13:22:47.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/secrets/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/secrets/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/secrets/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/secrets/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.173095 digitalhub_core-0.4.0b3/digitalhub_core/entities/services/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:49:32.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/services/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6043 2024-05-02 13:22:47.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/services/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7249 2024-05-02 13:22:48.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/services/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/services/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      368 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/services/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:37.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/services/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.173095 digitalhub_core-0.4.0b3/digitalhub_core/entities/tasks/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/tasks/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5472 2024-05-02 13:22:47.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/tasks/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10491 2024-05-02 13:22:48.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/tasks/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/tasks/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/tasks/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/tasks/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/tasks/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.177095 digitalhub_core-0.4.0b3/digitalhub_core/entities/workflows/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/workflows/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6280 2024-05-02 13:22:48.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/workflows/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15763 2024-05-02 13:22:48.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/workflows/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/workflows/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/workflows/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.4.0b3/digitalhub_core/entities/workflows/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.177095 digitalhub_core-0.4.0b3/digitalhub_core/registry/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/registry/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2543 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/registry/import_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1468 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/registry/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1866 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/registry/registry.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.177095 digitalhub_core-0.4.0b3/digitalhub_core/runtimes/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/runtimes/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3931 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/runtimes/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1012 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/runtimes/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.177095 digitalhub_core-0.4.0b3/digitalhub_core/stores/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/stores/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-05-02 13:22:48.000000 digitalhub_core-0.4.0b3/digitalhub_core/stores/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.177095 digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/local.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/remote.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/s3.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/sql.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.177095 digitalhub_core-0.4.0b3/digitalhub_core/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b3/digitalhub_core/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.4.0b3/digitalhub_core/utils/api.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/utils/env_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.4.0b3/digitalhub_core/utils/exceptions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.4.0b3/digitalhub_core/utils/file_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4237 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/utils/generic_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3054 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/utils/git_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.4.0b3/digitalhub_core/utils/io_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.4.0b3/digitalhub_core/utils/logger.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b3/digitalhub_core/utils/uri_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:37:20.177095 digitalhub_core-0.4.0b3/digitalhub_core.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-02 13:37:20.000000 digitalhub_core-0.4.0b3/digitalhub_core.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4131 2024-05-02 13:37:20.000000 digitalhub_core-0.4.0b3/digitalhub_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-02 13:37:20.000000 digitalhub_core-0.4.0b3/digitalhub_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-05-02 13:37:20.000000 digitalhub_core-0.4.0b3/digitalhub_core.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-02 13:37:20.000000 digitalhub_core-0.4.0b3/digitalhub_core.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1731 2024-05-02 08:14:16.000000 digitalhub_core-0.4.0b3/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-02 13:37:20.181095 digitalhub_core-0.4.0b3/setup.cfg
```

### Comparing `digitalhub_core-0.4.0b2/LICENSE.txt` & `digitalhub_core-0.4.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/PKG-INFO` & `digitalhub_core-0.4.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.4.0b2
+Version: 0.4.0b3
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/__init__.py` & `digitalhub_core-0.4.0b3/digitalhub_core/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/client/builder.py` & `digitalhub_core-0.4.0b3/digitalhub_core/client/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/client/objects/base.py` & `digitalhub_core-0.4.0b3/digitalhub_core/client/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/client/objects/dhcore.py` & `digitalhub_core-0.4.0b3/digitalhub_core/client/objects/dhcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 
 from digitalhub_core.client.objects.base import Client
 from digitalhub_core.utils.exceptions import BackendError
 from pydantic import BaseModel
 from requests import request
-from requests.exceptions import RequestException, Timeout
+from requests.exceptions import JSONDecodeError, RequestException, Timeout
 
 
 class AuthConfig(BaseModel):
     """Client configuration model."""
 
     user: str = None
     """Username."""
@@ -214,14 +214,18 @@
             response.raise_for_status()
             return response.json()
         except RequestException as e:
             if isinstance(e, Timeout):
                 msg = "Request to DHCore backend timed out."
             elif isinstance(e, ConnectionError):
                 msg = "Unable to connect to DHCore backend."
+            elif isinstance(e, JSONDecodeError):
+                if call_type == "DELETE":
+                    return {}
+                msg = "Unable to parse response from DHCore backend."
             else:
                 msg = f"Backend error: {e}"
             raise BackendError(msg) from e
         except Exception as e:
             msg = f"Some error occurred: {e}"
             raise RuntimeError(msg) from e
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/client/objects/local.py` & `digitalhub_core-0.4.0b3/digitalhub_core/client/objects/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,16 +450,16 @@
     ########################
     # Utils
     ########################
 
     @staticmethod
     def _format_msg(
         error_code: int,
-        entity_type: str = None,
-        entity_id: str = None,
+        entity_type: str | None = None,
+        entity_id: str | None = None,
     ) -> str:
         """
         Format a message.
 
         Parameters
         ----------
         error_code : int
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/context/builder.py` & `digitalhub_core-0.4.0b3/digitalhub_core/context/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/context/context.py` & `digitalhub_core-0.4.0b3/digitalhub_core/context/context.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/base.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/entity.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,25 @@
 
     @abstractmethod
     def save(self, update: bool = False) -> Entity:
         """
         Abstract save method.
         """
 
+    @abstractmethod
+    def refresh(self) -> Entity:
+        """
+        Refresh object from backend.
+
+        Returns
+        -------
+        Entity
+            Entity object.
+        """
+
     def _update_attributes(self, obj: dict) -> None:
         """
         Update attributes.
 
         Parameters
         ----------
         obj : dict
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/metadata.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/spec.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/_base/status.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/_base/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/_builders/metadata.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/_builders/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/_builders/spec.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/_builders/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/_builders/status.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/_builders/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/artifacts/crud.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/artifacts/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/artifacts/entity.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/artifacts/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
 from digitalhub_core.stores.builder import get_store
-from digitalhub_core.utils.api import api_ctx_create, api_ctx_update
+from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.exceptions import EntityError
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 from digitalhub_core.utils.uri_utils import map_uri_scheme
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
@@ -79,15 +79,15 @@
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
     #############################
-    #  Save / Export
+    #  Save / Refresh / Export
     #############################
 
     def save(self, update: bool = False) -> Artifact:
         """
         Save entity into backend.
 
         Parameters
@@ -110,14 +110,28 @@
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "artifacts", self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
+    def refresh(self) -> Artifact:
+        """
+        Refresh object from backend.
+
+        Returns
+        -------
+        Artifact
+            Entity refreshed.
+        """
+        api = api_ctx_read(self.project, "artifacts", self.id)
+        obj = self._context().read_object(api)
+        self._update_attributes(obj)
+        return self
+
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
         filename : str
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/artifacts/spec.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/artifacts/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/functions/crud.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/functions/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/functions/entity.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/functions/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
 from digitalhub_core.entities.tasks.crud import create_task, create_task_from_dict, delete_task, new_task
-from digitalhub_core.utils.api import api_ctx_create, api_ctx_list, api_ctx_update
+from digitalhub_core.utils.api import api_ctx_create, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.exceptions import BackendError, EntityError
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
     from digitalhub_core.entities.functions.metadata import FunctionMetadata
@@ -79,15 +79,15 @@
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
         # Initialize tasks
         self._tasks: dict[str, Task] = {}
 
     #############################
-    #  Save / Export
+    #  Save / Refresh / Export
     #############################
 
     def save(self, update: bool = False) -> Function:
         """
         Save entity into backend.
 
         Parameters
@@ -110,14 +110,28 @@
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "functions", self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
+    def refresh(self) -> Function:
+        """
+        Refresh object from backend.
+
+        Returns
+        -------
+        Function
+            Entity refreshed.
+        """
+        api = api_ctx_read(self.project, "functions", self.id)
+        obj = self._context().read_object(api)
+        self._update_attributes(obj)
+        return self
+
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
         filename : str
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/functions/spec.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/functions/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/projects/crud.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/projects/entity.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/projects/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         # Set client
         self._client = get_client(local)
 
         # Set context
         set_context(self)
 
     #############################
-    #  Save / Export
+    #  Save / Refresh / Export
     #############################
 
     def save(self, update: bool = False) -> Project:
         """
         Save entity into backend.
 
         Parameters
@@ -131,19 +131,15 @@
             If True, the object will be updated.
 
         Returns
         -------
         Project
             Entity saved.
         """
-        # Try to refresh project if local client
-        if self._client.is_local():
-            obj = self._refresh().to_dict()
-        else:
-            obj = self.to_dict()
+        obj = self._refresh_to_dict()
 
         if not update:
             api = api_base_create("projects")
             new_obj = self._client.create_object(api, obj)
             new_obj["local"] = self._client.is_local()
             self._update_attributes(new_obj)
             return self
@@ -151,33 +147,43 @@
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_base_update("projects", self.id)
         new_obj = self._client.update_object(api, obj)
         new_obj["local"] = self._client.is_local()
         self._update_attributes(new_obj)
         return self
 
+    def refresh(self) -> Project:
+        """
+        Refresh object from backend.
+
+        Returns
+        -------
+        Project
+            Project object.
+        """
+        api = api_base_read("projects", self.name)
+        obj = self._client.read_object(api)
+        self._update_attributes(obj)
+        return self
+
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file. If the objects are not embedded, the objects are
         exported as a YAML file.
 
         Parameters
         ----------
         filename : str
             Name of the export YAML file. If not specified, the default value is used.
 
         Returns
         -------
         None
         """
-        # Try to refresh project if local client
-        if self._client.is_local():
-            obj = self._refresh().to_dict()
-        else:
-            obj = self.to_dict()
+        obj = self._refresh_to_dict()
 
         if filename is None:
             filename = f"{self.kind}_{self.name}.yml"
         pth = Path(self.spec.context) / filename
         pth.parent.mkdir(parents=True, exist_ok=True)
         write_yaml(pth, obj)
 
@@ -186,29 +192,27 @@
             for entity in self._get_objects(entity_type):
                 api = api_ctx_read(self.name, entity_type, entity["id"])
                 obj = self._client.read_object(api)
                 ctx_obj = FUNC_MAP[entity_type](obj)
                 if not ctx_obj.metadata.embedded:
                     ctx_obj.export()
 
-    def _refresh(self) -> "Project":
+    def _refresh_to_dict(self) -> dict:
         """
-        Refresh object from backend.
+        Try to refresh object to collect entities related to project.
 
         Returns
         -------
-        Project
-            Project object.
+        dict
+            Entity object in dictionary format.
         """
         try:
-            api = api_base_read("projects", self.name)
-            obj = self._client.read_object(api)
-            return self.from_dict(obj, validate=False)
+            self.refresh().to_dict()
         except BackendError:
-            return self
+            return self.to_dict()
 
     #############################
     #  Generic operations for objects
     #############################
 
     def _add_object(self, obj: Entity, entity_type: str) -> None:
         """
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/projects/spec.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/registries.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/runs/crud.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/runs/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/runs/entity.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/runs/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "id", "key"])
 
     #############################
-    #  Save / Export
+    #  Save / Refresh / Export
     #############################
 
     def save(self, update: bool = False) -> Run:
         """
         Save entity into backend.
 
         Parameters
@@ -256,15 +256,15 @@
         """
         value_list = getattr(self.spec, "values", [])
         value_list = value_list if value_list is not None else []
         return self.status.get_values(value_list)
 
     def refresh(self) -> Run:
         """
-        Get object from backend.
+        Refresh object from backend.
 
         Returns
         -------
         Run
             Run object.
         """
         api = api_ctx_read(self.project, "runs", self.id)
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/runs/spec.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/runs/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/runs/status.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/runs/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/secrets/crud.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/secrets/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/secrets/entity.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/secrets/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
-from digitalhub_core.utils.api import api_ctx_create, api_ctx_list, api_ctx_update
+from digitalhub_core.utils.api import api_ctx_create, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
     from digitalhub_core.entities.secrets.metadata import SecretMetadata
     from digitalhub_core.entities.secrets.spec import SecretSpec
@@ -71,15 +71,15 @@
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
     #############################
-    #  Save / Export
+    #  Save / Refresh / Export
     #############################
 
     def save(self, update: bool = False) -> Secret:
         """
         Save entity into backend.
 
         Parameters
@@ -102,14 +102,28 @@
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "secrets", self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
+    def refresh(self) -> Secret:
+        """
+        Refresh object from backend.
+
+        Returns
+        -------
+        Secret
+            Entity refreshed.
+        """
+        api = api_ctx_read(self.project, "secrets", self.id)
+        obj = self._context().read_object(api)
+        self._update_attributes(obj)
+        return self
+
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
         filename : str
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/secrets/spec.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/secrets/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/services/crud.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/services/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/services/entity.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/services/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
-from digitalhub_core.utils.api import api_ctx_create, api_ctx_update
+from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
     from digitalhub_core.entities.services.metadata import ServiceMetadata
     from digitalhub_core.entities.services.spec import ServiceSpec
@@ -71,15 +71,15 @@
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
     #############################
-    #  Save / Export
+    #  Save / Refresh / Export
     #############################
 
     def save(self, update: bool = False) -> Service:
         """
         Save entity into backend.
 
         Parameters
@@ -102,14 +102,28 @@
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "services", self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
+    def refresh(self) -> Service:
+        """
+        Refresh object from backend.
+
+        Returns
+        -------
+        Service
+            Entity refreshed.
+        """
+        api = api_ctx_read(self.project, "services", self.id)
+        obj = self._context().read_object(api)
+        self._update_attributes(obj)
+        return self
+
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
         filename : str
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/tasks/crud.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/tasks/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/tasks/entity.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/tasks/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
 from digitalhub_core.entities.runs.crud import delete_run, get_run, new_run, run_from_parameters
-from digitalhub_core.utils.api import api_ctx_create, api_ctx_update
+from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
     from digitalhub_core.entities.runs.entity import Run
     from digitalhub_core.entities.tasks.metadata import TaskMetadata
@@ -69,15 +69,15 @@
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "id", "key"])
 
     #############################
-    #  Save / Export
+    #  Save / Refresh / Export
     #############################
 
     def save(self, update: bool = False) -> Task:
         """
         Save entity into backend.
 
         Parameters
@@ -100,14 +100,28 @@
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "tasks", self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
+    def refresh(self) -> Task:
+        """
+        Refresh object from backend.
+
+        Returns
+        -------
+        Task
+            Entity refreshed.
+        """
+        api = api_ctx_read(self.project, "tasks", self.id)
+        obj = self._context().read_object(api)
+        self._update_attributes(obj)
+        return self
+
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
         filename : str
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/tasks/models.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/tasks/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/workflows/crud.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/workflows/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/entities/workflows/entity.py` & `digitalhub_core-0.4.0b3/digitalhub_core/entities/workflows/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
 from digitalhub_core.entities.tasks.crud import create_task, create_task_from_dict, delete_task, new_task
-from digitalhub_core.utils.api import api_ctx_create, api_ctx_list, api_ctx_update
+from digitalhub_core.utils.api import api_ctx_create, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.exceptions import BackendError, EntityError
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
     from digitalhub_core.entities.runs.entity import Run
@@ -79,15 +79,15 @@
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
         # Initialize tasks
         self._tasks: dict[str, Task] = {}
 
     #############################
-    #  Save / Export
+    #  Save / Refresh / Export
     #############################
 
     def save(self, update: bool = False) -> Workflow:
         """
         Save entity into backend.
 
         Parameters
@@ -110,14 +110,28 @@
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "workflows", self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
+    def refresh(self) -> Workflow:
+        """
+        Refresh object from backend.
+
+        Returns
+        -------
+        Workflow
+            Entity refreshed.
+        """
+        api = api_ctx_read(self.project, "workflows", self.id)
+        obj = self._context().read_object(api)
+        self._update_attributes(obj)
+        return self
+
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
         filename : str
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/registry/import_utils.py` & `digitalhub_core-0.4.0b3/digitalhub_core/registry/import_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/registry/models.py` & `digitalhub_core-0.4.0b3/digitalhub_core/registry/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/registry/registry.py` & `digitalhub_core-0.4.0b3/digitalhub_core/registry/registry.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/runtimes/base.py` & `digitalhub_core-0.4.0b3/digitalhub_core/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/runtimes/builder.py` & `digitalhub_core-0.4.0b3/digitalhub_core/runtimes/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/stores/builder.py` & `digitalhub_core-0.4.0b3/digitalhub_core/stores/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/base.py` & `digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/local.py` & `digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/local.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/remote.py` & `digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/remote.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/s3.py` & `digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/s3.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/stores/objects/sql.py` & `digitalhub_core-0.4.0b3/digitalhub_core/stores/objects/sql.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/utils/api.py` & `digitalhub_core-0.4.0b3/digitalhub_core/utils/api.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/utils/env_utils.py` & `digitalhub_core-0.4.0b3/digitalhub_core/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/utils/file_utils.py` & `digitalhub_core-0.4.0b3/digitalhub_core/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/utils/generic_utils.py` & `digitalhub_core-0.4.0b3/digitalhub_core/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/utils/git_utils.py` & `digitalhub_core-0.4.0b3/digitalhub_core/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/utils/io_utils.py` & `digitalhub_core-0.4.0b3/digitalhub_core/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core/utils/uri_utils.py` & `digitalhub_core-0.4.0b3/digitalhub_core/utils/uri_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core.egg-info/PKG-INFO` & `digitalhub_core-0.4.0b3/digitalhub_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.4.0b2
+Version: 0.4.0b3
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub_core-0.4.0b2/digitalhub_core.egg-info/SOURCES.txt` & `digitalhub_core-0.4.0b3/digitalhub_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b2/pyproject.toml` & `digitalhub_core-0.4.0b3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-core"
-version = "0.4.0b2"
+version = "0.4.0b3"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -61,15 +61,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.4.0b2"
+current_version = "0.4.0b3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

