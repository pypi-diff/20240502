# Comparing `tmp/mypy_boto3_redshift_serverless-1.34.89.tar.gz` & `tmp/mypy_boto3_redshift_serverless-1.34.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_redshift_serverless-1.34.89.tar", last modified: Mon Apr 22 19:19:12 2024, max compression
+gzip compressed data, was "mypy_boto3_redshift_serverless-1.34.97.tar", last modified: Thu May  2 19:33:16 2024, max compression
```

## Comparing `mypy_boto3_redshift_serverless-1.34.89.tar` & `mypy_boto3_redshift_serverless-1.34.97.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:12.647682 mypy_boto3_redshift_serverless-1.34.89/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-04-22 19:19:12.647682 mypy_boto3_redshift_serverless-1.34.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:12.647682 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45964 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    45961 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    45064 2024-04-22 19:18:36.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    45064 2024-04-22 19:18:36.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:12.647682 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-04-22 19:19:12.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-22 19:19:12.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:12.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:12.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 19:19:12.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 19:19:12.000000 mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:19:12.647682 mypy_boto3_redshift_serverless-1.34.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-22 19:18:35.000000 mypy_boto3_redshift_serverless-1.34.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:16.150128 mypy_boto3_redshift_serverless-1.34.97/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-02 19:33:16.150128 mypy_boto3_redshift_serverless-1.34.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:16.150128 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45994 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45991 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    46298 2024-05-02 19:33:02.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46298 2024-05-02 19:33:02.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 19:33:01.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:16.150128 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-02 19:33:16.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-02 19:33:16.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:33:16.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:33:16.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 19:33:16.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 19:33:16.000000 mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:33:16.150128 mypy_boto3_redshift_serverless-1.34.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-02 19:33:00.000000 mypy_boto3_redshift_serverless-1.34.97/setup.py
```

### Comparing `mypy_boto3_redshift_serverless-1.34.89/LICENSE` & `mypy_boto3_redshift_serverless-1.34.97/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_redshift_serverless-1.34.89/PKG-INFO` & `mypy_boto3_redshift_serverless-1.34.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-serverless
-Version: 1.34.89
-Summary: Type annotations for boto3.RedshiftServerless 1.34.89 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.97
+Summary: Type annotations for boto3.RedshiftServerless 1.34.97 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_redshift_serverless-1.34.89/README.md` & `mypy_boto3_redshift_serverless-1.34.97/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/__init__.py` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/__init__.pyi` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/__main__.py` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RedshiftServerless 1.34.89\n"
-        "Version:         1.34.89\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.RedshiftServerless 1.34.97\n"
+        "Version:         1.34.97\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.89")
+    print("1.34.97")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/client.py` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,17 +78,17 @@
     ListUsageLimitsResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     RestoreFromRecoveryPointResponseTypeDef,
     RestoreFromSnapshotResponseTypeDef,
     RestoreTableFromRecoveryPointResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
-    ScheduleTypeDef,
+    ScheduleUnionTypeDef,
     TagTypeDef,
-    TargetActionTypeDef,
+    TargetActionUnionTypeDef,
     TimestampTypeDef,
     UpdateCustomDomainAssociationResponseTypeDef,
     UpdateEndpointAccessResponseTypeDef,
     UpdateNamespaceResponseTypeDef,
     UpdateScheduledActionResponseTypeDef,
     UpdateSnapshotCopyConfigurationResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
