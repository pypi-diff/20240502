# Comparing `tmp/aws-cdk.cloud-assembly-schema-2.99.0.tar.gz` & `tmp/aws-cdk.cloud-assembly-schema-2.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src805316929/src/packages/@aws-cdk/cloud-assembly-schema/dist/python/aws-cdk.cloud-assembly-schema-2.99.0.tar", last modified: Wed Sep 27 19:38:47 2023, max compression
+gzip compressed data, was "/codebuild/output/src2270552867/src/packages/@aws-cdk/cloud-assembly-schema/dist/python/aws-cdk.cloud-assembly-schema-2.99.1.ta", last modified: Sat Sep 30 10:07:58 2023, max compression
```

## Comparing `aws-cdk.cloud-assembly-schema-2.99.0.tar` & `aws-cdk.cloud-assembly-schema-2.99.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-09-27 19:38:36.000000 aws-cdk.cloud-assembly-schema-2.99.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-09-27 19:38:36.000000 aws-cdk.cloud-assembly-schema-2.99.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3872 2023-09-27 19:38:36.000000 aws-cdk.cloud-assembly-schema-2.99.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3777 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2782 2023-09-27 19:38:36.000000 aws-cdk.cloud-assembly-schema-2.99.0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-09-27 19:38:36.000000 aws-cdk.cloud-assembly-schema-2.99.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1805 2023-09-27 19:38:36.000000 aws-cdk.cloud-assembly-schema-2.99.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk/cloud_assembly_schema/
--rw-r--r--   0 root         (0) root         (0)   374155 2023-09-27 19:38:36.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk/cloud_assembly_schema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk/cloud_assembly_schema/_jsii/
--rw-r--r--   0 root         (0) root         (0)      387 2023-09-27 19:38:36.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk/cloud_assembly_schema/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   182804 2023-09-27 19:38:36.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk/cloud_assembly_schema/_jsii/cloud-assembly-schema@2.99.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:36.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk/cloud_assembly_schema/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk.cloud_assembly_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3777 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk.cloud_assembly_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      563 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk.cloud_assembly_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk.cloud_assembly_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk.cloud_assembly_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-09-27 19:38:47.000000 aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk.cloud_assembly_schema.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-09-30 10:07:49.000000 aws-cdk.cloud-assembly-schema-2.99.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-09-30 10:07:49.000000 aws-cdk.cloud-assembly-schema-2.99.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-09-30 10:07:49.000000 aws-cdk.cloud-assembly-schema-2.99.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3777 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-09-30 10:07:49.000000 aws-cdk.cloud-assembly-schema-2.99.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-09-30 10:07:49.000000 aws-cdk.cloud-assembly-schema-2.99.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-09-30 10:07:49.000000 aws-cdk.cloud-assembly-schema-2.99.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk/cloud_assembly_schema/
+-rw-r--r--   0 root         (0) root         (0)   374155 2023-09-30 10:07:49.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk/cloud_assembly_schema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk/cloud_assembly_schema/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-09-30 10:07:49.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk/cloud_assembly_schema/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   182806 2023-09-30 10:07:49.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk/cloud_assembly_schema/_jsii/cloud-assembly-schema@2.99.1.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:07:49.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk/cloud_assembly_schema/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk.cloud_assembly_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3777 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk.cloud_assembly_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      563 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk.cloud_assembly_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk.cloud_assembly_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk.cloud_assembly_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-09-30 10:07:58.000000 aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk.cloud_assembly_schema.egg-info/top_level.txt
```

### Comparing `aws-cdk.cloud-assembly-schema-2.99.0/LICENSE` & `aws-cdk.cloud-assembly-schema-2.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cloud-assembly-schema-2.99.0/NOTICE` & `aws-cdk.cloud-assembly-schema-2.99.1/NOTICE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cloud-assembly-schema-2.99.0/PKG-INFO` & `aws-cdk.cloud-assembly-schema-2.99.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cloud-assembly-schema
-Version: 2.99.0
+Version: 2.99.1
 Summary: Cloud Assembly Schema
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.cloud-assembly-schema-2.99.0/README.md` & `aws-cdk.cloud-assembly-schema-2.99.1/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.cloud-assembly-schema-2.99.0/setup.py` & `aws-cdk.cloud-assembly-schema-2.99.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cloud-assembly-schema",
-    "version": "2.99.0",
+    "version": "2.99.1",
     "description": "Cloud Assembly Schema",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_cdk.cloud_assembly_schema",
         "aws_cdk.cloud_assembly_schema._jsii"
     ],
     "package_data": {
         "aws_cdk.cloud_assembly_schema._jsii": [
-            "cloud-assembly-schema@2.99.0.jsii.tgz"
+            "cloud-assembly-schema@2.99.1.jsii.tgz"
         ],
         "aws_cdk.cloud_assembly_schema": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk/cloud_assembly_schema/__init__.py` & `aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk/cloud_assembly_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk/cloud_assembly_schema/_jsii/cloud-assembly-schema@2.99.0.jsii.tgz` & `aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk/cloud_assembly_schema/_jsii/cloud-assembly-schema@2.99.1.jsii.tgz`

 * *Files 15% similar despite different names*

#### Comparing `cloud-assembly-schema@2.99.0.jsii.tgz-content` & `cloud-assembly-schema@2.99.1.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'version'": "'2.99.1'"}*

```diff
@@ -5906,9 +5906,9 @@
                         "primitive": "string"
                     }
                 }
             ],
             "symbolId": "lib/cloud-assembly/context-queries:VpcContextQuery"
         }
     },
-    "version": "2.99.0"
+    "version": "2.99.1"
 }
```

##### package/lib/manifest.js

###### js-beautify {}

```diff
@@ -269,15 +269,15 @@
     }
     constructor() {}
 }
 exports.Manifest = Manifest;
 _a = JSII_RTTI_SYMBOL_1;
 Manifest[_a] = {
     fqn: "@aws-cdk/cloud-assembly-schema.Manifest",
-    version: "2.99.0"
+    version: "2.99.1"
 };
 
 function mapValues(xs, fn) {
     if (!xs) {
         return undefined;
     }
     const ret = {};
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9722222222222221%*

 * *Differences: {"'devDependencies'": "{'@aws-cdk/cdk-build-tools': '2.99.1-alpha.0', '@aws-cdk/pkglint': "*

 * *                      "'2.99.1-alpha.0', 'aws-cdk-lib': '2.99.1'}",*

 * * "'version'": "'2.99.1'"}*

```diff
@@ -13,20 +13,20 @@
     ],
     "dependencies": {
         "jsonschema": "^1.4.1",
         "semver": "^7.5.4"
     },
     "description": "Cloud Assembly Schema",
     "devDependencies": {
-        "@aws-cdk/cdk-build-tools": "2.99.0-alpha.0",
-        "@aws-cdk/pkglint": "2.99.0-alpha.0",
+        "@aws-cdk/cdk-build-tools": "2.99.1-alpha.0",
+        "@aws-cdk/pkglint": "2.99.1-alpha.0",
         "@types/jest": "^29.5.5",
         "@types/mock-fs": "^4.13.1",
         "@types/semver": "^7.5.2",
-        "aws-cdk-lib": "2.99.0",
+        "aws-cdk-lib": "2.99.1",
         "jest": "^29.7.0",
         "mock-fs": "^4.14.0",
         "typescript-json-schema": "^0.61.0"
     },
     "engines": {
         "node": ">= 14.15.0"
     },
