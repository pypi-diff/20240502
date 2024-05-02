# Comparing `tmp/djimporter-0.5.tar.gz` & `tmp/djimporter-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djimporter-0.5.tar", last modified: Tue Feb 27 13:38:31 2024, max compression
+gzip compressed data, was "djimporter-0.6.tar", last modified: Thu May  2 09:28:34 2024, max compression
```

## Comparing `djimporter-0.5.tar` & `djimporter-0.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.320655 djimporter-0.5/
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     1141 2024-02-27 13:33:58.000000 djimporter-0.5/CHANGELOG.md
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     1776 2022-01-14 15:23:03.000000 djimporter-0.5/LICENSE
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      140 2022-07-06 11:08:17.000000 djimporter-0.5/MANIFEST.in
--rw-r--r--   0 santiago  (1001) santiago  (1001)     1211 2024-02-27 13:38:31.320655 djimporter-0.5/PKG-INFO
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     5105 2024-01-09 11:50:10.000000 djimporter-0.5/README.md
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.312655 djimporter-0.5/djimporter/
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     1638 2024-02-27 13:38:17.000000 djimporter-0.5/djimporter/__init__.py
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      256 2021-07-16 08:54:43.000000 djimporter-0.5/djimporter/apps.py
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      760 2021-07-16 08:54:43.000000 djimporter-0.5/djimporter/checks.py
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.316655 djimporter-0.5/djimporter/djimporter.egg-info/
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     1099 2022-07-06 15:07:05.000000 djimporter-0.5/djimporter/djimporter.egg-info/PKG-INFO
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     1190 2022-07-06 15:07:05.000000 djimporter-0.5/djimporter/djimporter.egg-info/SOURCES.txt
--rw-rw-r--   0 santiago  (1001) santiago  (1001)        1 2022-07-06 15:07:05.000000 djimporter-0.5/djimporter/djimporter.egg-info/dependency_links.txt
--rw-rw-r--   0 santiago  (1001) santiago  (1001)        1 2022-07-06 08:53:33.000000 djimporter-0.5/djimporter/djimporter.egg-info/not-zip-safe
--rw-rw-r--   0 santiago  (1001) santiago  (1001)       69 2022-07-06 15:07:05.000000 djimporter-0.5/djimporter/djimporter.egg-info/requires.txt
--rw-rw-r--   0 santiago  (1001) santiago  (1001)       11 2022-07-06 15:07:05.000000 djimporter-0.5/djimporter/djimporter.egg-info/top_level.txt
--rw-rw-r--   0 santiago  (1001) santiago  (1001)    13695 2024-02-27 13:31:15.000000 djimporter-0.5/djimporter/fields.py
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      944 2024-02-26 12:58:06.000000 djimporter-0.5/djimporter/forms.py
--rw-rw-r--   0 santiago  (1001) santiago  (1001)    15054 2024-02-27 13:31:15.000000 djimporter-0.5/djimporter/importers.py
--rw-rw-r--   0 santiago  (1001) santiago  (1001)    14433 2023-02-22 16:37:37.000000 djimporter-0.5/djimporter/importers.py.NEW-bug-52
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.316655 djimporter-0.5/djimporter/migrations/
--rw-r--r--   0 santiago  (1001) santiago  (1001)     1033 2020-11-09 11:02:32.000000 djimporter-0.5/djimporter/migrations/0001_initial.py
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      381 2024-01-09 11:50:10.000000 djimporter-0.5/djimporter/migrations/0002_alter_importlog_user.py
--rw-r--r--   0 santiago  (1001) santiago  (1001)        0 2020-05-05 14:03:50.000000 djimporter-0.5/djimporter/migrations/__init__.py
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      836 2024-02-26 12:58:06.000000 djimporter-0.5/djimporter/models.py
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.308655 djimporter-0.5/djimporter/static/
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.308655 djimporter-0.5/djimporter/static/djimporter/
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.316655 djimporter-0.5/djimporter/static/djimporter/js/
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     4498 2024-01-09 11:50:10.000000 djimporter-0.5/djimporter/static/djimporter/js/guess_csv_properties.js
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      647 2024-01-09 11:50:10.000000 djimporter-0.5/djimporter/static/djimporter/js/upload_status.js
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     1402 2024-02-26 12:58:06.000000 djimporter-0.5/djimporter/tasks.py
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.312655 djimporter-0.5/djimporter/templates/
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.316655 djimporter-0.5/djimporter/templates/djimporter/
--rw-r--r--   0 santiago  (1001) santiago  (1001)      126 2020-05-05 14:03:50.000000 djimporter-0.5/djimporter/templates/djimporter/base.example.html
--rw-r--r--   0 santiago  (1001) santiago  (1001)      126 2023-05-10 09:51:44.000000 djimporter-0.5/djimporter/templates/djimporter/base.html
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      454 2024-01-09 11:50:10.000000 djimporter-0.5/djimporter/templates/djimporter/importer_info.html
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      342 2020-07-31 10:12:58.000000 djimporter-0.5/djimporter/templates/djimporter/importlog_confirm_delete.html
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     2832 2024-01-09 11:50:10.000000 djimporter-0.5/djimporter/templates/djimporter/importlog_detail.html
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     1078 2020-07-31 10:12:58.000000 djimporter-0.5/djimporter/templates/djimporter/importlog_list.html
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      437 2024-01-09 11:50:10.000000 djimporter-0.5/djimporter/urls.py
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     5373 2024-02-26 12:58:06.000000 djimporter-0.5/djimporter/views.py
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.320655 djimporter-0.5/djimporter.egg-info/
--rw-r--r--   0 santiago  (1001) santiago  (1001)     1211 2024-02-27 13:38:31.000000 djimporter-0.5/djimporter.egg-info/PKG-INFO
--rw-r--r--   0 santiago  (1001) santiago  (1001)     1666 2024-02-27 13:38:31.000000 djimporter-0.5/djimporter.egg-info/SOURCES.txt
--rw-r--r--   0 santiago  (1001) santiago  (1001)        1 2024-02-27 13:38:31.000000 djimporter-0.5/djimporter.egg-info/dependency_links.txt
--rw-r--r--   0 santiago  (1001) santiago  (1001)        1 2020-04-28 06:19:47.000000 djimporter-0.5/djimporter.egg-info/not-zip-safe
--rw-r--r--   0 santiago  (1001) santiago  (1001)       69 2024-02-27 13:38:31.000000 djimporter-0.5/djimporter.egg-info/requires.txt
--rw-r--r--   0 santiago  (1001) santiago  (1001)       17 2024-02-27 13:38:31.000000 djimporter-0.5/djimporter.egg-info/top_level.txt
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.320655 djimporter-0.5/docs/
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      113 2020-07-31 10:22:33.000000 djimporter-0.5/docs/_config.yml
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     9702 2022-01-14 15:23:09.000000 djimporter-0.5/docs/csvmodels.md
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      745 2021-11-25 12:41:44.000000 djimporter-0.5/docs/deployment.md
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     2261 2020-07-31 10:12:58.000000 djimporter-0.5/docs/howto.md
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     1289 2020-10-30 16:54:42.000000 djimporter-0.5/docs/index.md
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      224 2020-07-31 10:12:58.000000 djimporter-0.5/docs/installation.md
--rw-rw-r--   0 santiago  (1001) santiago  (1001)      104 2022-01-14 15:23:03.000000 djimporter-0.5/pyproject.toml
--rw-rw-r--   0 santiago  (1001) santiago  (1001)       38 2024-02-27 13:38:31.320655 djimporter-0.5/setup.cfg
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     1707 2022-07-06 15:13:44.000000 djimporter-0.5/setup.py
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.320655 djimporter-0.5/tests/
--rw-r--r--   0 santiago  (1001) santiago  (1001)        0 2020-06-26 16:19:13.000000 djimporter-0.5/tests/__init__.py
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     2982 2020-07-31 10:12:58.000000 djimporter-0.5/tests/conftest.py
-drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-02-27 13:38:31.320655 djimporter-0.5/tests/data/
--rw-r--r--   0 santiago  (1001) santiago  (1001)       25 2021-11-29 09:45:50.000000 djimporter-0.5/tests/data/ForeignKeySource.csv
--rw-rw-r--   0 santiago  (1001) santiago  (1001)       29 2022-01-14 15:23:09.000000 djimporter-0.5/tests/data/ForeignKeySource_valid.csv
--rw-rw-r--   0 santiago  (1001) santiago  (1001)       94 2022-01-14 15:23:09.000000 djimporter-0.5/tests/data/albums.csv
--rw-rw-r--   0 santiago  (1001) santiago  (1001)       33 2024-02-27 13:31:15.000000 djimporter-0.5/tests/data/songs.csv
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     1099 2024-02-27 13:31:15.000000 djimporter-0.5/tests/models.py
--rw-r--r--   0 santiago  (1001) santiago  (1001)       84 2020-11-16 16:04:26.000000 djimporter-0.5/tests/requirements.txt
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     4468 2024-02-27 13:31:15.000000 djimporter-0.5/tests/test_csvmodels.py
--rw-rw-r--   0 santiago  (1001) santiago  (1001)     1339 2020-07-31 10:12:58.000000 djimporter-0.5/tests/test_logs.py
--rw-rw-r--   0 santiago  (1001) santiago  (1001)       99 2020-07-31 10:12:58.000000 djimporter-0.5/tests/urls.py
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.756410 djimporter-0.6/
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     1205 2024-05-02 09:24:31.000000 djimporter-0.6/CHANGELOG.md
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      899 2024-05-02 09:22:42.000000 djimporter-0.6/CONTRIBUTING.md
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     1776 2022-01-14 15:23:03.000000 djimporter-0.6/LICENSE
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      140 2022-07-06 11:08:17.000000 djimporter-0.6/MANIFEST.in
+-rw-r--r--   0 santiago  (1001) santiago  (1001)     1238 2024-05-02 09:28:34.756410 djimporter-0.6/PKG-INFO
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     5237 2024-05-02 09:12:46.000000 djimporter-0.6/README.md
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.748409 djimporter-0.6/djimporter/
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     1638 2024-05-02 09:24:17.000000 djimporter-0.6/djimporter/__init__.py
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      256 2021-07-16 08:54:43.000000 djimporter-0.6/djimporter/apps.py
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      760 2021-07-16 08:54:43.000000 djimporter-0.6/djimporter/checks.py
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.752410 djimporter-0.6/djimporter/djimporter.egg-info/
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     1099 2022-07-06 15:07:05.000000 djimporter-0.6/djimporter/djimporter.egg-info/PKG-INFO
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     1190 2022-07-06 15:07:05.000000 djimporter-0.6/djimporter/djimporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)        1 2022-07-06 15:07:05.000000 djimporter-0.6/djimporter/djimporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)        1 2022-07-06 08:53:33.000000 djimporter-0.6/djimporter/djimporter.egg-info/not-zip-safe
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)       69 2022-07-06 15:07:05.000000 djimporter-0.6/djimporter/djimporter.egg-info/requires.txt
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)       11 2022-07-06 15:07:05.000000 djimporter-0.6/djimporter/djimporter.egg-info/top_level.txt
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)    13695 2024-02-27 13:31:15.000000 djimporter-0.6/djimporter/fields.py
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      944 2024-02-26 12:58:06.000000 djimporter-0.6/djimporter/forms.py
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)    15054 2024-02-27 13:31:15.000000 djimporter-0.6/djimporter/importers.py
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.752410 djimporter-0.6/djimporter/migrations/
+-rw-r--r--   0 santiago  (1001) santiago  (1001)     1033 2020-11-09 11:02:32.000000 djimporter-0.6/djimporter/migrations/0001_initial.py
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      381 2024-01-09 11:50:10.000000 djimporter-0.6/djimporter/migrations/0002_alter_importlog_user.py
+-rw-r--r--   0 santiago  (1001) santiago  (1001)        0 2020-05-05 14:03:50.000000 djimporter-0.6/djimporter/migrations/__init__.py
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      836 2024-02-26 12:58:06.000000 djimporter-0.6/djimporter/models.py
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.748409 djimporter-0.6/djimporter/static/
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.748409 djimporter-0.6/djimporter/static/djimporter/
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.752410 djimporter-0.6/djimporter/static/djimporter/js/
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     4498 2024-01-09 11:50:10.000000 djimporter-0.6/djimporter/static/djimporter/js/guess_csv_properties.js
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      647 2024-01-09 11:50:10.000000 djimporter-0.6/djimporter/static/djimporter/js/upload_status.js
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     1402 2024-02-26 12:58:06.000000 djimporter-0.6/djimporter/tasks.py
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.748409 djimporter-0.6/djimporter/templates/
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.756410 djimporter-0.6/djimporter/templates/djimporter/
+-rw-r--r--   0 santiago  (1001) santiago  (1001)      126 2020-05-05 14:03:50.000000 djimporter-0.6/djimporter/templates/djimporter/base.example.html
+-rw-r--r--   0 santiago  (1001) santiago  (1001)      126 2023-05-10 09:51:44.000000 djimporter-0.6/djimporter/templates/djimporter/base.html
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      454 2024-01-09 11:50:10.000000 djimporter-0.6/djimporter/templates/djimporter/importer_info.html
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      342 2020-07-31 10:12:58.000000 djimporter-0.6/djimporter/templates/djimporter/importlog_confirm_delete.html
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     2832 2024-01-09 11:50:10.000000 djimporter-0.6/djimporter/templates/djimporter/importlog_detail.html
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     1078 2020-07-31 10:12:58.000000 djimporter-0.6/djimporter/templates/djimporter/importlog_list.html
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      437 2024-01-09 11:50:10.000000 djimporter-0.6/djimporter/urls.py
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     5373 2024-02-26 12:58:06.000000 djimporter-0.6/djimporter/views.py
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.756410 djimporter-0.6/djimporter.egg-info/
+-rw-r--r--   0 santiago  (1001) santiago  (1001)     1238 2024-05-02 09:28:34.000000 djimporter-0.6/djimporter.egg-info/PKG-INFO
+-rw-r--r--   0 santiago  (1001) santiago  (1001)     1647 2024-05-02 09:28:34.000000 djimporter-0.6/djimporter.egg-info/SOURCES.txt
+-rw-r--r--   0 santiago  (1001) santiago  (1001)        1 2024-05-02 09:28:34.000000 djimporter-0.6/djimporter.egg-info/dependency_links.txt
+-rw-r--r--   0 santiago  (1001) santiago  (1001)        1 2020-04-28 06:19:47.000000 djimporter-0.6/djimporter.egg-info/not-zip-safe
+-rw-r--r--   0 santiago  (1001) santiago  (1001)       70 2024-05-02 09:28:34.000000 djimporter-0.6/djimporter.egg-info/requires.txt
+-rw-r--r--   0 santiago  (1001) santiago  (1001)       17 2024-05-02 09:28:34.000000 djimporter-0.6/djimporter.egg-info/top_level.txt
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.756410 djimporter-0.6/docs/
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      113 2020-07-31 10:22:33.000000 djimporter-0.6/docs/_config.yml
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     9702 2022-01-14 15:23:09.000000 djimporter-0.6/docs/csvmodels.md
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      745 2021-11-25 12:41:44.000000 djimporter-0.6/docs/deployment.md
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     2261 2020-07-31 10:12:58.000000 djimporter-0.6/docs/howto.md
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     1289 2020-10-30 16:54:42.000000 djimporter-0.6/docs/index.md
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      224 2020-07-31 10:12:58.000000 djimporter-0.6/docs/installation.md
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)      104 2022-01-14 15:23:03.000000 djimporter-0.6/pyproject.toml
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)       38 2024-05-02 09:28:34.756410 djimporter-0.6/setup.cfg
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     1732 2024-05-02 09:12:46.000000 djimporter-0.6/setup.py
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.756410 djimporter-0.6/tests/
+-rw-r--r--   0 santiago  (1001) santiago  (1001)        0 2020-06-26 16:19:13.000000 djimporter-0.6/tests/__init__.py
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     2982 2020-07-31 10:12:58.000000 djimporter-0.6/tests/conftest.py
+drwxrwxr-x   0 santiago  (1001) santiago  (1001)        0 2024-05-02 09:28:34.756410 djimporter-0.6/tests/data/
+-rw-r--r--   0 santiago  (1001) santiago  (1001)       25 2021-11-29 09:45:50.000000 djimporter-0.6/tests/data/ForeignKeySource.csv
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)       29 2022-01-14 15:23:09.000000 djimporter-0.6/tests/data/ForeignKeySource_valid.csv
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)       94 2022-01-14 15:23:09.000000 djimporter-0.6/tests/data/albums.csv
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)       33 2024-02-27 13:31:15.000000 djimporter-0.6/tests/data/songs.csv
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     1099 2024-02-27 13:31:15.000000 djimporter-0.6/tests/models.py
+-rw-r--r--   0 santiago  (1001) santiago  (1001)       84 2020-11-16 16:04:26.000000 djimporter-0.6/tests/requirements.txt
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     4468 2024-02-27 13:31:15.000000 djimporter-0.6/tests/test_csvmodels.py
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)     1339 2020-07-31 10:12:58.000000 djimporter-0.6/tests/test_logs.py
+-rw-rw-r--   0 santiago  (1001) santiago  (1001)       99 2020-07-31 10:12:58.000000 djimporter-0.6/tests/urls.py
```

### Comparing `djimporter-0.5/CHANGELOG.md` & `djimporter-0.6/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## main
 
