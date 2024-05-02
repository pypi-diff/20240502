# Comparing `tmp/dynamic_import-2024.2.13.tar.gz` & `tmp/dynamic_import-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_import-2024.2.13.tar", last modified: Wed Feb 14 00:17:36 2024, max compression
+gzip compressed data, was "dynamic_import-2024.5.2.tar", last modified: Thu May  2 16:24:52 2024, max compression
```

## Comparing `dynamic_import-2024.2.13.tar` & `dynamic_import-2024.5.2.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.410105 dynamic_import-2024.2.13/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     7048 2020-02-25 14:17:19.000000 dynamic_import-2024.2.13/LICENSE.txt
--rw-r--r--   0 stealth   (1000) stealth   (1000)      178 2024-01-31 21:50:28.000000 dynamic_import-2024.2.13/MANIFEST.in
--rw-r--r--   0 stealth   (1000) stealth   (1000)    14823 2024-02-14 00:17:36.410105 dynamic_import-2024.2.13/PKG-INFO
--rw-r--r--   0 stealth   (1000) stealth   (1000)     5833 2024-02-14 00:11:12.000000 dynamic_import-2024.2.13/README.rst
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.400106 dynamic_import-2024.2.13/dynamic_import/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      277 2024-01-27 17:35:22.000000 dynamic_import-2024.2.13/dynamic_import/__init__.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3776 2024-01-31 23:24:39.000000 dynamic_import-2024.2.13/dynamic_import/cache.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     4793 2024-01-31 23:26:36.000000 dynamic_import-2024.2.13/dynamic_import/check.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3056 2024-02-13 23:29:08.000000 dynamic_import-2024.2.13/dynamic_import/extract.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3731 2024-02-13 23:30:20.000000 dynamic_import-2024.2.13/dynamic_import/importer.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2946 2024-02-13 23:36:12.000000 dynamic_import-2024.2.13/dynamic_import/module.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     4190 2024-01-31 23:29:31.000000 dynamic_import-2024.2.13/dynamic_import/prep.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      918 2024-01-28 06:53:10.000000 dynamic_import-2024.2.13/dynamic_import/special.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       44 2024-02-13 07:36:15.000000 dynamic_import-2024.2.13/dynamic_import/version.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.410105 dynamic_import-2024.2.13/dynamic_import.egg-info/
--rw-r--r--   0 stealth   (1000) stealth   (1000)    14823 2024-02-14 00:17:36.000000 dynamic_import-2024.2.13/dynamic_import.egg-info/PKG-INFO
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1270 2024-02-14 00:17:36.000000 dynamic_import-2024.2.13/dynamic_import.egg-info/SOURCES.txt
--rw-r--r--   0 stealth   (1000) stealth   (1000)        1 2024-02-14 00:17:36.000000 dynamic_import-2024.2.13/dynamic_import.egg-info/dependency_links.txt
--rw-r--r--   0 stealth   (1000) stealth   (1000)       15 2024-02-14 00:17:36.000000 dynamic_import-2024.2.13/dynamic_import.egg-info/top_level.txt
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.400106 dynamic_import-2024.2.13/example/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      216 2024-01-24 03:59:57.000000 dynamic_import-2024.2.13/example/calling.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.403439 dynamic_import-2024.2.13/example/pkg/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      452 2024-01-31 21:50:28.000000 dynamic_import-2024.2.13/example/pkg/__init__.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.403439 dynamic_import-2024.2.13/example/pkg/classes/
--rw-r--r--   0 stealth   (1000) stealth   (1000)       48 2024-01-05 03:34:55.000000 dynamic_import-2024.2.13/example/pkg/classes/__init__.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.403439 dynamic_import-2024.2.13/example/pkg/functions/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      234 2024-02-01 14:02:20.000000 dynamic_import-2024.2.13/example/pkg/functions/myfunction.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      162 2024-01-05 03:34:44.000000 dynamic_import-2024.2.13/example/pkg/var.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1511 2024-02-01 20:25:33.000000 dynamic_import-2024.2.13/pyproject.toml
--rw-r--r--   0 stealth   (1000) stealth   (1000)       38 2024-02-14 00:17:36.410105 dynamic_import-2024.2.13/setup.cfg
--rw-r--r--   0 stealth   (1000) stealth   (1000)       70 2024-01-27 17:20:13.000000 dynamic_import-2024.2.13/setup.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.406772 dynamic_import-2024.2.13/test/
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.406772 dynamic_import-2024.2.13/test/basic/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      173 2024-01-31 21:55:23.000000 dynamic_import-2024.2.13/test/basic/__init__.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       90 2024-01-07 07:52:04.000000 dynamic_import-2024.2.13/test/basic/one.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.406772 dynamic_import-2024.2.13/test/basic/skip/
--rw-r--r--   0 stealth   (1000) stealth   (1000)       49 2024-01-25 18:03:26.000000 dynamic_import-2024.2.13/test/basic/skip/bad-file.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       14 2024-01-30 09:43:20.000000 dynamic_import-2024.2.13/test/basic/skip/bad_all.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.406772 dynamic_import-2024.2.13/test/basic/so/
--rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-01-31 21:46:21.000000 dynamic_import-2024.2.13/test/basic/so/__init__.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.406772 dynamic_import-2024.2.13/test/basic/sub/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      277 2024-02-01 14:03:14.000000 dynamic_import-2024.2.13/test/basic/sub/auto_find.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.406772 dynamic_import-2024.2.13/test/basic/sub/child/
--rw-r--r--   0 stealth   (1000) stealth   (1000)       61 2021-05-01 03:35:14.000000 dynamic_import-2024.2.13/test/basic/sub/child/child.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.406772 dynamic_import-2024.2.13/test/basic/sub/conflict/
--rw-r--r--   0 stealth   (1000) stealth   (1000)       81 2024-01-05 06:46:07.000000 dynamic_import-2024.2.13/test/basic/sub/conflict/__init__.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      119 2021-04-29 23:24:22.000000 dynamic_import-2024.2.13/test/basic/sub/four_five.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       24 2024-01-25 14:28:21.000000 dynamic_import-2024.2.13/test/basic/sub/skip-me.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       63 2021-04-29 23:22:27.000000 dynamic_import-2024.2.13/test/basic/sub/three.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       91 2021-04-29 23:22:47.000000 dynamic_import-2024.2.13/test/basic/two.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.410105 dynamic_import-2024.2.13/test/block/
--rw-r--r--   0 stealth   (1000) stealth   (1000)       60 2024-01-31 21:55:45.000000 dynamic_import-2024.2.13/test/block/__init__.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      151 2024-01-31 21:56:03.000000 dynamic_import-2024.2.13/test/block/block.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.410105 dynamic_import-2024.2.13/test/block1/
--rw-r--r--   0 stealth   (1000) stealth   (1000)       79 2024-01-31 21:56:10.000000 dynamic_import-2024.2.13/test/block1/__init__.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.410105 dynamic_import-2024.2.13/test/block_cache/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      269 2024-02-14 00:07:34.000000 dynamic_import-2024.2.13/test/block_cache/__init__.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.410105 dynamic_import-2024.2.13/test/block_nocache/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      277 2024-01-28 12:34:53.000000 dynamic_import-2024.2.13/test/block_nocache/__init__.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3954 2024-02-01 15:33:03.000000 dynamic_import-2024.2.13/test/cache_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3504 2024-02-01 13:40:02.000000 dynamic_import-2024.2.13/test/check_test.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.410105 dynamic_import-2024.2.13/test/conflict/
--rw-r--r--   0 stealth   (1000) stealth   (1000)       60 2024-02-14 00:05:30.000000 dynamic_import-2024.2.13/test/conflict/__init__.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       86 2024-02-14 00:06:23.000000 dynamic_import-2024.2.13/test/conflict/my_func.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       97 2024-02-14 00:06:54.000000 dynamic_import-2024.2.13/test/conflict_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      924 2024-02-01 14:44:06.000000 dynamic_import-2024.2.13/test/conftest.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-02-14 00:17:36.410105 dynamic_import-2024.2.13/test/error_test/
--rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-01-30 21:10:54.000000 dynamic_import-2024.2.13/test/error_test/__init__.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       72 2024-01-30 21:30:02.000000 dynamic_import-2024.2.13/test/error_test/not_init.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2953 2024-02-03 23:06:27.000000 dynamic_import-2024.2.13/test/extract_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1879 2024-01-31 23:35:18.000000 dynamic_import-2024.2.13/test/other_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     4054 2024-02-01 13:42:19.000000 dynamic_import-2024.2.13/test/prep_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1801 2024-02-01 14:06:16.000000 dynamic_import-2024.2.13/test/special_test.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.222427 dynamic_import-2024.5.2/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     7048 2020-02-25 14:17:19.000000 dynamic_import-2024.5.2/LICENSE.txt
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      178 2024-01-31 21:50:28.000000 dynamic_import-2024.5.2/MANIFEST.in
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    14918 2024-05-02 16:24:52.222427 dynamic_import-2024.5.2/PKG-INFO
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     5929 2024-04-03 00:00:34.000000 dynamic_import-2024.5.2/README.rst
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.212427 dynamic_import-2024.5.2/dynamic_import/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      277 2024-01-27 17:35:22.000000 dynamic_import-2024.5.2/dynamic_import/__init__.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3801 2024-05-02 16:18:39.000000 dynamic_import-2024.5.2/dynamic_import/cache.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     4793 2024-01-31 23:26:36.000000 dynamic_import-2024.5.2/dynamic_import/check.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3056 2024-02-13 23:29:08.000000 dynamic_import-2024.5.2/dynamic_import/extract.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3811 2024-04-02 06:10:13.000000 dynamic_import-2024.5.2/dynamic_import/importer.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2947 2024-05-02 16:04:58.000000 dynamic_import-2024.5.2/dynamic_import/module.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     4387 2024-05-02 15:18:24.000000 dynamic_import-2024.5.2/dynamic_import/prep.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1272 2024-04-02 04:34:19.000000 dynamic_import-2024.5.2/dynamic_import/record.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      936 2024-05-02 16:05:36.000000 dynamic_import-2024.5.2/dynamic_import/special.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       21 2024-05-02 15:16:32.000000 dynamic_import-2024.5.2/dynamic_import/version.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.222427 dynamic_import-2024.5.2/dynamic_import.egg-info/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    14918 2024-05-02 16:24:52.000000 dynamic_import-2024.5.2/dynamic_import.egg-info/PKG-INFO
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1315 2024-05-02 16:24:52.000000 dynamic_import-2024.5.2/dynamic_import.egg-info/SOURCES.txt
+-rw-r--r--   0 stealth   (1000) stealth   (1000)        1 2024-05-02 16:24:52.000000 dynamic_import-2024.5.2/dynamic_import.egg-info/dependency_links.txt
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       15 2024-05-02 16:24:52.000000 dynamic_import-2024.5.2/dynamic_import.egg-info/top_level.txt
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.212427 dynamic_import-2024.5.2/example/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      216 2024-01-24 03:59:57.000000 dynamic_import-2024.5.2/example/calling.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.212427 dynamic_import-2024.5.2/example/pkg/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      452 2024-01-31 21:50:28.000000 dynamic_import-2024.5.2/example/pkg/__init__.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.215760 dynamic_import-2024.5.2/example/pkg/classes/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       48 2024-01-05 03:34:55.000000 dynamic_import-2024.5.2/example/pkg/classes/__init__.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.215760 dynamic_import-2024.5.2/example/pkg/functions/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      234 2024-02-01 14:02:20.000000 dynamic_import-2024.5.2/example/pkg/functions/myfunction.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      162 2024-01-05 03:34:44.000000 dynamic_import-2024.5.2/example/pkg/var.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1511 2024-02-01 20:25:33.000000 dynamic_import-2024.5.2/pyproject.toml
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       38 2024-05-02 16:24:52.222427 dynamic_import-2024.5.2/setup.cfg
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       70 2024-01-27 17:20:13.000000 dynamic_import-2024.5.2/setup.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.215760 dynamic_import-2024.5.2/test/
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.215760 dynamic_import-2024.5.2/test/basic/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      173 2024-01-31 21:55:23.000000 dynamic_import-2024.5.2/test/basic/__init__.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       90 2024-01-07 07:52:04.000000 dynamic_import-2024.5.2/test/basic/one.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.215760 dynamic_import-2024.5.2/test/basic/skip/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       49 2024-01-25 18:03:26.000000 dynamic_import-2024.5.2/test/basic/skip/bad-file.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       14 2024-01-30 09:43:20.000000 dynamic_import-2024.5.2/test/basic/skip/bad_all.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.219093 dynamic_import-2024.5.2/test/basic/so/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-01-31 21:46:21.000000 dynamic_import-2024.5.2/test/basic/so/__init__.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.219093 dynamic_import-2024.5.2/test/basic/sub/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      277 2024-02-01 14:03:14.000000 dynamic_import-2024.5.2/test/basic/sub/auto_find.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.219093 dynamic_import-2024.5.2/test/basic/sub/child/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       61 2021-05-01 03:35:14.000000 dynamic_import-2024.5.2/test/basic/sub/child/child.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.219093 dynamic_import-2024.5.2/test/basic/sub/conflict/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       81 2024-01-05 06:46:07.000000 dynamic_import-2024.5.2/test/basic/sub/conflict/__init__.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      119 2021-04-29 23:24:22.000000 dynamic_import-2024.5.2/test/basic/sub/four_five.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       24 2024-01-25 14:28:21.000000 dynamic_import-2024.5.2/test/basic/sub/skip-me.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       63 2021-04-29 23:22:27.000000 dynamic_import-2024.5.2/test/basic/sub/three.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       91 2021-04-29 23:22:47.000000 dynamic_import-2024.5.2/test/basic/two.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.219093 dynamic_import-2024.5.2/test/block/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       60 2024-01-31 21:55:45.000000 dynamic_import-2024.5.2/test/block/__init__.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      151 2024-01-31 21:56:03.000000 dynamic_import-2024.5.2/test/block/block.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.219093 dynamic_import-2024.5.2/test/block1/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       79 2024-01-31 21:56:10.000000 dynamic_import-2024.5.2/test/block1/__init__.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.219093 dynamic_import-2024.5.2/test/block_cache/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      269 2024-05-02 16:06:19.000000 dynamic_import-2024.5.2/test/block_cache/__init__.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.219093 dynamic_import-2024.5.2/test/block_nocache/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      277 2024-01-28 12:34:53.000000 dynamic_import-2024.5.2/test/block_nocache/__init__.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3954 2024-02-01 15:33:03.000000 dynamic_import-2024.5.2/test/cache_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3504 2024-02-01 13:40:02.000000 dynamic_import-2024.5.2/test/check_test.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.219093 dynamic_import-2024.5.2/test/conflict/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       60 2024-05-02 15:24:35.000000 dynamic_import-2024.5.2/test/conflict/__init__.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      143 2024-02-19 06:13:10.000000 dynamic_import-2024.5.2/test/conflict/my_func.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      479 2024-02-19 19:46:24.000000 dynamic_import-2024.5.2/test/conflict_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      924 2024-02-01 14:44:06.000000 dynamic_import-2024.5.2/test/conftest.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-02 16:24:52.219093 dynamic_import-2024.5.2/test/error_test/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-01-30 21:10:54.000000 dynamic_import-2024.5.2/test/error_test/__init__.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       72 2024-01-30 21:30:02.000000 dynamic_import-2024.5.2/test/error_test/not_init.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2953 2024-02-03 23:06:27.000000 dynamic_import-2024.5.2/test/extract_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1879 2024-01-31 23:35:18.000000 dynamic_import-2024.5.2/test/other_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     4054 2024-02-01 13:42:19.000000 dynamic_import-2024.5.2/test/prep_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1265 2024-04-03 04:32:42.000000 dynamic_import-2024.5.2/test/record_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1891 2024-05-02 16:05:16.000000 dynamic_import-2024.5.2/test/special_test.py
```

### Comparing `dynamic_import-2024.2.13/LICENSE.txt` & `dynamic_import-2024.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynamic_import-2024.2.13/PKG-INFO` & `dynamic_import-2024.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_import
-Version: 2024.2.13
+Version: 2024.5.2
 Summary: Let Dynamic Import handle your projects(package) import needs. Enables you to dynamically(lazily) import module as needed on run-time.
 Author: Ritesh
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
@@ -143,21 +143,24 @@
 License-File: LICENSE.txt
 
 |test-status| |downloads|
 
 Dynamic Import
 ==============
 
