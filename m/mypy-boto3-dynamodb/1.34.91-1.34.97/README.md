# Comparing `tmp/mypy_boto3_dynamodb-1.34.91.tar.gz` & `tmp/mypy_boto3_dynamodb-1.34.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_dynamodb-1.34.91.tar", last modified: Thu Apr 25 00:48:24 2024, max compression
+gzip compressed data, was "mypy_boto3_dynamodb-1.34.97.tar", last modified: Thu May  2 19:33:14 2024, max compression
```

## Comparing `mypy_boto3_dynamodb-1.34.91.tar` & `mypy_boto3_dynamodb-1.34.97.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:24.528523 mypy_boto3_dynamodb-1.34.91/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2024-04-24 23:44:27.000000 mypy_boto3_dynamodb-1.34.91/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16270 2024-04-25 00:48:24.528523 mypy_boto3_dynamodb-1.34.91/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14711 2024-04-24 23:44:27.000000 mypy_boto3_dynamodb-1.34.91/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:24.528523 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1857 2024-04-24 23:44:27.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1857 2024-04-24 23:44:27.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      923 2024-04-24 23:44:27.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    51570 2024-04-24 23:44:28.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    51567 2024-04-24 23:44:28.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14002 2024-04-24 23:44:30.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    14002 2024-04-24 23:44:30.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7480 2024-04-24 23:44:29.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7474 2024-04-24 23:44:29.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2024-04-24 23:44:27.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22603 2024-04-24 23:44:29.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/service_resource.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    22598 2024-04-24 23:44:29.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/service_resource.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)   103055 2024-04-24 23:44:37.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   103055 2024-04-24 23:44:34.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       62 2024-04-24 23:44:27.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2259 2024-04-24 23:44:29.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2257 2024-04-24 23:44:29.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-25 00:48:24.528523 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    16270 2024-04-25 00:48:24.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      841 2024-04-25 00:48:24.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 00:48:24.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-25 00:48:24.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       53 2024-04-25 00:48:24.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       20 2024-04-25 00:48:24.000000 mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2024-04-25 00:48:24.528523 mypy_boto3_dynamodb-1.34.91/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1981 2024-04-24 23:44:27.000000 mypy_boto3_dynamodb-1.34.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:14.718119 mypy_boto3_dynamodb-1.34.97/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 19:32:08.000000 mypy_boto3_dynamodb-1.34.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16270 2024-05-02 19:33:14.718119 mypy_boto3_dynamodb-1.34.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14711 2024-05-02 19:32:08.000000 mypy_boto3_dynamodb-1.34.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:14.714119 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-02 19:32:08.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-02 19:32:08.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-02 19:32:08.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51861 2024-05-02 19:32:08.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51858 2024-05-02 19:32:08.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-02 19:32:10.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-02 19:32:09.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-05-02 19:32:09.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-02 19:32:09.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:32:08.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    22855 2024-05-02 19:32:09.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22850 2024-05-02 19:32:09.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   105316 2024-05-02 19:32:11.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105316 2024-05-02 19:32:11.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 19:32:08.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-02 19:32:09.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-02 19:32:09.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:14.718119 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16270 2024-05-02 19:33:14.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-02 19:33:14.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:33:14.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:33:14.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 19:33:14.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 19:33:14.000000 mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:33:14.718119 mypy_boto3_dynamodb-1.34.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-02 19:32:08.000000 mypy_boto3_dynamodb-1.34.97/setup.py
```

### Comparing `mypy_boto3_dynamodb-1.34.91/LICENSE` & `mypy_boto3_dynamodb-1.34.97/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_dynamodb-1.34.91/PKG-INFO` & `mypy_boto3_dynamodb-1.34.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.34.91
-Summary: Type annotations for boto3.DynamoDB 1.34.91 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.97
+Summary: Type annotations for boto3.DynamoDB 1.34.97 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodb)](https://pepy.tech/project/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_dynamodb-1.34.91/README.md` & `mypy_boto3_dynamodb-1.34.97/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodb)](https://pepy.tech/project/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/__init__.py` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/__init__.pyi` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/__main__.py` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDB 1.34.91\n"
-        "Version:         1.34.91\n"
+        "Type annotations for boto3.DynamoDB 1.34.97\n"
+        "Version:         1.34.97\n"
         "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.91")
