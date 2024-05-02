# Comparing `tmp/ml_project_tracker-0.0.3.dev1.tar.gz` & `tmp/ml_project_tracker-0.0.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_project_tracker-0.0.3.dev1.tar", last modified: Thu May  2 08:19:15 2024, max compression
+gzip compressed data, was "ml_project_tracker-0.0.3.dev3.tar", last modified: Thu May  2 11:49:21 2024, max compression
```

## Comparing `ml_project_tracker-0.0.3.dev1.tar` & `ml_project_tracker-0.0.3.dev3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 08:19:15.593798 ml_project_tracker-0.0.3.dev1/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 08:19:15.593798 ml_project_tracker-0.0.3.dev1/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev1/README.md
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 08:19:15.593798 ml_project_tracker-0.0.3.dev1/ml_project_tracker/
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker/__init__.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     6860 2024-05-02 07:56:13.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker/neptune_tools.py
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker/wandb_tools.py
-drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 08:19:15.593798 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/
--rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 08:19:15.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 08:19:15.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 08:19:15.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 08:19:15.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/requires.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 08:19:15.000000 ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/top_level.txt
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 08:19:15.593798 ml_project_tracker-0.0.3.dev1/setup.cfg
--rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 08:19:07.000000 ml_project_tracker-0.0.3.dev1/setup.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 11:49:21.185478 ml_project_tracker-0.0.3.dev3/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 11:49:21.185478 ml_project_tracker-0.0.3.dev3/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       12 2024-04-25 20:46:44.000000 ml_project_tracker-0.0.3.dev3/README.md
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 11:49:21.185478 ml_project_tracker-0.0.3.dev3/ml_project_tracker/
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       77 2024-05-02 08:18:54.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker/__init__.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     7136 2024-05-02 09:07:56.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker/neptune_tools.py
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)     4921 2024-05-02 07:07:04.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker/wandb_tools.py
+drwxrwxr-x   0 limahdid  (1002) limahdid  (1002)        0 2024-05-02 11:49:21.185478 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/
+-rw-r--r--   0 limahdid  (1002) limahdid  (1002)      597 2024-05-02 11:49:21.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      328 2024-05-02 11:49:21.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)        1 2024-05-02 11:49:21.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 11:49:21.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/requires.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       19 2024-05-02 11:49:21.000000 ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)       38 2024-05-02 11:49:21.185478 ml_project_tracker-0.0.3.dev3/setup.cfg
+-rw-rw-r--   0 limahdid  (1002) limahdid  (1002)      930 2024-05-02 11:49:19.000000 ml_project_tracker-0.0.3.dev3/setup.py
```

### Comparing `ml_project_tracker-0.0.3.dev1/PKG-INFO` & `ml_project_tracker-0.0.3.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev1
+Version: 0.0.3.dev3
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev1/ml_project_tracker/neptune_tools.py` & `ml_project_tracker-0.0.3.dev3/ml_project_tracker/neptune_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,25 @@
             Returns:
                 None
             """
             assert isinstance(file_path, str), "file_path must be a string"
             assert isinstance(file_name, str), "file_name must be a string"
 
             self.run[file_name].upload(file_path)
+        def stop_run(self):
+            """
+            Stops the Neptune run and synchronizes the data with the Neptune servers.
+
+            Args:
+                run: Neptune run object.
 
+            Returns:
+                None
+            """
+            self.run.stop()
     # @staticmethod
     # def connect_to_neptune(api_token, project_name, run_id_dir, run_name, run_id_file_name="run_ids.json"):
     #     """
     #     Connects to Neptune and initializes a run with the provided API token, project name, and run name.
     #     If the run ID file exists:
     #         - If the run name exists, it uploads the existing run ID.
     #         - If the run name doesn't exist, it creates a new run, adds the run ID to the file with the run name as the key.
```

### Comparing `ml_project_tracker-0.0.3.dev1/ml_project_tracker/wandb_tools.py` & `ml_project_tracker-0.0.3.dev3/ml_project_tracker/wandb_tools.py`

 * *Files identical despite different names*

### Comparing `ml_project_tracker-0.0.3.dev1/ml_project_tracker.egg-info/PKG-INFO` & `ml_project_tracker-0.0.3.dev3/ml_project_tracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-project-tracker
-Version: 0.0.3.dev1
+Version: 0.0.3.dev3
 Summary: A package for tracking the ML projects
 Home-page: https://github.com/mahdid-lilia/ML-Project-Tracker
 Author: Lilia MAHDID
 Author-email: jl_mahdid@esi.dz
 Keywords: Deep Learning,Machine Learning,Wandb,Neptune
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ml_project_tracker-0.0.3.dev1/setup.py` & `ml_project_tracker-0.0.3.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ml-project-tracker',
-    version='0.0.3.dev1',
+    version='0.0.3.dev3',
     description='A package for tracking the ML projects',
     author='Lilia MAHDID',
     author_email='jl_mahdid@esi.dz',
     packages=find_packages(exclude=['requirements.sh', 'build.sh']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/mahdid-lilia/ML-Project-Tracker',
```

