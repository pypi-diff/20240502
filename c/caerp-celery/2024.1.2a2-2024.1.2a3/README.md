# Comparing `tmp/caerp_celery-2024.1.2a2.tar.gz` & `tmp/caerp_celery-2024.1.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caerp_celery-2024.1.2a2.tar", last modified: Thu Apr 25 10:37:02 2024, max compression
+gzip compressed data, was "caerp_celery-2024.1.2a3.tar", last modified: Thu May  2 15:11:22 2024, max compression
```

## Comparing `caerp_celery-2024.1.2a2.tar` & `caerp_celery-2024.1.2a3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.019475 caerp_celery-2024.1.2a2/
--rw-r--r--   0 gas       (1000) gas       (1000)      334 2024-03-06 11:08:10.000000 caerp_celery-2024.1.2a2/CHANGELOG
--rw-r--r--   0 gas       (1000) gas       (1000)       11 2024-04-25 10:36:14.000000 caerp_celery-2024.1.2a2/CURRENT_VERSION
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 caerp_celery-2024.1.2a2/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      210 2024-03-06 10:24:06.000000 caerp_celery-2024.1.2a2/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-04-25 10:37:02.018475 caerp_celery-2024.1.2a2/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     2627 2024-03-05 16:04:43.000000 caerp_celery-2024.1.2a2/README.rst
--rw-r--r--   0 gas       (1000) gas       (1000)       46 2024-03-08 17:12:36.000000 caerp_celery-2024.1.2a2/requirements.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       38 2024-04-25 10:37:02.019475 caerp_celery-2024.1.2a2/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1372 2024-03-06 11:04:59.000000 caerp_celery-2024.1.2a2/setup.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.001475 caerp_celery-2024.1.2a2/src/
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.006475 caerp_celery-2024.1.2a2/src/caerp_celery/
--rw-r--r--   0 gas       (1000) gas       (1000)     4579 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1789 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/conf.py
--rw-r--r--   0 gas       (1000) gas       (1000)      585 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/exception.py
--rw-r--r--   0 gas       (1000) gas       (1000)      576 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/hacks.py
--rw-r--r--   0 gas       (1000) gas       (1000)      753 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/interfaces.py
--rw-r--r--   0 gas       (1000) gas       (1000)      852 2024-04-25 10:10:38.000000 caerp_celery-2024.1.2a2/src/caerp_celery/locks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5747 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     7465 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/models.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.010475 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/
--rw-r--r--   0 gas       (1000) gas       (1000)     2163 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3533 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/cegid.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3133 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/ebp.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3376 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/isacompta.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3264 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/quadra.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3391 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/sage.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5798 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/parsers/sage_generation_expert.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.011475 caerp_celery-2024.1.2a2/src/caerp_celery/schedulers/
--rw-r--r--   0 gas       (1000) gas       (1000)       29 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/schedulers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)      428 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/schedulers/tasks.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.018475 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/
--rw-r--r--   0 gas       (1000) gas       (1000)    10899 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)    39090 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/accounting_measure_compute.py
--rw-r--r--   0 gas       (1000) gas       (1000)    14135 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/accounting_parser.py
--rw-r--r--   0 gas       (1000) gas       (1000)    29193 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/csv_import.py
--rw-r--r--   0 gas       (1000) gas       (1000)    21494 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/export.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2015 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/json_import.py
--rw-r--r--   0 gas       (1000) gas       (1000)      392 2024-04-25 07:56:31.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/locks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     4428 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1423 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/notification.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3397 2024-03-15 11:24:28.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/tasks.py
--rw-r--r--   0 gas       (1000) gas       (1000)      509 2024-03-15 11:23:43.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/user_connections.py
--rw-r--r--   0 gas       (1000) gas       (1000)     6912 2024-04-25 09:04:32.000000 caerp_celery-2024.1.2a2/src/caerp_celery/tasks/utils.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2765 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a2/src/caerp_celery/transactional_task.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-04-25 10:37:02.008475 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     1411 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       84 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/entry_points.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-03-06 10:23:24.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/not-zip-safe
--rw-r--r--   0 gas       (1000) gas       (1000)       45 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       13 2024-04-25 10:37:01.000000 caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/top_level.txt
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.434054 caerp_celery-2024.1.2a3/
+-rw-r--r--   0 gas       (1000) gas       (1000)      334 2024-03-06 11:08:10.000000 caerp_celery-2024.1.2a3/CHANGELOG
+-rw-r--r--   0 gas       (1000) gas       (1000)       11 2024-05-02 15:09:51.000000 caerp_celery-2024.1.2a3/CURRENT_VERSION
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 caerp_celery-2024.1.2a3/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      210 2024-03-06 10:24:06.000000 caerp_celery-2024.1.2a3/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-05-02 15:11:22.433054 caerp_celery-2024.1.2a3/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     2627 2024-03-05 16:04:43.000000 caerp_celery-2024.1.2a3/README.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)       46 2024-03-08 17:12:36.000000 caerp_celery-2024.1.2a3/requirements.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       38 2024-05-02 15:11:22.434054 caerp_celery-2024.1.2a3/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1372 2024-03-06 11:04:59.000000 caerp_celery-2024.1.2a3/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.418054 caerp_celery-2024.1.2a3/src/
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.423054 caerp_celery-2024.1.2a3/src/caerp_celery/
+-rw-r--r--   0 gas       (1000) gas       (1000)     4579 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1789 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/conf.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      585 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/exception.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      576 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/hacks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      753 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/interfaces.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      885 2024-05-02 14:38:26.000000 caerp_celery-2024.1.2a3/src/caerp_celery/locks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5747 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     7465 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/models.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.427054 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/
+-rw-r--r--   0 gas       (1000) gas       (1000)     2163 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3533 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/cegid.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3133 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/ebp.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3376 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/isacompta.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3264 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/quadra.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3391 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/sage.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5798 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/sage_generation_expert.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.428054 caerp_celery-2024.1.2a3/src/caerp_celery/schedulers/
+-rw-r--r--   0 gas       (1000) gas       (1000)       29 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/schedulers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      428 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/schedulers/tasks.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.433054 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/
+-rw-r--r--   0 gas       (1000) gas       (1000)    10899 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    39090 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/accounting_measure_compute.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    14135 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/accounting_parser.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    29193 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/csv_import.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    21494 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/export.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2015 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/json_import.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      392 2024-04-25 07:56:31.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/locks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     4428 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1423 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/notification.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3397 2024-03-15 11:24:28.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/tasks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      509 2024-03-15 11:23:43.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/user_connections.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     6912 2024-04-25 09:04:32.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/utils.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2765 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/transactional_task.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.425054 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     1411 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       84 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/entry_points.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-03-06 10:23:24.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/not-zip-safe
+-rw-r--r--   0 gas       (1000) gas       (1000)       45 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       13 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/top_level.txt
```

### Comparing `caerp_celery-2024.1.2a2/LICENSE.txt` & `caerp_celery-2024.1.2a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/PKG-INFO` & `caerp_celery-2024.1.2a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caerp_celery
-Version: 2024.1.2a2
+Version: 2024.1.2a3
 Summary: caerp_celery
 Home-page: https://framagit.org/caerp/caerp_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `caerp_celery-2024.1.2a2/README.rst` & `caerp_celery-2024.1.2a3/README.rst`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/setup.py` & `caerp_celery-2024.1.2a3/setup.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/__init__.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/__init__.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/conf.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/conf.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/exception.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/exception.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/hacks.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/hacks.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/interfaces.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/interfaces.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/locks.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/locks.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 
 def is_locked(lockname, max_age: Optional[int] = None):
     """
     lockname: the name of the lock
     max_age: the maximum age of the lock file in seconds
     """
     p = _get_lock_path(lockname)
