# Comparing `tmp/dragonfly-radiance-0.3.8.tar.gz` & `tmp/dragonfly-radiance-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dragonfly-radiance-0.3.8.tar", last modified: Thu Feb 22 00:36:28 2024, max compression
+gzip compressed data, was "dist/dragonfly-radiance-0.3.9.tar", last modified: Fri Feb 23 05:29:46 2024, max compression
```

## Comparing `dragonfly-radiance-0.3.8.tar` & `dragonfly-radiance-0.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/_extend_dragonfly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)    25643 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/gridpar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/properties/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/properties/building.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/properties/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/properties/room2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/dragonfly_radiance/properties/story.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/dragonfly_radiance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/dragonfly_radiance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/dragonfly_radiance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/dragonfly_radiance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/dragonfly_radiance.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/dragonfly_radiance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/dragonfly_radiance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 00:36:28.000000 dragonfly-radiance-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-22 00:35:27.000000 dragonfly-radiance-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/_extend_dragonfly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25643 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/gridpar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/properties/building.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/properties/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/properties/room2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/dragonfly_radiance/properties/story.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/dragonfly_radiance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/dragonfly_radiance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/dragonfly_radiance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/dragonfly_radiance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/dragonfly_radiance.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/dragonfly_radiance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/dragonfly_radiance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-23 05:29:46.000000 dragonfly-radiance-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-23 05:28:47.000000 dragonfly-radiance-0.3.9/setup.py
```

### Comparing `dragonfly-radiance-0.3.8/LICENSE` & `dragonfly-radiance-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/PKG-INFO` & `dragonfly-radiance-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-radiance
-Version: 0.3.8
+Version: 0.3.9
 Summary: Dragonfly extension for radiance simulation.
 Home-page: https://github.com/ladybug-tools/dragonfly-radiance
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dragonfly-radiance-0.3.8/README.md` & `dragonfly-radiance-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/dev-requirements.txt` & `dragonfly-radiance-0.3.9/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/dragonfly_radiance/_extend_dragonfly.py` & `dragonfly-radiance-0.3.9/dragonfly_radiance/_extend_dragonfly.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/dragonfly_radiance/cli/translate.py` & `dragonfly-radiance-0.3.9/dragonfly_radiance/cli/translate.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/dragonfly_radiance/gridpar.py` & `dragonfly-radiance-0.3.9/dragonfly_radiance/gridpar.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/dragonfly_radiance/properties/building.py` & `dragonfly-radiance-0.3.9/dragonfly_radiance/properties/building.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/dragonfly_radiance/properties/context.py` & `dragonfly-radiance-0.3.9/dragonfly_radiance/properties/context.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/dragonfly_radiance/properties/model.py` & `dragonfly-radiance-0.3.9/dragonfly_radiance/properties/model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/dragonfly_radiance/properties/room2d.py` & `dragonfly-radiance-0.3.9/dragonfly_radiance/properties/room2d.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/dragonfly_radiance/properties/story.py` & `dragonfly-radiance-0.3.9/dragonfly_radiance/properties/story.py`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/dragonfly_radiance.egg-info/PKG-INFO` & `dragonfly-radiance-0.3.9/dragonfly_radiance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-radiance
-Version: 0.3.8
+Version: 0.3.9
 Summary: Dragonfly extension for radiance simulation.
 Home-page: https://github.com/ladybug-tools/dragonfly-radiance
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dragonfly-radiance-0.3.8/dragonfly_radiance.egg-info/SOURCES.txt` & `dragonfly-radiance-0.3.9/dragonfly_radiance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dragonfly-radiance-0.3.8/setup.py` & `dragonfly-radiance-0.3.9/setup.py`

 * *Files identical despite different names*

