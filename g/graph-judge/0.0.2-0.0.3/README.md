# Comparing `tmp/graph_judge-0.0.2.tar.gz` & `tmp/graph_judge-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_judge-0.0.2.tar", last modified: Thu May  2 20:10:03 2024, max compression
+gzip compressed data, was "graph_judge-0.0.3.tar", last modified: Thu May  2 20:35:42 2024, max compression
```

## Comparing `graph_judge-0.0.2.tar` & `graph_judge-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 20:10:03.800000 graph_judge-0.0.2/
--rw-rw-rw-   0        0        0    35823 2024-05-02 19:31:03.000000 graph_judge-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0      256 2024-05-02 20:10:03.799353 graph_judge-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       15 2024-05-02 20:04:09.000000 graph_judge-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-02 20:10:03.794228 graph_judge-0.0.2/graph_judge/
--rw-rw-rw-   0        0        0       24 2024-05-02 19:53:13.000000 graph_judge-0.0.2/graph_judge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:10:03.798275 graph_judge-0.0.2/graph_judge.egg-info/
--rw-rw-rw-   0        0        0      256 2024-05-02 20:10:03.000000 graph_judge-0.0.2/graph_judge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-05-02 20:10:03.000000 graph_judge-0.0.2/graph_judge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 20:10:03.000000 graph_judge-0.0.2/graph_judge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-02 20:10:03.000000 graph_judge-0.0.2/graph_judge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 20:10:03.800000 graph_judge-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      662 2024-05-02 20:10:03.000000 graph_judge-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:35:42.218867 graph_judge-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2024-05-02 19:31:03.000000 graph_judge-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0      199 2024-05-02 20:35:42.217634 graph_judge-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2024-05-02 20:04:09.000000 graph_judge-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-02 20:35:42.214095 graph_judge-0.0.3/graph_judge/
+-rw-rw-rw-   0        0        0       24 2024-05-02 20:35:11.000000 graph_judge-0.0.3/graph_judge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:35:42.217634 graph_judge-0.0.3/graph_judge.egg-info/
+-rw-rw-rw-   0        0        0      199 2024-05-02 20:35:42.000000 graph_judge-0.0.3/graph_judge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2024-05-02 20:35:42.000000 graph_judge-0.0.3/graph_judge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 20:35:42.000000 graph_judge-0.0.3/graph_judge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-02 20:35:42.000000 graph_judge-0.0.3/graph_judge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 20:35:42.218867 graph_judge-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      605 2024-05-02 20:35:30.000000 graph_judge-0.0.3/setup.py
```

### Comparing `graph_judge-0.0.2/LICENSE.md` & `graph_judge-0.0.3/LICENSE.md`

 * *Files identical despite different names*

