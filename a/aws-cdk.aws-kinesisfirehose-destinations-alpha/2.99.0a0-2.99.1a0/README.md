# Comparing `tmp/aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0.tar.gz` & `tmp/aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src805316929/src/packages/@aws-cdk/aws-kinesisfirehose-destinations-alpha/dist/python/aws-cdk.aws-kinesisfire", last modified: Wed Sep 27 19:39:07 2023, max compression
+gzip compressed data, was "/codebuild/output/src2270552867/src/packages/@aws-cdk/aws-kinesisfirehose-destinations-alpha/dist/python/aws-cdk.aws-kinesisfir", last modified: Sat Sep 30 10:08:18 2023, max compression
```

## Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0.tar` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-09-27 19:38:56.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-09-27 19:38:56.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-09-27 19:38:56.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2185 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1153 2023-09-27 19:38:56.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-09-27 19:38:56.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2062 2023-09-27 19:38:56.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/
--rw-r--r--   0 root         (0) root         (0)    60965 2023-09-27 19:38:56.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      530 2023-09-27 19:38:56.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39901 2023-09-27 19:38:56.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/aws-kinesisfirehose-destinations-alpha@2.99.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:56.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2185 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      741 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-09-27 19:39:07.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-09-30 10:08:05.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-09-30 10:08:05.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-09-30 10:08:05.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2185 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-09-30 10:08:05.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-09-30 10:08:05.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-09-30 10:08:05.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/
+-rw-r--r--   0 root         (0) root         (0)    60965 2023-09-30 10:08:05.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      530 2023-09-30 10:08:05.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39900 2023-09-30 10:08:05.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/aws-kinesisfirehose-destinations-alpha@2.99.1-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:08:05.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2185 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      741 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-09-30 10:08:18.000000 aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/LICENSE` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/PKG-INFO` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-kinesisfirehose-destinations-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: CDK Destinations Constructs for AWS Kinesis Firehose
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/README.md` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/setup.py` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-kinesisfirehose-destinations-alpha",
-    "version": "2.99.0.a0",
+    "version": "2.99.1.a0",
     "description": "CDK Destinations Constructs for AWS Kinesis Firehose",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "aws_cdk.aws_kinesisfirehose_destinations_alpha",
         "aws_cdk.aws_kinesisfirehose_destinations_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_kinesisfirehose_destinations_alpha._jsii": [
-            "aws-kinesisfirehose-destinations-alpha@2.99.0-alpha.0.jsii.tgz"
+            "aws-kinesisfirehose-destinations-alpha@2.99.1-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_kinesisfirehose_destinations_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.99.0",
-        "aws-cdk.aws-kinesisfirehose-alpha==2.99.0.a0",
+        "aws-cdk-lib==2.99.1",
+        "aws-cdk.aws-kinesisfirehose-alpha==2.99.1.a0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.88.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/__init__.py` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/__init__.py` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 import aws_cdk._jsii
 import aws_cdk.aws_kinesisfirehose_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@aws-cdk/aws-kinesisfirehose-destinations-alpha",
-    "2.99.0-alpha.0",
+    "2.99.1-alpha.0",
     __name__[0:-6],
-    "aws-kinesisfirehose-destinations-alpha@2.99.0-alpha.0.jsii.tgz",
+    "aws-kinesisfirehose-destinations-alpha@2.99.1-alpha.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/aws-kinesisfirehose-destinations-alpha@2.99.0-alpha.0.jsii.tgz` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/aws-kinesisfirehose-destinations-alpha@2.99.1-alpha.0.jsii.tgz`

 * *Files 25% similar despite different names*

#### Comparing `aws-kinesisfirehose-destinations-alpha@2.99.0-alpha.0.jsii.tgz-content` & `aws-kinesisfirehose-destinations-alpha@2.99.1-alpha.0.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9629629629629629%*

 * *Differences: {"'dependencies'": "{'@aws-cdk/aws-kinesisfirehose-alpha': '2.99.1-alpha.0', 'aws-cdk-lib': "*

 * *                   "'2.99.1'}",*

 * * "'version'": "'2.99.1-alpha.0'"}*

```diff
@@ -4,16 +4,16 @@
         "organization": true,
         "roles": [
             "author"
         ],
         "url": "https://aws.amazon.com"
     },
     "dependencies": {
-        "@aws-cdk/aws-kinesisfirehose-alpha": "2.99.0-alpha.0",
-        "aws-cdk-lib": "2.99.0",
+        "@aws-cdk/aws-kinesisfirehose-alpha": "2.99.1-alpha.0",
+        "aws-cdk-lib": "2.99.1",
         "constructs": "^10.0.0"
     },
     "dependencyClosure": {
         "@aws-cdk/asset-awscli-v1": {
             "targets": {
                 "dotnet": {
                     "namespace": "Amazon.CDK.Asset.AwsCliV1",
@@ -4267,9 +4267,9 @@
                 "filename": "lib/s3-bucket.ts",
                 "line": 11
             },
             "name": "S3BucketProps",
             "symbolId": "lib/s3-bucket:S3BucketProps"
         }
     },
-    "version": "2.99.0-alpha.0"
+    "version": "2.99.1-alpha.0"
 }
```

##### package/lib/common.js

###### js-beautify {}

```diff
@@ -22,15 +22,15 @@
         this.value = value;
     }
 }
 exports.Compression = Compression;
 _a = JSII_RTTI_SYMBOL_1;
 Compression[_a] = {
     fqn: "@aws-cdk/aws-kinesisfirehose-destinations-alpha.Compression",
-    version: "2.99.0-alpha.0"
+    version: "2.99.1-alpha.0"
 };
 /**
  * gzip
  */
 Compression.GZIP = new Compression('GZIP');
 /**
  * Hadoop-compatible Snappy
```

##### package/lib/s3-bucket.js

###### js-beautify {}

```diff
@@ -69,10 +69,10 @@
             undefined;
     }
 }
 exports.S3Bucket = S3Bucket;
 _a = JSII_RTTI_SYMBOL_1;
 S3Bucket[_a] = {
     fqn: "@aws-cdk/aws-kinesisfirehose-destinations-alpha.S3Bucket",
-    version: "2.99.0-alpha.0"
+    version: "2.99.1-alpha.0"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiczMtYnVja2V0LmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiczMtYnVja2V0LnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7Ozs7OztBQUFBLDJDQUEyQztBQUkzQyxxQ0FBd0Y7QUFDeEYsK0NBQW1KO0FBUW5KOztHQUVHO0FBQ0gsTUFBYSxRQUFRO0lBQ25CLFlBQTZCLE1BQWtCLEVBQW1CLFFBQXVCLEVBQUU7UUFBOUQsV0FBTSxHQUFOLE1BQU0sQ0FBWTtRQUFtQixVQUFLLEdBQUwsS0FBSyxDQUFvQjs7Ozs7OytDQURoRixRQUFROzs7O1FBRWpCLElBQUksSUFBSSxDQUFDLEtBQUssQ0FBQyxRQUFRLEVBQUUsSUFBSSxLQUFLLG1CQUFVLENBQUMsTUFBTSxFQUFFO1lBQ25ELE1BQU0sSUFBSSxLQUFLLENBQUMsa0RBQWtELENBQUMsQ0FBQztTQUNyRTtLQUNGO0lBRUQsSUFBSSxDQUFDLEtBQWdCLEVBQUUsUUFBeUM7UUFDOUQsTUFBTSxJQUFJLEdBQUcsSUFBSSxDQUFDLEtBQUssQ0FBQyxJQUFJLElBQUksSUFBSSxHQUFHLENBQUMsSUFBSSxDQUFDLEtBQUssRUFBRSxxQkFBcUIsRUFBRTtZQUN6RSxTQUFTLEVBQUUsSUFBSSxHQUFHLENBQUMsZ0JBQWdCLENBQUMsd0JBQXdCLENBQUM7U0FDOUQsQ0FBQyxDQUFDO1FBRUgsTUFBTSxXQUFXLEdBQUcsSUFBSSxDQUFDLE1BQU0sQ0FBQyxjQUFjLENBQUMsSUFBSSxDQUFDLENBQUM7UUFFckQsTUFBTSxFQUFFLGNBQWMsRUFBRSxXQUFXLEVBQUUsa0JBQWtCLEVBQUUsR0FBRyxJQUFBLDhCQUFvQixFQUFDLEtBQUssRUFBRTtZQUN0RixPQUFPLEVBQUUsSUFBSSxDQUFDLEtBQUssQ0FBQyxPQUFPO1lBQzNCLFFBQVEsRUFBRSxJQUFJLENBQUMsS0FBSyxDQUFDLFFBQVE7WUFDN0IsSUFBSTtZQUNKLFFBQVEsRUFBRSxlQUFlO1NBQzFCLENBQUMsSUFBSSxFQUFFLENBQUM7UUFFVCxNQUFNLEVBQUUsWUFBWSxFQUFFLFdBQVcsRUFBRSxpQkFBaUIsRUFBRSxHQUFHLElBQUEsNEJBQWtCLEVBQUMsS0FBSyxFQUFFLElBQUksRUFBRSxJQUFJLENBQUMsS0FBSyxDQUFDLFFBQVEsQ0FBQyxJQUFJLEVBQUUsQ0FBQztRQUNwSCxPQUFPO1lBQ0wsa0NBQWtDLEVBQUU7Z0JBQ2xDLHdCQUF3QixFQUFFLGNBQWM7Z0JBQ3hDLHVCQUF1QixFQUFFLElBQUEsZ0NBQXNCLEVBQUMsS0FBSyxFQUFFLElBQUksRUFBRSxJQUFJLENBQUMsS0FBSyxDQUFDLFNBQVMsQ0FBQztnQkFDbEYsT0FBTyxFQUFFLElBQUksQ0FBQyxPQUFPO2dCQUNyQixxQkFBcUIsRUFBRSxZQUFZO2dCQUNuQyxZQUFZLEVBQUUsSUFBSSxDQUFDLGVBQWUsRUFBRTtnQkFDcEMsY0FBYyxFQUFFLElBQUEsOEJBQW9CLEVBQUMsSUFBSSxDQUFDLEtBQUssQ0FBQyxpQkFBaUIsRUFBRSxJQUFJLENBQUMsS0FBSyxDQUFDLGFBQWEsQ0FBQztnQkFDNUYsU0FBUyxFQUFFLElBQUksQ0FBQyxNQUFNLENBQUMsU0FBUztnQkFDaEMsaUJBQWlCLEVBQUUsSUFBSSxDQUFDLEtBQUssQ0FBQyxXQUFXLEVBQUUsS0FBSztnQkFDaEQsdUJBQXVCLEVBQUUsSUFBQSxnQ0FBc0IsRUFBQyxJQUFJLEVBQUUsSUFBSSxDQUFDLEtBQUssQ0FBQyxhQUFhLENBQUM7Z0JBQy9FLGlCQUFpQixFQUFFLElBQUksQ0FBQyxLQUFLLENBQUMsaUJBQWlCO2dCQUMvQyxNQUFNLEVBQUUsSUFBSSxDQUFDLEtBQUssQ0FBQyxnQkFBZ0I7YUFDcEM7WUFDRCxXQUFXLEVBQUUsQ0FBQyxXQUFXLEVBQUUsR0FBRyxDQUFDLGtCQUFrQixJQUFJLEVBQUUsQ0FBQyxFQUFFLEdBQUcsQ0FBQyxpQkFBaUIsSUFBSSxFQUFFLENBQUMsQ0FBQztTQUN4RixDQUFDO0tBQ0g7SUFFTyxlQUFlO1FBQ3JCLE9BQU8sSUFBSSxDQUFDLEtBQUssQ0FBQyxRQUFRLEVBQUUsTUFBTSxJQUFJLElBQUksQ0FBQyxLQUFLLENBQUMsUUFBUSxFQUFFLElBQUksS0FBSyxtQkFBVSxDQUFDLEdBQUc7WUFDaEYsQ0FBQyxDQUFDLFNBQVM7WUFDWCxDQUFDLENBQUMsU0FBUyxDQUFDO0tBQ2Y7O0FBNUNILDRCQTZDQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCAqIGFzIGlhbSBmcm9tICdhd3MtY2RrLWxpYi9hd3MtaWFtJztcbmltcG9ydCAqIGFzIGZpcmVob3NlIGZyb20gJ0Bhd3MtY2RrL2F3cy1raW5lc2lzZmlyZWhvc2UtYWxwaGEnO1xuaW1wb3J0ICogYXMgczMgZnJvbSAnYXdzLWNkay1saWIvYXdzLXMzJztcbmltcG9ydCB7IENvbnN0cnVjdCB9IGZyb20gJ2NvbnN0cnVjdHMnO1xuaW1wb3J0IHsgQmFja3VwTW9kZSwgQ29tbW9uRGVzdGluYXRpb25Qcm9wcywgQ29tbW9uRGVzdGluYXRpb25TM1Byb3BzIH0gZnJvbSAnLi9jb21tb24nO1xuaW1wb3J0IHsgY3JlYXRlQmFja3VwQ29uZmlnLCBjcmVhdGVCdWZmZXJpbmdIaW50cywgY3JlYXRlRW5jcnlwdGlvbkNvbmZpZywgY3JlYXRlTG9nZ2luZ09wdGlvbnMsIGNyZWF0ZVByb2Nlc3NpbmdDb25maWcgfSBmcm9tICcuL3ByaXZhdGUvaGVscGVycyc7XG5cbi8qKlxuICogUHJvcHMgZm9yIGRlZmluaW5nIGFuIFMzIGRlc3RpbmF0aW9uIG9mIGEgS2luZXNpcyBEYXRhIEZpcmVob3NlIGRlbGl2ZXJ5IHN0cmVhbS5cbiAqL1xuZXhwb3J0IGludGVyZmFjZSBTM0J1Y2tldFByb3BzIGV4dGVuZHMgQ29tbW9uRGVzdGluYXRpb25TM1Byb3BzLCBDb21tb25EZXN0aW5hdGlvblByb3BzIHtcbn1cblxuLyoqXG4gKiBBbiBTMyBidWNrZXQgZGVzdGluYXRpb24gZm9yIGRhdGEgZnJvbSBhIEtpbmVzaXMgRGF0YSBGaXJlaG9zZSBkZWxpdmVyeSBzdHJlYW0uXG4gKi9cbmV4cG9ydCBjbGFzcyBTM0J1Y2tldCBpbXBsZW1lbnRzIGZpcmVob3NlLklEZXN0aW5hdGlvbiB7XG4gIGNvbnN0cnVjdG9yKHByaXZhdGUgcmVhZG9ubHkgYnVja2V0OiBzMy5JQnVja2V0LCBwcml2YXRlIHJlYWRvbmx5IHByb3BzOiBTM0J1Y2tldFByb3BzID0ge30pIHtcbiAgICBpZiAodGhpcy5wcm9wcy5zM0JhY2t1cD8ubW9kZSA9PT0gQmFja3VwTW9kZS5GQUlMRUQpIHtcbiAgICAgIHRocm93IG5ldyBFcnJvcignUzMgZGVzdGluYXRpb25zIGRvIG5vdCBzdXBwb3J0IEJhY2t1cE1vZGUuRkFJTEVEJyk7XG4gICAgfVxuICB9XG5cbiAgYmluZChzY29wZTogQ29uc3RydWN0LCBfb3B0aW9uczogZmlyZWhvc2UuRGVzdGluYXRpb25CaW5kT3B0aW9ucyk6IGZpcmVob3NlLkRlc3RpbmF0aW9uQ29uZmlnIHtcbiAgICBjb25zdCByb2xlID0gdGhpcy5wcm9wcy5yb2xlID8/IG5ldyBpYW0uUm9sZShzY29wZSwgJ1MzIERlc3RpbmF0aW9uIFJvbGUnLCB7XG4gICAgICBhc3N1bWVkQnk6IG5ldyBpYW0uU2VydmljZVByaW5jaXBhbCgnZmlyZWhvc2UuYW1hem9uYXdzLmNvbScpLFxuICAgIH0pO1xuXG4gICAgY29uc3QgYnVja2V0R3JhbnQgPSB0aGlzLmJ1Y2tldC5ncmFudFJlYWRXcml0ZShyb2xlKTtcblxuICAgIGNvbnN0IHsgbG9nZ2luZ09wdGlvbnMsIGRlcGVuZGFibGVzOiBsb2dnaW5nRGVwZW5kYWJsZXMgfSA9IGNyZWF0ZUxvZ2dpbmdPcHRpb25zKHNjb3BlLCB7XG4gICAgICBsb2dnaW5nOiB0aGlzLnByb3BzLmxvZ2dpbmcsXG4gICAgICBsb2dHcm91cDogdGhpcy5wcm9wcy5sb2dHcm91cCxcbiAgICAgIHJvbGUsXG4gICAgICBzdHJlYW1JZDogJ1MzRGVzdGluYXRpb24nLFxuICAgIH0pID8/IHt9O1xuXG4gICAgY29uc3QgeyBiYWNrdXBDb25maWcsIGRlcGVuZGFibGVzOiBiYWNrdXBEZXBlbmRhYmxlcyB9ID0gY3JlYXRlQmFja3VwQ29uZmlnKHNjb3BlLCByb2xlLCB0aGlzLnByb3BzLnMzQmFja3VwKSA/PyB7fTtcbiAgICByZXR1cm4ge1xuICAgICAgZXh0ZW5kZWRTM0Rlc3RpbmF0aW9uQ29uZmlndXJhdGlvbjoge1xuICAgICAgICBjbG91ZFdhdGNoTG9nZ2luZ09wdGlvbnM6IGxvZ2dpbmdPcHRpb25zLFxuICAgICAgICBwcm9jZXNzaW5nQ29uZmlndXJhdGlvbjogY3JlYXRlUHJvY2Vzc2luZ0NvbmZpZyhzY29wZSwgcm9sZSwgdGhpcy5wcm9wcy5wcm9jZXNzb3IpLFxuICAgICAgICByb2xlQXJuOiByb2xlLnJvbGVBcm4sXG4gICAgICAgIHMzQmFja3VwQ29uZmlndXJhdGlvbjogYmFja3VwQ29uZmlnLFxuICAgICAgICBzM0JhY2t1cE1vZGU6IHRoaXMuZ2V0UzNCYWNrdXBNb2RlKCksXG4gICAgICAgIGJ1ZmZlcmluZ0hpbnRzOiBjcmVhdGVCdWZmZXJpbmdIaW50cyh0aGlzLnByb3BzLmJ1ZmZlcmluZ0ludGVydmFsLCB0aGlzLnByb3BzLmJ1ZmZlcmluZ1NpemUpLFxuICAgICAgICBidWNrZXRBcm46IHRoaXMuYnVja2V0LmJ1Y2tldEFybixcbiAgICAgICAgY29tcHJlc3Npb25Gb3JtYXQ6IHRoaXMucHJvcHMuY29tcHJlc3Npb24/LnZhbHVlLFxuICAgICAgICBlbmNyeXB0aW9uQ29uZmlndXJhdGlvbjogY3JlYXRlRW5jcnlwdGlvbkNvbmZpZyhyb2xlLCB0aGlzLnByb3BzLmVuY3J5cHRpb25LZXkpLFxuICAgICAgICBlcnJvck91dHB1dFByZWZpeDogdGhpcy5wcm9wcy5lcnJvck91dHB1dFByZWZpeCxcbiAgICAgICAgcHJlZml4OiB0aGlzLnByb3BzLmRhdGFPdXRwdXRQcmVmaXgsXG4gICAgICB9LFxuICAgICAgZGVwZW5kYWJsZXM6IFtidWNrZXRHcmFudCwgLi4uKGxvZ2dpbmdEZXBlbmRhYmxlcyA/PyBbXSksIC4uLihiYWNrdXBEZXBlbmRhYmxlcyA/PyBbXSldLFxuICAgIH07XG4gIH1cblxuICBwcml2YXRlIGdldFMzQmFja3VwTW9kZSgpOiBzdHJpbmcgfCB1bmRlZmluZWQge1xuICAgIHJldHVybiB0aGlzLnByb3BzLnMzQmFja3VwPy5idWNrZXQgfHwgdGhpcy5wcm9wcy5zM0JhY2t1cD8ubW9kZSA9PT0gQmFja3VwTW9kZS5BTExcbiAgICAgID8gJ0VuYWJsZWQnXG4gICAgICA6IHVuZGVmaW5lZDtcbiAgfVxufVxuIl19
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9642210144927538%*

 * *Differences: {"'devDependencies'": "{'@aws-cdk/cdk-build-tools': '2.99.1-alpha.0', '@aws-cdk/integ-runner': "*

 * *                      "'2.99.1-alpha.0', '@aws-cdk/pkglint': '2.99.1-alpha.0', 'aws-cdk-lib': "*

 * *                      "'2.99.1', '@aws-cdk/aws-kinesisfirehose-alpha': '2.99.1-alpha.0'}",*

 * * "'peerDependencies'": "{'@aws-cdk/aws-kinesisfirehose-alpha': '2.99.1-alpha.0', 'aws-cdk-lib': "*

 * *                       "'2.99.1'}",*

 * * "'version'": "'2.99.1-alpha.0'"}*

```diff
@@ -11,20 +11,20 @@
         "env": {
             "AWSLINT_BASE_CONSTRUCT": true
         }
     },
     "dependencies": {},
     "description": "CDK Destinations Constructs for AWS Kinesis Firehose",
     "devDependencies": {
-        "@aws-cdk/aws-kinesisfirehose-alpha": "2.99.0-alpha.0",
-        "@aws-cdk/cdk-build-tools": "2.99.0-alpha.0",
-        "@aws-cdk/integ-runner": "2.99.0-alpha.0",
-        "@aws-cdk/pkglint": "2.99.0-alpha.0",
+        "@aws-cdk/aws-kinesisfirehose-alpha": "2.99.1-alpha.0",
+        "@aws-cdk/cdk-build-tools": "2.99.1-alpha.0",
+        "@aws-cdk/integ-runner": "2.99.1-alpha.0",
+        "@aws-cdk/pkglint": "2.99.1-alpha.0",
         "@types/jest": "^29.5.5",
-        "aws-cdk-lib": "2.99.0",
+        "aws-cdk-lib": "2.99.1",
         "constructs": "^10.0.0",
         "jest": "^29.7.0"
     },
     "engines": {
         "node": ">= 14.15.0"
     },
     "homepage": "https://github.com/aws/aws-cdk",