-Let Dynamic Import handle your projects(package) import needs. Enables you to dynamically(lazily) import module as needed within the project and for external usage on run-time.
+Let Dynamic Import handle your projects(package) import needs. Enables you to dynamically(lazily)
+import module as needed within the project and for external usage on run-time.
 
-* Place ``importer()`` into top ``__init__.py`` file and forget about where variable, function, class, ... are located.
-* Just call ``from <package> import <variable>`` while coding and when end-user calls from your project. All names are accessible at top level, easy to remember.
+* Place ``importer()`` into top ``__init__.py`` file and forget about where
+  variable, function, class, ... are located.
+* Just call ``from <package> import <variable>`` while coding and when end-user calls from your
+  project. All names are accessible at top level, easy to remember.
 * Move/rename file within your project? No problem, auto updates. 
 * Supports ``.py`` and ``.so`` (experimental)
-* Saves memory.
+* Saves memory(for medium to large projects).
 
 Ultimate worry free management comfort as your project grows from small to large.
 
 
 Requires
 --------
 
@@ -274,15 +277,16 @@
 Calling
 _______
 
 
 .. code-block:: python
 
     # ./example/calling.py
-    from pkg import my_var, my_function, MyClass  # import all 3 names regardless of where module is located
+    # import all 3 names regardless of where module is located
+    from pkg import my_var, my_function, MyClass
 
     # or 
     import pkg
 
     MyClass()
     print(my_var, pkg.my_var is my_var) # 3 True
     print(my_function())                # 4
