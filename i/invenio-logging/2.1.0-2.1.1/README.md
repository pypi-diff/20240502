# Comparing `tmp/invenio-logging-2.1.0.tar.gz` & `tmp/invenio-logging-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-logging-2.1.0.tar", last modified: Sun Oct 15 07:56:55 2023, max compression
+gzip compressed data, was "dist/invenio-logging-2.1.1.tar", last modified: Wed May  1 22:46:59 2024, max compression
```

## Comparing `invenio-logging-2.1.0.tar` & `invenio-logging-2.1.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/examplesapp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)      158 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/examples/app-fixtures.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      176 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/examples/app-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      203 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/examples/app-teardown.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/examples/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/invenio_logging/
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/invenio_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/invenio_logging/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/invenio_logging/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/invenio_logging/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/invenio_logging/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/invenio_logging/sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/invenio_logging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/invenio_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/invenio_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/invenio_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/invenio_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/invenio_logging.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/invenio_logging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/invenio_logging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/invenio_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      459 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 07:56:55.000000 invenio-logging-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/tests/test_console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/tests/test_examples_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/tests/test_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/tests/test_invenio_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-10-15 07:56:50.000000 invenio-logging-2.1.0/tests/test_sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:46:59.000000 invenio-logging-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-01 22:46:59.000000 invenio-logging-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:46:59.000000 invenio-logging-2.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/examplesapp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:46:59.000000 invenio-logging-2.1.1/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      158 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/examples/app-fixtures.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/examples/app-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      203 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/examples/app-teardown.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/examples/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:46:59.000000 invenio-logging-2.1.1/invenio_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/invenio_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/invenio_logging/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/invenio_logging/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/invenio_logging/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/invenio_logging/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/invenio_logging/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/invenio_logging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:46:59.000000 invenio-logging-2.1.1/invenio_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-01 22:46:58.000000 invenio-logging-2.1.1/invenio_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-01 22:46:58.000000 invenio-logging-2.1.1/invenio_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:46:58.000000 invenio-logging-2.1.1/invenio_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-01 22:46:58.000000 invenio-logging-2.1.1/invenio_logging.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:46:58.000000 invenio-logging-2.1.1/invenio_logging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-01 22:46:58.000000 invenio-logging-2.1.1/invenio_logging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 22:46:58.000000 invenio-logging-2.1.1/invenio_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-01 22:46:59.000000 invenio-logging-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:46:59.000000 invenio-logging-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/tests/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/tests/test_examples_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/tests/test_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/tests/test_invenio_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-01 22:46:52.000000 invenio-logging-2.1.1/tests/test_sentry.py
```

### Comparing `invenio-logging-2.1.0/.editorconfig` & `invenio-logging-2.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/CHANGES.rst` & `invenio-logging-2.1.1/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 ..
     This file is part of Invenio.
-    Copyright (C) 2015-2019 CERN.
+    Copyright (C) 2015-2024 CERN.
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.1.1 (released 2024-04-30)
+
+- installation: upper pin Sentry-SDK
+
 Version 2.1.0 (released 2023-10-15)
 
 - set sentry_event_id in templates
 
 Version 2.0.1 (released 2023-10-14)
 
 - set sentry_event_id
```

### Comparing `invenio-logging-2.1.0/CONTRIBUTING.rst` & `invenio-logging-2.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/LICENSE` & `invenio-logging-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/MANIFEST.in` & `invenio-logging-2.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/PKG-INFO` & `invenio-logging-2.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-logging
-Version: 2.1.0
+Version: 2.1.1
 Summary: "Module providing logging capabilities."
 Home-page: https://github.com/inveniosoftware/invenio-logging
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -33,22 +33,26 @@
         Invenio-Logging is a core component of Invenio responsible for configuring
         the Flask application logger.
         
         Further documentation at: https://invenio-logging.readthedocs.io/
         
         ..
             This file is part of Invenio.
-            Copyright (C) 2015-2019 CERN.
+            Copyright (C) 2015-2024 CERN.
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.1 (released 2024-04-30)
+        
+        - installation: upper pin Sentry-SDK
+        
         Version 2.1.0 (released 2023-10-15)
         
         - set sentry_event_id in templates
         
         Version 2.0.1 (released 2023-10-14)
         
         - set sentry_event_id
