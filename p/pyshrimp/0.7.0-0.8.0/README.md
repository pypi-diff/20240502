# Comparing `tmp/pyshrimp-0.7.0.tar.gz` & `tmp/pyshrimp-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyshrimp-0.7.0.tar", last modified: Fri Mar  8 15:45:05 2024, max compression
+gzip compressed data, was "pyshrimp-0.8.0.tar", last modified: Thu May  2 13:53:08 2024, max compression
```

## Comparing `pyshrimp-0.7.0.tar` & `pyshrimp-0.8.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.030713 pyshrimp-0.7.0/
--rw-rw-r--   0 ali       (1000) ali       (1000)     1077 2021-11-26 08:32:42.000000 pyshrimp-0.7.0/LICENSE.txt
--rw-r--r--   0 ali       (1000) ali       (1000)    13354 2024-03-08 15:45:05.030713 pyshrimp-0.7.0/PKG-INFO
--rw-r--r--   0 ali       (1000) ali       (1000)    12832 2024-03-08 14:08:44.000000 pyshrimp-0.7.0/README.md
--rw-rw-r--   0 ali       (1000) ali       (1000)      104 2021-11-13 16:38:41.000000 pyshrimp-0.7.0/pyproject.toml
--rw-r--r--   0 ali       (1000) ali       (1000)      773 2024-03-08 15:45:05.030713 pyshrimp-0.7.0/setup.cfg
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.026713 pyshrimp-0.7.0/src/
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.026713 pyshrimp-0.7.0/src/pyshrimp/
--rw-rw-r--   0 ali       (1000) ali       (1000)     1403 2024-03-08 14:45:35.000000 pyshrimp-0.7.0/src/pyshrimp/__init__.py
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.026713 pyshrimp-0.7.0/src/pyshrimp/_internal/
--rw-r--r--   0 ali       (1000) ali       (1000)        0 2021-10-22 15:22:12.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/__init__.py
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.026713 pyshrimp-0.7.0/src/pyshrimp/_internal/locking/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2022-11-27 18:49:00.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/locking/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      392 2022-11-28 19:52:17.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/locking/file_based_lock_internal.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1960 2022-12-01 17:35:14.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/locking/file_based_lock_posix.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3422 2022-12-01 17:33:02.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/locking/file_based_lock_windows.py
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.026713 pyshrimp-0.7.0/src/pyshrimp/_internal/pipes/
--rw-r--r--   0 ali       (1000) ali       (1000)        0 2021-10-22 15:22:12.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/pipes/__init__.py
--rw-r--r--   0 ali       (1000) ali       (1000)     2044 2021-11-11 11:59:33.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/pipes/async_function.py
--rw-r--r--   0 ali       (1000) ali       (1000)      175 2021-11-06 08:28:16.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/pipes/utils.py
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.026713 pyshrimp-0.7.0/src/pyshrimp/_internal/scriptrunner/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2021-10-22 15:22:12.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/scriptrunner/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    15324 2024-03-08 14:07:11.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/scriptrunner/bootstrap.py
--rw-r--r--   0 ali       (1000) ali       (1000)     2914 2021-11-28 12:26:26.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/scriptrunner/cli.py
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.030713 pyshrimp-0.7.0/src/pyshrimp/_internal/utils/
--rw-r--r--   0 ali       (1000) ali       (1000)        0 2021-10-23 12:09:56.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/utils/__init__.py
--rw-r--r--   0 ali       (1000) ali       (1000)       91 2021-11-21 10:42:33.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/utils/errors.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      117 2022-12-04 12:30:48.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/utils/platformspecific.py
--rw-r--r--   0 ali       (1000) ali       (1000)     1841 2021-12-18 16:11:03.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/utils/subprocess_utils.py
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.030713 pyshrimp-0.7.0/src/pyshrimp/_internal/wrapper/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2021-10-22 15:22:12.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/wrapper/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1423 2021-11-21 10:45:35.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/wrapper/magicwrapper.py
--rw-r--r--   0 ali       (1000) ali       (1000)      189 2021-11-21 10:36:11.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/wrapper/magicwrapper_state.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4140 2021-11-21 10:47:04.000000 pyshrimp-0.7.0/src/pyshrimp/_internal/wrapper/mainwrapper.py
--rw-r--r--   0 ali       (1000) ali       (1000)      382 2021-11-06 08:53:27.000000 pyshrimp-0.7.0/src/pyshrimp/exception.py
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.030713 pyshrimp-0.7.0/src/pyshrimp/execution_pipeline/
--rw-r--r--   0 ali       (1000) ali       (1000)        0 2021-10-23 12:26:41.000000 pyshrimp-0.7.0/src/pyshrimp/execution_pipeline/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4831 2021-11-13 10:51:52.000000 pyshrimp-0.7.0/src/pyshrimp/execution_pipeline/pipeline.py
--rw-r--r--   0 ali       (1000) ali       (1000)     1817 2021-11-11 11:59:51.000000 pyshrimp-0.7.0/src/pyshrimp/execution_pipeline/pipeline_api.py
--rw-r--r--   0 ali       (1000) ali       (1000)      763 2021-11-11 11:59:33.000000 pyshrimp-0.7.0/src/pyshrimp/execution_pipeline/pipeline_starter.py
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.030713 pyshrimp-0.7.0/src/pyshrimp/utils/
--rw-r--r--   0 ali       (1000) ali       (1000)        0 2021-10-23 12:08:37.000000 pyshrimp-0.7.0/src/pyshrimp/utils/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      132 2023-03-10 18:25:32.000000 pyshrimp-0.7.0/src/pyshrimp/utils/collections.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     6549 2023-03-10 19:40:10.000000 pyshrimp-0.7.0/src/pyshrimp/utils/command.py
--rw-r--r--   0 ali       (1000) ali       (1000)     3408 2022-05-07 15:14:38.000000 pyshrimp-0.7.0/src/pyshrimp/utils/dotdict.py
--rw-r--r--   0 ali       (1000) ali       (1000)     2817 2022-12-04 16:22:52.000000 pyshrimp-0.7.0/src/pyshrimp/utils/filesystem.py
--rw-r--r--   0 ali       (1000) ali       (1000)     1359 2022-12-04 12:30:51.000000 pyshrimp-0.7.0/src/pyshrimp/utils/locking.py
--rw-r--r--   0 ali       (1000) ali       (1000)      223 2021-11-13 20:03:54.000000 pyshrimp-0.7.0/src/pyshrimp/utils/logging.py
--rw-r--r--   0 ali       (1000) ali       (1000)      210 2021-11-12 17:03:18.000000 pyshrimp-0.7.0/src/pyshrimp/utils/matching.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      333 2021-11-13 14:18:42.000000 pyshrimp-0.7.0/src/pyshrimp/utils/parallel.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      781 2021-11-29 14:54:29.000000 pyshrimp-0.7.0/src/pyshrimp/utils/splitter.py
--rw-r--r--   0 ali       (1000) ali       (1000)     1690 2021-11-29 14:52:58.000000 pyshrimp-0.7.0/src/pyshrimp/utils/string_wrapper.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3389 2021-12-05 18:42:43.000000 pyshrimp-0.7.0/src/pyshrimp/utils/subprocess_utils.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1052 2021-11-29 14:52:58.000000 pyshrimp-0.7.0/src/pyshrimp/utils/table_parser.py
--rw-r--r--   0 ali       (1000) ali       (1000)     1728 2021-11-13 20:16:51.000000 pyshrimp-0.7.0/src/pyshrimp/utils/wait.py
-drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-03-08 15:45:05.030713 pyshrimp-0.7.0/src/pyshrimp.egg-info/
--rw-r--r--   0 ali       (1000) ali       (1000)    13354 2024-03-08 15:45:05.000000 pyshrimp-0.7.0/src/pyshrimp.egg-info/PKG-INFO
--rw-r--r--   0 ali       (1000) ali       (1000)     1801 2024-03-08 15:45:05.000000 pyshrimp-0.7.0/src/pyshrimp.egg-info/SOURCES.txt
--rw-r--r--   0 ali       (1000) ali       (1000)        1 2024-03-08 15:45:05.000000 pyshrimp-0.7.0/src/pyshrimp.egg-info/dependency_links.txt
--rw-r--r--   0 ali       (1000) ali       (1000)       82 2024-03-08 15:45:05.000000 pyshrimp-0.7.0/src/pyshrimp.egg-info/entry_points.txt
--rw-r--r--   0 ali       (1000) ali       (1000)        9 2024-03-08 15:45:05.000000 pyshrimp-0.7.0/src/pyshrimp.egg-info/top_level.txt
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.439751 pyshrimp-0.8.0/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1077 2021-11-26 08:32:42.000000 pyshrimp-0.8.0/LICENSE.txt
+-rw-r--r--   0 ali       (1000) ali       (1000)    13257 2024-05-02 13:53:08.439751 pyshrimp-0.8.0/PKG-INFO
+-rw-r--r--   0 ali       (1000) ali       (1000)    12735 2024-03-10 16:46:17.000000 pyshrimp-0.8.0/README.md
+-rw-rw-r--   0 ali       (1000) ali       (1000)      104 2021-11-13 16:38:41.000000 pyshrimp-0.8.0/pyproject.toml
+-rw-r--r--   0 ali       (1000) ali       (1000)      773 2024-05-02 13:53:08.439751 pyshrimp-0.8.0/setup.cfg
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.431752 pyshrimp-0.8.0/src/
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.435752 pyshrimp-0.8.0/src/pyshrimp/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1403 2024-05-02 13:25:40.000000 pyshrimp-0.8.0/src/pyshrimp/__init__.py
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.435752 pyshrimp-0.8.0/src/pyshrimp/_internal/
+-rw-r--r--   0 ali       (1000) ali       (1000)        0 2021-10-22 15:22:12.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/__init__.py
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.435752 pyshrimp-0.8.0/src/pyshrimp/_internal/locking/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2022-11-27 18:49:00.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/locking/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      392 2022-11-28 19:52:17.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/locking/file_based_lock_internal.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1960 2022-12-01 17:35:14.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/locking/file_based_lock_posix.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3422 2022-12-01 17:33:02.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/locking/file_based_lock_windows.py
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.435752 pyshrimp-0.8.0/src/pyshrimp/_internal/pipes/
+-rw-r--r--   0 ali       (1000) ali       (1000)        0 2021-10-22 15:22:12.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/pipes/__init__.py
+-rw-r--r--   0 ali       (1000) ali       (1000)     2044 2021-11-11 11:59:33.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/pipes/async_function.py
+-rw-r--r--   0 ali       (1000) ali       (1000)      175 2021-11-06 08:28:16.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/pipes/utils.py
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.435752 pyshrimp-0.8.0/src/pyshrimp/_internal/scriptrunner/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2021-10-22 15:22:12.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/scriptrunner/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    15325 2024-05-02 13:22:38.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/scriptrunner/bootstrap.py
+-rw-r--r--   0 ali       (1000) ali       (1000)     2914 2021-11-28 12:26:26.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/scriptrunner/cli.py
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.435752 pyshrimp-0.8.0/src/pyshrimp/_internal/utils/
+-rw-r--r--   0 ali       (1000) ali       (1000)        0 2021-10-23 12:09:56.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/utils/__init__.py
+-rw-r--r--   0 ali       (1000) ali       (1000)       91 2021-11-21 10:42:33.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/utils/errors.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      117 2022-12-04 12:30:48.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/utils/platformspecific.py
+-rw-r--r--   0 ali       (1000) ali       (1000)     1841 2021-12-18 16:11:03.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/utils/subprocess_utils.py
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.435752 pyshrimp-0.8.0/src/pyshrimp/_internal/wrapper/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2021-10-22 15:22:12.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/wrapper/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1423 2021-11-21 10:45:35.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/wrapper/magicwrapper.py
+-rw-r--r--   0 ali       (1000) ali       (1000)      189 2021-11-21 10:36:11.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/wrapper/magicwrapper_state.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4140 2021-11-21 10:47:04.000000 pyshrimp-0.8.0/src/pyshrimp/_internal/wrapper/mainwrapper.py
+-rw-r--r--   0 ali       (1000) ali       (1000)      382 2021-11-06 08:53:27.000000 pyshrimp-0.8.0/src/pyshrimp/exception.py
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.435752 pyshrimp-0.8.0/src/pyshrimp/execution_pipeline/
+-rw-r--r--   0 ali       (1000) ali       (1000)        0 2021-10-23 12:26:41.000000 pyshrimp-0.8.0/src/pyshrimp/execution_pipeline/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4831 2021-11-13 10:51:52.000000 pyshrimp-0.8.0/src/pyshrimp/execution_pipeline/pipeline.py
+-rw-r--r--   0 ali       (1000) ali       (1000)     1817 2021-11-11 11:59:51.000000 pyshrimp-0.8.0/src/pyshrimp/execution_pipeline/pipeline_api.py
+-rw-r--r--   0 ali       (1000) ali       (1000)      763 2021-11-11 11:59:33.000000 pyshrimp-0.8.0/src/pyshrimp/execution_pipeline/pipeline_starter.py
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.439751 pyshrimp-0.8.0/src/pyshrimp/utils/
+-rw-r--r--   0 ali       (1000) ali       (1000)        0 2021-10-23 12:08:37.000000 pyshrimp-0.8.0/src/pyshrimp/utils/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      132 2023-03-10 18:25:32.000000 pyshrimp-0.8.0/src/pyshrimp/utils/collections.py
+-rw-r--r--   0 ali       (1000) ali       (1000)     6549 2024-05-02 13:52:52.000000 pyshrimp-0.8.0/src/pyshrimp/utils/command.py
+-rw-r--r--   0 ali       (1000) ali       (1000)     3408 2022-05-07 15:14:38.000000 pyshrimp-0.8.0/src/pyshrimp/utils/dotdict.py
+-rw-r--r--   0 ali       (1000) ali       (1000)     2817 2022-12-04 16:22:52.000000 pyshrimp-0.8.0/src/pyshrimp/utils/filesystem.py
+-rw-r--r--   0 ali       (1000) ali       (1000)     1359 2022-12-04 12:30:51.000000 pyshrimp-0.8.0/src/pyshrimp/utils/locking.py
+-rw-r--r--   0 ali       (1000) ali       (1000)      223 2021-11-13 20:03:54.000000 pyshrimp-0.8.0/src/pyshrimp/utils/logging.py
+-rw-r--r--   0 ali       (1000) ali       (1000)      210 2021-11-12 17:03:18.000000 pyshrimp-0.8.0/src/pyshrimp/utils/matching.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      333 2021-11-13 14:18:42.000000 pyshrimp-0.8.0/src/pyshrimp/utils/parallel.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      781 2021-11-29 14:54:29.000000 pyshrimp-0.8.0/src/pyshrimp/utils/splitter.py
+-rw-r--r--   0 ali       (1000) ali       (1000)     1690 2021-11-29 14:52:58.000000 pyshrimp-0.8.0/src/pyshrimp/utils/string_wrapper.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3389 2021-12-05 18:42:43.000000 pyshrimp-0.8.0/src/pyshrimp/utils/subprocess_utils.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1052 2021-11-29 14:52:58.000000 pyshrimp-0.8.0/src/pyshrimp/utils/table_parser.py
+-rw-r--r--   0 ali       (1000) ali       (1000)     1728 2021-11-13 20:16:51.000000 pyshrimp-0.8.0/src/pyshrimp/utils/wait.py
+drwxr-xr-x   0 ali       (1000) ali       (1000)        0 2024-05-02 13:53:08.439751 pyshrimp-0.8.0/src/pyshrimp.egg-info/
+-rw-r--r--   0 ali       (1000) ali       (1000)    13257 2024-05-02 13:53:08.000000 pyshrimp-0.8.0/src/pyshrimp.egg-info/PKG-INFO
+-rw-r--r--   0 ali       (1000) ali       (1000)     1801 2024-05-02 13:53:08.000000 pyshrimp-0.8.0/src/pyshrimp.egg-info/SOURCES.txt
+-rw-r--r--   0 ali       (1000) ali       (1000)        1 2024-05-02 13:53:08.000000 pyshrimp-0.8.0/src/pyshrimp.egg-info/dependency_links.txt
+-rw-r--r--   0 ali       (1000) ali       (1000)       82 2024-05-02 13:53:08.000000 pyshrimp-0.8.0/src/pyshrimp.egg-info/entry_points.txt
+-rw-r--r--   0 ali       (1000) ali       (1000)        9 2024-05-02 13:53:08.000000 pyshrimp-0.8.0/src/pyshrimp.egg-info/top_level.txt
```

### Comparing `pyshrimp-0.7.0/LICENSE.txt` & `pyshrimp-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/PKG-INFO` & `pyshrimp-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshrimp
-Version: 0.7.0
+Version: 0.8.0
 Summary: PyShrimp
 Home-page: https://github.com/osomdev/pyshrimp
 Author: Aleksander Mierzwicki
 Author-email: ali.pypipublic@osomdev.pl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/osomdev/pyshrimp/issues
 Platform: Linux