@@ -291,32 +295,37 @@
 
 Note
 ----
     - Only need to call ``importer()`` once inside ``__init__.py`` file.
     - All sub-directories will be scanned for ``.py, .so`` file as ``recursive=True`` by default.
     - Use ``exclude_dir`` to list sub-directories you would like to avoid scanning.
     - You can still use normal static/relative import.
-    - For one word import name you can use string e.g. ``__all__ = 'function'`` vs ``__all__ = ('function',)``
+    - For one word import name you can use string
+      e.g. ``__all__ = 'function'`` vs ``__all__ = ('function',)``
     - All import names must be unique.
     - Cache can be disabled & removed by using ``importer(cache=False)``
     - Cached temporary files are stored in ``./__pycache__/__init__.importer-<python-version>.pyc``
-    - You can move or rename any ``.py`` file within project directory or sub-directory and import will not break.
+    - You can move or rename any ``.py`` file within project directory or sub-directory and 
+      import will not break.
     - Special name e.g: ``__something__`` are ignored. If need to use special name place it 
-      above ``importer()`` e.g: ``__version__ = '1.2.3'; importer()``
+      above ``importer()`` e.g.``__version__ = '1.2.3'; importer()``
     - Using ``from <package> import *`` is not recommended unless you want to load all the modules.