```

### Comparing `invenio-logging-2.1.0/README.rst` & `invenio-logging-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/docs/Makefile` & `invenio-logging-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/docs/conf.py` & `invenio-logging-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/docs/index.rst` & `invenio-logging-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/docs/make.bat` & `invenio-logging-2.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/examples/app.py` & `invenio-logging-2.1.1/examples/app.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/invenio_logging/__init__.py` & `invenio-logging-2.1.1/invenio_logging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2015-2024 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Module providing logging capabilities.
 
 Invenio-Logging is a core component of Invenio responsible for configuring
@@ -83,10 +83,10 @@
  * https://flask.palletsprojects.com/en/1.1.x/quickstart/#logging
  * https://docs.python.org/3/library/logging.html
 
 """
 
 from __future__ import absolute_import, print_function
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 __all__ = ("__version__",)
```

### Comparing `invenio-logging-2.1.0/invenio_logging/config.py` & `invenio-logging-2.1.1/invenio_logging/config.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/invenio_logging/console.py` & `invenio-logging-2.1.1/invenio_logging/console.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/invenio_logging/ext.py` & `invenio-logging-2.1.1/invenio_logging/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/invenio_logging/fs.py` & `invenio-logging-2.1.1/invenio_logging/fs.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/invenio_logging/sentry.py` & `invenio-logging-2.1.1/invenio_logging/sentry.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/invenio_logging/utils.py` & `invenio-logging-2.1.1/invenio_logging/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/invenio_logging.egg-info/PKG-INFO` & `invenio-logging-2.1.1/invenio_logging.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-logging
-Version: 2.1.0
+Version: 2.1.1
 Summary: "Module providing logging capabilities."
 Home-page: https://github.com/inveniosoftware/invenio-logging
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -33,22 +33,26 @@
         Invenio-Logging is a core component of Invenio responsible for configuring
         the Flask application logger.
         
         Further documentation at: https://invenio-logging.readthedocs.io/
         
         ..
             This file is part of Invenio.
-            Copyright (C) 2015-2019 CERN.
+            Copyright (C) 2015-2024 CERN.
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.1 (released 2024-04-30)
+        
+        - installation: upper pin Sentry-SDK
+        
         Version 2.1.0 (released 2023-10-15)
         
         - set sentry_event_id in templates
         
         Version 2.0.1 (released 2023-10-14)
         
         - set sentry_event_id
```

### Comparing `invenio-logging-2.1.0/invenio_logging.egg-info/SOURCES.txt` & `invenio-logging-2.1.1/invenio_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/setup.cfg` & `invenio-logging-2.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 	pytest-black>=0.3.0,<0.3.10
 	flask-login>=0.6.1
 	httpretty>=0.8.14
 	mock>=1.3.0
 	pytest-invenio>=1.4.2
 	iniconfig>=1.1.1
 	sphinx>=4.5
-	sentry-sdk[flask]>=1.0.0
+	sentry-sdk[flask]>=1.0.0,<2.0.0
 sentry_sdk = 
-	sentry-sdk[flask]>=1.0.0
+	sentry-sdk[flask]>=1.0.0,<2.0.0
 
 [options.entry_points]
 invenio_base.apps = 
 	invenio_logging_console = invenio_logging.console:InvenioLoggingConsole
 	invenio_logging_fs = invenio_logging.fs:InvenioLoggingFS
 	invenio_logging_sentry = invenio_logging.sentry:InvenioLoggingSentry
 invenio_base.api_apps =
```

### Comparing `invenio-logging-2.1.0/tests/conftest.py` & `invenio-logging-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/tests/test_console.py` & `invenio-logging-2.1.1/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/tests/test_examples_app.py` & `invenio-logging-2.1.1/tests/test_examples_app.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/tests/test_ext.py` & `invenio-logging-2.1.1/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/tests/test_fs.py` & `invenio-logging-2.1.1/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `invenio-logging-2.1.0/tests/test_sentry.py` & `invenio-logging-2.1.1/tests/test_sentry.py`

 * *Files identical despite different names*

