# Comparing `tmp/ml_project_tracker-0.0.3.tar.gz` & `tmp/ml_project_tracker-0.0.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_project_tracker-0.0.3.tar", last modified: Thu May  2 08:11:01 2024, max compression
+gzip compressed data, was "ml_project_tracker-0.0.3.dev1.tar", last modified: Thu May  2 08:19:15 2024, max compression
```

## Comparing `ml_project_tracker-0.0.3.tar` & `ml_project_tracker-0.0.3.dev1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 08:11:01.012434 ml_project_tracker-0.0.3/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      592 2024-05-02 08:11:01.012434 ml_project_tracker-0.0.3/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3/README.md
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 08:11:01.012434 ml_project_tracker-0.0.3/ml_project_tracker/
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       40 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3/ml_project_tracker/__init__.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     6860 2024-05-02 07:56:13.000000 ml_project_tracker-0.0.3/ml_project_tracker/neptune_tools.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3/ml_project_tracker/wandb_tools.py
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 08:11:01.012434 ml_project_tracker-0.0.3/ml_project_tracker.egg-info/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      592 2024-05-02 08:11:01.000000 ml_project_tracker-0.0.3/ml_project_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 08:11:01.000000 ml_project_tracker-0.0.3/ml_project_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 08:11:01.000000 ml_project_tracker-0.0.3/ml_project_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 08:11:01.000000 ml_project_tracker-0.0.3/ml_project_tracker.egg-info/requires.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 08:11:01.000000 ml_project_tracker-0.0.3/ml_project_tracker.egg-info/top_level.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 08:11:01.012434 ml_project_tracker-0.0.3/setup.cfg
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      925 2024-05-02 08:10:57.000000 ml_project_tracker-0.0.3/setup.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 08:19:15.593798 ml_project_tracker-0.0.3.dev1/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 08:19:15.593798 ml_project_tracker-0.0.3.dev1/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev1/README.md
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 08:19:15.593798 ml_project_tracker-0.0.3.dev1/ml_project_tracker/
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker/__init__.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     6860 2024-05-02 07:56:13.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker/neptune_tools.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker/wandb_tools.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 08:19:15.593798 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 08:19:15.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 08:19:15.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 08:19:15.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 08:19:15.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/requires.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 08:19:15.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 08:19:15.593798 ml_project_tracker-0.0.3.dev1/setup.cfg
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 08:19:07.000000 ml_project_tracker-0.0.3.dev1/setup.py
```

### Comparing `ml_project_tracker-0.0.3/PKG-INFO` & `ml_project_tracker-0.0.3.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3
+Version: 0.0.3.dev1
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3/ml_project_tracker/neptune_tools.py` & `ml_project_tracker-0.0.3.dev1/ml_project_tracker/neptune_tools.py`

 * *Files identical despite different names*

### Comparing `ml_project_tracker-0.0.3/ml_project_tracker/wandb_tools.py` & `ml_project_tracker-0.0.3.dev1/ml_project_tracker/wandb_tools.py`

 * *Files identical despite different names*

### Comparing `ml_project_tracker-0.0.3/ml_project_tracker.egg-info/PKG-INFO` & `ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3
+Version: 0.0.3.dev1
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3/setup.py` & `ml_project_tracker-0.0.3.dev1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ml-project-tracker',
-    version='0.0.3',
+    version='0.0.3.dev1',
     description='A package for tracking the ML projects',
     author='Lilia MAHDID',
     author_email='jl_mahdid@esi.dz',
     packages=find_packages(exclude=['requirements.sh', 'build.sh']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/mahdid-lilia/ML-Project-Tracker',
```

