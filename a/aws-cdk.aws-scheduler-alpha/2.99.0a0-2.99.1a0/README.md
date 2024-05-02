# Comparing `tmp/aws-cdk.aws-scheduler-alpha-2.99.0a0.tar.gz` & `tmp/aws-cdk.aws-scheduler-alpha-2.99.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src805316929/src/packages/@aws-cdk/aws-scheduler-alpha/dist/python/aws-cdk.aws-scheduler-alpha-2.99.0a0.tar", last modified: Wed Sep 27 19:39:10 2023, max compression
+gzip compressed data, was "/codebuild/output/src2270552867/src/packages/@aws-cdk/aws-scheduler-alpha/dist/python/aws-cdk.aws-scheduler-alpha-2.99.1a0.tar", last modified: Sat Sep 30 10:08:19 2023, max compression
```

## Comparing `aws-cdk.aws-scheduler-alpha-2.99.0a0.tar` & `aws-cdk.aws-scheduler-alpha-2.99.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-09-27 19:38:56.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-09-27 19:38:56.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-09-27 19:38:56.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12305 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11298 2023-09-27 19:38:56.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-09-27 19:38:56.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1886 2023-09-27 19:38:56.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk/aws_scheduler_alpha/
--rw-r--r--   0 root         (0) root         (0)   176361 2023-09-27 19:38:56.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      445 2023-09-27 19:38:56.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60142 2023-09-27 19:38:56.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.99.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:38:56.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk/aws_scheduler_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12305 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-09-27 19:39:10.000000 aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-09-30 10:08:05.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-09-30 10:08:05.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-09-30 10:08:05.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12305 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11298 2023-09-30 10:08:05.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-09-30 10:08:05.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-09-30 10:08:05.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk/aws_scheduler_alpha/
+-rw-r--r--   0 root         (0) root         (0)   176361 2023-09-30 10:08:05.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk/aws_scheduler_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk/aws_scheduler_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-09-30 10:08:05.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60141 2023-09-30 10:08:05.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.99.1-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:08:05.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk/aws_scheduler_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk.aws_scheduler_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12305 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      551 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-09-30 10:08:19.000000 aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.99.0a0/LICENSE` & `aws-cdk.aws-scheduler-alpha-2.99.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-scheduler-alpha-2.99.0a0/PKG-INFO` & `aws-cdk.aws-scheduler-alpha-2.99.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-scheduler-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: The CDK Construct Library for Amazon Scheduler
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.99.0a0/README.md` & `aws-cdk.aws-scheduler-alpha-2.99.1a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-scheduler-alpha-2.99.0a0/setup.py` & `aws-cdk.aws-scheduler-alpha-2.99.1a0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-scheduler-alpha",
-    "version": "2.99.0.a0",
+    "version": "2.99.1.a0",
     "description": "The CDK Construct Library for Amazon Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.aws_scheduler_alpha",
         "aws_cdk.aws_scheduler_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_scheduler_alpha._jsii": [
-            "aws-scheduler-alpha@2.99.0-alpha.0.jsii.tgz"
+            "aws-scheduler-alpha@2.99.1-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_scheduler_alpha": [
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

### Comparing `aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk/aws_scheduler_alpha/__init__.py` & `aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk/aws_scheduler_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.99.0-alpha.0.jsii.tgz` & `aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.99.1-alpha.0.jsii.tgz`

 * *Files 27% similar despite different names*

#### Comparing `aws-scheduler-alpha@2.99.0-alpha.0.jsii.tgz-content` & `aws-scheduler-alpha@2.99.1-alpha.0.jsii.tgz-content`

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
@@ -5714,9 +5714,9 @@
                     }
                 }
             ],
             "name": "ScheduleTargetInput",
             "symbolId": "lib/input:ScheduleTargetInput"
         }
     },
-    "version": "2.99.0-alpha.0"
+    "version": "2.99.1-alpha.0"
 }