+## [0.6.0] - 2024-05-02
+- [fixed] #59 Django 4.0 compatibility
+
 ## [0.5.0] - 2024-02-27
 - [added] #53 Implement CSV guesser to allow dynamic column mapping using JS.
 - [changed] #58 Allow null values on SlugRelatedField.
 - [fixed] #56 Handle too long values of ImportLog.user.
 
 ## [0.4.0] - 2022-07-06
 - [added] #48 CachedSlugRelatedField: optimize DB queries (1 big vs N small)
```

### Comparing `djimporter-0.5/LICENSE` & `djimporter-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/PKG-INFO` & `djimporter-0.6/djimporter/djimporter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djimporter
-Version: 0.5
+Version: 0.4a0
 Summary: Django importer, another CSV import library.
 Home-page: https://github.com/ico-apps/django-importer
 Author: ICO - Institut Catala Ornitologia
 Author-email: ico@ornitologia.org
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -19,12 +19,9 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 License-File: LICENSE
-Requires-Dist: django<4.0,>=2.2
-Requires-Dist: django-background-tasks==1.2.5
-Requires-Dist: python-magic==0.4.24
 
 Django importer, another CSV import library.
```

### Comparing `djimporter-0.5/README.md` & `djimporter-0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ```
 ## Custom import views
 You need to create the import view form template in your project extending your base template. You can create basic importers or advanced importers using field mapper and separator guesser.
 
 ### Basic importer view
 
 ![simple_importer](https://github.com/ico-apps/django-importer/assets/2751315/fc310978-88ad-41ac-a45a-0992ec232845)
- 
+
 You can create a basic importer extending ImportFormView (from djimporter.views) and creating a template including a basic form:
 
 ```
 <!-- include information on required fields and csv separator -->
 {% include "djimporter/importer_info.html" %}
 
 <form class="import-form" role="form" method="post" enctype="multipart/form-data">
