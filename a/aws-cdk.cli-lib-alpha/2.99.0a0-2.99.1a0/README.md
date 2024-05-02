# Comparing `tmp/aws-cdk.cli-lib-alpha-2.99.0a0.tar.gz` & `tmp/aws-cdk.cli-lib-alpha-2.99.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src805316929/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.99.0a0.tar", last modified: Wed Sep 27 19:38:50 2023, max compression
+gzip compressed data, was "/codebuild/output/src2270552867/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.99.1a0.tar", last modified: Sat Sep 30 10:08:00 2023, max compression
```

## Comparing `aws-cdk.cli-lib-alpha-2.99.0a0.tar` & `aws-cdk.cli-lib-alpha-2.99.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-09-27 19:38:36.000000 aws-cdk.cli-lib-alpha-2.99.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-09-27 19:38:39.000000 aws-cdk.cli-lib-alpha-2.99.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      726 2023-09-27 19:38:38.000000 aws-cdk.cli-lib-alpha-2.99.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4306 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3319 2023-09-27 19:38:39.000000 aws-cdk.cli-lib-alpha-2.99.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-09-27 19:38:39.000000 aws-cdk.cli-lib-alpha-2.99.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1766 2023-09-27 19:38:39.000000 aws-cdk.cli-lib-alpha-2.99.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk/cli_lib_alpha/
--rw-r--r--   0 root         (0) root         (0)   258198 2023-09-27 19:38:39.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk/cli_lib_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk/cli_lib_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      387 2023-09-27 19:38:39.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)  4476563 2023-09-27 19:38:36.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.99.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:39.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk/cli_lib_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk.cli_lib_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4306 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-09-27 19:38:50.000000 aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-09-30 10:07:49.000000 aws-cdk.cli-lib-alpha-2.99.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-09-30 10:07:52.000000 aws-cdk.cli-lib-alpha-2.99.1a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      726 2023-09-30 10:07:50.000000 aws-cdk.cli-lib-alpha-2.99.1a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4306 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-09-30 10:07:52.000000 aws-cdk.cli-lib-alpha-2.99.1a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-09-30 10:07:52.000000 aws-cdk.cli-lib-alpha-2.99.1a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-09-30 10:07:52.000000 aws-cdk.cli-lib-alpha-2.99.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk/cli_lib_alpha/
+-rw-r--r--   0 root         (0) root         (0)   258198 2023-09-30 10:07:52.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk/cli_lib_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk/cli_lib_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-09-30 10:07:52.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  4476561 2023-09-30 10:07:49.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.99.1-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:07:52.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk/cli_lib_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk.cli_lib_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4306 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-09-30 10:08:00.000000 aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.cli-lib-alpha-2.99.0a0/LICENSE` & `aws-cdk.cli-lib-alpha-2.99.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.99.0a0/NOTICE` & `aws-cdk.cli-lib-alpha-2.99.1a0/NOTICE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.99.0a0/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.99.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.cli-lib-alpha-2.99.0a0/README.md` & `aws-cdk.cli-lib-alpha-2.99.1a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.99.0a0/setup.py` & `aws-cdk.cli-lib-alpha-2.99.1a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cli-lib-alpha",
-    "version": "2.99.0.a0",
+    "version": "2.99.1.a0",
     "description": "AWS CDK Programmatic CLI library",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_cdk.cli_lib_alpha",
         "aws_cdk.cli_lib_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.cli_lib_alpha._jsii": [
-            "cli-lib-alpha@2.99.0-alpha.0.jsii.tgz"
+            "cli-lib-alpha@2.99.1-alpha.0.jsii.tgz"
         ],
         "aws_cdk.cli_lib_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk/cli_lib_alpha/__init__.py` & `aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk/cli_lib_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.99.0-alpha.0.jsii.tgz` & `aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.99.1-alpha.0.jsii.tgz`

 * *Files 15% similar despite different names*

#### Comparing `cli-lib-alpha@2.99.0-alpha.0.jsii.tgz-content` & `cli-lib-alpha@2.99.1-alpha.0.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'2.99.1-alpha.0'"}*

```diff
@@ -1902,9 +1902,9 @@
                         "primitive": "boolean"
                     }
                 }
             ],
             "symbolId": "lib/commands/synth:SynthOptions"
         }
     },
-    "version": "2.99.0-alpha.0"
+    "version": "2.99.1-alpha.0"
 }
```

##### package/lib/main.js

###### js-beautify {}

