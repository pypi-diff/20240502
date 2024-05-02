# Comparing `tmp/ml_project_tracker-0.0.3.dev7.tar.gz` & `tmp/ml_project_tracker-0.0.3.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_project_tracker-0.0.3.dev7.tar", last modified: Thu May  2 13:18:41 2024, max compression
+gzip compressed data, was "ml_project_tracker-0.0.3.dev8.tar", last modified: Thu May  2 13:20:28 2024, max compression
```

## Comparing `ml_project_tracker-0.0.3.dev7.tar` & `ml_project_tracker-0.0.3.dev8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:18:41.954946 ml_project_tracker-0.0.3.dev7/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:18:41.954946 ml_project_tracker-0.0.3.dev7/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev7/README.md
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:18:41.950946 ml_project_tracker-0.0.3.dev7/ml_project_tracker/
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker/__init__.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     7357 2024-05-02 13:18:26.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker/neptune_tools.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker/wandb_tools.py
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:18:41.954946 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:18:41.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 13:18:41.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 13:18:41.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:18:41.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/requires.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 13:18:41.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/top_level.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:18:41.954946 ml_project_tracker-0.0.3.dev7/setup.cfg
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 13:18:40.000000 ml_project_tracker-0.0.3.dev7/setup.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:20:28.162485 ml_project_tracker-0.0.3.dev8/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:20:28.162485 ml_project_tracker-0.0.3.dev8/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev8/README.md
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:20:28.158485 ml_project_tracker-0.0.3.dev8/ml_project_tracker/
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker/__init__.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     7324 2024-05-02 13:20:06.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker/neptune_tools.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker/wandb_tools.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:20:28.162485 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:20:28.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 13:20:28.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 13:20:28.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:20:28.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/requires.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 13:20:28.000000 ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:20:28.162485 ml_project_tracker-0.0.3.dev8/setup.cfg
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 13:20:26.000000 ml_project_tracker-0.0.3.dev8/setup.py
```

### Comparing `ml_project_tracker-0.0.3.dev7/PKG-INFO` & `ml_project_tracker-0.0.3.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev7
+Version: 0.0.3.dev8
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev7/ml_project_tracker/neptune_tools.py` & `ml_project_tracker-0.0.3.dev8/ml_project_tracker/neptune_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,19 +63,19 @@
             with open(run_id_file, 'r') as file:
                 run_ids = json.load(file)
 
             # Check if the run name already exists in the run IDs
             if run_name in run_ids:
                 run_id = run_ids[run_name]
                 # Resume the existing run
-                self.run = neptune.init_run(api_token= NeptuneLogger.api_token, project=NeptuneLogger.project_name, with_id=run_id,  timestamp=None)
+                self.run = neptune.init_run(api_token= NeptuneLogger.api_token, project=NeptuneLogger.project_name, with_id=run_id)
     
             else:
                 # Initialize a new run with the specified project name and run name
-                self.run = neptune.init_run(api_token= NeptuneLogger.api_token, project=NeptuneLogger.project_name, name=run_name, timestamp=None)
+                self.run = neptune.init_run(api_token= NeptuneLogger.api_token, project=NeptuneLogger.project_name, name=run_name)
                 # Get the run ID
                 run_id = self.run["sys/id"].fetch()
                 # Update the run IDs dictionary
                 run_ids[run_name] = run_id
             
                 # Dump the updated run IDs to the file
                 with open(run_id_file, 'w') as file:
```

### Comparing `ml_project_tracker-0.0.3.dev7/ml_project_tracker/wandb_tools.py` & `ml_project_tracker-0.0.3.dev8/ml_project_tracker/wandb_tools.py`

 * *Files identical despite different names*

### Comparing `ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/PKG-INFO` & `ml_project_tracker-0.0.3.dev8/ml_project_tracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev7
+Version: 0.0.3.dev8
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev7/setup.py` & `ml_project_tracker-0.0.3.dev8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ml-project-tracker',
-    version='0.0.3.dev7',
+    version='0.0.3.dev8',
     description='A package for tracking the ML projects',
     author='Lilia MAHDID',
     author_email='jl_mahdid@esi.dz',
     packages=find_packages(exclude=['requirements.sh', 'build.sh']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/mahdid-lilia/ML-Project-Tracker',
```

