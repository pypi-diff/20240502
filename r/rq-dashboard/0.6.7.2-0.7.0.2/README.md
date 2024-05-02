# Comparing `tmp/rq-dashboard-0.6.7.2.tar.gz` & `tmp/rq_dashboard-0.7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rq-dashboard-0.6.7.2.tar", last modified: Wed Feb 14 14:03:31 2024, max compression
+gzip compressed data, was "rq_dashboard-0.7.0.2.tar", last modified: Thu May  2 10:23:27 2024, max compression
```

## Comparing `rq-dashboard-0.6.7.2.tar` & `rq_dashboard-0.7.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 14:03:31.695944 rq-dashboard-0.6.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-02-14 14:03:31.695944 rq-dashboard-0.6.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 14:03:31.687944 rq-dashboard-0.6.7.2/rq_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7847 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/legacy_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 14:03:31.691944 rq-dashboard-0.6.7.2/rq_dashboard/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 14:03:31.691944 rq-dashboard-0.6.7.2/rq_dashboard/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)   192348 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/static/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   155713 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/static/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 14:03:31.691944 rq-dashboard-0.6.7.2/rq_dashboard/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   222911 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/static/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)    78587 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    88145 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/static/js/jquery-3.4.1.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    49651 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/static/js/sugar-1.2.1.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/static/js/underscore-umd-min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 14:03:31.687944 rq-dashboard-0.6.7.2/rq_dashboard/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 14:03:31.695944 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/inline_js.html
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/job.html
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/jobs.html
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/queues.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 14:03:31.695944 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/scripts/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/scripts/job.js
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/scripts/jobs.js
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/scripts/queues.js
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/scripts/workers.js
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/workers.html
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19274 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/rq_dashboard/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 14:03:31.695944 rq-dashboard-0.6.7.2/rq_dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-02-14 14:03:31.000000 rq-dashboard-0.6.7.2/rq_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-02-14 14:03:31.000000 rq-dashboard-0.6.7.2/rq_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 14:03:31.000000 rq-dashboard-0.6.7.2/rq_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-14 14:03:31.000000 rq-dashboard-0.6.7.2/rq_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 14:03:31.000000 rq-dashboard-0.6.7.2/rq_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-14 14:03:31.000000 rq-dashboard-0.6.7.2/rq_dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-14 14:03:31.000000 rq-dashboard-0.6.7.2/rq_dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-14 14:03:31.695944 rq-dashboard-0.6.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 14:03:31.695944 rq-dashboard-0.6.7.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 14:03:31.695944 rq-dashboard-0.6.7.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33579 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/tests/fixtures/rq_1_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-02-14 14:02:49.000000 rq-dashboard-0.6.7.2/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:23:27.165264 rq_dashboard-0.7.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-02 10:23:27.165264 rq_dashboard-0.7.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:23:27.161265 rq_dashboard-0.7.0.2/rq_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8115 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/legacy_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:23:27.161265 rq_dashboard-0.7.0.2/rq_dashboard/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:23:27.161265 rq_dashboard-0.7.0.2/rq_dashboard/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   192348 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/static/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   155713 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/static/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:23:27.165264 rq_dashboard-0.7.0.2/rq_dashboard/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   222911 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/static/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)    78587 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    88145 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/static/js/jquery-3.4.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    49651 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/static/js/sugar-1.2.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/static/js/underscore-umd-min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:23:27.157265 rq_dashboard-0.7.0.2/rq_dashboard/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:23:27.165264 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/inline_js.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/job.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/jobs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/queues.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:23:27.165264 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/scripts/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/scripts/job.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/scripts/jobs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/scripts/queues.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/scripts/workers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/workers.html
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20054 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/rq_dashboard/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:23:27.165264 rq_dashboard-0.7.0.2/rq_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-02 10:23:27.000000 rq_dashboard-0.7.0.2/rq_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-02 10:23:27.000000 rq_dashboard-0.7.0.2/rq_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:23:27.000000 rq_dashboard-0.7.0.2/rq_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 10:23:27.000000 rq_dashboard-0.7.0.2/rq_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:23:26.000000 rq_dashboard-0.7.0.2/rq_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 10:23:27.000000 rq_dashboard-0.7.0.2/rq_dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 10:23:27.000000 rq_dashboard-0.7.0.2/rq_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-02 10:23:27.169264 rq_dashboard-0.7.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:23:27.165264 rq_dashboard-0.7.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:23:27.165264 rq_dashboard-0.7.0.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33579 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/tests/fixtures/rq_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-02 10:22:54.000000 rq_dashboard-0.7.0.2/tests/test_basic.py
```

### Comparing `rq-dashboard-0.6.7.2/AUTHORS` & `rq_dashboard-0.7.0.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/LICENSE` & `rq_dashboard-0.7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/PKG-INFO` & `rq_dashboard-0.7.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rq-dashboard
-Version: 0.6.7.2
+Version: 0.7.0.2
 Summary: rq-dashboard is a general purpose, lightweight, web interface to monitor your RQ queues, jobs, and workers in realtime.
 Home-page: https://github.com/Parallels/rq-dashboard
 Author: Vincent Driessen
 Author-email: vincent@3rdcloud.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -115,17 +115,18 @@
   -c, --config TEXT               Configuration file (Python module on search
                                   path)
   -u, --redis-url TEXT            Redis URL. Can be specified multiple times.
                                   Default: redis://127.0.0.1:6379
   --poll-interval, --interval INTEGER
                                   Refresh interval in ms
   --extra-path TEXT               Append specified directories to sys.path