@@ -336,19 +336,17 @@
 ```
 
 ## Supported environment
 
 This project was developed on **Ubuntu Linux**. It should work with any linux system, but I can imagine the tests
 failing in case some system binaries are missing.
 
-It was not tested on macOS (probably will work fine) and some parts for sure will not work on Windows
-(e.g. shell wrapping is depending on bash).
-
-Feel free to raise bugs found when using this project on macOS - it shouldn't be too hard to address them.
+The project is also tested on macOS before new version is released.
 
+Some parts for sure will not work on Windows (e.g. shell wrapping is depending on bash).
 The author does not have plans to introduce support for Windows but contributions are welcome ;).
 
 ## License
 
 The project is licensed under [MIT License](./LICENSE.txt) with exceptions listed below.
 
 Project license exceptions:
```

### Comparing `pyshrimp-0.7.0/README.md` & `pyshrimp-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -319,19 +319,17 @@
 ```
 
 ## Supported environment
 
 This project was developed on **Ubuntu Linux**. It should work with any linux system, but I can imagine the tests
 failing in case some system binaries are missing.
 
-It was not tested on macOS (probably will work fine) and some parts for sure will not work on Windows
-(e.g. shell wrapping is depending on bash).
-
-Feel free to raise bugs found when using this project on macOS - it shouldn't be too hard to address them.
+The project is also tested on macOS before new version is released.
 
+Some parts for sure will not work on Windows (e.g. shell wrapping is depending on bash).
 The author does not have plans to introduce support for Windows but contributions are welcome ;).
 
 ## License
 
 The project is licensed under [MIT License](./LICENSE.txt) with exceptions listed below.
 
 Project license exceptions:
```