```diff
@@ -1089632,15 +1089632,15 @@
     }
 });
 var require_package2 = __commonJS({
     "../../aws-cdk/package.json"(exports, module2) {
         module2.exports = {
             name: "aws-cdk",
             description: "CDK Toolkit, the command line tool for CDK apps",
-            version: "2.99.0",
+            version: "2.99.1",
             bin: {
                 cdk: "bin/cdk"
             },
             scripts: {
                 build: "cdk-build",
                 watch: "cdk-watch",
                 lint: "cdk-lint",
@@ -1089680,31 +1089680,31 @@
             author: {
                 name: "Amazon Web Services",
                 url: "https://aws.amazon.com",
                 organization: true
             },
             license: "Apache-2.0",
             devDependencies: {
-                "@aws-cdk/cdk-build-tools": "2.99.0-alpha.0",
-                "@aws-cdk/pkglint": "2.99.0-alpha.0",
+                "@aws-cdk/cdk-build-tools": "2.99.1-alpha.0",
+                "@aws-cdk/pkglint": "2.99.1-alpha.0",
                 "@octokit/rest": "^18.12.0",
                 "@types/archiver": "^5.3.2",
                 "@types/fs-extra": "^9.0.13",
                 "@types/glob": "^7.2.0",
                 "@types/jest": "^29.5.5",
                 "@types/mockery": "^1.4.30",
                 "@types/promptly": "^3.0.2",
                 "@types/semver": "^7.5.2",
                 "@types/sinon": "^9.0.11",
                 "@types/source-map-support": "^0.5.7",
                 "@types/table": "^6.0.0",
                 "@types/uuid": "^8.3.4",
                 "@types/wrap-ansi": "^3.0.0",
                 "@types/yargs": "^15.0.15",
-                "aws-cdk-lib": "2.99.0",
+                "aws-cdk-lib": "2.99.1",
                 "aws-sdk-mock": "5.6.0",
                 axios: "^0.27.2",
                 "cdk-from-cfn": "^0.17.0",
                 constructs: "^10.0.0",
                 "fast-check": "^3.13.0",
                 jest: "^29.7.0",
                 "jest-mock": "^29.7.0",
@@ -1089713,23 +1089713,23 @@
                 nock: "^13.3.3",
                 sinon: "^9.2.4",
                 "ts-jest": "^29.1.1",
                 "ts-mock-imports": "^1.3.8",
                 "xml-js": "^1.6.11"
             },
             dependencies: {
-                "@aws-cdk/cloud-assembly-schema": "2.99.0",
-                "@aws-cdk/cloudformation-diff": "2.99.0",
-                "@aws-cdk/cx-api": "2.99.0",
-                "@aws-cdk/region-info": "2.99.0",
+                "@aws-cdk/cloud-assembly-schema": "2.99.1",
+                "@aws-cdk/cloudformation-diff": "2.99.1",
+                "@aws-cdk/cx-api": "2.99.1",
+                "@aws-cdk/region-info": "2.99.1",
                 "@jsii/check-node": "1.88.0",
                 archiver: "^5.3.2",
                 "aws-sdk": "^2.1461.0",
                 camelcase: "^6.3.0",
-                "cdk-assets": "2.99.0",
+                "cdk-assets": "2.99.1",
                 "cdk-from-cfn": "^0.17.0",
                 chalk: "^4",
                 chokidar: "^3.5.3",
                 decamelize: "^5.0.1",
                 "fs-extra": "^9.1.0",
                 glob: "^7.2.3",
                 "json-diff": "^0.10.0",
```

##### package/build-info.json

###### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'comment'": "'Generated at 2023-09-30T09:35:04Z by generate.sh'", "'commit'": "'b2a895e'"}*

```diff
@@ -1,4 +1,4 @@
 {
-    "comment": "Generated at 2023-09-27T19:01:43Z by generate.sh",
-    "commit": "0aa1096"
+    "comment": "Generated at 2023-09-30T09:35:04Z by generate.sh",
+    "commit": "b2a895e"
 }
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'devDependencies'": "{'@aws-cdk/cdk-build-tools': '2.99.1-alpha.0', 'aws-cdk-lib': '2.99.1', "*

 * *                      "'@aws-cdk/pkglint': '2.99.1-alpha.0', 'aws-cdk': '2.99.1'}",*

 * * "'version'": "'2.99.1-alpha.0'"}*

```diff
@@ -18,19 +18,19 @@
             "yarn bundle",
             "node ./lib/main.js >/dev/null 2>/dev/null </dev/null"
         ]
     },
     "dependencies": {},
     "description": "AWS CDK Programmatic CLI library",
     "devDependencies": {
-        "@aws-cdk/cdk-build-tools": "2.99.0-alpha.0",
-        "@aws-cdk/pkglint": "2.99.0-alpha.0",
+        "@aws-cdk/cdk-build-tools": "2.99.1-alpha.0",
+        "@aws-cdk/pkglint": "2.99.1-alpha.0",
         "@types/jest": "^29.5.5",
-        "aws-cdk": "2.99.0",
-        "aws-cdk-lib": "2.99.0",
+        "aws-cdk": "2.99.1",
+        "aws-cdk-lib": "2.99.1",
         "constructs": "^10.0.0",
         "jest": "^29.7.0",
         "ts-node": "^10.9.1"
     },
     "engines": {
         "node": ">= 14.15.0"
     },
@@ -116,9 +116,9 @@
     },
     "separate-module": true,
     "stability": "experimental",
     "types": "lib/index.d.ts",
     "ubergen": {
         "exclude": true
     },
-    "version": "2.99.0-alpha.0"
+    "version": "2.99.1-alpha.0"
 }
```

### Comparing `aws-cdk.cli-lib-alpha-2.99.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.99.1a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

