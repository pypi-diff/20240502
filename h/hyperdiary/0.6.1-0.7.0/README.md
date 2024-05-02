# Comparing `tmp/hyperdiary-0.6.1.tar.gz` & `tmp/hyperdiary-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hyperdiary-0.6.1.tar", last modified: Wed Oct 21 15:49:59 2020, max compression
+gzip compressed data, was "hyperdiary-0.7.0.tar", last modified: Thu May  2 20:34:10 2024, max compression
```

## Comparing `hyperdiary-0.6.1.tar` & `hyperdiary-0.7.0.tar`

### file list

```diff
@@ -1,55 +1,61 @@
-drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2020-10-21 15:49:59.000000 hyperdiary-0.6.1/
--rw-r--r--   0 luphord   (1000) luphord   (1000)      155 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/AUTHORS.rst
--rw-r--r--   0 luphord   (1000) luphord   (1000)     3545 2020-10-21 15:24:35.000000 hyperdiary-0.6.1/CONTRIBUTING.rst
--rw-r--r--   0 luphord   (1000) luphord   (1000)     2027 2020-10-21 15:48:32.000000 hyperdiary-0.6.1/HISTORY.rst
--rw-r--r--   0 luphord   (1000) luphord   (1000)     1066 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/LICENSE
--rw-r--r--   0 luphord   (1000) luphord   (1000)      262 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/MANIFEST.in
--rw-r--r--   0 luphord   (1000) luphord   (1000)     7204 2020-10-21 15:49:59.000000 hyperdiary-0.6.1/PKG-INFO
--rw-r--r--   0 luphord   (1000) luphord   (1000)     3106 2020-10-21 15:25:12.000000 hyperdiary-0.6.1/README.rst
-drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2020-10-21 15:49:59.000000 hyperdiary-0.6.1/docs/
--rw-r--r--   0 luphord   (1000) luphord   (1000)      611 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/docs/Makefile
--rw-r--r--   0 luphord   (1000) luphord   (1000)       28 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/docs/authors.rst
--rwxr-xr-x   0 luphord   (1000) luphord   (1000)     4858 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/docs/conf.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)       33 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/docs/contributing.rst
--rw-r--r--   0 luphord   (1000) luphord   (1000)       28 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/docs/history.rst
--rw-r--r--   0 luphord   (1000) luphord   (1000)     1631 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/docs/hyperdiary.rst
--rw-r--r--   0 luphord   (1000) luphord   (1000)      276 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/docs/index.rst
--rw-r--r--   0 luphord   (1000) luphord   (1000)     1134 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/docs/installation.rst
--rw-r--r--   0 luphord   (1000) luphord   (1000)       67 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/docs/modules.rst
--rw-r--r--   0 luphord   (1000) luphord   (1000)       27 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/docs/readme.rst
-drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2020-10-21 15:49:59.000000 hyperdiary-0.6.1/hyperdiary/
--rw-r--r--   0 luphord   (1000) luphord   (1000)     5317 2020-10-21 15:49:27.000000 hyperdiary-0.6.1/hyperdiary/__init__.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)       58 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/hyperdiary/__main__.py
-drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2020-10-21 15:49:59.000000 hyperdiary-0.6.1/hyperdiary/assets/
-drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2020-10-21 15:49:59.000000 hyperdiary-0.6.1/hyperdiary/assets/css/
--rw-r--r--   0 luphord   (1000) luphord   (1000)    38127 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/hyperdiary/assets/css/picnic.min.css
--rw-r--r--   0 luphord   (1000) luphord   (1000)      399 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/hyperdiary/check.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)     8393 2020-10-21 15:34:38.000000 hyperdiary-0.6.1/hyperdiary/diary.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)     7857 2020-10-21 15:35:28.000000 hyperdiary-0.6.1/hyperdiary/html.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)     5006 2020-10-21 15:37:14.000000 hyperdiary-0.6.1/hyperdiary/htmltags.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)     1886 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/hyperdiary/hugo.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)     2547 2020-10-21 15:32:42.000000 hyperdiary-0.6.1/hyperdiary/localization.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)     6149 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/hyperdiary/simplepath.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)      670 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/hyperdiary/stats.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)     7442 2020-10-21 15:39:48.000000 hyperdiary-0.6.1/hyperdiary/tiddlywiki.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)      231 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/hyperdiary/view.py
-drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2020-10-21 15:49:59.000000 hyperdiary-0.6.1/hyperdiary.egg-info/
--rw-r--r--   0 luphord   (1000) luphord   (1000)     7204 2020-10-21 15:49:58.000000 hyperdiary-0.6.1/hyperdiary.egg-info/PKG-INFO
--rw-r--r--   0 luphord   (1000) luphord   (1000)      975 2020-10-21 15:49:58.000000 hyperdiary-0.6.1/hyperdiary.egg-info/SOURCES.txt
--rw-r--r--   0 luphord   (1000) luphord   (1000)        1 2020-10-21 15:49:58.000000 hyperdiary-0.6.1/hyperdiary.egg-info/dependency_links.txt
--rw-r--r--   0 luphord   (1000) luphord   (1000)       57 2020-10-21 15:49:58.000000 hyperdiary-0.6.1/hyperdiary.egg-info/entry_points.txt
--rw-r--r--   0 luphord   (1000) luphord   (1000)        1 2020-10-21 15:49:58.000000 hyperdiary-0.6.1/hyperdiary.egg-info/not-zip-safe
--rw-r--r--   0 luphord   (1000) luphord   (1000)       28 2020-10-21 15:49:58.000000 hyperdiary-0.6.1/hyperdiary.egg-info/requires.txt
--rw-r--r--   0 luphord   (1000) luphord   (1000)       17 2020-10-21 15:49:58.000000 hyperdiary-0.6.1/hyperdiary.egg-info/top_level.txt
--rw-r--r--   0 luphord   (1000) luphord   (1000)      393 2020-10-21 15:49:59.000000 hyperdiary-0.6.1/setup.cfg
--rw-r--r--   0 luphord   (1000) luphord   (1000)     1560 2020-10-21 15:49:27.000000 hyperdiary-0.6.1/setup.py
-drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2020-10-21 15:49:59.000000 hyperdiary-0.6.1/tests/
--rw-r--r--   0 luphord   (1000) luphord   (1000)       24 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/tests/__init__.py
-drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2020-10-21 15:49:59.000000 hyperdiary-0.6.1/tests/src/
-drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2020-10-21 15:49:59.000000 hyperdiary-0.6.1/tests/src/2019/
--rw-r--r--   0 luphord   (1000) luphord   (1000)       32 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/tests/src/2019/05.yaml
--rw-r--r--   0 luphord   (1000) luphord   (1000)      101 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/tests/src/2019/05_bad_entries.yaml
--rw-r--r--   0 luphord   (1000) luphord   (1000)      251 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/tests/src/2019/06.yaml
--rw-r--r--   0 luphord   (1000) luphord   (1000)      413 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/tests/src/hyperdiary.json
--rw-r--r--   0 luphord   (1000) luphord   (1000)      501 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/tests/test_doctests.py
--rw-r--r--   0 luphord   (1000) luphord   (1000)     5228 2020-04-23 11:10:24.000000 hyperdiary-0.6.1/tests/test_hyperdiary.py
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.240973 hyperdiary-0.7.0/
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      155 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/AUTHORS.rst
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     3545 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     2328 2024-05-02 20:03:28.000000 hyperdiary-0.7.0/HISTORY.rst
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     1066 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/LICENSE
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      262 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/MANIFEST.in
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     6298 2024-05-02 20:34:10.240973 hyperdiary-0.7.0/PKG-INFO
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     3181 2024-05-02 19:49:51.000000 hyperdiary-0.7.0/README.rst
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.220973 hyperdiary-0.7.0/docs/
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      611 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/docs/Makefile
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.212973 hyperdiary-0.7.0/docs/_build/
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.212973 hyperdiary-0.7.0/docs/_build/html/
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.224973 hyperdiary-0.7.0/docs/_build/html/_static/
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      286 2024-05-02 19:30:54.000000 hyperdiary-0.7.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       90 2024-05-02 19:30:54.000000 hyperdiary-0.7.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       90 2024-05-02 19:30:54.000000 hyperdiary-0.7.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       28 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/docs/authors.rst
+-rwxr-xr-x   0 luphord   (1000) luphord   (1000)     4855 2024-05-02 19:41:17.000000 hyperdiary-0.7.0/docs/conf.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       33 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/docs/contributing.rst
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       28 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/docs/history.rst
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     1597 2024-05-02 20:16:04.000000 hyperdiary-0.7.0/docs/hyperdiary.rst
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      276 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/docs/index.rst
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     1134 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/docs/installation.rst
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       67 2024-05-02 20:16:04.000000 hyperdiary-0.7.0/docs/modules.rst
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       27 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/docs/readme.rst
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.232973 hyperdiary-0.7.0/hyperdiary/
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     4834 2024-05-02 20:15:41.000000 hyperdiary-0.7.0/hyperdiary/__init__.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       58 2024-05-02 19:41:17.000000 hyperdiary-0.7.0/hyperdiary/__main__.py
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.212973 hyperdiary-0.7.0/hyperdiary/assets/
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.236973 hyperdiary-0.7.0/hyperdiary/assets/css/
+-rw-r--r--   0 luphord   (1000) luphord   (1000)    38127 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/hyperdiary/assets/css/picnic.min.css
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      399 2024-05-02 19:41:17.000000 hyperdiary-0.7.0/hyperdiary/check.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     8253 2024-05-02 19:41:18.000000 hyperdiary-0.7.0/hyperdiary/diary.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     7720 2024-05-02 19:41:18.000000 hyperdiary-0.7.0/hyperdiary/html.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     4960 2024-05-02 19:41:18.000000 hyperdiary-0.7.0/hyperdiary/htmltags.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     1790 2024-05-02 19:41:18.000000 hyperdiary-0.7.0/hyperdiary/hugo.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     2420 2024-05-02 19:41:18.000000 hyperdiary-0.7.0/hyperdiary/localization.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     6083 2024-05-02 19:41:18.000000 hyperdiary-0.7.0/hyperdiary/simplepath.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      615 2024-05-02 19:41:18.000000 hyperdiary-0.7.0/hyperdiary/stats.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     7574 2024-05-02 19:57:33.000000 hyperdiary-0.7.0/hyperdiary/tiddlywiki.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      231 2024-05-02 19:41:18.000000 hyperdiary-0.7.0/hyperdiary/view.py
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.236973 hyperdiary-0.7.0/hyperdiary.egg-info/
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     6298 2024-05-02 20:34:09.000000 hyperdiary-0.7.0/hyperdiary.egg-info/PKG-INFO
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     1078 2024-05-02 20:34:10.000000 hyperdiary-0.7.0/hyperdiary.egg-info/SOURCES.txt
+-rw-r--r--   0 luphord   (1000) luphord   (1000)        1 2024-05-02 20:34:09.000000 hyperdiary-0.7.0/hyperdiary.egg-info/dependency_links.txt
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       56 2024-05-02 20:34:09.000000 hyperdiary-0.7.0/hyperdiary.egg-info/entry_points.txt
+-rw-r--r--   0 luphord   (1000) luphord   (1000)        1 2024-05-02 20:34:09.000000 hyperdiary-0.7.0/hyperdiary.egg-info/not-zip-safe
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       28 2024-05-02 20:34:09.000000 hyperdiary-0.7.0/hyperdiary.egg-info/requires.txt
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       17 2024-05-02 20:34:09.000000 hyperdiary-0.7.0/hyperdiary.egg-info/top_level.txt
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      414 2024-05-02 20:34:10.244973 hyperdiary-0.7.0/setup.cfg
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     1595 2024-05-02 20:15:41.000000 hyperdiary-0.7.0/setup.py
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.240973 hyperdiary-0.7.0/tests/
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       24 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/tests/__init__.py
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.240973 hyperdiary-0.7.0/tests/src/
+drwxr-xr-x   0 luphord   (1000) luphord   (1000)        0 2024-05-02 20:34:10.240973 hyperdiary-0.7.0/tests/src/2019/
+-rw-r--r--   0 luphord   (1000) luphord   (1000)       32 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/tests/src/2019/05.yaml
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      101 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/tests/src/2019/05_bad_entries.yaml
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      251 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/tests/src/2019/06.yaml
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      413 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/tests/src/hyperdiary.json
+-rw-r--r--   0 luphord   (1000) luphord   (1000)      501 2024-01-28 17:59:26.000000 hyperdiary-0.7.0/tests/test_doctests.py
+-rw-r--r--   0 luphord   (1000) luphord   (1000)     5231 2024-05-02 20:01:53.000000 hyperdiary-0.7.0/tests/test_hyperdiary.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hyperdiary-0.6.1/CONTRIBUTING.rst` & `hyperdiary-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyperdiary-0.6.1/HISTORY.rst` & `hyperdiary-0.7.0/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =======
 History
 =======
 