@@ -114,9 +114,9 @@
         "pkglint": "pkglint -f",
         "rosetta:extract": "yarn --silent jsii-rosetta extract",
         "test": "cdk-test",
         "watch": "cdk-watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "2.99.0"
+    "version": "2.99.1"
 }
```

### Comparing `aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk.cloud_assembly_schema.egg-info/PKG-INFO` & `aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk.cloud_assembly_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cloud-assembly-schema
-Version: 2.99.0
+Version: 2.99.1
 Summary: Cloud Assembly Schema
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.cloud-assembly-schema-2.99.0/src/aws_cdk.cloud_assembly_schema.egg-info/SOURCES.txt` & `aws-cdk.cloud-assembly-schema-2.99.1/src/aws_cdk.cloud_assembly_schema.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.cloud_assembly_schema.egg-info/SOURCES.txt
 src/aws_cdk.cloud_assembly_schema.egg-info/dependency_links.txt
 src/aws_cdk.cloud_assembly_schema.egg-info/requires.txt
 src/aws_cdk.cloud_assembly_schema.egg-info/top_level.txt
 src/aws_cdk/cloud_assembly_schema/__init__.py
 src/aws_cdk/cloud_assembly_schema/py.typed
 src/aws_cdk/cloud_assembly_schema/_jsii/__init__.py
-src/aws_cdk/cloud_assembly_schema/_jsii/cloud-assembly-schema@2.99.0.jsii.tgz
+src/aws_cdk/cloud_assembly_schema/_jsii/cloud-assembly-schema@2.99.1.jsii.tgz
```