+    print("1.34.97")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/client.py` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     ListContributorInsightsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
     ListTablesOutputTypeDef,
     ListTagsOfResourceOutputTypeDef,
     LocalSecondaryIndexTypeDef,
+    OnDemandThroughputTypeDef,
     ParameterizedStatementTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
     ProvisionedThroughputTypeDef,
     PutItemOutputTypeDef,
     PutResourcePolicyOutputTypeDef,
     QueryOutputTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
@@ -141,23 +142,21 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("DynamoDBClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BackupInUseException: Type[BotocoreClientError]
     BackupNotFoundException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConditionalCheckFailedException: Type[BotocoreClientError]
     ContinuousBackupsUnavailableException: Type[BotocoreClientError]
     DuplicateItemException: Type[BotocoreClientError]
@@ -185,15 +184,14 @@
     TableAlreadyExistsException: Type[BotocoreClientError]
     TableInUseException: Type[BotocoreClientError]
     TableNotFoundException: Type[BotocoreClientError]
     TransactionCanceledException: Type[BotocoreClientError]
     TransactionConflictException: Type[BotocoreClientError]
     TransactionInProgressException: Type[BotocoreClientError]
 
-
 class DynamoDBClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/)
     """
 
     meta: ClientMeta
@@ -298,14 +296,15 @@
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...,
         ResourcePolicy: str = ...,
+        OnDemandThroughput: OnDemandThroughputTypeDef = ...,
     ) -> CreateTableOutputTypeDef:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#create_table)
         """
@@ -788,14 +787,15 @@
         *,
         TargetTableName: str,
         BackupArn: str,
         BillingModeOverride: BillingModeType = ...,
         GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
+        OnDemandThroughputOverride: OnDemandThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...,
     ) -> RestoreTableFromBackupOutputTypeDef:
         """
         Creates a new table from an existing backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.restore_table_from_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#restore_table_from_backup)
@@ -809,14 +809,15 @@
         SourceTableName: str = ...,
         UseLatestRestorableTime: bool = ...,
         RestoreDateTime: TimestampTypeDef = ...,
         BillingModeOverride: BillingModeType = ...,
         GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
+        OnDemandThroughputOverride: OnDemandThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...,
     ) -> RestoreTableToPointInTimeOutputTypeDef:
         """
         Restores the specified table to the specified point in time within
         `EarliestRestorableDateTime` and
         `LatestRestorableDateTime`.
 
@@ -1013,14 +1014,15 @@
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...,
+        OnDemandThroughput: OnDemandThroughputTypeDef = ...,
     ) -> UpdateTableOutputTypeDef:
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_table)
```

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/client.pyi` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     ListContributorInsightsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
     ListTablesOutputTypeDef,
     ListTagsOfResourceOutputTypeDef,
     LocalSecondaryIndexTypeDef,
+    OnDemandThroughputTypeDef,
     ParameterizedStatementTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
     ProvisionedThroughputTypeDef,
     PutItemOutputTypeDef,
     PutResourcePolicyOutputTypeDef,
     QueryOutputTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
@@ -141,21 +142,23 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("DynamoDBClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BackupInUseException: Type[BotocoreClientError]
     BackupNotFoundException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConditionalCheckFailedException: Type[BotocoreClientError]
     ContinuousBackupsUnavailableException: Type[BotocoreClientError]
     DuplicateItemException: Type[BotocoreClientError]
@@ -183,14 +186,15 @@
     TableAlreadyExistsException: Type[BotocoreClientError]
     TableInUseException: Type[BotocoreClientError]
     TableNotFoundException: Type[BotocoreClientError]
     TransactionCanceledException: Type[BotocoreClientError]
     TransactionConflictException: Type[BotocoreClientError]
     TransactionInProgressException: Type[BotocoreClientError]
 
+
 class DynamoDBClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/)
     """
 
     meta: ClientMeta
@@ -295,14 +299,15 @@
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...,
         ResourcePolicy: str = ...,
+        OnDemandThroughput: OnDemandThroughputTypeDef = ...,
     ) -> CreateTableOutputTypeDef:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#create_table)
         """
@@ -785,14 +790,15 @@
         *,
         TargetTableName: str,
         BackupArn: str,
         BillingModeOverride: BillingModeType = ...,
         GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
+        OnDemandThroughputOverride: OnDemandThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...,
     ) -> RestoreTableFromBackupOutputTypeDef:
         """
         Creates a new table from an existing backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.restore_table_from_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#restore_table_from_backup)
@@ -806,14 +812,15 @@
         SourceTableName: str = ...,
         UseLatestRestorableTime: bool = ...,
         RestoreDateTime: TimestampTypeDef = ...,
         BillingModeOverride: BillingModeType = ...,
         GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
+        OnDemandThroughputOverride: OnDemandThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...,
     ) -> RestoreTableToPointInTimeOutputTypeDef:
         """
         Restores the specified table to the specified point in time within
         `EarliestRestorableDateTime` and
         `LatestRestorableDateTime`.
 
@@ -1010,14 +1017,15 @@
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...,
+        OnDemandThroughput: OnDemandThroughputTypeDef = ...,
     ) -> UpdateTableOutputTypeDef:
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_table)
```

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/literals.py` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/literals.pyi` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/paginator.py` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/paginator.pyi` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/service_resource.py` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     GlobalSecondaryIndexDescriptionTypeDef,
     GlobalSecondaryIndexUnionTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
     KeysAndAttributesServiceResourceUnionTypeDef,
     KeySchemaElementTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
     LocalSecondaryIndexTypeDef,
+    OnDemandThroughputResponseTypeDef,
+    OnDemandThroughputTypeDef,
     ProvisionedThroughputDescriptionResponseTypeDef,
     ProvisionedThroughputTypeDef,
     PutItemOutputTableTypeDef,
     QueryOutputTableTypeDef,
     ReplicaDescriptionTypeDef,
     ReplicationGroupUpdateTypeDef,
     RestoreSummaryResponseTypeDef,
@@ -161,14 +163,15 @@
     global_table_version: str
     replicas: List[ReplicaDescriptionTypeDef]
     restore_summary: RestoreSummaryResponseTypeDef
     sse_description: SSEDescriptionResponseTypeDef
     archival_summary: ArchivalSummaryResponseTypeDef
     table_class_summary: TableClassSummaryResponseTypeDef
     deletion_protection_enabled: bool
+    on_demand_throughput: OnDemandThroughputResponseTypeDef
     name: str
     meta: "DynamoDBResourceMeta"
 
     def batch_writer(self, overwrite_by_pkeys: List[str] = ...) -> BatchWriter:
         """
         Create a batch writer object.
 
@@ -338,14 +341,15 @@
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...,
+        OnDemandThroughput: OnDemandThroughputTypeDef = ...,
     ) -> "_Table":
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update)
@@ -460,14 +464,15 @@
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...,
         ResourcePolicy: str = ...,
+        OnDemandThroughput: OnDemandThroughputTypeDef = ...,
     ) -> "_Table":
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcecreate_table-method)
         """
```

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/service_resource.pyi` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     GlobalSecondaryIndexDescriptionTypeDef,
     GlobalSecondaryIndexUnionTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
     KeysAndAttributesServiceResourceUnionTypeDef,
     KeySchemaElementTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
     LocalSecondaryIndexTypeDef,
+    OnDemandThroughputResponseTypeDef,
+    OnDemandThroughputTypeDef,
     ProvisionedThroughputDescriptionResponseTypeDef,
     ProvisionedThroughputTypeDef,
     PutItemOutputTableTypeDef,
     QueryOutputTableTypeDef,
     ReplicaDescriptionTypeDef,
     ReplicationGroupUpdateTypeDef,
     RestoreSummaryResponseTypeDef,
@@ -159,14 +161,15 @@
     global_table_version: str
     replicas: List[ReplicaDescriptionTypeDef]
     restore_summary: RestoreSummaryResponseTypeDef
     sse_description: SSEDescriptionResponseTypeDef
     archival_summary: ArchivalSummaryResponseTypeDef
     table_class_summary: TableClassSummaryResponseTypeDef
     deletion_protection_enabled: bool
+    on_demand_throughput: OnDemandThroughputResponseTypeDef
     name: str
     meta: "DynamoDBResourceMeta"
 
     def batch_writer(self, overwrite_by_pkeys: List[str] = ...) -> BatchWriter:
         """
         Create a batch writer object.
 
@@ -336,14 +339,15 @@
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...,
+        OnDemandThroughput: OnDemandThroughputTypeDef = ...,
     ) -> "_Table":
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update)
@@ -455,14 +459,15 @@
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...,
         ResourcePolicy: str = ...,
+        OnDemandThroughput: OnDemandThroughputTypeDef = ...,
     ) -> "_Table":
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#dynamodbserviceresourcecreate_table-method)
         """
```

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/type_defs.py` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,18 +83,20 @@
     "BillingModeSummaryTypeDef",
     "CapacityTypeDef",
     "ConditionBaseImportTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
     "ContributorInsightsSummaryTypeDef",
     "CreateBackupInputRequestTypeDef",
     "KeySchemaElementTypeDef",
+    "OnDemandThroughputTypeDef",
     "ProjectionTypeDef",
     "ProvisionedThroughputTypeDef",
     "ReplicaTypeDef",
     "CreateReplicaActionTypeDef",
+    "OnDemandThroughputOverrideTypeDef",
     "ProvisionedThroughputOverrideTypeDef",
     "SSESpecificationTypeDef",
     "StreamSpecificationTypeDef",
     "TagTypeDef",
     "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
     "DeleteBackupInputRequestTypeDef",
@@ -148,14 +150,15 @@
     "ArchivalSummaryResponseTypeDef",
     "BillingModeSummaryResponseTypeDef",
     "DeleteResourcePolicyOutputTypeDef",
     "DescribeLimitsOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetResourcePolicyOutputTypeDef",
     "ListTablesOutputTypeDef",
+    "OnDemandThroughputResponseTypeDef",
     "ProvisionedThroughputDescriptionResponseTypeDef",
     "PutResourcePolicyOutputTypeDef",
     "RestoreSummaryResponseTypeDef",
     "SSEDescriptionResponseTypeDef",
     "StreamSpecificationResponseTypeDef",
     "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
@@ -500,14 +503,21 @@
 KeySchemaElementTypeDef = TypedDict(
     "KeySchemaElementTypeDef",
     {
         "AttributeName": str,
         "KeyType": KeyTypeType,
     },
 )
+OnDemandThroughputTypeDef = TypedDict(
+    "OnDemandThroughputTypeDef",
+    {
+        "MaxReadRequestUnits": NotRequired[int],
+        "MaxWriteRequestUnits": NotRequired[int],
+    },
+)
 ProjectionTypeDef = TypedDict(
     "ProjectionTypeDef",
     {
         "ProjectionType": NotRequired[ProjectionTypeType],
         "NonKeyAttributes": NotRequired[Sequence[str]],
     },
 )
@@ -526,14 +536,20 @@
 )
 CreateReplicaActionTypeDef = TypedDict(
     "CreateReplicaActionTypeDef",
     {
         "RegionName": str,
     },
 )
+OnDemandThroughputOverrideTypeDef = TypedDict(
+    "OnDemandThroughputOverrideTypeDef",
+    {
+        "MaxReadRequestUnits": NotRequired[int],
+    },
+)
 ProvisionedThroughputOverrideTypeDef = TypedDict(
     "ProvisionedThroughputOverrideTypeDef",
     {
         "ReadCapacityUnits": NotRequired[int],
     },
 )
 SSESpecificationTypeDef = TypedDict(
@@ -960,14 +976,22 @@
     "ListTablesOutputTypeDef",
     {
         "TableNames": List[str],
         "LastEvaluatedTableName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+OnDemandThroughputResponseTypeDef = TypedDict(
+    "OnDemandThroughputResponseTypeDef",
+    {
+        "MaxReadRequestUnits": int,
+        "MaxWriteRequestUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ProvisionedThroughputDescriptionResponseTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionResponseTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
@@ -1248,44 +1272,48 @@
 CreateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "CreateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 GlobalSecondaryIndexTypeDef = TypedDict(
     "GlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 SourceTableDetailsTypeDef = TypedDict(
     "SourceTableDetailsTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "KeySchema": List[KeySchemaElementTypeDef],
         "TableCreationDateTime": datetime,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "TableArn": NotRequired[str],
         "TableSizeBytes": NotRequired[int],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
         "ItemCount": NotRequired[int],
         "BillingMode": NotRequired[BillingModeType],
     },
 )
 UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 CreateGlobalTableInputRequestTypeDef = TypedDict(
     "CreateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicationGroup": Sequence[ReplicaTypeDef],
@@ -1299,21 +1327,23 @@
     },
 )
 ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": NotRequired[str],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputOverrideTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputOverrideTypeDef],
     },
 )
 ReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputOverrideTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputOverrideTypeDef],
     },
 )
 ListTagsOfResourceOutputTypeDef = TypedDict(
     "ListTagsOfResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1486,32 +1516,35 @@
         "Projection": NotRequired[ProjectionExtraOutputTypeDef],
         "IndexStatus": NotRequired[IndexStatusType],
         "Backfilling": NotRequired[bool],
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputDescriptionTypeDef],
         "IndexSizeBytes": NotRequired[int],
         "ItemCount": NotRequired[int],
         "IndexArn": NotRequired[str],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 GlobalSecondaryIndexInfoTypeDef = TypedDict(
     "GlobalSecondaryIndexInfoTypeDef",
     {
         "IndexName": NotRequired[str],
         "KeySchema": NotRequired[List[KeySchemaElementTypeDef]],
         "Projection": NotRequired[ProjectionOutputTypeDef],
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 GlobalSecondaryIndexOutputTypeDef = TypedDict(
     "GlobalSecondaryIndexOutputTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementTypeDef],
         "Projection": ProjectionOutputTypeDef,
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 LocalSecondaryIndexInfoTypeDef = TypedDict(
     "LocalSecondaryIndexInfoTypeDef",
     {
         "IndexName": NotRequired[str],
         "KeySchema": NotRequired[List[KeySchemaElementTypeDef]],
@@ -2059,14 +2092,15 @@
     "TableCreationParametersTypeDef",
     {
         "TableName": str,
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "BillingMode": NotRequired[BillingModeType],
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "GlobalSecondaryIndexes": NotRequired[Sequence[GlobalSecondaryIndexTypeDef]],
     },
 )
 GlobalSecondaryIndexUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTypeDef",
     {
@@ -2088,35 +2122,38 @@
     {
         "RegionName": NotRequired[str],
         "ReplicaStatus": NotRequired[ReplicaStatusType],
         "ReplicaStatusDescription": NotRequired[str],
         "ReplicaStatusPercentProgress": NotRequired[str],
         "KMSMasterKeyId": NotRequired[str],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputOverrideTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputOverrideTypeDef],
         "GlobalSecondaryIndexes": NotRequired[List[ReplicaGlobalSecondaryIndexDescriptionTypeDef]],
         "ReplicaInaccessibleDateTime": NotRequired[datetime],
         "ReplicaTableClassSummary": NotRequired[TableClassSummaryTypeDef],
     },
 )
 CreateReplicationGroupMemberActionTypeDef = TypedDict(
     "CreateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
         "KMSMasterKeyId": NotRequired[str],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputOverrideTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputOverrideTypeDef],
         "GlobalSecondaryIndexes": NotRequired[Sequence[ReplicaGlobalSecondaryIndexTypeDef]],
         "TableClassOverride": NotRequired[TableClassType],
     },
 )
 UpdateReplicationGroupMemberActionTypeDef = TypedDict(
     "UpdateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
         "KMSMasterKeyId": NotRequired[str],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputOverrideTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputOverrideTypeDef],
         "GlobalSecondaryIndexes": NotRequired[Sequence[ReplicaGlobalSecondaryIndexTypeDef]],
         "TableClassOverride": NotRequired[TableClassType],
     },
 )
 InputFormatOptionsUnionTypeDef = Union[InputFormatOptionsTypeDef, InputFormatOptionsOutputTypeDef]
 UpdateGlobalTableInputRequestTypeDef = TypedDict(
     "UpdateGlobalTableInputRequestTypeDef",
@@ -2165,14 +2202,15 @@
     "TableCreationParametersOutputTypeDef",
     {
         "TableName": str,
         "AttributeDefinitions": List[AttributeDefinitionTypeDef],
         "KeySchema": List[KeySchemaElementTypeDef],
         "BillingMode": NotRequired[BillingModeType],
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "GlobalSecondaryIndexes": NotRequired[List[GlobalSecondaryIndexOutputTypeDef]],
     },
 )
 SourceTableFeatureDetailsTypeDef = TypedDict(
     "SourceTableFeatureDetailsTypeDef",
     {
@@ -2504,14 +2542,15 @@
         "GlobalTableVersion": NotRequired[str],
         "Replicas": NotRequired[List[ReplicaDescriptionTypeDef]],
         "RestoreSummary": NotRequired[RestoreSummaryTypeDef],
         "SSEDescription": NotRequired[SSEDescriptionTypeDef],
         "ArchivalSummary": NotRequired[ArchivalSummaryTypeDef],
         "TableClassSummary": NotRequired[TableClassSummaryTypeDef],
         "DeletionProtectionEnabled": NotRequired[bool],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 ReplicationGroupUpdateTypeDef = TypedDict(
     "ReplicationGroupUpdateTypeDef",
     {
         "Create": NotRequired[CreateReplicationGroupMemberActionTypeDef],
         "Update": NotRequired[UpdateReplicationGroupMemberActionTypeDef],
@@ -2530,14 +2569,15 @@
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
         "StreamSpecification": NotRequired[StreamSpecificationTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "TableClass": NotRequired[TableClassType],
         "DeletionProtectionEnabled": NotRequired[bool],
         "ResourcePolicy": NotRequired[str],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 CreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
     "CreateTableInputServiceResourceCreateTableTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "TableName": str,
@@ -2548,25 +2588,27 @@
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
         "StreamSpecification": NotRequired[StreamSpecificationTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "TableClass": NotRequired[TableClassType],
         "DeletionProtectionEnabled": NotRequired[bool],
         "ResourcePolicy": NotRequired[str],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 RestoreTableFromBackupInputRequestTypeDef = TypedDict(
     "RestoreTableFromBackupInputRequestTypeDef",
     {
         "TargetTableName": str,
         "BackupArn": str,
         "BillingModeOverride": NotRequired[BillingModeType],
         "GlobalSecondaryIndexOverride": NotRequired[Sequence[GlobalSecondaryIndexUnionTypeDef]],
         "LocalSecondaryIndexOverride": NotRequired[Sequence[LocalSecondaryIndexTypeDef]],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputTypeDef],
         "SSESpecificationOverride": NotRequired[SSESpecificationTypeDef],
     },
 )
 RestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
     "RestoreTableToPointInTimeInputRequestTypeDef",
     {
         "TargetTableName": str,
@@ -2574,14 +2616,15 @@
         "SourceTableName": NotRequired[str],
         "UseLatestRestorableTime": NotRequired[bool],
         "RestoreDateTime": NotRequired[TimestampTypeDef],
         "BillingModeOverride": NotRequired[BillingModeType],
         "GlobalSecondaryIndexOverride": NotRequired[Sequence[GlobalSecondaryIndexUnionTypeDef]],
         "LocalSecondaryIndexOverride": NotRequired[Sequence[LocalSecondaryIndexTypeDef]],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputTypeDef],
         "SSESpecificationOverride": NotRequired[SSESpecificationTypeDef],
     },
 )
 ImportTableDescriptionTypeDef = TypedDict(
     "ImportTableDescriptionTypeDef",
     {
         "ImportArn": NotRequired[str],
@@ -2782,28 +2825,30 @@
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
         "GlobalSecondaryIndexUpdates": NotRequired[Sequence[GlobalSecondaryIndexUpdateTypeDef]],
         "StreamSpecification": NotRequired[StreamSpecificationTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "ReplicaUpdates": NotRequired[Sequence[ReplicationGroupUpdateTypeDef]],
         "TableClass": NotRequired[TableClassType],
         "DeletionProtectionEnabled": NotRequired[bool],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 UpdateTableInputTableUpdateTypeDef = TypedDict(
     "UpdateTableInputTableUpdateTypeDef",
     {
         "AttributeDefinitions": NotRequired[Sequence[AttributeDefinitionTypeDef]],
         "BillingMode": NotRequired[BillingModeType],
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
         "GlobalSecondaryIndexUpdates": NotRequired[Sequence[GlobalSecondaryIndexUpdateTypeDef]],
         "StreamSpecification": NotRequired[StreamSpecificationTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "ReplicaUpdates": NotRequired[Sequence[ReplicationGroupUpdateTypeDef]],
         "TableClass": NotRequired[TableClassType],
         "DeletionProtectionEnabled": NotRequired[bool],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 DescribeImportOutputTypeDef = TypedDict(
     "DescribeImportOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/type_defs.pyi` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -83,18 +83,20 @@
     "BillingModeSummaryTypeDef",
     "CapacityTypeDef",
     "ConditionBaseImportTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
     "ContributorInsightsSummaryTypeDef",
     "CreateBackupInputRequestTypeDef",
     "KeySchemaElementTypeDef",