-  -j, --json                      Use JSONSerializer
+  --disable-delete                Disable delete jobs, clean up registries
   --debug / --normal              Enter DEBUG mode
   -v, --verbose                   Enable verbose logging
+  -j, --json                      Enable JSONSerializer
   --help                          Show this message and exit.
 ```
 
 Integrating the dashboard in your Flask app
 -------------------------------------------
 
 The dashboard can be integrated in to your own [Flask](http://flask.pocoo.org/) app by accessing the blueprint directly in the normal way, e.g.:
```

### Comparing `rq-dashboard-0.6.7.2/README.md` & `rq_dashboard-0.7.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,18 @@
   -c, --config TEXT               Configuration file (Python module on search
                                   path)
   -u, --redis-url TEXT            Redis URL. Can be specified multiple times.
                                   Default: redis://127.0.0.1:6379
   --poll-interval, --interval INTEGER
                                   Refresh interval in ms
   --extra-path TEXT               Append specified directories to sys.path
-  -j, --json                      Use JSONSerializer
+  --disable-delete                Disable delete jobs, clean up registries
   --debug / --normal              Enter DEBUG mode
   -v, --verbose                   Enable verbose logging
+  -j, --json                      Enable JSONSerializer
   --help                          Show this message and exit.
 ```
 
 Integrating the dashboard in your Flask app
 -------------------------------------------
 
 The dashboard can be integrated in to your own [Flask](http://flask.pocoo.org/) app by accessing the blueprint directly in the normal way, e.g.:
```

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/cli.py` & `rq_dashboard-0.7.0.2/rq_dashboard/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,17 @@
 )
 @click.option(
     "--delete-jobs",
     default=None,
     hidden=True,
     help="[DEPRECATED] Delete jobs instead of cancel",
 )
+@click.option(
+    "--disable-delete", is_flag=True, default=False, help="Disable delete jobs, clean up registries"
+)
 @click.option("--debug/--normal", default=False, help="Enter DEBUG mode")
 @click.option(
     "-v", "--verbose", is_flag=True, default=False, help="Enable verbose logging"
 )
 @click.option(
     "-j", "--json", is_flag=True, default=False, help="Enable JSONSerializer"
 )
@@ -174,14 +177,15 @@
     redis_sentinels,
     redis_master_name,
     poll_interval,
     extra_path,
     web_background,
     debug,
     delete_jobs,
