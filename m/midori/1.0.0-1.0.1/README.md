# Comparing `tmp/midori-1.0.0.tar.gz` & `tmp/midori-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midori-1.0.0.tar", max compression
+gzip compressed data, was "midori-1.0.1.tar", max compression
```

## Comparing `midori-1.0.0.tar` & `midori-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6670 2024-05-02 20:19:41.986739 midori-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-02 20:19:41.990738 midori-1.0.0/midori/__init__.py
--rw-r--r--   0        0        0     4640 2024-05-02 20:19:41.990738 midori-1.0.0/midori/core.py
--rw-r--r--   0        0        0     1886 2024-05-02 20:19:41.990738 midori-1.0.0/midori/plugins/base.py
--rw-r--r--   0        0        0      928 2024-05-02 20:19:41.990738 midori-1.0.0/midori/plugins/example_plugins.py
--rw-r--r--   0        0        0     5473 2024-05-02 20:19:41.990738 midori-1.0.0/midori/plugins/helpers.py
--rw-r--r--   0        0        0      484 2024-05-02 20:19:41.990738 midori-1.0.0/midori/treatments_helper.py
--rw-r--r--   0        0        0      425 2024-05-02 20:19:41.990738 midori-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7059 1970-01-01 00:00:00.000000 midori-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6670 2024-05-02 20:25:29.117017 midori-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 20:25:29.121017 midori-1.0.1/midori/__init__.py
+-rw-r--r--   0        0        0     4640 2024-05-02 20:25:29.121017 midori-1.0.1/midori/core.py
+-rw-r--r--   0        0        0     1886 2024-05-02 20:25:29.121017 midori-1.0.1/midori/plugins/base.py
+-rw-r--r--   0        0        0      928 2024-05-02 20:25:29.121017 midori-1.0.1/midori/plugins/example_plugins.py
+-rw-r--r--   0        0        0     5473 2024-05-02 20:25:29.121017 midori-1.0.1/midori/plugins/helpers.py
+-rw-r--r--   0        0        0      484 2024-05-02 20:25:29.121017 midori-1.0.1/midori/treatments_helper.py
+-rw-r--r--   0        0        0      425 2024-05-02 20:25:29.121017 midori-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7059 1970-01-01 00:00:00.000000 midori-1.0.1/PKG-INFO
```

### Comparing `midori-1.0.0/README.md` & `midori-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 - **Why Midori?** Because there are so many things to consider when it comes to running software engineering experiments, such as:
   - Cooling down before each trial.
   - SSH Connection.
   - Randomizing the order of the trials.
   - Switching between different treatments.
   - ...
-- **What is an orchestrator?** Mitori is meant to be a local tool that manipulates the remote cluster to run the experiments using SSH. In this way, the overhead of the experiment on the remote cluster is minimized.
+- **What is an orchestrator?** Midori is meant to be a local tool that manipulates the remote cluster to run the experiments using SSH. In this way, the overhead of the experiment on the remote cluster is minimized.
 
 <div align="center">
   <img src="./illustrations/communication.png" alt="Midori as an orchestrator" width="50%">
 </div>
 
 ## 🚀 Getting Started
 
@@ -60,15 +60,15 @@
 variables = {'drink': ['orange', 'apple', 'watermelon'], 'size': [300, 600, 100], 'temperature': [20, 30]}
 ```
 
 The `subject_path` should be a git repository that contains branches named `orange-300-20`, `orange-300-30`, `orange-600-20`, `orange-600-30`, etc. You do not have to include all the combinations, Midori will skip the missing branches.
 
 ### Parameters
 
-- `hostname`, `username`, `password`: Mitori needs these parameters to connect to the remote node via SSH.
+- `hostname`, `username`, `password`: Midori needs these parameters to connect to the remote node via SSH.
 - `repetitions`: The number of repetitions for the experiment.
 - `before_trial_cooling_time`: The cooling time before each trial, in seconds.
 - `trial_timespan`: The time span of each trial, in seconds.
 - `after_trial_cooling_time`: The cooling time after each trial, in seconds.
 - `variables`: The variables to be manipulated in the experiment. For example, if you have two variables, `x` and `y`, and you want to run the experiment with the values of `x` as `[1, 2, 3]` and the values of `y` as `[4, 5, 6]`, you can define the variables as `{'x': [1, 2, 3], 'y': [4, 5, 6]}`.
 - `subject_path`: The path of the subject to be run on the remote cluster. For example, if you want to run the subject in the `~/subject` directory, you can define the path as `~/subject`.
 - `before_experiment_plugins`: The plugins to be run before the experiment, such as setting environment variables, installing dependencies, close unnecessary services, etc.
```

