# Comparing `tmp/aws-cdk.cx-api-2.99.0.tar.gz` & `tmp/aws-cdk.cx-api-2.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src805316929/src/packages/@aws-cdk/cx-api/dist/python/aws-cdk.cx-api-2.99.0.tar", last modified: Wed Sep 27 19:39:09 2023, max compression
+gzip compressed data, was "/codebuild/output/src2270552867/src/packages/@aws-cdk/cx-api/dist/python/aws-cdk.cx-api-2.99.1.tar", last modified: Sat Sep 30 10:08:17 2023, max compression
```

## Comparing `aws-cdk.cx-api-2.99.0.tar` & `aws-cdk.cx-api-2.99.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-09-27 19:38:56.000000 aws-cdk.cx-api-2.99.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-09-27 19:38:56.000000 aws-cdk.cx-api-2.99.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2718 2023-09-27 19:38:56.000000 aws-cdk.cx-api-2.99.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8924 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7940 2023-09-27 19:38:56.000000 aws-cdk.cx-api-2.99.0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-09-27 19:38:56.000000 aws-cdk.cx-api-2.99.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1768 2023-09-27 19:38:56.000000 aws-cdk.cx-api-2.99.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk/cx_api/
--rw-r--r--   0 root         (0) root         (0)   175135 2023-09-27 19:38:56.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk/cx_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk/cx_api/_jsii/
--rw-r--r--   0 root         (0) root         (0)      388 2023-09-27 19:38:56.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk/cx_api/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   208927 2023-09-27 19:38:56.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk/cx_api/_jsii/cx-api@2.99.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:56.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk/cx_api/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk.cx_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8924 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk.cx_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk.cx_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk.cx_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk.cx_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-09-27 19:39:09.000000 aws-cdk.cx-api-2.99.0/src/aws_cdk.cx_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-09-30 10:08:05.000000 aws-cdk.cx-api-2.99.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-09-30 10:08:05.000000 aws-cdk.cx-api-2.99.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-09-30 10:08:05.000000 aws-cdk.cx-api-2.99.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8924 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7940 2023-09-30 10:08:05.000000 aws-cdk.cx-api-2.99.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-09-30 10:08:05.000000 aws-cdk.cx-api-2.99.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-09-30 10:08:05.000000 aws-cdk.cx-api-2.99.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk/cx_api/
+-rw-r--r--   0 root         (0) root         (0)   175135 2023-09-30 10:08:05.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk/cx_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk/cx_api/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      388 2023-09-30 10:08:05.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk/cx_api/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   208926 2023-09-30 10:08:05.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk/cx_api/_jsii/cx-api@2.99.1.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:08:05.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk/cx_api/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk.cx_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8924 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk.cx_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      413 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk.cx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk.cx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk.cx_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-09-30 10:08:17.000000 aws-cdk.cx-api-2.99.1/src/aws_cdk.cx_api.egg-info/top_level.txt
```

### Comparing `aws-cdk.cx-api-2.99.0/LICENSE` & `aws-cdk.cx-api-2.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cx-api-2.99.0/NOTICE` & `aws-cdk.cx-api-2.99.1/NOTICE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cx-api-2.99.0/PKG-INFO` & `aws-cdk.cx-api-2.99.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cx-api
-Version: 2.99.0
+Version: 2.99.1
 Summary: Cloud executable protocol
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.cx-api-2.99.0/README.md` & `aws-cdk.cx-api-2.99.1/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.cx-api-2.99.0/setup.py` & `aws-cdk.cx-api-2.99.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cx-api",
-    "version": "2.99.0",
+    "version": "2.99.1",
     "description": "Cloud executable protocol",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.cx_api",
         "aws_cdk.cx_api._jsii"
     ],
     "package_data": {
         "aws_cdk.cx_api._jsii": [
-            "cx-api@2.99.0.jsii.tgz"
+            "cx-api@2.99.1.jsii.tgz"
         ],
         "aws_cdk.cx_api": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk.cloud-assembly-schema==2.99.0",
+        "aws-cdk.cloud-assembly-schema==2.99.1",
         "jsii>=1.88.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `aws-cdk.cx-api-2.99.0/src/aws_cdk/cx_api/__init__.py` & `aws-cdk.cx-api-2.99.1/src/aws_cdk/cx_api/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.cx-api-2.99.0/src/aws_cdk.cx_api.egg-info/PKG-INFO` & `aws-cdk.cx-api-2.99.1/src/aws_cdk.cx_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cx-api
-Version: 2.99.0
+Version: 2.99.1
 Summary: Cloud executable protocol
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