-    if max_age is not None and _get_file_age(p) > max_age:
+    result = p.exists()
+    if result and max_age is not None and _get_file_age(p) > max_age:
         p.unlink()
-        return False
-    return p.exists()
+        result = False
+    return result
 
 
 def acquire_lock(lockname):
     p = _get_lock_path(lockname)
     p.touch()
```

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/mail.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/mail.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/models.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/models.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/__init__.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/cegid.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/cegid.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/ebp.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/ebp.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/isacompta.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/isacompta.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/quadra.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/quadra.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/sage.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/sage.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/parsers/sage_generation_expert.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/sage_generation_expert.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/__init__.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/accounting_measure_compute.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/accounting_measure_compute.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/accounting_parser.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/accounting_parser.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/csv_import.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/csv_import.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/export.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/export.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/json_import.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/json_import.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/mail.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/mail.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/notification.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/notification.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/tasks.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/tasks/utils.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery/transactional_task.py` & `caerp_celery-2024.1.2a3/src/caerp_celery/transactional_task.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/PKG-INFO` & `caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caerp-celery
-Version: 2024.1.2a2
+Version: 2024.1.2a3
 Summary: caerp_celery
 Home-page: https://framagit.org/caerp/caerp_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `caerp_celery-2024.1.2a2/src/caerp_celery.egg-info/SOURCES.txt` & `caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