-    - No need to have empty ``__init__.py`` inside sub-directories. Namespace + Package combined into one.
-    - Calling ``dir(<package>)`` enables you to show all importable names without actually loading modules.
-    - Having module name and function name the same is ok! e.g. ``from pkg import my_fun`` while ``./pkg/my_fun.py``
-      and calling `my_fun()` will not conflict with module name. Module will still load in the background.
+    - No need to have empty ``__init__.py`` inside sub-directories. Its "like" Namespace + Package
+      combined into one! but not technically.
+    - Calling ``dir(<package>)`` enables you to show all importable names without loading modules.
 
 
 Experimental
 ------------
-    - ``importer()`` also works with certain ``.cpython-<...>.so`` ``.abi3.so`` file (tested with cython created ``.so``).
-    - ``.so`` should not contain any function/class that auto-run on import, e.g: ``run_something()``
+    - Having module name and function name the same is ok! e.g. ``from pkg import my_fun`` while
+      ``./pkg/my_fun.py`` and calling ``my_fun()`` will not conflict with module name. Module will
+      still load in the background.
+    - ``importer()`` also works with certain ``.cpython-<...>.so`` ``.abi3.so`` file
+      (only tested with cython created ``*.so``).
+    - ``.so`` should not contain any function/class that auto-run on import e.g.``run_something()``
     - Visit `Liburing`_ to see project using Dynamic Import with ``.so`` files in action.
 
 
 License
 -------
 Free, Public Domain (CC0). `Read more`_