+0.7.0 (2024-05-02)
+------------------
+* fix issue with tiddlywiki export (as the tiddlywiki file format has changed)
+* add support for Python 3.9 - 3.12
+* drop support for Python versions prior to 3.8
+* upgrade dependencies and dev dependencies
+* reformat code with black
+* migrate to github actions
+
 0.6.1 (2020-10-21)
 ------------------
 
 * add support for Python 3.8
 * upgrade to flake8 3.8.4 and fix linter issues
 * replace deprecated test command
 * move to travis-ci.com
```

### Comparing `hyperdiary-0.6.1/LICENSE` & `hyperdiary-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdiary-0.6.1/README.rst` & `hyperdiary-0.7.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 ============
 hyperdiary
 ============
 
 .. image:: https://img.shields.io/pypi/v/hyperdiary.svg
         :target: https://pypi.python.org/pypi/hyperdiary
 
-.. image:: https://travis-ci.com/luphord/hyperdiary.svg
-        :target: https://travis-ci.com/luphord/hyperdiary
+.. image:: https://github.com/luphord/hyperdiary/actions/workflows/lint-test.yml/badge.svg
+        :target: https://github.com/luphord/hyperdiary/actions
 
 .. image:: https://readthedocs.org/projects/hyperdiary/badge/?version=latest
         :target: https://hyperdiary.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 A command line tool for writing diaries with hyperlinks. Free software, licensed under MIT license.
 
 Installation
 ------------
 
