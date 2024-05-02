# Comparing `tmp/remotemanager-0.9.8.tar.gz` & `tmp/remotemanager-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.9.8.tar", last modified: Mon Jul 31 11:04:29 2023, max compression
+gzip compressed data, was "remotemanager-0.9.9.tar", last modified: Tue Aug  1 10:42:24 2023, max compression
```

## Comparing `remotemanager-0.9.8.tar` & `remotemanager-0.9.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.803992 remotemanager-0.9.8/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-31 11:04:29.803992 remotemanager-0.9.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:43:02.000000 remotemanager-0.9.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-31 10:33:38.000000 remotemanager-0.9.8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.795992 remotemanager-0.9.8/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      452 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.795992 remotemanager-0.9.8/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:02.000000 remotemanager-0.9.8/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.799992 remotemanager-0.9.8/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12848 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2023-07-31 09:51:39.000000 remotemanager-0.9.8/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 07:32:25.000000 remotemanager-0.9.8/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:40:04.000000 remotemanager-0.9.8/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6671 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    26005 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.799992 remotemanager-0.9.8/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    55681 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    10837 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-13 05:21:38.000000 remotemanager-0.9.8/remotemanager/dataset/lazy_append.py
--rw-rw-rw-   0 root         (0) root         (0)    23111 2023-07-28 11:41:58.000000 remotemanager-0.9.8/remotemanager/dataset/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-24 14:12:04.000000 remotemanager-0.9.8/remotemanager/dataset/runnerstates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.799992 remotemanager-0.9.8/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.8/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-31 09:51:39.000000 remotemanager-0.9.8/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.799992 remotemanager-0.9.8/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:02.000000 remotemanager-0.9.8/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:37.000000 remotemanager-0.9.8/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.8/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1892 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.803992 remotemanager-0.9.8/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:49.000000 remotemanager-0.9.8/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.8/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.8/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.803992 remotemanager-0.9.8/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6197 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5243 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:30.000000 remotemanager-0.9.8/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3694 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.803992 remotemanager-0.9.8/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2249 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)    10025 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.803992 remotemanager-0.9.8/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.8/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4504 2023-07-31 10:33:38.000000 remotemanager-0.9.8/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-21 10:04:17.000000 remotemanager-0.9.8/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 09:35:30.000000 remotemanager-0.9.8/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:04:29.795992 remotemanager-0.9.8/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-31 11:04:29.000000 remotemanager-0.9.8/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-31 11:04:29.000000 remotemanager-0.9.8/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 11:04:29.000000 remotemanager-0.9.8/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-31 11:04:29.000000 remotemanager-0.9.8/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-31 11:04:29.000000 remotemanager-0.9.8/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 11:04:29.803992 remotemanager-0.9.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.385930 remotemanager-0.9.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-08-01 10:42:24.385930 remotemanager-0.9.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:43:02.000000 remotemanager-0.9.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-08-01 09:45:06.000000 remotemanager-0.9.9/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.377930 remotemanager-0.9.9/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      452 2023-08-01 09:45:06.000000 remotemanager-0.9.9/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.377930 remotemanager-0.9.9/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-21 10:04:17.000000 remotemanager-0.9.9/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:02.000000 remotemanager-0.9.9/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.381930 remotemanager-0.9.9/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-21 10:04:17.000000 remotemanager-0.9.9/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12848 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2023-07-31 09:51:39.000000 remotemanager-0.9.9/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 07:32:25.000000 remotemanager-0.9.9/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:40:04.000000 remotemanager-0.9.9/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6671 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    26005 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.381930 remotemanager-0.9.9/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 10:04:17.000000 remotemanager-0.9.9/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    55814 2023-08-01 09:45:06.000000 remotemanager-0.9.9/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    10837 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-13 05:21:38.000000 remotemanager-0.9.9/remotemanager/dataset/lazy_append.py
+-rw-rw-rw-   0 root         (0) root         (0)    23184 2023-08-01 09:45:06.000000 remotemanager-0.9.9/remotemanager/dataset/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-24 14:12:04.000000 remotemanager-0.9.9/remotemanager/dataset/runnerstates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.381930 remotemanager-0.9.9/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.9/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-31 09:51:39.000000 remotemanager-0.9.9/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.381930 remotemanager-0.9.9/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:02.000000 remotemanager-0.9.9/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:37.000000 remotemanager-0.9.9/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.9/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1892 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-21 10:04:17.000000 remotemanager-0.9.9/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.381930 remotemanager-0.9.9/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:49.000000 remotemanager-0.9.9/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-21 10:04:17.000000 remotemanager-0.9.9/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.9/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.9/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-21 10:04:17.000000 remotemanager-0.9.9/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-21 10:04:17.000000 remotemanager-0.9.9/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.385930 remotemanager-0.9.9/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 10:04:17.000000 remotemanager-0.9.9/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6197 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5243 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    12878 2023-08-01 09:45:06.000000 remotemanager-0.9.9/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3694 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.385930 remotemanager-0.9.9/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-21 10:04:17.000000 remotemanager-0.9.9/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2249 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10025 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.385930 remotemanager-0.9.9/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.9/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4504 2023-07-31 10:33:38.000000 remotemanager-0.9.9/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-21 10:04:17.000000 remotemanager-0.9.9/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 09:35:30.000000 remotemanager-0.9.9/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:42:24.377930 remotemanager-0.9.9/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-08-01 10:42:24.000000 remotemanager-0.9.9/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-08-01 10:42:24.000000 remotemanager-0.9.9/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 10:42:24.000000 remotemanager-0.9.9/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-08-01 10:42:24.000000 remotemanager-0.9.9/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-08-01 10:42:24.000000 remotemanager-0.9.9/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 10:42:24.385930 remotemanager-0.9.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.9/setup.py
```

### Comparing `remotemanager-0.9.8/LICENSE` & `remotemanager-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/PKG-INFO` & `remotemanager-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.8
+Version: 0.9.9
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.8/README.md` & `remotemanager-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/pyproject.toml` & `remotemanager-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.9.8"
+current_version = "0.9.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.9.8/remotemanager/connection/cmd.py` & `remotemanager-0.9.9/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/connection/computers/base.py` & `remotemanager-0.9.9/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/connection/computers/example.py` & `remotemanager-0.9.9/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/connection/computers/options.py` & `remotemanager-0.9.9/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/connection/computers/parsers.py` & `remotemanager-0.9.9/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/connection/testing_object.py` & `remotemanager-0.9.9/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/connection/url.py` & `remotemanager-0.9.9/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/dataset/dataset.py` & `remotemanager-0.9.9/remotemanager/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1448,38 +1448,48 @@
         return self._run_cmd
 
     def check_runner_outputs(self):
         # check the files of the runners not reporting as completed
         # files to check
         resultfiles = []
         errorfiles = []