```

### Comparing `dynamic_import-2024.2.13/README.rst` & `dynamic_import-2024.5.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 |test-status| |downloads|
 
 Dynamic Import
 ==============
 
-Let Dynamic Import handle your projects(package) import needs. Enables you to dynamically(lazily) import module as needed within the project and for external usage on run-time.
+Let Dynamic Import handle your projects(package) import needs. Enables you to dynamically(lazily)
+import module as needed within the project and for external usage on run-time.
 
-* Place ``importer()`` into top ``__init__.py`` file and forget about where variable, function, class, ... are located.
-* Just call ``from <package> import <variable>`` while coding and when end-user calls from your project. All names are accessible at top level, easy to remember.
+* Place ``importer()`` into top ``__init__.py`` file and forget about where
+  variable, function, class, ... are located.
+* Just call ``from <package> import <variable>`` while coding and when end-user calls from your
+  project. All names are accessible at top level, easy to remember.
 * Move/rename file within your project? No problem, auto updates. 
 * Supports ``.py`` and ``.so`` (experimental)
-* Saves memory.
+* Saves memory(for medium to large projects).
 
 Ultimate worry free management comfort as your project grows from small to large.
 
 
 Requires
 --------
 
@@ -130,15 +133,16 @@
 Calling
 _______
 
 
 .. code-block:: python
 
     # ./example/calling.py
-    from pkg import my_var, my_function, MyClass  # import all 3 names regardless of where module is located
+    # import all 3 names regardless of where module is located
+    from pkg import my_var, my_function, MyClass
 
     # or 
     import pkg
 
     MyClass()
     print(my_var, pkg.my_var is my_var) # 3 True
     print(my_function())                # 4
@@ -147,32 +151,37 @@
 
 Note
 ----
     - Only need to call ``importer()`` once inside ``__init__.py`` file.
     - All sub-directories will be scanned for ``.py, .so`` file as ``recursive=True`` by default.
     - Use ``exclude_dir`` to list sub-directories you would like to avoid scanning.
     - You can still use normal static/relative import.
-    - For one word import name you can use string e.g. ``__all__ = 'function'`` vs ``__all__ = ('function',)``
+    - For one word import name you can use string
+      e.g. ``__all__ = 'function'`` vs ``__all__ = ('function',)``
     - All import names must be unique.
     - Cache can be disabled & removed by using ``importer(cache=False)``
     - Cached temporary files are stored in ``./__pycache__/__init__.importer-<python-version>.pyc``
-    - You can move or rename any ``.py`` file within project directory or sub-directory and import will not break.
+    - You can move or rename any ``.py`` file within project directory or sub-directory and 
+      import will not break.
     - Special name e.g: ``__something__`` are ignored. If need to use special name place it 
-      above ``importer()`` e.g: ``__version__ = '1.2.3'; importer()``
+      above ``importer()`` e.g.``__version__ = '1.2.3'; importer()``
     - Using ``from <package> import *`` is not recommended unless you want to load all the modules.
-    - No need to have empty ``__init__.py`` inside sub-directories. Namespace + Package combined into one.
-    - Calling ``dir(<package>)`` enables you to show all importable names without actually loading modules.
-    - Having module name and function name the same is ok! e.g. ``from pkg import my_fun`` while ``./pkg/my_fun.py``
-      and calling `my_fun()` will not conflict with module name. Module will still load in the background.
+    - No need to have empty ``__init__.py`` inside sub-directories. Its "like" Namespace + Package
+      combined into one! but not technically.
+    - Calling ``dir(<package>)`` enables you to show all importable names without loading modules.
 
 
 Experimental
 ------------
