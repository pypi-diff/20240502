# Comparing `tmp/cloudcix-0.9.6.tar.gz` & `tmp/cloudcix-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudcix-0.9.6.tar", last modified: Mon May  8 12:12:42 2023, max compression
+gzip compressed data, was "dist/cloudcix-0.9.7.tar", last modified: Wed Jul  5 12:39:59 2023, max compression
```

## Comparing `cloudcix-0.9.6.tar` & `cloudcix-0.9.7.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 12:12:42.000000 cloudcix-0.9.6/
--rw-r--r--   0 root         (0) root         (0)     4262 2023-05-08 12:12:42.000000 cloudcix-0.9.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 12:12:42.000000 cloudcix-0.9.6/cloudcix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4262 2023-05-08 12:12:42.000000 cloudcix-0.9.6/cloudcix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      803 2023-05-08 12:12:42.000000 cloudcix-0.9.6/cloudcix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-05-08 12:12:42.000000 cloudcix-0.9.6/cloudcix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-08 12:12:42.000000 cloudcix-0.9.6/cloudcix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 12:12:42.000000 cloudcix-0.9.6/cloudcix.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 12:12:42.000000 cloudcix-0.9.6/cloudcix/
--rw-rw-rw-   0 root         (0) root         (0)     3632 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2815 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    14902 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 12:12:42.000000 cloudcix-0.9.6/cloudcix/api/
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     1260 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/repository.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/otp.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/training.py
--rw-rw-rw-   0 root         (0) root         (0)     3638 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/iaas.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/reporting.py
--rw-rw-rw-   0 root         (0) root         (0)     1394 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/contacts.py
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/documentation.py
--rw-rw-rw-   0 root         (0) root         (0)     7440 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/financial.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/scm.py
--rw-rw-rw-   0 root         (0) root         (0)      534 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/circuit.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/app_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/membership.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/asset.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/pat.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      817 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/vault.py
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/security.py
--rw-rw-rw-   0 root         (0) root         (0)     3288 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/api/support.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-08 12:12:41.000000 cloudcix-0.9.6/cloudcix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3299 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     3007 2023-05-05 10:55:09.000000 cloudcix-0.9.6/cloudcix/auth.py
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-05 10:55:09.000000 cloudcix-0.9.6/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-05-05 10:55:09.000000 cloudcix-0.9.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     2966 2023-05-05 10:55:09.000000 cloudcix-0.9.6/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-08 12:12:42.000000 cloudcix-0.9.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-05 10:55:09.000000 cloudcix-0.9.6/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-05-08 12:12:41.000000 cloudcix-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:39:59.000000 cloudcix-0.9.7/
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-05 12:39:59.000000 cloudcix-0.9.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4262 2023-07-05 12:39:59.000000 cloudcix-0.9.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-05 12:39:25.000000 cloudcix-0.9.7/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-07-05 12:39:25.000000 cloudcix-0.9.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     2966 2023-07-05 12:39:25.000000 cloudcix-0.9.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:39:59.000000 cloudcix-0.9.7/cloudcix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4262 2023-07-05 12:39:59.000000 cloudcix-0.9.7/cloudcix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 12:39:59.000000 cloudcix-0.9.7/cloudcix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-05 12:39:59.000000 cloudcix-0.9.7/cloudcix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-05 12:39:59.000000 cloudcix-0.9.7/cloudcix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      845 2023-07-05 12:39:59.000000 cloudcix-0.9.7/cloudcix.egg-info/SOURCES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:39:59.000000 cloudcix-0.9.7/cloudcix/
+-rw-rw-rw-   0 root         (0) root         (0)     3697 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     3632 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3007 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-05 12:39:57.000000 cloudcix-0.9.7/cloudcix/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3299 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)    14902 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3951 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/lock_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     2815 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:39:59.000000 cloudcix-0.9.7/cloudcix/api/
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/otp.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/training.py
+-rw-rw-rw-   0 root         (0) root         (0)      817 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/vault.py
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/documentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/security.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/app_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      534 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3638 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/iaas.py
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/contacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/reporting.py
+-rw-rw-rw-   0 root         (0) root         (0)     3288 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/membership.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/pat.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/scm.py
+-rw-rw-rw-   0 root         (0) root         (0)     7440 2023-07-05 12:39:25.000000 cloudcix-0.9.7/cloudcix/api/financial.py
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-05 12:39:25.000000 cloudcix-0.9.7/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-07-05 12:39:57.000000 cloudcix-0.9.7/setup.py
```

### Comparing `cloudcix-0.9.6/PKG-INFO` & `cloudcix-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudcix
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python3 bindings and utils for CloudCIX API.
 Home-page: https://python-cloudcix.readthedocs.io/en/latest/
 Author: CloudCIX
 Author-email: developers@cloudcix.com
 License: Apache 2.0
 Description: Overview
         ========