+    "OnDemandThroughputTypeDef",
     "ProjectionTypeDef",
     "ProvisionedThroughputTypeDef",
     "ReplicaTypeDef",
     "CreateReplicaActionTypeDef",
+    "OnDemandThroughputOverrideTypeDef",
     "ProvisionedThroughputOverrideTypeDef",
     "SSESpecificationTypeDef",
     "StreamSpecificationTypeDef",
     "TagTypeDef",
     "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
     "DeleteBackupInputRequestTypeDef",
@@ -148,14 +150,15 @@
     "ArchivalSummaryResponseTypeDef",
     "BillingModeSummaryResponseTypeDef",
     "DeleteResourcePolicyOutputTypeDef",
     "DescribeLimitsOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetResourcePolicyOutputTypeDef",
     "ListTablesOutputTypeDef",
+    "OnDemandThroughputResponseTypeDef",
     "ProvisionedThroughputDescriptionResponseTypeDef",
     "PutResourcePolicyOutputTypeDef",
     "RestoreSummaryResponseTypeDef",
     "SSEDescriptionResponseTypeDef",
     "StreamSpecificationResponseTypeDef",
     "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
@@ -500,14 +503,21 @@
 KeySchemaElementTypeDef = TypedDict(
     "KeySchemaElementTypeDef",
     {
         "AttributeName": str,
         "KeyType": KeyTypeType,
     },
 )