@@ -72,16 +72,16 @@
         "kinesisfirehose"
     ],
     "license": "Apache-2.0",
     "main": "lib/index.js",
     "maturity": "experimental",
     "name": "@aws-cdk/aws-kinesisfirehose-destinations-alpha",
     "peerDependencies": {
-        "@aws-cdk/aws-kinesisfirehose-alpha": "2.99.0-alpha.0",
-        "aws-cdk-lib": "2.99.0",
+        "@aws-cdk/aws-kinesisfirehose-alpha": "2.99.1-alpha.0",
+        "aws-cdk-lib": "2.99.1",
         "constructs": "^10.0.0"
     },
     "pkglint": {
         "exclude": [
             "naming/package-matches-directory",
             "assert/assert-dependency"
         ]
@@ -109,9 +109,9 @@
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

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-kinesisfirehose-destinations-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: CDK Destinations Constructs for AWS Kinesis Firehose
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.0a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-kinesisfirehose-destinations-alpha-2.99.1a0/src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/requires.txt
 src/aws_cdk.aws_kinesisfirehose_destinations_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_kinesisfirehose_destinations_alpha/__init__.py
 src/aws_cdk/aws_kinesisfirehose_destinations_alpha/py.typed
 src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/__init__.py
-src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/aws-kinesisfirehose-destinations-alpha@2.99.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_kinesisfirehose_destinations_alpha/_jsii/aws-kinesisfirehose-destinations-alpha@2.99.1-alpha.0.jsii.tgz
```