+    disable_delete,
     verbose,
     json,
 ):
     """Run the RQ Dashboard Flask server.
 
     All configuration can be set on the command line or through environment
     variables of the form RQ_DASHBOARD_*. For example RQ_DASHBOARD_USERNAME.
@@ -194,18 +198,19 @@
     """
     if extra_path:
         sys.path += list(extra_path)
 
     click.echo("RQ Dashboard version {}".format(VERSION))
     app = make_flask_app(config, username, password, url_prefix)
     app.config["DEPRECATED_OPTIONS"] = []
-    if redis_url:
-        app.config["RQ_DASHBOARD_REDIS_URL"] = redis_url
-    else:
-        app.config["RQ_DASHBOARD_REDIS_URL"] = "redis://127.0.0.1:6379"
+    if app.config.get("RQ_DASHBOARD_REDIS_URL") is None:
+        if redis_url:
+            app.config["RQ_DASHBOARD_REDIS_URL"] = redis_url
+        else:
+            app.config["RQ_DASHBOARD_REDIS_URL"] = "redis://127.0.0.1:6379"
     if redis_host:
         app.config["DEPRECATED_OPTIONS"].append("--redis-host")
     if redis_port:
         app.config["DEPRECATED_OPTIONS"].append("--redis-port")
     if redis_password:
         app.config["DEPRECATED_OPTIONS"].append("--redis-password")
     if redis_database:
@@ -248,17 +253,19 @@
         url = urlunparse((scheme, netloc, path, "", "", ""))
         log.error(
             "Use --redis-url=%s configuration option "
             "instead of specifying host, port and other parameters separately",
             url,
         )
         app.config["RQ_DASHBOARD_REDIS_URL"] = url
-        
+
+    app.config["RQ_DASHBOARD_DISABLE_DELETE"] = disable_delete
+
     if json:
         service_config.serializer = JSONSerializer
 
     setup_rq_connection(app)
     app.run(host=bind, port=port, debug=debug)
 
 
 def main():
-    run(auto_envvar_prefix="RQ_DASHBOARD")
+    run(auto_envvar_prefix="RQ_DASHBOARD")
```

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/legacy_config.py` & `rq_dashboard-0.7.0.2/rq_dashboard/legacy_config.py`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/static/css/bootstrap.css` & `rq_dashboard-0.7.0.2/rq_dashboard/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/static/css/bootstrap.min.css` & `rq_dashboard-0.7.0.2/rq_dashboard/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/static/css/main.css` & `rq_dashboard-0.7.0.2/rq_dashboard/static/css/main.css`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/static/favicon.ico` & `rq_dashboard-0.7.0.2/rq_dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/static/js/bootstrap.bundle.js` & `rq_dashboard-0.7.0.2/rq_dashboard/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/static/js/bootstrap.bundle.min.js` & `rq_dashboard-0.7.0.2/rq_dashboard/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/static/js/jquery-3.4.1.min.js` & `rq_dashboard-0.7.0.2/rq_dashboard/static/js/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/static/js/sugar-1.2.1.min.js` & `rq_dashboard-0.7.0.2/rq_dashboard/static/js/sugar-1.2.1.min.js`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/static/js/underscore-umd-min.js` & `rq_dashboard-0.7.0.2/rq_dashboard/static/js/underscore-umd-min.js`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/base.html` & `rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/base.html`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/job.html` & `rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/job.html`

 * *Files 20% similar despite different names*

```diff
@@ -2,47 +2,43 @@
 
 {% block content %}
 <div class="section">
     <div class="row">
         <span class="col-10">
             <h2><strong>Job ID</strong>: {{ id }}</h2>
         </span>
-            
+
         <span class="col-2">
             <button id="requeue-job-btn" class="btn btn-outline-warning btn-sm" style="display: none">Requeue</button>
+            {% if enable_delete %}
             <button id="delete-job-btn" class="btn btn-outline-danger btn-sm">Delete</button>
+            {% endif %}
         </span>
     </div>
     <div id="job-data" class="row"></div>
-    
+
 
     <script name="job-info" type="text/template">
 
         <span class="col-6">
             <p class="ellipsify"><strong>Description</strong>:<br><%= d.description %></p>
             <p><strong>Origin queue</strong>:<br><%= d.origin %></p>
             <p><strong>Status</strong>:<br><%= d.status %></p>