+OnDemandThroughputTypeDef = TypedDict(
+    "OnDemandThroughputTypeDef",
+    {
+        "MaxReadRequestUnits": NotRequired[int],
+        "MaxWriteRequestUnits": NotRequired[int],
+    },
+)
 ProjectionTypeDef = TypedDict(
     "ProjectionTypeDef",
     {
         "ProjectionType": NotRequired[ProjectionTypeType],
         "NonKeyAttributes": NotRequired[Sequence[str]],
     },
 )
@@ -526,14 +536,20 @@
 )
 CreateReplicaActionTypeDef = TypedDict(
     "CreateReplicaActionTypeDef",
     {
         "RegionName": str,
     },
 )
+OnDemandThroughputOverrideTypeDef = TypedDict(
+    "OnDemandThroughputOverrideTypeDef",
+    {
+        "MaxReadRequestUnits": NotRequired[int],
+    },
+)
 ProvisionedThroughputOverrideTypeDef = TypedDict(
     "ProvisionedThroughputOverrideTypeDef",
     {
         "ReadCapacityUnits": NotRequired[int],
     },
 )
 SSESpecificationTypeDef = TypedDict(
@@ -960,14 +976,22 @@
     "ListTablesOutputTypeDef",
     {
         "TableNames": List[str],
         "LastEvaluatedTableName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+OnDemandThroughputResponseTypeDef = TypedDict(
+    "OnDemandThroughputResponseTypeDef",
+    {
+        "MaxReadRequestUnits": int,
+        "MaxWriteRequestUnits": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ProvisionedThroughputDescriptionResponseTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionResponseTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
@@ -1248,44 +1272,48 @@
 CreateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "CreateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 GlobalSecondaryIndexTypeDef = TypedDict(
     "GlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 SourceTableDetailsTypeDef = TypedDict(
     "SourceTableDetailsTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "KeySchema": List[KeySchemaElementTypeDef],
         "TableCreationDateTime": datetime,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
         "TableArn": NotRequired[str],
         "TableSizeBytes": NotRequired[int],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
         "ItemCount": NotRequired[int],
         "BillingMode": NotRequired[BillingModeType],
     },
 )
 UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 CreateGlobalTableInputRequestTypeDef = TypedDict(
     "CreateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicationGroup": Sequence[ReplicaTypeDef],
@@ -1299,21 +1327,23 @@
     },
 )
 ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": NotRequired[str],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputOverrideTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputOverrideTypeDef],
     },
 )
 ReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputOverrideTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputOverrideTypeDef],
     },
 )
 ListTagsOfResourceOutputTypeDef = TypedDict(
     "ListTagsOfResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1486,32 +1516,35 @@
         "Projection": NotRequired[ProjectionExtraOutputTypeDef],
         "IndexStatus": NotRequired[IndexStatusType],
         "Backfilling": NotRequired[bool],
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputDescriptionTypeDef],
         "IndexSizeBytes": NotRequired[int],
         "ItemCount": NotRequired[int],
         "IndexArn": NotRequired[str],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 GlobalSecondaryIndexInfoTypeDef = TypedDict(
     "GlobalSecondaryIndexInfoTypeDef",
     {
         "IndexName": NotRequired[str],
         "KeySchema": NotRequired[List[KeySchemaElementTypeDef]],
         "Projection": NotRequired[ProjectionOutputTypeDef],
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 GlobalSecondaryIndexOutputTypeDef = TypedDict(
     "GlobalSecondaryIndexOutputTypeDef",
     {
         "IndexName": str,
         "KeySchema": List[KeySchemaElementTypeDef],
         "Projection": ProjectionOutputTypeDef,
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 LocalSecondaryIndexInfoTypeDef = TypedDict(
     "LocalSecondaryIndexInfoTypeDef",
     {
         "IndexName": NotRequired[str],
         "KeySchema": NotRequired[List[KeySchemaElementTypeDef]],
@@ -2059,14 +2092,15 @@
     "TableCreationParametersTypeDef",
     {
         "TableName": str,
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "BillingMode": NotRequired[BillingModeType],
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "GlobalSecondaryIndexes": NotRequired[Sequence[GlobalSecondaryIndexTypeDef]],
     },
 )
 GlobalSecondaryIndexUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTypeDef",
     {
@@ -2088,35 +2122,38 @@
     {
         "RegionName": NotRequired[str],
         "ReplicaStatus": NotRequired[ReplicaStatusType],
         "ReplicaStatusDescription": NotRequired[str],
         "ReplicaStatusPercentProgress": NotRequired[str],
         "KMSMasterKeyId": NotRequired[str],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputOverrideTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputOverrideTypeDef],
         "GlobalSecondaryIndexes": NotRequired[List[ReplicaGlobalSecondaryIndexDescriptionTypeDef]],
         "ReplicaInaccessibleDateTime": NotRequired[datetime],
         "ReplicaTableClassSummary": NotRequired[TableClassSummaryTypeDef],
     },
 )
 CreateReplicationGroupMemberActionTypeDef = TypedDict(
     "CreateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
         "KMSMasterKeyId": NotRequired[str],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputOverrideTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputOverrideTypeDef],
         "GlobalSecondaryIndexes": NotRequired[Sequence[ReplicaGlobalSecondaryIndexTypeDef]],
         "TableClassOverride": NotRequired[TableClassType],
     },
 )
 UpdateReplicationGroupMemberActionTypeDef = TypedDict(
     "UpdateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
         "KMSMasterKeyId": NotRequired[str],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputOverrideTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputOverrideTypeDef],
         "GlobalSecondaryIndexes": NotRequired[Sequence[ReplicaGlobalSecondaryIndexTypeDef]],
         "TableClassOverride": NotRequired[TableClassType],
     },
 )
 InputFormatOptionsUnionTypeDef = Union[InputFormatOptionsTypeDef, InputFormatOptionsOutputTypeDef]
 UpdateGlobalTableInputRequestTypeDef = TypedDict(
     "UpdateGlobalTableInputRequestTypeDef",
@@ -2165,14 +2202,15 @@
     "TableCreationParametersOutputTypeDef",
     {
         "TableName": str,
         "AttributeDefinitions": List[AttributeDefinitionTypeDef],
         "KeySchema": List[KeySchemaElementTypeDef],
         "BillingMode": NotRequired[BillingModeType],
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "GlobalSecondaryIndexes": NotRequired[List[GlobalSecondaryIndexOutputTypeDef]],
     },
 )
 SourceTableFeatureDetailsTypeDef = TypedDict(
     "SourceTableFeatureDetailsTypeDef",
     {
@@ -2504,14 +2542,15 @@
         "GlobalTableVersion": NotRequired[str],
         "Replicas": NotRequired[List[ReplicaDescriptionTypeDef]],
         "RestoreSummary": NotRequired[RestoreSummaryTypeDef],
         "SSEDescription": NotRequired[SSEDescriptionTypeDef],
         "ArchivalSummary": NotRequired[ArchivalSummaryTypeDef],
         "TableClassSummary": NotRequired[TableClassSummaryTypeDef],
         "DeletionProtectionEnabled": NotRequired[bool],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 ReplicationGroupUpdateTypeDef = TypedDict(
     "ReplicationGroupUpdateTypeDef",
     {
         "Create": NotRequired[CreateReplicationGroupMemberActionTypeDef],
         "Update": NotRequired[UpdateReplicationGroupMemberActionTypeDef],
@@ -2530,14 +2569,15 @@
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
         "StreamSpecification": NotRequired[StreamSpecificationTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "TableClass": NotRequired[TableClassType],
         "DeletionProtectionEnabled": NotRequired[bool],
         "ResourcePolicy": NotRequired[str],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 CreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
     "CreateTableInputServiceResourceCreateTableTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "TableName": str,
@@ -2548,25 +2588,27 @@
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
         "StreamSpecification": NotRequired[StreamSpecificationTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "TableClass": NotRequired[TableClassType],
         "DeletionProtectionEnabled": NotRequired[bool],
         "ResourcePolicy": NotRequired[str],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 RestoreTableFromBackupInputRequestTypeDef = TypedDict(
     "RestoreTableFromBackupInputRequestTypeDef",
     {
         "TargetTableName": str,
         "BackupArn": str,
         "BillingModeOverride": NotRequired[BillingModeType],
         "GlobalSecondaryIndexOverride": NotRequired[Sequence[GlobalSecondaryIndexUnionTypeDef]],
         "LocalSecondaryIndexOverride": NotRequired[Sequence[LocalSecondaryIndexTypeDef]],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputTypeDef],
         "SSESpecificationOverride": NotRequired[SSESpecificationTypeDef],
     },
 )
 RestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
     "RestoreTableToPointInTimeInputRequestTypeDef",
     {
         "TargetTableName": str,
@@ -2574,14 +2616,15 @@
         "SourceTableName": NotRequired[str],
         "UseLatestRestorableTime": NotRequired[bool],
         "RestoreDateTime": NotRequired[TimestampTypeDef],
         "BillingModeOverride": NotRequired[BillingModeType],
         "GlobalSecondaryIndexOverride": NotRequired[Sequence[GlobalSecondaryIndexUnionTypeDef]],
         "LocalSecondaryIndexOverride": NotRequired[Sequence[LocalSecondaryIndexTypeDef]],
         "ProvisionedThroughputOverride": NotRequired[ProvisionedThroughputTypeDef],
+        "OnDemandThroughputOverride": NotRequired[OnDemandThroughputTypeDef],
         "SSESpecificationOverride": NotRequired[SSESpecificationTypeDef],
     },
 )
 ImportTableDescriptionTypeDef = TypedDict(
     "ImportTableDescriptionTypeDef",
     {
         "ImportArn": NotRequired[str],
@@ -2782,28 +2825,30 @@
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
         "GlobalSecondaryIndexUpdates": NotRequired[Sequence[GlobalSecondaryIndexUpdateTypeDef]],
         "StreamSpecification": NotRequired[StreamSpecificationTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "ReplicaUpdates": NotRequired[Sequence[ReplicationGroupUpdateTypeDef]],
         "TableClass": NotRequired[TableClassType],
         "DeletionProtectionEnabled": NotRequired[bool],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 UpdateTableInputTableUpdateTypeDef = TypedDict(
     "UpdateTableInputTableUpdateTypeDef",
     {
         "AttributeDefinitions": NotRequired[Sequence[AttributeDefinitionTypeDef]],
         "BillingMode": NotRequired[BillingModeType],
         "ProvisionedThroughput": NotRequired[ProvisionedThroughputTypeDef],
         "GlobalSecondaryIndexUpdates": NotRequired[Sequence[GlobalSecondaryIndexUpdateTypeDef]],
         "StreamSpecification": NotRequired[StreamSpecificationTypeDef],
         "SSESpecification": NotRequired[SSESpecificationTypeDef],
         "ReplicaUpdates": NotRequired[Sequence[ReplicationGroupUpdateTypeDef]],
         "TableClass": NotRequired[TableClassType],
         "DeletionProtectionEnabled": NotRequired[bool],
+        "OnDemandThroughput": NotRequired[OnDemandThroughputTypeDef],
     },
 )
 DescribeImportOutputTypeDef = TypedDict(
     "DescribeImportOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/waiter.py` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb/waiter.pyi` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb.egg-info/PKG-INFO` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.34.91
-Summary: Type annotations for boto3.DynamoDB 1.34.91 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.97
+Summary: Type annotations for boto3.DynamoDB 1.34.97 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodb)](https://pepy.tech/project/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_dynamodb-1.34.91/mypy_boto3_dynamodb.egg-info/SOURCES.txt` & `mypy_boto3_dynamodb-1.34.97/mypy_boto3_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_dynamodb-1.34.91/setup.py` & `mypy_boto3_dynamodb-1.34.97/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodb",
-    version="1.34.91",
+    version="1.34.97",
     packages=["mypy_boto3_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.DynamoDB 1.34.91 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.DynamoDB 1.34.97 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

