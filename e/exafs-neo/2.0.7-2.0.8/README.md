# Comparing `tmp/exafs_neo-2.0.7.tar.gz` & `tmp/exafs_neo-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exafs_neo-2.0.7.tar", last modified: Fri Apr 26 21:42:40 2024, max compression
+gzip compressed data, was "exafs_neo-2.0.8.tar", last modified: Thu May  2 01:38:04 2024, max compression
```

## Comparing `exafs_neo-2.0.7.tar` & `exafs_neo-2.0.8.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.966621 exafs_neo-2.0.7/
--rw-r--r--   0 andy       (501) staff       (20)    35198 2021-08-14 12:28:51.000000 exafs_neo-2.0.7/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)     5782 2024-04-26 21:42:40.966747 exafs_neo-2.0.7/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     5337 2024-04-24 22:21:42.000000 exafs_neo-2.0.7/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.958024 exafs_neo-2.0.7/exafs_neo/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-03 07:16:06.000000 exafs_neo-2.0.7/exafs_neo/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)      152 2024-04-26 21:42:38.000000 exafs_neo-2.0.7/exafs_neo/_version.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.959884 exafs_neo-2.0.7/exafs_neo/analysis/
--rw-r--r--   0 andy       (501) staff       (20)    28217 2024-04-02 02:45:54.000000 exafs_neo-2.0.7/exafs_neo/analysis/EXAFS_Analysis.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-19 04:33:48.000000 exafs_neo-2.0.7/exafs_neo/analysis/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)    20093 2024-03-19 06:15:52.000000 exafs_neo-2.0.7/exafs_neo/analysis/larch_score.py
--rw-r--r--   0 andy       (501) staff       (20)     4478 2024-04-26 06:10:02.000000 exafs_neo-2.0.7/exafs_neo/exafs.py
--rw-r--r--   0 andy       (501) staff       (20)     5812 2024-04-02 02:57:21.000000 exafs_neo-2.0.7/exafs_neo/exafs_pop.py
--rw-r--r--   0 andy       (501) staff       (20)     5293 2024-04-25 22:22:56.000000 exafs_neo-2.0.7/exafs_neo/exafsfileobj.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.962020 exafs_neo-2.0.7/exafs_neo/gui/
--rw-r--r--   0 andy       (501) staff       (20)     3079 2024-03-19 04:34:51.000000 exafs_neo-2.0.7/exafs_neo/gui/Analysis_plot.py
--rw-r--r--   0 andy       (501) staff       (20)     5721 2024-03-18 17:12:48.000000 exafs_neo-2.0.7/exafs_neo/gui/Background_plot.py
--rw-r--r--   0 andy       (501) staff       (20)     2124 2024-03-18 17:11:48.000000 exafs_neo-2.0.7/exafs_neo/gui/Console.py
--rw-r--r--   0 andy       (501) staff       (20)     1575 2024-04-20 17:28:50.000000 exafs_neo-2.0.7/exafs_neo/gui/Misc_Function.py
--rw-r--r--   0 andy       (501) staff       (20)    56143 2024-04-26 06:57:47.000000 exafs_neo-2.0.7/exafs_neo/gui/XAFS_GUI.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-18 05:23:32.000000 exafs_neo-2.0.7/exafs_neo/gui/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     3268 2024-03-18 17:10:18.000000 exafs_neo-2.0.7/exafs_neo/gui/feff_folder_larch.py
--rw-r--r--   0 andy       (501) staff       (20)      265 2023-05-16 01:15:35.000000 exafs_neo-2.0.7/exafs_neo/gui/first_shell_fits.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.962924 exafs_neo-2.0.7/exafs_neo/gui/media/
--rw-r--r--   0 andy       (501) staff       (20)      539 2023-07-01 21:09:31.000000 exafs_neo-2.0.7/exafs_neo/gui/media/Citation
--rw-r--r--   0 andy       (501) staff       (20)    35198 2024-04-02 19:10:46.000000 exafs_neo-2.0.7/exafs_neo/gui/media/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)     3848 2021-08-14 12:28:51.000000 exafs_neo-2.0.7/exafs_neo/gui/media/icon.png
--rw-r--r--   0 andy       (501) staff       (20)      983 2024-04-02 03:00:16.000000 exafs_neo-2.0.7/exafs_neo/helper.py
--rw-r--r--   0 andy       (501) staff       (20)     3909 2024-04-02 03:07:35.000000 exafs_neo-2.0.7/exafs_neo/individual.py
--rw-r--r--   0 andy       (501) staff       (20)     6206 2024-04-02 03:12:20.000000 exafs_neo-2.0.7/exafs_neo/ini_parser.py
--rwxr-xr-x   0 andy       (501) staff       (20)     1317 2024-04-02 03:13:29.000000 exafs_neo-2.0.7/exafs_neo/input_arg.py
--rw-r--r--   0 andy       (501) staff       (20)     9291 2024-04-26 05:59:11.000000 exafs_neo-2.0.7/exafs_neo/neoCrossOver.py
--rw-r--r--   0 andy       (501) staff       (20)     4310 2024-04-26 06:10:55.000000 exafs_neo-2.0.7/exafs_neo/neoFilePars.py
--rw-r--r--   0 andy       (501) staff       (20)     9294 2024-04-26 06:13:20.000000 exafs_neo-2.0.7/exafs_neo/neoMutator.py
--rw-r--r--   0 andy       (501) staff       (20)    14134 2024-04-26 06:13:35.000000 exafs_neo-2.0.7/exafs_neo/neoPars.py
--rw-r--r--   0 andy       (501) staff       (20)     3289 2024-04-26 05:59:28.000000 exafs_neo-2.0.7/exafs_neo/neoResult.py
--rw-r--r--   0 andy       (501) staff       (20)     3904 2024-04-24 02:04:22.000000 exafs_neo-2.0.7/exafs_neo/neoSelector.py
--rw-r--r--   0 andy       (501) staff       (20)     3835 2024-04-25 02:28:34.000000 exafs_neo-2.0.7/exafs_neo/neoSolver.py
--rwxr-xr-x   0 andy       (501) staff       (20)     5748 2024-04-02 05:25:47.000000 exafs_neo-2.0.7/exafs_neo/parser.py
--rw-r--r--   0 andy       (501) staff       (20)     2953 2024-04-02 05:26:13.000000 exafs_neo-2.0.7/exafs_neo/pathObj.py
--rw-r--r--   0 andy       (501) staff       (20)     5121 2024-04-02 03:36:53.000000 exafs_neo-2.0.7/exafs_neo/pathrange.py
--rw-r--r--   0 andy       (501) staff       (20)     1321 2024-04-02 03:39:27.000000 exafs_neo-2.0.7/exafs_neo/pathrange_file.py
--rw-r--r--   0 andy       (501) staff       (20)    19175 2024-04-02 05:26:30.000000 exafs_neo-2.0.7/exafs_neo/utils.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.959257 exafs_neo-2.0.7/exafs_neo.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)     5782 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     1529 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       99 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/entry_points.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-02-18 07:51:41.000000 exafs_neo-2.0.7/exafs_neo.egg-info/not-zip-safe
--rw-r--r--   0 andy       (501) staff       (20)       40 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)       16 2024-04-26 21:42:40.000000 exafs_neo-2.0.7/exafs_neo.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)       79 2024-04-26 21:42:40.966982 exafs_neo-2.0.7/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)     1240 2024-04-19 05:22:39.000000 exafs_neo-2.0.7/setup.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-26 21:42:40.966379 exafs_neo-2.0.7/tests/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-17 22:01:17.000000 exafs_neo-2.0.7/tests/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     4089 2024-03-23 20:03:07.000000 exafs_neo-2.0.7/tests/test_EXAFS_analysis.py
--rw-r--r--   0 andy       (501) staff       (20)     1589 2024-04-25 05:22:20.000000 exafs_neo-2.0.7/tests/test_exafs_fileobj.py
--rw-r--r--   0 andy       (501) staff       (20)     3857 2024-03-23 20:01:49.000000 exafs_neo-2.0.7/tests/test_exafs_pars.py
--rw-r--r--   0 andy       (501) staff       (20)     2280 2024-03-20 02:02:00.000000 exafs_neo-2.0.7/tests/test_exafs_pathObj.py
--rw-r--r--   0 andy       (501) staff       (20)     1573 2024-02-03 07:05:06.000000 exafs_neo-2.0.7/tests/test_exafs_pathrange.py
--rw-r--r--   0 andy       (501) staff       (20)     1053 2024-03-20 03:41:05.000000 exafs_neo-2.0.7/tests/test_individual.py
--rw-r--r--   0 andy       (501) staff       (20)      514 2024-03-17 20:09:18.000000 exafs_neo-2.0.7/tests/test_ini_parser.py
--rw-r--r--   0 andy       (501) staff       (20)     3385 2024-03-23 20:03:36.000000 exafs_neo-2.0.7/tests/test_larchscore.py
--rw-r--r--   0 andy       (501) staff       (20)      976 2024-03-23 23:13:20.000000 exafs_neo-2.0.7/tests/test_neo_pop.py
--rw-r--r--   0 andy       (501) staff       (20)     5754 2024-03-31 00:14:43.000000 exafs_neo-2.0.7/tests/test_neocrossover.py
--rw-r--r--   0 andy       (501) staff       (20)     3771 2024-04-03 00:18:39.000000 exafs_neo-2.0.7/tests/test_neomutator.py
--rw-r--r--   0 andy       (501) staff       (20)     3725 2024-04-24 06:01:42.000000 exafs_neo-2.0.7/tests/test_neosolver.py
--rw-r--r--   0 andy       (501) staff       (20)      338 2024-02-18 20:02:49.000000 exafs_neo-2.0.7/tests/test_utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 01:38:04.772784 exafs_neo-2.0.8/
+-rw-r--r--   0 andy       (501) staff       (20)    35198 2021-08-14 12:28:51.000000 exafs_neo-2.0.8/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)     6114 2024-05-02 01:38:04.772710 exafs_neo-2.0.8/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     5554 2024-05-02 01:37:02.000000 exafs_neo-2.0.8/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 01:38:04.761391 exafs_neo-2.0.8/exafs_neo/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-03 07:16:06.000000 exafs_neo-2.0.8/exafs_neo/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)      152 2024-05-02 01:37:38.000000 exafs_neo-2.0.8/exafs_neo/_version.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 01:38:04.763977 exafs_neo-2.0.8/exafs_neo/analysis/
+-rw-r--r--   0 andy       (501) staff       (20)    28217 2024-04-02 02:45:54.000000 exafs_neo-2.0.8/exafs_neo/analysis/EXAFS_Analysis.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-19 04:33:48.000000 exafs_neo-2.0.8/exafs_neo/analysis/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)    20093 2024-03-19 06:15:52.000000 exafs_neo-2.0.8/exafs_neo/analysis/larch_score.py
+-rw-r--r--   0 andy       (501) staff       (20)     4369 2024-04-27 18:27:46.000000 exafs_neo-2.0.8/exafs_neo/exafs.py
+-rw-r--r--   0 andy       (501) staff       (20)     5812 2024-04-02 02:57:21.000000 exafs_neo-2.0.8/exafs_neo/exafs_pop.py
+-rw-r--r--   0 andy       (501) staff       (20)     5293 2024-04-25 22:22:56.000000 exafs_neo-2.0.8/exafs_neo/exafsfileobj.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 01:38:04.766173 exafs_neo-2.0.8/exafs_neo/gui/
+-rw-r--r--   0 andy       (501) staff       (20)     3079 2024-03-19 04:34:51.000000 exafs_neo-2.0.8/exafs_neo/gui/Analysis_plot.py
+-rw-r--r--   0 andy       (501) staff       (20)     5721 2024-03-18 17:12:48.000000 exafs_neo-2.0.8/exafs_neo/gui/Background_plot.py
+-rw-r--r--   0 andy       (501) staff       (20)     2124 2024-03-18 17:11:48.000000 exafs_neo-2.0.8/exafs_neo/gui/Console.py
+-rw-r--r--   0 andy       (501) staff       (20)     1575 2024-04-20 17:28:50.000000 exafs_neo-2.0.8/exafs_neo/gui/Misc_Function.py
+-rw-r--r--   0 andy       (501) staff       (20)    58748 2024-05-02 01:11:19.000000 exafs_neo-2.0.8/exafs_neo/gui/XAFS_GUI.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-18 05:23:32.000000 exafs_neo-2.0.8/exafs_neo/gui/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     3268 2024-03-18 17:10:18.000000 exafs_neo-2.0.8/exafs_neo/gui/feff_folder_larch.py
+-rw-r--r--   0 andy       (501) staff       (20)      265 2023-05-16 01:15:35.000000 exafs_neo-2.0.8/exafs_neo/gui/first_shell_fits.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 01:38:04.767535 exafs_neo-2.0.8/exafs_neo/gui/media/
+-rw-r--r--   0 andy       (501) staff       (20)      539 2023-07-01 21:09:31.000000 exafs_neo-2.0.8/exafs_neo/gui/media/Citation
+-rw-r--r--   0 andy       (501) staff       (20)    35198 2024-04-02 19:10:46.000000 exafs_neo-2.0.8/exafs_neo/gui/media/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)     3848 2021-08-14 12:28:51.000000 exafs_neo-2.0.8/exafs_neo/gui/media/icon.png
+-rw-r--r--   0 andy       (501) staff       (20)      983 2024-04-02 03:00:16.000000 exafs_neo-2.0.8/exafs_neo/helper.py
+-rw-r--r--   0 andy       (501) staff       (20)     3909 2024-04-02 03:07:35.000000 exafs_neo-2.0.8/exafs_neo/individual.py
+-rw-r--r--   0 andy       (501) staff       (20)     6206 2024-04-02 03:12:20.000000 exafs_neo-2.0.8/exafs_neo/ini_parser.py
+-rwxr-xr-x   0 andy       (501) staff       (20)     1317 2024-04-02 03:13:29.000000 exafs_neo-2.0.8/exafs_neo/input_arg.py
+-rw-r--r--   0 andy       (501) staff       (20)     9292 2024-05-02 00:39:42.000000 exafs_neo-2.0.8/exafs_neo/neoCrossOver.py
+-rw-r--r--   0 andy       (501) staff       (20)     4298 2024-04-26 22:42:06.000000 exafs_neo-2.0.8/exafs_neo/neoFilePars.py
+-rw-r--r--   0 andy       (501) staff       (20)     8358 2024-04-27 20:51:47.000000 exafs_neo-2.0.8/exafs_neo/neoMutator.py
+-rw-r--r--   0 andy       (501) staff       (20)    14134 2024-04-26 06:13:35.000000 exafs_neo-2.0.8/exafs_neo/neoPars.py
+-rw-r--r--   0 andy       (501) staff       (20)     3289 2024-04-26 22:42:36.000000 exafs_neo-2.0.8/exafs_neo/neoResult.py
+-rw-r--r--   0 andy       (501) staff       (20)     3907 2024-04-27 20:50:59.000000 exafs_neo-2.0.8/exafs_neo/neoSelector.py
+-rw-r--r--   0 andy       (501) staff       (20)     5393 2024-04-27 20:51:06.000000 exafs_neo-2.0.8/exafs_neo/neoSolver.py
+-rwxr-xr-x   0 andy       (501) staff       (20)     5748 2024-04-02 05:25:47.000000 exafs_neo-2.0.8/exafs_neo/parser.py
+-rw-r--r--   0 andy       (501) staff       (20)     2953 2024-04-02 05:26:13.000000 exafs_neo-2.0.8/exafs_neo/pathObj.py
+-rw-r--r--   0 andy       (501) staff       (20)     5121 2024-04-02 03:36:53.000000 exafs_neo-2.0.8/exafs_neo/pathrange.py
+-rw-r--r--   0 andy       (501) staff       (20)     1321 2024-04-02 03:39:27.000000 exafs_neo-2.0.8/exafs_neo/pathrange_file.py
+-rw-r--r--   0 andy       (501) staff       (20)    19774 2024-04-28 01:05:35.000000 exafs_neo-2.0.8/exafs_neo/utils.py
+-rw-r--r--   0 andy       (501) staff       (20)     3574 2024-05-02 01:18:18.000000 exafs_neo-2.0.8/exafs_neo/utils_mapping.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 01:38:04.772348 exafs_neo-2.0.8/exafs_neo.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)     6114 2024-05-02 01:38:04.000000 exafs_neo-2.0.8/exafs_neo.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     1556 2024-05-02 01:38:04.000000 exafs_neo-2.0.8/exafs_neo.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-02 01:38:04.000000 exafs_neo-2.0.8/exafs_neo.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       99 2024-05-02 01:38:04.000000 exafs_neo-2.0.8/exafs_neo.egg-info/entry_points.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-02-18 07:51:41.000000 exafs_neo-2.0.8/exafs_neo.egg-info/not-zip-safe
+-rw-r--r--   0 andy       (501) staff       (20)       40 2024-05-02 01:38:04.000000 exafs_neo-2.0.8/exafs_neo.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)       16 2024-05-02 01:38:04.000000 exafs_neo-2.0.8/exafs_neo.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)       79 2024-05-02 01:38:04.773086 exafs_neo-2.0.8/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)     1240 2024-04-19 05:22:39.000000 exafs_neo-2.0.8/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-02 01:38:04.771810 exafs_neo-2.0.8/tests/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-17 22:01:17.000000 exafs_neo-2.0.8/tests/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     4089 2024-03-23 20:03:07.000000 exafs_neo-2.0.8/tests/test_EXAFS_analysis.py
+-rw-r--r--   0 andy       (501) staff       (20)     1589 2024-04-25 05:22:20.000000 exafs_neo-2.0.8/tests/test_exafs_fileobj.py
+-rw-r--r--   0 andy       (501) staff       (20)     3857 2024-03-23 20:01:49.000000 exafs_neo-2.0.8/tests/test_exafs_pars.py
+-rw-r--r--   0 andy       (501) staff       (20)     2280 2024-03-20 02:02:00.000000 exafs_neo-2.0.8/tests/test_exafs_pathObj.py
+-rw-r--r--   0 andy       (501) staff       (20)     1573 2024-02-03 07:05:06.000000 exafs_neo-2.0.8/tests/test_exafs_pathrange.py
+-rw-r--r--   0 andy       (501) staff       (20)     1053 2024-03-20 03:41:05.000000 exafs_neo-2.0.8/tests/test_individual.py
+-rw-r--r--   0 andy       (501) staff       (20)      514 2024-03-17 20:09:18.000000 exafs_neo-2.0.8/tests/test_ini_parser.py
+-rw-r--r--   0 andy       (501) staff       (20)     3385 2024-03-23 20:03:36.000000 exafs_neo-2.0.8/tests/test_larchscore.py
+-rw-r--r--   0 andy       (501) staff       (20)      976 2024-03-23 23:13:20.000000 exafs_neo-2.0.8/tests/test_neo_pop.py
+-rw-r--r--   0 andy       (501) staff       (20)     5754 2024-03-31 00:14:43.000000 exafs_neo-2.0.8/tests/test_neocrossover.py
+-rw-r--r--   0 andy       (501) staff       (20)     3771 2024-04-03 00:18:39.000000 exafs_neo-2.0.8/tests/test_neomutator.py
+-rw-r--r--   0 andy       (501) staff       (20)     2483 2024-04-26 22:42:19.000000 exafs_neo-2.0.8/tests/test_neosolver.py
+-rw-r--r--   0 andy       (501) staff       (20)      338 2024-02-18 20:02:49.000000 exafs_neo-2.0.8/tests/test_utils.py
```

### Comparing `exafs_neo-2.0.7/LICENSE` & `exafs_neo-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/PKG-INFO` & `exafs_neo-2.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: exafs_neo
-Version: 2.0.7
+Version: 2.0.8
 Summary: exafs_neo AI analysis using GA
 Home-page: https://github.com/laumiulun/EXAFS_Neo
 Download-URL: https://github.com/laumiulun/EXAFS_Neo/tarball/master
 Author: Miu Lun Lau, Jeff Terry, Min Long
 Author-email: andylau@u.boisestate.edu, jterry98@iit.edu, minlong@boisestate.edu
 License: GPLv3
 Keywords: exafs_neo,AI,analysis
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: xraylarch
+Requires-Dist: attrs
+Requires-Dist: matplotlib
+Requires-Dist: psutil
 
 # EXAFS Neo
 