@@ -42,18 +42,18 @@
 
 
 ```
 <!-- Form using boostrap4 libs -->
 
 <form class="import-form" role="form" method="post" enctype="multipart/form-data">
         {% csrf_token %}
-        
+
         <!-- Upload field -->
         {% bootstrap_field form.upfile layout='horizontal' %}
-        
+
         <div class="row justify-content-md-center">
           <div class="col-11">
             <div class="card shadow-sm mb-3">
               <div class="card-header">CSV options</div>
               <div class="card-body">
                 <div class="row mb-2">
                   <div class="col-12">
@@ -138,7 +138,13 @@
 pip install -r requirements.txt
 pip install -r tests/requirements.txt
 cp djimporter/templates/djimporter/base.example.html djimporter/templates/djimporter/base.html
 
 # 3. run test suite!
 pytest
 ```
+
+NOTE: to test against several environments (python version and Django version) you can use tox:
+```bash
+# check configurations on `tox.ini`
+tox
+```
```

### Comparing `djimporter-0.5/djimporter/__init__.py` & `djimporter-0.6/djimporter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Package metadata definition.
 """
-VERSION = (0, 5, 0, 'final', 1)
+VERSION = (0, 6, 0, 'final', 0)
 
 
 default_app_config = 'djimporter.apps.ImporterConfig'
 
 
 def get_version():
     "Returns a PEP 386-compliant version number from VERSION."
```

### Comparing `djimporter-0.5/djimporter/checks.py` & `djimporter-0.6/djimporter/checks.py`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/djimporter.egg-info/PKG-INFO` & `djimporter-0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: djimporter
-Version: 0.4a0
+Version: 0.6
 Summary: Django importer, another CSV import library.
 Home-page: https://github.com/ico-apps/django-importer
 Author: ICO - Institut Catala Ornitologia
 Author-email: ico@ornitologia.org
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 License-File: LICENSE
+Requires-Dist: django<4.1,>=2.2
+Requires-Dist: django4-background-tasks>=1.2.9
+Requires-Dist: python-magic>=0.4.27
 
 Django importer, another CSV import library.
```

### Comparing `djimporter-0.5/djimporter/djimporter.egg-info/SOURCES.txt` & `djimporter-0.6/djimporter/djimporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/fields.py` & `djimporter-0.6/djimporter/fields.py`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/forms.py` & `djimporter-0.6/djimporter/forms.py`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/importers.py` & `djimporter-0.6/djimporter/importers.py`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/migrations/0001_initial.py` & `djimporter-0.6/djimporter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/models.py` & `djimporter-0.6/djimporter/models.py`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/static/djimporter/js/guess_csv_properties.js` & `djimporter-0.6/djimporter/static/djimporter/js/guess_csv_properties.js`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/static/djimporter/js/upload_status.js` & `djimporter-0.6/djimporter/static/djimporter/js/upload_status.js`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/tasks.py` & `djimporter-0.6/djimporter/tasks.py`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/templates/djimporter/importlog_detail.html` & `djimporter-0.6/djimporter/templates/djimporter/importlog_detail.html`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/templates/djimporter/importlog_list.html` & `djimporter-0.6/djimporter/templates/djimporter/importlog_list.html`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter/views.py` & `djimporter-0.6/djimporter/views.py`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/djimporter.egg-info/PKG-INFO` & `djimporter-0.6/djimporter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: djimporter
-Version: 0.5
+Version: 0.6
 Summary: Django importer, another CSV import library.
 Home-page: https://github.com/ico-apps/django-importer
 Author: ICO - Institut Catala Ornitologia
 Author-email: ico@ornitologia.org
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 License-File: LICENSE
-Requires-Dist: django<4.0,>=2.2
-Requires-Dist: django-background-tasks==1.2.5
-Requires-Dist: python-magic==0.4.24
+Requires-Dist: django<4.1,>=2.2
+Requires-Dist: django4-background-tasks>=1.2.9
+Requires-Dist: python-magic>=0.4.27
 
 Django importer, another CSV import library.
```

### Comparing `djimporter-0.5/djimporter.egg-info/SOURCES.txt` & `djimporter-0.6/djimporter.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 CHANGELOG.md
+CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 djimporter/__init__.py
 djimporter/apps.py
 djimporter/checks.py
 djimporter/fields.py
 djimporter/forms.py
 djimporter/importers.py
-djimporter/importers.py.NEW-bug-52
 djimporter/models.py
 djimporter/tasks.py
 djimporter/urls.py
 djimporter/views.py
 djimporter.egg-info/PKG-INFO
 djimporter.egg-info/SOURCES.txt
 djimporter.egg-info/dependency_links.txt
```

### Comparing `djimporter-0.5/docs/csvmodels.md` & `djimporter-0.6/docs/csvmodels.md`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/docs/deployment.md` & `djimporter-0.6/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/docs/howto.md` & `djimporter-0.6/docs/howto.md`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/docs/index.md` & `djimporter-0.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/setup.py` & `djimporter-0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 from distutils.util import convert_path
 
 from setuptools import find_packages, setup
 
-
 main_ns = {}
 ver_path = convert_path('djimporter/__init__.py')
 with open(ver_path) as ver_file:
     exec(ver_file.read(), main_ns)
 
 version = main_ns['get_version']()
 
@@ -22,28 +21,29 @@
     author='ICO - Institut Catala Ornitologia',
     author_email='ico@ornitologia.org',
     description='Django importer, another CSV import library.',
     long_description=('Django importer, another CSV import library.'),
     license='BSD-3-Clause',
     packages=find_packages(),
     include_package_data=True,
-    install_requires=["django>=2.2,<4.0", "django-background-tasks==1.2.5", "python-magic==0.4.24"],
+    install_requires=["django>=2.2,<4.1", "django4-background-tasks>=1.2.9", "python-magic>=0.4.27"],
     zip_safe=False,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 2.2',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Internet :: WWW/HTTP :: WSGI',
         'Topic :: Internet :: WWW/HTTP :: WSGI :: Application',
     ],
 )
```

### Comparing `djimporter-0.5/tests/conftest.py` & `djimporter-0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/tests/models.py` & `djimporter-0.6/tests/models.py`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/tests/test_csvmodels.py` & `djimporter-0.6/tests/test_csvmodels.py`

 * *Files identical despite different names*

### Comparing `djimporter-0.5/tests/test_logs.py` & `djimporter-0.6/tests/test_logs.py`

 * *Files identical despite different names*

