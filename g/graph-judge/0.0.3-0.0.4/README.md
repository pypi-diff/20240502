# Comparing `tmp/graph_judge-0.0.3.tar.gz` & `tmp/graph_judge-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_judge-0.0.3.tar", last modified: Thu May  2 20:35:42 2024, max compression
+gzip compressed data, was "graph_judge-0.0.4.tar", last modified: Thu May  2 20:38:50 2024, max compression
```

## Comparing `graph_judge-0.0.3.tar` & `graph_judge-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 20:35:42.218867 graph_judge-0.0.3/
--rw-rw-rw-   0        0        0    35823 2024-05-02 19:31:03.000000 graph_judge-0.0.3/LICENSE.md
--rw-rw-rw-   0        0        0      199 2024-05-02 20:35:42.217634 graph_judge-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       15 2024-05-02 20:04:09.000000 graph_judge-0.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-02 20:35:42.214095 graph_judge-0.0.3/graph_judge/
--rw-rw-rw-   0        0        0       24 2024-05-02 20:35:11.000000 graph_judge-0.0.3/graph_judge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:35:42.217634 graph_judge-0.0.3/graph_judge.egg-info/
--rw-rw-rw-   0        0        0      199 2024-05-02 20:35:42.000000 graph_judge-0.0.3/graph_judge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-05-02 20:35:42.000000 graph_judge-0.0.3/graph_judge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 20:35:42.000000 graph_judge-0.0.3/graph_judge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-02 20:35:42.000000 graph_judge-0.0.3/graph_judge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 20:35:42.218867 graph_judge-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      605 2024-05-02 20:35:30.000000 graph_judge-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:38:50.795834 graph_judge-0.0.4/
+-rw-rw-rw-   0        0        0    35823 2024-05-02 19:31:03.000000 graph_judge-0.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0      256 2024-05-02 20:38:50.795834 graph_judge-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2024-05-02 20:04:09.000000 graph_judge-0.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-02 20:38:50.795834 graph_judge-0.0.4/graph_judge/
+-rw-rw-rw-   0        0        0       24 2024-05-02 20:35:11.000000 graph_judge-0.0.4/graph_judge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:38:50.795834 graph_judge-0.0.4/graph_judge.egg-info/
+-rw-rw-rw-   0        0        0      256 2024-05-02 20:38:50.000000 graph_judge-0.0.4/graph_judge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2024-05-02 20:38:50.000000 graph_judge-0.0.4/graph_judge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 20:38:50.000000 graph_judge-0.0.4/graph_judge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-02 20:38:50.000000 graph_judge-0.0.4/graph_judge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 20:38:50.795834 graph_judge-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      662 2024-05-02 20:38:49.000000 graph_judge-0.0.4/setup.py
```

### Comparing `graph_judge-0.0.3/LICENSE.md` & `graph_judge-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `graph_judge-0.0.3/setup.py` & `graph_judge-0.0.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
 
 
@@ -15,14 +15,15 @@
 setup(
     name='graph_judge',
     packages=find_packages(),
     version=VERSION,
     description='TODO edit me',
     author='Spencer Hanson',
     long_description=long_description,
+    url="https://github.com/spencer-hanson/GraphJudge",
     install_requires=parse_requirements('requirements.txt'),
     keywords=[],
     classifiers=[
         'Programming Language :: Python :: 3'
     ]
 )
```