+        extrafiles = []
         for runner in self.runners:
             if runner.state == "reset":
                 self._logger.info("runner is in a reset state, ignoring")
                 continue
             resultfiles.append(runner.resultfile.remote)
             errorfiles.append(runner.errorfile.remote)
 
+            extrafiles += [f"{runner.run_path}/{f}" for f in runner.extra_files["recv"]]
+
         self._logger.runtime("checking remotely for runner outputs")
         search, _ = self.url.utils._file_mtime(
-            resultfiles + errorfiles,
+            resultfiles + errorfiles + extrafiles,
             local=self.url.is_local,
             python=False,
             dry_run=False,
         )
 
         # separate out the error files into their own dict
         errors = {}
+        extras = {}
         for file in errorfiles:
             try:
                 errors[file] = search.pop(file)
             except KeyError:
                 pass
 
-        return search, errors
+        for file in extrafiles:
+            try:
+                extras[file] = search.pop(file)
+            except KeyError:
+                pass
+
+        return search, errors, extras
 
     @property
     def is_finished(self):
         return self._is_finished()
 
     def _is_finished(self):
         self.avoid_runtime()
@@ -1494,15 +1504,15 @@
                 fin[runner.uuid] = True
 
         if all(fin.values()):
             self._logger.runtime("all runners are marked Completed, returning early")
             return list(fin.values())
 
         self._logger.runtime("runners polled, checking for files")