@@ -224,17 +224,17 @@
         """
 
     def create_scheduled_action(
         self,
         *,
         namespaceName: str,
         roleArn: str,
-        schedule: ScheduleTypeDef,
+        schedule: ScheduleUnionTypeDef,
         scheduledActionName: str,
-        targetAction: TargetActionTypeDef,
+        targetAction: TargetActionUnionTypeDef,
         enabled: bool = ...,
         endTime: TimestampTypeDef = ...,
         scheduledActionDescription: str = ...,
         startTime: TimestampTypeDef = ...,
     ) -> CreateScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
@@ -802,18 +802,18 @@
     def update_scheduled_action(
         self,
         *,
         scheduledActionName: str,
         enabled: bool = ...,
         endTime: TimestampTypeDef = ...,
         roleArn: str = ...,
-        schedule: ScheduleTypeDef = ...,
+        schedule: ScheduleUnionTypeDef = ...,
         scheduledActionDescription: str = ...,
         startTime: TimestampTypeDef = ...,
-        targetAction: TargetActionTypeDef = ...,
+        targetAction: TargetActionUnionTypeDef = ...,
     ) -> UpdateScheduledActionResponseTypeDef:
         """
         Updates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.update_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/client/#update_scheduled_action)
         """
```

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/client.pyi` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -78,17 +78,17 @@
     ListUsageLimitsResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     RestoreFromRecoveryPointResponseTypeDef,
     RestoreFromSnapshotResponseTypeDef,
     RestoreTableFromRecoveryPointResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
-    ScheduleTypeDef,
+    ScheduleUnionTypeDef,
     TagTypeDef,
-    TargetActionTypeDef,
+    TargetActionUnionTypeDef,
     TimestampTypeDef,
     UpdateCustomDomainAssociationResponseTypeDef,
     UpdateEndpointAccessResponseTypeDef,
     UpdateNamespaceResponseTypeDef,
     UpdateScheduledActionResponseTypeDef,
     UpdateSnapshotCopyConfigurationResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
@@ -221,17 +221,17 @@
         """
 
     def create_scheduled_action(
         self,
         *,
         namespaceName: str,
         roleArn: str,
-        schedule: ScheduleTypeDef,
+        schedule: ScheduleUnionTypeDef,
         scheduledActionName: str,
-        targetAction: TargetActionTypeDef,
+        targetAction: TargetActionUnionTypeDef,
         enabled: bool = ...,
         endTime: TimestampTypeDef = ...,
         scheduledActionDescription: str = ...,
         startTime: TimestampTypeDef = ...,
     ) -> CreateScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
@@ -799,18 +799,18 @@
     def update_scheduled_action(
         self,
         *,
         scheduledActionName: str,
         enabled: bool = ...,
         endTime: TimestampTypeDef = ...,
         roleArn: str = ...,
-        schedule: ScheduleTypeDef = ...,
+        schedule: ScheduleUnionTypeDef = ...,
         scheduledActionDescription: str = ...,
         startTime: TimestampTypeDef = ...,
-        targetAction: TargetActionTypeDef = ...,
+        targetAction: TargetActionUnionTypeDef = ...,
     ) -> UpdateScheduledActionResponseTypeDef:
         """
         Updates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.update_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/client/#update_scheduled_action)
         """
```

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/literals.py` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/literals.pyi` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/paginator.py` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/paginator.pyi` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/type_defs.py` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,44 +75,46 @@
     "GetUsageLimitRequestRequestTypeDef",
     "GetWorkgroupRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListCustomDomainAssociationsRequestRequestTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListScheduledActionsRequestRequestTypeDef",
+    "ScheduledActionAssociationTypeDef",
     "ListSnapshotCopyConfigurationsRequestRequestTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "RestoreTableFromRecoveryPointRequestRequestTypeDef",
     "RestoreTableFromSnapshotRequestRequestTypeDef",
+    "ScheduleOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCustomDomainAssociationRequestRequestTypeDef",
     "UpdateEndpointAccessRequestRequestTypeDef",
     "UpdateNamespaceRequestRequestTypeDef",
     "UpdateSnapshotCopyConfigurationRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateUsageLimitRequestRequestTypeDef",
     "UpdateWorkgroupRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
+    "CreateSnapshotScheduleActionParametersOutputTypeDef",
     "CreateSnapshotScheduleActionParametersTypeDef",
     "CreateWorkgroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateCustomDomainAssociationResponseTypeDef",
     "GetCredentialsResponseTypeDef",
     "GetCustomDomainAssociationResponseTypeDef",
     "ListCustomDomainAssociationsResponseTypeDef",
-    "ListScheduledActionsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateCustomDomainAssociationResponseTypeDef",
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DeleteSnapshotResponseTypeDef",
     "GetSnapshotResponseTypeDef",
     "ListSnapshotsResponseTypeDef",
