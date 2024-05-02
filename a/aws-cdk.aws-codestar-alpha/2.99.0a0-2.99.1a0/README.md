# Comparing `tmp/aws-cdk.aws-codestar-alpha-2.99.0a0.tar.gz` & `tmp/aws-cdk.aws-codestar-alpha-2.99.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src805316929/src/packages/@aws-cdk/aws-codestar-alpha/dist/python/aws-cdk.aws-codestar-alpha-2.99.0a0.tar", last modified: Wed Sep 27 19:38:47 2023, max compression
+gzip compressed data, was "/codebuild/output/src2270552867/src/packages/@aws-cdk/aws-codestar-alpha/dist/python/aws-cdk.aws-codestar-alpha-2.99.1a0.tar", last modified: Sat Sep 30 10:07:56 2023, max compression
```

## Comparing `aws-cdk.aws-codestar-alpha-2.99.0a0.tar` & `aws-cdk.aws-codestar-alpha-2.99.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-09-27 19:38:36.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-09-27 19:38:36.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-09-27 19:38:36.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2488 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1485 2023-09-27 19:38:36.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-09-27 19:38:36.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1877 2023-09-27 19:38:36.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk/aws_codestar_alpha/
--rw-r--r--   0 root         (0) root         (0)    18998 2023-09-27 19:38:36.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk/aws_codestar_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk/aws_codestar_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      443 2023-09-27 19:38:36.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk/aws_codestar_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22776 2023-09-27 19:38:36.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk/aws_codestar_alpha/_jsii/aws-codestar-alpha@2.99.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:36.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk/aws_codestar_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2488 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-09-27 19:38:47.000000 aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-09-30 10:07:49.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-09-30 10:07:49.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-09-30 10:07:49.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-09-30 10:07:49.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-09-30 10:07:49.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-09-30 10:07:49.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk/aws_codestar_alpha/
+-rw-r--r--   0 root         (0) root         (0)    18998 2023-09-30 10:07:49.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk/aws_codestar_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk/aws_codestar_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-09-30 10:07:49.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk/aws_codestar_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22775 2023-09-30 10:07:49.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk/aws_codestar_alpha/_jsii/aws-codestar-alpha@2.99.1-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:07:49.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk/aws_codestar_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk.aws_codestar_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk.aws_codestar_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk.aws_codestar_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk.aws_codestar_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk.aws_codestar_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-09-30 10:07:56.000000 aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk.aws_codestar_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-codestar-alpha-2.99.0a0/LICENSE` & `aws-cdk.aws-codestar-alpha-2.99.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-codestar-alpha-2.99.0a0/PKG-INFO` & `aws-cdk.aws-codestar-alpha-2.99.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-codestar-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: The CDK Construct Library for AWS::CodeStar
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-codestar-alpha-2.99.0a0/README.md` & `aws-cdk.aws-codestar-alpha-2.99.1a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-codestar-alpha-2.99.0a0/setup.py` & `aws-cdk.aws-codestar-alpha-2.99.1a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-codestar-alpha",
-    "version": "2.99.0.a0",
+    "version": "2.99.1.a0",
     "description": "The CDK Construct Library for AWS::CodeStar",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.aws_codestar_alpha",
         "aws_cdk.aws_codestar_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_codestar_alpha._jsii": [
-            "aws-codestar-alpha@2.99.0-alpha.0.jsii.tgz"
+            "aws-codestar-alpha@2.99.1-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_codestar_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.99.0",
+        "aws-cdk-lib==2.99.1",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.88.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk/aws_codestar_alpha/__init__.py` & `aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk/aws_codestar_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk/aws_codestar_alpha/_jsii/aws-codestar-alpha@2.99.0-alpha.0.jsii.tgz` & `aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk/aws_codestar_alpha/_jsii/aws-codestar-alpha@2.99.1-alpha.0.jsii.tgz`

 * *Files 4% similar despite different names*

#### Comparing `aws-codestar-alpha@2.99.0-alpha.0.jsii.tgz-content` & `aws-codestar-alpha@2.99.1-alpha.0.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9652777777777778%*

 * *Differences: {"'dependencies'": "{'aws-cdk-lib': '2.99.1'}", "'version'": "'2.99.1-alpha.0'"}*

```diff
@@ -4,15 +4,15 @@
         "organization": true,
         "roles": [
             "author"
         ],
         "url": "https://aws.amazon.com"
     },
     "dependencies": {
-        "aws-cdk-lib": "2.99.0",
+        "aws-cdk-lib": "2.99.1",
         "constructs": "^10.0.0"
     },
     "dependencyClosure": {
         "@aws-cdk/asset-awscli-v1": {
             "targets": {
                 "dotnet": {
                     "namespace": "Amazon.CDK.Asset.AwsCliV1",
@@ -3962,9 +3962,9 @@
                     "name": "PUBLIC"
                 }
             ],
             "name": "RepositoryVisibility",
             "symbolId": "lib/github-repository:RepositoryVisibility"
         }
     },
-    "version": "2.99.0-alpha.0"
+    "version": "2.99.1-alpha.0"
 }
```

##### package/lib/github-repository.js

###### js-beautify {}

```diff
@@ -41,15 +41,15 @@
         this.repo = cdk.Fn.select(1, cdk.Fn.split('/', resource.ref));
     }
 }
 exports.GitHubRepository = GitHubRepository;
 _a = JSII_RTTI_SYMBOL_1;
 GitHubRepository[_a] = {
     fqn: "@aws-cdk/aws-codestar-alpha.GitHubRepository",
-    version: "2.99.0-alpha.0"
+    version: "2.99.1-alpha.0"
 };
 /**
  * Visibility of the GitHubRepository
  */
 var RepositoryVisibility;
 (function(RepositoryVisibility) {
     /**
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9655797101449276%*

 * *Differences: {"'devDependencies'": "{'@aws-cdk/cdk-build-tools': '2.99.1-alpha.0', '@aws-cdk/integ-runner': "*

 * *                      "'2.99.1-alpha.0', '@aws-cdk/pkglint': '2.99.1-alpha.0', 'aws-cdk-lib': "*

 * *                      "'2.99.1'}",*

 * * "'peerDependencies'": "{'aws-cdk-lib': '2.99.1'}",*

 * * "'version'": "'2.99.1-alpha.0'"}*

```diff
@@ -11,19 +11,19 @@
         "env": {
             "AWSLINT_BASE_CONSTRUCT": true
         }
     },
     "dependencies": {},
     "description": "The CDK Construct Library for AWS::CodeStar",
     "devDependencies": {
-        "@aws-cdk/cdk-build-tools": "2.99.0-alpha.0",
-        "@aws-cdk/integ-runner": "2.99.0-alpha.0",
-        "@aws-cdk/pkglint": "2.99.0-alpha.0",
+        "@aws-cdk/cdk-build-tools": "2.99.1-alpha.0",
+        "@aws-cdk/integ-runner": "2.99.1-alpha.0",
+        "@aws-cdk/pkglint": "2.99.1-alpha.0",
         "@types/jest": "^29.5.5",
-        "aws-cdk-lib": "2.99.0",
+        "aws-cdk-lib": "2.99.1",
         "constructs": "^10.0.0"
     },
     "engines": {
         "node": ">= 14.15.0"
     },
     "homepage": "https://github.com/aws/aws-cdk",
     "jsii": {
@@ -71,15 +71,15 @@
         "aws-codestar"
     ],
     "license": "Apache-2.0",
     "main": "lib/index.js",
     "maturity": "experimental",
     "name": "@aws-cdk/aws-codestar-alpha",
     "peerDependencies": {
-        "aws-cdk-lib": "2.99.0",
+        "aws-cdk-lib": "2.99.1",
         "constructs": "^10.0.0"
     },
     "pkglint": {
         "exclude": [
             "naming/package-matches-directory",
             "assert/assert-dependency"
         ]
@@ -107,9 +107,9 @@
         "pkglint": "pkglint -f",
         "rosetta:extract": "yarn --silent jsii-rosetta extract",
         "test": "cdk-test",
         "watch": "cdk-watch"
     },
     "stability": "experimental",
     "types": "lib/index.d.ts",
-    "version": "2.99.0-alpha.0"
+    "version": "2.99.1-alpha.0"
 }
```

### Comparing `aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk.aws_codestar_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-codestar-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: The CDK Construct Library for AWS::CodeStar
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-codestar-alpha-2.99.0a0/src/aws_cdk.aws_codestar_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-codestar-alpha-2.99.1a0/src/aws_cdk.aws_codestar_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_codestar_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_codestar_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_codestar_alpha.egg-info/requires.txt
 src/aws_cdk.aws_codestar_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_codestar_alpha/__init__.py
 src/aws_cdk/aws_codestar_alpha/py.typed
 src/aws_cdk/aws_codestar_alpha/_jsii/__init__.py
-src/aws_cdk/aws_codestar_alpha/_jsii/aws-codestar-alpha@2.99.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_codestar_alpha/_jsii/aws-codestar-alpha@2.99.1-alpha.0.jsii.tgz
```