```

### Comparing `cloudcix-0.9.6/cloudcix.egg-info/PKG-INFO` & `cloudcix-0.9.7/cloudcix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudcix
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python3 bindings and utils for CloudCIX API.
 Home-page: https://python-cloudcix.readthedocs.io/en/latest/
 Author: CloudCIX
 Author-email: developers@cloudcix.com
 License: Apache 2.0
 Description: Overview
         ========
```

### Comparing `cloudcix-0.9.6/cloudcix.egg-info/SOURCES.txt` & `cloudcix-0.9.7/cloudcix.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 setup.cfg
 setup.py
 cloudcix/__init__.py
 cloudcix/auth.py
 cloudcix/client.py
 cloudcix/conf.py
 cloudcix/exceptions.py
+cloudcix/lock.py
+cloudcix/lock_backend.py
 cloudcix/utils.py
 cloudcix.egg-info/PKG-INFO
 cloudcix.egg-info/SOURCES.txt
 cloudcix.egg-info/dependency_links.txt
 cloudcix.egg-info/requires.txt
 cloudcix.egg-info/top_level.txt
 cloudcix/api/__init__.py
```

### Comparing `cloudcix-0.9.6/cloudcix/utils.py` & `cloudcix-0.9.7/cloudcix/utils.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/exceptions.py` & `cloudcix-0.9.7/cloudcix/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/client.py` & `cloudcix-0.9.7/cloudcix/client.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/scheduler.py` & `cloudcix-0.9.7/cloudcix/api/scheduler.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/repository.py` & `cloudcix-0.9.7/cloudcix/api/repository.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/otp.py` & `cloudcix-0.9.7/cloudcix/api/otp.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/iaas.py` & `cloudcix-0.9.7/cloudcix/api/iaas.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/reporting.py` & `cloudcix-0.9.7/cloudcix/api/reporting.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/contacts.py` & `cloudcix-0.9.7/cloudcix/api/contacts.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/financial.py` & `cloudcix-0.9.7/cloudcix/api/financial.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/scm.py` & `cloudcix-0.9.7/cloudcix/api/scm.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/circuit.py` & `cloudcix-0.9.7/cloudcix/api/circuit.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/app_manager.py` & `cloudcix-0.9.7/cloudcix/api/app_manager.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/membership.py` & `cloudcix-0.9.7/cloudcix/api/membership.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/asset.py` & `cloudcix-0.9.7/cloudcix/api/asset.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/__init__.py` & `cloudcix-0.9.7/cloudcix/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/vault.py` & `cloudcix-0.9.7/cloudcix/api/vault.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/security.py` & `cloudcix-0.9.7/cloudcix/api/security.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/api/support.py` & `cloudcix-0.9.7/cloudcix/api/support.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/conf.py` & `cloudcix-0.9.7/cloudcix/conf.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/cloudcix/auth.py` & `cloudcix-0.9.7/cloudcix/auth.py`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/LICENSE` & `cloudcix-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/README.rst` & `cloudcix-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `cloudcix-0.9.6/setup.py` & `cloudcix-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open('requirements.txt', 'r') as f:
     requires = f.read().split('\n')
 
 setup(
     name='cloudcix',
-    version='0.9.6',
+    version='0.9.7',
     description='Python3 bindings and utils for CloudCIX API.',
     long_description=readme,
     author='CloudCIX',
     author_email='developers@cloudcix.com',
     url='https://python-cloudcix.readthedocs.io/en/latest/',
     packages=[
         'cloudcix',
```