-#### Versions: 2.0.6
+#### Versions: 2.0.8
 
-#### Last update: Apr 24, 2024
+#### Last update: May 1, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
 [![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
 
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
@@ -40,23 +45,31 @@
 
         xcode-select --install
 
 ## Dependencies
 
 EXAFS Neo requires the following dependencies to run:
 
+Notes: this step below is only needed if you are installing using source code
+
         # Create new anaconda environment
         conda create -y --name exafs python=>3.9.10
         conda activate exafs
         conda install -y -c conda-forge "numpy>=1.23" "scipy>=1.8" "matplotlib>=3.6" "h5py>=3.5" "wxpython>=4.1" scikit-image scikit-learn pycifrw pandas jupyter plotly pyparsing pytest pytest-cov coverage
         pip install lmfit peakutils pyepics pyshortcuts termcolor sphinx dill pycifrw xraydb wxmplot wxutils fabio silx imageio charset-normalizer
         pip install xraylarch
 
 ## Installations
 
+To install via PIP:
+
+        conda create --name "exafs_neo" "python=3.12"
+        conda activate exafs_neo
+        pip install exafs_neo
+
 To install EXAFS Neo, simply clone the repo:
 
         git clone https://github.com/laumiulun/EXAFS_Neo.git
         cd EXAFS_Neo/
         pip install .
 
 ## Usage
```

### Comparing `exafs_neo-2.0.7/README.md` & `exafs_neo-2.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # EXAFS Neo
 
-#### Versions: 2.0.6
+#### Versions: 2.0.8
 
-#### Last update: Apr 24, 2024
+#### Last update: May 1, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
 [![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
 
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
@@ -27,23 +27,31 @@
 
         xcode-select --install
 
 ## Dependencies
 
 EXAFS Neo requires the following dependencies to run:
 
+Notes: this step below is only needed if you are installing using source code
+
         # Create new anaconda environment
         conda create -y --name exafs python=>3.9.10
         conda activate exafs
         conda install -y -c conda-forge "numpy>=1.23" "scipy>=1.8" "matplotlib>=3.6" "h5py>=3.5" "wxpython>=4.1" scikit-image scikit-learn pycifrw pandas jupyter plotly pyparsing pytest pytest-cov coverage
         pip install lmfit peakutils pyepics pyshortcuts termcolor sphinx dill pycifrw xraydb wxmplot wxutils fabio silx imageio charset-normalizer
         pip install xraylarch
 
 ## Installations
 
+To install via PIP:
+
+        conda create --name "exafs_neo" "python=3.12"
+        conda activate exafs_neo
+        pip install exafs_neo
+
 To install EXAFS Neo, simply clone the repo:
 
         git clone https://github.com/laumiulun/EXAFS_Neo.git
         cd EXAFS_Neo/
         pip install .
 
 ## Usage
```

### Comparing `exafs_neo-2.0.7/exafs_neo/analysis/EXAFS_Analysis.py` & `exafs_neo-2.0.8/exafs_neo/analysis/EXAFS_Analysis.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/analysis/larch_score.py` & `exafs_neo-2.0.8/exafs_neo/analysis/larch_score.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/exafs.py` & `exafs_neo-2.0.8/exafs_neo/exafs.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,21 +77,15 @@
         :return: result class 
         """
         STRColors.run_verbose_start(self.logger, self.exafs_neo_pars, verbose_lvl=self.verbose_lvl)
 
         for currGen in range(self.exafs_neo_pars.fixedPars.nGen):
             self.exafs_neo_pars.runPars.start_gen()
 
-            self.selector.select(self.neo_population)
-            self.crossOver.crossover(self.neo_population)
-            self.mutator.mutate(self.neo_population)
-
-            self.neo_population.eval_population()
-
-            # self.solver.solve()
+            self.solver.solve(self.neo_population, self.selector, self.crossOver, self.mutator, self.exafs_neo_pars)
 
             # End of generation verbose
             STRColors.run_verbose_gen(self.logger, self.exafs_neo_pars, self.neo_population,
                                       verbose_lvl=self.verbose_lvl)
             self.result.collect(self.neo_population, self.exafs_neo_pars)
 
             # self.exafs_neo_pars.runPars.end_gen(self.neo_population)
@@ -118,14 +112,14 @@
         'kweight': 3.0,
         'deltak': 0.05,
         'rbkg': 1.1,
         'bkgkw': 1.0,
         'bkgkmax': 15.0,
         'printGraph': False,
         'pathrange': [1, 2, 3, 4, 5],
-
+        'solver_type': 1,
     }
     exafs_temp.exafs_read(input_parameters=input_dict)
     exafs_temp.exafs_setup()
 
     result = exafs_temp.run()
     print(result)
```

### Comparing `exafs_neo-2.0.7/exafs_neo/exafs_pop.py` & `exafs_neo-2.0.8/exafs_neo/exafs_pop.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/exafsfileobj.py` & `exafs_neo-2.0.8/exafs_neo/exafsfileobj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/gui/Analysis_plot.py` & `exafs_neo-2.0.8/exafs_neo/gui/Analysis_plot.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/gui/Background_plot.py` & `exafs_neo-2.0.8/exafs_neo/gui/Background_plot.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/gui/Console.py` & `exafs_neo-2.0.8/exafs_neo/gui/Console.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/gui/Misc_Function.py` & `exafs_neo-2.0.8/exafs_neo/gui/Misc_Function.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/gui/XAFS_GUI.py` & `exafs_neo-2.0.8/exafs_neo/gui/XAFS_GUI.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     LabelFrame, scrolledtext
 from tkinter.font import Font
 import ast
 
 from psutil import cpu_count
 
 from exafs_neo.helper import Bcolors
+from exafs_neo.utils_mapping import neomutator_str2int, neoselector_str2int, neocrossover_str2int, neosolver_str2int
 
 os.environ['NUMEXPR_MAX_THREADS'] = str(cpu_count())
 # import Larch
 import larch
 
 # import matplotlib for figures
 import matplotlib
@@ -102,15 +103,24 @@
         self.best_sample = IntVar(self.root, 20)
         self.lucky_few = IntVar(self.root, 20)
 
         # Mutations
         self.chance_of_mutation = IntVar(self.root, 20)
         self.orginal_chance_of_mutation = IntVar(self.root, 20)
         self.chance_of_mutation_e0 = IntVar(self.root, 20)
-        self.mutation_options = IntVar(self.root, 0)
+        self.mutation_options = StringVar(self.root, 'Mutate Per Individual')
+
+        # Selection
+        self.selection_options = StringVar(self.root, 'Roulette Wheel')
+
+        # Crossover
+        self.crossover_options = StringVar(self.root, 'Uniform Crossover')
+
+        # Solver
+        self.solver_options = StringVar(self.root, 'Genetic Algorithm')
 
         # Paths
         self.individual_path = BooleanVar(self.root, True)
         self.path_range = IntVar(self.root, 20)
         temp_list = ",".join(np.char.mod('%i', np.arange(1, self.path_range.get() + 1)))
         self.path_list = StringVar(self.root, temp_list)
         self.path_optimize = BooleanVar(self.root, False)
@@ -132,15 +142,15 @@
         self.steady_state_exit = BooleanVar(self.root, True)
 
         # Pertubutuions
         self.n_ini = IntVar(self.root, 100)
 
         # Sabcor initalizes variables
         self.sabcor_input_file = StringVar(self.root, 'Please choose a file')
-        self.sabcor_executable = StringVar(self.root,'Please choose the sabcor executable')
+        self.sabcor_executable = StringVar(self.root, 'Please choose the sabcor executable')
         self.sabcor_toggle = BooleanVar(self.root, False)
 
     def initialize_tab(self):
         """
         Initialize tab for the main frame. more tabs
         """
 
@@ -226,45 +236,69 @@
                     luck=str(self.lucky_few.get())))
 
         mutations = (
             "\n\n[Mutations] \nchance_of_mutation = {chance} \noriginal_chance_of_mutation = {original} \nchance_of_mutation_e0 = {e0} \nmutated_options = {opt}"
             .format(chance=str(self.chance_of_mutation.get()),
                     original=str(self.orginal_chance_of_mutation.get()),
                     e0=str(self.chance_of_mutation_e0.get()),
-                    opt=str(self.mutation_options.get())))
+                    opt=str(neomutator_str2int(self.mutation_options.get())))
+        )
+
+        selector = (
+            "\n\n[Selector] \nselection_options = {sel}"
+            .format(sel=str(neoselector_str2int(self.selection_options.get())))
+        )
+
+        crossover = (
+            "\n\n[Crossover] \ncrossover_options = {croOpt}"
+            .format(croOpt=str(neocrossover_str2int(self.crossover_options.get())))
+        )
+
+        solver = (
+            "\n\n[Solver] \nsolver_options = {solOpt}"
+            .format(solOpt=str(neosolver_str2int(self.solver_options.get())))
+        )
 
         paths = (
             "\n\n[Paths] \nindividual_path = {tf}  \npath_range = {range} \npath_list = {list} \npath_optimize = {optimize} \noptimize_percent = {optimize_pert} \noptimize_only = {optimize_only}"
             .format(tf=str(self.individual_path.get()),
                     range=str(self.path_range.get()),
                     list=str(self.path_list.get().replace(" ", "")),
                     optimize=str(self.path_optimize.get()),
                     optimize_pert=str(self.path_optimize_pert.get()),
                     optimize_only=str(self.path_optimize_only.get())
-                    ))
+                    )
+        )
 
         larch_paths = (
             "\n\n[Larch_Paths] \nkmin = {min} \nkmax = {max} \nkweight = {weight} \ndeltak = {delk} \nrbkg = {rb} \nbkgkw = {bk} \nbkgkmax = {bmax}"
             .format(min=self.kmin.get(),
                     max=self.kmax.get(),
                     weight=self.k_weight.get(),
                     delk=self.delta_k.get(),
                     rb=self.r_bkg.get(),
                     bk=self.bkg_kw.get(),
-                    bmax=self.bkg_kmax.get()))
+                    bmax=self.bkg_kmax.get()
+                    )
+        )
 
         outputs = ("\n\n[Outputs] \nprint_graph = {pg} \nnum_output_paths = {outpath}\nsteady_state_exit = {steady}"
                    .format(pg=self.print_graph.get(),
                            outpath=self.num_output_paths.get(),
-                           steady=self.steady_state_exit.get()))
+                           steady=self.steady_state_exit.get()
+                           )
+                   )
 
         with open(filename, 'w') as writer:
             writer.write(str(inputs))
             writer.write(str(populations))
             writer.write(str(mutations))
+            writer.write(str(crossover))
+            writer.write(str(selector))
+            writer.write(str(solver))
             writer.write(str(paths))
             writer.write(str(larch_paths))
             writer.write(str(outputs))
 
     def Generate_ini(self):
         # while proceed ==  False:
         ini_file = filedialog.asksaveasfilename(initialdir=os.getcwd(),
@@ -273,15 +307,14 @@
         if ini_file is None:
             return
         if not isinstance(ini_file, tuple):
             if len(ini_file) != 0:
                 self.Write_ini(ini_file)
                 messagebox.showinfo('', 'Ini file written to {fileloc}'.format(fileloc=ini_file))
 
-
     def stop_term(self):
         if hasattr(self, 'proc'):
             # print("Stopped EXAFS")
             self.proc.kill()
 
     def run_term(self, file='test_temp.i'):
         """
@@ -546,15 +579,14 @@
             if not folder_name:
                 var.set('Please choose a directory')
             else:
                 check_feff_folder(folder_name)
                 folder_name = os.path.join(folder_name, 'feff')
                 var.set(folder_name)
 
-
         # add trace back
         self.ncomp.trace_add('write', gen_feff_folder)
         self.ncomp.set(1)
 
         button_data_file = ttk.Button(self.tab_Inputs, text="Choose",
                                       command=select_data_file, style='my.TButton')
         button_data_file.grid(column=3, row=0, sticky=W, padx=self.padx, pady=self.pady)
@@ -766,19 +798,22 @@
                                                 textvariable=self.orginal_chance_of_mutation, font=self.entryFont)
         entry_chance_of_mutation.grid(column=1, row=1, sticky=(W, E), padx=self.padx)
 
         entry_chance_of_mutation = ttk.Combobox(self.tab_Mutation, width=7, values=mut_list,
                                                 textvariable=self.chance_of_mutation_e0, font=self.entryFont)
         entry_chance_of_mutation.grid(column=1, row=2, sticky=(W, E), padx=self.padx)
 
-        mut_list = list(range(3))
+        mut_list = ['Mutate Per Individual', 'Mutate Per Path', 'Mutate Per Trait', 'Mutate Metropolis',
+                    'Mutate Bounded Per Range', 'Mutate Differential Evolution']
         entry_chance_of_mutation = ttk.Combobox(self.tab_Mutation, width=7, values=mut_list,
                                                 textvariable=self.mutation_options, font=self.entryFont)
         entry_chance_of_mutation.grid(column=1, row=3, sticky=(W, E), padx=self.padx)
 
+        self.tab_Mutation.columnconfigure(1, weight=1)
+
     def Build_larch_tab(self):
         arr_larch = ["Kmin", "Kmax", "Kweight", "Delta k", "R Bkg", "Bkg Kw", "Bkg Kmax"]
         self.description_tabs(arr_larch, self.tab_Larch)
 
         entry_kmin = ttk.Entry(self.tab_Larch, textvariable=self.kmin, font=self.entryFont)
         entry_kmin.grid(column=1, row=0, sticky=(W, E), padx=self.padx)
 
@@ -1129,14 +1164,15 @@
         def select_sabcor_executable():
             file_name = filedialog.askopenfilename(initialdir=os.getcwd(), title="Choose Sabcor Executable",
                                                    filetypes=(("exe file", "*.exe"), ("all files", "*.*")))
             if not file_name:
                 self.sabcor_executable.set('Please choose a file')
             else:
                 self.sabcor_executable.set(file_name)
+
         def checkbox_sabcor():
             if self.sabcor_toggle.get() == True:
                 sabcor_input_file.config(state='normal')
                 button_sabcor_input_file.config(state='normal')
                 sabcor_executable.config(state='normal')
                 button_sabcor_executable.config(state='normal')
                 # allow only single entry
@@ -1146,49 +1182,66 @@
             else:
                 sabcor_input_file.config(state='disabled')
                 button_sabcor_input_file.config(state='disabled')
                 sabcor_executable.config(state='disabled')
                 button_sabcor_executable.config(state='disabled')
                 entry_ncomp.config(state='normal')
 
-        arr_expert = ["Override Num Compounds", "Sabcor Toggle", "Sabcor Input File","Sabcor Executable"]
-        self.description_tabs(arr_expert, self.tab_Expert, row=[0, 2, 3, 4])
+        arr_expert = ["Selector Options", "Crossover Options", "Solver Options", "Override Num Compounds",
+                      "Sabcor Toggle", "Sabcor Input File", "Sabcor Executable"]
+        self.description_tabs(arr_expert, self.tab_Expert, row=[0, 1, 2, 3, 5, 6, 7])
 
         self.tab_Expert.grid_columnconfigure(1, weight=1)
 
+        sel_list = ['Roulette Wheel', 'Tournament']
+        selection_combo = ttk.Combobox(self.tab_Expert, width=7, values=sel_list,
+                                       textvariable=self.selection_options, font=self.entryFont)
+        selection_combo.grid(column=1, row=0, columnspan=3,sticky=(W, E), padx=self.padx)
+
+        cro_list = ['Uniform Crossover', 'Single Point Corssover', 'Dual Point Crossover', 'Arithmetic Crossover',
+                    'Or Crossover', 'Average Crossover']
+        crossover_combo = ttk.Combobox(self.tab_Expert, width=7, values=cro_list,
+                                       textvariable=self.crossover_options, font=self.entryFont)
+        crossover_combo.grid(column=1, row=1, columnspan=3,sticky=(W, E), padx=self.padx)
+
+        sol_list = ['Genetic Algorithm', 'Genetic Algorithm with Rechenberg', 'Differential Evolution']
+        solver_combo = ttk.Combobox(self.tab_Expert, width=7, values=sol_list,
+                                    textvariable=self.solver_options, font=self.entryFont)
+        solver_combo.grid(column=1, row=2, columnspan=3,sticky=(W, E), padx=self.padx)
+
         ncomp_list = list(range(1, 101))
         entry_ncomp = ttk.Combobox(self.tab_Expert, width=7, values=ncomp_list, textvariable=self.ncomp,
                                    font=self.entryFont)
-        entry_ncomp.grid(column=1, row=0, sticky=(W, E), padx=self.padx)
+        entry_ncomp.grid(column=1, row=3, columnspan=3, sticky=(W, E), padx=self.padx)
 
         separator = ttk.Separator(self.tab_Expert, orient='horizontal')
-        separator.grid(column=0, row=1, columnspan=4, sticky=W + E, padx=self.padx)
+        separator.grid(column=0, row=4, columnspan=4, sticky=W + E, padx=self.padx)
 
         sabcor_toggle = ttk.Checkbutton(self.tab_Expert,
                                         variable=self.sabcor_toggle, command=checkbox_sabcor)
-        sabcor_toggle.grid(column=1, row=2, sticky=(W, E), padx=self.padx)
+        sabcor_toggle.grid(column=1, row=5, sticky=(W, E), padx=self.padx)
         if self.os == "Windows":
             sabcor_toggle.configure(state='disabled')
 
         sabcor_input_file = tk.Entry(self.tab_Expert, textvariable=self.sabcor_input_file, font=self.entryFont)
-        sabcor_input_file.grid(column=1, row=3, sticky=(W, E), padx=self.padx, pady=self.pady)
+        sabcor_input_file.grid(column=1, row=6, sticky=(W, E), padx=self.padx, pady=self.pady)
         sabcor_input_file.config(state='disabled')
 
         button_sabcor_input_file = ttk.Button(self.tab_Expert, text="Choose",
                                               command=select_sabcor_file, style='my.TButton')
-        button_sabcor_input_file.grid(column=3, row=3, sticky=W, padx=self.padx, pady=self.pady)
+        button_sabcor_input_file.grid(column=3, row=6, sticky=W, padx=self.padx, pady=self.pady)
         button_sabcor_input_file.config(state='disabled')
 
         sabcor_executable = tk.Entry(self.tab_Expert, textvariable=self.sabcor_executable, font=self.entryFont)
-        sabcor_executable.grid(column=1, row=4, sticky=(W, E), padx=self.padx, pady=self.pady)
+        sabcor_executable.grid(column=1, row=7, sticky=(W, E), padx=self.padx, pady=self.pady)
         sabcor_executable.config(state='disabled')
 
         button_sabcor_executable = ttk.Button(self.tab_Expert, text="Choose",
                                               command=select_sabcor_executable, style='my.TButton')
-        button_sabcor_executable.grid(column=3, row=4, sticky=W, padx=self.padx, pady=self.pady)
+        button_sabcor_executable.grid(column=3, row=7, sticky=W, padx=self.padx, pady=self.pady)
         button_sabcor_executable.config(state='disabled')
 
     def On_closing(self):
         """
         on closing function
         """
         if messagebox.askokcancel("Quit", "Do you want to quit?"):
```

### Comparing `exafs_neo-2.0.7/exafs_neo/gui/feff_folder_larch.py` & `exafs_neo-2.0.8/exafs_neo/gui/feff_folder_larch.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/gui/media/Citation` & `exafs_neo-2.0.8/exafs_neo/gui/media/Citation`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/gui/media/LICENSE` & `exafs_neo-2.0.8/exafs_neo/gui/media/LICENSE`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/gui/media/icon.png` & `exafs_neo-2.0.8/exafs_neo/gui/media/icon.png`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/helper.py` & `exafs_neo-2.0.8/exafs_neo/helper.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/individual.py` & `exafs_neo-2.0.8/exafs_neo/individual.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/ini_parser.py` & `exafs_neo-2.0.8/exafs_neo/ini_parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/input_arg.py` & `exafs_neo-2.0.8/exafs_neo/input_arg.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/neoCrossOver.py` & `exafs_neo-2.0.8/exafs_neo/neoCrossOver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 
 from exafs_neo.exafs_pop import NeoPopulations
 from exafs_neo.neoPars import NeoPars
 
 
+
 class EXAFS_CrossoverBase:
     def __init__(self, exafs_pars, logger=None):
         self.logger = logger
         self.exafs_pars = exafs_pars
         self.croOpt = self.exafs_pars.crossPars.croOpt
         self.croType = None
 
@@ -236,15 +237,15 @@
 if __name__ == "__main__":
     inputs_pars = {'data_file': '../path_files/Cu/cu_10k.xmu', 'output_file': '',
                    'feff_file': '../path_files/Cu/path_75/feff', 'kmin': 0.95,
                    'kmax': 9.775,
                    'kweight': 3.0, 'pathrange': [1, 2, 3, 4, 5],
                    'deltak': 0.05, 'rbkg': 1.1, 'bkgkw': 1.0, 'bkgkmax': 15.0,
                    'mut_options': 1,
-                   'croOpt': 0}
+                   'croOpt': 1}
     exafs_Pars = NeoPars()
     exafs_Pars.read_inputs(inputs_pars)
 
     neo_population = NeoPopulations(exafs_Pars)
     neo_population.initialize_populations()
     print(neo_population.population[0].get_var())
```

### Comparing `exafs_neo-2.0.7/exafs_neo/neoFilePars.py` & `exafs_neo-2.0.8/exafs_neo/neoFilePars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # from dataclasses import dataclass, field
-import csv
-
 from attrs import define, field
 
 from pathlib import Path
 
 from exafs_neo.utils import checkKey
```

### Comparing `exafs_neo-2.0.7/exafs_neo/neoMutator.py` & `exafs_neo-2.0.8/exafs_neo/neoMutator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import copy
 import numpy as np
 from exafs_neo.exafs_pop import NeoPopulations, fitness
 from exafs_neo.neoPars import NeoPars
 
 
+
+
 class ExafsMutatorBase:
     def __init__(self, exafs_pars, logger):
         self.logger = logger
         self.exafs_pars = exafs_pars
         self.mutOpt = self.exafs_pars.mutPars.mutOpt
         self.mutChance = self.exafs_pars.mutPars.mutChance
         self.mutChanceE0 = self.exafs_pars.mutPars.mutChanceE0
@@ -24,33 +26,14 @@
     def __init__(self, exafs_pars, logger):
         super().__init__(exafs_pars, logger)
         self.mutOpt = 1
 
         self.mutType = "Mutate Per Individual"
 
     def mutate(self, pops):
-        # Recehenberg mutation
-        diffCounter = self.exafs_pars.runPars.diffCounter
-        if self.exafs_pars.runPars.currGen > 20:
-            if diffCounter < 0.1:
-                diffCounter += 1
-            else:
-                diffCounter -= 1
-
-            if (abs(diffCounter) / float(self.exafs_pars.runPars.currGen)) > 0.2:
-                self.exafs_pars.mutPars.mutChance += 0.025
-                self.exafs_pars.mutPars.mutChance = abs(self.exafs_pars.mutPars.mutChance)
-            elif (abs(diffCounter) / float(self.exafs_pars.runPars.currGen)) < 0.2:
-                if (self.exafs_pars.mutPars.mutChance - 0.025) > 0:
-                    self.exafs_pars.mutPars.mutChance -= 0.025
-                    self.exafs_pars.mutPars.mutChance = abs(self.exafs_pars.mutPars.mutChance)
-
-            # Clip between 0 and 100%
-            self.exafs_pars.mutPars.mutChance = np.clip(self.exafs_pars.mutPars.mutChance, 0, 100)
-
         for i, _ in enumerate(pops.population):
             if np.random.random() < self.mutChance:
                 new_ind = pops.generate_individual()
                 pops.population[i] = new_ind
                 self.exafs_pars.mutPars.nmut += 1
```

### Comparing `exafs_neo-2.0.7/exafs_neo/neoPars.py` & `exafs_neo-2.0.8/exafs_neo/neoPars.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/neoResult.py` & `exafs_neo-2.0.8/exafs_neo/neoResult.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/neoSelector.py` & `exafs_neo-2.0.8/exafs_neo/neoSelector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from exafs_neo.exafs_pop import NeoPopulations
 from exafs_neo.neoPars import NeoPars
 
 
+
+
+
 class NeoSelectorBase:
     def __init__(self, exafs_pars, logger):
         """
         Initialize the selector base class
         :param exafs_pars:
         :param logger:
         """
```

### Comparing `exafs_neo-2.0.7/exafs_neo/parser.py` & `exafs_neo-2.0.8/exafs_neo/parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/pathObj.py` & `exafs_neo-2.0.8/exafs_neo/pathObj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/pathrange.py` & `exafs_neo-2.0.8/exafs_neo/pathrange.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/pathrange_file.py` & `exafs_neo-2.0.8/exafs_neo/pathrange_file.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/exafs_neo/utils.py` & `exafs_neo-2.0.8/exafs_neo/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import datetime
 import logging
 import pathlib
 import sys
 
 import numpy as np
 from exafs_neo.helper import time_call
-
+from exafs_neo.utils_mapping import neocrossover_int2str, neomutator_int2str, neoselector_int2str
 
 def raise_error(msg='Error'):
     raise Exception(msg)
 
 
+
 def checkKey(key, dictionary, alt_value=None, logger=None, verbose=False):
     # TODO: Raise checker for alternative response
     if key not in dictionary:
         if verbose:
             warn_str = f'{key} not found! Using default value of {key}: {alt_value}'
             if logger is None:
                 print(warn_str)
@@ -153,30 +154,35 @@
                                                     verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger,
                                                     f"{STRColors.BOLD}Path Optimize Percent{STRColors.ENDC}: {exafs_NeoPars.fixedPars.pathOptimizePercent}",
                                                     verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger,
                                                     f"{STRColors.BOLD}Path Optimize Only{STRColors.ENDC}: {exafs_NeoPars.fixedPars.pathOptimizeOnly}",
                                                     verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger, "-----------------Solvers-------------------",
+                                                    verbose_lvl, 5)
+        # STRColors.logger_print_based_on_verbose_lvl(logger,
+        #                                             f"{STRColors.BOLD}Solver Options{STRColors.ENDC}: {exafs_NeoPars.mutPars.}",
+        #                                             verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger, "----------------Mutations------------------",
                                                     verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger,
                                                     f"{STRColors.BOLD}Mutations{STRColors.ENDC}: {exafs_NeoPars.mutPars.mutChance}",
                                                     verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger,
                                                     f"{STRColors.BOLD}E0 Mutations{STRColors.ENDC}: {exafs_NeoPars.mutPars.mutChanceE0}",
                                                     verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger,
-                                                    f"{STRColors.BOLD}Mutation Options{STRColors.ENDC}: {exafs_NeoPars.mutPars.mutOpt}",
+                                                    f"{STRColors.BOLD}Mutation Options{STRColors.ENDC}: {neomutator_int2str(exafs_NeoPars.mutPars.mutOpt)}",
                                                     verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger,
-                                                    f"{STRColors.BOLD}Selection Options{STRColors.ENDC}: {exafs_NeoPars.selPars.selOpt}",
+                                                    f"{STRColors.BOLD}Selection Options{STRColors.ENDC}: {neoselector_int2str(exafs_NeoPars.selPars.selOpt)}",
                                                     verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger,
-                                                    f"{STRColors.BOLD}Crossover Options{STRColors.ENDC}: {exafs_NeoPars.crossPars.croOpt}",
+                                                    f"{STRColors.BOLD}Crossover Options{STRColors.ENDC}: {neocrossover_int2str(exafs_NeoPars.crossPars.croOpt)}",
                                                     verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger, "---------------Larch Paths-----------------", verbose_lvl,
                                                     5)
         STRColors.logger_print_based_on_verbose_lvl(logger,
                                                     f"{STRColors.BOLD}Kmin{STRColors.ENDC}: {exafs_NeoPars.exafsPars.kmin}",
                                                     verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger,
```

### Comparing `exafs_neo-2.0.7/exafs_neo.egg-info/PKG-INFO` & `exafs_neo-2.0.8/exafs_neo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
-Name: exafs-neo
-Version: 2.0.7
+Name: exafs_neo
+Version: 2.0.8
 Summary: exafs_neo AI analysis using GA
 Home-page: https://github.com/laumiulun/EXAFS_Neo
 Download-URL: https://github.com/laumiulun/EXAFS_Neo/tarball/master
 Author: Miu Lun Lau, Jeff Terry, Min Long
 Author-email: andylau@u.boisestate.edu, jterry98@iit.edu, minlong@boisestate.edu
 License: GPLv3
 Keywords: exafs_neo,AI,analysis
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: xraylarch
+Requires-Dist: attrs
+Requires-Dist: matplotlib
+Requires-Dist: psutil
 
 # EXAFS Neo
 
-#### Versions: 2.0.6
+#### Versions: 2.0.8
 
-#### Last update: Apr 24, 2024
+#### Last update: May 1, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
 [![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
 
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
@@ -40,23 +45,31 @@
 
         xcode-select --install
 
 ## Dependencies
 
 EXAFS Neo requires the following dependencies to run:
 
+Notes: this step below is only needed if you are installing using source code
+
         # Create new anaconda environment
         conda create -y --name exafs python=>3.9.10
         conda activate exafs
         conda install -y -c conda-forge "numpy>=1.23" "scipy>=1.8" "matplotlib>=3.6" "h5py>=3.5" "wxpython>=4.1" scikit-image scikit-learn pycifrw pandas jupyter plotly pyparsing pytest pytest-cov coverage
         pip install lmfit peakutils pyepics pyshortcuts termcolor sphinx dill pycifrw xraydb wxmplot wxutils fabio silx imageio charset-normalizer
         pip install xraylarch
 
 ## Installations
 
+To install via PIP:
+
+        conda create --name "exafs_neo" "python=3.12"
+        conda activate exafs_neo
+        pip install exafs_neo
+
 To install EXAFS Neo, simply clone the repo:
 
         git clone https://github.com/laumiulun/EXAFS_Neo.git
         cd EXAFS_Neo/
         pip install .
 
 ## Usage
```

### Comparing `exafs_neo-2.0.7/exafs_neo.egg-info/SOURCES.txt` & `exafs_neo-2.0.8/exafs_neo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 exafs_neo/neoSelector.py
 exafs_neo/neoSolver.py
 exafs_neo/parser.py
 exafs_neo/pathObj.py
 exafs_neo/pathrange.py
 exafs_neo/pathrange_file.py
 exafs_neo/utils.py
+exafs_neo/utils_mapping.py
 exafs_neo.egg-info/PKG-INFO
 exafs_neo.egg-info/SOURCES.txt
 exafs_neo.egg-info/dependency_links.txt
 exafs_neo.egg-info/entry_points.txt
 exafs_neo.egg-info/not-zip-safe
 exafs_neo.egg-info/requires.txt
 exafs_neo.egg-info/top_level.txt
```

### Comparing `exafs_neo-2.0.7/setup.py` & `exafs_neo-2.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/tests/test_EXAFS_analysis.py` & `exafs_neo-2.0.8/tests/test_EXAFS_analysis.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/tests/test_exafs_fileobj.py` & `exafs_neo-2.0.8/tests/test_exafs_fileobj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/tests/test_exafs_pars.py` & `exafs_neo-2.0.8/tests/test_exafs_pars.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/tests/test_exafs_pathObj.py` & `exafs_neo-2.0.8/tests/test_exafs_pathObj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/tests/test_exafs_pathrange.py` & `exafs_neo-2.0.8/tests/test_exafs_pathrange.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/tests/test_individual.py` & `exafs_neo-2.0.8/tests/test_individual.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/tests/test_ini_parser.py` & `exafs_neo-2.0.8/tests/test_ini_parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/tests/test_larchscore.py` & `exafs_neo-2.0.8/tests/test_larchscore.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/tests/test_neo_pop.py` & `exafs_neo-2.0.8/tests/test_neo_pop.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/tests/test_neocrossover.py` & `exafs_neo-2.0.8/tests/test_neocrossover.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.7/tests/test_neomutator.py` & `exafs_neo-2.0.8/tests/test_neomutator.py`

 * *Files identical despite different names*

