# Comparing `tmp/sifflet-0.3.8.tar.gz` & `tmp/sifflet-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sifflet-0.3.8.tar", last modified: Tue Mar 26 14:23:57 2024, max compression
+gzip compressed data, was "sifflet-0.3.9.tar", last modified: Thu May  2 08:09:26 2024, max compression
```

## Comparing `sifflet-0.3.8.tar` & `sifflet-0.3.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 14:23:57.617148 sifflet-0.3.8/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 14:23:44.000000 sifflet-0.3.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-02-07 09:37:18.000000 sifflet-0.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4079 2024-03-26 14:23:57.617148 sifflet-0.3.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3652 2024-02-07 09:37:18.000000 sifflet-0.3.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      724 2024-02-07 09:37:18.000000 sifflet-0.3.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-26 14:19:40.000000 sifflet-0.3.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 14:23:57.617148 sifflet-0.3.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-02-07 09:37:18.000000 sifflet-0.3.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 14:23:57.613148 sifflet-0.3.8/sifflet.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4079 2024-03-26 14:23:57.000000 sifflet-0.3.8/sifflet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      819 2024-03-26 14:23:57.000000 sifflet-0.3.8/sifflet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 14:23:57.000000 sifflet-0.3.8/sifflet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-03-26 14:23:57.000000 sifflet-0.3.8/sifflet.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-03-26 14:23:57.000000 sifflet-0.3.8/sifflet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-26 14:23:57.000000 sifflet-0.3.8/sifflet.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 14:23:57.613148 sifflet-0.3.8/sifflet_cli/
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-03-26 14:19:40.000000 sifflet-0.3.8/sifflet_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-02-07 09:37:18.000000 sifflet-0.3.8/sifflet_cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 14:23:57.613148 sifflet-0.3.8/sifflet_cli/code/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 14:23:44.000000 sifflet-0.3.8/sifflet_cli/code/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2024-02-07 09:37:18.000000 sifflet-0.3.8/sifflet_cli/code/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 14:23:57.613148 sifflet-0.3.8/sifflet_cli/code/monitor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 14:23:44.000000 sifflet-0.3.8/sifflet_cli/code/monitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2024-02-07 09:37:18.000000 sifflet-0.3.8/sifflet_cli/code/monitor/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 14:23:57.613148 sifflet-0.3.8/sifflet_cli/code/workspace/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 14:23:44.000000 sifflet-0.3.8/sifflet_cli/code/workspace/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4305 2024-03-22 08:08:42.000000 sifflet-0.3.8/sifflet_cli/code/workspace/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 14:23:57.613148 sifflet-0.3.8/sifflet_cli/configure/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 14:23:44.000000 sifflet-0.3.8/sifflet_cli/configure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1938 2024-02-07 09:37:18.000000 sifflet-0.3.8/sifflet_cli/configure/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 14:23:57.617148 sifflet-0.3.8/sifflet_cli/ingest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 14:23:44.000000 sifflet-0.3.8/sifflet_cli/ingest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1086 2024-02-07 09:37:18.000000 sifflet-0.3.8/sifflet_cli/ingest/commands.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-02-07 09:37:18.000000 sifflet-0.3.8/sifflet_cli/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 14:23:57.617148 sifflet-0.3.8/sifflet_cli/rules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 14:23:44.000000 sifflet-0.3.8/sifflet_cli/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3362 2024-02-07 09:37:18.000000 sifflet-0.3.8/sifflet_cli/rules/commands.py
--rw-rw-rw-   0 root         (0) root         (0)     6082 2024-02-07 09:37:18.000000 sifflet-0.3.8/sifflet_cli/rules/displayrules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 14:23:57.617148 sifflet-0.3.8/sifflet_cli/status/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 14:23:44.000000 sifflet-0.3.8/sifflet_cli/status/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      750 2024-02-07 09:37:18.000000 sifflet-0.3.8/sifflet_cli/status/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:09:26.467012 sifflet-0.3.9/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 08:09:13.000000 sifflet-0.3.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-02-07 09:48:44.000000 sifflet-0.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4079 2024-05-02 08:09:26.467012 sifflet-0.3.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2024-02-07 09:48:44.000000 sifflet-0.3.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      724 2024-02-07 09:48:44.000000 sifflet-0.3.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-02 08:03:19.000000 sifflet-0.3.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 08:09:26.467012 sifflet-0.3.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-02-07 09:48:44.000000 sifflet-0.3.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:09:26.467012 sifflet-0.3.9/sifflet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4079 2024-05-02 08:09:26.000000 sifflet-0.3.9/sifflet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      819 2024-05-02 08:09:26.000000 sifflet-0.3.9/sifflet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 08:09:26.000000 sifflet-0.3.9/sifflet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-02 08:09:26.000000 sifflet-0.3.9/sifflet.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-05-02 08:09:26.000000 sifflet-0.3.9/sifflet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-02 08:09:26.000000 sifflet-0.3.9/sifflet.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:09:26.467012 sifflet-0.3.9/sifflet_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-02 08:03:19.000000 sifflet-0.3.9/sifflet_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-02-07 09:48:44.000000 sifflet-0.3.9/sifflet_cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:09:26.467012 sifflet-0.3.9/sifflet_cli/code/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 08:09:13.000000 sifflet-0.3.9/sifflet_cli/code/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2024-02-07 09:48:44.000000 sifflet-0.3.9/sifflet_cli/code/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:09:26.467012 sifflet-0.3.9/sifflet_cli/code/monitor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 08:09:13.000000 sifflet-0.3.9/sifflet_cli/code/monitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2024-02-07 09:48:44.000000 sifflet-0.3.9/sifflet_cli/code/monitor/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:09:26.467012 sifflet-0.3.9/sifflet_cli/code/workspace/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 08:09:13.000000 sifflet-0.3.9/sifflet_cli/code/workspace/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4305 2024-03-22 08:10:56.000000 sifflet-0.3.9/sifflet_cli/code/workspace/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:09:26.467012 sifflet-0.3.9/sifflet_cli/configure/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 08:09:13.000000 sifflet-0.3.9/sifflet_cli/configure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2024-02-07 09:48:44.000000 sifflet-0.3.9/sifflet_cli/configure/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:09:26.467012 sifflet-0.3.9/sifflet_cli/ingest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 08:09:13.000000 sifflet-0.3.9/sifflet_cli/ingest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-02-07 09:48:44.000000 sifflet-0.3.9/sifflet_cli/ingest/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-02-07 09:48:44.000000 sifflet-0.3.9/sifflet_cli/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:09:26.467012 sifflet-0.3.9/sifflet_cli/rules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 08:09:13.000000 sifflet-0.3.9/sifflet_cli/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3362 2024-02-07 09:48:44.000000 sifflet-0.3.9/sifflet_cli/rules/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     6082 2024-02-07 09:48:44.000000 sifflet-0.3.9/sifflet_cli/rules/displayrules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:09:26.467012 sifflet-0.3.9/sifflet_cli/status/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 08:09:13.000000 sifflet-0.3.9/sifflet_cli/status/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      750 2024-02-07 09:48:44.000000 sifflet-0.3.9/sifflet_cli/status/commands.py
```

### Comparing `sifflet-0.3.8/PKG-INFO` & `sifflet-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sifflet
-Version: 0.3.8
+Version: 0.3.9
 Summary: Sifflet CLI
 Home-page: https://www.siffletdata.com/
 Author: Sifflet
 Author-email: support@siffletdata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sifflet-0.3.8/README.md` & `sifflet-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `sifflet-0.3.8/pyproject.toml` & `sifflet-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sifflet-0.3.8/setup.py` & `sifflet-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `sifflet-0.3.8/sifflet.egg-info/PKG-INFO` & `sifflet-0.3.9/sifflet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sifflet
