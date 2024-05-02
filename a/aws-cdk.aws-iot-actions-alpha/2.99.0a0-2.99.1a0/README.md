# Comparing `tmp/aws-cdk.aws-iot-actions-alpha-2.99.0a0.tar.gz` & `tmp/aws-cdk.aws-iot-actions-alpha-2.99.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src805316929/src/packages/@aws-cdk/aws-iot-actions-alpha/dist/python/aws-cdk.aws-iot-actions-alpha-2.99.0a0.t", last modified: Wed Sep 27 19:39:26 2023, max compression
+gzip compressed data, was "/codebuild/output/src2270552867/src/packages/@aws-cdk/aws-iot-actions-alpha/dist/python/aws-cdk.aws-iot-actions-alpha-2.99.1a0.", last modified: Sat Sep 30 10:08:33 2023, max compression
```

## Comparing `aws-cdk.aws-iot-actions-alpha-2.99.0a0.tar` & `aws-cdk.aws-iot-actions-alpha-2.99.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-09-27 19:39:19.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-09-27 19:39:19.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1382 2023-09-27 19:39:19.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12017 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11022 2023-09-27 19:39:19.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-09-27 19:39:19.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2103 2023-09-27 19:39:19.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk/aws_iot_actions_alpha/
--rw-r--r--   0 root         (0) root         (0)   115283 2023-09-27 19:39:19.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk/aws_iot_actions_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      632 2023-09-27 19:39:19.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80922 2023-09-27 19:39:19.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/aws-iot-actions-alpha@2.99.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:39:19.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk/aws_iot_actions_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12017 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      571 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      279 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-09-27 19:39:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-09-30 10:08:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-09-30 10:08:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-09-30 10:08:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12017 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11022 2023-09-30 10:08:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-09-30 10:08:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-09-30 10:08:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk/aws_iot_actions_alpha/
+-rw-r--r--   0 root         (0) root         (0)   115283 2023-09-30 10:08:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk/aws_iot_actions_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-09-30 10:08:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80922 2023-09-30 10:08:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/aws-iot-actions-alpha@2.99.1-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:08:26.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk/aws_iot_actions_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12017 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      571 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      279 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-09-30 10:08:33.000000 aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.99.0a0/LICENSE` & `aws-cdk.aws-iot-actions-alpha-2.99.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-iot-actions-alpha-2.99.0a0/NOTICE` & `aws-cdk.aws-iot-actions-alpha-2.99.1a0/NOTICE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-iot-actions-alpha-2.99.0a0/PKG-INFO` & `aws-cdk.aws-iot-actions-alpha-2.99.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-iot-actions-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: Receipt rule actions for AWS IoT
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.99.0a0/README.md` & `aws-cdk.aws-iot-actions-alpha-2.99.1a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-iot-actions-alpha-2.99.0a0/setup.py` & `aws-cdk.aws-iot-actions-alpha-2.99.1a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-iot-actions-alpha",
-    "version": "2.99.0.a0",
+    "version": "2.99.1.a0",
     "description": "Receipt rule actions for AWS IoT",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,27 +22,27 @@
     },
     "packages": [
         "aws_cdk.aws_iot_actions_alpha",
         "aws_cdk.aws_iot_actions_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_iot_actions_alpha._jsii": [
-            "aws-iot-actions-alpha@2.99.0-alpha.0.jsii.tgz"
+            "aws-iot-actions-alpha@2.99.1-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_iot_actions_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.99.0",
-        "aws-cdk.aws-iot-alpha==2.99.0.a0",
-        "aws-cdk.aws-iotevents-alpha==2.99.0.a0",
-        "aws-cdk.aws-kinesisfirehose-alpha==2.99.0.a0",
-        "aws-cdk.aws-kinesisfirehose-destinations-alpha==2.99.0.a0",
+        "aws-cdk-lib==2.99.1",
+        "aws-cdk.aws-iot-alpha==2.99.1.a0",
+        "aws-cdk.aws-iotevents-alpha==2.99.1.a0",
+        "aws-cdk.aws-kinesisfirehose-alpha==2.99.1.a0",
+        "aws-cdk.aws-kinesisfirehose-destinations-alpha==2.99.1.a0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.88.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk/aws_iot_actions_alpha/__init__.py` & `aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk/aws_iot_actions_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/__init__.py` & `aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk/aws_iot_actions_alpha/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 import aws_cdk.aws_iotevents_alpha._jsii
 import aws_cdk.aws_kinesisfirehose_alpha._jsii
 import aws_cdk.aws_kinesisfirehose_destinations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-cdk/aws-iot-actions-alpha",
-    "2.99.0-alpha.0",
+    "2.99.1-alpha.0",
     __name__[0:-6],
-    "aws-iot-actions-alpha@2.99.0-alpha.0.jsii.tgz",
+    "aws-iot-actions-alpha@2.99.1-alpha.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-iot-actions-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: Receipt rule actions for AWS IoT
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-iot-actions-alpha-2.99.0a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-iot-actions-alpha-2.99.1a0/src/aws_cdk.aws_iot_actions_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_iot_actions_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_iot_actions_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_iot_actions_alpha.egg-info/requires.txt
 src/aws_cdk.aws_iot_actions_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_iot_actions_alpha/__init__.py
 src/aws_cdk/aws_iot_actions_alpha/py.typed
 src/aws_cdk/aws_iot_actions_alpha/_jsii/__init__.py
-src/aws_cdk/aws_iot_actions_alpha/_jsii/aws-iot-actions-alpha@2.99.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_iot_actions_alpha/_jsii/aws-iot-actions-alpha@2.99.1-alpha.0.jsii.tgz
```