### Comparing `pyshrimp-0.7.0/setup.cfg` & `pyshrimp-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/__init__.py` & `pyshrimp-0.8.0/src/pyshrimp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.7.0'
+__version__ = '0.8.0'
 
 # noinspection PyProtectedMember
 from pyshrimp._internal.wrapper.mainwrapper import _run as run
 # noinspection PyProtectedMember
 from pyshrimp._internal.wrapper.mainwrapper import _init_logging as init_logging
 from pyshrimp.execution_pipeline.pipeline import pipe, ExecutionPipeline
 from pyshrimp.execution_pipeline.pipeline_api import PipelineExecutionResult
```

### Comparing `pyshrimp-0.7.0/src/pyshrimp/_internal/locking/file_based_lock_posix.py` & `pyshrimp-0.8.0/src/pyshrimp/_internal/locking/file_based_lock_posix.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/_internal/locking/file_based_lock_windows.py` & `pyshrimp-0.8.0/src/pyshrimp/_internal/locking/file_based_lock_windows.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/_internal/pipes/async_function.py` & `pyshrimp-0.8.0/src/pyshrimp/_internal/pipes/async_function.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/_internal/scriptrunner/bootstrap.py` & `pyshrimp-0.8.0/src/pyshrimp/_internal/scriptrunner/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 
         return python_executable_path
 
     def setup_virtual_env_using_venv(self, venv_dir):
         import venv
         try:
             self.log(f'Setting up venv using venv')
