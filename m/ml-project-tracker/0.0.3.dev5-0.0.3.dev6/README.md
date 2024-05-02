# Comparing `tmp/ml_project_tracker-0.0.3.dev5.tar.gz` & `tmp/ml_project_tracker-0.0.3.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_project_tracker-0.0.3.dev5.tar", last modified: Thu May  2 13:09:46 2024, max compression
+gzip compressed data, was "ml_project_tracker-0.0.3.dev6.tar", last modified: Thu May  2 13:15:31 2024, max compression
```

## Comparing `ml_project_tracker-0.0.3.dev5.tar` & `ml_project_tracker-0.0.3.dev6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:09:46.317271 ml_project_tracker-0.0.3.dev5/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:09:46.317271 ml_project_tracker-0.0.3.dev5/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev5/README.md
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:09:46.317271 ml_project_tracker-0.0.3.dev5/ml_project_tracker/
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev5/ml_project_tracker/__init__.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     7364 2024-05-02 13:08:59.000000 ml_project_tracker-0.0.3.dev5/ml_project_tracker/neptune_tools.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev5/ml_project_tracker/wandb_tools.py
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:09:46.317271 ml_project_tracker-0.0.3.dev5/ml_project_tracker.egg-info/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:09:46.000000 ml_project_tracker-0.0.3.dev5/ml_project_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 13:09:46.000000 ml_project_tracker-0.0.3.dev5/ml_project_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 13:09:46.000000 ml_project_tracker-0.0.3.dev5/ml_project_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:09:46.000000 ml_project_tracker-0.0.3.dev5/ml_project_tracker.egg-info/requires.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 13:09:46.000000 ml_project_tracker-0.0.3.dev5/ml_project_tracker.egg-info/top_level.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:09:46.317271 ml_project_tracker-0.0.3.dev5/setup.cfg
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 13:09:44.000000 ml_project_tracker-0.0.3.dev5/setup.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:15:31.671772 ml_project_tracker-0.0.3.dev6/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:15:31.671772 ml_project_tracker-0.0.3.dev6/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev6/README.md
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:15:31.671772 ml_project_tracker-0.0.3.dev6/ml_project_tracker/
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker/__init__.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     7750 2024-05-02 13:14:22.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker/neptune_tools.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker/wandb_tools.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 13:15:31.671772 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 13:15:31.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 13:15:31.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 13:15:31.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:15:31.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/requires.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 13:15:31.000000 ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 13:15:31.671772 ml_project_tracker-0.0.3.dev6/setup.cfg
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 13:15:29.000000 ml_project_tracker-0.0.3.dev6/setup.py
```

### Comparing `ml_project_tracker-0.0.3.dev5/PKG-INFO` & `ml_project_tracker-0.0.3.dev6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev5
+Version: 0.0.3.dev6
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev5/ml_project_tracker/neptune_tools.py` & `ml_project_tracker-0.0.3.dev6/ml_project_tracker/neptune_tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -75,17 +75,25 @@
                 # Get the run ID
                 run_id = self.run["sys/id"].fetch()
                 # Update the run IDs dictionary
                 run_ids[run_name] = run_id
             
                 # Dump the updated run IDs to the file
                 with open(run_id_file, 'w') as file:
-                    json.dump(run_ids, file)
+                        json.dump(run_ids, file)
             # Check if there are any logged timestamps
+            logged_timestamps = self.run["monitoring/f5430792/stdout"].fetch()
+            if logged_timestamps:
+                # Get the latest timestamp
+                latest_timestamp = max(logged_timestamps)
+            else:
+                latest_timestamp = None
 
+            # Store the latest timestamp
+            self.latest_timestamp = latest_timestamp
 
         def log_files_neptune(self, file_path, file_name):
             """
             Logs files to Neptune.
 
             Args:
                 run: Neptune run object.
@@ -94,18 +102,18 @@
 
             Returns:
                 None
             """
             assert isinstance(file_path, str), "file_path must be a string"
             assert isinstance(file_name, str), "file_name must be a string"
 
-            # Generate timestamp
-            timestamp = time.time()  # Current time in seconds since epoch
+            # # Generate timestamp
+            # timestamp = time.time()  # Current time in seconds since epoch
 
-            self.run[file_name].upload(file_path, timestamp=timestamp)
+            self.run[file_name].upload(file_path, timestamp=self.latest_timestamp)
         def stop_run(self):
             """
             Stops the Neptune run and synchronizes the data with the Neptune servers.
 
             Args:
                 run: Neptune run object.
```

### Comparing `ml_project_tracker-0.0.3.dev5/ml_project_tracker/wandb_tools.py` & `ml_project_tracker-0.0.3.dev6/ml_project_tracker/wandb_tools.py`

 * *Files identical despite different names*

### Comparing `ml_project_tracker-0.0.3.dev5/ml_project_tracker.egg-info/PKG-INFO` & `ml_project_tracker-0.0.3.dev6/ml_project_tracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev5
+Version: 0.0.3.dev6
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev5/setup.py` & `ml_project_tracker-0.0.3.dev6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ml-project-tracker',
-    version='0.0.3.dev5',
+    version='0.0.3.dev6',
     description='A package for tracking the ML projects',
     author='Lilia MAHDID',
     author_email='jl_mahdid@esi.dz',
     packages=find_packages(exclude=['requirements.sh', 'build.sh']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/mahdid-lilia/ML-Project-Tracker',
```

