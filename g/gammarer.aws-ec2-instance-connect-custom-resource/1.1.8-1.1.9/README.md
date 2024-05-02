# Comparing `tmp/gammarer.aws-ec2-instance-connect-custom-resource-1.1.8.tar.gz` & `tmp/gammarer.aws-ec2-instance-connect-custom-resource-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ec2-instance-connect-custom-resource-1.1.8.tar", last modified: Thu Nov  9 16:20:39 2023, max compression
+gzip compressed data, was "gammarer.aws-ec2-instance-connect-custom-resource-1.1.9.tar", last modified: Thu Nov 23 16:17:52 2023, max compression
```

## Comparing `gammarer.aws-ec2-instance-connect-custom-resource-1.1.8.tar` & `gammarer.aws-ec2-instance-connect-custom-resource-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 16:20:39.239339 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-11-09 16:20:27.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-09 16:20:27.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-11-09 16:20:39.239339 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-11-09 16:20:27.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-11-09 16:20:27.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-09 16:20:39.239339 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2023-11-09 16:20:27.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 16:20:39.235339 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 16:20:39.235339 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 16:20:39.239339 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer/aws_ec2_instance_connect_custom_resource/
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2023-11-09 16:20:27.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 16:20:39.239339 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-09 16:20:27.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18114 2023-11-09 16:20:27.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@1.1.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 16:20:27.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer/aws_ec2_instance_connect_custom_resource/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 16:20:39.239339 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-11-09 16:20:39.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-11-09 16:20:39.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 16:20:39.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-11-09 16:20:39.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-09 16:20:39.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 16:17:52.342213 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-11-23 16:17:41.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-23 16:17:41.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2023-11-23 16:17:52.342213 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-11-23 16:17:41.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-11-23 16:17:41.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-23 16:17:52.342213 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2023-11-23 16:17:41.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 16:17:52.338213 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 16:17:52.338213 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 16:17:52.342213 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer/aws_ec2_instance_connect_custom_resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     6865 2023-11-23 16:17:41.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 16:17:52.342213 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-23 16:17:41.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18099 2023-11-23 16:17:41.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@1.1.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 16:17:41.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer/aws_ec2_instance_connect_custom_resource/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 16:17:52.338213 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2023-11-23 16:17:52.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2023-11-23 16:17:52.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 16:17:52.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-11-23 16:17:52.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-23 16:17:52.000000 gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/LICENSE` & `gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/PKG-INFO` & `gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-connect-custom-resource
-Version: 1.1.8
+Version: 1.1.9
 Summary: AWS EC2 instance connect custom resource
 Home-page: https://github.com/gammarer/aws-ec2-instance-connect-custom-resource.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-ec2-instance-connect-custom-resource.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![GitHub](https://img.shields.io/github/license/yicr/aws-ec2-instance-connect-custom-resource?style=flat-square)](https://github.com/yicr/aws-ec2-instance-connect-custom-resource/blob/main/LICENSE)
 [![npm (scoped)](https://img.shields.io/npm/v/@gammarer/aws-ec2-instance-connect-custom-resource?style=flat-square)](https://www.npmjs.com/package/@gammarer/aws-ec2-instance-connect-custom-resource)
 [![PyPI](https://img.shields.io/pypi/v/gammarer.aws-ec2-instance-connect-custom-resource?style=flat-square)](https://pypi.org/project/gammarer.aws-ec2-instance-connect-custom-resource/)
 [![Nuget](https://img.shields.io/nuget/v/Gammarer.CDK.AWS.Ec2InstanceConnectCustomResource?style=flat-square)](https://www.nuget.org/packages/Gammarer.CDK.AWS.Ec2InstanceConnectCustomResource/)
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/README.md` & `gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/setup.py` & `gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ec2-instance-connect-custom-resource",
-    "version": "1.1.8",
+    "version": "1.1.9",
     "description": "AWS EC2 instance connect custom resource",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-ec2-instance-connect-custom-resource.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,34 +22,33 @@
     },
     "packages": [
         "gammarer.aws_ec2_instance_connect_custom_resource",
         "gammarer.aws_ec2_instance_connect_custom_resource._jsii"
     ],
     "package_data": {
         "gammarer.aws_ec2_instance_connect_custom_resource._jsii": [
-            "aws-ec2-instance-connect-custom-resource@1.1.8.jsii.tgz"
+            "aws-ec2-instance-connect-custom-resource@1.1.9.jsii.tgz"
         ],
         "gammarer.aws_ec2_instance_connect_custom_resource": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.91.0, <2.0.0",
+        "jsii>=1.92.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py` & `gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO` & `gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-connect-custom-resource
-Version: 1.1.8
+Version: 1.1.9
 Summary: AWS EC2 instance connect custom resource
 Home-page: https://github.com/gammarer/aws-ec2-instance-connect-custom-resource.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-ec2-instance-connect-custom-resource.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![GitHub](https://img.shields.io/github/license/yicr/aws-ec2-instance-connect-custom-resource?style=flat-square)](https://github.com/yicr/aws-ec2-instance-connect-custom-resource/blob/main/LICENSE)
 [![npm (scoped)](https://img.shields.io/npm/v/@gammarer/aws-ec2-instance-connect-custom-resource?style=flat-square)](https://www.npmjs.com/package/@gammarer/aws-ec2-instance-connect-custom-resource)
 [![PyPI](https://img.shields.io/pypi/v/gammarer.aws-ec2-instance-connect-custom-resource?style=flat-square)](https://pypi.org/project/gammarer.aws-ec2-instance-connect-custom-resource/)
 [![Nuget](https://img.shields.io/nuget/v/Gammarer.CDK.AWS.Ec2InstanceConnectCustomResource?style=flat-square)](https://www.nuget.org/packages/Gammarer.CDK.AWS.Ec2InstanceConnectCustomResource/)
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-1.1.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt` & `gammarer.aws-ec2-instance-connect-custom-resource-1.1.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/dependency_links.txt
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/requires.txt
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/top_level.txt
 src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py
 src/gammarer/aws_ec2_instance_connect_custom_resource/py.typed
 src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/__init__.py
-src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@1.1.8.jsii.tgz
+src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@1.1.9.jsii.tgz
```

