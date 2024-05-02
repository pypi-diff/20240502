# Comparing `tmp/gddoc2yml-0.0.1.tar.gz` & `tmp/gddoc2yml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gddoc2yml-0.0.1.tar", last modified: Fri Apr 12 07:51:28 2024, max compression
+gzip compressed data, was "gddoc2yml-0.1.0.tar", last modified: Thu May  2 07:25:30 2024, max compression
```

## Comparing `gddoc2yml-0.0.1.tar` & `gddoc2yml-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.339531 gddoc2yml-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.339531 gddoc2yml-0.0.1/src/gddoc2yml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/src/gddoc2yml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/src/gddoc2yml/gdxml2yml.py
--rw-r--r--   0 runner    (1001) docker     (127)   106910 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/src/gddoc2yml/make_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/src/gddoc2yml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/CollisionObject3D.xml
--rw-r--r--   0 runner    (1001) docker     (127)    79398 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/Node.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20604 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/Node3D.xml
--rw-r--r--   0 runner    (1001) docker     (127)    54560 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/Object.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/PhysicsBody3D.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/StaticBody3D.xml
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/test_console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/test_gdxml2yml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:25:30.346348 gddoc2yml-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-02 07:25:30.346348 gddoc2yml-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 07:25:30.346348 gddoc2yml-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:25:30.338348 gddoc2yml-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:25:30.342348 gddoc2yml-0.1.0/src/gddoc2yml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/src/gddoc2yml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20472 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/src/gddoc2yml/gdxml2yml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44543 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/src/gddoc2yml/gdxml_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106910 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/src/gddoc2yml/make_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/src/gddoc2yml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:25:30.346348 gddoc2yml-0.1.0/src/gddoc2yml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-02 07:25:30.000000 gddoc2yml-0.1.0/src/gddoc2yml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-02 07:25:30.000000 gddoc2yml-0.1.0/src/gddoc2yml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:25:30.000000 gddoc2yml-0.1.0/src/gddoc2yml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 07:25:30.000000 gddoc2yml-0.1.0/src/gddoc2yml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 07:25:30.000000 gddoc2yml-0.1.0/src/gddoc2yml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 07:25:30.000000 gddoc2yml-0.1.0/src/gddoc2yml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:25:30.342348 gddoc2yml-0.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:25:30.342348 gddoc2yml-0.1.0/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/tests/classes/CollisionObject3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    79398 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/tests/classes/Node.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20604 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/tests/classes/Node3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    54560 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/tests/classes/Object.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/tests/classes/PhysicsBody3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/tests/classes/StaticBody3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14229 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/tests/classes/int.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/tests/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 07:25:17.000000 gddoc2yml-0.1.0/tests/test_gdxml2yml.py
```

### Comparing `gddoc2yml-0.0.1/LICENSE` & `gddoc2yml-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.1/pyproject.toml` & `gddoc2yml-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "pathvalidate>=3.2.0", "PyYAML>=6.0.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gddoc2yml"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Nick Maltbie", email="nick.dmalt@gmail.com" },
 ]
 description = "Convert godot xml docs to docfx yml"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
@@ -32,10 +32,12 @@
   "PyYAML"
 ]
 keywords = ["godot", "docfx", "yml", "xml", "documentation"]
 
 [project.urls]
 Homepage = "https://github.com/nicholas-maltbie/gddoc2yml"
 Issues = "https://github.com/nicholas-maltbie/gddoc2yml/issues"
+GitHub = "https://github.com/nicholas-maltbie/gddoc2yml"
+Changelog = "https://github.com/nicholas-maltbie/gddoc2yml/blob/main/CHANGELOG.md"
 
 [project.scripts]
 gdxml2yml = "gddoc2yml.gdxml2yml:main"
```

### Comparing `gddoc2yml-0.0.1/src/gddoc2yml/make_rst.py` & `gddoc2yml-0.1.0/src/gddoc2yml/make_rst.py`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.1/tests/classes/CollisionObject3D.xml` & `gddoc2yml-0.1.0/tests/classes/CollisionObject3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.1/tests/classes/Node.xml` & `gddoc2yml-0.1.0/tests/classes/Node.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.1/tests/classes/Node3D.xml` & `gddoc2yml-0.1.0/tests/classes/Node3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.1/tests/classes/Object.xml` & `gddoc2yml-0.1.0/tests/classes/Object.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.1/tests/classes/PhysicsBody3D.xml` & `gddoc2yml-0.1.0/tests/classes/PhysicsBody3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.1/tests/classes/StaticBody3D.xml` & `gddoc2yml-0.1.0/tests/classes/StaticBody3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.1/tests/test_console.py` & `gddoc2yml-0.1.0/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.1/tests/test_gdxml2yml.py` & `gddoc2yml-0.1.0/tests/test_gdxml2yml.py`

 * *Files identical despite different names*