-        search, errors = self.check_runner_outputs()
+        search, errors, extras = self.check_runner_outputs()
 
         # parse runner states
         for runner in self.runners:
             if fin[runner.uuid]:
                 self._logger.runtime(f"runner {runner} is already marked as completed")
                 continue
             self._logger.runtime(f"checking outputs for {runner}")
@@ -1646,20 +1656,15 @@
                 continue
             if runner.state == "completed":
                 transfer = True
                 self._logger.info("runner marked as completed, pulling result")
                 self.transport.queue_for_pull(runner.resultfile)
 
                 for file in runner.extra_files["recv"]:
-                    rmt = (
-                        runner.run_dir
-                        if runner.run_dir is not None
-                        else runner.remote_dir
-                    )
-                    remote = os.path.join(rmt, os.path.split(file)[0])
+                    remote = os.path.join(runner.run_path, os.path.split(file)[0])
                     self.transport.queue_for_pull(
                         os.path.split(file)[1], runner.local_dir, remote
                     )
 
             elif runner.state == "failed":
                 transfer = True
                 self._logger.info("runner marked as completed, pulling error")
```

### Comparing `remotemanager-0.9.8/remotemanager/dataset/dependency.py` & `remotemanager-0.9.9/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/dataset/lazy_append.py` & `remotemanager-0.9.9/remotemanager/dataset/lazy_append.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/dataset/runner.py` & `remotemanager-0.9.9/remotemanager/dataset/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 import os
 import time
 
 from remotemanager.dataset.runnerstates import RunnerState
 from remotemanager.storage.database import Database
 from remotemanager.storage import SendableMixin, TrackedFile
 from remotemanager.logging.utils import format_iterable
-from remotemanager.storage.sendablemixin import SERIALISED_STORAGE_KEY
+from remotemanager.storage.sendablemixin import INTERNAL_STORAGE_KEYS
 from remotemanager.utils.uuid import generate_uuid
 from remotemanager.utils import object_from_uuid, _time_format, ensure_list
 from remotemanager.logging import LoggingMixin
 from remotemanager.logging.verbosity import Verbosity
 
 from datetime import datetime
 
+SERIALISED_STORAGE_KEY = INTERNAL_STORAGE_KEYS["SERIALISED_STORAGE_KEY"]
+
 localwinerror = """Local runs on windows machines are not supported.
 Please use a URL which connects to a non-windows machine or consider using
 Docker to continue."""
 
 
 class Runner(SendableMixin, LoggingMixin):
     """
```

### Comparing `remotemanager-0.9.8/remotemanager/dataset/runnerstates.py` & `remotemanager-0.9.9/remotemanager/dataset/runnerstates.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/jupyter/magic.py` & `remotemanager-0.9.9/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/logging/__init__.py` & `remotemanager-0.9.9/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/logging/log.py` & `remotemanager-0.9.9/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/logging/utils.py` & `remotemanager-0.9.9/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/logging/verbosity.py` & `remotemanager-0.9.9/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/serialisation/__init__.py` & `remotemanager-0.9.9/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/serialisation/serial.py` & `remotemanager-0.9.9/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.9.9/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.9.9/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/storage/database.py` & `remotemanager-0.9.9/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/storage/function.py` & `remotemanager-0.9.9/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/storage/remotefunction.py` & `remotemanager-0.9.9/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/storage/sendablemixin.py` & `remotemanager-0.9.9/remotemanager/storage/sendablemixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 import json
 import logging
 import os.path
 from collections import deque
 
 import yaml
 
-CLASS_STORAGE_KEY = "~serialisedclass~"
-TUPLE_STORAGE_KEY = "~serialisedtuple~"
-SET_STORAGE_KEY = "~serialisedset~"
-DEQUE_STORAGE_KEY = "~serialiseddeque"
-SERIALISED_STORAGE_KEY = "~serialisedobject~"
+INTERNAL_STORAGE_KEYS = {
+    "CLASS_STORAGE_KEY": "~serialisedclass~",
+    "TUPLE_STORAGE_KEY": "~serialisedtuple~",
+    "SET_STORAGE_KEY": "~serialisedset~",
+    "DEQUE_STORAGE_KEY": "~serialiseddeque",
+    "SERIALISED_STORAGE_KEY": "~serialisedobject~",
+    "SLOTS_ENABLE_KEY": "~usesslots~",
+}
 
 _logger = logging.getLogger(__name__)
 
 
 class SendableMixin:
     """
     Mixin class to create "sendable" object.