-    - ``importer()`` also works with certain ``.cpython-<...>.so`` ``.abi3.so`` file (tested with cython created ``.so``).
-    - ``.so`` should not contain any function/class that auto-run on import, e.g: ``run_something()``
+    - Having module name and function name the same is ok! e.g. ``from pkg import my_fun`` while
+      ``./pkg/my_fun.py`` and calling ``my_fun()`` will not conflict with module name. Module will
+      still load in the background.
+    - ``importer()`` also works with certain ``.cpython-<...>.so`` ``.abi3.so`` file
+      (only tested with cython created ``*.so``).
+    - ``.so`` should not contain any function/class that auto-run on import e.g.``run_something()``
     - Visit `Liburing`_ to see project using Dynamic Import with ``.so`` files in action.
 
 
 License
 -------
 Free, Public Domain (CC0). `Read more`_
```

### Comparing `dynamic_import-2024.2.13/dynamic_import/cache.py` & `dynamic_import-2024.5.2/dynamic_import/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
             version:      str
             return:       None
 
         Example
             >>> dump_cache('/path/pkg/__pycache__/__init__.importer-312', ...)
     '''
     with open(cache_path, 'w+b') as file:
-        dump((version, recursive, exclude_file, exclude_dir, dir_mtime, data), file, MARSHAL_VERSION)
+        dump((version, recursive, exclude_file, exclude_dir, dir_mtime, data),
+             file, MARSHAL_VERSION)
 
 
 def load_cache(cache_path, recursive, exclude_file, exclude_dir, version):
     ''' Load cached file
 
         Type
             cache_path:   str
@@ -79,15 +80,16 @@
             return:       any
 
         Example
             >>> load_cache('/path/pkg/__pycache__/__init__.importer-312.pyc')
     '''
     try:
         with open(cache_path, 'rb') as file:
-            cached_version, cached_recursive, cached_exclude_file, cached_exclude_dir, dir_mtime, data = load(file)
+            cached_version, cached_recursive, cached_exclude_file,
+            cached_exclude_dir, dir_mtime, data = load(file)
 
             if version != cached_version:
                 return None  # check if Dynamic Import version has changed!
             elif recursive != cached_recursive:
                 return None  # check if `recursive` has changed!'
             elif exclude_file != cached_exclude_file:
                 return None  # check if `exclude_file` has changed!
```

### Comparing `dynamic_import-2024.2.13/dynamic_import/check.py` & `dynamic_import-2024.5.2/dynamic_import/check.py`

 * *Files identical despite different names*

### Comparing `dynamic_import-2024.2.13/dynamic_import/extract.py` & `dynamic_import-2024.5.2/dynamic_import/extract.py`

 * *Files identical despite different names*

### Comparing `dynamic_import-2024.2.13/dynamic_import/importer.py` & `dynamic_import-2024.5.2/dynamic_import/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from os import remove
 from sys import _getframe, modules
 from os.path import exists, split
 from .module import Module
 from .check import importer_called, exclude_file_check, exclude_dir_check
 from .cache import pkg_cache_path, create_cache_dir, dump_cache, load_cache
 from .prep import prep_package
+from .record import add_record
 from .version import version
 
 
 __all__ = 'importer',
 
 
 def importer(*, cache=True, recursive=True, exclude_file=None, exclude_dir=None):
@@ -75,14 +76,15 @@
                 else:
                     remove(cache_path)
                     continue
             else:
                 info, dir_mtime = prep_package(pkg_name, pkg_path, recursive, exclude_file_path, exclude_dir_path)
                 create_cache_dir(cache_path)
                 dump_cache(cache_path, info, recursive, exclude_file_path, exclude_dir_path, dir_mtime, version)
+                add_record(pkg_name, cache_path)
                 break
     else:
         if exists(cache_path):
             remove(cache_path)
         info, _ = prep_package(pkg_name, pkg_path, recursive, exclude_file_path, exclude_dir_path)
 
     module = modules.get(pkg_name)
```

### Comparing `dynamic_import-2024.2.13/dynamic_import/module.py` & `dynamic_import-2024.5.2/dynamic_import/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 args:    Tuple[any]
                 kwargs:  Dict[str, any]
                 return:  None
         '''
         super().__init__(package, None, *args, **kwargs)
         self.__PACKAGE__ = package
         self.__INFO__ = info
-        # note: ^ this needs to mimic magic method name since those are made to raise error
+        # note: ^ these needs to mimic magic method name since those are made to raise error
 
         # only include special name from previous module, all other names should be
         # imported through this `Module`
         for key, value in module.__dict__.items():
             if (key[0:2] == '__' == key[-2:]) and (key[2] != '_' != key[-3]):
                 self.__dict__[key] = value  # only update `__special__` names
         setattr(self, '__all__', (*self.__dict__, *self.__INFO__))
```

### Comparing `dynamic_import-2024.2.13/dynamic_import/prep.py` & `dynamic_import-2024.5.2/dynamic_import/prep.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,20 @@
 
         Example
             >>> prep_package('pkg', 'path/pkg/', True, [], [])
             {'one': ('pkg.module', 'pkg/module.py', ('one', ...), 123.45), ...}, {'pkg/': 123.45, ...}
     '''
     info = {}
     dir_mtime = {}
-    for module, file_path, mtime in prep_files(pkg_name, pkg_path, recursive, dir_mtime, exclude_file, exclude_dir):
+    for module, file_path, mtime in prep_files(pkg_name,
+                                               pkg_path,
+                                               recursive,
+                                               dir_mtime,
+                                               exclude_file,
+                                               exclude_dir):
         for var, variables in prep_variables(module, file_path):
             info[var] = (module, file_path, variables, mtime)
     return info, dir_mtime
 
 
 def prep_files(pkg_name, pkg_path, recursive, dir_mtime, exclude_file, exclude_dir):
     ''' Prepare python files and module names
