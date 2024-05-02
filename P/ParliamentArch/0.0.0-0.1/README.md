# Comparing `tmp/parliamentarch-0.0.0.tar.gz` & `tmp/parliamentarch-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parliamentarch-0.0.0.tar", last modified: Sun Apr 14 14:13:47 2024, max compression
+gzip compressed data, was "parliamentarch-0.1.tar", last modified: Thu May  2 17:47:48 2024, max compression
```

## Comparing `parliamentarch-0.0.0.tar` & `parliamentarch-0.1.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:13:47.735324 parliamentarch-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-14 14:13:40.000000 parliamentarch-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-04-14 14:13:47.735324 parliamentarch-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-04-14 14:13:40.000000 parliamentarch-0.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-14 14:13:40.000000 parliamentarch-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 14:13:47.735324 parliamentarch-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:13:47.731324 parliamentarch-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:13:47.735324 parliamentarch-0.0.0/src/ParliamentArch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-04-14 14:13:47.000000 parliamentarch-0.0.0/src/ParliamentArch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-14 14:13:47.000000 parliamentarch-0.0.0/src/ParliamentArch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 14:13:47.000000 parliamentarch-0.0.0/src/ParliamentArch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 14:13:47.000000 parliamentarch-0.0.0/src/ParliamentArch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:13:47.735324 parliamentarch-0.0.0/src/parliamentarch/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-14 14:13:40.000000 parliamentarch-0.0.0/src/parliamentarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-14 14:13:40.000000 parliamentarch-0.0.0/src/parliamentarch/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-04-14 14:13:40.000000 parliamentarch-0.0.0/src/parliamentarch/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-14 14:13:40.000000 parliamentarch-0.0.0/src/parliamentarch/svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.157703 parliamentarch-0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.153703 parliamentarch-0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.153703 parliamentarch-0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-02 17:47:43.000000 parliamentarch-0.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-02 17:47:43.000000 parliamentarch-0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 17:47:43.000000 parliamentarch-0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-02 17:47:43.000000 parliamentarch-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-02 17:47:43.000000 parliamentarch-0.1/LISEZMOI.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14134 2024-05-02 17:47:48.157703 parliamentarch-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-05-02 17:47:43.000000 parliamentarch-0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 17:47:43.000000 parliamentarch-0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:47:48.157703 parliamentarch-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.153703 parliamentarch-0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.153703 parliamentarch-0.1/src/ParliamentArch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14134 2024-05-02 17:47:48.000000 parliamentarch-0.1/src/ParliamentArch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-02 17:47:48.000000 parliamentarch-0.1/src/ParliamentArch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:47:48.000000 parliamentarch-0.1/src/ParliamentArch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 17:47:48.000000 parliamentarch-0.1/src/ParliamentArch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.153703 parliamentarch-0.1/src/parliamentarch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-02 17:47:43.000000 parliamentarch-0.1/src/parliamentarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-02 17:47:43.000000 parliamentarch-0.1/src/parliamentarch/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-05-02 17:47:43.000000 parliamentarch-0.1/src/parliamentarch/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-02 17:47:43.000000 parliamentarch-0.1/src/parliamentarch/svg.py
```

### Comparing `parliamentarch-0.0.0/LICENSE` & `parliamentarch-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.0.0/PKG-INFO` & `parliamentarch-0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParliamentArch
-Version: 0.0.0
+Version: 0.1
 Summary: Generation of arch-styled parliamentary arches
 Author: Gouvernathor
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Gouvernathor
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `parliamentarch-0.0.0/README.rst` & `parliamentarch-0.1/README.rst`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.0.0/src/ParliamentArch.egg-info/PKG-INFO` & `parliamentarch-0.1/src/ParliamentArch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParliamentArch
-Version: 0.0.0
+Version: 0.1
 Summary: Generation of arch-styled parliamentary arches
 Author: Gouvernathor
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Gouvernathor
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `parliamentarch-0.0.0/src/parliamentarch/__init__.py` & `parliamentarch-0.1/src/parliamentarch/__init__.py`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.0.0/src/parliamentarch/_util.py` & `parliamentarch-0.1/src/parliamentarch/_util.py`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.0.0/src/parliamentarch/geometry.py` & `parliamentarch-0.1/src/parliamentarch/geometry.py`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.0.0/src/parliamentarch/svg.py` & `parliamentarch-0.1/src/parliamentarch/svg.py`

 * *Files identical despite different names*