-Version: 0.3.8
+Version: 0.3.9
 Summary: Sifflet CLI
 Home-page: https://www.siffletdata.com/
 Author: Sifflet
 Author-email: support@siffletdata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sifflet-0.3.8/sifflet.egg-info/SOURCES.txt` & `sifflet-0.3.9/sifflet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sifflet-0.3.8/sifflet_cli/cli.py` & `sifflet-0.3.9/sifflet_cli/cli.py`

 * *Files identical despite different names*

### Comparing `sifflet-0.3.8/sifflet_cli/code/monitor/commands.py` & `sifflet-0.3.9/sifflet_cli/code/monitor/commands.py`

 * *Files identical despite different names*

### Comparing `sifflet-0.3.8/sifflet_cli/code/workspace/commands.py` & `sifflet-0.3.9/sifflet_cli/code/workspace/commands.py`

 * *Files identical despite different names*

### Comparing `sifflet-0.3.8/sifflet_cli/configure/commands.py` & `sifflet-0.3.9/sifflet_cli/configure/commands.py`

 * *Files identical despite different names*

### Comparing `sifflet-0.3.8/sifflet_cli/ingest/commands.py` & `sifflet-0.3.9/sifflet_cli/ingest/commands.py`

 * *Files identical despite different names*

### Comparing `sifflet-0.3.8/sifflet_cli/rules/commands.py` & `sifflet-0.3.9/sifflet_cli/rules/commands.py`

 * *Files identical despite different names*

### Comparing `sifflet-0.3.8/sifflet_cli/rules/displayrules.py` & `sifflet-0.3.9/sifflet_cli/rules/displayrules.py`

 * *Files identical despite different names*

### Comparing `sifflet-0.3.8/sifflet_cli/status/commands.py` & `sifflet-0.3.9/sifflet_cli/status/commands.py`

 * *Files identical despite different names*

