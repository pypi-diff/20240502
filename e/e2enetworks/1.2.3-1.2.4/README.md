# Comparing `tmp/e2enetworks-1.2.3.tar.gz` & `tmp/e2enetworks-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-1.2.3.tar", last modified: Fri Apr 26 12:50:45 2024, max compression
+gzip compressed data, was "e2enetworks-1.2.4.tar", last modified: Thu May  2 10:18:52 2024, max compression
```

## Comparing `e2enetworks-1.2.3.tar` & `e2enetworks-1.2.4.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-26 12:50:45.184798 e2enetworks-1.2.3/
--rw-r--r--   0 jagga      (501) staff       (20)    10786 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/LICENSE.txt
--rw-r--r--   0 jagga      (501) staff       (20)     1418 2024-04-26 12:50:45.184532 e2enetworks-1.2.3/PKG-INFO
--rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/README.rst
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-26 12:50:45.178562 e2enetworks-1.2.3/e2enetworks/
--rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/__init__.py
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-26 12:50:45.179627 e2enetworks-1.2.3/e2enetworks/cloud/
--rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/__init__.py
--rw-r--r--   0 jagga      (501) staff       (20)      147 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/test.py
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-26 12:50:45.183981 e2enetworks-1.2.3/e2enetworks/cloud/tir/
--rw-r--r--   0 jagga      (501) staff       (20)     2290 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/__init__.py
--rw-r--r--   0 jagga      (501) staff       (20)     9305 2024-04-17 10:17:07.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/api_client.py
--rw-r--r--   0 jagga      (501) staff       (20)     2794 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/apitoken.py
--rw-r--r--   0 jagga      (501) staff       (20)     9405 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/client.py
--rw-r--r--   0 jagga      (501) staff       (20)     8779 2024-04-26 12:46:31.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/constants.py
--rw-r--r--   0 jagga      (501) staff       (20)     5788 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/datasets.py
--rw-r--r--   0 jagga      (501) staff       (20)    13823 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/endpoints.py
--rw-r--r--   0 jagga      (501) staff       (20)     2619 2024-04-17 10:17:07.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/helpers.py
--rw-r--r--   0 jagga      (501) staff       (20)     1368 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/images.py
--rw-r--r--   0 jagga      (501) staff       (20)     2105 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/minio_service.py
--rw-r--r--   0 jagga      (501) staff       (20)     6455 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/models.py
--rw-r--r--   0 jagga      (501) staff       (20)     6022 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/notebook.py
--rw-r--r--   0 jagga      (501) staff       (20)     9999 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/pipelines.py
--rw-r--r--   0 jagga      (501) staff       (20)     2849 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/projects.py
--rw-r--r--   0 jagga      (501) staff       (20)     4268 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/skus.py
--rw-r--r--   0 jagga      (501) staff       (20)     2391 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/teams.py
--rw-r--r--   0 jagga      (501) staff       (20)     1159 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/utils.py
--rw-r--r--   0 jagga      (501) staff       (20)       23 2024-04-15 09:47:56.000000 e2enetworks-1.2.3/e2enetworks/cloud/tir/version.py
--rw-r--r--   0 jagga      (501) staff       (20)     1561 2024-04-26 12:43:02.000000 e2enetworks-1.2.3/e2enetworks/constants.py
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-26 12:50:45.184229 e2enetworks-1.2.3/e2enetworks.egg-info/
--rw-r--r--   0 jagga      (501) staff       (20)     1418 2024-04-26 12:50:45.000000 e2enetworks-1.2.3/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 jagga      (501) staff       (20)      914 2024-04-26 12:50:45.000000 e2enetworks-1.2.3/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 jagga      (501) staff       (20)        1 2024-04-26 12:50:45.000000 e2enetworks-1.2.3/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 jagga      (501) staff       (20)      138 2024-04-26 12:50:45.000000 e2enetworks-1.2.3/e2enetworks.egg-info/requires.txt
--rw-r--r--   0 jagga      (501) staff       (20)       12 2024-04-26 12:50:45.000000 e2enetworks-1.2.3/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 jagga      (501) staff       (20)       38 2024-04-26 12:50:45.184851 e2enetworks-1.2.3/setup.cfg
--rw-r--r--   0 jagga      (501) staff       (20)     1829 2024-04-26 12:49:58.000000 e2enetworks-1.2.3/setup.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.197772 e2enetworks-1.2.4/
+-rw-r--r--   0 aman       (501) staff       (20)    10786 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/LICENSE.txt
+-rw-r--r--   0 aman       (501) staff       (20)     1160 2024-05-02 10:18:52.197592 e2enetworks-1.2.4/PKG-INFO
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/README.rst
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.189750 e2enetworks-1.2.4/e2enetworks/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/__init__.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.191265 e2enetworks-1.2.4/e2enetworks/cloud/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)      147 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/test.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.196534 e2enetworks-1.2.4/e2enetworks/cloud/tir/
+-rw-r--r--   0 aman       (501) staff       (20)     2390 2024-05-01 12:23:40.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)     9305 2024-04-23 09:50:02.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/api_client.py
+-rw-r--r--   0 aman       (501) staff       (20)     2794 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/apitoken.py
+-rw-r--r--   0 aman       (501) staff       (20)     9394 2024-05-01 11:52:21.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/client.py
+-rw-r--r--   0 aman       (501) staff       (20)     8779 2024-05-02 06:03:17.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/constants.py
+-rw-r--r--   0 aman       (501) staff       (20)     5630 2024-05-01 11:21:31.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/datasets.py
+-rw-r--r--   0 aman       (501) staff       (20)    13823 2023-12-15 09:21:32.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/endpoints.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.197276 e2enetworks-1.2.4/e2enetworks/cloud/tir/finetuning/
+-rw-r--r--   0 aman       (501) staff       (20)        0 2024-04-30 09:51:50.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/finetuning/__init__.py
+-rw-r--r--   0 aman       (501) staff       (20)      382 2024-05-01 09:25:21.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/finetuning/constants.py
+-rw-r--r--   0 aman       (501) staff       (20)     9809 2024-05-02 06:26:59.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/finetuning/finetuner.py
+-rw-r--r--   0 aman       (501) staff       (20)     3057 2024-04-30 05:41:18.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/helpers.py
+-rw-r--r--   0 aman       (501) staff       (20)     1368 2023-11-28 07:27:23.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/images.py
+-rw-r--r--   0 aman       (501) staff       (20)     2105 2024-04-23 09:50:02.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/minio_service.py
+-rw-r--r--   0 aman       (501) staff       (20)     6455 2024-04-23 09:50:02.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/models.py
+-rw-r--r--   0 aman       (501) staff       (20)     6022 2023-12-15 09:21:32.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/notebook.py
+-rw-r--r--   0 aman       (501) staff       (20)     9999 2023-12-15 09:21:32.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/pipelines.py
+-rw-r--r--   0 aman       (501) staff       (20)     2849 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/projects.py
+-rw-r--r--   0 aman       (501) staff       (20)     4268 2024-05-01 10:15:57.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/skus.py
+-rw-r--r--   0 aman       (501) staff       (20)     2391 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/teams.py
+-rw-r--r--   0 aman       (501) staff       (20)     1059 2024-05-02 06:16:05.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/utils.py
+-rw-r--r--   0 aman       (501) staff       (20)       23 2023-11-21 11:03:20.000000 e2enetworks-1.2.4/e2enetworks/cloud/tir/version.py
+-rw-r--r--   0 aman       (501) staff       (20)     1561 2024-05-02 06:03:17.000000 e2enetworks-1.2.4/e2enetworks/constants.py
+drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-02 10:18:52.190865 e2enetworks-1.2.4/e2enetworks.egg-info/
+-rw-r--r--   0 aman       (501) staff       (20)     1160 2024-05-02 10:18:52.000000 e2enetworks-1.2.4/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 aman       (501) staff       (20)     1051 2024-05-02 10:18:52.000000 e2enetworks-1.2.4/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 aman       (501) staff       (20)        1 2024-05-02 10:18:52.000000 e2enetworks-1.2.4/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 aman       (501) staff       (20)       40 2024-05-02 10:18:52.000000 e2enetworks-1.2.4/e2enetworks.egg-info/requires.txt
+-rw-r--r--   0 aman       (501) staff       (20)       12 2024-05-02 10:18:52.000000 e2enetworks-1.2.4/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 aman       (501) staff       (20)       38 2024-05-02 10:18:52.197838 e2enetworks-1.2.4/setup.cfg
+-rw-r--r--   0 aman       (501) staff       (20)     1710 2024-05-02 07:30:01.000000 e2enetworks-1.2.4/setup.py
```

### Comparing `e2enetworks-1.2.3/LICENSE.txt` & `e2enetworks-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/PKG-INFO` & `e2enetworks-1.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 1.2.3
+Version: 1.2.4
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
@@ -23,15 +23,7 @@
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: requests~=2.30.0
-Requires-Dist: urllib3==1.26.6
-Requires-Dist: kfp==1.8.22
-Requires-Dist: kfp-pipeline-spec==0.1.16
-Requires-Dist: kfp-server-api==1.8.5
-Requires-Dist: minio==7.1.3
-Requires-Dist: prettytable==3.9.0
-Requires-Dist: tqdm==4.66.2
```

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/__init__.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from e2enetworks.cloud.tir.models import Models
 from e2enetworks.cloud.tir.notebook import Notebooks
 from e2enetworks.cloud.tir.pipelines import PipelineClient
 from e2enetworks.cloud.tir.projects import Projects
 from e2enetworks.cloud.tir.skus import Plans
 from e2enetworks.cloud.tir.teams import Teams
 from e2enetworks.cloud.tir.api_client import ModelAPIClient
+from e2enetworks.cloud.tir.finetuning.finetuner import FinetuningClient
 
 init = client.Default.init
 
 __all__ = (
     "init",
     "PipelineClient"
 )
@@ -52,11 +53,12 @@
     Notebooks.help()
     Datasets.help()
     EndPoints.help()
     PipelineClient.help()
     Models.help()
     APITokens.help()
     ModelAPIClient.help()
+    FinetuningClient.help()
 
 
 def list_endpoint_plans():
     return Plans().list_endpoint_plans()
```

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/api_client.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/api_client.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/apitoken.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/apitoken.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/client.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import kfp
 from e2enetworks.cloud.tir import client
 from typing import Optional
 from requests import Request, Session, Response
 import e2enetworks.constants as constants
 
 E2E_UI_HOST = "localhost:3000"
