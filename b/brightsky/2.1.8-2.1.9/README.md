# Comparing `tmp/brightsky-2.1.8.tar.gz` & `tmp/brightsky-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightsky-2.1.8.tar", last modified: Mon Feb 19 11:02:44 2024, max compression
+gzip compressed data, was "brightsky-2.1.9.tar", last modified: Thu May  2 10:08:14 2024, max compression
```

## Comparing `brightsky-2.1.8.tar` & `brightsky-2.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:02:44.776514 brightsky-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-19 11:02:41.000000 brightsky-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-02-19 11:02:44.776514 brightsky-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-02-19 11:02:41.000000 brightsky-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:02:44.772514 brightsky-2.1.8/brightsky/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/polling.py
--rw-r--r--   0 runner    (1001) docker     (127)    16876 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/web.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-02-19 11:02:41.000000 brightsky-2.1.8/brightsky/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:02:44.776514 brightsky-2.1.8/brightsky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-02-19 11:02:44.000000 brightsky-2.1.8/brightsky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-19 11:02:44.000000 brightsky-2.1.8/brightsky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 11:02:44.000000 brightsky-2.1.8/brightsky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-19 11:02:44.000000 brightsky-2.1.8/brightsky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-19 11:02:44.000000 brightsky-2.1.8/brightsky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-19 11:02:41.000000 brightsky-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 11:02:44.776514 brightsky-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-19 11:02:41.000000 brightsky-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:02:44.776514 brightsky-2.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-19 11:02:41.000000 brightsky-2.1.8/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-02-19 11:02:41.000000 brightsky-2.1.8/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-02-19 11:02:41.000000 brightsky-2.1.8/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-02-19 11:02:41.000000 brightsky-2.1.8/tests/test_polling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-02-19 11:02:41.000000 brightsky-2.1.8/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-02-19 11:02:41.000000 brightsky-2.1.8/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-02-19 11:02:41.000000 brightsky-2.1.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-02-19 11:02:41.000000 brightsky-2.1.8/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:08:14.203262 brightsky-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-02 10:08:10.000000 brightsky-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-02 10:08:14.203262 brightsky-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-02 10:08:10.000000 brightsky-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:08:14.199262 brightsky-2.1.9/brightsky/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13549 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16876 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-02 10:08:10.000000 brightsky-2.1.9/brightsky/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:08:14.203262 brightsky-2.1.9/brightsky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-02 10:08:14.000000 brightsky-2.1.9/brightsky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-02 10:08:14.000000 brightsky-2.1.9/brightsky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:08:14.000000 brightsky-2.1.9/brightsky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-02 10:08:14.000000 brightsky-2.1.9/brightsky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 10:08:14.000000 brightsky-2.1.9/brightsky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-02 10:08:11.000000 brightsky-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:08:14.203262 brightsky-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-02 10:08:11.000000 brightsky-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:08:14.203262 brightsky-2.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 10:08:11.000000 brightsky-2.1.9/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-02 10:08:11.000000 brightsky-2.1.9/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-02 10:08:11.000000 brightsky-2.1.9/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-02 10:08:11.000000 brightsky-2.1.9/tests/test_polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-02 10:08:11.000000 brightsky-2.1.9/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-02 10:08:11.000000 brightsky-2.1.9/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-02 10:08:11.000000 brightsky-2.1.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-05-02 10:08:11.000000 brightsky-2.1.9/tests/test_web.py
```

### Comparing `brightsky-2.1.8/LICENSE` & `brightsky-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/PKG-INFO` & `brightsky-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.1.8
+Version: 2.1.9
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@brightsky.dev
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.1.8/README.md` & `brightsky-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky/__main__.py` & `brightsky-2.1.9/brightsky/__main__.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky/cli.py` & `brightsky-2.1.9/brightsky/cli.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky/db.py` & `brightsky-2.1.9/brightsky/db.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky/export.py` & `brightsky-2.1.9/brightsky/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,14 +290,15 @@
         SELECT setval(
             'alerts_id_seq',
             GREATEST(%(max_id)s, (SELECT max(id) FROM alerts))
         );
     """
     ELEMENT_FIELDS = [
         'alert_id',
+        'status',
         'effective',
         'onset',
         'expires',
         'category',
         'response_type',
         'urgency',
         'severity',
```

### Comparing `brightsky-2.1.8/brightsky/parsers.py` & `brightsky-2.1.9/brightsky/parsers.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky/polling.py` & `brightsky-2.1.9/brightsky/polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky/query.py` & `brightsky-2.1.9/brightsky/query.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky/settings.py` & `brightsky-2.1.9/brightsky/settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky/tasks.py` & `brightsky-2.1.9/brightsky/tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky/utils.py` & `brightsky-2.1.9/brightsky/utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky/web.py` & `brightsky-2.1.9/brightsky/web.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky/worker.py` & `brightsky-2.1.9/brightsky/worker.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/brightsky.egg-info/PKG-INFO` & `brightsky-2.1.9/brightsky.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.1.8
+Version: 2.1.9
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@brightsky.dev
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.1.8/brightsky.egg-info/SOURCES.txt` & `brightsky-2.1.9/brightsky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/setup.py` & `brightsky-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/tests/test_export.py` & `brightsky-2.1.9/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/tests/test_parsers.py` & `brightsky-2.1.9/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/tests/test_polling.py` & `brightsky-2.1.9/tests/test_polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/tests/test_settings.py` & `brightsky-2.1.9/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/tests/test_tasks.py` & `brightsky-2.1.9/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/tests/test_utils.py` & `brightsky-2.1.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.1.8/tests/test_web.py` & `brightsky-2.1.9/tests/test_web.py`

 * *Files identical despite different names*