-            <% if (d.result) { %>
             <p><strong>Result</strong>:<br><%= d.result %></p>
-            <% } %>
         </span>
 
         <span class="col-6">
             <p><strong>Created at</strong>:<br> <%= d.created_at %></p>
             <p><strong>Enqueued at</strong>:<br> <%= d.enqueued_at %></p>
-            <% if (d.exc_info) { %>
             <p><strong>Ended at</strong>:<br> <%= d.ended_at %></p>
-            <% } %>
         </span>
 
-        <% if (d.exc_info) { %>
         <div class = "row col-12">
             <pre class="exc_info col-12"><%= d.exc_info %></pre>
         </div>
-        <% } %>
     </script>
 </div>
 
 {% endblock %}
 
 {% block content_scripts %}
     {% include "rq_dashboard/scripts/job.js" %}
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 {% extends "rq_dashboard/base.html" %} {% block content %}
 ********** JJoobb IIDD:: {{{{ iidd }}}} **********
-Requeue Delete
+Requeue {% if enable_delete %} Delete {% endif %}
 {% endblock %} {% block content_scripts %} {% include "rq_dashboard/scripts/
 job.js" %} {% endblock %}
```

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/jobs.html` & `rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/jobs.html`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,19 @@
             <option {% if registry_name == 'finished' %} selected {% endif %}>finished</option>
             <option {% if registry_name == 'failed' %} selected {% endif %}>failed</option>
             <option {% if registry_name == 'canceled' %} selected {% endif %}>canceled</option>
         </select>
     </div>
 
     <p class="intro">
+        {% if enable_delete %}
         <a href="{{ url_for('rq_dashboard.empty_queue', queue_name=queue.name, registry_name=registry_name) }}" id="empty-btn"
             class="btn btn-outline-danger btn-sm" style="float: right" data-toggle="tooltip"
             title="Remove all jobs from this queue (<b>destructive</b>)" data-html=true>Empty queue</a>
+        {% endif %}
         {% if registry_name == 'queued' %}
         <a href="{{ url_for('rq_dashboard.compact_queue', queue_name=queue.name) }}" id="compact-btn"
             class="btn btn-outline-success btn-sm" style="float: right; margin-right: 8px;" data-toggle="tooltip"
             title="Remove all stale jobs from this queue (non-destructive)">Compact</a>
         {% endif %}
         {% if registry_name == 'failed' %}
         <a href="{{ url_for('rq_dashboard.requeue_all', queue_name=queue.name) }}" id="requeue-all-btn" class="btn btn-outline-warning btn-sm"
@@ -72,15 +74,17 @@
                 <% } %>
             </td>
             <td><span class="creation_date"><%= d.created_at %></span></td>
             <td class="actions narrow">
                 <% if (d.exc_info) { %>
                 <a href="#" data-role="requeue-job-btn" class="btn btn-outline-warning btn-sm btn-block">Requeue</a>
                 <% } %>
+                {% if enable_delete %}
                 <a href="#" data-role="delete-job-btn" class="btn btn-outline-danger btn-sm">Delete</a>
+                {% endif %}
             </td>
         </tr>
     </script>
 
     <script name="no-jobs-row" type="text/template">
         <tr>
             <td colspan="3">No jobs.</td>
```

#### html2text {}

```diff
@@ -6,16 +6,17 @@
 % if registry_name == 'queued' %} selected {% endif %}>queued
 % if registry_name == 'scheduled' %} selected {% endif %}>scheduled
 % if registry_name == 'deferred' %} selected {% endif %}>deferred
 % if registry_name == 'started' %} selected {% endif %}>started
 % if registry_name == 'finished' %} selected {% endif %}>finished
 % if registry_name == 'failed' %} selected {% endif %}>failed
 % if registry_name == 'canceled' %} selected {% endif %}>canceled