@@ -74,16 +79,16 @@
                     dir_mtime[root_path] = stat(root_path).st_mtime  # cached called
                     mtime = stat(file_path).st_mtime
 
                     if file == '__init__.py':
                         yield f'{module_name}', file_path, mtime
                     else:
                         yield f'{module_name}.{file.split(".")[0]}', file_path, mtime
-                        # ('pkg.sub.module', '/path/pkg/sub/module.py', 123.45)
-                        # ('pkg.sub.module', '/path/pkg/sub/module.cpython-312-x86_64-linux-gnu.so', 123.45)
+                        # ('pkg.sub.module', '/pkg/sub/module.py', 123.45)
+                        # ('pkg.sub.module', '/pkg/sub/module*.so', 123.45)
         if not recursive:
             break
 
 
 def prep_variables(module_name, file_path):
     ''' Prepare `__all__` variable names
```

### Comparing `dynamic_import-2024.2.13/dynamic_import/special.py` & `dynamic_import-2024.5.2/dynamic_import/special.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,12 +17,12 @@
             ...     ValueError: special name like '__name__' is not supported
 
         Note
             - special name are ignored by default. e.g: `__something__`
             - if `error=True` will raise exception if special name is found.
     '''
     for name in iterable:
-        if (name[0:2] == '__' == name[-2:]) and (name[2] != '_' != name[-3]):
+        if len(name) > 4 and (name[0:2] == '__' == name[-2:]) and (name[2] != '_' != name[-3]):
             if error:
                 raise ValueError(f'special name like {name!r} is not supported')
             continue
         yield name
```

### Comparing `dynamic_import-2024.2.13/dynamic_import.egg-info/PKG-INFO` & `dynamic_import-2024.5.2/dynamic_import.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_import
-Version: 2024.2.13
+Version: 2024.5.2
 Summary: Let Dynamic Import handle your projects(package) import needs. Enables you to dynamically(lazily) import module as needed on run-time.
 Author: Ritesh
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
@@ -143,21 +143,24 @@
 License-File: LICENSE.txt
 
 |test-status| |downloads|
 
 Dynamic Import
 ==============
 
-Let Dynamic Import handle your projects(package) import needs. Enables you to dynamically(lazily) import module as needed within the project and for external usage on run-time.
+Let Dynamic Import handle your projects(package) import needs. Enables you to dynamically(lazily)
+import module as needed within the project and for external usage on run-time.
 
-* Place ``importer()`` into top ``__init__.py`` file and forget about where variable, function, class, ... are located.
-* Just call ``from <package> import <variable>`` while coding and when end-user calls from your project. All names are accessible at top level, easy to remember.
+* Place ``importer()`` into top ``__init__.py`` file and forget about where
+  variable, function, class, ... are located.
+* Just call ``from <package> import <variable>`` while coding and when end-user calls from your
+  project. All names are accessible at top level, easy to remember.
 * Move/rename file within your project? No problem, auto updates. 
 * Supports ``.py`` and ``.so`` (experimental)
-* Saves memory.
+* Saves memory(for medium to large projects).
 
 Ultimate worry free management comfort as your project grows from small to large.
 
 
 Requires
 --------
 
@@ -274,15 +277,16 @@
 Calling
 _______
 
 
 .. code-block:: python
 
     # ./example/calling.py
-    from pkg import my_var, my_function, MyClass  # import all 3 names regardless of where module is located
+    # import all 3 names regardless of where module is located
+    from pkg import my_var, my_function, MyClass
 
     # or 
     import pkg
 
     MyClass()
     print(my_var, pkg.my_var is my_var) # 3 True
     print(my_function())                # 4
@@ -291,32 +295,37 @@
 
 Note
 ----
     - Only need to call ``importer()`` once inside ``__init__.py`` file.
     - All sub-directories will be scanned for ``.py, .so`` file as ``recursive=True`` by default.
     - Use ``exclude_dir`` to list sub-directories you would like to avoid scanning.
     - You can still use normal static/relative import.
-    - For one word import name you can use string e.g. ``__all__ = 'function'`` vs ``__all__ = ('function',)``
+    - For one word import name you can use string
+      e.g. ``__all__ = 'function'`` vs ``__all__ = ('function',)``
     - All import names must be unique.
     - Cache can be disabled & removed by using ``importer(cache=False)``
     - Cached temporary files are stored in ``./__pycache__/__init__.importer-<python-version>.pyc``
-    - You can move or rename any ``.py`` file within project directory or sub-directory and import will not break.
+    - You can move or rename any ``.py`` file within project directory or sub-directory and 
+      import will not break.
     - Special name e.g: ``__something__`` are ignored. If need to use special name place it 
