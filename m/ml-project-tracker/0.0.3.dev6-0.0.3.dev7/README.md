# Comparing `tmp/ml_project_tracker-0.0.3.dev6.tar.gz` & `tmp/ml_project_tracker-0.0.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_project_tracker-0.0.3.dev6.tar", last modified: Thu May  2 13:15:31 2024, max compression
+gzip compressed data, was "ml_project_tracker-0.0.3.dev7.tar", last modified: Thu May  2 13:18:41 2024, max compression
```

## Comparing `ml_project_tracker-0.0.3.dev6.tar` & `ml_project_tracker-0.0.3.dev7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:15:31.671772 ml_project_tracker-0.0.3.dev6/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:15:31.671772 ml_project_tracker-0.0.3.dev6/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev6/README.md
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:15:31.671772 ml_project_tracker-0.0.3.dev6/ml_project_tracker/
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker/__init__.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     7750 2024-05-02 13:14:22.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker/neptune_tools.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker/wandb_tools.py
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:15:31.671772 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:15:31.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 13:15:31.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 13:15:31.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:15:31.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/requires.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 13:15:31.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/top_level.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:15:31.671772 ml_project_tracker-0.0.3.dev6/setup.cfg
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 13:15:29.000000 ml_project_tracker-0.0.3.dev6/setup.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:18:41.954946 ml_project_tracker-0.0.3.dev7/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:18:41.954946 ml_project_tracker-0.0.3.dev7/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev7/README.md
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:18:41.950946 ml_project_tracker-0.0.3.dev7/ml_project_tracker/
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker/__init__.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     7357 2024-05-02 13:18:26.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker/neptune_tools.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker/wandb_tools.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:18:41.954946 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:18:41.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 13:18:41.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 13:18:41.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:18:41.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/requires.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 13:18:41.000000 ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:18:41.954946 ml_project_tracker-0.0.3.dev7/setup.cfg
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 13:18:40.000000 ml_project_tracker-0.0.3.dev7/setup.py
```

### Comparing `ml_project_tracker-0.0.3.dev6/PKG-INFO` & `ml_project_tracker-0.0.3.dev7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev6
+Version: 0.0.3.dev7
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev6/ml_project_tracker/neptune_tools.py` & `ml_project_tracker-0.0.3.dev7/ml_project_tracker/neptune_tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -63,37 +63,28 @@
             with open(run_id_file, 'r') as file:
                 run_ids = json.load(file)
 
             # Check if the run name already exists in the run IDs
             if run_name in run_ids:
                 run_id = run_ids[run_name]
                 # Resume the existing run
-                self.run = neptune.init_run(api_token= NeptuneLogger.api_token, project=NeptuneLogger.project_name, with_id=run_id)
+                self.run = neptune.init_run(api_token= NeptuneLogger.api_token, project=NeptuneLogger.project_name, with_id=run_id,  timestamp=None)
     
             else:
                 # Initialize a new run with the specified project name and run name
-                self.run = neptune.init_run(api_token= NeptuneLogger.api_token, project=NeptuneLogger.project_name, name=run_name)
+                self.run = neptune.init_run(api_token= NeptuneLogger.api_token, project=NeptuneLogger.project_name, name=run_name, timestamp=None)
                 # Get the run ID
                 run_id = self.run["sys/id"].fetch()
                 # Update the run IDs dictionary
                 run_ids[run_name] = run_id
             
                 # Dump the updated run IDs to the file
                 with open(run_id_file, 'w') as file:
                         json.dump(run_ids, file)
-            # Check if there are any logged timestamps
-            logged_timestamps = self.run["monitoring/f5430792/stdout"].fetch()
-            if logged_timestamps:
-                # Get the latest timestamp
-                latest_timestamp = max(logged_timestamps)
-            else:
-                latest_timestamp = None
-
-            # Store the latest timestamp
-            self.latest_timestamp = latest_timestamp
+            
 
         def log_files_neptune(self, file_path, file_name):
             """
             Logs files to Neptune.
 
             Args:
                 run: Neptune run object.
@@ -105,15 +96,15 @@
             """
             assert isinstance(file_path, str), "file_path must be a string"
             assert isinstance(file_name, str), "file_name must be a string"
 
             # # Generate timestamp
             # timestamp = time.time()  # Current time in seconds since epoch
 
-            self.run[file_name].upload(file_path, timestamp=self.latest_timestamp)
+            self.run[file_name].upload(file_path, timestamp=None)
         def stop_run(self):
             """
             Stops the Neptune run and synchronizes the data with the Neptune servers.
 
             Args:
                 run: Neptune run object.
```

### Comparing `ml_project_tracker-0.0.3.dev6/ml_project_tracker/wandb_tools.py` & `ml_project_tracker-0.0.3.dev7/ml_project_tracker/wandb_tools.py`

 * *Files identical despite different names*

### Comparing `ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/PKG-INFO` & `ml_project_tracker-0.0.3.dev7/ml_project_tracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev6
+Version: 0.0.3.dev7
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev6/setup.py` & `ml_project_tracker-0.0.3.dev7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ml-project-tracker',
-    version='0.0.3.dev6',
+    version='0.0.3.dev7',
     description='A package for tracking the ML projects',
     author='Lilia MAHDID',
     author_email='jl_mahdid@esi.dz',
     packages=find_packages(exclude=['requirements.sh', 'build.sh']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/mahdid-lilia/ML-Project-Tracker',
```