-_E_m_p_t_y_ _q_u_e_u_e {% if registry_name == 'queued' %} _C_o_m_p_a_c_t {% endif %} {% if
-registry_name == 'failed' %} _R_e_q_u_e_u_e_ _A_l_l {% endif %} This list below contains
-all the queued jobs on queue {{{{ qquueeuuee..nnaammee }}}}, sorted by age (oldest on top).
+{% if enable_delete %} _E_m_p_t_y_ _q_u_e_u_e {% endif %} {% if registry_name == 'queued'
+%} _C_o_m_p_a_c_t {% endif %} {% if registry_name == 'failed' %} _R_e_q_u_e_u_e_ _A_l_l {% endif
+%} This list below contains all the queued jobs on queue {{{{ qquueeuuee..nnaammee }}}},
+sorted by age (oldest on top).
 NNaammee AAggee AAccttiioonnss
 Loading...
 On page:
 [Unknown INPUT type]
 {% endblock %} {% block content_scripts %} {% include "rq_dashboard/scripts/
 jobs.js" %} {% endblock %}
```

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/navbar.html` & `rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/navbar.html`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/queues.html` & `rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/queues.html`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/scripts/dashboard.js` & `rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/scripts/dashboard.js`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/scripts/job.js` & `rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/scripts/job.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -24,20 +24,25 @@
 
     var onJobLoaded = function(job, done) {
         var html = '';
 
         $job_data.empty();
 
         job.created_at = toRelative(Date.create(job.created_at)) + ' / ' + toShort(Date.create(job.created_at));
-        if (job.enqueued_at !== undefined) {
+        if (job.enqueued_at !== null) {
             job.enqueued_at = toRelative(Date.create(job.enqueued_at)) + ' / ' + toShort(Date.create(job.enqueued_at));
+        } else {
+            job.enqueued_at = '-'
         }
-        if (job.ended_at !== undefined) {
+        if (job.ended_at !== null) {
             job.ended_at = toRelative(Date.create(job.ended_at)) + ' / ' + toShort(Date.create(job.ended_at));
+        } else {
+            job.ended_at = '-'
         }
+
         if (job.status === "failed") {
             $("#requeue-job-btn").show()
         }
         html += template({
             d: job
         }, {
             variable: 'd'
```

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/scripts/jobs.js` & `rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/scripts/jobs.js`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/scripts/queues.js` & `rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/scripts/queues.js`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/scripts/workers.js` & `rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/scripts/workers.js`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/templates/rq_dashboard/workers.html` & `rq_dashboard-0.7.0.2/rq_dashboard/templates/rq_dashboard/workers.html`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard/web.py` & `rq_dashboard-0.7.0.2/rq_dashboard/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     VERSION as rq_version,
     Queue,
     Worker,
     pop_connection,
     push_connection,
     requeue_job,
 )
+from rq.exceptions import NoSuchJobError
 from rq.job import Job
 from rq.registry import (
     DeferredJobRegistry,
     FailedJobRegistry,
     FinishedJobRegistry,
     StartedJobRegistry,
     ScheduledJobRegistry,
@@ -109,14 +110,21 @@
         from flask import jsonify as flask_jsonify
 
         result_dict = f(*args, **kwargs)
         return flask_jsonify(**result_dict), {"Cache-Control": "no-store"}
 
     return _wrapped
 
+def check_delete_enable(f):
+    @wraps(f)
+    def wrapper(*args, **kwargs):
+        if current_app.config.get("RQ_DASHBOARD_DISABLE_DELETE"):
+            return dict(status="DISABLED")
+        return f(*args, **kwargs)
+    return wrapper
 
 def serialize_queues(instance_number, queues):
     return [
         dict(
             name=q.name,
             count=q.count,
             queued_url=url_for(
@@ -266,17 +274,17 @@
     jobs = [serialize_job(job) for job in current_queue_jobs if job]
 
     return (total_items, jobs)
 
 
 def escape_format_instance_list(url_list):
     if isinstance(url_list, (list, tuple)):
-        url_list = [re.sub(r"://:[^@]*@", "://:***@", x) for x in url_list]
+        url_list = [re.sub(r":\/\/[^@]*@", "://***:***@", x) for x in url_list]
     elif isinstance(url_list, string_types):
-        url_list = [re.sub(r"://:[^@]*@", "://:***@", url_list)]
+        url_list = [re.sub(r":\/\/[^@]*@", "://***:***@", url_list)]
     return url_list
 
 
 @blueprint.route("/", defaults={"instance_number": 0})
 @blueprint.route("/<int:instance_number>/")
 @blueprint.route("/<int:instance_number>/view")
 @blueprint.route("/<int:instance_number>/view/queues")
@@ -356,14 +364,15 @@
             rq_url_prefix=url_for(".queues_overview"),
             rq_dashboard_version=rq_dashboard_version,
             rq_version=rq_version,
             active_tab="jobs",
             deprecation_options_usage=current_app.config.get(
                 "DEPRECATED_OPTIONS", False
             ),
+            enable_delete=not current_app.config.get("RQ_DASHBOARD_DISABLE_DELETE"),
         )
     )
     r.headers.set("Cache-Control", "no-store")
     return r
 
 
 @blueprint.route("/<int:instance_number>/view/job/<job_id>")
@@ -377,25 +386,33 @@
             id=job.id,
             rq_url_prefix=url_for(".queues_overview"),
             rq_dashboard_version=rq_dashboard_version,
             rq_version=rq_version,
             deprecation_options_usage=current_app.config.get(
                 "DEPRECATED_OPTIONS", False
             ),
+            enable_delete=not current_app.config.get("RQ_DASHBOARD_DISABLE_DELETE"),
         )
     )
     r.headers.set("Cache-Control", "no-store")
     return r
 
 
 @blueprint.route("/job/<job_id>/delete", methods=["POST"])
+@check_delete_enable
 @jsonify
-def delete_job_view(job_id):
-    job = Job.fetch(job_id)
-    job.delete()
+def delete_job_view(job_id, registry=None):
+    try:
+        job = Job.fetch(job_id)
+        job.delete()
+    except NoSuchJobError:
+        if registry:
+            registry.remove(job_id)
+        return dict(status="ERROR")
+
     return dict(status="OK")
 
 
 @blueprint.route("/job/<job_id>/requeue", methods=["POST"])
 @jsonify
 def requeue_job_view(job_id):
     requeue_job(job_id, connection=current_app.redis_conn)
@@ -410,43 +427,45 @@
     count = len(job_ids)
     for job_id in job_ids:
         requeue_job(job_id, connection=current_app.redis_conn)
     return dict(status="OK", count=count)
 
 
 @blueprint.route("/queue/<queue_name>/<registry_name>/empty", methods=["POST"])
+@check_delete_enable
 @jsonify
 def empty_queue(queue_name, registry_name):
     if registry_name == "queued":
         q = Queue(queue_name, serializer=config.serializer)
         q.empty()
     elif registry_name == "failed":
-        ids = FailedJobRegistry(queue_name).get_job_ids()
-        for id in ids:
-            delete_job_view(id)
+        registry = FailedJobRegistry(queue_name)
+        for id in registry.get_job_ids():
+            delete_job_view(id, registry)
     elif registry_name == "deferred":
-        ids = DeferredJobRegistry(queue_name).get_job_ids()
-        for id in ids:
-            delete_job_view(id)
+        registry = DeferredJobRegistry(queue_name)
+        for id in registry.get_job_ids():
+            delete_job_view(id, registry)
     elif registry_name == "started":
-        ids = StartedJobRegistry(queue_name).get_job_ids()
-        for id in ids:
-            delete_job_view(id)
+        registry = StartedJobRegistry(queue_name)
+        for id in registry.get_job_ids():
+            delete_job_view(id, registry)
     elif registry_name == "finished":
-        ids = FinishedJobRegistry(queue_name).get_job_ids()
-        for id in ids:
-            delete_job_view(id)
+        registry = FinishedJobRegistry(queue_name)
+        for id in registry.get_job_ids():
+            delete_job_view(id, registry)
     elif registry_name == "canceled":
-        ids = CanceledJobRegistry(queue_name).get_job_ids()
-        for id in ids:
-            delete_job_view(id)
+        registry = CanceledJobRegistry(queue_name)
+        for id in registry.get_job_ids():
+            delete_job_view(id, registry)
     elif registry_name == "scheduled":
-        ids = ScheduledJobRegistry(queue_name).get_job_ids()
-        for id in ids:
-            delete_job_view(id)
+        registry = ScheduledJobRegistry(queue_name)
+        for id in registry.get_job_ids():
+            delete_job_view(id, registry)
+
     return dict(status="OK")
 
 
 @blueprint.route("/queue/<queue_name>/compact", methods=["POST"])
 @jsonify
 def compact_queue(queue_name):
     q = Queue(queue_name, serializer=config.serializer)
@@ -561,15 +580,15 @@
     return dict(
         id=job.id,
         created_at=serialize_date(job.created_at),
         enqueued_at=serialize_date(job.enqueued_at),
         ended_at=serialize_date(job.ended_at),
         origin=job.origin,
         status=job.get_status(),
-        result=job._result,
+        result=job.return_value(),
         exc_info=str(job.exc_info) if job.exc_info else None,
         description=job.description,
     )
 
 
 @blueprint.route("/<int:instance_number>/data/workers.json")
 @jsonify
```

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard.egg-info/PKG-INFO` & `rq_dashboard-0.7.0.2/rq_dashboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rq-dashboard
-Version: 0.6.7.2
+Version: 0.7.0.2
 Summary: rq-dashboard is a general purpose, lightweight, web interface to monitor your RQ queues, jobs, and workers in realtime.
 Home-page: https://github.com/Parallels/rq-dashboard
 Author: Vincent Driessen
 Author-email: vincent@3rdcloud.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -115,17 +115,18 @@
   -c, --config TEXT               Configuration file (Python module on search
                                   path)
   -u, --redis-url TEXT            Redis URL. Can be specified multiple times.
                                   Default: redis://127.0.0.1:6379
   --poll-interval, --interval INTEGER
                                   Refresh interval in ms
   --extra-path TEXT               Append specified directories to sys.path
-  -j, --json                      Use JSONSerializer
+  --disable-delete                Disable delete jobs, clean up registries
   --debug / --normal              Enter DEBUG mode
   -v, --verbose                   Enable verbose logging
+  -j, --json                      Enable JSONSerializer
   --help                          Show this message and exit.
 ```
 
 Integrating the dashboard in your Flask app
 -------------------------------------------
 
 The dashboard can be integrated in to your own [Flask](http://flask.pocoo.org/) app by accessing the blueprint directly in the normal way, e.g.:
```

### Comparing `rq-dashboard-0.6.7.2/rq_dashboard.egg-info/SOURCES.txt` & `rq_dashboard-0.7.0.2/rq_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/setup.py` & `rq_dashboard-0.7.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/tests/fixtures/rq_1_0.py` & `rq_dashboard-0.7.0.2/tests/fixtures/rq_1_0.py`

 * *Files identical despite different names*

### Comparing `rq-dashboard-0.6.7.2/tests/test_basic.py` & `rq_dashboard-0.7.0.2/tests/test_basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import unittest
 
 import redis
 from rq import Queue, Worker, pop_connection, push_connection
 
 from rq_dashboard.cli import make_flask_app
+from rq_dashboard.web import escape_format_instance_list
 
 
 HTTP_OK = 200
 
 class BasicTestCase(unittest.TestCase):
     redis_client = None
 
@@ -103,10 +104,24 @@
         if getattr(w, 'version', None):
             self.assertEqual(w.version, data['workers'][0]['version'])
         else:
             self.assertEqual('', data['workers'][0]['version'])
         w.register_death()
 
 
+    def test_instance_escaping(self):
+        expected_redis_instance = "redis://***:***@redis.example.com:6379"
+        self.assertEqual(
+            escape_format_instance_list(
+                [
+                    "redis://myuser:secretpassword@redis.example.com:6379",
+                    "redis://:secretpassword@redis.example.com:6379",
+                    "redis://:@redis.example.com:6379",
+                ]
+            ),
+            [expected_redis_instance, expected_redis_instance, expected_redis_instance],
+        )
+
+
 __all__ = [
     'BasicTestCase',
-]
+]
```