@@ -150,20 +152,24 @@
     "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
     "ListScheduledActionsRequestListScheduledActionsPaginateTypeDef",
     "ListSnapshotCopyConfigurationsRequestListSnapshotCopyConfigurationsPaginateTypeDef",
     "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
     "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    "ListScheduledActionsResponseTypeDef",
     "VpcEndpointTypeDef",
+    "TargetActionOutputTypeDef",
     "TargetActionTypeDef",
+    "ScheduleUnionTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
-    "CreateScheduledActionRequestRequestTypeDef",
     "ScheduledActionResponseTypeDef",
+    "CreateScheduledActionRequestRequestTypeDef",
+    "TargetActionUnionTypeDef",
     "UpdateScheduledActionRequestRequestTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
     "UpdateEndpointAccessResponseTypeDef",
     "WorkgroupTypeDef",
@@ -530,14 +536,21 @@
     "ListScheduledActionsRequestRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "namespaceName": NotRequired[str],
         "nextToken": NotRequired[str],
     },
 )
+ScheduledActionAssociationTypeDef = TypedDict(
+    "ScheduledActionAssociationTypeDef",
+    {
+        "namespaceName": NotRequired[str],
+        "scheduledActionName": NotRequired[str],
+    },
+)
 ListSnapshotCopyConfigurationsRequestRequestTypeDef = TypedDict(
     "ListSnapshotCopyConfigurationsRequestRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "namespaceName": NotRequired[str],
         "nextToken": NotRequired[str],
     },
@@ -636,14 +649,21 @@
         "workgroupName": str,
         "activateCaseSensitiveIdentifier": NotRequired[bool],
         "sourceSchemaName": NotRequired[str],
         "targetDatabaseName": NotRequired[str],
         "targetSchemaName": NotRequired[str],
     },
 )
