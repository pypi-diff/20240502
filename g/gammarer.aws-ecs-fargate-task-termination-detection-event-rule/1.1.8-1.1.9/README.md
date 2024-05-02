# Comparing `tmp/gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8.tar.gz` & `tmp/gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8.tar", last modified: Thu Mar 21 18:13:25 2024, max compression
+gzip compressed data, was "gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9.tar", last modified: Thu Mar 28 18:13:44 2024, max compression
```

## Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8.tar` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:13:25.898666 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-21 18:13:15.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-21 18:13:15.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-03-21 18:13:25.898666 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-21 18:13:15.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-21 18:13:15.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 18:13:25.898666 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-03-21 18:13:15.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:13:25.894666 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:13:25.894666 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:13:25.898666 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-03-21 18:13:15.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:13:25.898666 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-21 18:13:15.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18158 2024-03-21 18:13:15.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@1.1.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 18:13:15.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 18:13:25.898666 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-03-21 18:13:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-21 18:13:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 18:13:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-21 18:13:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-21 18:13:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:44.174926 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-28 18:13:32.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-28 18:13:32.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-03-28 18:13:44.174926 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-28 18:13:32.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-28 18:13:32.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 18:13:44.174926 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-03-28 18:13:32.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:44.170926 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:44.170926 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:44.174926 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-03-28 18:13:32.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:44.174926 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-28 18:13:32.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18158 2024-03-28 18:13:32.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@1.1.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:13:32.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:44.170926 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-03-28 18:13:44.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-28 18:13:44.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:13:44.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-28 18:13:44.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 18:13:44.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/LICENSE` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/PKG-INFO` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ecs-fargate-task-termination-detection-event-rule
-Version: 1.1.8
+Version: 1.1.9
 Summary: This an AWS ECS Fargate task termination detection Event Rule.
 Home-page: https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/README.md` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/setup.py` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ecs-fargate-task-termination-detection-event-rule",
-    "version": "1.1.8",
+    "version": "1.1.9",
     "description": "This an AWS ECS Fargate task termination detection Event Rule.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule",
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule._jsii"
     ],
     "package_data": {
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule._jsii": [
-            "aws-ecs-fargate-task-termination-detection-event-rule@1.1.8.jsii.tgz"
+            "aws-ecs-fargate-task-termination-detection-event-rule@1.1.9.jsii.tgz"
         ],
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.95.0, <2.0.0",
+        "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 const rule = new EcsFargateTaskTerminationDetectionEventRule(stack, 'EcsFargateTaskTerminationDetectionEventRule', {
   ruleName: 'example-event-rule',
   description: 'example event rule.',
   clusterArn,
 });
 ```
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ecs-fargate-task-termination-detection-event-rule
-Version: 1.1.8
+Version: 1.1.9
 Summary: This an AWS ECS Fargate task termination detection Event Rule.
 Home-page: https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-1.1.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
-src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@1.1.8.jsii.tgz
+src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@1.1.9.jsii.tgz
```