@@ -30,14 +33,16 @@
     converted to and from dict format
 
     >>> new = MyObject()
     >>> payload = new.pack()  # store the object in a dict object
     >>> recreated = MyObject.unpack(payload)  # create an instance from dict
     """
 
+    __slots__ = ["_unpack_validate"]
+
     def pack(self, uuid: str = None, file: str = None) -> [dict, None]:
         """
         "packs" the object into a dict-format, ready for yaml-dump
 
         Args:
             uuid (str):
                 Optional uuid string to package this data inside.
@@ -64,27 +69,35 @@
         # the mro of the object, and extracting it from the set
         # parent_class_names = get_mro_classnames(self)
 
         # if the class specifies a solo _do_not_package, add that
         never_package += getattr(self.__class__, "_do_not_package", [])
 
         payload = {}
-        for k, v in self.__dict__.items():
-            if k in never_package:
-                payload[k] = {
-                    CLASS_STORAGE_KEY: {
-                        "mod": "remotemanager.storage.sendablemixin",
-                        "name": "Unloaded",
+        if hasattr(self, "__dict__"):
+            # print("standard pack")
+            for k, v in self.__dict__.items():
+                if k in never_package:
+                    # print(f"skipping k = {k}")
+                    payload[k] = {
+                        INTERNAL_STORAGE_KEYS["CLASS_STORAGE_KEY"]: {
+                            "mod": "remotemanager.storage.sendablemixin",
+                            "name": "Unloaded",
+                        }
                     }
-                }
-                continue
+                    continue
 
-            payload[self.serialise(k)] = self.serialise(v)
+                payload[self.serialise(k)] = self.serialise(v)
+        else:
+            # print("slots pack")
+            payload[INTERNAL_STORAGE_KEYS["SLOTS_ENABLE_KEY"]] = True
+            for key in self.__slots__:
+                payload[self.serialise(key)] = self.__getattribute__(key)
 
-        payload[CLASS_STORAGE_KEY] = class_storage
+        payload[INTERNAL_STORAGE_KEYS["CLASS_STORAGE_KEY"]] = class_storage
 
         if uuid:
             if "_uuid" in payload and payload["_uuid"] != uuid:
                 raise ValueError("passed uuid and _uuid key in payload do" "not match!")
 
             payload["_uuid"] = uuid
 
@@ -177,29 +190,39 @@
 
         if hasattr(self, "_logger"):
             self._logger.info(f"finalising unpacking of {type(self)}")
 
         # temporary attribute to check for a valid class
         self._unpack_validate = True
 
-        if CLASS_STORAGE_KEY in payload:
+        if INTERNAL_STORAGE_KEYS["CLASS_STORAGE_KEY"] in payload:
             selfkey = get_class_storage(self)
-            packkey = payload[CLASS_STORAGE_KEY]
+            packkey = payload[INTERNAL_STORAGE_KEYS["CLASS_STORAGE_KEY"]]
 
             if selfkey != packkey:
                 raise RuntimeError(
                     f"attempting to unpack class "
                     f'{packkey["name"]} as '
                     f'{selfkey["name"]}'
                 )
 
             delattr(self, "_unpack_validate")
 
-        for k, v in payload.items():
-            self.__dict__[k] = self.unserialise(v, limit)
+        if payload.get(INTERNAL_STORAGE_KEYS["SLOTS_ENABLE_KEY"], False):
+            # print("unpacking into slots")
+            for k, v in payload.items():
+                if k in list(INTERNAL_STORAGE_KEYS.values()):
+                    continue
+                self.__setattr__(k, v)
+        else:
+            # print("standard unpack")
+            for k, v in payload.items():
+                if k in list(INTERNAL_STORAGE_KEYS.values()):
+                    continue
+                self.__dict__[k] = self.unserialise(v, limit)
 
     def serialise(self, obj):
         """
         Recurse over any iterable objects, or call the pack() method of any
         `SendableMixin` objects, for serialisation
 
         Args:
@@ -228,29 +251,38 @@
 
         elif isinstance(obj, list):
             # list-type
             return [self.serialise(v) for v in obj]
 
         elif isinstance(obj, tuple):
             # tuple-type
-            return [TUPLE_STORAGE_KEY] + [self.serialise(v) for v in obj]
+            return [INTERNAL_STORAGE_KEYS["TUPLE_STORAGE_KEY"]] + [
+                self.serialise(v) for v in obj
+            ]
 
         elif isinstance(obj, set):
             # set-type
-            return [SET_STORAGE_KEY] + [self.serialise(v) for v in obj]
+            return [INTERNAL_STORAGE_KEYS["SET_STORAGE_KEY"]] + [
+                self.serialise(v) for v in obj
+            ]
 
         elif isinstance(obj, deque):
             # collections deque
-            return [DEQUE_STORAGE_KEY, obj.maxlen] + [self.serialise(v) for v in obj]
+            return [INTERNAL_STORAGE_KEYS["DEQUE_STORAGE_KEY"], obj.maxlen] + [
+                self.serialise(v) for v in obj
+            ]
 
         if basic_available(obj):
             return obj
 
         try:
-            return [SERIALISED_STORAGE_KEY, self.serialiser.dumps(obj)]
+            return [
+                INTERNAL_STORAGE_KEYS["SERIALISED_STORAGE_KEY"],
+                self.serialiser.dumps(obj),
+            ]
         except AttributeError:
             pass
 
         raise RuntimeError(
             f"Failed to yaml dump {obj.__class__.__name__} " f"object {obj}"
         )
 
@@ -266,22 +298,22 @@
                 exit if the object to be unpacked is not part of the
                 remotemanager package
 
         Returns:
             object before packaging
         """
         try:
-            unpackable = obj.get(CLASS_STORAGE_KEY)
+            unpackable = obj.get(INTERNAL_STORAGE_KEYS["CLASS_STORAGE_KEY"])
         except AttributeError:
             unpackable = False
 
         if unpackable:
             # print(f'unserialising unpackable object {obj}')
             # extract the class to import
-            source = obj.pop(CLASS_STORAGE_KEY)
+            source = obj.pop(INTERNAL_STORAGE_KEYS["CLASS_STORAGE_KEY"])
 
             if "_conn" in obj:
                 # disable protection for URLs
                 limit = False
 
             # import the module
             modulename = source["mod"]
@@ -300,19 +332,19 @@
         elif isinstance(obj, collections.abc.Mapping):
             # dict type
             return {self.unserialise(k): self.unserialise(v) for k, v in obj.items()}
 
         # coming from the yaml file, output should _only_ be list
         elif isinstance(obj, list):
             try:
-                if obj[0] == TUPLE_STORAGE_KEY:
+                if obj[0] == INTERNAL_STORAGE_KEYS["TUPLE_STORAGE_KEY"]:
                     return tuple([self.unserialise(o) for o in obj[1:]])
-                elif obj[0] == SET_STORAGE_KEY:
+                elif obj[0] == INTERNAL_STORAGE_KEYS["SET_STORAGE_KEY"]:
                     return set([self.unserialise(o) for o in obj[1:]])
-                elif obj[0] == DEQUE_STORAGE_KEY:
+                elif obj[0] == INTERNAL_STORAGE_KEYS["DEQUE_STORAGE_KEY"]:
                     maxlen = obj[1]
                     dqobj = obj[2:]
                     return deque([self.unserialise(o) for o in dqobj], maxlen=maxlen)
             except IndexError:
                 return [self.unserialise(v) for v in obj]
 
         if basic_available(obj):
```

### Comparing `remotemanager-0.9.8/remotemanager/storage/trackedfile.py` & `remotemanager-0.9.9/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/transport/cp.py` & `remotemanager-0.9.9/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/transport/rsync.py` & `remotemanager-0.9.9/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/transport/scp.py` & `remotemanager-0.9.9/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/transport/transport.py` & `remotemanager-0.9.9/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/utils/__init__.py` & `remotemanager-0.9.9/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/utils/flags.py` & `remotemanager-0.9.9/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager/utils/version.py` & `remotemanager-0.9.9/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.8/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.9.9/remotemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.8
+Version: 0.9.9
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.8/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.9.9/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