```

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/constants.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/constants.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/datasets.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/datasets.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,49 +24,41 @@
 
         if project:
             client.Default.set_project(project)
 
         if team:
             client.Default.set_team(team)
 
-    def create(self, name=None, bucket_name=None, bucket_type=None, description=""):
+    def create(self, name, bucket_name=None, bucket_type='managed', description=""):
         payload = json.dumps({
             "type": bucket_type,
             "name": name,
             "bucket_name": bucket_name,
             "description": description,
         })
         headers['Authorization'] = f'Bearer {client.Default.access_token()}'
         url = f"{BASE_GPU_URL}teams/{client.Default.team()}/projects/{client.Default.project()}/datasets/?" \
               f"apikey={client.Default.api_key()}"
         response = requests.post(url=url, headers=headers, data=payload)
         return prepare_object(response)
 
     def get(self, dataset_id):
-
-        if type(dataset_id) != int:
-            raise ValueError(dataset_id)
-
         url = f"{BASE_GPU_URL}teams/{client.Default.team()}/projects/{client.Default.project()}/datasets/" \
               f"{dataset_id}/"
         req = requests.Request('GET', url)
         response = client.Default.make_request(req)
         return prepare_object(response)
 
     def list(self):
-
         url = f"{BASE_GPU_URL}teams/{client.Default.team()}/projects/{client.Default.project()}/datasets/"
         req = requests.Request('GET', url)
         response = client.Default.make_request(req)
         return prepare_object(response)
 
     def delete(self, dataset_id):
-        if type(dataset_id) != int:
-            raise ValueError(dataset_id)
-
         url = f"{BASE_GPU_URL}teams/{client.Default.team()}/projects/{client.Default.project()}/datasets/" \
               f"{dataset_id}/"
         req = requests.Request('DELETE', url)
         response = client.Default.make_request(req)
         return prepare_object(response)
     
     def upload_dataset(self, dataset_path, prefix="", dataset_id=None):
```

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/endpoints.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/endpoints.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/helpers.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,7 +62,19 @@
             key_data["data"].append(parameters.get(input_key))
             fromatted_data["inputs"].append(key_data)
         else:
             extra_keys.append(input_key)
     if len(extra_keys):
         return False, extra_keys
     return True, fromatted_data
