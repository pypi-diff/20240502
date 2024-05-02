# Comparing `tmp/ml_project_tracker-0.0.3.dev3.tar.gz` & `tmp/ml_project_tracker-0.0.3.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_project_tracker-0.0.3.dev3.tar", last modified: Thu May  2 11:49:21 2024, max compression
+gzip compressed data, was "ml_project_tracker-0.0.3.dev4.tar", last modified: Thu May  2 12:57:05 2024, max compression
```

## Comparing `ml_project_tracker-0.0.3.dev3.tar` & `ml_project_tracker-0.0.3.dev4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 11:49:21.185478 ml_project_tracker-0.0.3.dev3/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 11:49:21.185478 ml_project_tracker-0.0.3.dev3/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev3/README.md
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 11:49:21.185478 ml_project_tracker-0.0.3.dev3/ml_project_tracker/
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker/__init__.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     7136 2024-05-02 09:07:56.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker/neptune_tools.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker/wandb_tools.py
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 11:49:21.185478 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 11:49:21.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 11:49:21.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 11:49:21.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 11:49:21.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/requires.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 11:49:21.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/top_level.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 11:49:21.185478 ml_project_tracker-0.0.3.dev3/setup.cfg
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 11:49:19.000000 ml_project_tracker-0.0.3.dev3/setup.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 12:57:05.284570 ml_project_tracker-0.0.3.dev4/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 12:57:05.284570 ml_project_tracker-0.0.3.dev4/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev4/README.md
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 12:57:05.280570 ml_project_tracker-0.0.3.dev4/ml_project_tracker/
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev4/ml_project_tracker/__init__.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     7732 2024-05-02 12:56:38.000000 ml_project_tracker-0.0.3.dev4/ml_project_tracker/neptune_tools.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev4/ml_project_tracker/wandb_tools.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 12:57:05.284570 ml_project_tracker-0.0.3.dev4/ml_project_tracker.egg-info/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 12:57:05.000000 ml_project_tracker-0.0.3.dev4/ml_project_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 12:57:05.000000 ml_project_tracker-0.0.3.dev4/ml_project_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 12:57:05.000000 ml_project_tracker-0.0.3.dev4/ml_project_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 12:57:05.000000 ml_project_tracker-0.0.3.dev4/ml_project_tracker.egg-info/requires.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 12:57:05.000000 ml_project_tracker-0.0.3.dev4/ml_project_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 12:57:05.284570 ml_project_tracker-0.0.3.dev4/setup.cfg
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 12:57:03.000000 ml_project_tracker-0.0.3.dev4/setup.py
```

### Comparing `ml_project_tracker-0.0.3.dev3/PKG-INFO` & `ml_project_tracker-0.0.3.dev4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev3
+Version: 0.0.3.dev4
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev3/ml_project_tracker/neptune_tools.py` & `ml_project_tracker-0.0.3.dev4/ml_project_tracker/neptune_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import json
 import neptune
+import time 
 
 class NeptuneLogger:
     """
     A utility class for logging to Neptune.
 
     Attributes:
         None
@@ -75,14 +76,25 @@
                 run_id = self.run["sys/id"].fetch()
                 # Update the run IDs dictionary
                 run_ids[run_name] = run_id
             
                 # Dump the updated run IDs to the file
                 with open(run_id_file, 'w') as file:
                     json.dump(run_ids, file)
+            # Check if there are any logged timestamps
+
+            logged_timestamps = self.run["monitoring/26d09d0e/stdout"].fetch()
+            if logged_timestamps:
+                # Get the latest timestamp
+                latest_timestamp = max(logged_timestamps)
+            else:
+                latest_timestamp = None
+
+            # Store the latest timestamp
+            self.latest_timestamp = latest_timestamp
 
 
         def log_files_neptune(self, file_path, file_name):
             """
             Logs files to Neptune.
 
             Args:
@@ -92,26 +104,35 @@
 
             Returns:
                 None
             """
             assert isinstance(file_path, str), "file_path must be a string"
             assert isinstance(file_name, str), "file_name must be a string"
 
-            self.run[file_name].upload(file_path)
+            # Generate timestamp
+            timestamp = time.time()  # Current time in seconds since epoch
+
+            self.run[file_name].upload(file_path, timestamp=timestamp)
         def stop_run(self):
             """
             Stops the Neptune run and synchronizes the data with the Neptune servers.
 
             Args:
                 run: Neptune run object.
 
             Returns:
                 None
             """
             self.run.stop()
+    
+    
+    
+    
+    
+    
     # @staticmethod
     # def connect_to_neptune(api_token, project_name, run_id_dir, run_name, run_id_file_name="run_ids.json"):
     #     """
     #     Connects to Neptune and initializes a run with the provided API token, project name, and run name.
     #     If the run ID file exists:
     #         - If the run name exists, it uploads the existing run ID.
     #         - If the run name doesn't exist, it creates a new run, adds the run ID to the file with the run name as the key.
```

### Comparing `ml_project_tracker-0.0.3.dev3/ml_project_tracker/wandb_tools.py` & `ml_project_tracker-0.0.3.dev4/ml_project_tracker/wandb_tools.py`

 * *Files identical despite different names*

### Comparing `ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/PKG-INFO` & `ml_project_tracker-0.0.3.dev4/ml_project_tracker.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev3
+Version: 0.0.3.dev4
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev3/setup.py` & `ml_project_tracker-0.0.3.dev4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ml-project-tracker',
-    version='0.0.3.dev3',
+    version='0.0.3.dev4',
     description='A package for tracking the ML projects',
     author='Lilia MAHDID',
     author_email='jl_mahdid@esi.dz',
     packages=find_packages(exclude=['requirements.sh', 'build.sh']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/mahdid-lilia/ML-Project-Tracker',
```

