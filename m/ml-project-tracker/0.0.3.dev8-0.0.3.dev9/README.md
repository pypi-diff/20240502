# Comparing `tmp/ml_project_tracker-0.0.3.dev8.tar.gz` & `tmp/ml_project_tracker-0.0.3.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_project_tracker-0.0.3.dev8.tar", last modified: Thu May  2 13:20:28 2024, max compression
+gzip compressed data, was "ml_project_tracker-0.0.3.dev9.tar", last modified: Thu May  2 13:22:09 2024, max compression
```

## Comparing `ml_project_tracker-0.0.3.dev8.tar` & `ml_project_tracker-0.0.3.dev9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:20:28.162485 ml_project_tracker-0.0.3.dev8/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:20:28.162485 ml_project_tracker-0.0.3.dev8/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev8/README.md
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:20:28.158485 ml_project_tracker-0.0.3.dev8/ml_project_tracker/
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker/__init__.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     7324 2024-05-02 13:20:06.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker/neptune_tools.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker/wandb_tools.py
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:20:28.162485 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:20:28.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 13:20:28.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 13:20:28.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:20:28.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/requires.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 13:20:28.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/top_level.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:20:28.162485 ml_project_tracker-0.0.3.dev8/setup.cfg
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 13:20:26.000000 ml_project_tracker-0.0.3.dev8/setup.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:22:09.457585 ml_project_tracker-0.0.3.dev9/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:22:09.457585 ml_project_tracker-0.0.3.dev9/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev9/README.md
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:22:09.457585 ml_project_tracker-0.0.3.dev9/ml_project_tracker/
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev9/ml_project_tracker/__init__.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     7308 2024-05-02 13:21:50.000000 ml_project_tracker-0.0.3.dev9/ml_project_tracker/neptune_tools.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev9/ml_project_tracker/wandb_tools.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:22:09.457585 ml_project_tracker-0.0.3.dev9/ml_project_tracker.egg-info/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:22:09.000000 ml_project_tracker-0.0.3.dev9/ml_project_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 13:22:09.000000 ml_project_tracker-0.0.3.dev9/ml_project_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 13:22:09.000000 ml_project_tracker-0.0.3.dev9/ml_project_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:22:09.000000 ml_project_tracker-0.0.3.dev9/ml_project_tracker.egg-info/requires.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 13:22:09.000000 ml_project_tracker-0.0.3.dev9/ml_project_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:22:09.457585 ml_project_tracker-0.0.3.dev9/setup.cfg
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 13:22:07.000000 ml_project_tracker-0.0.3.dev9/setup.py
```

### Comparing `ml_project_tracker-0.0.3.dev8/PKG-INFO` & `ml_project_tracker-0.0.3.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev8
+Version: 0.0.3.dev9
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev8/ml_project_tracker/neptune_tools.py` & `ml_project_tracker-0.0.3.dev9/ml_project_tracker/neptune_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             """
             assert isinstance(file_path, str), "file_path must be a string"
             assert isinstance(file_name, str), "file_name must be a string"
 
             # # Generate timestamp
             # timestamp = time.time()  # Current time in seconds since epoch
 
-            self.run[file_name].upload(file_path, timestamp=None)
+            self.run[file_name].upload(file_path)
         def stop_run(self):
             """
             Stops the Neptune run and synchronizes the data with the Neptune servers.
 
             Args:
                 run: Neptune run object.
```

### Comparing `ml_project_tracker-0.0.3.dev8/ml_project_tracker/wandb_tools.py` & `ml_project_tracker-0.0.3.dev9/ml_project_tracker/wandb_tools.py`

 * *Files identical despite different names*

### Comparing `ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/PKG-INFO` & `ml_project_tracker-0.0.3.dev9/ml_project_tracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev8
+Version: 0.0.3.dev9
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev8/setup.py` & `ml_project_tracker-0.0.3.dev9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ml-project-tracker',
-    version='0.0.3.dev8',
+    version='0.0.3.dev9',
     description='A package for tracking the ML projects',
     author='Lilia MAHDID',
     author_email='jl_mahdid@esi.dz',
     packages=find_packages(exclude=['requirements.sh', 'build.sh']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/mahdid-lilia/ML-Project-Tracker',
```

