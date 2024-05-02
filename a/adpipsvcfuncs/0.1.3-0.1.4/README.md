# Comparing `tmp/adpipsvcfuncs-0.1.3.tar.gz` & `tmp/adpipsvcfuncs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adpipsvcfuncs-0.1.3.tar", last modified: Thu Apr 11 18:52:04 2024, max compression
+gzip compressed data, was "adpipsvcfuncs-0.1.4.tar", last modified: Thu May  2 20:11:58 2024, max compression
```

## Comparing `adpipsvcfuncs-0.1.3.tar` & `adpipsvcfuncs-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:52:04.786392 adpipsvcfuncs-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-04-11 18:51:10.000000 adpipsvcfuncs-0.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-11 18:52:04.786392 adpipsvcfuncs-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       74 2024-04-11 18:51:10.000000 adpipsvcfuncs-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:52:04.782391 adpipsvcfuncs-0.1.3/adpipsvcfuncs/
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-11 18:51:10.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-04-11 18:51:10.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs/adpipsvcfuncs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:52:04.786392 adpipsvcfuncs-0.1.3/adpipsvcfuncs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-11 18:52:04.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2024-04-11 18:52:04.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:52:04.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-11 18:52:04.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 18:52:04.786392 adpipsvcfuncs-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      424 2024-04-11 18:51:10.000000 adpipsvcfuncs-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:11:58.954490 adpipsvcfuncs-0.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-02 20:11:27.000000 adpipsvcfuncs-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      329 2024-05-02 20:11:58.954490 adpipsvcfuncs-0.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       74 2024-05-02 20:11:27.000000 adpipsvcfuncs-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:11:58.954490 adpipsvcfuncs-0.1.4/adpipsvcfuncs/
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-02 20:11:27.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-05-02 20:11:27.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs/adpipsvcfuncs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:11:58.954490 adpipsvcfuncs-0.1.4/adpipsvcfuncs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      329 2024-05-02 20:11:58.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-02 20:11:58.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:11:58.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-02 20:11:58.000000 adpipsvcfuncs-0.1.4/adpipsvcfuncs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 20:11:58.954490 adpipsvcfuncs-0.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      424 2024-05-02 20:11:27.000000 adpipsvcfuncs-0.1.4/setup.py
```

### Comparing `adpipsvcfuncs-0.1.3/LICENSE` & `adpipsvcfuncs-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adpipsvcfuncs-0.1.3/adpipsvcfuncs/adpipsvcfuncs.py` & `adpipsvcfuncs-0.1.4/adpipsvcfuncs/adpipsvcfuncs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 import json
-from google.cloud import pubsub_v1
+from google.cloud import pubsub_v1, secretmanager
 import requests
 import logging
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)  # Capture DEBUG, INFO, WARNING, ERROR, CRITICAL
 
+def fetch_gcp_secret(secret_name: str) -> str:
+    # Fetch Project ID from Metadata Server
+    metadata_server_url = "http://metadata/computeMetadata/v1/project/project-id"
+    headers = {"Metadata-Flavor": "Google"}
+    project_id = requests.get(metadata_server_url, headers=headers).text
+    
+    # Create the Secret Manager client.
+    client = secretmanager.SecretManagerServiceClient()
+
+    # Build the resource name of the secret.
+    secret_version = 'latest'
+    name = f"projects/{project_id}/secrets/{secret_name}/versions/{secret_version}"
+
+    # Access the secret version.
+    response = client.access_secret_version(request={"name": name})
+    secret_string = response.payload.data.decode("UTF-8")
+    return secret_string
+
 def publish_to_pubsub(topic_name : str, data : dict) -> bool:
     """Publishes a message to a Google Cloud Pub/Sub topic."""
     # Fetch Project ID from Metadata Server
     metadata_server_url = "http://metadata/computeMetadata/v1/project/project-id"
     headers = {"Metadata-Flavor": "Google"}
     project_id = requests.get(metadata_server_url, headers=headers).text
     # Publish the message to Pub/Sub
```