-            venv.create(venv_dir, system_site_packages=True, with_pip=True, clear=True)
+            venv.create(venv_dir, system_site_packages=False, with_pip=True, clear=True)
         except BaseException:
             raise self.exit_error(f'Failed to setup virtualenv! Check previous messages for details.', exc_info=True)
 
     def setup_virtual_env_using_virtualenv(self, venv_dir):
         command = [sys.executable, '-m', 'virtualenv', '-p', sys.executable, '--clear', venv_dir]
         self.log(f'Setting up venv using virtualenv: {command}')
         result = subprocess.run(command, stdout=subprocess.PIPE)
```

### Comparing `pyshrimp-0.7.0/src/pyshrimp/_internal/scriptrunner/cli.py` & `pyshrimp-0.8.0/src/pyshrimp/_internal/scriptrunner/cli.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/_internal/utils/subprocess_utils.py` & `pyshrimp-0.8.0/src/pyshrimp/_internal/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/_internal/wrapper/magicwrapper.py` & `pyshrimp-0.8.0/src/pyshrimp/_internal/wrapper/magicwrapper.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/_internal/wrapper/mainwrapper.py` & `pyshrimp-0.8.0/src/pyshrimp/_internal/wrapper/mainwrapper.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/execution_pipeline/pipeline.py` & `pyshrimp-0.8.0/src/pyshrimp/execution_pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/execution_pipeline/pipeline_api.py` & `pyshrimp-0.8.0/src/pyshrimp/execution_pipeline/pipeline_api.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/execution_pipeline/pipeline_starter.py` & `pyshrimp-0.8.0/src/pyshrimp/execution_pipeline/pipeline_starter.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/utils/command.py` & `pyshrimp-0.8.0/src/pyshrimp/utils/command.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/utils/dotdict.py` & `pyshrimp-0.8.0/src/pyshrimp/utils/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/utils/filesystem.py` & `pyshrimp-0.8.0/src/pyshrimp/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/utils/locking.py` & `pyshrimp-0.8.0/src/pyshrimp/utils/locking.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/utils/splitter.py` & `pyshrimp-0.8.0/src/pyshrimp/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/utils/string_wrapper.py` & `pyshrimp-0.8.0/src/pyshrimp/utils/string_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/utils/subprocess_utils.py` & `pyshrimp-0.8.0/src/pyshrimp/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/utils/table_parser.py` & `pyshrimp-0.8.0/src/pyshrimp/utils/table_parser.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp/utils/wait.py` & `pyshrimp-0.8.0/src/pyshrimp/utils/wait.py`

 * *Files identical despite different names*

### Comparing `pyshrimp-0.7.0/src/pyshrimp.egg-info/PKG-INFO` & `pyshrimp-0.8.0/src/pyshrimp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshrimp
-Version: 0.7.0
+Version: 0.8.0
 Summary: PyShrimp
 Home-page: https://github.com/osomdev/pyshrimp
 Author: Aleksander Mierzwicki
 Author-email: ali.pypipublic@osomdev.pl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/osomdev/pyshrimp/issues
 Platform: Linux
@@ -336,19 +336,17 @@
 ```
 
 ## Supported environment
 
 This project was developed on **Ubuntu Linux**. It should work with any linux system, but I can imagine the tests
 failing in case some system binaries are missing.
 
-It was not tested on macOS (probably will work fine) and some parts for sure will not work on Windows
-(e.g. shell wrapping is depending on bash).
-
-Feel free to raise bugs found when using this project on macOS - it shouldn't be too hard to address them.
+The project is also tested on macOS before new version is released.
 
+Some parts for sure will not work on Windows (e.g. shell wrapping is depending on bash).
 The author does not have plans to introduce support for Windows but contributions are welcome ;).
 
 ## License
 
 The project is licensed under [MIT License](./LICENSE.txt) with exceptions listed below.
 
 Project license exceptions:
```

### Comparing `pyshrimp-0.7.0/src/pyshrimp.egg-info/SOURCES.txt` & `pyshrimp-0.8.0/src/pyshrimp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