+
+
+def get_argument_from_kwargs(argument_name, kwargs, type=str, default="", is_required=False):
+    try:
+        value = kwargs[argument_name]
+    except KeyError as e:
+        if is_required:
+            raise Exception(f'Argument is a required : {argument_name}')
+        value = default
+    if not isinstance(value, type):
+        raise TypeError(f"Argument type is invalid : {argument_name}, valid types are {type}")
+    return value
```

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/images.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/images.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/minio_service.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/minio_service.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/models.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/models.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/notebook.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/notebook.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/pipelines.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/pipelines.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/projects.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/projects.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/skus.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/skus.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/teams.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/teams.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks/cloud/tir/utils.py` & `e2enetworks-1.2.4/e2enetworks/cloud/tir/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import yaml
 import json
 from typing import Dict, Any
 from requests import Response
-from kfp_server_api import ApiListExperimentsResponse, ApiExperiment
 from types import SimpleNamespace
 
 
 def load_yaml(
         path: str,
 ) -> Dict[str, Any]:
     _load_from_local(path)
@@ -17,19 +16,18 @@
         return yaml.safe_load(f)
 
 
 def load_json(b: bytes, object_hook=None) -> Dict:
     return json.loads(b, object_hook=object_hook)
 
 
-def prepare_object(response: Response) -> ApiListExperimentsResponse:
+def prepare_object(response: Response):
     if not response.ok:
         try:
             output = response.json()
-
         except:
             output = response.reason
         print("failed to load response:", output)
         return None
     response = load_json(response.content, object_hook=lambda d: SimpleNamespace(**d))
     return response.data if hasattr(response, "data") else response
```