### Comparing `midori-1.0.0/midori/core.py` & `midori-1.0.1/midori/core.py`

 * *Files identical despite different names*

### Comparing `midori-1.0.0/midori/plugins/base.py` & `midori-1.0.1/midori/plugins/base.py`

 * *Files identical despite different names*

### Comparing `midori-1.0.0/midori/plugins/example_plugins.py` & `midori-1.0.1/midori/plugins/example_plugins.py`

 * *Files identical despite different names*

### Comparing `midori-1.0.0/midori/plugins/helpers.py` & `midori-1.0.1/midori/plugins/helpers.py`

 * *Files identical despite different names*

### Comparing `midori-1.0.0/PKG-INFO` & `midori-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midori
-Version: 1.0.0
+Version: 1.0.1
 Summary: 🍃 streamline remote software engineering experiments
 Author: Xingwen Xiao
 Author-email: xingwen.xiao@student.uva.nl
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: paramiko (>=3.4.0,<4.0.0)
@@ -18,15 +18,15 @@
 
 - **Why Midori?** Because there are so many things to consider when it comes to running software engineering experiments, such as:
   - Cooling down before each trial.
   - SSH Connection.
   - Randomizing the order of the trials.
   - Switching between different treatments.
   - ...
-- **What is an orchestrator?** Mitori is meant to be a local tool that manipulates the remote cluster to run the experiments using SSH. In this way, the overhead of the experiment on the remote cluster is minimized.
+- **What is an orchestrator?** Midori is meant to be a local tool that manipulates the remote cluster to run the experiments using SSH. In this way, the overhead of the experiment on the remote cluster is minimized.
 
 <div align="center">
   <img src="./illustrations/communication.png" alt="Midori as an orchestrator" width="50%">
 </div>
 
 ## 🚀 Getting Started
 
@@ -72,15 +72,15 @@
 variables = {'drink': ['orange', 'apple', 'watermelon'], 'size': [300, 600, 100], 'temperature': [20, 30]}
 ```
 
 The `subject_path` should be a git repository that contains branches named `orange-300-20`, `orange-300-30`, `orange-600-20`, `orange-600-30`, etc. You do not have to include all the combinations, Midori will skip the missing branches.
 
 ### Parameters
 
-- `hostname`, `username`, `password`: Mitori needs these parameters to connect to the remote node via SSH.
+- `hostname`, `username`, `password`: Midori needs these parameters to connect to the remote node via SSH.
 - `repetitions`: The number of repetitions for the experiment.
 - `before_trial_cooling_time`: The cooling time before each trial, in seconds.
 - `trial_timespan`: The time span of each trial, in seconds.
 - `after_trial_cooling_time`: The cooling time after each trial, in seconds.
 - `variables`: The variables to be manipulated in the experiment. For example, if you have two variables, `x` and `y`, and you want to run the experiment with the values of `x` as `[1, 2, 3]` and the values of `y` as `[4, 5, 6]`, you can define the variables as `{'x': [1, 2, 3], 'y': [4, 5, 6]}`.
 - `subject_path`: The path of the subject to be run on the remote cluster. For example, if you want to run the subject in the `~/subject` directory, you can define the path as `~/subject`.
 - `before_experiment_plugins`: The plugins to be run before the experiment, such as setting environment variables, installing dependencies, close unnecessary services, etc.
```

