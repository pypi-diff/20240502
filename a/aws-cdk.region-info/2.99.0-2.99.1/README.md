# Comparing `tmp/aws-cdk.region-info-2.99.0.tar.gz` & `tmp/aws-cdk.region-info-2.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src805316929/src/packages/@aws-cdk/region-info/dist/python/aws-cdk.region-info-2.99.0.tar", last modified: Wed Sep 27 19:38:48 2023, max compression
+gzip compressed data, was "/codebuild/output/src2270552867/src/packages/@aws-cdk/region-info/dist/python/aws-cdk.region-info-2.99.1.tar", last modified: Sat Sep 30 10:07:58 2023, max compression
```

## Comparing `aws-cdk.region-info-2.99.0.tar` & `aws-cdk.region-info-2.99.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-09-27 19:38:36.000000 aws-cdk.region-info-2.99.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-09-27 19:38:36.000000 aws-cdk.region-info-2.99.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-09-27 19:38:36.000000 aws-cdk.region-info-2.99.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3487 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2468 2023-09-27 19:38:36.000000 aws-cdk.region-info-2.99.0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-09-27 19:38:36.000000 aws-cdk.region-info-2.99.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1779 2023-09-27 19:38:36.000000 aws-cdk.region-info-2.99.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/src/aws_cdk/region_info/
--rw-r--r--   0 root         (0) root         (0)    36474 2023-09-27 19:38:36.000000 aws-cdk.region-info-2.99.0/src/aws_cdk/region_info/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/src/aws_cdk/region_info/_jsii/
--rw-r--r--   0 root         (0) root         (0)      354 2023-09-27 19:38:36.000000 aws-cdk.region-info-2.99.0/src/aws_cdk/region_info/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   196932 2023-09-27 19:38:36.000000 aws-cdk.region-info-2.99.0/src/aws_cdk/region_info/_jsii/region-info@2.99.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:36.000000 aws-cdk.region-info-2.99.0/src/aws_cdk/region_info/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/src/aws_cdk.region_info.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3487 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/src/aws_cdk.region_info.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      463 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/src/aws_cdk.region_info.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/src/aws_cdk.region_info.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/src/aws_cdk.region_info.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-09-27 19:38:48.000000 aws-cdk.region-info-2.99.0/src/aws_cdk.region_info.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-09-30 10:07:49.000000 aws-cdk.region-info-2.99.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-09-30 10:07:49.000000 aws-cdk.region-info-2.99.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-09-30 10:07:49.000000 aws-cdk.region-info-2.99.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3487 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-09-30 10:07:49.000000 aws-cdk.region-info-2.99.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-09-30 10:07:49.000000 aws-cdk.region-info-2.99.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-09-30 10:07:49.000000 aws-cdk.region-info-2.99.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/src/aws_cdk/region_info/
+-rw-r--r--   0 root         (0) root         (0)    36474 2023-09-30 10:07:49.000000 aws-cdk.region-info-2.99.1/src/aws_cdk/region_info/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/src/aws_cdk/region_info/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-09-30 10:07:49.000000 aws-cdk.region-info-2.99.1/src/aws_cdk/region_info/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   196932 2023-09-30 10:07:49.000000 aws-cdk.region-info-2.99.1/src/aws_cdk/region_info/_jsii/region-info@2.99.1.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:07:49.000000 aws-cdk.region-info-2.99.1/src/aws_cdk/region_info/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/src/aws_cdk.region_info.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3487 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/src/aws_cdk.region_info.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      463 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/src/aws_cdk.region_info.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/src/aws_cdk.region_info.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/src/aws_cdk.region_info.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-09-30 10:07:58.000000 aws-cdk.region-info-2.99.1/src/aws_cdk.region_info.egg-info/top_level.txt
```

### Comparing `aws-cdk.region-info-2.99.0/LICENSE` & `aws-cdk.region-info-2.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.region-info-2.99.0/PKG-INFO` & `aws-cdk.region-info-2.99.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.region-info
-Version: 2.99.0
+Version: 2.99.1
 Summary: AWS region information, such as service principal names
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.region-info-2.99.0/README.md` & `aws-cdk.region-info-2.99.1/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.region-info-2.99.0/setup.py` & `aws-cdk.region-info-2.99.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.region-info",
-    "version": "2.99.0",
+    "version": "2.99.1",
     "description": "AWS region information, such as service principal names",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_cdk.region_info",
         "aws_cdk.region_info._jsii"
     ],
     "package_data": {
         "aws_cdk.region_info._jsii": [
-            "region-info@2.99.0.jsii.tgz"
+            "region-info@2.99.1.jsii.tgz"
         ],
         "aws_cdk.region_info": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-cdk.region-info-2.99.0/src/aws_cdk/region_info/__init__.py` & `aws-cdk.region-info-2.99.1/src/aws_cdk/region_info/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.region-info-2.99.0/src/aws_cdk.region_info.egg-info/PKG-INFO` & `aws-cdk.region-info-2.99.1/src/aws_cdk.region_info.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.region-info
-Version: 2.99.0
+Version: 2.99.1
 Summary: AWS region information, such as service principal names
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