### Comparing `e2enetworks-1.2.3/e2enetworks/constants.py` & `e2enetworks-1.2.4/e2enetworks/constants.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.3/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-1.2.4/e2enetworks.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 1.2.3
+Version: 1.2.4
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
@@ -23,15 +23,7 @@
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: requests~=2.30.0
-Requires-Dist: urllib3==1.26.6
-Requires-Dist: kfp==1.8.22
-Requires-Dist: kfp-pipeline-spec==0.1.16
-Requires-Dist: kfp-server-api==1.8.5
-Requires-Dist: minio==7.1.3
-Requires-Dist: prettytable==3.9.0
-Requires-Dist: tqdm==4.66.2
```

### Comparing `e2enetworks-1.2.3/e2enetworks.egg-info/SOURCES.txt` & `e2enetworks-1.2.4/e2enetworks.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,11 @@
 e2enetworks/cloud/tir/models.py
 e2enetworks/cloud/tir/notebook.py
 e2enetworks/cloud/tir/pipelines.py
 e2enetworks/cloud/tir/projects.py
 e2enetworks/cloud/tir/skus.py
 e2enetworks/cloud/tir/teams.py
 e2enetworks/cloud/tir/utils.py
-e2enetworks/cloud/tir/version.py
+e2enetworks/cloud/tir/version.py
+e2enetworks/cloud/tir/finetuning/__init__.py
+e2enetworks/cloud/tir/finetuning/constants.py
+e2enetworks/cloud/tir/finetuning/finetuner.py
```

### Comparing `e2enetworks-1.2.3/setup.py` & `e2enetworks-1.2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "1.2.3"
+version = "1.2.4"
 install_requires = [
-    "requests~=2.30.0",
-    "urllib3==1.26.6",
-    "kfp==1.8.22",
-    "kfp-pipeline-spec==0.1.16",
-    "kfp-server-api==1.8.5",
-    "minio==7.1.3",
-    "prettytable==3.9.0",
-    "tqdm==4.66.2"
+    "requests",
+    "urllib3",
+    "minio",
+    "prettytable",
+    "tqdm"
 ]
 # read the contents of your README file
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst")) as f:
     long_description = f.read()
```