```

##### package/lib/group.js

###### js-beautify {}

```diff
@@ -222,10 +222,10 @@
         this.groupName = this.physicalName;
     }
 }
 exports.Group = Group;
 _a = JSII_RTTI_SYMBOL_1;
 Group[_a] = {
     fqn: "@aws-cdk/aws-scheduler-alpha.Group",
-    version: "2.99.0-alpha.0"
+    version: "2.99.1-alpha.0"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZ3JvdXAuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyJncm91cC50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7Ozs7QUFBQSx5REFBeUQ7QUFDekQsMkNBQTJDO0FBQzNDLDZEQUE2RDtBQUM3RCwyQ0FBZ0g7QUF1SGhILE1BQWUsU0FBVSxTQUFRLGVBQVE7SUFldkM7Ozs7T0FJRztJQUNJLE1BQU0sQ0FBQyxVQUFrQixFQUFFLEtBQWdDO1FBQ2hFLE9BQU8sSUFBSSxVQUFVLENBQUMsTUFBTSxDQUFDO1lBQzNCLFNBQVMsRUFBRSxlQUFlO1lBQzFCLFVBQVU7WUFDVixhQUFhLEVBQUUsRUFBRSxhQUFhLEVBQUUsSUFBSSxDQUFDLFNBQVMsRUFBRTtZQUNoRCxTQUFTLEVBQUUsS0FBSztZQUNoQixHQUFHLEtBQUs7U0FDVCxDQUFDLENBQUMsUUFBUSxDQUFDLElBQUksQ0FBQyxDQUFDO0tBQ25CO0lBRUQ7Ozs7OztPQU1HO0lBQ0ksZUFBZSxDQUFDLEtBQWdDO1FBQ3JELE9BQU8sSUFBSSxDQUFDLE1BQU0sQ0FBQyx5QkFBeUIsRUFBRSxLQUFLLENBQUMsQ0FBQztLQUN0RDtJQUVEOzs7O09BSUc7SUFDSSxjQUFjLENBQUMsS0FBZ0M7UUFDcEQsT0FBTyxJQUFJLENBQUMsTUFBTSxDQUFDLHdCQUF3QixFQUFFLEtBQUssQ0FBQyxDQUFDO0tBQ3JEO0lBRUQ7Ozs7T0FJRztJQUNJLGtCQUFrQixDQUFDLEtBQWdDO1FBQ3hELE9BQU8sSUFBSSxDQUFDLE1BQU0sQ0FBQyxrQkFBa0IsRUFBRSxLQUFLLENBQUMsQ0FBQztLQUMvQztJQUVEOzs7O09BSUc7SUFDSSxxQkFBcUIsQ0FBQyxLQUFnQztRQUMzRCxPQUFPLElBQUksQ0FBQyxNQUFNLENBQUMsMkJBQTJCLEVBQUUsS0FBSyxDQUFDLENBQUM7S0FDeEQ7SUFFRDs7OztPQUlHO0lBQ0ksYUFBYSxDQUFDLEtBQWdDO1FBQ25ELE9BQU8sSUFBSSxDQUFDLE1BQU0sQ0FBQyx3QkFBd0IsRUFBRSxLQUFLLENBQUMsQ0FBQztLQUNyRDtJQUVEOzs7O09BSUc7SUFDSCxlQUFlLENBQUMsS0FBZ0M7UUFDOUMsT0FBTyxJQUFJLENBQUMsTUFBTSxDQUFDLGtDQUFrQyxFQUFFLEtBQUssQ0FBQyxDQUFDO0tBQy9EO0lBRUQ7Ozs7T0FJRztJQUNJLHlCQUF5QixDQUFDLFNBQWtCLEVBQUUsS0FBZ0M7UUFDbkYsSUFBSSxTQUFTLEVBQUU7WUFDYixPQUFPLElBQUksQ0FBQyxNQUFNLENBQUMsOENBQThDLFNBQVMsRUFBRSxFQUFFLEtBQUssQ0FBQyxDQUFDO1NBQ3RGO1FBRUQsT0FBTyxJQUFJLENBQUMsTUFBTSxDQUFDLDRDQUE0QyxFQUFFLEtBQUssQ0FBQyxDQUFDO0tBQ3pFO0lBRUQ7Ozs7T0FJRztJQUNJLHdCQUF3QixDQUFDLEtBQWdDO1FBQzlELE9BQU8sSUFBSSxDQUFDLE1BQU0sQ0FBQyxnRUFBZ0UsRUFBRSxLQUFLLENBQUMsQ0FBQztLQUM3RjtJQUVEOztPQUVHO0lBQ0ksS0FBSyxDQUFDLE9BQXVCLEVBQUUsR0FBRyxPQUFpQjtRQUN4RCxPQUFPLEdBQUcsQ0FBQyxLQUFLLENBQUMsY0FBYyxDQUFDO1lBQzlCLE9BQU87WUFDUCxPQUFPO1lBQ1AsWUFBWSxFQUFFLENBQUMsSUFBSSxDQUFDLFFBQVEsQ0FBQztZQUM3QixLQUFLLEVBQUUsSUFBSTtTQUNaLENBQUMsQ0FBQztLQUNKO0lBRU8scUJBQXFCLENBQUMsWUFBb0I7UUFDaEQsT0FBTyxVQUFHLENBQUMsTUFBTSxDQUFDO1lBQ2hCLE1BQU0sRUFBRSxJQUFJLENBQUMsR0FBRyxDQUFDLE1BQU07WUFDdkIsT0FBTyxFQUFFLElBQUksQ0FBQyxHQUFHLENBQUMsT0FBTztZQUN6QixTQUFTLEVBQUUsVUFBRyxDQUFDLFNBQVM7WUFDeEIsT0FBTyxFQUFFLFdBQVc7WUFDcEIsUUFBUSxFQUFFLFVBQVU7WUFDcEIsWUFBWSxFQUFFLElBQUksQ0FBQyxTQUFTLEdBQUcsR0FBRyxHQUFHLFlBQVk7U0FDbEQsQ0FBQyxDQUFDO0tBQ0o7SUFFRDs7T0FFRztJQUNJLGtCQUFrQixDQUFDLFFBQXdCO1FBQ2hELE9BQU8sR0FBRyxDQUFDLEtBQUssQ0FBQyxjQUFjLENBQUM7WUFDOUIsT0FBTyxFQUFFLFFBQVE7WUFDakIsT0FBTyxFQUFFLENBQUMsdUJBQXVCLEVBQUUseUJBQXlCLENBQUM7WUFDN0QsWUFBWSxFQUFFLENBQUMsSUFBSSxDQUFDLHFCQUFxQixDQUFDLEdBQUcsQ0FBQyxDQUFDO1lBQy9DLEtBQUssRUFBRSxJQUFJO1NBQ1osQ0FBQyxDQUFDO0tBQ0o7SUFFRDs7T0FFRztJQUNJLG1CQUFtQixDQUFDLFFBQXdCO1FBQ2pELE9BQU8sR0FBRyxDQUFDLEtBQUssQ0FBQyxjQUFjLENBQUM7WUFDOUIsT0FBTyxFQUFFLFFBQVE7WUFDakIsT0FBTyxFQUFFLENBQUMsMEJBQTBCLEVBQUUsMEJBQTBCLENBQUM7WUFDakUsWUFBWSxFQUFFLENBQUMsSUFBSSxDQUFDLHFCQUFxQixDQUFDLEdBQUcsQ0FBQyxDQUFDO1lBQy9DLEtBQUssRUFBRSxJQUFJO1NBQ1osQ0FBQyxDQUFDO0tBQ0o7SUFFRDs7T0FFRztJQUNJLG9CQUFvQixDQUFDLFFBQXdCO1FBQ2xELE9BQU8sR0FBRyxDQUFDLEtBQUssQ0FBQyxjQUFjLENBQUM7WUFDOUIsT0FBTyxFQUFFLFFBQVE7WUFDakIsT0FBTyxFQUFFLENBQUMsMEJBQTBCLENBQUM7WUFDckMsWUFBWSxFQUFFLENBQUMsSUFBSSxDQUFDLHFCQUFxQixDQUFDLEdBQUcsQ0FBQyxDQUFDO1lBQy9DLEtBQUssRUFBRSxJQUFJO1NBQ1osQ0FBQyxDQUFDO0tBQ0o7Q0FDRjtBQUNEOztHQUVHO0FBQ0gsTUFBYSxLQUFNLFNBQVEsU0FBUztJQUNsQzs7Ozs7O09BTUc7SUFDSSxNQUFNLENBQUMsWUFBWSxDQUFDLEtBQWdCLEVBQUUsRUFBVSxFQUFFLFFBQWdCO1FBQ3ZFLE1BQU0sYUFBYSxHQUFHLFlBQUssQ0FBQyxFQUFFLENBQUMsS0FBSyxDQUFDLENBQUMsUUFBUSxDQUFDLFFBQVEsRUFBRSxnQkFBUyxDQUFDLG1CQUFtQixDQUFDLENBQUM7UUFDeEYsTUFBTSxTQUFTLEdBQUcsYUFBYSxDQUFDLFlBQWEsQ0FBQztRQUM5QyxNQUFNLE1BQU8sU0FBUSxTQUFTO1lBQTlCOztnQkFDRSxjQUFTLEdBQUcsU0FBUyxDQUFDO2dCQUN0QixhQUFRLEdBQUcsUUFBUSxDQUFDO1lBQ3RCLENBQUM7U0FBQTtRQUNELE9BQU8sSUFBSSxNQUFNLENBQUMsS0FBSyxFQUFFLEVBQUUsQ0FBQyxDQUFDO0tBQzlCO0lBRUQ7Ozs7O09BS0c7SUFDSSxNQUFNLENBQUMsZ0JBQWdCLENBQUMsS0FBZ0IsRUFBRSxFQUFVO1FBQ3pELE9BQU8sS0FBSyxDQUFDLGFBQWEsQ0FBQyxLQUFLLEVBQUUsRUFBRSxFQUFFLFNBQVMsQ0FBQyxDQUFDO0tBQ2xEO0lBRUQ7Ozs7OztPQU1HO0lBQ0ksTUFBTSxDQUFDLGFBQWEsQ0FBQyxLQUFnQixFQUFFLEVBQVUsRUFBRSxTQUFpQjtRQUN6RSxNQUFNLFFBQVEsR0FBRyxZQUFLLENBQUMsRUFBRSxDQUFDLEtBQUssQ0FBQyxDQUFDLFNBQVMsQ0FBQztZQUN6QyxPQUFPLEVBQUUsV0FBVztZQUNwQixRQUFRLEVBQUUsZ0JBQWdCO1lBQzFCLFlBQVksRUFBRSxTQUFTO1NBQ3hCLENBQUMsQ0FBQztRQUNILE9BQU8sS0FBSyxDQUFDLFlBQVksQ0FBQyxLQUFLLEVBQUUsRUFBRSxFQUFFLFFBQVEsQ0FBQyxDQUFDO0tBQ2hEO0lBS0QsWUFBbUIsS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBaUI7UUFDaEUsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLEVBQUU7WUFDZixZQUFZLEVBQUUsS0FBSyxDQUFDLFNBQVMsSUFBSSxtQkFBWSxDQUFDLGtCQUFrQjtTQUNqRSxDQUFDLENBQUM7Ozs7OzsrQ0FsRE0sS0FBSzs7OztRQW9EZCxNQUFNLEtBQUssR0FBRyxJQUFJLGdDQUFnQixDQUFDLElBQUksRUFBRSxVQUFVLEVBQUU7WUFDbkQsSUFBSSxFQUFFLElBQUksQ0FBQyxZQUFZO1NBQ3hCLENBQUMsQ0FBQztRQUVILEtBQUssQ0FBQyxrQkFBa0IsQ0FBQyxLQUFLLENBQUMsYUFBYSxDQUFDLENBQUM7UUFFOUMsSUFBSSxDQUFDLFFBQVEsR0FBRyxJQUFJLENBQUMsdUJBQXVCLENBQUMsS0FBSyxDQUFDLE9BQU8sRUFBRTtZQUMxRCxPQUFPLEVBQUUsV0FBVztZQUNwQixRQUFRLEVBQUUsZ0JBQWdCO1lBQzFCLFlBQVksRUFBRSxJQUFJLENBQUMsWUFBWTtTQUNoQyxDQUFDLENBQUM7UUFDSCxJQUFJLENBQUMsU0FBUyxHQUFHLElBQUksQ0FBQyxZQUFZLENBQUM7S0FDcEM7O0FBaEVILHNCQWlFQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCAqIGFzIGNsb3Vkd2F0Y2ggZnJvbSAnYXdzLWNkay1saWIvYXdzLWNsb3Vkd2F0Y2gnO1xuaW1wb3J0ICogYXMgaWFtIGZyb20gJ2F3cy1jZGstbGliL2F3cy1pYW0nO1xuaW1wb3J0IHsgQ2ZuU2NoZWR1bGVHcm91cCB9IGZyb20gJ2F3cy1jZGstbGliL2F3cy1zY2hlZHVsZXInO1xuaW1wb3J0IHsgQXJuLCBBcm5Gb3JtYXQsIEF3cywgSVJlc291cmNlLCBQaHlzaWNhbE5hbWUsIFJlbW92YWxQb2xpY3ksIFJlc291cmNlLCBTdGFjayB9IGZyb20gJ2F3cy1jZGstbGliL2NvcmUnO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5cbmV4cG9ydCBpbnRlcmZhY2UgR3JvdXBQcm9wcyB7XG4gIC8qKlxuICAgKiBUaGUgbmFtZSBvZiB0aGUgc2NoZWR1bGUgZ3JvdXAuXG4gICAqXG4gICAqIFVwIHRvIDY0IGxldHRlcnMgKHVwcGVyY2FzZSBhbmQgbG93ZXJjYXNlKSwgbnVtYmVycywgaHlwaGVucywgdW5kZXJzY29yZXMgYW5kIGRvdHMgYXJlIGFsbG93ZWQuXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gQSB1bmlxdWUgbmFtZSB3aWxsIGJlIGdlbmVyYXRlZFxuICAgKi9cbiAgcmVhZG9ubHkgZ3JvdXBOYW1lPzogc3RyaW5nO1xuXG4gIC8qKlxuICAgKiBUaGUgcmVtb3ZhbCBwb2xpY3kgZm9yIHRoZSBncm91cC4gSWYgdGhlIGdyb3VwIGlzIHJlbW92ZWQgYWxzbyBhbGwgc2NoZWR1bGVzIGFyZSByZW1vdmVkLlxuICAgKlxuICAgKiBAZGVmYXVsdCBSZW1vdmFsUG9saWN5LlJFVEFJTlxuICAgKi9cbiAgcmVhZG9ubHkgcmVtb3ZhbFBvbGljeT86IFJlbW92YWxQb2xpY3k7XG59XG5cbmV4cG9ydCBpbnRlcmZhY2UgSUdyb3VwIGV4dGVuZHMgSVJlc291cmNlIHtcbiAgLyoqXG4gICAqIFRoZSBuYW1lIG9mIHRoZSBzY2hlZHVsZSBncm91cFxuICAgKlxuICAgKiBAYXR0cmlidXRlXG4gICAqL1xuICByZWFkb25seSBncm91cE5hbWU6IHN0cmluZztcblxuICAvKipcbiAgICogVGhlIGFybiBvZiB0aGUgc2NoZWR1bGUgZ3JvdXBcbiAgICpcbiAgICogQGF0dHJpYnV0ZVxuICAgKi9cbiAgcmVhZG9ubHkgZ3JvdXBBcm46IHN0cmluZztcblxuICAvKipcbiAgICogUmV0dXJuIHRoZSBnaXZlbiBuYW1lZCBtZXRyaWMgZm9yIHRoaXMgZ3JvdXAgc2NoZWR1bGVzXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gc3VtIG92ZXIgNSBtaW51dGVzXG4gICAqL1xuICBtZXRyaWMobWV0cmljTmFtZTogc3RyaW5nLCBwcm9wcz86IGNsb3Vkd2F0Y2guTWV0cmljT3B0aW9ucyk6IGNsb3Vkd2F0Y2guTWV0cmljO1xuXG4gIC8qKlxuICAgKiBNZXRyaWMgZm9yIHRoZSBudW1iZXIgb2YgaW52b2NhdGlvbnMgdGhhdCB3ZXJlIHRocm90dGxlZCBiZWNhdXNlIGl0IGV4Y2VlZHMgeW91ciBzZXJ2aWNlIHF1b3Rhcy5cbiAgICpcbiAgICogQHNlZSBodHRwczovL2RvY3MuYXdzLmFtYXpvbi5jb20vc2NoZWR1bGVyL2xhdGVzdC9Vc2VyR3VpZGUvc2NoZWR1bGVyLXF1b3Rhcy5odG1sXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gc3VtIG92ZXIgNSBtaW51dGVzXG4gICAqL1xuICBtZXRyaWNUaHJvdHRsZWQocHJvcHM/OiBjbG91ZHdhdGNoLk1ldHJpY09wdGlvbnMpOiBjbG91ZHdhdGNoLk1ldHJpYztcblxuICAvKipcbiAgICogTWV0cmljIGZvciBhbGwgaW52b2NhdGlvbiBhdHRlbXB0cy5cbiAgICpcbiAgICogQGRlZmF1bHQgLSBzdW0gb3ZlciA1IG1pbnV0ZXNcbiAgICovXG4gIG1ldHJpY0F0dGVtcHRzKHByb3BzPzogY2xvdWR3YXRjaC5NZXRyaWNPcHRpb25zKTogY2xvdWR3YXRjaC5NZXRyaWM7XG5cbiAgLyoqXG4gICAqIEVtaXR0ZWQgd2hlbiB0aGUgdGFyZ2V0IHJldHVybnMgYW4gZXhjZXB0aW9uIGFmdGVyIEV2ZW50QnJpZGdlIFNjaGVkdWxlciBjYWxscyB0aGUgdGFyZ2V0IEFQSS5cbiAgICpcbiAgICogQGRlZmF1bHQgLSBzdW0gb3ZlciA1IG1pbnV0ZXNcbiAgICovXG4gIG1ldHJpY1RhcmdldEVycm9ycyhwcm9wcz86IGNsb3Vkd2F0Y2guTWV0cmljT3B0aW9ucyk6IGNsb3Vkd2F0Y2guTWV0cmljO1xuXG4gIC8qKlxuICAgKiBNZXRyaWMgZm9yIGludm9jYXRpb24gZmFpbHVyZXMgZHVlIHRvIEFQSSB0aHJvdHRsaW5nIGJ5IHRoZSB0YXJnZXQuXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gc3VtIG92ZXIgNSBtaW51dGVzXG4gICAqL1xuICBtZXRyaWNUYXJnZXRUaHJvdHRsZWQocHJvcHM/OiBjbG91ZHdhdGNoLk1ldHJpY09wdGlvbnMpOiBjbG91ZHdhdGNoLk1ldHJpYztcblxuICAvKipcbiAgICogTWV0cmljIGZvciBkcm9wcGVkIGludm9jYXRpb25zIHdoZW4gRXZlbnRCcmlkZ2UgU2NoZWR1bGVyIHN0b3BzIGF0dGVtcHRpbmcgdG8gaW52b2tlIHRoZSB0YXJnZXQgYWZ0ZXIgYSBzY2hlZHVsZSdzIHJldHJ5IHBvbGljeSBoYXMgYmVlbiBleGhhdXN0ZWQuXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gc3VtIG92ZXIgNSBtaW51dGVzXG4gICAqL1xuICBtZXRyaWNEcm9wcGVkKHByb3BzPzogY2xvdWR3YXRjaC5NZXRyaWNPcHRpb25zKTogY2xvdWR3YXRjaC5NZXRyaWM7XG5cbiAgLyoqXG4gICAqIE1ldHJpYyBmb3IgaW52b2NhdGlvbnMgZGVsaXZlcmVkIHRvIHRoZSBETFFcbiAgICpcbiAgICogQGRlZmF1bHQgLSBzdW0gb3ZlciA1IG1pbnV0ZXNcbiAgICovXG4gIG1ldHJpY1NlbnRUb0RMUShwcm9wcz86IGNsb3Vkd2F0Y2guTWV0cmljT3B0aW9ucyk6IGNsb3Vkd2F0Y2guTWV0cmljO1xuXG4gIC8qKlxuICAgKiBNZXRyaWMgZm9yIGZhaWxlZCBpbnZvY2F0aW9ucyB0aGF0IGFsc28gZmFpbGVkIHRvIGRlbGl2ZXIgdG8gRExRLlxuICAgKlxuICAgKiBAZGVmYXVsdCAtIHN1bSBvdmVyIDUgbWludXRlc1xuICAgKi9cbiAgbWV0cmljRmFpbGVkVG9CZVNlbnRUb0RMUShlcnJvckNvZGU/OiBzdHJpbmcsIHByb3BzPzogY2xvdWR3YXRjaC5NZXRyaWNPcHRpb25zKTogY2xvdWR3YXRjaC5NZXRyaWM7XG5cbiAgLyoqXG4gICAqIE1ldHJpYyBmb3IgZGVsaXZlcnkgb2YgZmFpbGVkIGludm9jYXRpb25zIHRvIERMUSB3aGVuIHRoZSBwYXlsb2FkIG9mIHRoZSBldmVudCBzZW50IHRvIHRoZSBETFEgZXhjZWVkcyB0aGUgbWF4aW11bSBzaXplIGFsbG93ZWQgYnkgQW1hem9uIFNRUy5cbiAgICpcbiAgICogQGRlZmF1bHQgLSBzdW0gb3ZlciA1IG1pbnV0ZXNcbiAgICovXG4gIG1ldHJpY1NlbnRUb0RMUVRydW5hY3RlZChwcm9wcz86IGNsb3Vkd2F0Y2guTWV0cmljT3B0aW9ucyk6IGNsb3Vkd2F0Y2guTWV0cmljO1xuXG4gIC8qKlxuICAgKiBHcmFudCB0aGUgaW5kaWNhdGVkIHBlcm1pc3Npb25zIG9uIHRoaXMgZ3JvdXAgdG8gdGhlIGdpdmVuIHByaW5jaXBhbFxuICAgKi9cbiAgZ3JhbnQoZ3JhbnRlZTogaWFtLklHcmFudGFibGUsIC4uLmFjdGlvbnM6IHN0cmluZ1tdKTogaWFtLkdyYW50O1xuICAvKipcbiAgICogR3JhbnQgbGlzdCBhbmQgZ2V0IHNjaGVkdWxlIHBlcm1pc3Npb25zIGZvciBzY2hlZHVsZXMgaW4gdGhpcyBncm91cCB0byB0aGUgZ2l2ZW4gcHJpbmNpcGFsXG4gICAqL1xuICBncmFudFJlYWRTY2hlZHVsZXMoaWRlbnRpdHk6IGlhbS5JR3JhbnRhYmxlKTogaWFtLkdyYW50O1xuICAvKipcbiAgICogR3JhbnQgY3JlYXRlIGFuZCB1cGRhdGUgc2NoZWR1bGUgcGVybWlzc2lvbnMgZm9yIHNjaGVkdWxlcyBpbiB0aGlzIGdyb3VwIHRvIHRoZSBnaXZlbiBwcmluY2lwYWxcbiAgICovXG4gIGdyYW50V3JpdGVTY2hlZHVsZXMoaWRlbnRpdHk6IGlhbS5JR3JhbnRhYmxlKTogaWFtLkdyYW50O1xuICAvKipcbiAgICogR3JhbnQgZGVsZXRlIHNjaGVkdWxlIHBlcm1pc3Npb24gZm9yIHNjaGVkdWxlcyBpbiB0aGlzIGdyb3VwIHRvIHRoZSBnaXZlbiBwcmluY2lwYWxcbiAgICovXG4gIGdyYW50RGVsZXRlU2NoZWR1bGVzKGlkZW50aXR5OiBpYW0uSUdyYW50YWJsZSk6IGlhbS5HcmFudFxufVxuXG5hYnN0cmFjdCBjbGFzcyBHcm91cEJhc2UgZXh0ZW5kcyBSZXNvdXJjZSBpbXBsZW1lbnRzIElHcm91cCB7XG4gIC8qKlxuICAgKiBUaGUgbmFtZSBvZiB0aGUgc2NoZWR1bGUgZ3JvdXBcbiAgICpcbiAgICogQGF0dHJpYnV0ZVxuICAgKi9cbiAgcHVibGljIGFic3RyYWN0IHJlYWRvbmx5IGdyb3VwTmFtZTogc3RyaW5nO1xuXG4gIC8qKlxuICAgKiBUaGUgYXJuIG9mIHRoZSBzY2hlZHVsZSBncm91cFxuICAgKlxuICAgKiBAYXR0cmlidXRlXG4gICAqL1xuICBwdWJsaWMgYWJzdHJhY3QgcmVhZG9ubHkgZ3JvdXBBcm46IHN0cmluZztcblxuICAvKipcbiAgICogUmV0dXJuIHRoZSBnaXZlbiBuYW1lZCBtZXRyaWMgZm9yIHRoaXMgZ3JvdXAgc2NoZWR1bGVzXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gc3VtIG92ZXIgNSBtaW51dGVzXG4gICAqL1xuICBwdWJsaWMgbWV0cmljKG1ldHJpY05hbWU6IHN0cmluZywgcHJvcHM/OiBjbG91ZHdhdGNoLk1ldHJpY09wdGlvbnMpOiBjbG91ZHdhdGNoLk1ldHJpYyB7XG4gICAgcmV0dXJuIG5ldyBjbG91ZHdhdGNoLk1ldHJpYyh7XG4gICAgICBuYW1lc3BhY2U6ICdBV1MvU2NoZWR1bGVyJyxcbiAgICAgIG1ldHJpY05hbWUsXG4gICAgICBkaW1lbnNpb25zTWFwOiB7IFNjaGVkdWxlR3JvdXA6IHRoaXMuZ3JvdXBOYW1lIH0sXG4gICAgICBzdGF0aXN0aWM6ICdzdW0nLFxuICAgICAgLi4ucHJvcHMsXG4gICAgfSkuYXR0YWNoVG8odGhpcyk7XG4gIH1cblxuICAvKipcbiAgICogTWV0cmljIGZvciB0aGUgbnVtYmVyIG9mIGludm9jYXRpb25zIHRoYXQgd2VyZSB0aHJvdHRsZWQgYmVjYXVzZSBpdCBleGNlZWRzIHlvdXIgc2VydmljZSBxdW90YXMuXG4gICAqXG4gICAqIEBzZWUgaHR0cHM6Ly9kb2NzLmF3cy5hbWF6b24uY29tL3NjaGVkdWxlci9sYXRlc3QvVXNlckd1aWRlL3NjaGVkdWxlci1xdW90YXMuaHRtbFxuICAgKlxuICAgKiBAZGVmYXVsdCAtIHN1bSBvdmVyIDUgbWludXRlc1xuICAgKi9cbiAgcHVibGljIG1ldHJpY1Rocm90dGxlZChwcm9wcz86IGNsb3Vkd2F0Y2guTWV0cmljT3B0aW9ucyk6IGNsb3Vkd2F0Y2guTWV0cmljIHtcbiAgICByZXR1cm4gdGhpcy5tZXRyaWMoJ0ludm9jYXRpb25UaHJvdHRsZUNvdW50JywgcHJvcHMpO1xuICB9XG5cbiAgLyoqXG4gICAqIE1ldHJpYyBmb3IgYWxsIGludm9jYXRpb24gYXR0ZW1wdHMuXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gc3VtIG92ZXIgNSBtaW51dGVzXG4gICAqL1xuICBwdWJsaWMgbWV0cmljQXR0ZW1wdHMocHJvcHM/OiBjbG91ZHdhdGNoLk1ldHJpY09wdGlvbnMpOiBjbG91ZHdhdGNoLk1ldHJpYyB7XG4gICAgcmV0dXJuIHRoaXMubWV0cmljKCdJbnZvY2F0aW9uQXR0ZW1wdENvdW50JywgcHJvcHMpO1xuICB9XG5cbiAgLyoqXG4gICAqIEVtaXR0ZWQgd2hlbiB0aGUgdGFyZ2V0IHJldHVybnMgYW4gZXhjZXB0aW9uIGFmdGVyIEV2ZW50QnJpZGdlIFNjaGVkdWxlciBjYWxscyB0aGUgdGFyZ2V0IEFQSS5cbiAgICpcbiAgICogQGRlZmF1bHQgLSBzdW0gb3ZlciA1IG1pbnV0ZXNcbiAgICovXG4gIHB1YmxpYyBtZXRyaWNUYXJnZXRFcnJvcnMocHJvcHM/OiBjbG91ZHdhdGNoLk1ldHJpY09wdGlvbnMpOiBjbG91ZHdhdGNoLk1ldHJpYyB7XG4gICAgcmV0dXJuIHRoaXMubWV0cmljKCdUYXJnZXRFcnJvckNvdW50JywgcHJvcHMpO1xuICB9XG5cbiAgLyoqXG4gICAqIE1ldHJpYyBmb3IgaW52b2NhdGlvbiBmYWlsdXJlcyBkdWUgdG8gQVBJIHRocm90dGxpbmcgYnkgdGhlIHRhcmdldC5cbiAgICpcbiAgICogQGRlZmF1bHQgLSBzdW0gb3ZlciA1IG1pbnV0ZXNcbiAgICovXG4gIHB1YmxpYyBtZXRyaWNUYXJnZXRUaHJvdHRsZWQocHJvcHM/OiBjbG91ZHdhdGNoLk1ldHJpY09wdGlvbnMpOiBjbG91ZHdhdGNoLk1ldHJpYyB7XG4gICAgcmV0dXJuIHRoaXMubWV0cmljKCdUYXJnZXRFcnJvclRocm90dGxlZENvdW50JywgcHJvcHMpO1xuICB9XG5cbiAgLyoqXG4gICAqIE1ldHJpYyBmb3IgZHJvcHBlZCBpbnZvY2F0aW9ucyB3aGVuIEV2ZW50QnJpZGdlIFNjaGVkdWxlciBzdG9wcyBhdHRlbXB0aW5nIHRvIGludm9rZSB0aGUgdGFyZ2V0IGFmdGVyIGEgc2NoZWR1bGUncyByZXRyeSBwb2xpY3kgaGFzIGJlZW4gZXhoYXVzdGVkLlxuICAgKlxuICAgKiBAZGVmYXVsdCAtIHN1bSBvdmVyIDUgbWludXRlc1xuICAgKi9cbiAgcHVibGljIG1ldHJpY0Ryb3BwZWQocHJvcHM/OiBjbG91ZHdhdGNoLk1ldHJpY09wdGlvbnMpOiBjbG91ZHdhdGNoLk1ldHJpYyB7XG4gICAgcmV0dXJuIHRoaXMubWV0cmljKCdJbnZvY2F0aW9uRHJvcHBlZENvdW50JywgcHJvcHMpO1xuICB9XG5cbiAgLyoqXG4gICAqIE1ldHJpYyBmb3IgaW52b2NhdGlvbnMgZGVsaXZlcmVkIHRvIHRoZSBETFFcbiAgICpcbiAgICogQGRlZmF1bHQgLSBzdW0gb3ZlciA1IG1pbnV0ZXNcbiAgICovXG4gIG1ldHJpY1NlbnRUb0RMUShwcm9wcz86IGNsb3Vkd2F0Y2guTWV0cmljT3B0aW9ucyk6IGNsb3Vkd2F0Y2guTWV0cmljIHtcbiAgICByZXR1cm4gdGhpcy5tZXRyaWMoJ0ludm9jYXRpb25zU2VudFRvRGVhZExldHRlckNvdW50JywgcHJvcHMpO1xuICB9XG5cbiAgLyoqXG4gICAqIE1ldHJpYyBmb3IgZmFpbGVkIGludm9jYXRpb25zIHRoYXQgYWxzbyBmYWlsZWQgdG8gZGVsaXZlciB0byBETFEuXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gc3VtIG92ZXIgNSBtaW51dGVzXG4gICAqL1xuICBwdWJsaWMgbWV0cmljRmFpbGVkVG9CZVNlbnRUb0RMUShlcnJvckNvZGU/OiBzdHJpbmcsIHByb3BzPzogY2xvdWR3YXRjaC5NZXRyaWNPcHRpb25zKTogY2xvdWR3YXRjaC5NZXRyaWMge1xuICAgIGlmIChlcnJvckNvZGUpIHtcbiAgICAgIHJldHVybiB0aGlzLm1ldHJpYyhgSW52b2NhdGlvbnNGYWlsZWRUb0JlU2VudFRvRGVhZExldHRlckNvdW50XyR7ZXJyb3JDb2RlfWAsIHByb3BzKTtcbiAgICB9XG5cbiAgICByZXR1cm4gdGhpcy5tZXRyaWMoJ0ludm9jYXRpb25zRmFpbGVkVG9CZVNlbnRUb0RlYWRMZXR0ZXJDb3VudCcsIHByb3BzKTtcbiAgfVxuXG4gIC8qKlxuICAgKiBNZXRyaWMgZm9yIGRlbGl2ZXJ5IG9mIGZhaWxlZCBpbnZvY2F0aW9ucyB0byBETFEgd2hlbiB0aGUgcGF5bG9hZCBvZiB0aGUgZXZlbnQgc2VudCB0byB0aGUgRExRIGV4Y2VlZHMgdGhlIG1heGltdW0gc2l6ZSBhbGxvd2VkIGJ5IEFtYXpvbiBTUVMuXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gc3VtIG92ZXIgNSBtaW51dGVzXG4gICAqL1xuICBwdWJsaWMgbWV0cmljU2VudFRvRExRVHJ1bmFjdGVkKHByb3BzPzogY2xvdWR3YXRjaC5NZXRyaWNPcHRpb25zKTogY2xvdWR3YXRjaC5NZXRyaWMge1xuICAgIHJldHVybiB0aGlzLm1ldHJpYygnSW52b2NhdGlvbnNTZW50VG9EZWFkTGV0dGVyQ291bnRfVHJ1bmNhdGVkX01lc3NhZ2VTaXplRXhjZWVkZWQnLCBwcm9wcyk7XG4gIH1cblxuICAvKipcbiAgICogR3JhbnQgdGhlIGluZGljYXRlZCBwZXJtaXNzaW9ucyBvbiB0aGlzIGdyb3VwIHRvIHRoZSBnaXZlbiBwcmluY2lwYWxcbiAgICovXG4gIHB1YmxpYyBncmFudChncmFudGVlOiBpYW0uSUdyYW50YWJsZSwgLi4uYWN0aW9uczogc3RyaW5nW10pOiBpYW0uR3JhbnQge1xuICAgIHJldHVybiBpYW0uR3JhbnQuYWRkVG9QcmluY2lwYWwoe1xuICAgICAgZ3JhbnRlZSxcbiAgICAgIGFjdGlvbnMsXG4gICAgICByZXNvdXJjZUFybnM6IFt0aGlzLmdyb3VwQXJuXSxcbiAgICAgIHNjb3BlOiB0aGlzLFxuICAgIH0pO1xuICB9XG5cbiAgcHJpdmF0ZSBhcm5Gb3JTY2hlZHVsZUluR3JvdXAoc2NoZWR1bGVOYW1lOiBzdHJpbmcpOiBzdHJpbmcge1xuICAgIHJldHVybiBBcm4uZm9ybWF0KHtcbiAgICAgIHJlZ2lvbjogdGhpcy5lbnYucmVnaW9uLFxuICAgICAgYWNjb3VudDogdGhpcy5lbnYuYWNjb3VudCxcbiAgICAgIHBhcnRpdGlvbjogQXdzLlBBUlRJVElPTixcbiAgICAgIHNlcnZpY2U6ICdzY2hlZHVsZXInLFxuICAgICAgcmVzb3VyY2U6ICdzY2hlZHVsZScsXG4gICAgICByZXNvdXJjZU5hbWU6IHRoaXMuZ3JvdXBOYW1lICsgJy8nICsgc2NoZWR1bGVOYW1lLFxuICAgIH0pO1xuICB9XG5cbiAgLyoqXG4gICAqIEdyYW50IGxpc3QgYW5kIGdldCBzY2hlZHVsZSBwZXJtaXNzaW9ucyBmb3Igc2NoZWR1bGVzIGluIHRoaXMgZ3JvdXAgdG8gdGhlIGdpdmVuIHByaW5jaXBhbFxuICAgKi9cbiAgcHVibGljIGdyYW50UmVhZFNjaGVkdWxlcyhpZGVudGl0eTogaWFtLklHcmFudGFibGUpIHtcbiAgICByZXR1cm4gaWFtLkdyYW50LmFkZFRvUHJpbmNpcGFsKHtcbiAgICAgIGdyYW50ZWU6IGlkZW50aXR5LFxuICAgICAgYWN0aW9uczogWydzY2hlZHVsZXI6R2V0U2NoZWR1bGUnLCAnc2NoZWR1bGVyOkxpc3RTY2hlZHVsZXMnXSxcbiAgICAgIHJlc291cmNlQXJuczogW3RoaXMuYXJuRm9yU2NoZWR1bGVJbkdyb3VwKCcqJyldLFxuICAgICAgc2NvcGU6IHRoaXMsXG4gICAgfSk7XG4gIH1cblxuICAvKipcbiAgICogR3JhbnQgY3JlYXRlIGFuZCB1cGRhdGUgc2NoZWR1bGUgcGVybWlzc2lvbnMgZm9yIHNjaGVkdWxlcyBpbiB0aGlzIGdyb3VwIHRvIHRoZSBnaXZlbiBwcmluY2lwYWxcbiAgICovXG4gIHB1YmxpYyBncmFudFdyaXRlU2NoZWR1bGVzKGlkZW50aXR5OiBpYW0uSUdyYW50YWJsZSk6IGlhbS5HcmFudCB7XG4gICAgcmV0dXJuIGlhbS5HcmFudC5hZGRUb1ByaW5jaXBhbCh7XG4gICAgICBncmFudGVlOiBpZGVudGl0eSxcbiAgICAgIGFjdGlvbnM6IFsnc2NoZWR1bGVyOkNyZWF0ZVNjaGVkdWxlJywgJ3NjaGVkdWxlcjpVcGRhdGVTY2hlZHVsZSddLFxuICAgICAgcmVzb3VyY2VBcm5zOiBbdGhpcy5hcm5Gb3JTY2hlZHVsZUluR3JvdXAoJyonKV0sXG4gICAgICBzY29wZTogdGhpcyxcbiAgICB9KTtcbiAgfVxuXG4gIC8qKlxuICAgKiBHcmFudCBkZWxldGUgc2NoZWR1bGUgcGVybWlzc2lvbiBmb3Igc2NoZWR1bGVzIGluIHRoaXMgZ3JvdXAgdG8gdGhlIGdpdmVuIHByaW5jaXBhbFxuICAgKi9cbiAgcHVibGljIGdyYW50RGVsZXRlU2NoZWR1bGVzKGlkZW50aXR5OiBpYW0uSUdyYW50YWJsZSk6IGlhbS5HcmFudCB7XG4gICAgcmV0dXJuIGlhbS5HcmFudC5hZGRUb1ByaW5jaXBhbCh7XG4gICAgICBncmFudGVlOiBpZGVudGl0eSxcbiAgICAgIGFjdGlvbnM6IFsnc2NoZWR1bGVyOkRlbGV0ZVNjaGVkdWxlJ10sXG4gICAgICByZXNvdXJjZUFybnM6IFt0aGlzLmFybkZvclNjaGVkdWxlSW5Hcm91cCgnKicpXSxcbiAgICAgIHNjb3BlOiB0aGlzLFxuICAgIH0pO1xuICB9XG59XG4vKipcbiAqIEByZXNvdXJjZSBBV1M6OlNjaGVkdWxlcjo6U2NoZWR1bGVHcm91cFxuICovXG5leHBvcnQgY2xhc3MgR3JvdXAgZXh0ZW5kcyBHcm91cEJhc2Uge1xuICAvKipcbiAgICogSW1wb3J0IGFuIGV4dGVybmFsIGdyb3VwIGJ5IEFSTi5cbiAgICpcbiAgICogQHBhcmFtIHNjb3BlIGNvbnN0cnVjdCBzY29wZVxuICAgKiBAcGFyYW0gaWQgY29uc3RydWN0IGlkXG4gICAqIEBwYXJhbSBncm91cEFybiB0aGUgQVJOIG9mIHRoZSBncm91cCB0byBpbXBvcnQgKGUuZy4gYGFybjphd3M6c2NoZWR1bGVyOnJlZ2lvbjphY2NvdW50LWlkOnNjaGVkdWxlLWdyb3VwL2dyb3VwLW5hbWVgKVxuICAgKi9cbiAgcHVibGljIHN0YXRpYyBmcm9tR3JvdXBBcm4oc2NvcGU6IENvbnN0cnVjdCwgaWQ6IHN0cmluZywgZ3JvdXBBcm46IHN0cmluZyk6IElHcm91cCB7XG4gICAgY29uc3QgYXJuQ29tcG9uZW50cyA9IFN0YWNrLm9mKHNjb3BlKS5zcGxpdEFybihncm91cEFybiwgQXJuRm9ybWF0LlNMQVNIX1JFU09VUkNFX05BTUUpO1xuICAgIGNvbnN0IGdyb3VwTmFtZSA9IGFybkNvbXBvbmVudHMucmVzb3VyY2VOYW1lITtcbiAgICBjbGFzcyBJbXBvcnQgZXh0ZW5kcyBHcm91cEJhc2Uge1xuICAgICAgZ3JvdXBOYW1lID0gZ3JvdXBOYW1lO1xuICAgICAgZ3JvdXBBcm4gPSBncm91cEFybjtcbiAgICB9XG4gICAgcmV0dXJuIG5ldyBJbXBvcnQoc2NvcGUsIGlkKTtcbiAgfVxuXG4gIC8qKlxuICAgKiBJbXBvcnQgYSBkZWZhdWx0IHNjaGVkdWxlIGdyb3VwLlxuICAgKlxuICAgKiBAcGFyYW0gc2NvcGUgY29uc3RydWN0IHNjb3BlXG4gICAqIEBwYXJhbSBpZCBjb25zdHJ1Y3QgaWRcbiAgICovXG4gIHB1YmxpYyBzdGF0aWMgZnJvbURlZmF1bHRHcm91cChzY29wZTogQ29uc3RydWN0LCBpZDogc3RyaW5nKTogSUdyb3VwIHtcbiAgICByZXR1cm4gR3JvdXAuZnJvbUdyb3VwTmFtZShzY29wZSwgaWQsICdkZWZhdWx0Jyk7XG4gIH1cblxuICAvKipcbiAgICogSW1wb3J0IGFuIGV4aXN0aW5nIGdyb3VwIHdpdGggYSBnaXZlbiBuYW1lLlxuICAgKlxuICAgKiBAcGFyYW0gc2NvcGUgY29uc3RydWN0IHNjb3BlXG4gICAqIEBwYXJhbSBpZCBjb25zdHJ1Y3QgaWRcbiAgICogQHBhcmFtIGdyb3VwTmFtZSB0aGUgbmFtZSBvZiB0aGUgZXhpc3RpbmcgZ3JvdXAgdG8gaW1wb3J0XG4gICAqL1xuICBwdWJsaWMgc3RhdGljIGZyb21Hcm91cE5hbWUoc2NvcGU6IENvbnN0cnVjdCwgaWQ6IHN0cmluZywgZ3JvdXBOYW1lOiBzdHJpbmcpOiBJR3JvdXAge1xuICAgIGNvbnN0IGdyb3VwQXJuID0gU3RhY2sub2Yoc2NvcGUpLmZvcm1hdEFybih7XG4gICAgICBzZXJ2aWNlOiAnc2NoZWR1bGVyJyxcbiAgICAgIHJlc291cmNlOiAnc2NoZWR1bGUtZ3JvdXAnLFxuICAgICAgcmVzb3VyY2VOYW1lOiBncm91cE5hbWUsXG4gICAgfSk7XG4gICAgcmV0dXJuIEdyb3VwLmZyb21Hcm91cEFybihzY29wZSwgaWQsIGdyb3VwQXJuKTtcbiAgfVxuXG4gIHB1YmxpYyByZWFkb25seSBncm91cE5hbWU6IHN0cmluZztcbiAgcHVibGljIHJlYWRvbmx5IGdyb3VwQXJuOiBzdHJpbmc7XG5cbiAgcHVibGljIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBHcm91cFByb3BzKSB7XG4gICAgc3VwZXIoc2NvcGUsIGlkLCB7XG4gICAgICBwaHlzaWNhbE5hbWU6IHByb3BzLmdyb3VwTmFtZSA/PyBQaHlzaWNhbE5hbWUuR0VORVJBVEVfSUZfTkVFREVELFxuICAgIH0pO1xuXG4gICAgY29uc3QgZ3JvdXAgPSBuZXcgQ2ZuU2NoZWR1bGVHcm91cCh0aGlzLCAnUmVzb3VyY2UnLCB7XG4gICAgICBuYW1lOiB0aGlzLnBoeXNpY2FsTmFtZSxcbiAgICB9KTtcblxuICAgIGdyb3VwLmFwcGx5UmVtb3ZhbFBvbGljeShwcm9wcy5yZW1vdmFsUG9saWN5KTtcblxuICAgIHRoaXMuZ3JvdXBBcm4gPSB0aGlzLmdldFJlc291cmNlQXJuQXR0cmlidXRlKGdyb3VwLmF0dHJBcm4sIHtcbiAgICAgIHNlcnZpY2U6ICdzY2hlZHVsZXInLFxuICAgICAgcmVzb3VyY2U6ICdzY2hlZHVsZS1ncm91cCcsXG4gICAgICByZXNvdXJjZU5hbWU6IHRoaXMucGh5c2ljYWxOYW1lLFxuICAgIH0pO1xuICAgIHRoaXMuZ3JvdXBOYW1lID0gdGhpcy5waHlzaWNhbE5hbWU7XG4gIH1cbn0iXX0=
```

##### package/lib/input.js

###### js-beautify {}

```diff
@@ -36,15 +36,15 @@
     }
     constructor() {}
 }
 exports.ScheduleTargetInput = ScheduleTargetInput;
 _a = JSII_RTTI_SYMBOL_1;
 ScheduleTargetInput[_a] = {
     fqn: "@aws-cdk/aws-scheduler-alpha.ScheduleTargetInput",
-    version: "2.99.0-alpha.0"
+    version: "2.99.1-alpha.0"
 };
 class FieldAwareEventInput extends ScheduleTargetInput {
     constructor(input) {
         super();
         this.input = input;
     }
     bind(schedule) {
@@ -114,10 +114,10 @@
         return `<aws.scheduler.${this.name}>`;
     }
 }
 exports.ContextAttribute = ContextAttribute;
 _b = JSII_RTTI_SYMBOL_1;
 ContextAttribute[_b] = {
     fqn: "@aws-cdk/aws-scheduler-alpha.ContextAttribute",
-    version: "2.99.0-alpha.0"
+    version: "2.99.1-alpha.0"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5wdXQuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyJpbnB1dC50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7OztBQUFBLDZDQUE4RztBQUc5Rzs7R0FFRztBQUNILE1BQXNCLG1CQUFtQjtJQUN2Qzs7Ozs7Ozs7Ozs7T0FXRztJQUNJLE1BQU0sQ0FBQyxRQUFRLENBQUMsSUFBWTtRQUNqQyxPQUFPLElBQUksb0JBQW9CLENBQUMsSUFBSSxDQUFDLENBQUM7S0FDdkM7SUFFRDs7Ozs7T0FLRztJQUNJLE1BQU0sQ0FBQyxVQUFVLENBQUMsR0FBUTtRQUMvQixPQUFPLElBQUksb0JBQW9CLENBQUMsR0FBRyxDQUFDLENBQUM7S0FDdEM7SUFFRDtLQUNDOztBQTVCSCxrREFrQ0M7OztBQUVELE1BQU0sb0JBQXFCLFNBQVEsbUJBQW1CO0lBQ3BELFlBQTZCLEtBQVU7UUFDckMsS0FBSyxFQUFFLENBQUM7UUFEbUIsVUFBSyxHQUFMLEtBQUssQ0FBSztLQUV0QztJQUVNLElBQUksQ0FBQyxRQUFtQjtRQUM3QixNQUFNLFFBQVMsU0FBUSxrQ0FBb0I7WUFDekM7Z0JBQ0UsS0FBSyxDQUFDLElBQUksMEJBQVksRUFBRSxDQUFDLENBQUM7WUFDNUIsQ0FBQztZQUVNLFlBQVksQ0FBQyxDQUFRLEVBQUUsUUFBeUI7Z0JBQ3JELE9BQU8sbUJBQUssQ0FBQyxRQUFRLENBQUMsQ0FBQyxDQUFDLENBQUM7WUFDM0IsQ0FBQztTQUNGO1FBRUQsTUFBTSxLQUFLLEdBQUcsbUJBQUssQ0FBQyxFQUFFLENBQUMsUUFBUSxDQUFDLENBQUM7UUFDakMsT0FBTyxLQUFLLENBQUMsWUFBWSxDQUFDLDBCQUFZLENBQUMsT0FBTyxDQUFDLElBQUksQ0FBQyxLQUFLLEVBQUU7WUFDekQsS0FBSyxFQUFFLFFBQVE7WUFDZixRQUFRLEVBQUUsSUFBSSxRQUFRLEVBQUU7U0FDekIsQ0FBQyxDQUFDLENBQUM7S0FDTDtDQUNGO0FBRUQ7Ozs7R0FJRztBQUNILE1BQWEsZ0JBQWdCO0lBQzNCOztPQUVHO0lBQ0ksTUFBTSxLQUFLLFdBQVc7UUFDM0IsT0FBTyxJQUFJLENBQUMsUUFBUSxDQUFDLGNBQWMsQ0FBQyxDQUFDO0tBQ3RDO0lBRUQ7OztPQUdHO0lBQ0ksTUFBTSxLQUFLLGFBQWE7UUFDN0IsT0FBTyxJQUFJLENBQUMsUUFBUSxDQUFDLGdCQUFnQixDQUFDLENBQUM7S0FDeEM7SUFFRDs7O09BR0c7SUFDSSxNQUFNLEtBQUssV0FBVztRQUMzQixPQUFPLElBQUksQ0FBQyxRQUFRLENBQUMsY0FBYyxDQUFDLENBQUM7S0FDdEM7SUFFRDs7O09BR0c7SUFDSSxNQUFNLEtBQUssYUFBYTtRQUM3QixPQUFPLElBQUksQ0FBQyxRQUFRLENBQUMsZ0JBQWdCLENBQUMsQ0FBQztLQUN4QztJQUVEOzs7O09BSUc7SUFDSSxNQUFNLENBQUMsUUFBUSxDQUFDLElBQVk7UUFDakMsT0FBTyxJQUFJLGdCQUFnQixDQUFDLElBQUksQ0FBQyxDQUFDLFFBQVEsRUFBRSxDQUFDO0tBQzlDO0lBRUQsWUFBb0MsSUFBWTtRQUFaLFNBQUksR0FBSixJQUFJLENBQVE7S0FDL0M7SUFFRDs7T0FFRztJQUNJLFFBQVE7UUFDYixPQUFPLGtCQUFrQixJQUFJLENBQUMsSUFBSSxHQUFHLENBQUM7S0FDdkM7O0FBakRILDRDQWtEQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IERlZmF1bHRUb2tlblJlc29sdmVyLCBJUmVzb2x2ZUNvbnRleHQsIFN0YWNrLCBTdHJpbmdDb25jYXQsIFRva2VuLCBUb2tlbml6YXRpb24gfSBmcm9tICdhd3MtY2RrLWxpYic7XG5pbXBvcnQgeyBJU2NoZWR1bGUgfSBmcm9tICcuL3NjaGVkdWxlJztcblxuLyoqXG4gKiBUaGUgdGV4dCwgb3Igd2VsbC1mb3JtZWQgSlNPTiwgcGFzc2VkIHRvIHRoZSB0YXJnZXQgb2YgdGhlIHNjaGVkdWxlLlxuICovXG5leHBvcnQgYWJzdHJhY3QgY2xhc3MgU2NoZWR1bGVUYXJnZXRJbnB1dCB7XG4gIC8qKlxuICAgKiBQYXNzIHRleHQgdG8gdGhlIHRhcmdldCwgaXQgaXMgcG9zc2libGUgdG8gZW1iZWQgYENvbnRleHRBdHRyaWJ1dGVzYFxuICAgKiB0aGF0IHdpbGwgYmUgcmVzb2x2ZWQgdG8gYWN0dWFsIHZhbHVlcyB3aGlsZSB0aGUgQ2xvdWRGb3JtYXRpb24gaXNcbiAgICogZGVwbG95ZWQgb3IgY2RrIFRva2VucyB0aGF0IHdpbGwgYmUgcmVzb2x2ZWQgd2hlbiB0aGUgQ2xvdWRGb3JtYXRpb25cbiAgICogdGVtcGxhdGVzIGFyZSBnZW5lcmF0ZWQgYnkgQ0RLLlxuICAgKlxuICAgKiBUaGUgdGFyZ2V0IGlucHV0IHZhbHVlIHdpbGwgYmUgYSBzaW5nbGUgc3RyaW5nIHRoYXQgeW91IHBhc3MuXG4gICAqIEZvciBwYXNzaW5nIGNvbXBsZXggdmFsdWVzIGxpa2UgSlNPTiBvYmplY3QgdG8gYSB0YXJnZXQgdXNlIG1ldGhvZFxuICAgKiBgU2NoZWR1bGVUYXJnZXRJbnB1dC5mcm9tT2JqZWN0KClgIGluc3RlYWQuXG4gICAqXG4gICAqIEBwYXJhbSB0ZXh0IFRleHQgdG8gdXNlIGFzIHRoZSBpbnB1dCBmb3IgdGhlIHRhcmdldFxuICAgKi9cbiAgcHVibGljIHN0YXRpYyBmcm9tVGV4dCh0ZXh0OiBzdHJpbmcpOiBTY2hlZHVsZVRhcmdldElucHV0IHtcbiAgICByZXR1cm4gbmV3IEZpZWxkQXdhcmVFdmVudElucHV0KHRleHQpO1xuICB9XG5cbiAgLyoqXG4gICAqIFBhc3MgYSBKU09OIG9iamVjdCB0byB0aGUgdGFyZ2V0LCBpdCBpcyBwb3NzaWJsZSB0byBlbWJlZCBgQ29udGV4dEF0dHJpYnV0ZXNgIGFuZCBvdGhlclxuICAgKiBjZGsgcmVmZXJlbmNlcy5cbiAgICpcbiAgICogQHBhcmFtIG9iaiBvYmplY3QgdG8gdXNlIHRvIGNvbnZlcnQgdG8gSlNPTiB0byB1c2UgYXMgaW5wdXQgZm9yIHRoZSB0YXJnZXRcbiAgICovXG4gIHB1YmxpYyBzdGF0aWMgZnJvbU9iamVjdChvYmo6IGFueSk6IFNjaGVkdWxlVGFyZ2V0SW5wdXQge1xuICAgIHJldHVybiBuZXcgRmllbGRBd2FyZUV2ZW50SW5wdXQob2JqKTtcbiAgfVxuXG4gIHByb3RlY3RlZCBjb25zdHJ1Y3RvcigpIHtcbiAgfVxuXG4gIC8qKlxuICAgKiBSZXR1cm4gdGhlIGlucHV0IHByb3BlcnRpZXMgZm9yIHRoaXMgaW5wdXQgb2JqZWN0XG4gICAqL1xuICBwdWJsaWMgYWJzdHJhY3QgYmluZChzY2hlZHVsZTogSVNjaGVkdWxlKTogc3RyaW5nO1xufVxuXG5jbGFzcyBGaWVsZEF3YXJlRXZlbnRJbnB1dCBleHRlbmRzIFNjaGVkdWxlVGFyZ2V0SW5wdXQge1xuICBjb25zdHJ1Y3Rvcihwcml2YXRlIHJlYWRvbmx5IGlucHV0OiBhbnkpIHtcbiAgICBzdXBlcigpO1xuICB9XG5cbiAgcHVibGljIGJpbmQoc2NoZWR1bGU6IElTY2hlZHVsZSk6IHN0cmluZyB7XG4gICAgY2xhc3MgUmVwbGFjZXIgZXh0ZW5kcyBEZWZhdWx0VG9rZW5SZXNvbHZlciB7XG4gICAgICBjb25zdHJ1Y3RvcigpIHtcbiAgICAgICAgc3VwZXIobmV3IFN0cmluZ0NvbmNhdCgpKTtcbiAgICAgIH1cblxuICAgICAgcHVibGljIHJlc29sdmVUb2tlbih0OiBUb2tlbiwgX2NvbnRleHQ6IElSZXNvbHZlQ29udGV4dCkge1xuICAgICAgICByZXR1cm4gVG9rZW4uYXNTdHJpbmcodCk7XG4gICAgICB9XG4gICAgfVxuXG4gICAgY29uc3Qgc3RhY2sgPSBTdGFjay5vZihzY2hlZHVsZSk7XG4gICAgcmV0dXJuIHN0YWNrLnRvSnNvblN0cmluZyhUb2tlbml6YXRpb24ucmVzb2x2ZSh0aGlzLmlucHV0LCB7XG4gICAgICBzY29wZTogc2NoZWR1bGUsXG4gICAgICByZXNvbHZlcjogbmV3IFJlcGxhY2VyKCksXG4gICAgfSkpO1xuICB9XG59XG5cbi8qKlxuICogUmVwcmVzZW50cyBhIGZpZWxkIGluIHRoZSBldmVudCBwYXR0ZXJuXG4gKlxuICogQHNlZSBodHRwczovL2RvY3MuYXdzLmFtYXpvbi5jb20vc2NoZWR1bGVyL2xhdGVzdC9Vc2VyR3VpZGUvbWFuYWdpbmctc2NoZWR1bGUtY29udGV4dC1hdHRyaWJ1dGVzLmh0bWxcbiAqL1xuZXhwb3J0IGNsYXNzIENvbnRleHRBdHRyaWJ1dGUge1xuICAvKipcbiAgICogVGhlIEFSTiBvZiB0aGUgc2NoZWR1bGUuXG4gICAqL1xuICBwdWJsaWMgc3RhdGljIGdldCBzY2hlZHVsZUFybigpOiBzdHJpbmcge1xuICAgIHJldHVybiB0aGlzLmZyb21OYW1lKCdzY2hlZHVsZS1hcm4nKTtcbiAgfVxuXG4gIC8qKlxuICAgKiBUaGUgdGltZSB5b3Ugc3BlY2lmaWVkIGZvciB0aGUgc2NoZWR1bGUgdG8gaW52b2tlIGl0cyB0YXJnZXQsIGZvciBleGFtcGxlLFxuICAgKiAyMDIyLTAzLTIyVDE4OjU5OjQzWi5cbiAgICovXG4gIHB1YmxpYyBzdGF0aWMgZ2V0IHNjaGVkdWxlZFRpbWUoKTogc3RyaW5nIHtcbiAgICByZXR1cm4gdGhpcy5mcm9tTmFtZSgnc2NoZWR1bGVkLXRpbWUnKTtcbiAgfVxuXG4gIC8qKlxuICAgKiBUaGUgdW5pcXVlIElEIHRoYXQgRXZlbnRCcmlkZ2UgU2NoZWR1bGVyIGFzc2lnbnMgZm9yIGVhY2ggYXR0ZW1wdGVkIGludm9jYXRpb24gb2ZcbiAgICogYSB0YXJnZXQsIGZvciBleGFtcGxlLCBkMzJjNWtkZGNmNWJiOGMzLlxuICAgKi9cbiAgcHVibGljIHN0YXRpYyBnZXQgZXhlY3V0aW9uSWQoKTogc3RyaW5nIHtcbiAgICByZXR1cm4gdGhpcy5mcm9tTmFtZSgnZXhlY3V0aW9uLWlkJyk7XG4gIH1cblxuICAvKipcbiAgICogQSBjb3VudGVyIHRoYXQgaWRlbnRpZmllcyB0aGUgYXR0ZW1wdCBudW1iZXIgZm9yIHRoZSBjdXJyZW50IGludm9jYXRpb24sIGZvclxuICAgKiBleGFtcGxlLCAxLlxuICAgKi9cbiAgcHVibGljIHN0YXRpYyBnZXQgYXR0ZW1wdE51bWJlcigpOiBzdHJpbmcge1xuICAgIHJldHVybiB0aGlzLmZyb21OYW1lKCdhdHRlbXB0LW51bWJlcicpO1xuICB9XG5cbiAgLyoqXG4gICAqIEVzY2FwZSBoYXRjaCBmb3Igb3RoZXIgQ29udGV4dEF0dHJpYnV0ZSB0aGF0IG1pZ2h0IGJlIHJlc29sdmVkIGluIGZ1dHVyZS5cbiAgICpcbiAgICogQHBhcmFtIG5hbWUgLSBuYW1lIHdpbGwgcmVwbGFjZSB4eHggaW4gPGF3cy5zY2hlZHVsZXIueHh4PlxuICAgKi9cbiAgcHVibGljIHN0YXRpYyBmcm9tTmFtZShuYW1lOiBzdHJpbmcpOiBzdHJpbmcge1xuICAgIHJldHVybiBuZXcgQ29udGV4dEF0dHJpYnV0ZShuYW1lKS50b1N0cmluZygpO1xuICB9XG5cbiAgcHJpdmF0ZSBjb25zdHJ1Y3RvcihwdWJsaWMgcmVhZG9ubHkgbmFtZTogc3RyaW5nKSB7XG4gIH1cblxuICAvKipcbiAgICogQ29udmVydCB0aGUgcGF0aCB0byB0aGUgZmllbGQgaW4gdGhlIGV2ZW50IHBhdHRlcm4gdG8gSlNPTlxuICAgKi9cbiAgcHVibGljIHRvU3RyaW5nKCkge1xuICAgIHJldHVybiBgPGF3cy5zY2hlZHVsZXIuJHt0aGlzLm5hbWV9PmA7XG4gIH1cbn1cbiJdfQ==
```

##### package/lib/schedule-expression.js

###### js-beautify {}

```diff
@@ -72,15 +72,15 @@
     }
     constructor() {}
 }
 exports.ScheduleExpression = ScheduleExpression;
 _a = JSII_RTTI_SYMBOL_1;
 ScheduleExpression[_a] = {
     fqn: "@aws-cdk/aws-scheduler-alpha.ScheduleExpression",
-    version: "2.99.0-alpha.0"
+    version: "2.99.1-alpha.0"
 };
 const DEFAULT_TIMEZONE = core_1.TimeZone.ETC_UTC;
 class LiteralScheduleExpression extends ScheduleExpression {
     constructor(expressionString, timeZone = DEFAULT_TIMEZONE) {
         super();
         this.expressionString = expressionString;
         this.timeZone = timeZone;
```

##### package/lib/schedule.js

###### js-beautify {}

```diff
@@ -56,10 +56,10 @@
         });
     }
 }
 exports.Schedule = Schedule;
 _a = JSII_RTTI_SYMBOL_1;
 Schedule[_a] = {
     fqn: "@aws-cdk/aws-scheduler-alpha.Schedule",
-    version: "2.99.0-alpha.0"
+    version: "2.99.1-alpha.0"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoic2NoZWR1bGUuanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyJzY2hlZHVsZS50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiOzs7Ozs7QUFBQSw2Q0FBa0Q7QUFDbEQsNkRBQXdEO0FBcUV4RDs7R0FFRztBQUNILE1BQWEsUUFBUyxTQUFRLHNCQUFRO0lBY3BDLFlBQVksS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBb0I7UUFDNUQsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLEVBQUU7WUFDZixZQUFZLEVBQUUsS0FBSyxDQUFDLFlBQVk7U0FDakMsQ0FBQyxDQUFDOzs7Ozs7K0NBakJNLFFBQVE7Ozs7UUFtQmpCLElBQUksQ0FBQyxLQUFLLEdBQUcsS0FBSyxDQUFDLEtBQUssQ0FBQztRQUV6QixNQUFNLFlBQVksR0FBRyxLQUFLLENBQUMsTUFBTSxDQUFDLElBQUksQ0FBQyxJQUFJLENBQUMsQ0FBQztRQUU3QyxNQUFNLFFBQVEsR0FBRyxJQUFJLDJCQUFXLENBQUMsSUFBSSxFQUFFLFVBQVUsRUFBRTtZQUNqRCxJQUFJLEVBQUUsSUFBSSxDQUFDLFlBQVk7WUFDdkIsa0JBQWtCLEVBQUUsRUFBRSxJQUFJLEVBQUUsS0FBSyxFQUFFO1lBQ25DLGtCQUFrQixFQUFFLEtBQUssQ0FBQyxRQUFRLENBQUMsZ0JBQWdCO1lBQ25ELDBCQUEwQixFQUFFLEtBQUssQ0FBQyxRQUFRLENBQUMsUUFBUSxFQUFFLFlBQVk7WUFDakUsU0FBUyxFQUFFLElBQUksQ0FBQyxLQUFLLEVBQUUsU0FBUztZQUNoQyxLQUFLLEVBQUUsQ0FBQyxLQUFLLENBQUMsT0FBTyxJQUFJLElBQUksQ0FBQyxDQUFDLENBQUMsQ0FBQyxTQUFTLENBQUMsQ0FBQyxDQUFDLFVBQVU7WUFDdkQsTUFBTSxFQUFFO2dCQUNOLEdBQUcsRUFBRSxZQUFZLENBQUMsR0FBRztnQkFDckIsT0FBTyxFQUFFLFlBQVksQ0FBQyxJQUFJLENBQUMsT0FBTztnQkFDbEMsS0FBSyxFQUFFLFlBQVksQ0FBQyxLQUFLLEVBQUUsSUFBSSxDQUFDLElBQUksQ0FBQztnQkFDckMsZ0JBQWdCLEVBQUUsWUFBWSxDQUFDLGdCQUFnQjtnQkFDL0MsV0FBVyxFQUFFLFlBQVksQ0FBQyxXQUFXO2dCQUNyQyxhQUFhLEVBQUUsWUFBWSxDQUFDLGFBQWE7Z0JBQ3pDLGlCQUFpQixFQUFFLFlBQVksQ0FBQyxpQkFBaUI7Z0JBQ2pELHFCQUFxQixFQUFFLFlBQVksQ0FBQyxxQkFBcUI7Z0JBQ3pELDJCQUEyQixFQUFFLFlBQVksQ0FBQywyQkFBMkI7Z0JBQ3JFLGFBQWEsRUFBRSxZQUFZLENBQUMsYUFBYTthQUMxQztTQUNGLENBQUMsQ0FBQztRQUVILElBQUksQ0FBQyxZQUFZLEdBQUcsSUFBSSxDQUFDLHdCQUF3QixDQUFDLFFBQVEsQ0FBQyxHQUFHLENBQUMsQ0FBQztRQUNoRSxJQUFJLENBQUMsV0FBVyxHQUFHLElBQUksQ0FBQyx1QkFBdUIsQ0FBQyxRQUFRLENBQUMsT0FBTyxFQUFFO1lBQ2hFLE9BQU8sRUFBRSxXQUFXO1lBQ3BCLFFBQVEsRUFBRSxVQUFVO1lBQ3BCLFlBQVksRUFBRSxHQUFHLElBQUksQ0FBQyxLQUFLLEVBQUUsU0FBUyxJQUFJLFNBQVMsSUFBSSxJQUFJLENBQUMsWUFBWSxFQUFFO1NBQzNFLENBQUMsQ0FBQztLQUNKOztBQWxESCw0QkFtREMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgeyBJUmVzb3VyY2UsIFJlc291cmNlIH0gZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0IHsgQ2ZuU2NoZWR1bGUgfSBmcm9tICdhd3MtY2RrLWxpYi9hd3Mtc2NoZWR1bGVyJztcbmltcG9ydCB7IENvbnN0cnVjdCB9IGZyb20gJ2NvbnN0cnVjdHMnO1xuaW1wb3J0IHsgSUdyb3VwIH0gZnJvbSAnLi9ncm91cCc7XG5pbXBvcnQgeyBTY2hlZHVsZUV4cHJlc3Npb24gfSBmcm9tICcuL3NjaGVkdWxlLWV4cHJlc3Npb24nO1xuaW1wb3J0IHsgSVNjaGVkdWxlVGFyZ2V0IH0gZnJvbSAnLi90YXJnZXQnO1xuXG4vKipcbiAqIEludGVyZmFjZSByZXByZXNlbnRpbmcgYSBjcmVhdGVkIG9yIGFuIGltcG9ydGVkIGBTY2hlZHVsZWAuXG4gKi9cbmV4cG9ydCBpbnRlcmZhY2UgSVNjaGVkdWxlIGV4dGVuZHMgSVJlc291cmNlIHtcbiAgLyoqXG4gICAqIFRoZSBuYW1lIG9mIHRoZSBzY2hlZHVsZS5cbiAgICovXG4gIHJlYWRvbmx5IHNjaGVkdWxlTmFtZTogc3RyaW5nO1xuICAvKipcbiAgICogVGhlIHNjaGVkdWxlIGdyb3VwIGFzc29jaWF0ZWQgd2l0aCB0aGlzIHNjaGVkdWxlLlxuICAgKi9cbiAgcmVhZG9ubHkgZ3JvdXA/OiBJR3JvdXA7XG4gIC8qKlxuICAgKiBUaGUgYXJuIG9mIHRoZSBzY2hlZHVsZS5cbiAgICovXG4gIHJlYWRvbmx5IHNjaGVkdWxlQXJuOiBzdHJpbmc7XG59XG5cbi8qKlxuICogQ29uc3RydWN0aW9uIHByb3BlcnRpZXMgZm9yIGBTY2hlZHVsZWAuXG4gKi9cbmV4cG9ydCBpbnRlcmZhY2UgU2NoZWR1bGVQcm9wcyB7XG4gIC8qKlxuICAgKiBUaGUgZXhwcmVzc2lvbiB0aGF0IGRlZmluZXMgd2hlbiB0aGUgc2NoZWR1bGUgcnVucy4gQ2FuIGJlIGVpdGhlciBhIGBhdGAsIGByYXRlYFxuICAgKiBvciBgY3JvbmAgZXhwcmVzc2lvbi5cbiAgICovXG4gIHJlYWRvbmx5IHNjaGVkdWxlOiBTY2hlZHVsZUV4cHJlc3Npb247XG5cbiAgLyoqXG4gICAqIFRoZSBzY2hlZHVsZSdzIHRhcmdldCBkZXRhaWxzLlxuICAgKi9cbiAgcmVhZG9ubHkgdGFyZ2V0OiBJU2NoZWR1bGVUYXJnZXQ7XG5cbiAgLyoqXG4gICAqIFRoZSBuYW1lIG9mIHRoZSBzY2hlZHVsZS5cbiAgICpcbiAgICogVXAgdG8gNjQgbGV0dGVycyAodXBwZXJjYXNlIGFuZCBsb3dlcmNhc2UpLCBudW1iZXJzLCBoeXBoZW5zLCB1bmRlcnNjb3JlcyBhbmQgZG90cyBhcmUgYWxsb3dlZC5cbiAgICpcbiAgICogQGRlZmF1bHQgLSBBIHVuaXF1ZSBuYW1lIHdpbGwgYmUgZ2VuZXJhdGVkXG4gICAqL1xuICByZWFkb25seSBzY2hlZHVsZU5hbWU/OiBzdHJpbmc7XG5cbiAgLyoqXG4gICAqIFRoZSBkZXNjcmlwdGlvbiB5b3Ugc3BlY2lmeSBmb3IgdGhlIHNjaGVkdWxlLlxuICAgKlxuICAgKiBAZGVmYXVsdCAtIG5vIHZhbHVlXG4gICAqL1xuICByZWFkb25seSBkZXNjcmlwdGlvbj86IHN0cmluZztcblxuICAvKipcbiAgICogVGhlIHNjaGVkdWxlJ3MgZ3JvdXAuXG4gICAqXG4gICAqIEBkZWZhdWx0IC0gQnkgZGVmYXVsdCBhIHNjaGVkdWxlIHdpbGwgYmUgYXNzb2NpYXRlZCB3aXRoIHRoZSBgZGVmYXVsdGAgZ3JvdXAuXG4gICAqL1xuICByZWFkb25seSBncm91cD86IElHcm91cDtcblxuICAvKipcbiAgICogSW5kaWNhdGVzIHdoZXRoZXIgdGhlIHNjaGVkdWxlIGlzIGVuYWJsZWQuXG4gICAqIEBkZWZhdWx0IHRydWVcbiAgICovXG4gIHJlYWRvbmx5IGVuYWJsZWQ/OiBib29sZWFuO1xufVxuXG4vKipcbiAqIEFuIEV2ZW50QnJpZGdlIFNjaGVkdWxlXG4gKi9cbmV4cG9ydCBjbGFzcyBTY2hlZHVsZSBleHRlbmRzIFJlc291cmNlIGltcGxlbWVudHMgSVNjaGVkdWxlIHtcbiAgLyoqXG4gICAqIFRoZSBzY2hlZHVsZSBncm91cCBhc3NvY2lhdGVkIHdpdGggdGhpcyBzY2hlZHVsZS5cbiAgICovXG4gIHB1YmxpYyByZWFkb25seSBncm91cD86IElHcm91cDtcbiAgLyoqXG4gICAqIFRoZSBhcm4gb2YgdGhlIHNjaGVkdWxlLlxuICAgKi9cbiAgcHVibGljIHJlYWRvbmx5IHNjaGVkdWxlQXJuOiBzdHJpbmc7XG4gIC8qKlxuICAgKiBUaGUgbmFtZSBvZiB0aGUgc2NoZWR1bGUuXG4gICAqL1xuICBwdWJsaWMgcmVhZG9ubHkgc2NoZWR1bGVOYW1lOiBzdHJpbmc7XG5cbiAgY29uc3RydWN0b3Ioc2NvcGU6IENvbnN0cnVjdCwgaWQ6IHN0cmluZywgcHJvcHM6IFNjaGVkdWxlUHJvcHMpIHtcbiAgICBzdXBlcihzY29wZSwgaWQsIHtcbiAgICAgIHBoeXNpY2FsTmFtZTogcHJvcHMuc2NoZWR1bGVOYW1lLFxuICAgIH0pO1xuXG4gICAgdGhpcy5ncm91cCA9IHByb3BzLmdyb3VwO1xuXG4gICAgY29uc3QgdGFyZ2V0Q29uZmlnID0gcHJvcHMudGFyZ2V0LmJpbmQodGhpcyk7XG5cbiAgICBjb25zdCByZXNvdXJjZSA9IG5ldyBDZm5TY2hlZHVsZSh0aGlzLCAnUmVzb3VyY2UnLCB7XG4gICAgICBuYW1lOiB0aGlzLnBoeXNpY2FsTmFtZSxcbiAgICAgIGZsZXhpYmxlVGltZVdpbmRvdzogeyBtb2RlOiAnT0ZGJyB9LFxuICAgICAgc2NoZWR1bGVFeHByZXNzaW9uOiBwcm9wcy5zY2hlZHVsZS5leHByZXNzaW9uU3RyaW5nLFxuICAgICAgc2NoZWR1bGVFeHByZXNzaW9uVGltZXpvbmU6IHByb3BzLnNjaGVkdWxlLnRpbWVab25lPy50aW1lem9uZU5hbWUsXG4gICAgICBncm91cE5hbWU6IHRoaXMuZ3JvdXA/Lmdyb3VwTmFtZSxcbiAgICAgIHN0YXRlOiAocHJvcHMuZW5hYmxlZCA/PyB0cnVlKSA/ICdFTkFCTEVEJyA6ICdESVNBQkxFRCcsXG4gICAgICB0YXJnZXQ6IHtcbiAgICAgICAgYXJuOiB0YXJnZXRDb25maWcuYXJuLFxuICAgICAgICByb2xlQXJuOiB0YXJnZXRDb25maWcucm9sZS5yb2xlQXJuLFxuICAgICAgICBpbnB1dDogdGFyZ2V0Q29uZmlnLmlucHV0Py5iaW5kKHRoaXMpLFxuICAgICAgICBkZWFkTGV0dGVyQ29uZmlnOiB0YXJnZXRDb25maWcuZGVhZExldHRlckNvbmZpZyxcbiAgICAgICAgcmV0cnlQb2xpY3k6IHRhcmdldENvbmZpZy5yZXRyeVBvbGljeSxcbiAgICAgICAgZWNzUGFyYW1ldGVyczogdGFyZ2V0Q29uZmlnLmVjc1BhcmFtZXRlcnMsXG4gICAgICAgIGtpbmVzaXNQYXJhbWV0ZXJzOiB0YXJnZXRDb25maWcua2luZXNpc1BhcmFtZXRlcnMsXG4gICAgICAgIGV2ZW50QnJpZGdlUGFyYW1ldGVyczogdGFyZ2V0Q29uZmlnLmV2ZW50QnJpZGdlUGFyYW1ldGVycyxcbiAgICAgICAgc2FnZU1ha2VyUGlwZWxpbmVQYXJhbWV0ZXJzOiB0YXJnZXRDb25maWcuc2FnZU1ha2VyUGlwZWxpbmVQYXJhbWV0ZXJzLFxuICAgICAgICBzcXNQYXJhbWV0ZXJzOiB0YXJnZXRDb25maWcuc3FzUGFyYW1ldGVycyxcbiAgICAgIH0sXG4gICAgfSk7XG5cbiAgICB0aGlzLnNjaGVkdWxlTmFtZSA9IHRoaXMuZ2V0UmVzb3VyY2VOYW1lQXR0cmlidXRlKHJlc291cmNlLnJlZik7XG4gICAgdGhpcy5zY2hlZHVsZUFybiA9IHRoaXMuZ2V0UmVzb3VyY2VBcm5BdHRyaWJ1dGUocmVzb3VyY2UuYXR0ckFybiwge1xuICAgICAgc2VydmljZTogJ3NjaGVkdWxlcicsXG4gICAgICByZXNvdXJjZTogJ3NjaGVkdWxlJyxcbiAgICAgIHJlc291cmNlTmFtZTogYCR7dGhpcy5ncm91cD8uZ3JvdXBOYW1lID8/ICdkZWZhdWx0J30vJHt0aGlzLnBoeXNpY2FsTmFtZX1gLFxuICAgIH0pO1xuICB9XG59Il19
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9650621118012421%*

 * *Differences: {"'devDependencies'": "{'@aws-cdk/cdk-build-tools': '2.99.1-alpha.0', '@aws-cdk/integ-runner': "*

 * *                      "'2.99.1-alpha.0', '@aws-cdk/pkglint': '2.99.1-alpha.0', 'aws-cdk-lib': "*

 * *                      "'2.99.1', '@aws-cdk/integ-tests-alpha': '2.99.1-alpha.0'}",*

 * * "'peerDependencies'": "{'aws-cdk-lib': '2.99.1'}",*

 * * "'version'": "'2.99.1-alpha.0'"}*

```diff
@@ -11,20 +11,20 @@
         "env": {
             "AWSLINT_BASE_CONSTRUCT": true
         }
     },
     "dependencies": {},
     "description": "The CDK Construct Library for Amazon Scheduler",
     "devDependencies": {
-        "@aws-cdk/cdk-build-tools": "2.99.0-alpha.0",
-        "@aws-cdk/integ-runner": "2.99.0-alpha.0",
-        "@aws-cdk/integ-tests-alpha": "2.99.0-alpha.0",
-        "@aws-cdk/pkglint": "2.99.0-alpha.0",
+        "@aws-cdk/cdk-build-tools": "2.99.1-alpha.0",
+        "@aws-cdk/integ-runner": "2.99.1-alpha.0",
+        "@aws-cdk/integ-tests-alpha": "2.99.1-alpha.0",
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
@@ -76,15 +76,15 @@
         "aws-scheduler"
     ],
     "license": "Apache-2.0",
     "main": "lib/index.js",
     "maturity": "experimental",
     "name": "@aws-cdk/aws-scheduler-alpha",
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
@@ -111,9 +111,9 @@
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

### Comparing `aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk.aws_scheduler_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-scheduler-alpha
-Version: 2.99.0a0
+Version: 2.99.1a0
 Summary: The CDK Construct Library for Amazon Scheduler
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-scheduler-alpha-2.99.0a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-scheduler-alpha-2.99.1a0/src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_scheduler_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/requires.txt
 src/aws_cdk.aws_scheduler_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_scheduler_alpha/__init__.py
 src/aws_cdk/aws_scheduler_alpha/py.typed
 src/aws_cdk/aws_scheduler_alpha/_jsii/__init__.py
-src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.99.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_scheduler_alpha/_jsii/aws-scheduler-alpha@2.99.1-alpha.0.jsii.tgz
```