-      above ``importer()`` e.g: ``__version__ = '1.2.3'; importer()``
+      above ``importer()`` e.g.``__version__ = '1.2.3'; importer()``
     - Using ``from <package> import *`` is not recommended unless you want to load all the modules.
-    - No need to have empty ``__init__.py`` inside sub-directories. Namespace + Package combined into one.
-    - Calling ``dir(<package>)`` enables you to show all importable names without actually loading modules.
-    - Having module name and function name the same is ok! e.g. ``from pkg import my_fun`` while ``./pkg/my_fun.py``
-      and calling `my_fun()` will not conflict with module name. Module will still load in the background.
+    - No need to have empty ``__init__.py`` inside sub-directories. Its "like" Namespace + Package
+      combined into one! but not technically.
+    - Calling ``dir(<package>)`` enables you to show all importable names without loading modules.
 
 
 Experimental
 ------------
-    - ``importer()`` also works with certain ``.cpython-<...>.so`` ``.abi3.so`` file (tested with cython created ``.so``).
-    - ``.so`` should not contain any function/class that auto-run on import, e.g: ``run_something()``
+    - Having module name and function name the same is ok! e.g. ``from pkg import my_fun`` while
+      ``./pkg/my_fun.py`` and calling ``my_fun()`` will not conflict with module name. Module will
+      still load in the background.
+    - ``importer()`` also works with certain ``.cpython-<...>.so`` ``.abi3.so`` file
+      (only tested with cython created ``*.so``).
+    - ``.so`` should not contain any function/class that auto-run on import e.g.``run_something()``
     - Visit `Liburing`_ to see project using Dynamic Import with ``.so`` files in action.
 
 
 License
 -------
 Free, Public Domain (CC0). `Read more`_
```

### Comparing `dynamic_import-2024.2.13/dynamic_import.egg-info/SOURCES.txt` & `dynamic_import-2024.5.2/dynamic_import.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 dynamic_import/__init__.py
 dynamic_import/cache.py
 dynamic_import/check.py
 dynamic_import/extract.py
 dynamic_import/importer.py
 dynamic_import/module.py
 dynamic_import/prep.py
+dynamic_import/record.py
 dynamic_import/special.py
 dynamic_import/version.py
 dynamic_import.egg-info/PKG-INFO
 dynamic_import.egg-info/SOURCES.txt
 dynamic_import.egg-info/dependency_links.txt
 dynamic_import.egg-info/top_level.txt
 example/calling.py
@@ -24,14 +25,15 @@
 test/cache_test.py
 test/check_test.py
 test/conflict_test.py
 test/conftest.py
 test/extract_test.py
 test/other_test.py
 test/prep_test.py
+test/record_test.py
 test/special_test.py
 test/basic/__init__.py
 test/basic/one.py
 test/basic/two.py
 test/basic/skip/bad-file.py
 test/basic/skip/bad_all.py
 test/basic/so/__init__.py
```

### Comparing `dynamic_import-2024.2.13/pyproject.toml` & `dynamic_import-2024.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dynamic_import-2024.2.13/test/cache_test.py` & `dynamic_import-2024.5.2/test/cache_test.py`

 * *Files identical despite different names*

### Comparing `dynamic_import-2024.2.13/test/check_test.py` & `dynamic_import-2024.5.2/test/check_test.py`

 * *Files identical despite different names*

### Comparing `dynamic_import-2024.2.13/test/conftest.py` & `dynamic_import-2024.5.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `dynamic_import-2024.2.13/test/extract_test.py` & `dynamic_import-2024.5.2/test/extract_test.py`

 * *Files identical despite different names*

### Comparing `dynamic_import-2024.2.13/test/other_test.py` & `dynamic_import-2024.5.2/test/other_test.py`

 * *Files identical despite different names*

### Comparing `dynamic_import-2024.2.13/test/prep_test.py` & `dynamic_import-2024.5.2/test/prep_test.py`

 * *Files identical despite different names*

### Comparing `dynamic_import-2024.2.13/test/special_test.py` & `dynamic_import-2024.5.2/test/special_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import sys
 import pytest
 import pathlib
 from dynamic_import.special import special
 
 
 def test_special():
-    my_list = ['first', '__name__', '_name', 'name_', 'name', 'name__', '__name', '___name___', '', 'last']
-    result = ('first', '_name', 'name_', 'name', 'name__', '__name', '___name___', '', 'last')
+    my_list = ['first', '__name__', '_name', 'name_', 'name', 'name__', '__name', '___name___',
+               '', 'last', '__q__', '____', '___', '__', '_']
+    result = ('first', '_name', 'name_', 'name', 'name__', '__name', '___name___',
+              '', 'last', '____', '___', '__', '_')
     assert tuple(special(my_list)) == result
 
     with pytest.raises(ValueError, match="special name like '__name__' is not supported"):
         [_ for _ in special(my_list, error=True)]
 
 
 def test_block():
```