-hyperdiary requires Python version 3.5 or later. Once you have Python and pip installed on your machine (and available in your path) you can install hyperdiary by executing
+hyperdiary requires Python version 3.8 or later. Once you have Python and [pipx](https://pipx.pypa.io/stable/) installed on your machine (and available in your path), you can install hyperdiary by executing
 
 .. code-block:: console
 
-        pip install hyperdiary
+        pipx install hyperdiary
 
 Setup
 -----
 
 A project file *hyperdiary.json* is required to setup your diary. It should be of this form:
 
 .. code-block:: json
 
         {
                 "sources": [
-                        "2019/05.yaml",
-                        "2019/06.yaml"
+                        "2024/05.yaml",
+                        "2024/06.yaml"
                 ],
                 "expected": [
-                        {"start": "2019-05-01", "end": "2019-05-01"},
-                        {"start": "2019-06-09", "end": "2019-06-10"}
+                        {"start": "2024-05-01", "end": "2024-05-01"},
+                        {"start": "2024-06-09", "end": "2024-06-10"}
                 ],
                 "localization": {
                         "months": ["Jan", "Feb", "Mar", "Apr", "May", "Jun",
                                    "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
                         "date_fmt": "%-d.%-m.%Y"
                 }
         }
 
-You diary content itself is entered in yaml files like this (*2019/06.yaml*):
+You diary content itself is entered in yaml files like this (*2024/06.yaml*):
 
 .. code-block:: yaml
 
-        2019-06-09:
+        2024-06-09:
           - Some entry goes here with a $special_identity|link
           - This entry is +surprise tagged +mytag +nexttag
           - This entry contains nothing new
-        2019-06-10:
+        2024-06-10:
           - Same $special_identity|link again and $New_Identity|NewIdentity
           - $test +mytag
 
 Use *$target|linktext* to create a hyperlink to *target* showing text *linktext*. Use *+mytag* to add tag *mytag*.
 
 Usage
 -----
```

### Comparing `hyperdiary-0.6.1/docs/Makefile` & `hyperdiary-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyperdiary-0.6.1/docs/conf.py` & `hyperdiary-0.7.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,44 +16,45 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
-sys.path.insert(0, os.path.abspath('..'))
+
+sys.path.insert(0, os.path.abspath(".."))
 
 import hyperdiary
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'hyperdiary'
-copyright = u"2019, luphord"
-author = u"luphord"
+project = "hyperdiary"
+copyright = "2019, luphord"
+author = "luphord"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = hyperdiary.__version__
@@ -66,97 +67,89 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
-html_theme_options = {
-    'logo': 'hyperdiary.png'
-}
+html_theme_options = {"logo": "hyperdiary.png"}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'hyperdiarydoc'
+htmlhelp_basename = "hyperdiarydoc"
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'hyperdiary.tex',
-     u'hyperdiary Documentation',
-     u'luphord', 'manual'),
+    (master_doc, "hyperdiary.tex", "hyperdiary Documentation", "luphord", "manual"),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'hyperdiary',
-     u'hyperdiary Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "hyperdiary", "hyperdiary Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'hyperdiary',
-     u'hyperdiary Documentation',
-     author,
-     'hyperdiary',
-     'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "hyperdiary",
+        "hyperdiary Documentation",
+        author,
+        "hyperdiary",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
```

### Comparing `hyperdiary-0.6.1/docs/hyperdiary.rst` & `hyperdiary-0.7.0/docs/hyperdiary.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,91 +4,90 @@
 Submodules
 ----------
 
 hyperdiary.check module
 -----------------------
 
 .. automodule:: hyperdiary.check
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 hyperdiary.diary module
 -----------------------
 
 .. automodule:: hyperdiary.diary
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 hyperdiary.html module
 ----------------------
 
 .. automodule:: hyperdiary.html
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 hyperdiary.htmltags module
 --------------------------
 
 .. automodule:: hyperdiary.htmltags
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 hyperdiary.hugo module
 ----------------------
 
 .. automodule:: hyperdiary.hugo
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 hyperdiary.localization module
 ------------------------------
 
 .. automodule:: hyperdiary.localization
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 hyperdiary.simplepath module
 ----------------------------
 
 .. automodule:: hyperdiary.simplepath
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 hyperdiary.stats module
 -----------------------
 
 .. automodule:: hyperdiary.stats
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 hyperdiary.tiddlywiki module
 ----------------------------
 
 .. automodule:: hyperdiary.tiddlywiki
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 hyperdiary.view module
 ----------------------
 
 .. automodule:: hyperdiary.view
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 Module contents
 ---------------
 
 .. automodule:: hyperdiary
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `hyperdiary-0.6.1/docs/installation.rst` & `hyperdiary-0.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hyperdiary-0.6.1/hyperdiary/__init__.py` & `hyperdiary-0.7.0/hyperdiary/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,167 +1,178 @@
-__author__ = 'luphord'
-__email__ = 'luphord@protonmail.com'
-__version__ = '0.6.1'
+__author__ = "luphord"
+__email__ = "luphord@protonmail.com"
+__version__ = "0.7.0"
 
 from argparse import ArgumentParser, Namespace
 from datetime import datetime, date, timedelta
 
 from .diary import Diary
 from .check import check
 from .stats import stats
 from .html import diary_to_html, diary_to_html_folder
 from .hugo import diary_to_hugo
 from .tiddlywiki import diary_to_tiddlers_export, diary_to_tiddlywiki_export
 from .view import view
 
-diary_path = '.'
+diary_path = "."
 
-parser = ArgumentParser(
-    description='The hyperdiary main command line interface.')
+parser = ArgumentParser(description="The hyperdiary main command line interface.")
 
-subparsers = parser.add_subparsers(title='subcommands', dest='subcommand',
-                                   help='Available subcommands')
+subparsers = parser.add_subparsers(
+    title="subcommands", dest="subcommand", help="Available subcommands"
+)
 subparsers.required = True
 
-check_parser = subparsers.add_parser('check', help='Check entire diary for '
-                                                   'integrity up-to-dateness')
+check_parser = subparsers.add_parser(
+    "check", help="Check entire diary for " "integrity up-to-dateness"
+)
 
 
 def _check_exec(args: Namespace) -> None:
-    print('Checking diary...')
+    print("Checking diary...")
     check(Diary.discover_and_load(diary_path))
 
 
 check_parser.set_defaults(func=_check_exec)
 
-stats_parser = subparsers.add_parser('stats', help='Calculate impressive '
-                                                   'diary statistics')
-stats_parser.add_argument('file', nargs='?')
+stats_parser = subparsers.add_parser(
+    "stats", help="Calculate impressive " "diary statistics"
+)
+stats_parser.add_argument("file", nargs="?")
 
 
 def _stats_exec(args: Namespace) -> None:
-    print('Stats\n-----')
+    print("Stats\n-----")
     if args.file:
         diary = Diary(dict(sources=[str(args.file)]))
         diary.load_entries()
     else:
         diary = Diary.discover_and_load(diary_path)
     stats(diary)
 
 
 stats_parser.set_defaults(func=_stats_exec)
 
-html_parser = subparsers.add_parser('html', help='Export diary to html')
-html_parser.add_argument('file')
+html_parser = subparsers.add_parser("html", help="Export diary to html")
+html_parser.add_argument("file")
 
 
 def _html_exec(args: Namespace) -> None:
-    print('Exporting diary in HTML to {}'.format(args.file))
+    print("Exporting diary in HTML to {}".format(args.file))
     diary_to_html(Diary.discover_and_load(diary_path), args.file)
 
 
 html_parser.set_defaults(func=_html_exec)
 
-html_folder_parser = subparsers.add_parser('htmlfolder',
-                                           help='Export diary to html '
-                                                'in folders')
-html_folder_parser.add_argument('folder')
+html_folder_parser = subparsers.add_parser(
+    "htmlfolder", help="Export diary to html " "in folders"
+)
+html_folder_parser.add_argument("folder")
 
 
 def _html_folder_exec(args: Namespace) -> None:
-    print('Exporting diary in HTML to {}'.format(args.folder))
+    print("Exporting diary in HTML to {}".format(args.folder))
     diary_to_html_folder(Diary.discover_and_load(diary_path), args.folder)
 
 
 html_folder_parser.set_defaults(func=_html_folder_exec)
 
-hugo_parser = subparsers.add_parser('hugo', help='Export diary to hugo static '
-                                                 'site format')
-hugo_parser.add_argument('folder')
+hugo_parser = subparsers.add_parser(
+    "hugo", help="Export diary to hugo static " "site format"
+)
+hugo_parser.add_argument("folder")
 
 
 def _hugo_exec(args: Namespace) -> None:
-    print('Exporting diary in hugo static site format to {}'
-          .format(args.folder))
+    print("Exporting diary in hugo static site format to {}".format(args.folder))
     diary_to_hugo(Diary.discover_and_load(diary_path), args.folder)
 
 
 hugo_parser.set_defaults(func=_hugo_exec)
 
-tiddler_parser = subparsers.add_parser('tiddlers',
-                                       help='Export diary to tiddlywiki '
-                                            'tiddlers format')
-tiddler_parser.add_argument('folder')
+tiddler_parser = subparsers.add_parser(
+    "tiddlers", help="Export diary to tiddlywiki " "tiddlers format"
+)
+tiddler_parser.add_argument("folder")
 
 
 def _tiddlers_exec(args: Namespace) -> None:
-    print('Exporting diary in tiddlywiki tiddlers format to {}'
-          .format(args.folder))
+    print("Exporting diary in tiddlywiki tiddlers format to {}".format(args.folder))
     diary_to_tiddlers_export(Diary.discover_and_load(diary_path), args.folder)
 
 
 tiddler_parser.set_defaults(func=_tiddlers_exec)
 
-tiddlywiki_parser = subparsers.add_parser('tiddlywiki',
-                                          help='Export diary to tiddlywiki')
-tiddlywiki_parser.add_argument('-t', '--tiddlywiki-base-file',
-                               help='path to tiddlywiki base file to '
-                                    'copy for export',
-                               default='empty.html', type=str)
-tiddlywiki_parser.add_argument('file')
+tiddlywiki_parser = subparsers.add_parser(
+    "tiddlywiki", help="Export diary to tiddlywiki"
+)
+tiddlywiki_parser.add_argument(
+    "-t",
+    "--tiddlywiki-base-file",
+    help="path to tiddlywiki base file to " "copy for export",
+    default="empty.html",
+    type=str,
+)
+tiddlywiki_parser.add_argument("file")
 
 
 def _tiddlywiki_exec(args: Namespace) -> None:
-    print('Exporting diary to tiddlywiki as {} with tiddlywiki base file {}'
-          .format(args.file, args.tiddlywiki_base_file))
-    diary_to_tiddlywiki_export(Diary.discover_and_load(diary_path),
-                               args.file, args.tiddlywiki_base_file)
+    print(
+        "Exporting diary to tiddlywiki as {} with tiddlywiki base file {}".format(
+            args.file, args.tiddlywiki_base_file
+        )
+    )
+    diary_to_tiddlywiki_export(
+        Diary.discover_and_load(diary_path), args.file, args.tiddlywiki_base_file
+    )
 
 
 tiddlywiki_parser.set_defaults(func=_tiddlywiki_exec)
 
-view_parser = subparsers.add_parser('view',
-                                    help='View entries on command line')
+view_parser = subparsers.add_parser("view", help="View entries on command line")
 
 
 def parse_date(sdate: str) -> date:
-    if sdate.lower() == 'today':
+    if sdate.lower() == "today":
         return date.today()
-    if sdate.lower() == 'yesterday':
-        return date.today()-timedelta(days=1)
-    if sdate.lower() == 'lastyear':
+    if sdate.lower() == "yesterday":
+        return date.today() - timedelta(days=1)
+    if sdate.lower() == "lastyear":
         t = date.today()
-        return date(t.year-1, t.month, t.day)
-    return datetime.strptime(sdate, '%Y-%m-%d').date()
+        return date(t.year - 1, t.month, t.day)
+    return datetime.strptime(sdate, "%Y-%m-%d").date()
 
 
-view_parser.add_argument('date', type=parse_date)
+view_parser.add_argument("date", type=parse_date)
 
 
 def _view_exec(args: Namespace) -> None:
     view(Diary.discover_and_load(diary_path), args.date)
 
 
 view_parser.set_defaults(func=_view_exec)
 
 
 def main() -> None:
     import sys
+
     try:
         if len(sys.argv) <= 1:
-            print('hyperdiary version {}'.format(__version__))
+            print("hyperdiary version {}".format(__version__))
             parser.print_help()
         else:
             args = parser.parse_args()
             args.func(args)
     except Exception as e:
         import traceback
+
         tb = sys.exc_info()[2]
-        RED = ''
+        RED = ""
         try:
             import colorama
+
             colorama.init(autoreset=True)
             RED = colorama.Back.RED
         except ImportError:
             pass
         traceback.print_tb(tb)
-        print(RED + type(e).__name__ + ': ' + str(e))
+        print(RED + type(e).__name__ + ": " + str(e))
```

### Comparing `hyperdiary-0.6.1/hyperdiary/assets/css/picnic.min.css` & `hyperdiary-0.7.0/hyperdiary/assets/css/picnic.min.css`

 * *Files identical despite different names*

### Comparing `hyperdiary-0.6.1/hyperdiary/diary.py` & `hyperdiary-0.7.0/hyperdiary/diary.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,91 +11,93 @@
 
 from .localization import Localization
 
 Pathlike = Union[Path, str]
 
 
 class DayEntry:
-    '''Diary entry for a specific date, contains multiple
-       lines of text.
-    '''
+    """Diary entry for a specific date, contains multiple
+    lines of text.
+    """
+
     def __init__(self, dt: date, lines: List[str]):
         self.dt = dt
         self.lines = lines
 
     def iter_lines(self) -> Iterable[Tuple[date, str]]:
         for line in self.lines:
             yield (self.dt, line)
 
 
 class Diary:
     def __init__(self, hyperdiary_json: Mapping) -> None:
         j = hyperdiary_json
-        self.sources = j.get('sources', [])  # type: List[str]
-        self.expected = [DateRange.from_json(obj)
-                         for obj in j.get('expected', [])] \
-            # type: List[DateRange]
+        self.sources = j.get("sources", [])  # type: List[str]
+        self.expected = [
+            DateRange.from_json(obj) for obj in j.get("expected", [])
+        ]  # type: List[DateRange]
         self.entries = list()  # type: List[DayEntry]
-        self.localization = Localization(**j.get('localization', {}))
+        self.localization = Localization(**j.get("localization", {}))
 
     def load_entries(self) -> None:
         self.entries = list()
         dates_loaded = set([])  # type: Set[date]
         for fname in self.sources:
             with open(fname) as f:
                 for dt, lines in yaml.load(f, Loader=yaml.SafeLoader).items():
-                    if not isinstance(lines, list) or \
-                            any(not isinstance(line, str) for line in lines):
-                        msg = 'Bad entry for date {}: {}'.format(dt, lines)
+                    if not isinstance(lines, list) or any(
+                        not isinstance(line, str) for line in lines
+                    ):
+                        msg = "Bad entry for date {}: {}".format(dt, lines)
                         raise BadEntryException(msg)
                     if dt in dates_loaded:
-                        msg = 'Double definition for {0} in file {1}' \
-                              .format(dt, fname)
+                        msg = "Double definition for {0} in file {1}".format(dt, fname)
                         raise Exception(msg)
                     self.entries.append(DayEntry(dt, lines))
                     dates_loaded.add(dt)
         self.entries.sort(key=lambda entry: entry.dt)
 
     def iter_lines(self) -> Iterable[Tuple[date, str]]:
         for entry in self.entries:
             yield from entry.iter_lines()
 
-    def iter_entries_by_year_and_month(self) \
-            -> Iterable[Tuple[int, Iterable[Tuple[int, Iterable[DayEntry]]]]]:
-        for year, year_entries in groupby(self.entries,
-                                          lambda entry: entry.dt.year):
-            yield year, groupby(year_entries,
-                                lambda entry: entry.dt.month)
-
-    def nested_dicts_by_year_and_month(self) \
-            -> Mapping[int, Mapping[int, Mapping[date, DayEntry]]]:
-        d = defaultdict(lambda: defaultdict(dict)) \
-            # type: Dict[int, Dict[int, Dict[date, DayEntry]]]
+    def iter_entries_by_year_and_month(
+        self,
+    ) -> Iterable[Tuple[int, Iterable[Tuple[int, Iterable[DayEntry]]]]]:
+        for year, year_entries in groupby(self.entries, lambda entry: entry.dt.year):
+            yield year, groupby(year_entries, lambda entry: entry.dt.month)
+
+    def nested_dicts_by_year_and_month(
+        self,
+    ) -> Mapping[int, Mapping[int, Mapping[date, DayEntry]]]:
+        d = defaultdict(
+            lambda: defaultdict(dict)
+        )  # type: Dict[int, Dict[int, Dict[date, DayEntry]]]
         for year, year_group in self.iter_entries_by_year_and_month():
             for month, month_entries in year_group:
                 d[year][month] = {entry.dt: entry for entry in month_entries}
         return d
 
     @staticmethod
-    def discover(subpath: Pathlike) -> 'Diary':
+    def discover(subpath: Pathlike) -> "Diary":
         path = Path(subpath).resolve()
-        while not (path / 'hyperdiary.json').exists() and len(path.parts) > 1:
+        while not (path / "hyperdiary.json").exists() and len(path.parts) > 1:
             path = path.parent
-        hyperdiary_json_path = path / 'hyperdiary.json'
+        hyperdiary_json_path = path / "hyperdiary.json"
         if not hyperdiary_json_path.exists():
-            msg = 'No hyperdiary.json found in any parent directories'
+            msg = "No hyperdiary.json found in any parent directories"
             raise FileNotFoundError(msg)
-        with open(str(hyperdiary_json_path), 'r') as f:
+        with open(str(hyperdiary_json_path), "r") as f:
             hyperdiary_json = json.load(f)
-            sources = [str(path / f) for f in hyperdiary_json['sources']]
-            hyperdiary_json['sources'] = sources
+            sources = [str(path / f) for f in hyperdiary_json["sources"]]
+            hyperdiary_json["sources"] = sources
             return Diary(hyperdiary_json)
 
     @staticmethod
-    def discover_and_load(path: Pathlike = '.') -> 'Diary':
+    def discover_and_load(path: Pathlike = ".") -> "Diary":
         diary = Diary.discover(path)
         diary.load_entries()
         return diary
 
 
 class DateRange:
     def __init__(self, start: date, end: date) -> None:
@@ -106,154 +108,148 @@
         current = self.start
         one_day = timedelta(days=1)
         while current <= self.end:
             yield current
             current += one_day
 
     @staticmethod
-    def from_json(obj: Mapping[str, str]) -> 'DateRange':
-        if 'start' not in obj:
+    def from_json(obj: Mapping[str, str]) -> "DateRange":
+        if "start" not in obj:
             raise KeyError('"start" is required in an expected date range')
-        start = datetime.strptime(obj['start'], '%Y-%m-%d').date()
-        if 'end' in obj:
-            end = datetime.strptime(obj['end'], '%Y-%m-%d').date()
+        start = datetime.strptime(obj["start"], "%Y-%m-%d").date()
+        if "end" in obj:
+            end = datetime.strptime(obj["end"], "%Y-%m-%d").date()
         else:
             end = datetime.today().date() - timedelta(days=1)
         return DateRange(start, end)
 
 
 class BadEntryException(Exception):
     pass
 
 
-def find_tags(line: str) -> Iterable['Token']:
-    '''
+def find_tags(line: str) -> Iterable["Token"]:
+    """
     >>> line = "+tag1 +tag2 some content goes here +tag3"
     >>> res = [t.text for t in find_tags(line)]
     >>> res == ["tag1", "tag2", "tag3"]
     True
-    '''
+    """
     return find_token_of_type(line, TokenType.Tag)
 
 
-def find_ids(line: str) -> Iterable['Token']:
+def find_ids(line: str) -> Iterable["Token"]:
     return find_token_of_type(line, TokenType.Id)
 
 
-def find_token_of_type(line: str, token_type: 'TokenType') \
-        -> Iterable['Token']:
+def find_token_of_type(line: str, token_type: "TokenType") -> Iterable["Token"]:
     return [token for token in tokenize(line) if token.type == token_type]
 
 
 @enum.unique
 class TokenType(enum.Enum):
     Text = 1
     Tag = 2
     Id = 3
 
 
-_REPLACEMENTS = {
-    '&': 'and',
-    'ä': 'ae',
-    'ö': 'oe',
-    'ü': 'ue',
-    'ß': 'ss',
-    '\'': ''
-}
+_REPLACEMENTS = {"&": "and", "ä": "ae", "ö": "oe", "ü": "ue", "ß": "ss", "'": ""}
 
 
 def _make_id(sid: str) -> str:
     sid = sid.lower()
     for k, v in _REPLACEMENTS.items():
         sid = sid.replace(k, v)
-    assert ' ' not in sid, sid
+    assert " " not in sid, sid
     return sid
 
 
 def _capitalize(s: str) -> Iterable[str]:
     up = True
     for letter in s:
         if up:
             yield letter.upper()
             up = False
         else:
-            if letter == ' ':
+            if letter == " ":
                 up = True
             yield letter
 
 
 def _beautify_id(sid: str) -> str:
-    return ''.join(_capitalize(sid.replace('_', ' ')))
+    return "".join(_capitalize(sid.replace("_", " ")))
 
 
 class Token:
-    def __init__(self, type: TokenType, text: str, ref: str = None) -> None:
+    def __init__(self, type: TokenType, text: str, ref: Optional[str] = None) -> None:
         self.type = type
         self.text = text
         self.ref = ref
         if type == TokenType.Id:
             if not ref:
-                s = text.split('|', 1)
+                s = text.split("|", 1)
                 self.text = _beautify_id(s[1] if len(s) == 2 else s[0])
                 self.ref = _make_id(s[0])
 
     def __repr__(self) -> str:
-        return 'Token({0}, "{1}", "{2}")'.format(self.type, self.text,
-                                                 self.ref)
+        return 'Token({0}, "{1}", "{2}")'.format(self.type, self.text, self.ref)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Token):
             return False
         if self.type == TokenType.Id and other.type == TokenType.Id:
             return self.ref == other.ref
-        return self.type == other.type and self.text == other.text \
+        return (
+            self.type == other.type
+            and self.text == other.text
             and self.ref == other.ref
+        )
 
     def __hash__(self) -> int:
         if self.type == TokenType.Id:
             return hash(self.type) ^ hash(self.ref)
         return hash(self.type) ^ hash(self.text) ^ hash(self.ref)
 
-    def __lt__(self, other: 'Token') -> bool:
+    def __lt__(self, other: "Token") -> bool:
         return self.text < other.text
 
 
-_re_separator = re.compile(r' |;|,|\)|\.')
+_re_separator = re.compile(r" |;|,|\)|\.")
 
 
 def _fragmented_tokenize(line: str) -> Iterable[Token]:
     current = []  # type: List[str]
     current_type = TokenType.Text
     for letter in line:
         if _re_separator.match(letter):
             if current:
-                yield Token(current_type, ''.join(current))
+                yield Token(current_type, "".join(current))
             yield Token(TokenType.Text, letter)
             current = []
             current_type = TokenType.Text
             continue
         if not current:
-            if letter == '+':
+            if letter == "+":
                 current_type = TokenType.Tag
-            elif letter == '$':
+            elif letter == "$":
                 current_type = TokenType.Id
             else:
                 current_type = TokenType.Text
-            current.append(letter if current_type == TokenType.Text else '')
+            current.append(letter if current_type == TokenType.Text else "")
             continue
         current.append(letter)
     if current:
-        yield Token(current_type, ''.join(current))
+        yield Token(current_type, "".join(current))
 
 
 def tokenize(line: str) -> Iterable[Token]:
-    text_token = Token(TokenType.Text, '')
+    text_token = Token(TokenType.Text, "")
     for next in _fragmented_tokenize(line):
         if next.type == TokenType.Text:
             text_token = Token(TokenType.Text, text_token.text + next.text)
         else:
             if text_token.text:
                 yield text_token
-                text_token = Token(TokenType.Text, '')
+                text_token = Token(TokenType.Text, "")
             yield next
     if text_token.text:
         yield text_token
```

### Comparing `hyperdiary-0.6.1/hyperdiary/html.py` & `hyperdiary-0.7.0/hyperdiary/html.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,97 +1,123 @@
 import os
 from datetime import timedelta, date
 from collections import defaultdict
 from typing import Iterable, Dict, Union, Callable, Optional  # noqa: F401
 from . import diary
 from .localization import Localization
 from .simplepath import AbsolutePath, RelativePath
-from .htmltags import article, header, head, h1, h4, ul, li, a, span, div, \
-    footer, meta, link, style, html, body, title, HTMLElement, HTMLContent
-
-
-def wrap_page(body_content: HTMLContent, page_title: str = None,
-              encoding: str = 'utf-8', css_references: Iterable[str] = [],
-              inline_css: str = None) -> html:
+from .htmltags import (
+    article,
+    header,
+    head,
+    h1,
+    h4,
+    ul,
+    li,
+    a,
+    span,
+    div,
+    footer,
+    meta,
+    link,
+    style,
+    html,
+    body,
+    title,
+    HTMLElement,
+    HTMLContent,
+)
+
+
+def wrap_page(
+    body_content: HTMLContent,
+    page_title: Optional[str] = None,
+    encoding: str = "utf-8",
+    css_references: Iterable[str] = [],
+    inline_css: Optional[str] = None,
+) -> html:
     h = head(
-            meta(charset=encoding),
-            meta(name='viewport',
-                 content='width=device-width, initial-scale=1')
-        )
+        meta(charset=encoding),
+        meta(name="viewport", content="width=device-width, initial-scale=1"),
+    )
     if page_title:
         h.append(title(page_title))
     for css in css_references:
         h.append(link(href=css, rel="stylesheet"))
     if inline_css:
         h.append(style(inline_css))
     return html(h, body(body_content))
 
 
-def day_to_html(current: date, entry: Iterable[str],
-                localization: Localization,
-                link_to_id_fn: Callable[[Optional[str]], str] = None) \
-        -> HTMLElement:
-    day = article(_class='card', _id=str(path_for_date(current)))(
-                header(h4(localization.format_date(current)))
-            )
+def day_to_html(
+    current: date,
+    entry: Iterable[str],
+    localization: Localization,
+    link_to_id_fn: Optional[Callable[[Optional[str]], str]] = None,
+) -> HTMLElement:
+    day = article(_class="card", _id=str(path_for_date(current)))(
+        header(h4(localization.format_date(current)))
+    )
     day_list = day.subelement(ul())
     for e in entry:
         if isinstance(e, str):
             eli = li()
             if link_to_id_fn:
                 tags_to_print = []
                 for token in diary.tokenize(e):
                     if token.type == diary.TokenType.Id:
-                        eli.append(a(token.text,
-                                     href=link_to_id_fn(token.ref)))
+                        eli.append(a(token.text, href=link_to_id_fn(token.ref)))
                     elif token.type == diary.TokenType.Text:
                         eli.append(span(token.text))
                     elif token.type == diary.TokenType.Tag:
                         tags_to_print.append(token)
                     else:
-                        raise NotImplementedError('Unknown TokenType')
+                        raise NotImplementedError("Unknown TokenType")
                 for tag in tags_to_print:
-                    eli.append(' ')
-                    eli.append(span(tag.text, _class='tag'))
+                    eli.append(" ")
+                    eli.append(span(tag.text, _class="tag"))
             else:
                 eli.append(e)
             day_list.append(eli)
     return day
 
 
-def wrap_html_page(content: HTMLContent, title: str = None, level: int = 0) \
-        -> html:
+def wrap_html_page(
+    content: HTMLContent, title: Optional[str] = None, level: int = 0
+) -> html:
     return wrap_page(
-        div(content, _class='content'),
+        div(content, _class="content"),
         page_title=title,
-        css_references=[('../'*level) + 'assets/css/picnic.min.css'],
-        inline_css='.content { max-width: 800px; margin: auto; '
-                   'font-family: lato, sans-serif;}'
-                   '.tag { background-color: #ffeeaa;}'
+        css_references=[("../" * level) + "assets/css/picnic.min.css"],
+        inline_css=".content { max-width: 800px; margin: auto; "
+        "font-family: lato, sans-serif;}"
+        ".tag { background-color: #ffeeaa;}",
     )
 
 
 def diary_to_html(diary_instance: diary.Diary, fname: str) -> None:
     entries = diary_instance.entries
 
-    content = div(h1('Entries'))
+    content = div(h1("Entries"))
     entries_html = content.subelement(div())
 
     for entry in entries:
-        entries_html.append(day_to_html(entry.dt, entry.lines,
-                                        diary_instance.localization,
-                                        lambda ref: '#'))
+        entries_html.append(
+            day_to_html(
+                entry.dt, entry.lines, diary_instance.localization, lambda ref: "#"
+            )
+        )
 
-    wrap_html_page(content, title='Diary').write(fname)
+    wrap_html_page(content, title="Diary").write(fname)
 
 
 def diary_to_html_folder(diary_instance: diary.Diary, folder: str) -> None:
-    root_path = AbsolutePath('/')
-    entries_path = AbsolutePath('/entries')
-    ids_path = AbsolutePath('/ids')
+    root_path = AbsolutePath("/")
+    entries_path = AbsolutePath("/entries")
+    ids_path = AbsolutePath("/ids")
 
     loc = diary_instance.localization
 
     def folder_from_path(p: AbsolutePath) -> str:
         return os.path.join(folder, str(p - root_path))
 
     entries_ul = ul()
@@ -99,95 +125,102 @@
     identifiers = defaultdict(list)  # type: Dict[diary.Token, list]
 
     for year, year_group in diary_instance.iter_entries_by_year_and_month():
         year_path = entries_path + rel_path(year)
         year_ul = ul()
 
         for month, month_entries in year_group:
-            s_month = '{:02d}'.format(month)
+            s_month = "{:02d}".format(month)
             month_path = year_path + rel_path(s_month)
-            month_html = div(h1('{} {}'.format(loc.get_month(month-1), year)))
+            month_html = div(h1("{} {}".format(loc.get_month(month - 1), year)))
             month_ul = month_html.subelement(ul())
 
             for entry in month_entries:
                 current = entry.dt
-                s_day = '{:02d}'.format(current.day)
+                s_day = "{:02d}".format(current.day)
                 day_path = month_path + rel_path(s_day)
                 day_folder = folder_from_path(day_path)
                 os.makedirs(day_folder, exist_ok=True)
 
                 def link_to_id_fn(sid: Optional[str]) -> str:
-                    assert sid is not None, \
-                        'Got invalid identifier {}'.format(sid)
+                    assert sid is not None, "Got invalid identifier {}".format(sid)
                     return str(ids_path + rel_path(sid) - day_path)
 
-                day_html = day_to_html(current, entry.lines,
-                                       diary_instance.localization,
-                                       link_to_id_fn)
+                day_html = day_to_html(
+                    current, entry.lines, diary_instance.localization, link_to_id_fn
+                )
 
-                foot = div(_class='flex four')
+                foot = div(_class="flex four")
                 day_html.append(footer(foot))
                 yesterday = current - timedelta(days=1)
-                foot.append(div(a('Yesterday ({})'.format(yesterday),
-                                href=str(path_for_date(yesterday) - day_path)))
-                            )
+                foot.append(
+                    div(
+                        a(
+                            "Yesterday ({})".format(yesterday),
+                            href=str(path_for_date(yesterday) - day_path),
+                        )
+                    )
+                )
 
                 tomorrow = current + timedelta(days=1)
-                foot.append(div(a('Tomorrow ({})'.format(tomorrow),
-                                  href=str(path_for_date(tomorrow) -
-                                           day_path)),
-                                _class='off-fourth'))
+                foot.append(
+                    div(
+                        a(
+                            "Tomorrow ({})".format(tomorrow),
+                            href=str(path_for_date(tomorrow) - day_path),
+                        ),
+                        _class="off-fourth",
+                    )
+                )
 
-                index_path = os.path.join(day_folder, 'index.html')
+                index_path = os.path.join(day_folder, "index.html")
                 wrap_html_page(day_html, level=4).write(index_path)
                 append_li_a(month_ul, str(current), str(day_path - month_path))
 
                 for dt, e in entry.iter_lines():
                     for identifier in diary.find_ids(e):
                         identifiers[identifier].append(dt)
 
-            index_path = os.path.join(folder_from_path(month_path),
-                                      'index.html')
+            index_path = os.path.join(folder_from_path(month_path), "index.html")
             wrap_html_page(month_html, level=3).write(index_path)
-            append_li_a(year_ul, loc.get_month(month-1), s_month)
+            append_li_a(year_ul, loc.get_month(month - 1), s_month)
 
-        index_path = os.path.join(folder_from_path(year_path), 'index.html')
+        index_path = os.path.join(folder_from_path(year_path), "index.html")
         wrap_html_page(year_ul, level=2).write(index_path)
         append_li_a(entries_ul, str(year), str(year))
 
-    index_path = os.path.join(folder_from_path(entries_path), 'index.html')
+    index_path = os.path.join(folder_from_path(entries_path), "index.html")
     wrap_html_page(entries_ul, level=1).write(index_path)
 
     ids_ul = ul()
     for identifier, days in sorted(identifiers.items()):
-        assert identifier.ref is not None, \
-            '{} has broken ref'.format(identifier)
+        assert identifier.ref is not None, "{} has broken ref".format(identifier)
         id_path = ids_path + rel_path(identifier.ref)
         id_folder = folder_from_path(id_path)
         os.makedirs(id_folder, exist_ok=True)
         append_li_a(ids_ul, identifier.text, str(id_path - ids_path))
         identifier_ul = ul()
         for day in days:
-            append_li_a(identifier_ul, str(day), str(path_for_date(day) -
-                                                     id_path))
-        index_path = os.path.join(id_folder, 'index.html')
+            append_li_a(identifier_ul, str(day), str(path_for_date(day) - id_path))
+        index_path = os.path.join(id_folder, "index.html")
         wrap_html_page(identifier_ul, level=2).write(index_path)
-    index_path = os.path.join(folder_from_path(ids_path), 'index.html')
+    index_path = os.path.join(folder_from_path(ids_path), "index.html")
     wrap_html_page(ids_ul, level=1).write(index_path)
     import shutil
-    shutil.rmtree(os.path.join(folder, 'assets'), ignore_errors=True)
-    shutil.copytree(os.path.join(os.path.dirname(__file__), 'assets'),
-                    os.path.join(folder, 'assets'))
+
+    shutil.rmtree(os.path.join(folder, "assets"), ignore_errors=True)
+    shutil.copytree(
+        os.path.join(os.path.dirname(__file__), "assets"),
+        os.path.join(folder, "assets"),
+    )
 
 
 def rel_path(spath: Union[date, str, int]) -> RelativePath:
     return RelativePath(str(spath))
 
 
 def path_for_date(dt: date) -> AbsolutePath:
-    return AbsolutePath('/entries/{}/{:02d}/{:02d}'.format(dt.year,
-                                                           dt.month,
-                                                           dt.day))
+    return AbsolutePath("/entries/{}/{:02d}/{:02d}".format(dt.year, dt.month, dt.day))
 
 
 def append_li_a(ul: HTMLElement, text: str, href: str) -> None:
     ul.append(li(a(text, href=href)))
```

### Comparing `hyperdiary-0.6.1/hyperdiary/htmltags.py` & `hyperdiary-0.7.0/hyperdiary/htmltags.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,253 +1,253 @@
 from typing import Iterable, Union
 
-HTMLContent = Union['HTMLElement', str]
+HTMLContent = Union["HTMLElement", str]
 
-_escaped_attrs = ('id', 'class', 'type')
+_escaped_attrs = ("id", "class", "type")
 
 
 class HTMLElement(object):
-    tag = 'div'  # type: str
+    tag = "div"  # type: str
     render_compact = False  # type: bool
 
     def __init__(self, *content: HTMLContent, **attributes: str) -> None:
         self.content = list(content)
         self.attributes = attributes
         for a in _escaped_attrs:
-            if '_' + a in self.attributes:
-                self.attributes[a] = self.attributes.pop('_' + a)
+            if "_" + a in self.attributes:
+                self.attributes[a] = self.attributes.pop("_" + a)
 
-    def append(self, *items: HTMLContent) -> 'HTMLElement':
+    def append(self, *items: HTMLContent) -> "HTMLElement":
         self.content += items
         return self
 
-    def __call__(self, *items: HTMLContent) -> 'HTMLElement':
+    def __call__(self, *items: HTMLContent) -> "HTMLElement":
         return self.append(*items)
 
-    def subelement(self, item: 'HTMLElement') -> 'HTMLElement':
+    def subelement(self, item: "HTMLElement") -> "HTMLElement":
         self.content.append(item)
         return item
 
     def lazy_render_attributes(self) -> Iterable[str]:
         if self.attributes:
             for k, v in self.attributes.items():
-                yield ' '
+                yield " "
                 yield str(k)
                 yield '="'
                 yield str(v)
                 yield '"'
 
-    def lazy_render(self, indent: str = '', add_indent: str = '') \
-            -> Iterable[str]:
-        is_doc_root = self.tag.lower() == 'html'
+    def lazy_render(self, indent: str = "", add_indent: str = "") -> Iterable[str]:
+        is_doc_root = self.tag.lower() == "html"
         if is_doc_root:
-            yield '<!DOCTYPE HTML>\n'
+            yield "<!DOCTYPE HTML>\n"
         do_linebreak = not self.render_compact and self.content
         yield indent
-        yield '<'
+        yield "<"
         yield self.tag
         yield from self.lazy_render_attributes()
-        yield '>'
+        yield ">"
         if do_linebreak:
-            yield '\n'
-        child_indent = indent + add_indent if do_linebreak else ''
+            yield "\n"
+        child_indent = indent + add_indent if do_linebreak else ""
         if not do_linebreak:
-            add_indent = ''
+            add_indent = ""
         for child in self.content:
             if isinstance(child, HTMLElement):
                 yield from child.lazy_render(child_indent, add_indent)
             else:
-                yield '{}{}'.format(child_indent, child)
+                yield "{}{}".format(child_indent, child)
             if do_linebreak:
-                yield '\n'
+                yield "\n"
         if do_linebreak:
             yield indent
-        yield '</'
+        yield "</"
         yield self.tag
-        yield '>'
+        yield ">"
         if is_doc_root:
-            yield '\n'
+            yield "\n"
 
     def __str__(self) -> str:
-        '''Render element to string.
+        """Render element to string.
         >>> str(a('Somewhere', href="#"))
         '<a href="#">Somewhere</a>'
         >>> str(p())
         '<p></p>'
         >>> str(div('Hello World'))
         '<div>\\n  Hello World\\n</div>'
         >>> str(table())
         '<table></table>'
-        '''
-        return ''.join(self.lazy_render(add_indent='  '))
+        """
+        return "".join(self.lazy_render(add_indent="  "))
 
     def write(self, fname: str) -> None:
-        with open(fname, 'w') as f:
-            for s in self.lazy_render(add_indent='  '):
+        with open(fname, "w") as f:
+            for s in self.lazy_render(add_indent="  "):
                 f.write(s)
 
 
 # TAGS
 
-class a (HTMLElement):
-    tag = 'a'
+
+class a(HTMLElement):
+    tag = "a"
     render_compact = True
 
 
-class article (HTMLElement):
-    tag = 'article'
+class article(HTMLElement):
+    tag = "article"
     render_compact = False
 
 
-class body (HTMLElement):
-    tag = 'body'
+class body(HTMLElement):
+    tag = "body"
     render_compact = False
 
 
-class button (HTMLElement):
-    tag = 'button'
+class button(HTMLElement):
+    tag = "button"
     render_compact = True
 
 
-class div (HTMLElement):
-    tag = 'div'
+class div(HTMLElement):
+    tag = "div"
     render_compact = False
 
 
-class footer (HTMLElement):
-    tag = 'footer'
+class footer(HTMLElement):
+    tag = "footer"
     render_compact = False
 
 
-class form (HTMLElement):
-    tag = 'form'
+class form(HTMLElement):
+    tag = "form"
     render_compact = False
 
 
-class h1 (HTMLElement):
-    tag = 'h1'
+class h1(HTMLElement):
+    tag = "h1"
     render_compact = True
 
 
-class h2 (HTMLElement):
-    tag = 'h2'
+class h2(HTMLElement):
+    tag = "h2"
     render_compact = True
 
 
-class h3 (HTMLElement):
-    tag = 'h3'
+class h3(HTMLElement):
+    tag = "h3"
     render_compact = True
 
 
-class h4 (HTMLElement):
-    tag = 'h4'
+class h4(HTMLElement):
+    tag = "h4"
     render_compact = True
 
 
-class head (HTMLElement):
-    tag = 'head'
+class head(HTMLElement):
+    tag = "head"
     render_compact = False
 
 
-class header (HTMLElement):
-    tag = 'header'
+class header(HTMLElement):
+    tag = "header"
     render_compact = False
 
 
-class hr (HTMLElement):
-    tag = 'hr'
+class hr(HTMLElement):
+    tag = "hr"
     render_compact = False
 
 
-class html (HTMLElement):
-    tag = 'html'
+class html(HTMLElement):
+    tag = "html"
     render_compact = False
 
 
-class img (HTMLElement):
-    tag = 'img'
+class img(HTMLElement):
+    tag = "img"
     render_compact = False
 
 
-class li (HTMLElement):
-    tag = 'li'
+class li(HTMLElement):
+    tag = "li"
     render_compact = True
 
 
-class link (HTMLElement):
-    tag = 'link'
+class link(HTMLElement):
+    tag = "link"
     render_compact = False
 
 
-class meta (HTMLElement):
-    tag = 'meta'
+class meta(HTMLElement):
+    tag = "meta"
     render_compact = False
 
 
-class nav (HTMLElement):
-    tag = 'nav'
+class nav(HTMLElement):
+    tag = "nav"
     render_compact = False
 
 
-class ol (HTMLElement):
-    tag = 'ol'
+class ol(HTMLElement):
+    tag = "ol"
     render_compact = False
 
 
-class p (HTMLElement):
-    tag = 'p'
+class p(HTMLElement):
+    tag = "p"
     render_compact = True
 
 
-class small (HTMLElement):
-    tag = 'small'
+class small(HTMLElement):
+    tag = "small"
     render_compact = True
 
 
-class span (HTMLElement):
-    tag = 'span'
+class span(HTMLElement):
+    tag = "span"
     render_compact = True
 
 
-class style (HTMLElement):
-    tag = 'style'
+class style(HTMLElement):
+    tag = "style"
     render_compact = False
 
 
-class table (HTMLElement):
-    tag = 'table'
+class table(HTMLElement):
+    tag = "table"
     render_compact = False
 
 
-class tbody (HTMLElement):
-    tag = 'tbody'
+class tbody(HTMLElement):
+    tag = "tbody"
     render_compact = False
 
 
-class td (HTMLElement):
-    tag = 'td'
+class td(HTMLElement):
+    tag = "td"
     render_compact = True
 
 
-class th (HTMLElement):
-    tag = 'th'
+class th(HTMLElement):
+    tag = "th"
     render_compact = False
 
 
-class thead (HTMLElement):
-    tag = 'thead'
+class thead(HTMLElement):
+    tag = "thead"
     render_compact = False
 
 
-class title (HTMLElement):
-    tag = 'title'
+class title(HTMLElement):
+    tag = "title"
     render_compact = True
 
 
-class tr (HTMLElement):
-    tag = 'tr'
+class tr(HTMLElement):
+    tag = "tr"
     render_compact = False
 
 
-class ul (HTMLElement):
-    tag = 'ul'
+class ul(HTMLElement):
+    tag = "ul"
     render_compact = False
```

### Comparing `hyperdiary-0.6.1/hyperdiary/hugo.py` & `hyperdiary-0.7.0/hyperdiary/hugo.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,43 +5,44 @@
 
 
 def nice_date(dt: date) -> str:
     return dt.strftime("%d.%m.%Y")
 
 
 def diary_to_hugo(diary_instance: diary.Diary, folder: diary.Pathlike) -> None:
-    content_dir = os.path.join(str(folder), 'content')
+    content_dir = os.path.join(str(folder), "content")
     os.makedirs(content_dir, exist_ok=True)
 
     for entry in diary_instance.entries:
         current = entry.dt
-        month_dir = os.path.join(content_dir, 'post',
-                                 '{:04d}'.format(current.year),
-                                 '{:02d}'.format(current.month))
+        month_dir = os.path.join(
+            content_dir,
+            "post",
+            "{:04d}".format(current.year),
+            "{:02d}".format(current.month),
+        )
         os.makedirs(month_dir, exist_ok=True)
-        with open(os.path.join(month_dir,
-                               '{:02d}.md'.format(current.day)), 'w') as f:
+        with open(os.path.join(month_dir, "{:02d}.md".format(current.day)), "w") as f:
             tags = []
             day_text = io.StringIO()
             for line in entry.lines:
-                day_text.write('- ')
+                day_text.write("- ")
                 for token in diary.tokenize(line):
                     if token.type == diary.TokenType.Id:
-                        day_text.write('[{}](#{})'.format(token.text,
-                                                          token.ref))
+                        day_text.write("[{}](#{})".format(token.text, token.ref))
                     elif token.type == diary.TokenType.Text:
                         day_text.write(token.text)
                     elif token.type == diary.TokenType.Tag:
                         tags.append(token.text)
                     else:
-                        raise NotImplementedError('Unknown TokenType')
-                day_text.write('\n')
-            f.write('+++\n')
+                        raise NotImplementedError("Unknown TokenType")
+                day_text.write("\n")
+            f.write("+++\n")
             f.write('title = "{0}"\n'.format(nice_date(current)))
             f.write('date = "{0}"\n'.format(current.isoformat()))
             f.write('categories = ["day"]\n')
-            f.write('draft = false\n')
-            f.write('tags = {}\n'.format(tags))
-            f.write('\n+++\n\n')
+            f.write("draft = false\n")
+            f.write("tags = {}\n".format(tags))
+            f.write("\n+++\n\n")
             day_text.seek(0)
             f.write(day_text.read())
-            f.write('\n')
+            f.write("\n")
```

### Comparing `hyperdiary-0.6.1/hyperdiary/localization.py` & `hyperdiary-0.7.0/hyperdiary/localization.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,94 @@
 from typing import List
 from datetime import date
 
-MONTHS_EN = ['January', 'February', 'March', 'April', 'May', 'June',
-             'July', 'August', 'September', 'October', 'November',
-             'December']
+MONTHS_EN = [
+    "January",
+    "February",
+    "March",
+    "April",
+    "May",
+    "June",
+    "July",
+    "August",
+    "September",
+    "October",
+    "November",
+    "December",
+]
 
-DAYS_SHORT_EN = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
+DAYS_SHORT_EN = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
 
 
 class Localization:
-    def __init__(self,
-                 months: List[str] = MONTHS_EN,
-                 days_short: List[str] = DAYS_SHORT_EN,
-                 date_fmt: str = '%Y-%m-%d') \
-            -> None:
+    def __init__(
+        self,
+        months: List[str] = MONTHS_EN,
+        days_short: List[str] = DAYS_SHORT_EN,
+        date_fmt: str = "%Y-%m-%d",
+    ) -> None:
         assert len(months) == 12
         self.months = months
         assert len(days_short) == 7
         self.days_short = days_short
         self.date_fmt = date_fmt
 
     def get_month(self, i: int) -> str:
-        '''Get the localized name of month i (zero-based index).
-           >>> l = Localization()
-           >>> l.get_month(0)
-           'January'
-           >>> l.get_month(11)
-           'December'
-           >>> l.get_month(12)
-           Traceback (most recent call last):
-           ...
-           AssertionError
-           >>> Localization(months=['Just January'])
-           Traceback (most recent call last):
-           ...
-           AssertionError
-           >>> l2 = Localization(months=list('123456789ond'))
-           >>> l2.get_month(3)
-           '4'
-           >>> l2.get_month(10)
-           'n'
-        '''
+        """Get the localized name of month i (zero-based index).
+        >>> l = Localization()
+        >>> l.get_month(0)
+        'January'
+        >>> l.get_month(11)
+        'December'
+        >>> l.get_month(12)
+        Traceback (most recent call last):
+        ...
+        AssertionError
+        >>> Localization(months=['Just January'])
+        Traceback (most recent call last):
+        ...
+        AssertionError
+        >>> l2 = Localization(months=list('123456789ond'))
+        >>> l2.get_month(3)
+        '4'
+        >>> l2.get_month(10)
+        'n'
+        """
         assert i >= 0
         assert i < 12
         return self.months[i]
 
     def get_day_short(self, i: int) -> str:
-        '''Get the localized name of day i (zero-based index starting Monday).
-           >>> l = Localization()
-           >>> l.get_day_short(0)
-           'Mon'
-           >>> l.get_day_short(6)
-           'Sun'
-           >>> l.get_day_short(7)
-           Traceback (most recent call last):
-           ...
-           AssertionError
-           >>> Localization(days_short=['Just Mon'])
-           Traceback (most recent call last):
-           ...
-           AssertionError
-           >>> l2 = Localization(days_short=list('1234567'))
-           >>> l2.get_day_short(3)
-           '4'
-           >>> l2.get_day_short(6)
-           '7'
-        '''
+        """Get the localized name of day i (zero-based index starting Monday).
+        >>> l = Localization()
+        >>> l.get_day_short(0)
+        'Mon'
+        >>> l.get_day_short(6)
+        'Sun'
+        >>> l.get_day_short(7)
+        Traceback (most recent call last):
+        ...
+        AssertionError
+        >>> Localization(days_short=['Just Mon'])
+        Traceback (most recent call last):
+        ...
+        AssertionError
+        >>> l2 = Localization(days_short=list('1234567'))
+        >>> l2.get_day_short(3)
+        '4'
+        >>> l2.get_day_short(6)
+        '7'
+        """
         assert i >= 0
         assert i < 7
         return self.days_short[i]
 
     def format_date(self, dt: date) -> str:
-        '''Format to localized string.
-           >>> l = Localization()
-           >>> l.format_date(date(2019, 11, 3))
-           '2019-11-03'
-           >>> l = Localization(date_fmt='%d.%m.%Y')
-           >>> l.format_date(date(2019, 11, 3))
-           '03.11.2019'
-        '''
+        """Format to localized string.
+        >>> l = Localization()
+        >>> l.format_date(date(2019, 11, 3))
+        '2019-11-03'
+        >>> l = Localization(date_fmt='%d.%m.%Y')
+        >>> l.format_date(date(2019, 11, 3))
+        '03.11.2019'
+        """
         return dt.strftime(self.date_fmt)
```

### Comparing `hyperdiary-0.6.1/hyperdiary/simplepath.py` & `hyperdiary-0.7.0/hyperdiary/simplepath.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,19 @@
     pass
 
 
 class NotAnAbsolutePathError(InvalidPathError):
     pass
 
 
-_valid_path_chars = 'abcdefghijklmnopqrstuvwxyz0123456789-_.'
+_valid_path_chars = "abcdefghijklmnopqrstuvwxyz0123456789-_."
 
 
-def _validate_and_shorten(is_absolute: bool, elements: Iterable[str]) \
-        -> List[str]:
-    '''
+def _validate_and_shorten(is_absolute: bool, elements: Iterable[str]) -> List[str]:
+    """
     >>> _validate_and_shorten(True, ['a', 'b', 'c', '..', '..'])
     ['a']
 
     >>> _validate_and_shorten(False, ['..', '..'])
     ['..', '..']
 
     >>> _validate_and_shorten(True, ['..', '..'])
@@ -43,81 +42,82 @@
     []
     >>> _validate_and_shorten(False, [''])
     []
     >>> _validate_and_shorten(False, [])
     []
     >>> _validate_and_shorten(False, ['.'])
     []
-    '''
+    """
     new_elements = []  # type: List[str]
     for el in elements:
-        if el == '.' or not el:
+        if el == "." or not el:
             continue
-        elif el == '..':
+        elif el == "..":
             if not new_elements:
                 if is_absolute:
-                    raise InvalidPathError('traversing over root')
+                    raise InvalidPathError("traversing over root")
                 else:
-                    new_elements.append('..')
+                    new_elements.append("..")
             else:
-                if new_elements[-1] == '..':
-                    new_elements.append('..')
+                if new_elements[-1] == "..":
+                    new_elements.append("..")
                 else:
                     new_elements.pop()
         else:
             if not all(c in _valid_path_chars for c in el):
-                raise InvalidPathError('invalid character in path element "{}"'
-                                       .format(el))
+                raise InvalidPathError(
+                    'invalid character in path element "{}"'.format(el)
+                )
             new_elements.append(el)
     return new_elements
 
 
 class RelativePath:
     def __init__(self, path: str) -> None:
-        '''
+        """
         >>> RelativePath('a/b/c')
         RelativePath('./a/b/c')
 
         >>> RelativePath('..')
         RelativePath('..')
 
         >>> RelativePath('.')
         RelativePath('.')
 
         >>> RelativePath('')
         RelativePath('.')
-        '''
-        if path.startswith('/'):
+        """
+        if path.startswith("/"):
             raise NotARelativePathError(path)
-        self.elements = _validate_and_shorten(False, path.split('/'))
+        self.elements = _validate_and_shorten(False, path.split("/"))
 
     def __str__(self) -> str:
-        '''
+        """
         >>> str(RelativePath('a/b/c'))
         './a/b/c'
-        '''
-        prefix = '.' + ('/' if self.elements else '')
-        if self.elements and self.elements[0] == '..':
-            prefix = ''
-        return prefix + '/'.join(self.elements)
+        """
+        prefix = "." + ("/" if self.elements else "")
+        if self.elements and self.elements[0] == "..":
+            prefix = ""
+        return prefix + "/".join(self.elements)
 
     def __repr__(self) -> str:
-        '''
+        """
         >>> RelativePath('d/e/f')
         RelativePath('./d/e/f')
 
         >>> RelativePath('./../f')
         RelativePath('../f')
-        '''
-        return 'RelativePath(\'{}\')'.format(self)
+        """
+        return "RelativePath('{}')".format(self)
 
 
 class AbsolutePath:
     def __init__(self, path: str) -> None:
-        '''
+        """
         >>> AbsolutePath('/a/b/c')
         AbsolutePath('/a/b/c')
 
         >>> AbsolutePath('/')
         AbsolutePath('/')
 
         >>> AbsolutePath('/folder/index.html')
@@ -128,42 +128,41 @@
             ...
         hyperdiary.simplepath.NotAnAbsolutePathError: a/b/c
 
         >>> AbsolutePath('')
         Traceback (most recent call last):
             ...
         hyperdiary.simplepath.NotAnAbsolutePathError
-        '''
-        if not path.startswith('/'):
+        """
+        if not path.startswith("/"):
             raise NotAnAbsolutePathError(path)
-        self.elements = _validate_and_shorten(True, path.split('/'))
+        self.elements = _validate_and_shorten(True, path.split("/"))
 
     def __eq__(self, other: object) -> bool:
-        '''
+        """
         >>> AbsolutePath('/a/b/c') == AbsolutePath('/a/b/c')
         True
 
         >>> AbsolutePath('/a/b/c') == AbsolutePath('/a/./b/c/../c')
         True
 
         >>> AbsolutePath('/a/b/c') == AbsolutePath('/a')
         False
 
         >>> AbsolutePath('/a/b/c') != AbsolutePath('/a')
         True
-        '''
+        """
         if not isinstance(other, AbsolutePath):
             return False
         if not len(self.elements) == len(other.elements):
             return False
-        return all(el1 == el2 for el1, el2 in zip(self.elements,
-                                                  other.elements))
+        return all(el1 == el2 for el1, el2 in zip(self.elements, other.elements))
 
-    def __add__(self, other: RelativePath) -> 'AbsolutePath':
-        '''
+    def __add__(self, other: RelativePath) -> "AbsolutePath":
+        """
         >>> AbsolutePath('/a/b/c') + RelativePath('d/e/f')
         AbsolutePath('/a/b/c/d/e/f')
 
         >>> AbsolutePath('/a/b/c') + RelativePath('../..')
         AbsolutePath('/a')
 
         >>> AbsolutePath('/a/b/c') + RelativePath('../../..')
@@ -173,50 +172,50 @@
         Traceback (most recent call last):
             ...
         hyperdiary.simplepath.InvalidPathError: traversing over root
 
         >>> AbsolutePath('/a/b/c/././') + RelativePath('../../../x/y') \
             == AbsolutePath('/x/y')
         True
-        '''
-        return AbsolutePath('{}/{}'.format(self, other))
+        """
+        return AbsolutePath("{}/{}".format(self, other))
 
-    def __sub__(self, other: 'AbsolutePath') -> RelativePath:
-        '''
+    def __sub__(self, other: "AbsolutePath") -> RelativePath:
+        """
         >>> AbsolutePath('/a/b/c') - AbsolutePath('/a/b/c')
         RelativePath('.')
 
         >>> AbsolutePath('/a/b/c') - AbsolutePath('/a/b/x')
         RelativePath('../c')
 
         >>> AbsolutePath('/a/b/c') - AbsolutePath('/d/e/f')
         RelativePath('../../../a/b/c')
 
         >>> a = AbsolutePath('/a/b/c'); b = AbsolutePath('/a/x/y')
         >>> b + (a - b) == a
         True
         >>> a + (b - a) == b
         True
-        '''
+        """
         e1 = self.elements.copy()
         e2 = other.elements.copy()
         while e1 and e2 and e1[0] == e2[0]:
             e1.pop(0)
             e2.pop(0)
-        return RelativePath('../' * len(e2) + '/'.join(e1))
+        return RelativePath("../" * len(e2) + "/".join(e1))
 
     def __str__(self) -> str:
-        '''
+        """
         >>> str(AbsolutePath('/a/b/c'))
         '/a/b/c'
-        '''
-        return '/' + '/'.join(self.elements)
+        """
+        return "/" + "/".join(self.elements)
 
     def __repr__(self) -> str:
-        '''
+        """
         >>> AbsolutePath('/a/b/c')
         AbsolutePath('/a/b/c')
-        '''
-        return 'AbsolutePath(\'{}\')'.format(self)
+        """
+        return "AbsolutePath('{}')".format(self)
 
     def __hash__(self) -> int:
         return hash(repr(self))
```

### Comparing `hyperdiary-0.6.1/hyperdiary/stats.py` & `hyperdiary-0.7.0/hyperdiary/stats.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from collections import OrderedDict
 from typing import Dict
 from .diary import find_tags, find_ids, Diary
 
 
 def stats(diary: Diary) -> Dict[str, int]:
     output = OrderedDict()  # type: Dict[str, int]
-    output['# Days'] = len(diary.entries)
-    output['# Lines'] = sum(len(entry.lines) for entry in diary.entries)
-    output['# Taggings'] = sum(len(list(find_tags(l)))
-                               for d, l in diary.iter_lines())
-    output['# Identifications'] = sum(len(list(find_ids(l)))
-                                      for d, l in diary.iter_lines())
+    output["# Days"] = len(diary.entries)
+    output["# Lines"] = sum(len(entry.lines) for entry in diary.entries)
+    output["# Taggings"] = sum(len(list(find_tags(l))) for d, l in diary.iter_lines())
+    output["# Identifications"] = sum(
+        len(list(find_ids(l))) for d, l in diary.iter_lines()
+    )
 
     for key, val in output.items():
-        print('{:.<20}{:.>5}'.format(key, val))
+        print("{:.<20}{:.>5}".format(key, val))
 
     return output
```

### Comparing `hyperdiary-0.6.1/hyperdiary/tiddlywiki.py` & `hyperdiary-0.7.0/hyperdiary/tiddlywiki.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,190 +7,216 @@
 from typing import Union, Iterable, Iterator, Tuple, Any
 from . import diary
 from .localization import Localization
 
 
 class _TiddlerCalendar(TextCalendar):
 
-    def __init__(self,
-                 tiddler_titles: Iterable[Tuple[int, str]],
-                 loc: Localization,
-                 firstweekday: int = 0) -> None:
+    def __init__(
+        self,
+        tiddler_titles: Iterable[Tuple[int, str]],
+        loc: Localization,
+        firstweekday: int = 0,
+    ) -> None:
         super().__init__(firstweekday=firstweekday)
         self.links = {day: ttl for day, ttl in tiddler_titles}
         self.loc = loc
 
     def formatday(self, day: int, weekday: int, width: int) -> str:
-        daystr = str(day) if day > 0 else ''
+        daystr = str(day) if day > 0 else ""
         if day in self.links:
-            daystr = '[[{}|{}]]'.format(daystr, self.links[day])
+            daystr = "[[{}|{}]]".format(daystr, self.links[day])
         return daystr
 
     def formatweekheader(self, width: int) -> str:
-        header = ' | '.join(self.loc.get_day_short(
-                            i - self.getfirstweekday() % 7)
-                            for i in self.iterweekdays())
-        return '|{}|h'.format(header)
-
-    def formatweek(self,
-                   theweek: Any,
-                   width: int) -> str:
-        w = ' | '.join(self.formatday(d, wd, width) for (d, wd) in theweek)
-        return '|{}|'.format(w)
-
-    def formatmonthname(self, theyear: int, themonth: int, width: int,
-                        withyear: bool = True) -> str:
-        return ''
+        header = " | ".join(
+            self.loc.get_day_short(i - self.getfirstweekday() % 7)
+            for i in self.iterweekdays()
+        )
+        return "|{}|h".format(header)
+
+    def formatweek(self, theweek: Any, width: int) -> str:
+        w = " | ".join(self.formatday(d, wd, width) for (d, wd) in theweek)
+        return "|{}|".format(w)
+
+    def formatmonthname(
+        self, theyear: int, themonth: int, width: int, withyear: bool = True
+    ) -> str:
+        return ""
 
 
 def make_tiddler_filename(o: Union[str, date]) -> str:
-    '''
+    """
     >>> make_tiddler_filename(" Frühstück Ähre Grüße Föhn")
     'fruehstueck-aehre-gruesse-foehn.tid'
     >>> make_tiddler_filename("a.v-_'üöß' tiddler")
     'av-_ueoess-tiddler.tid'
     >>> make_tiddler_filename(date(2019, 2, 3))
     '2019-02-03.tid'
-    '''
+    """
     if isinstance(o, str):
-        s = o.lower() \
-             .replace('ß', 'ss') \
-             .replace('ä', 'ae') \
-             .replace('ö', 'oe') \
-             .replace('ü', 'ue')
-        s = unicodedata.normalize('NFKD', s)
-        s = s.encode('ascii', 'ignore').decode('ascii')
-        s = re.sub(r'[^\w\s-]', '', s).strip()
-        s = re.sub(r'[-\s]+', '-', s)
+        s = (
+            o.lower()
+            .replace("ß", "ss")
+            .replace("ä", "ae")
+            .replace("ö", "oe")
+            .replace("ü", "ue")
+        )
+        s = unicodedata.normalize("NFKD", s)
+        s = s.encode("ascii", "ignore").decode("ascii")
+        s = re.sub(r"[^\w\s-]", "", s).strip()
+        s = re.sub(r"[-\s]+", "-", s)
     elif isinstance(o, date):
-        s = '{:04d}-{:02d}-{:02d}'.format(o.year, o.month, o.day)
+        s = "{:04d}-{:02d}-{:02d}".format(o.year, o.month, o.day)
     else:
-        raise NotImplementedError('Cannot convert object of type '
-                                  '{} to filename'.format(type(o)))
-    return '{}.tid'.format(s)
+        raise NotImplementedError(
+            "Cannot convert object of type " "{} to filename".format(type(o))
+        )
+    return "{}.tid".format(s)
 
 
 class Tiddler:
     def __init__(self, fname: diary.Pathlike, **fields: str) -> None:
         self.fname = fname
         self.fields = dict(**fields)
 
     @property
     def title(self) -> str:
-        return self.fields['title']
+        return self.fields["title"]
 
     @property
     def text(self) -> str:
-        return self.fields['text']
+        return self.fields["text"]
 
     def __str__(self) -> str:
         return '<Tiddler(title="{0}")>'.format(self.title)
 
     def __repr__(self) -> str:
-        return 'Tiddler({0})'.format(', '.join(
-            '{}="{}"'.format(k, v) for k, v in self.fields.items()))
+        return "Tiddler({0})".format(
+            ", ".join('{}="{}"'.format(k, v) for k, v in self.fields.items())
+        )
 
     def _fields_without_text(self) -> Iterator[Tuple[str, str]]:
         for key, val in self.fields.items():
-            if key.lower() != 'text':
+            if key.lower() != "text":
                 yield key, val
 
     def to_tid(self) -> str:
-        return '\n'.join(['{} = {}'.format(k, v) for k, v in
-                          self._fields_without_text()]) \
-            + '\ntype: text/vnd.tiddlywik\n\n' \
+        return (
+            "\n".join(["{} = {}".format(k, v) for k, v in self._fields_without_text()])
+            + "\ntype: text/vnd.tiddlywik\n\n"
             + self.text
+        )
 
     def to_div(self) -> str:
-        args = ' '.join(['{}="{}"'.format(k, v) for k, v in
-                         self._fields_without_text()])
-        return '<div {}>\n<pre>\n{}\n</pre>\n</div>'.format(args, self.text)
+        args = " ".join(
+            ['{}="{}"'.format(k, v) for k, v in self._fields_without_text()]
+        )
+        return "<div {}>\n<pre>\n{}\n</pre>\n</div>".format(args, self.text)
 
     @staticmethod
-    def from_entry(dt: date, entry: Iterable[str],
-                   localization: Localization) -> 'Tiddler':
+    def from_entry(
+        dt: date, entry: Iterable[str], localization: Localization
+    ) -> "Tiddler":
         tags = []
         day_text = io.StringIO()
         for line in entry:
-            day_text.write('* ')
+            day_text.write("* ")
             for token in diary.tokenize(line):
                 if token.type == diary.TokenType.Id:
-                    day_text.write('[[{}|{}]]'.format(token.text, token.ref))
+                    day_text.write("[[{}|{}]]".format(token.text, token.ref))
                 elif token.type == diary.TokenType.Text:
                     day_text.write(token.text)
                 elif token.type == diary.TokenType.Tag:
                     tags.append(token.text)
                 else:
-                    raise NotImplementedError('Unknown TokenType')
-            day_text.write('\n')
+                    raise NotImplementedError("Unknown TokenType")
+            day_text.write("\n")
         day_text.seek(0)
-        compact_date = '{:04d}{:02d}{:02d}1200000000'.format(dt.year, dt.month,
-                                                             dt.day)
+        compact_date = "{:04d}{:02d}{:02d}1200000000".format(dt.year, dt.month, dt.day)
 
-        fields = dict(title=localization.format_date(dt),
-                      text=day_text.read(),
-                      tags=' '.join(sorted(set(tags))),
-                      created=compact_date,
-                      modified=compact_date)
+        fields = dict(
+            title=localization.format_date(dt),
+            text=day_text.read(),
+            tags=" ".join(sorted(set(tags))),
+            created=compact_date,
+            modified=compact_date,
+        )
 
         return Tiddler(make_tiddler_filename(dt), **fields)
 
 
 def diary_to_tiddlers(diary_instance: diary.Diary) -> Iterator[Tiddler]:
     loc = diary_instance.localization
     year_titles = []
     for year, year_group in diary_instance.iter_entries_by_year_and_month():
         month_titles = []
         for month, month_entries in year_group:
             tiddler_titles = []
             for entry in month_entries:
-                tiddler = Tiddler.from_entry(entry.dt, entry.lines,
-                                             diary_instance.localization)
+                tiddler = Tiddler.from_entry(
+                    entry.dt, entry.lines, diary_instance.localization
+                )
                 tiddler_titles.append((entry.dt.day, tiddler.title))
                 yield tiddler
             month_name = loc.get_month(month - 1)
-            title = '{} {}'.format(month_name, year)
+            title = "{} {}".format(month_name, year)
             cal = _TiddlerCalendar(tiddler_titles, loc)
             text = cal.formatmonth(year, month)
             yield Tiddler(fname=title, title=title, text=text)
             month_titles.append((month_name, title))
-        title = '{}'.format(year)
-        text = '\n'.join('[[{}|{}]]'.format(month_name, ttl)
-                         for month_name, ttl in month_titles)
+        title = "{}".format(year)
+        text = "\n".join(
+            "[[{}|{}]]".format(month_name, ttl) for month_name, ttl in month_titles
+        )
         yield Tiddler(fname=title, title=title, text=text)
         year_titles.append(title)
-    title = 'Home'
-    text = '\n'.join('[[{}]]'.format(ttl) for ttl in year_titles)
+    title = "Home"
+    text = "\n".join("[[{}]]".format(ttl) for ttl in year_titles)
     yield Tiddler(fname=title, title=title, text=text)
-    yield Tiddler(title='$:/DefaultTiddlers', fname='DefaultTiddlers',
-                  text='[[{}]]'.format(title))
+    yield Tiddler(
+        title="$:/DefaultTiddlers", fname="DefaultTiddlers", text="[[{}]]".format(title)
+    )
     # ToDo: add additional (system) tiddlers
 
 
-def diary_to_tiddlers_export(diary_instance: diary.Diary,
-                             tiddler_dir: diary.Pathlike) -> None:
+def diary_to_tiddlers_export(
+    diary_instance: diary.Diary, tiddler_dir: diary.Pathlike
+) -> None:
     os.makedirs(str(tiddler_dir), exist_ok=True)
     for tiddler in diary_to_tiddlers(diary_instance):
-        with open(os.path.join(str(tiddler_dir), str(tiddler.fname)), 'w') \
-                as f:
+        with open(os.path.join(str(tiddler_dir), str(tiddler.fname)), "w") as f:
             f.write(tiddler.to_tid())
 
 
 _STORE_AREA_SENTINEL = 'id="storeArea"'
 
 
-def diary_to_tiddlywiki_export(diary_instance: diary.Diary,
-                               file: diary.Pathlike,
-                               tiddlywiki_base_file: diary.Pathlike) -> None:
-    content = '\n'.join(tiddler.to_div() for tiddler in
-                        diary_to_tiddlers(diary_instance))
+def diary_to_tiddlywiki_export(
+    diary_instance: diary.Diary,
+    file: diary.Pathlike,
+    tiddlywiki_base_file: diary.Pathlike,
+) -> None:
+    content = "\n".join(
+        tiddler.to_div() for tiddler in diary_to_tiddlers(diary_instance)
+    )
     sentinel_found = False
-    with open(str(file), 'w') as f, \
-            open(str(tiddlywiki_base_file), 'r') as wiki:
+    with open(str(file), "w") as f, open(str(tiddlywiki_base_file), "r") as wiki:
         for line in wiki:
-            f.write(line)
-            if _STORE_AREA_SENTINEL in line:
+            if not sentinel_found and _STORE_AREA_SENTINEL in line:
+                [before_sentinel, after_sentinel] = line.split(_STORE_AREA_SENTINEL, 1)
+                [before_close, after_close] = after_sentinel.split(">", 1)
+                f.write(before_sentinel)
+                f.write(_STORE_AREA_SENTINEL)
+                f.write(before_close)
+                f.write(">")
                 f.write(content)
+                f.write(after_close)
                 sentinel_found = True
+            else:
+                f.write(line)
     if not sentinel_found:
-        raise Exception('Could not find \'{}\' in file {}'
-                        .format(_STORE_AREA_SENTINEL, tiddlywiki_base_file))
+        raise Exception(
+            "Could not find '{}' in file {}".format(
+                _STORE_AREA_SENTINEL, tiddlywiki_base_file
+            )
+        )
```

### Comparing `hyperdiary-0.6.1/setup.py` & `hyperdiary-0.7.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
-with open('README.rst') as readme_file:
+with open("README.rst") as readme_file:
     readme = readme_file.read()
 
-with open('HISTORY.rst') as history_file:
+with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ['PyYAML>=5.1', 'colorama>=0.4.1']
+requirements = ["PyYAML>=6.0", "colorama>=0.4.6"]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
-    author='luphord',
-    author_email='luphord@protonmail.com',
+    author="luphord",
+    author_email="luphord@protonmail.com",
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
-    description='A command line tool for my image processing needs.',
+    description="A command line tool for my image processing needs.",
     entry_points={
-        'console_scripts': [
-            'hyperdiary=hyperdiary.__main__:main',
+        "console_scripts": [
+            "hyperdiary=hyperdiary.__main__:main",
         ],
     },
-    data_files=[('hyperdiary/assets/css',
-                 ['hyperdiary/assets/css/picnic.min.css'])],
+    data_files=[("hyperdiary/assets/css", ["hyperdiary/assets/css/picnic.min.css"])],
     install_requires=requirements,
-    license='MIT license',
-    long_description=readme + '\n\n' + history,
+    license="MIT license",
+    long_description=readme + "\n\n" + history,
     include_package_data=True,
-    keywords='hyperdiary',
-    name='hyperdiary',
+    keywords="hyperdiary",
+    name="hyperdiary",
     packages=find_packages(),
     setup_requires=setup_requirements,
-    test_suite='tests',
+    test_suite="tests",
     tests_require=test_requirements,
-    url='https://github.com/luphord/hyperdiary',
-    version='0.6.1',
+    url="https://github.com/luphord/hyperdiary",
+    version="0.7.0",
     zip_safe=False,
 )
```

### Comparing `hyperdiary-0.6.1/tests/test_hyperdiary.py` & `hyperdiary-0.7.0/tests/test_hyperdiary.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,51 +3,53 @@
 
 import unittest
 from datetime import date
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 from hyperdiary import parser, Diary
-from hyperdiary.diary import find_ids, find_tags, tokenize, \
-    BadEntryException
+from hyperdiary.diary import find_ids, find_tags, tokenize, BadEntryException
 from hyperdiary.check import check
 from hyperdiary.stats import stats
 from hyperdiary.html import diary_to_html, diary_to_html_folder
-from hyperdiary.tiddlywiki import diary_to_tiddlers, \
-    diary_to_tiddlers_export, diary_to_tiddlywiki_export
+from hyperdiary.tiddlywiki import (
+    diary_to_tiddlers,
+    diary_to_tiddlers_export,
+    diary_to_tiddlywiki_export,
+)
 from hyperdiary.hugo import diary_to_hugo
 
 
-EXPECTED_TIDDLER_NAMES = {'2019-06-09.tid', '2019-05-01.tid', '2019-06-10.tid'}
+EXPECTED_TIDDLER_NAMES = {"2019-06-09.tid", "2019-05-01.tid", "2019-06-10.tid"}
 
 
 def in_test_folder(relative_path):
     return Path(__file__).parent / relative_path
 
 
 class TestHyperdiary(unittest.TestCase):
 
     def setUp(self):
-        self.diary = Diary.discover(in_test_folder('src'))
+        self.diary = Diary.discover(in_test_folder("src"))
         self.diary.load_entries()
 
     def test_command_line_interface(self):
-        self.assertEqual('check', parser.parse_args(['check']).subcommand)
+        self.assertEqual("check", parser.parse_args(["check"]).subcommand)
 
     def test_loading_of_entries(self):
         self.assertGreaterEqual(len(self.diary.entries), 3)
 
     def test_diary_without_expected(self):
         Diary({})
 
     def test_localization_loaded(self):
         loc = self.diary.localization
-        self.assertEqual('Aug', loc.get_month(7))
-        self.assertEqual('Mi', loc.get_day_short(2))
-        self.assertEqual('3.11.2019', loc.format_date(date(2019, 11, 3)))
+        self.assertEqual("Aug", loc.get_month(7))
+        self.assertEqual("Mi", loc.get_day_short(2))
+        self.assertEqual("3.11.2019", loc.format_date(date(2019, 11, 3)))
 
     def test_check(self):
         check(self.diary)
 
     def test_stats(self):
         self.assertGreater(len(stats(self.diary)), 3)
 
@@ -63,37 +65,38 @@
             for month, month_entries in year_group:
                 for entry in month_entries:
                     cnt += 1
         self.assertGreaterEqual(cnt, 3)
         self.assertEqual(cnt, len(self.diary.entries))
 
     def test_missing_hyperdiary_json(self):
-        self.assertRaises(FileNotFoundError, Diary.discover,
-                          subpath=in_test_folder('.'))
+        self.assertRaises(
+            FileNotFoundError, Diary.discover, subpath=in_test_folder(".")
+        )
 
     def test_bad_entries(self):
-        path = in_test_folder('src/2019/05_bad_entries.yaml')
+        path = in_test_folder("src/2019/05_bad_entries.yaml")
         diary = Diary(dict(sources=[str(path)]))
         self.assertRaises(BadEntryException, diary.load_entries)
 
     def test_tokenization(self):
-        line = '+tag A $test-line by $Jane_Doe|Jane; expect no content +hallo'
+        line = "+tag A $test-line by $Jane_Doe|Jane; expect no content +hallo"
         self.assertEqual(2, len(find_tags(line)))
         self.assertEqual(2, len(find_ids(line)))
         self.assertEqual(7, len(list(tokenize(line))))
-        line = '$just_an_id)'
+        line = "$just_an_id)"
         self.assertEqual(1, len(find_ids(line)))
         self.assertEqual(2, len(list(tokenize(line))))
 
     def test_html_export(self):
         with TemporaryDirectory() as folder:
-            outfname = Path(folder) / 'out.html'
+            outfname = Path(folder) / "out.html"
             diary_to_html(self.diary, str(outfname))
             self.assertTrue(outfname.exists())
-            with open(str(outfname), 'r') as f:
+            with open(str(outfname), "r") as f:
                 self.assertGreater(len(f.read()), 0)
 
     def test_htmlfolder_export(self):
         with TemporaryDirectory() as folder:
             diary_to_html_folder(self.diary, folder)
             folder = Path(folder)
             self.assertGreater(len(list(folder.iterdir())), 0)
@@ -104,28 +107,31 @@
             folder = Path(folder)
             files = set(f.name for f in folder.iterdir())
             self.assertGreater(len(files), 0)
             for fname in EXPECTED_TIDDLER_NAMES:
                 self.assertIn(fname, files)
 
     def test_tiddywiki_export(self):
-        tiddlywiki = 'tiddlywiki_mock.html'
+        tiddlywiki = "tiddlywiki_mock.html"
         with TemporaryDirectory() as folder:
             folder = Path(folder)
             tiddlywiki_path = folder / tiddlywiki
-            outfname = folder / 'out.html'
-            with open(str(tiddlywiki_path), 'w') as f:
-                f.write('---\n---\n')  # no "storeArea"
-            self.assertRaises(Exception, diary_to_tiddlywiki_export,
-                              diary_instance=self.diary, file=str(outfname),
-                              tiddlywiki_base_file=str(tiddlywiki_path))
-            with open(str(tiddlywiki_path), 'w') as f:
-                f.write('---\nid="storeArea"\n---\n')
-            diary_to_tiddlywiki_export(self.diary, str(outfname),
-                                       str(tiddlywiki_path))
+            outfname = folder / "out.html"
+            with open(str(tiddlywiki_path), "w") as f:
+                f.write("---\n---\n")  # no "storeArea"
+            self.assertRaises(
+                Exception,
+                diary_to_tiddlywiki_export,
+                diary_instance=self.diary,
+                file=str(outfname),
+                tiddlywiki_base_file=str(tiddlywiki_path),
+            )
+            with open(str(tiddlywiki_path), "w") as f:
+                f.write('---\n<div id="storeArea">\n---\n')
+            diary_to_tiddlywiki_export(self.diary, str(outfname), str(tiddlywiki_path))
             self.assertGreater(len(list(folder.iterdir())), 1)
 
     def test_tiddler_serialization(self):
         for tiddler in diary_to_tiddlers(self.diary):
             self.assertGreater(len(tiddler.to_tid()), 0)
             self.assertGreater(len(tiddler.to_div()), 0)
```