+ScheduleOutputTypeDef = TypedDict(
+    "ScheduleOutputTypeDef",
+    {
+        "at": NotRequired[datetime],
+        "cron": NotRequired[str],
+    },
+)
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -743,14 +763,23 @@
     {
         "namespaceName": str,
         "snapshotName": str,
         "retentionPeriod": NotRequired[int],
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+CreateSnapshotScheduleActionParametersOutputTypeDef = TypedDict(
+    "CreateSnapshotScheduleActionParametersOutputTypeDef",
+    {
+        "namespaceName": str,
+        "snapshotNamePrefix": str,
+        "retentionPeriod": NotRequired[int],
+        "tags": NotRequired[List[TagTypeDef]],
+    },
+)
 CreateSnapshotScheduleActionParametersTypeDef = TypedDict(
     "CreateSnapshotScheduleActionParametersTypeDef",
     {
         "namespaceName": str,
         "snapshotNamePrefix": str,
         "retentionPeriod": NotRequired[int],
         "tags": NotRequired[Sequence[TagTypeDef]],
@@ -813,22 +842,14 @@
     "ListCustomDomainAssociationsResponseTypeDef",
     {
         "associations": List[AssociationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListScheduledActionsResponseTypeDef = TypedDict(
-    "ListScheduledActionsResponseTypeDef",
-    {
-        "nextToken": str,
-        "scheduledActions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1168,28 +1189,43 @@
 ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
     "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     {
         "ownerAccount": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListScheduledActionsResponseTypeDef = TypedDict(
+    "ListScheduledActionsResponseTypeDef",
+    {
+        "nextToken": str,
+        "scheduledActions": List[ScheduledActionAssociationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "networkInterfaces": NotRequired[List[NetworkInterfaceTypeDef]],
         "vpcEndpointId": NotRequired[str],
         "vpcId": NotRequired[str],
     },
 )
+TargetActionOutputTypeDef = TypedDict(
+    "TargetActionOutputTypeDef",
+    {
+        "createSnapshot": NotRequired[CreateSnapshotScheduleActionParametersOutputTypeDef],
+    },
+)
 TargetActionTypeDef = TypedDict(
     "TargetActionTypeDef",
     {
         "createSnapshot": NotRequired[CreateSnapshotScheduleActionParametersTypeDef],
     },
 )
+ScheduleUnionTypeDef = Union[ScheduleTypeDef, ScheduleOutputTypeDef]
 EndpointAccessTypeDef = TypedDict(
     "EndpointAccessTypeDef",
     {
         "address": NotRequired[str],
         "endpointArn": NotRequired[str],
         "endpointCreateTime": NotRequired[datetime],
         "endpointName": NotRequired[str],
@@ -1205,44 +1241,45 @@
     "EndpointTypeDef",
     {
         "address": NotRequired[str],
         "port": NotRequired[int],
         "vpcEndpoints": NotRequired[List[VpcEndpointTypeDef]],
     },
 )
-CreateScheduledActionRequestRequestTypeDef = TypedDict(
-    "CreateScheduledActionRequestRequestTypeDef",
-    {
-        "namespaceName": str,
-        "roleArn": str,
-        "schedule": ScheduleTypeDef,
-        "scheduledActionName": str,
-        "targetAction": TargetActionTypeDef,
-        "enabled": NotRequired[bool],
-        "endTime": NotRequired[TimestampTypeDef],
-        "scheduledActionDescription": NotRequired[str],
-        "startTime": NotRequired[TimestampTypeDef],
-    },
-)
 ScheduledActionResponseTypeDef = TypedDict(
     "ScheduledActionResponseTypeDef",
     {
         "endTime": NotRequired[datetime],
         "namespaceName": NotRequired[str],
         "nextInvocations": NotRequired[List[datetime]],
         "roleArn": NotRequired[str],
-        "schedule": NotRequired[ScheduleTypeDef],
+        "schedule": NotRequired[ScheduleOutputTypeDef],
         "scheduledActionDescription": NotRequired[str],
         "scheduledActionName": NotRequired[str],
         "scheduledActionUuid": NotRequired[str],
         "startTime": NotRequired[datetime],
         "state": NotRequired[StateType],
-        "targetAction": NotRequired[TargetActionTypeDef],
+        "targetAction": NotRequired[TargetActionOutputTypeDef],
+    },
+)
+CreateScheduledActionRequestRequestTypeDef = TypedDict(
+    "CreateScheduledActionRequestRequestTypeDef",
+    {
+        "namespaceName": str,
+        "roleArn": str,
+        "schedule": ScheduleTypeDef,
+        "scheduledActionName": str,
+        "targetAction": TargetActionTypeDef,
+        "enabled": NotRequired[bool],
+        "endTime": NotRequired[TimestampTypeDef],
+        "scheduledActionDescription": NotRequired[str],
+        "startTime": NotRequired[TimestampTypeDef],
     },
 )
+TargetActionUnionTypeDef = Union[TargetActionTypeDef, TargetActionOutputTypeDef]
 UpdateScheduledActionRequestRequestTypeDef = TypedDict(
     "UpdateScheduledActionRequestRequestTypeDef",
     {
         "scheduledActionName": str,
         "enabled": NotRequired[bool],
         "endTime": NotRequired[TimestampTypeDef],
         "roleArn": NotRequired[str],
```

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless/type_defs.pyi` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -75,44 +75,46 @@
     "GetUsageLimitRequestRequestTypeDef",
     "GetWorkgroupRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListCustomDomainAssociationsRequestRequestTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListScheduledActionsRequestRequestTypeDef",
+    "ScheduledActionAssociationTypeDef",
     "ListSnapshotCopyConfigurationsRequestRequestTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "RestoreTableFromRecoveryPointRequestRequestTypeDef",
     "RestoreTableFromSnapshotRequestRequestTypeDef",
+    "ScheduleOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCustomDomainAssociationRequestRequestTypeDef",
     "UpdateEndpointAccessRequestRequestTypeDef",
     "UpdateNamespaceRequestRequestTypeDef",
     "UpdateSnapshotCopyConfigurationRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateUsageLimitRequestRequestTypeDef",
     "UpdateWorkgroupRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
+    "CreateSnapshotScheduleActionParametersOutputTypeDef",
     "CreateSnapshotScheduleActionParametersTypeDef",
     "CreateWorkgroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateCustomDomainAssociationResponseTypeDef",
     "GetCredentialsResponseTypeDef",
     "GetCustomDomainAssociationResponseTypeDef",
     "ListCustomDomainAssociationsResponseTypeDef",
-    "ListScheduledActionsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateCustomDomainAssociationResponseTypeDef",
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DeleteSnapshotResponseTypeDef",
     "GetSnapshotResponseTypeDef",
     "ListSnapshotsResponseTypeDef",
@@ -150,20 +152,24 @@
     "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
     "ListScheduledActionsRequestListScheduledActionsPaginateTypeDef",
     "ListSnapshotCopyConfigurationsRequestListSnapshotCopyConfigurationsPaginateTypeDef",
     "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
     "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    "ListScheduledActionsResponseTypeDef",
     "VpcEndpointTypeDef",
+    "TargetActionOutputTypeDef",
     "TargetActionTypeDef",
+    "ScheduleUnionTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
-    "CreateScheduledActionRequestRequestTypeDef",
     "ScheduledActionResponseTypeDef",
+    "CreateScheduledActionRequestRequestTypeDef",
+    "TargetActionUnionTypeDef",
     "UpdateScheduledActionRequestRequestTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
     "UpdateEndpointAccessResponseTypeDef",
     "WorkgroupTypeDef",
@@ -530,14 +536,21 @@
     "ListScheduledActionsRequestRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "namespaceName": NotRequired[str],
         "nextToken": NotRequired[str],
     },
 )
+ScheduledActionAssociationTypeDef = TypedDict(
+    "ScheduledActionAssociationTypeDef",
+    {
+        "namespaceName": NotRequired[str],
+        "scheduledActionName": NotRequired[str],
+    },
+)
 ListSnapshotCopyConfigurationsRequestRequestTypeDef = TypedDict(
     "ListSnapshotCopyConfigurationsRequestRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "namespaceName": NotRequired[str],
         "nextToken": NotRequired[str],
     },
@@ -636,14 +649,21 @@
         "workgroupName": str,
         "activateCaseSensitiveIdentifier": NotRequired[bool],
         "sourceSchemaName": NotRequired[str],
         "targetDatabaseName": NotRequired[str],
         "targetSchemaName": NotRequired[str],
     },
 )
+ScheduleOutputTypeDef = TypedDict(
+    "ScheduleOutputTypeDef",
+    {
+        "at": NotRequired[datetime],
+        "cron": NotRequired[str],
+    },
+)
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -743,14 +763,23 @@
     {
         "namespaceName": str,
         "snapshotName": str,
         "retentionPeriod": NotRequired[int],
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
+CreateSnapshotScheduleActionParametersOutputTypeDef = TypedDict(
+    "CreateSnapshotScheduleActionParametersOutputTypeDef",
+    {
+        "namespaceName": str,
+        "snapshotNamePrefix": str,
+        "retentionPeriod": NotRequired[int],
+        "tags": NotRequired[List[TagTypeDef]],
+    },
+)
 CreateSnapshotScheduleActionParametersTypeDef = TypedDict(
     "CreateSnapshotScheduleActionParametersTypeDef",
     {
         "namespaceName": str,
         "snapshotNamePrefix": str,
         "retentionPeriod": NotRequired[int],
         "tags": NotRequired[Sequence[TagTypeDef]],
@@ -813,22 +842,14 @@
     "ListCustomDomainAssociationsResponseTypeDef",
     {
         "associations": List[AssociationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListScheduledActionsResponseTypeDef = TypedDict(
-    "ListScheduledActionsResponseTypeDef",
-    {
-        "nextToken": str,
-        "scheduledActions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1168,28 +1189,43 @@
 ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
     "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     {
         "ownerAccount": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListScheduledActionsResponseTypeDef = TypedDict(
+    "ListScheduledActionsResponseTypeDef",
+    {
+        "nextToken": str,
+        "scheduledActions": List[ScheduledActionAssociationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "networkInterfaces": NotRequired[List[NetworkInterfaceTypeDef]],
         "vpcEndpointId": NotRequired[str],
         "vpcId": NotRequired[str],
     },
 )
+TargetActionOutputTypeDef = TypedDict(
+    "TargetActionOutputTypeDef",
+    {
+        "createSnapshot": NotRequired[CreateSnapshotScheduleActionParametersOutputTypeDef],
+    },
+)
 TargetActionTypeDef = TypedDict(
     "TargetActionTypeDef",
     {
         "createSnapshot": NotRequired[CreateSnapshotScheduleActionParametersTypeDef],
     },
 )
+ScheduleUnionTypeDef = Union[ScheduleTypeDef, ScheduleOutputTypeDef]
 EndpointAccessTypeDef = TypedDict(
     "EndpointAccessTypeDef",
     {
         "address": NotRequired[str],
         "endpointArn": NotRequired[str],
         "endpointCreateTime": NotRequired[datetime],
         "endpointName": NotRequired[str],
@@ -1205,44 +1241,45 @@
     "EndpointTypeDef",
     {
         "address": NotRequired[str],
         "port": NotRequired[int],
         "vpcEndpoints": NotRequired[List[VpcEndpointTypeDef]],
     },
 )
-CreateScheduledActionRequestRequestTypeDef = TypedDict(
-    "CreateScheduledActionRequestRequestTypeDef",
-    {
-        "namespaceName": str,
-        "roleArn": str,
-        "schedule": ScheduleTypeDef,
-        "scheduledActionName": str,
-        "targetAction": TargetActionTypeDef,
-        "enabled": NotRequired[bool],
-        "endTime": NotRequired[TimestampTypeDef],
-        "scheduledActionDescription": NotRequired[str],
-        "startTime": NotRequired[TimestampTypeDef],
-    },
-)
 ScheduledActionResponseTypeDef = TypedDict(
     "ScheduledActionResponseTypeDef",
     {
         "endTime": NotRequired[datetime],
         "namespaceName": NotRequired[str],
         "nextInvocations": NotRequired[List[datetime]],
         "roleArn": NotRequired[str],
-        "schedule": NotRequired[ScheduleTypeDef],
+        "schedule": NotRequired[ScheduleOutputTypeDef],
         "scheduledActionDescription": NotRequired[str],
         "scheduledActionName": NotRequired[str],
         "scheduledActionUuid": NotRequired[str],
         "startTime": NotRequired[datetime],
         "state": NotRequired[StateType],
-        "targetAction": NotRequired[TargetActionTypeDef],
+        "targetAction": NotRequired[TargetActionOutputTypeDef],
+    },
+)
+CreateScheduledActionRequestRequestTypeDef = TypedDict(
+    "CreateScheduledActionRequestRequestTypeDef",
+    {
+        "namespaceName": str,
+        "roleArn": str,
+        "schedule": ScheduleTypeDef,
+        "scheduledActionName": str,
+        "targetAction": TargetActionTypeDef,
+        "enabled": NotRequired[bool],
+        "endTime": NotRequired[TimestampTypeDef],
+        "scheduledActionDescription": NotRequired[str],
+        "startTime": NotRequired[TimestampTypeDef],
     },
 )
+TargetActionUnionTypeDef = Union[TargetActionTypeDef, TargetActionOutputTypeDef]
 UpdateScheduledActionRequestRequestTypeDef = TypedDict(
     "UpdateScheduledActionRequestRequestTypeDef",
     {
         "scheduledActionName": str,
         "enabled": NotRequired[bool],
         "endTime": NotRequired[TimestampTypeDef],
         "roleArn": NotRequired[str],
```

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless.egg-info/PKG-INFO` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-serverless
-Version: 1.34.89
-Summary: Type annotations for boto3.RedshiftServerless 1.34.89 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.97
+Summary: Type annotations for boto3.RedshiftServerless 1.34.97 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_redshift_serverless-1.34.89/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt` & `mypy_boto3_redshift_serverless-1.34.97/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_redshift_serverless-1.34.89/setup.py` & `mypy_boto3_redshift_serverless-1.34.97/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift-serverless",
-    version="1.34.89",
+    version="1.34.97",
     packages=["mypy_boto3_redshift_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.RedshiftServerless 1.34.89 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.RedshiftServerless 1.34.97 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

