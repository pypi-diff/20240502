# Comparing `tmp/dagster-docker-0.23.2rc4.tar.gz` & `tmp/dagster-docker-0.23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-docker-0.23.2rc4.tar", last modified: Fri Apr 19 18:14:15 2024, max compression
+gzip compressed data, was "dagster-docker-0.23.3.tar", last modified: Thu Apr 25 20:19:15 2024, max compression
```

## Comparing `dagster-docker-0.23.2rc4.tar` & `dagster-docker-0.23.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:14:15.990538 dagster-docker-0.23.2rc4/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      696 2024-04-19 18:14:15.990538 dagster-docker-0.23.2rc4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:14:15.982538 dagster-docker-0.23.2rc4/dagster_docker/
--rw-r--r--   0 root         (0) root         (0)      553 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/dagster_docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6470 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/dagster_docker/container_context.py
--rw-r--r--   0 root         (0) root         (0)    11733 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/dagster_docker/docker_executor.py
--rw-r--r--   0 root         (0) root         (0)     7261 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/dagster_docker/docker_run_launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:14:15.986538 dagster-docker-0.23.2rc4/dagster_docker/ops/
--rw-r--r--   0 root         (0) root         (0)      143 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/dagster_docker/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6365 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/dagster_docker/ops/docker_container_op.py
--rw-r--r--   0 root         (0) root         (0)     8100 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/dagster_docker/pipes.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/dagster_docker/py.typed
--rw-r--r--   0 root         (0) root         (0)     1807 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/dagster_docker/utils.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/dagster_docker/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:14:15.986538 dagster-docker-0.23.2rc4/dagster_docker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      696 2024-04-19 18:14:15.000000 dagster-docker-0.23.2rc4/dagster_docker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2024-04-19 18:14:15.000000 dagster-docker-0.23.2rc4/dagster_docker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:14:15.000000 dagster-docker-0.23.2rc4/dagster_docker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:14:15.000000 dagster-docker-0.23.2rc4/dagster_docker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       41 2024-04-19 18:14:15.000000 dagster-docker-0.23.2rc4/dagster_docker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-19 18:14:15.000000 dagster-docker-0.23.2rc4/dagster_docker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2024-04-19 18:14:15.990538 dagster-docker-0.23.2rc4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1311 2024-04-19 18:01:50.000000 dagster-docker-0.23.2rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:19:15.282727 dagster-docker-0.23.3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      693 2024-04-25 20:19:15.282727 dagster-docker-0.23.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:19:15.282727 dagster-docker-0.23.3/dagster_docker/
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/dagster_docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/dagster_docker/container_context.py
+-rw-r--r--   0 root         (0) root         (0)    11733 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/dagster_docker/docker_executor.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/dagster_docker/docker_run_launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:19:15.282727 dagster-docker-0.23.3/dagster_docker/ops/
+-rw-r--r--   0 root         (0) root         (0)      143 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/dagster_docker/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6365 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/dagster_docker/ops/docker_container_op.py
+-rw-r--r--   0 root         (0) root         (0)     8100 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/dagster_docker/pipes.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/dagster_docker/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1807 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/dagster_docker/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/dagster_docker/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:19:15.282727 dagster-docker-0.23.3/dagster_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      693 2024-04-25 20:19:15.000000 dagster-docker-0.23.3/dagster_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2024-04-25 20:19:15.000000 dagster-docker-0.23.3/dagster_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:19:15.000000 dagster-docker-0.23.3/dagster_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:19:15.000000 dagster-docker-0.23.3/dagster_docker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 20:19:15.000000 dagster-docker-0.23.3/dagster_docker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-25 20:19:15.000000 dagster-docker-0.23.3/dagster_docker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2024-04-25 20:19:15.286727 dagster-docker-0.23.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-04-25 20:08:31.000000 dagster-docker-0.23.3/setup.py
```

### Comparing `dagster-docker-0.23.2rc4/LICENSE` & `dagster-docker-0.23.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.23.2rc4/PKG-INFO` & `dagster-docker-0.23.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-docker
-Version: 0.23.2rc4
+Version: 0.23.3
 Summary: A Dagster integration for docker
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-docker
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-docker-0.23.2rc4/dagster_docker/__init__.py` & `dagster-docker-0.23.3/dagster_docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.23.2rc4/dagster_docker/container_context.py` & `dagster-docker-0.23.3/dagster_docker/container_context.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.23.2rc4/dagster_docker/docker_executor.py` & `dagster-docker-0.23.3/dagster_docker/docker_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.23.2rc4/dagster_docker/docker_run_launcher.py` & `dagster-docker-0.23.3/dagster_docker/docker_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.23.2rc4/dagster_docker/ops/docker_container_op.py` & `dagster-docker-0.23.3/dagster_docker/ops/docker_container_op.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.23.2rc4/dagster_docker/pipes.py` & `dagster-docker-0.23.3/dagster_docker/pipes.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.23.2rc4/dagster_docker/utils.py` & `dagster-docker-0.23.3/dagster_docker/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.23.2rc4/dagster_docker.egg-info/PKG-INFO` & `dagster-docker-0.23.3/dagster_docker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-docker
-Version: 0.23.2rc4
+Version: 0.23.3
 Summary: A Dagster integration for docker
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-docker
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-docker-0.23.2rc4/dagster_docker.egg-info/SOURCES.txt` & `dagster-docker-0.23.3/dagster_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-docker-0.23.2rc4/setup.py` & `dagster-docker-0.23.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,10 +30,10 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_docker_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.2rc4", "docker", "docker-image-py"],
+    install_requires=["dagster==1.7.3", "docker", "docker-image-py"],
     zip_safe=False,
 )
```

