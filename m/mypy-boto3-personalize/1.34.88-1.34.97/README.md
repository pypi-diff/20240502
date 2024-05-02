# Comparing `tmp/mypy_boto3_personalize-1.34.88.tar.gz` & `tmp/mypy_boto3_personalize-1.34.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_personalize-1.34.88.tar", last modified: Fri Apr 19 19:32:14 2024, max compression
+gzip compressed data, was "mypy_boto3_personalize-1.34.97.tar", last modified: Thu May  2 19:33:15 2024, max compression
```

## Comparing `mypy_boto3_personalize-1.34.88.tar` & `mypy_boto3_personalize-1.34.97.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:14.733938 mypy_boto3_personalize-1.34.88/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-04-19 19:32:14.729938 mypy_boto3_personalize-1.34.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13478 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:14.729938 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51875 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    51872 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18712 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    65297 2024-04-19 19:32:03.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    65297 2024-04-19 19:32:02.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:14.729938 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:32:14.733938 mypy_boto3_personalize-1.34.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:15.766125 mypy_boto3_personalize-1.34.97/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-05-02 19:33:15.766125 mypy_boto3_personalize-1.34.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13478 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:15.766125 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54112 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54109 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18694 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    70757 2024-05-02 19:32:59.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70757 2024-05-02 19:32:58.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:33:15.766125 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-05-02 19:33:15.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-02 19:33:15.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:33:15.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:33:15.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 19:33:15.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 19:33:15.000000 mypy_boto3_personalize-1.34.97/mypy_boto3_personalize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:33:15.766125 mypy_boto3_personalize-1.34.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-02 19:32:57.000000 mypy_boto3_personalize-1.34.97/setup.py
```

### Comparing `mypy_boto3_personalize-1.34.88/LICENSE` & `mypy_boto3_personalize-1.34.97/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_personalize-1.34.88/PKG-INFO` & `mypy_boto3_personalize-1.34.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.34.88
-Summary: Type annotations for boto3.Personalize 1.34.88 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.97
+Summary: Type annotations for boto3.Personalize 1.34.97 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize)](https://pepy.tech/project/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.34.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
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
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_personalize-1.34.88/README.md` & `mypy_boto3_personalize-1.34.97/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize)](https://pepy.tech/project/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.34.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
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
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__init__.py` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__init__.pyi` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__main__.py` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Personalize 1.34.88\n"
-        "Version:         1.34.88\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.Personalize 1.34.97\n"
+        "Version:         1.34.97\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.88")
+    print("1.34.97")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/client.py` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,24 @@
     ListRecipesPaginator,
     ListRecommendersPaginator,
     ListSchemasPaginator,
     ListSolutionsPaginator,
     ListSolutionVersionsPaginator,
 )
 from .type_defs import (
-    BatchInferenceJobConfigTypeDef,
+    BatchInferenceJobConfigUnionTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
-    CampaignConfigTypeDef,
+    CampaignConfigUnionTypeDef,
     CreateBatchInferenceJobResponseTypeDef,
     CreateBatchSegmentJobResponseTypeDef,
     CreateCampaignResponseTypeDef,
+    CreateDataDeletionJobResponseTypeDef,
     CreateDatasetExportJobResponseTypeDef,
     CreateDatasetGroupResponseTypeDef,
     CreateDatasetImportJobResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateEventTrackerResponseTypeDef,
     CreateFilterResponseTypeDef,
     CreateMetricAttributionResponseTypeDef,
@@ -67,14 +68,15 @@
     CreateSolutionVersionResponseTypeDef,
     DatasetExportJobOutputTypeDef,
     DataSourceTypeDef,
     DescribeAlgorithmResponseTypeDef,
     DescribeBatchInferenceJobResponseTypeDef,
     DescribeBatchSegmentJobResponseTypeDef,
     DescribeCampaignResponseTypeDef,
+    DescribeDataDeletionJobResponseTypeDef,
     DescribeDatasetExportJobResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeEventTrackerResponseTypeDef,
     DescribeFeatureTransformationResponseTypeDef,
     DescribeFilterResponseTypeDef,
@@ -85,14 +87,15 @@
     DescribeSolutionResponseTypeDef,
     DescribeSolutionVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetSolutionMetricsResponseTypeDef,
     ListBatchInferenceJobsResponseTypeDef,
     ListBatchSegmentJobsResponseTypeDef,
     ListCampaignsResponseTypeDef,
+    ListDataDeletionJobsResponseTypeDef,
     ListDatasetExportJobsResponseTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListEventTrackersResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListMetricAttributionMetricsResponseTypeDef,
@@ -101,16 +104,16 @@
     ListRecommendersResponseTypeDef,
     ListSchemasResponseTypeDef,
     ListSolutionsResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetricAttributeTypeDef,
     MetricAttributionOutputTypeDef,
-    RecommenderConfigTypeDef,
-    SolutionConfigTypeDef,
+    RecommenderConfigUnionTypeDef,
+    SolutionConfigUnionTypeDef,
     StartRecommenderResponseTypeDef,
     StopRecommenderResponseTypeDef,
     TagTypeDef,
     ThemeGenerationConfigTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
@@ -120,35 +123,32 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("PersonalizeClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InvalidInputException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TooManyTagKeysException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
-
 class PersonalizeClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/)
     """
 
     meta: ClientMeta
@@ -184,15 +184,15 @@
         jobName: str,
         solutionVersionArn: str,
         jobInput: BatchInferenceJobInputTypeDef,
         jobOutput: BatchInferenceJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
-        batchInferenceJobConfig: BatchInferenceJobConfigTypeDef = ...,
+        batchInferenceJobConfig: BatchInferenceJobConfigUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         batchInferenceJobMode: BatchInferenceJobModeType = ...,
         themeGenerationConfig: ThemeGenerationConfigTypeDef = ...,
     ) -> CreateBatchInferenceJobResponseTypeDef:
         """
         Generates batch recommendations based on a list of items or users stored in
         Amazon S3 and exports the recommendations to an Amazon S3
@@ -223,24 +223,42 @@
 
     def create_campaign(
         self,
         *,
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
-        campaignConfig: CampaignConfigTypeDef = ...,
+        campaignConfig: CampaignConfigUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCampaignResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_campaign)
         """
 
+    def create_data_deletion_job(
+        self,
+        *,
+        jobName: str,
+        datasetGroupArn: str,
+        dataSource: DataSourceTypeDef,
+        roleArn: str,
+        tags: Sequence[TagTypeDef] = ...,
+    ) -> CreateDataDeletionJobResponseTypeDef:
+        """
+        Creates a batch job that deletes all references to specific users from an
+        Amazon Personalize dataset group in
+        batches.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_data_deletion_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_data_deletion_job)
+        """
+
     def create_dataset(
         self,
         *,
         name: str,
         schemaArn: str,
         datasetGroupArn: str,
         datasetType: str,
@@ -351,15 +369,15 @@
 
     def create_recommender(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         recipeArn: str,
-        recommenderConfig: RecommenderConfigTypeDef = ...,
+        recommenderConfig: RecommenderConfigUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRecommenderResponseTypeDef:
         """
         Creates a recommender with the recipe (a Domain dataset group use case) you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)
@@ -382,15 +400,15 @@
         name: str,
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
         performAutoTraining: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
-        solutionConfig: SolutionConfigTypeDef = ...,
+        solutionConfig: SolutionConfigUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSolutionResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution)
@@ -523,14 +541,27 @@
         """
         Describes the given campaign, including its status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_campaign)
         """
 
+    def describe_data_deletion_job(
+        self, *, dataDeletionJobArn: str
+    ) -> DescribeDataDeletionJobResponseTypeDef:
+        """
+        Describes the data deletion job created by
+        [CreateDataDeletionJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDataDeletionJob.html),
+        including the job
+        status.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_data_deletion_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_data_deletion_job)
+        """
+
     def describe_dataset(self, *, datasetArn: str) -> DescribeDatasetResponseTypeDef:
         """
         Describes the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset)
         """
@@ -703,14 +734,26 @@
         """
         Returns a list of campaigns that use the given solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_campaigns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_campaigns)
         """
 
+    def list_data_deletion_jobs(
+        self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
+    ) -> ListDataDeletionJobsResponseTypeDef:
+        """
+        Returns a list of data deletion jobs for a dataset group ordered by creation
+        time, with the most recent
+        first.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_data_deletion_jobs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_data_deletion_jobs)
+        """
+
     def list_dataset_export_jobs(
         self, *, datasetArn: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListDatasetExportJobsResponseTypeDef:
         """
         Returns a list of dataset export jobs that use the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_export_jobs)
@@ -899,15 +942,15 @@
 
     def update_campaign(
         self,
         *,
         campaignArn: str,
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
-        campaignConfig: CampaignConfigTypeDef = ...,
+        campaignConfig: CampaignConfigUnionTypeDef = ...,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign to deploy a retrained solution version with an existing
         campaign, change your campaign's `minProvisionedTPS`, or modify your campaign's
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
@@ -934,15 +977,15 @@
         Updates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_metric_attribution)
         """
 
     def update_recommender(
-        self, *, recommenderArn: str, recommenderConfig: RecommenderConfigTypeDef
+        self, *, recommenderArn: str, recommenderConfig: RecommenderConfigUnionTypeDef
     ) -> UpdateRecommenderResponseTypeDef:
         """
         Updates the recommender to modify the recommender configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_recommender)
         """
```

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/client.pyi` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,24 @@
     ListRecipesPaginator,
     ListRecommendersPaginator,
     ListSchemasPaginator,
     ListSolutionsPaginator,
     ListSolutionVersionsPaginator,
 )
 from .type_defs import (
-    BatchInferenceJobConfigTypeDef,
+    BatchInferenceJobConfigUnionTypeDef,
     BatchInferenceJobInputTypeDef,
     BatchInferenceJobOutputTypeDef,
     BatchSegmentJobInputTypeDef,
     BatchSegmentJobOutputTypeDef,
-    CampaignConfigTypeDef,
+    CampaignConfigUnionTypeDef,
     CreateBatchInferenceJobResponseTypeDef,
     CreateBatchSegmentJobResponseTypeDef,
     CreateCampaignResponseTypeDef,
+    CreateDataDeletionJobResponseTypeDef,
     CreateDatasetExportJobResponseTypeDef,
     CreateDatasetGroupResponseTypeDef,
     CreateDatasetImportJobResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateEventTrackerResponseTypeDef,
     CreateFilterResponseTypeDef,
     CreateMetricAttributionResponseTypeDef,
@@ -67,14 +68,15 @@
     CreateSolutionVersionResponseTypeDef,
     DatasetExportJobOutputTypeDef,
     DataSourceTypeDef,
     DescribeAlgorithmResponseTypeDef,
     DescribeBatchInferenceJobResponseTypeDef,
     DescribeBatchSegmentJobResponseTypeDef,
     DescribeCampaignResponseTypeDef,
+    DescribeDataDeletionJobResponseTypeDef,
     DescribeDatasetExportJobResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeEventTrackerResponseTypeDef,
     DescribeFeatureTransformationResponseTypeDef,
     DescribeFilterResponseTypeDef,
@@ -85,14 +87,15 @@
     DescribeSolutionResponseTypeDef,
     DescribeSolutionVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetSolutionMetricsResponseTypeDef,
     ListBatchInferenceJobsResponseTypeDef,
     ListBatchSegmentJobsResponseTypeDef,
     ListCampaignsResponseTypeDef,
+    ListDataDeletionJobsResponseTypeDef,
     ListDatasetExportJobsResponseTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListEventTrackersResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListMetricAttributionMetricsResponseTypeDef,
@@ -101,16 +104,16 @@
     ListRecommendersResponseTypeDef,
     ListSchemasResponseTypeDef,
     ListSolutionsResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MetricAttributeTypeDef,
     MetricAttributionOutputTypeDef,
-    RecommenderConfigTypeDef,
-    SolutionConfigTypeDef,
+    RecommenderConfigUnionTypeDef,
+    SolutionConfigUnionTypeDef,
     StartRecommenderResponseTypeDef,
     StopRecommenderResponseTypeDef,
     TagTypeDef,
     ThemeGenerationConfigTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateMetricAttributionResponseTypeDef,
@@ -120,32 +123,35 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("PersonalizeClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InvalidInputException: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TooManyTagKeysException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
+
 class PersonalizeClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/)
     """
 
     meta: ClientMeta
@@ -181,15 +187,15 @@
         jobName: str,
         solutionVersionArn: str,
         jobInput: BatchInferenceJobInputTypeDef,
         jobOutput: BatchInferenceJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
-        batchInferenceJobConfig: BatchInferenceJobConfigTypeDef = ...,
+        batchInferenceJobConfig: BatchInferenceJobConfigUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         batchInferenceJobMode: BatchInferenceJobModeType = ...,
         themeGenerationConfig: ThemeGenerationConfigTypeDef = ...,
     ) -> CreateBatchInferenceJobResponseTypeDef:
         """
         Generates batch recommendations based on a list of items or users stored in
         Amazon S3 and exports the recommendations to an Amazon S3
@@ -220,24 +226,42 @@
 
     def create_campaign(
         self,
         *,
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
-        campaignConfig: CampaignConfigTypeDef = ...,
+        campaignConfig: CampaignConfigUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCampaignResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_campaign)
         """
 
+    def create_data_deletion_job(
+        self,
+        *,
+        jobName: str,
+        datasetGroupArn: str,
+        dataSource: DataSourceTypeDef,
+        roleArn: str,
+        tags: Sequence[TagTypeDef] = ...,
+    ) -> CreateDataDeletionJobResponseTypeDef:
+        """
+        Creates a batch job that deletes all references to specific users from an
+        Amazon Personalize dataset group in
+        batches.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_data_deletion_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_data_deletion_job)
+        """
+
     def create_dataset(
         self,
         *,
         name: str,
         schemaArn: str,
         datasetGroupArn: str,
         datasetType: str,
@@ -348,15 +372,15 @@
 
     def create_recommender(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         recipeArn: str,
-        recommenderConfig: RecommenderConfigTypeDef = ...,
+        recommenderConfig: RecommenderConfigUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRecommenderResponseTypeDef:
         """
         Creates a recommender with the recipe (a Domain dataset group use case) you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)
@@ -379,15 +403,15 @@
         name: str,
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
         performAutoTraining: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
-        solutionConfig: SolutionConfigTypeDef = ...,
+        solutionConfig: SolutionConfigUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSolutionResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution)
@@ -520,14 +544,27 @@
         """
         Describes the given campaign, including its status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_campaign)
         """
 
+    def describe_data_deletion_job(
+        self, *, dataDeletionJobArn: str
+    ) -> DescribeDataDeletionJobResponseTypeDef:
+        """
+        Describes the data deletion job created by
+        [CreateDataDeletionJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDataDeletionJob.html),
+        including the job
+        status.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_data_deletion_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_data_deletion_job)
+        """
+
     def describe_dataset(self, *, datasetArn: str) -> DescribeDatasetResponseTypeDef:
         """
         Describes the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#describe_dataset)
         """
@@ -700,14 +737,26 @@
         """
         Returns a list of campaigns that use the given solution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_campaigns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_campaigns)
         """
 
+    def list_data_deletion_jobs(
+        self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
+    ) -> ListDataDeletionJobsResponseTypeDef:
+        """
+        Returns a list of data deletion jobs for a dataset group ordered by creation
+        time, with the most recent
+        first.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_data_deletion_jobs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_data_deletion_jobs)
+        """
+
     def list_dataset_export_jobs(
         self, *, datasetArn: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListDatasetExportJobsResponseTypeDef:
         """
         Returns a list of dataset export jobs that use the given dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_export_jobs)
@@ -896,15 +945,15 @@
 
     def update_campaign(
         self,
         *,
         campaignArn: str,
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
-        campaignConfig: CampaignConfigTypeDef = ...,
+        campaignConfig: CampaignConfigUnionTypeDef = ...,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign to deploy a retrained solution version with an existing
         campaign, change your campaign's `minProvisionedTPS`, or modify your campaign's
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
@@ -931,15 +980,15 @@
         Updates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_metric_attribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_metric_attribution)
         """
 
     def update_recommender(
-        self, *, recommenderArn: str, recommenderConfig: RecommenderConfigTypeDef
+        self, *, recommenderArn: str, recommenderConfig: RecommenderConfigUnionTypeDef
     ) -> UpdateRecommenderResponseTypeDef:
         """
         Updates the recommender to modify the recommender configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_recommender)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_recommender)
         """
```

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/literals.py` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,14 +380,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/literals.pyi` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -380,14 +380,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/paginator.py` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListEventTrackersResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListMetricAttributionMetricsResponseTypeDef,
     ListMetricAttributionsResponseTypeDef,
     ListRecipesResponseTypeDef,
-    ListRecommendersResponsePaginatorTypeDef,
+    ListRecommendersResponseTypeDef,
     ListSchemasResponseTypeDef,
     ListSolutionsResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 12):
@@ -298,15 +298,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListRecommendersResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListRecommendersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
         """
 
 
 class ListSchemasPaginator(Paginator):
```

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/paginator.pyi` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListEventTrackersResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListMetricAttributionMetricsResponseTypeDef,
     ListMetricAttributionsResponseTypeDef,
     ListRecipesResponseTypeDef,
-    ListRecommendersResponsePaginatorTypeDef,
+    ListRecommendersResponseTypeDef,
     ListSchemasResponseTypeDef,
     ListSolutionsResponseTypeDef,
     ListSolutionVersionsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 12):
@@ -284,15 +284,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
     """
 
     def paginate(
         self, *, datasetGroupArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListRecommendersResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListRecommendersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/paginators/#listrecommenderspaginator)
         """
 
 class ListSchemasPaginator(Paginator):
     """
```

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/type_defs.py` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AlgorithmImageTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BatchInferenceJobModeType,
     DomainType,
     ImportModeType,
     IngestionModeType,
     ObjectiveSensitivityType,
@@ -37,30 +37,35 @@
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlgorithmImageTypeDef",
+    "AutoMLConfigOutputTypeDef",
     "AutoMLConfigTypeDef",
     "AutoMLResultTypeDef",
     "AutoTrainingConfigTypeDef",
+    "BatchInferenceJobConfigOutputTypeDef",
     "BatchInferenceJobConfigTypeDef",
     "S3DataConfigTypeDef",
     "BatchInferenceJobSummaryTypeDef",
     "BatchSegmentJobSummaryTypeDef",
+    "CampaignConfigOutputTypeDef",
     "CampaignConfigTypeDef",
     "CampaignSummaryTypeDef",
+    "CategoricalHyperParameterRangeOutputTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DataSourceTypeDef",
     "MetricAttributeTypeDef",
     "CreateSchemaRequestRequestTypeDef",
+    "DataDeletionJobSummaryTypeDef",
     "DatasetExportJobSummaryTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetGroupTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DatasetSchemaSummaryTypeDef",
     "DatasetSchemaTypeDef",
     "DatasetSummaryTypeDef",
@@ -77,14 +82,15 @@
     "DeleteRecommenderRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteSolutionRequestRequestTypeDef",
     "DescribeAlgorithmRequestRequestTypeDef",
     "DescribeBatchInferenceJobRequestRequestTypeDef",
     "DescribeBatchSegmentJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
+    "DescribeDataDeletionJobRequestRequestTypeDef",
     "DescribeDatasetExportJobRequestRequestTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeEventTrackerRequestRequestTypeDef",
     "EventTrackerTypeDef",
     "DescribeFeatureTransformationRequestRequestTypeDef",
@@ -105,14 +111,15 @@
     "HPOObjectiveTypeDef",
     "HPOResourceConfigTypeDef",
     "IntegerHyperParameterRangeTypeDef",
     "PaginatorConfigTypeDef",
     "ListBatchInferenceJobsRequestRequestTypeDef",
     "ListBatchSegmentJobsRequestRequestTypeDef",
     "ListCampaignsRequestRequestTypeDef",
+    "ListDataDeletionJobsRequestRequestTypeDef",
     "ListDatasetExportJobsRequestRequestTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListEventTrackersRequestRequestTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "ListMetricAttributionMetricsRequestRequestTypeDef",
@@ -124,40 +131,44 @@
     "ListSchemasRequestRequestTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
     "SolutionVersionSummaryTypeDef",
     "ListSolutionsRequestRequestTypeDef",
     "SolutionSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OptimizationObjectiveTypeDef",
-    "TrainingDataConfigPaginatorTypeDef",
+    "TrainingDataConfigExtraOutputTypeDef",
+    "TrainingDataConfigOutputTypeDef",
     "TrainingDataConfigTypeDef",
     "TunedHPOParamsTypeDef",
     "StartRecommenderRequestRequestTypeDef",
     "StopRecommenderRequestRequestTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
+    "BatchInferenceJobConfigUnionTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
     "MetricAttributionOutputTypeDef",
     "CampaignUpdateSummaryTypeDef",
+    "CampaignConfigUnionTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateEventTrackerRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateSolutionVersionRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateBatchInferenceJobResponseTypeDef",
     "CreateBatchSegmentJobResponseTypeDef",
     "CreateCampaignResponseTypeDef",
+    "CreateDataDeletionJobResponseTypeDef",
     "CreateDatasetExportJobResponseTypeDef",
     "CreateDatasetGroupResponseTypeDef",
     "CreateDatasetImportJobResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateEventTrackerResponseTypeDef",
     "CreateFilterResponseTypeDef",
     "CreateMetricAttributionResponseTypeDef",
@@ -173,17 +184,20 @@
     "ListTagsForResourceResponseTypeDef",
     "StartRecommenderResponseTypeDef",
     "StopRecommenderResponseTypeDef",
     "UpdateCampaignResponseTypeDef",
     "UpdateDatasetResponseTypeDef",
     "UpdateMetricAttributionResponseTypeDef",
     "UpdateRecommenderResponseTypeDef",
+    "CreateDataDeletionJobRequestRequestTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
+    "DataDeletionJobTypeDef",
     "DatasetImportJobTypeDef",
     "ListMetricAttributionMetricsResponseTypeDef",
+    "ListDataDeletionJobsResponseTypeDef",
     "ListDatasetExportJobsResponseTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "DescribeSchemaResponseTypeDef",
     "ListDatasetsResponseTypeDef",
@@ -192,14 +206,15 @@
     "DescribeEventTrackerResponseTypeDef",
     "DescribeFeatureTransformationResponseTypeDef",
     "DescribeFilterResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "ListEventTrackersResponseTypeDef",
     "ThemeGenerationConfigTypeDef",
     "ListFiltersResponseTypeDef",
+    "HyperParameterRangesOutputTypeDef",
     "HyperParameterRangesTypeDef",
     "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
     "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
     "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
@@ -213,60 +228,71 @@
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListMetricAttributionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
     "ListSolutionVersionsResponseTypeDef",
     "ListSolutionsResponseTypeDef",
-    "RecommenderConfigPaginatorTypeDef",
+    "RecommenderConfigExtraOutputTypeDef",
+    "RecommenderConfigOutputTypeDef",
     "RecommenderConfigTypeDef",
     "BatchSegmentJobTypeDef",
     "CreateBatchSegmentJobRequestRequestTypeDef",
     "CreateDatasetExportJobRequestRequestTypeDef",
     "DatasetExportJobTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
     "MetricAttributionTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
     "CampaignTypeDef",
+    "DescribeDataDeletionJobResponseTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "AlgorithmTypeDef",
     "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
+    "HPOConfigOutputTypeDef",
     "HPOConfigTypeDef",
-    "RecommenderSummaryPaginatorTypeDef",
-    "CreateRecommenderRequestRequestTypeDef",
     "RecommenderSummaryTypeDef",
     "RecommenderUpdateSummaryTypeDef",
+    "CreateRecommenderRequestRequestTypeDef",
+    "RecommenderConfigUnionTypeDef",
     "UpdateRecommenderRequestRequestTypeDef",
     "DescribeBatchSegmentJobResponseTypeDef",
     "DescribeDatasetExportJobResponseTypeDef",
     "DescribeMetricAttributionResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
     "DescribeAlgorithmResponseTypeDef",
     "DescribeBatchInferenceJobResponseTypeDef",
+    "SolutionConfigOutputTypeDef",
     "SolutionConfigTypeDef",
-    "ListRecommendersResponsePaginatorTypeDef",
     "ListRecommendersResponseTypeDef",
     "RecommenderTypeDef",
-    "CreateSolutionRequestRequestTypeDef",
     "SolutionTypeDef",
     "SolutionVersionTypeDef",
+    "CreateSolutionRequestRequestTypeDef",
+    "SolutionConfigUnionTypeDef",
     "DescribeRecommenderResponseTypeDef",
     "DescribeSolutionResponseTypeDef",
     "DescribeSolutionVersionResponseTypeDef",
 )
 
 AlgorithmImageTypeDef = TypedDict(
     "AlgorithmImageTypeDef",
     {
         "dockerURI": str,
         "name": NotRequired[str],
     },
 )
+AutoMLConfigOutputTypeDef = TypedDict(
+    "AutoMLConfigOutputTypeDef",
+    {
+        "metricName": NotRequired[str],
+        "recipeList": NotRequired[List[str]],
+    },
+)
 AutoMLConfigTypeDef = TypedDict(
     "AutoMLConfigTypeDef",
     {
         "metricName": NotRequired[str],
         "recipeList": NotRequired[Sequence[str]],
     },
 )
@@ -278,14 +304,20 @@
 )
 AutoTrainingConfigTypeDef = TypedDict(
     "AutoTrainingConfigTypeDef",
     {
         "schedulingExpression": NotRequired[str],
     },
 )
+BatchInferenceJobConfigOutputTypeDef = TypedDict(
+    "BatchInferenceJobConfigOutputTypeDef",
+    {
+        "itemExplorationConfig": NotRequired[Dict[str, str]],
+    },
+)
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
     {
         "itemExplorationConfig": NotRequired[Mapping[str, str]],
     },
 )
 S3DataConfigTypeDef = TypedDict(
@@ -316,14 +348,22 @@
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "failureReason": NotRequired[str],
         "solutionVersionArn": NotRequired[str],
     },
 )
+CampaignConfigOutputTypeDef = TypedDict(
+    "CampaignConfigOutputTypeDef",
+    {
+        "itemExplorationConfig": NotRequired[Dict[str, str]],
+        "enableMetadataWithRecommendations": NotRequired[bool],
+        "syncWithLatestSolutionVersion": NotRequired[bool],
+    },
+)
 CampaignConfigTypeDef = TypedDict(
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": NotRequired[Mapping[str, str]],
         "enableMetadataWithRecommendations": NotRequired[bool],
         "syncWithLatestSolutionVersion": NotRequired[bool],
     },
@@ -335,14 +375,21 @@
         "campaignArn": NotRequired[str],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "failureReason": NotRequired[str],
     },
 )
+CategoricalHyperParameterRangeOutputTypeDef = TypedDict(
+    "CategoricalHyperParameterRangeOutputTypeDef",
+    {
+        "name": NotRequired[str],
+        "values": NotRequired[List[str]],
+    },
+)
 CategoricalHyperParameterRangeTypeDef = TypedDict(
     "CategoricalHyperParameterRangeTypeDef",
     {
         "name": NotRequired[str],
         "values": NotRequired[Sequence[str]],
     },
 )
@@ -389,14 +436,26 @@
     "CreateSchemaRequestRequestTypeDef",
     {
         "name": str,
         "schema": str,
         "domain": NotRequired[DomainType],
     },
 )
+DataDeletionJobSummaryTypeDef = TypedDict(
+    "DataDeletionJobSummaryTypeDef",
+    {
+        "dataDeletionJobArn": NotRequired[str],
+        "datasetGroupArn": NotRequired[str],
+        "jobName": NotRequired[str],
+        "status": NotRequired[str],
+        "creationDateTime": NotRequired[datetime],
+        "lastUpdatedDateTime": NotRequired[datetime],
+        "failureReason": NotRequired[str],
+    },
+)
 DatasetExportJobSummaryTypeDef = TypedDict(
     "DatasetExportJobSummaryTypeDef",
     {
         "datasetExportJobArn": NotRequired[str],
         "jobName": NotRequired[str],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
@@ -584,14 +643,20 @@
 )
 DescribeCampaignRequestRequestTypeDef = TypedDict(
     "DescribeCampaignRequestRequestTypeDef",
     {
         "campaignArn": str,
     },
 )
+DescribeDataDeletionJobRequestRequestTypeDef = TypedDict(
+    "DescribeDataDeletionJobRequestRequestTypeDef",
+    {
+        "dataDeletionJobArn": str,
+    },
+)
 DescribeDatasetExportJobRequestRequestTypeDef = TypedDict(
     "DescribeDatasetExportJobRequestRequestTypeDef",
     {
         "datasetExportJobArn": str,
     },
 )
 DescribeDatasetGroupRequestRequestTypeDef = TypedDict(
@@ -802,14 +867,22 @@
     "ListCampaignsRequestRequestTypeDef",
     {
         "solutionArn": NotRequired[str],
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
     },
 )
+ListDataDeletionJobsRequestRequestTypeDef = TypedDict(
+    "ListDataDeletionJobsRequestRequestTypeDef",
+    {
+        "datasetGroupArn": NotRequired[str],
+        "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
+    },
+)
 ListDatasetExportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetExportJobsRequestRequestTypeDef",
     {
         "datasetArn": NotRequired[str],
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
     },
@@ -963,16 +1036,22 @@
 OptimizationObjectiveTypeDef = TypedDict(
     "OptimizationObjectiveTypeDef",
     {
         "itemAttribute": NotRequired[str],
         "objectiveSensitivity": NotRequired[ObjectiveSensitivityType],
     },
 )
-TrainingDataConfigPaginatorTypeDef = TypedDict(
-    "TrainingDataConfigPaginatorTypeDef",
+TrainingDataConfigExtraOutputTypeDef = TypedDict(
+    "TrainingDataConfigExtraOutputTypeDef",
+    {
+        "excludedDatasetColumns": NotRequired[Dict[str, List[str]]],
+    },
+)
+TrainingDataConfigOutputTypeDef = TypedDict(
+    "TrainingDataConfigOutputTypeDef",
     {
         "excludedDatasetColumns": NotRequired[Dict[str, List[str]]],
     },
 )
 TrainingDataConfigTypeDef = TypedDict(
     "TrainingDataConfigTypeDef",
     {
@@ -1013,14 +1092,17 @@
 UpdateDatasetRequestRequestTypeDef = TypedDict(
     "UpdateDatasetRequestRequestTypeDef",
     {
         "datasetArn": str,
         "schemaArn": str,
     },
 )
+BatchInferenceJobConfigUnionTypeDef = Union[
+    BatchInferenceJobConfigTypeDef, BatchInferenceJobConfigOutputTypeDef
+]
 BatchInferenceJobInputTypeDef = TypedDict(
     "BatchInferenceJobInputTypeDef",
     {
         "s3DataSource": S3DataConfigTypeDef,
     },
 )
 BatchInferenceJobOutputTypeDef = TypedDict(
@@ -1055,21 +1137,22 @@
     },
 )
 CampaignUpdateSummaryTypeDef = TypedDict(
     "CampaignUpdateSummaryTypeDef",
     {
         "solutionVersionArn": NotRequired[str],
         "minProvisionedTPS": NotRequired[int],
-        "campaignConfig": NotRequired[CampaignConfigTypeDef],
+        "campaignConfig": NotRequired[CampaignConfigOutputTypeDef],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
     },
 )
+CampaignConfigUnionTypeDef = Union[CampaignConfigTypeDef, CampaignConfigOutputTypeDef]
 UpdateCampaignRequestRequestTypeDef = TypedDict(
     "UpdateCampaignRequestRequestTypeDef",
     {
         "campaignArn": str,
         "solutionVersionArn": NotRequired[str],
         "minProvisionedTPS": NotRequired[int],
         "campaignConfig": NotRequired[CampaignConfigTypeDef],
@@ -1155,14 +1238,21 @@
 CreateCampaignResponseTypeDef = TypedDict(
     "CreateCampaignResponseTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDataDeletionJobResponseTypeDef = TypedDict(
+    "CreateDataDeletionJobResponseTypeDef",
+    {
+        "dataDeletionJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateDatasetExportJobResponseTypeDef = TypedDict(
     "CreateDatasetExportJobResponseTypeDef",
     {
         "datasetExportJobArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1321,26 +1411,51 @@
 UpdateRecommenderResponseTypeDef = TypedDict(
     "UpdateRecommenderResponseTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDataDeletionJobRequestRequestTypeDef = TypedDict(
+    "CreateDataDeletionJobRequestRequestTypeDef",
+    {
+        "jobName": str,
+        "datasetGroupArn": str,
+        "dataSource": DataSourceTypeDef,
+        "roleArn": str,
+        "tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
 CreateDatasetImportJobRequestRequestTypeDef = TypedDict(
     "CreateDatasetImportJobRequestRequestTypeDef",
     {
         "jobName": str,
         "datasetArn": str,
         "dataSource": DataSourceTypeDef,
         "roleArn": str,
         "tags": NotRequired[Sequence[TagTypeDef]],
         "importMode": NotRequired[ImportModeType],
         "publishAttributionMetricsToS3": NotRequired[bool],
     },
 )
+DataDeletionJobTypeDef = TypedDict(
+    "DataDeletionJobTypeDef",
+    {
+        "jobName": NotRequired[str],
+        "dataDeletionJobArn": NotRequired[str],
+        "datasetGroupArn": NotRequired[str],
+        "dataSource": NotRequired[DataSourceTypeDef],
+        "roleArn": NotRequired[str],
+        "status": NotRequired[str],
+        "numDeleted": NotRequired[int],
+        "creationDateTime": NotRequired[datetime],
+        "lastUpdatedDateTime": NotRequired[datetime],
+        "failureReason": NotRequired[str],
+    },
+)
 DatasetImportJobTypeDef = TypedDict(
     "DatasetImportJobTypeDef",
     {
         "jobName": NotRequired[str],
         "datasetImportJobArn": NotRequired[str],
         "datasetArn": NotRequired[str],
         "dataSource": NotRequired[DataSourceTypeDef],
@@ -1357,14 +1472,22 @@
     "ListMetricAttributionMetricsResponseTypeDef",
     {
         "metrics": List[MetricAttributeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListDataDeletionJobsResponseTypeDef = TypedDict(
+    "ListDataDeletionJobsResponseTypeDef",
+    {
+        "dataDeletionJobs": List[DataDeletionJobSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListDatasetExportJobsResponseTypeDef = TypedDict(
     "ListDatasetExportJobsResponseTypeDef",
     {
         "datasetExportJobs": List[DatasetExportJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1488,14 +1611,24 @@
     "ListFiltersResponseTypeDef",
     {
         "Filters": List[FilterSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+HyperParameterRangesOutputTypeDef = TypedDict(
+    "HyperParameterRangesOutputTypeDef",
+    {
+        "integerHyperParameterRanges": NotRequired[List[IntegerHyperParameterRangeTypeDef]],
+        "continuousHyperParameterRanges": NotRequired[List[ContinuousHyperParameterRangeTypeDef]],
+        "categoricalHyperParameterRanges": NotRequired[
+            List[CategoricalHyperParameterRangeOutputTypeDef]
+        ],
+    },
+)
 HyperParameterRangesTypeDef = TypedDict(
     "HyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": NotRequired[Sequence[IntegerHyperParameterRangeTypeDef]],
         "continuousHyperParameterRanges": NotRequired[
             Sequence[ContinuousHyperParameterRangeTypeDef]
         ],
@@ -1643,20 +1776,29 @@
     "ListSolutionsResponseTypeDef",
     {
         "solutions": List[SolutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-RecommenderConfigPaginatorTypeDef = TypedDict(
-    "RecommenderConfigPaginatorTypeDef",
+RecommenderConfigExtraOutputTypeDef = TypedDict(
+    "RecommenderConfigExtraOutputTypeDef",
+    {
+        "itemExplorationConfig": NotRequired[Dict[str, str]],
+        "minRecommendationRequestsPerSecond": NotRequired[int],
+        "trainingDataConfig": NotRequired[TrainingDataConfigExtraOutputTypeDef],
+        "enableMetadataWithRecommendations": NotRequired[bool],
+    },
+)
+RecommenderConfigOutputTypeDef = TypedDict(
+    "RecommenderConfigOutputTypeDef",
     {
         "itemExplorationConfig": NotRequired[Dict[str, str]],
         "minRecommendationRequestsPerSecond": NotRequired[int],
-        "trainingDataConfig": NotRequired[TrainingDataConfigPaginatorTypeDef],
+        "trainingDataConfig": NotRequired[TrainingDataConfigOutputTypeDef],
         "enableMetadataWithRecommendations": NotRequired[bool],
     },
 )
 RecommenderConfigTypeDef = TypedDict(
     "RecommenderConfigTypeDef",
     {
         "itemExplorationConfig": NotRequired[Mapping[str, str]],
@@ -1755,22 +1897,29 @@
 CampaignTypeDef = TypedDict(
     "CampaignTypeDef",
     {
         "name": NotRequired[str],
         "campaignArn": NotRequired[str],
         "solutionVersionArn": NotRequired[str],
         "minProvisionedTPS": NotRequired[int],
-        "campaignConfig": NotRequired[CampaignConfigTypeDef],
+        "campaignConfig": NotRequired[CampaignConfigOutputTypeDef],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "latestCampaignUpdate": NotRequired[CampaignUpdateSummaryTypeDef],
     },
 )
+DescribeDataDeletionJobResponseTypeDef = TypedDict(
+    "DescribeDataDeletionJobResponseTypeDef",
+    {
+        "dataDeletionJob": DataDeletionJobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeDatasetImportJobResponseTypeDef = TypedDict(
     "DescribeDatasetImportJobResponseTypeDef",
     {
         "datasetImportJob": DatasetImportJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1803,15 +1952,15 @@
         "batchInferenceJobArn": NotRequired[str],
         "filterArn": NotRequired[str],
         "failureReason": NotRequired[str],
         "solutionVersionArn": NotRequired[str],
         "numResults": NotRequired[int],
         "jobInput": NotRequired[BatchInferenceJobInputTypeDef],
         "jobOutput": NotRequired[BatchInferenceJobOutputTypeDef],
-        "batchInferenceJobConfig": NotRequired[BatchInferenceJobConfigTypeDef],
+        "batchInferenceJobConfig": NotRequired[BatchInferenceJobConfigOutputTypeDef],
         "roleArn": NotRequired[str],
         "batchInferenceJobMode": NotRequired[BatchInferenceJobModeType],
         "themeGenerationConfig": NotRequired[ThemeGenerationConfigTypeDef],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
     },
@@ -1828,68 +1977,64 @@
         "numResults": NotRequired[int],
         "batchInferenceJobConfig": NotRequired[BatchInferenceJobConfigTypeDef],
         "tags": NotRequired[Sequence[TagTypeDef]],
         "batchInferenceJobMode": NotRequired[BatchInferenceJobModeType],
         "themeGenerationConfig": NotRequired[ThemeGenerationConfigTypeDef],
     },
 )
-HPOConfigTypeDef = TypedDict(
-    "HPOConfigTypeDef",
+HPOConfigOutputTypeDef = TypedDict(
+    "HPOConfigOutputTypeDef",
     {
         "hpoObjective": NotRequired[HPOObjectiveTypeDef],
         "hpoResourceConfig": NotRequired[HPOResourceConfigTypeDef],
-        "algorithmHyperParameterRanges": NotRequired[HyperParameterRangesTypeDef],
-    },
-)
-RecommenderSummaryPaginatorTypeDef = TypedDict(
-    "RecommenderSummaryPaginatorTypeDef",
-    {
-        "name": NotRequired[str],
-        "recommenderArn": NotRequired[str],
-        "datasetGroupArn": NotRequired[str],
-        "recipeArn": NotRequired[str],
-        "recommenderConfig": NotRequired[RecommenderConfigPaginatorTypeDef],
-        "status": NotRequired[str],
-        "creationDateTime": NotRequired[datetime],
-        "lastUpdatedDateTime": NotRequired[datetime],
+        "algorithmHyperParameterRanges": NotRequired[HyperParameterRangesOutputTypeDef],
     },
 )
-CreateRecommenderRequestRequestTypeDef = TypedDict(
-    "CreateRecommenderRequestRequestTypeDef",
+HPOConfigTypeDef = TypedDict(
+    "HPOConfigTypeDef",
     {
-        "name": str,
-        "datasetGroupArn": str,
-        "recipeArn": str,
-        "recommenderConfig": NotRequired[RecommenderConfigTypeDef],
-        "tags": NotRequired[Sequence[TagTypeDef]],
+        "hpoObjective": NotRequired[HPOObjectiveTypeDef],
+        "hpoResourceConfig": NotRequired[HPOResourceConfigTypeDef],
+        "algorithmHyperParameterRanges": NotRequired[HyperParameterRangesTypeDef],
     },
 )
 RecommenderSummaryTypeDef = TypedDict(
     "RecommenderSummaryTypeDef",
     {
         "name": NotRequired[str],
         "recommenderArn": NotRequired[str],
         "datasetGroupArn": NotRequired[str],
         "recipeArn": NotRequired[str],
-        "recommenderConfig": NotRequired[RecommenderConfigTypeDef],
+        "recommenderConfig": NotRequired[RecommenderConfigOutputTypeDef],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
     },
 )
 RecommenderUpdateSummaryTypeDef = TypedDict(
     "RecommenderUpdateSummaryTypeDef",
     {
-        "recommenderConfig": NotRequired[RecommenderConfigTypeDef],
+        "recommenderConfig": NotRequired[RecommenderConfigOutputTypeDef],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
     },
 )
+CreateRecommenderRequestRequestTypeDef = TypedDict(
+    "CreateRecommenderRequestRequestTypeDef",
+    {
+        "name": str,
+        "datasetGroupArn": str,
+        "recipeArn": str,
+        "recommenderConfig": NotRequired[RecommenderConfigTypeDef],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+RecommenderConfigUnionTypeDef = Union[RecommenderConfigTypeDef, RecommenderConfigExtraOutputTypeDef]
 UpdateRecommenderRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
         "recommenderConfig": RecommenderConfigTypeDef,
     },
 )
@@ -1931,35 +2076,40 @@
 DescribeBatchInferenceJobResponseTypeDef = TypedDict(
     "DescribeBatchInferenceJobResponseTypeDef",
     {
         "batchInferenceJob": BatchInferenceJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SolutionConfigOutputTypeDef = TypedDict(
+    "SolutionConfigOutputTypeDef",
+    {
+        "eventValueThreshold": NotRequired[str],
+        "hpoConfig": NotRequired[HPOConfigOutputTypeDef],
+        "algorithmHyperParameters": NotRequired[Dict[str, str]],
+        "featureTransformationParameters": NotRequired[Dict[str, str]],
+        "autoMLConfig": NotRequired[AutoMLConfigOutputTypeDef],
+        "optimizationObjective": NotRequired[OptimizationObjectiveTypeDef],
+        "trainingDataConfig": NotRequired[TrainingDataConfigOutputTypeDef],
+        "autoTrainingConfig": NotRequired[AutoTrainingConfigTypeDef],
+    },
+)
 SolutionConfigTypeDef = TypedDict(
     "SolutionConfigTypeDef",
     {
         "eventValueThreshold": NotRequired[str],
         "hpoConfig": NotRequired[HPOConfigTypeDef],
         "algorithmHyperParameters": NotRequired[Mapping[str, str]],
         "featureTransformationParameters": NotRequired[Mapping[str, str]],
         "autoMLConfig": NotRequired[AutoMLConfigTypeDef],
         "optimizationObjective": NotRequired[OptimizationObjectiveTypeDef],
         "trainingDataConfig": NotRequired[TrainingDataConfigTypeDef],
         "autoTrainingConfig": NotRequired[AutoTrainingConfigTypeDef],
     },
 )
-ListRecommendersResponsePaginatorTypeDef = TypedDict(
-    "ListRecommendersResponsePaginatorTypeDef",
-    {
-        "recommenders": List[RecommenderSummaryPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListRecommendersResponseTypeDef = TypedDict(
     "ListRecommendersResponseTypeDef",
     {
         "recommenders": List[RecommenderSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1967,49 +2117,35 @@
 RecommenderTypeDef = TypedDict(
     "RecommenderTypeDef",
     {
         "recommenderArn": NotRequired[str],
         "datasetGroupArn": NotRequired[str],
         "name": NotRequired[str],
         "recipeArn": NotRequired[str],
-        "recommenderConfig": NotRequired[RecommenderConfigTypeDef],
+        "recommenderConfig": NotRequired[RecommenderConfigOutputTypeDef],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
         "latestRecommenderUpdate": NotRequired[RecommenderUpdateSummaryTypeDef],
         "modelMetrics": NotRequired[Dict[str, float]],
     },
 )
-CreateSolutionRequestRequestTypeDef = TypedDict(
-    "CreateSolutionRequestRequestTypeDef",
-    {
-        "name": str,
-        "datasetGroupArn": str,
-        "performHPO": NotRequired[bool],
-        "performAutoML": NotRequired[bool],
-        "performAutoTraining": NotRequired[bool],
-        "recipeArn": NotRequired[str],
-        "eventType": NotRequired[str],
-        "solutionConfig": NotRequired[SolutionConfigTypeDef],
-        "tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 SolutionTypeDef = TypedDict(
     "SolutionTypeDef",
     {
         "name": NotRequired[str],
         "solutionArn": NotRequired[str],
         "performHPO": NotRequired[bool],
         "performAutoML": NotRequired[bool],
         "performAutoTraining": NotRequired[bool],
         "recipeArn": NotRequired[str],
         "datasetGroupArn": NotRequired[str],
         "eventType": NotRequired[str],
-        "solutionConfig": NotRequired[SolutionConfigTypeDef],
+        "solutionConfig": NotRequired[SolutionConfigOutputTypeDef],
         "autoMLResult": NotRequired[AutoMLResultTypeDef],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "latestSolutionVersion": NotRequired[SolutionVersionSummaryTypeDef],
     },
 )
@@ -2020,25 +2156,40 @@
         "solutionVersionArn": NotRequired[str],
         "solutionArn": NotRequired[str],
         "performHPO": NotRequired[bool],
         "performAutoML": NotRequired[bool],
         "recipeArn": NotRequired[str],
         "eventType": NotRequired[str],
         "datasetGroupArn": NotRequired[str],
-        "solutionConfig": NotRequired[SolutionConfigTypeDef],
+        "solutionConfig": NotRequired[SolutionConfigOutputTypeDef],
         "trainingHours": NotRequired[float],
         "trainingMode": NotRequired[TrainingModeType],
         "tunedHPOParams": NotRequired[TunedHPOParamsTypeDef],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "trainingType": NotRequired[TrainingTypeType],
     },
 )
+CreateSolutionRequestRequestTypeDef = TypedDict(
+    "CreateSolutionRequestRequestTypeDef",
+    {
+        "name": str,
+        "datasetGroupArn": str,
+        "performHPO": NotRequired[bool],
+        "performAutoML": NotRequired[bool],
+        "performAutoTraining": NotRequired[bool],
+        "recipeArn": NotRequired[str],
+        "eventType": NotRequired[str],
+        "solutionConfig": NotRequired[SolutionConfigTypeDef],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+SolutionConfigUnionTypeDef = Union[SolutionConfigTypeDef, SolutionConfigOutputTypeDef]
 DescribeRecommenderResponseTypeDef = TypedDict(
     "DescribeRecommenderResponseTypeDef",
     {
         "recommender": RecommenderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/type_defs.pyi` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AlgorithmImageTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BatchInferenceJobModeType,
     DomainType,
     ImportModeType,
     IngestionModeType,
     ObjectiveSensitivityType,
@@ -37,30 +37,35 @@
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlgorithmImageTypeDef",
+    "AutoMLConfigOutputTypeDef",
     "AutoMLConfigTypeDef",
     "AutoMLResultTypeDef",
     "AutoTrainingConfigTypeDef",
+    "BatchInferenceJobConfigOutputTypeDef",
     "BatchInferenceJobConfigTypeDef",
     "S3DataConfigTypeDef",
     "BatchInferenceJobSummaryTypeDef",
     "BatchSegmentJobSummaryTypeDef",
+    "CampaignConfigOutputTypeDef",
     "CampaignConfigTypeDef",
     "CampaignSummaryTypeDef",
+    "CategoricalHyperParameterRangeOutputTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
     "ContinuousHyperParameterRangeTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DataSourceTypeDef",
     "MetricAttributeTypeDef",
     "CreateSchemaRequestRequestTypeDef",
+    "DataDeletionJobSummaryTypeDef",
     "DatasetExportJobSummaryTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetGroupTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DatasetSchemaSummaryTypeDef",
     "DatasetSchemaTypeDef",
     "DatasetSummaryTypeDef",
@@ -77,14 +82,15 @@
     "DeleteRecommenderRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteSolutionRequestRequestTypeDef",
     "DescribeAlgorithmRequestRequestTypeDef",
     "DescribeBatchInferenceJobRequestRequestTypeDef",
     "DescribeBatchSegmentJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
+    "DescribeDataDeletionJobRequestRequestTypeDef",
     "DescribeDatasetExportJobRequestRequestTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeEventTrackerRequestRequestTypeDef",
     "EventTrackerTypeDef",
     "DescribeFeatureTransformationRequestRequestTypeDef",
@@ -105,14 +111,15 @@
     "HPOObjectiveTypeDef",
     "HPOResourceConfigTypeDef",
     "IntegerHyperParameterRangeTypeDef",
     "PaginatorConfigTypeDef",
     "ListBatchInferenceJobsRequestRequestTypeDef",
     "ListBatchSegmentJobsRequestRequestTypeDef",
     "ListCampaignsRequestRequestTypeDef",
+    "ListDataDeletionJobsRequestRequestTypeDef",
     "ListDatasetExportJobsRequestRequestTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListEventTrackersRequestRequestTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "ListMetricAttributionMetricsRequestRequestTypeDef",
@@ -124,40 +131,44 @@
     "ListSchemasRequestRequestTypeDef",
     "ListSolutionVersionsRequestRequestTypeDef",
     "SolutionVersionSummaryTypeDef",
     "ListSolutionsRequestRequestTypeDef",
     "SolutionSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OptimizationObjectiveTypeDef",
-    "TrainingDataConfigPaginatorTypeDef",
+    "TrainingDataConfigExtraOutputTypeDef",
+    "TrainingDataConfigOutputTypeDef",
     "TrainingDataConfigTypeDef",
     "TunedHPOParamsTypeDef",
     "StartRecommenderRequestRequestTypeDef",
     "StopRecommenderRequestRequestTypeDef",
     "StopSolutionVersionCreationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
+    "BatchInferenceJobConfigUnionTypeDef",
     "BatchInferenceJobInputTypeDef",
     "BatchInferenceJobOutputTypeDef",
     "BatchSegmentJobInputTypeDef",
     "BatchSegmentJobOutputTypeDef",
     "DatasetExportJobOutputTypeDef",
     "MetricAttributionOutputTypeDef",
     "CampaignUpdateSummaryTypeDef",
+    "CampaignConfigUnionTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateEventTrackerRequestRequestTypeDef",
     "CreateFilterRequestRequestTypeDef",
     "CreateSolutionVersionRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateBatchInferenceJobResponseTypeDef",
     "CreateBatchSegmentJobResponseTypeDef",
     "CreateCampaignResponseTypeDef",
+    "CreateDataDeletionJobResponseTypeDef",
     "CreateDatasetExportJobResponseTypeDef",
     "CreateDatasetGroupResponseTypeDef",
     "CreateDatasetImportJobResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateEventTrackerResponseTypeDef",
     "CreateFilterResponseTypeDef",
     "CreateMetricAttributionResponseTypeDef",
@@ -173,17 +184,20 @@
     "ListTagsForResourceResponseTypeDef",
     "StartRecommenderResponseTypeDef",
     "StopRecommenderResponseTypeDef",
     "UpdateCampaignResponseTypeDef",
     "UpdateDatasetResponseTypeDef",
     "UpdateMetricAttributionResponseTypeDef",
     "UpdateRecommenderResponseTypeDef",
+    "CreateDataDeletionJobRequestRequestTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
+    "DataDeletionJobTypeDef",
     "DatasetImportJobTypeDef",
     "ListMetricAttributionMetricsResponseTypeDef",
+    "ListDataDeletionJobsResponseTypeDef",
     "ListDatasetExportJobsResponseTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "DescribeDatasetGroupResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "DescribeSchemaResponseTypeDef",
     "ListDatasetsResponseTypeDef",
@@ -192,14 +206,15 @@
     "DescribeEventTrackerResponseTypeDef",
     "DescribeFeatureTransformationResponseTypeDef",
     "DescribeFilterResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "ListEventTrackersResponseTypeDef",
     "ThemeGenerationConfigTypeDef",
     "ListFiltersResponseTypeDef",
+    "HyperParameterRangesOutputTypeDef",
     "HyperParameterRangesTypeDef",
     "ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef",
     "ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef",
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef",
     "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
@@ -213,60 +228,71 @@
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef",
     "ListSolutionsRequestListSolutionsPaginateTypeDef",
     "ListMetricAttributionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
     "ListSolutionVersionsResponseTypeDef",
     "ListSolutionsResponseTypeDef",
-    "RecommenderConfigPaginatorTypeDef",
+    "RecommenderConfigExtraOutputTypeDef",
+    "RecommenderConfigOutputTypeDef",
     "RecommenderConfigTypeDef",
     "BatchSegmentJobTypeDef",
     "CreateBatchSegmentJobRequestRequestTypeDef",
     "CreateDatasetExportJobRequestRequestTypeDef",
     "DatasetExportJobTypeDef",
     "CreateMetricAttributionRequestRequestTypeDef",
     "MetricAttributionTypeDef",
     "UpdateMetricAttributionRequestRequestTypeDef",
     "CampaignTypeDef",
+    "DescribeDataDeletionJobResponseTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "AlgorithmTypeDef",
     "BatchInferenceJobTypeDef",
     "CreateBatchInferenceJobRequestRequestTypeDef",
+    "HPOConfigOutputTypeDef",
     "HPOConfigTypeDef",
-    "RecommenderSummaryPaginatorTypeDef",
-    "CreateRecommenderRequestRequestTypeDef",
     "RecommenderSummaryTypeDef",
     "RecommenderUpdateSummaryTypeDef",
+    "CreateRecommenderRequestRequestTypeDef",
+    "RecommenderConfigUnionTypeDef",
     "UpdateRecommenderRequestRequestTypeDef",
     "DescribeBatchSegmentJobResponseTypeDef",
     "DescribeDatasetExportJobResponseTypeDef",
     "DescribeMetricAttributionResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
     "DescribeAlgorithmResponseTypeDef",
     "DescribeBatchInferenceJobResponseTypeDef",
+    "SolutionConfigOutputTypeDef",
     "SolutionConfigTypeDef",
-    "ListRecommendersResponsePaginatorTypeDef",
     "ListRecommendersResponseTypeDef",
     "RecommenderTypeDef",
-    "CreateSolutionRequestRequestTypeDef",
     "SolutionTypeDef",
     "SolutionVersionTypeDef",
+    "CreateSolutionRequestRequestTypeDef",
+    "SolutionConfigUnionTypeDef",
     "DescribeRecommenderResponseTypeDef",
     "DescribeSolutionResponseTypeDef",
     "DescribeSolutionVersionResponseTypeDef",
 )
 
 AlgorithmImageTypeDef = TypedDict(
     "AlgorithmImageTypeDef",
     {
         "dockerURI": str,
         "name": NotRequired[str],
     },
 )
+AutoMLConfigOutputTypeDef = TypedDict(
+    "AutoMLConfigOutputTypeDef",
+    {
+        "metricName": NotRequired[str],
+        "recipeList": NotRequired[List[str]],
+    },
+)
 AutoMLConfigTypeDef = TypedDict(
     "AutoMLConfigTypeDef",
     {
         "metricName": NotRequired[str],
         "recipeList": NotRequired[Sequence[str]],
     },
 )
@@ -278,14 +304,20 @@
 )
 AutoTrainingConfigTypeDef = TypedDict(
     "AutoTrainingConfigTypeDef",
     {
         "schedulingExpression": NotRequired[str],
     },
 )
+BatchInferenceJobConfigOutputTypeDef = TypedDict(
+    "BatchInferenceJobConfigOutputTypeDef",
+    {
+        "itemExplorationConfig": NotRequired[Dict[str, str]],
+    },
+)
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
     {
         "itemExplorationConfig": NotRequired[Mapping[str, str]],
     },
 )
 S3DataConfigTypeDef = TypedDict(
@@ -316,14 +348,22 @@
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "failureReason": NotRequired[str],
         "solutionVersionArn": NotRequired[str],
     },
 )
+CampaignConfigOutputTypeDef = TypedDict(
+    "CampaignConfigOutputTypeDef",
+    {
+        "itemExplorationConfig": NotRequired[Dict[str, str]],
+        "enableMetadataWithRecommendations": NotRequired[bool],
+        "syncWithLatestSolutionVersion": NotRequired[bool],
+    },
+)
 CampaignConfigTypeDef = TypedDict(
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": NotRequired[Mapping[str, str]],
         "enableMetadataWithRecommendations": NotRequired[bool],
         "syncWithLatestSolutionVersion": NotRequired[bool],
     },
@@ -335,14 +375,21 @@
         "campaignArn": NotRequired[str],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "failureReason": NotRequired[str],
     },
 )
+CategoricalHyperParameterRangeOutputTypeDef = TypedDict(
+    "CategoricalHyperParameterRangeOutputTypeDef",
+    {
+        "name": NotRequired[str],
+        "values": NotRequired[List[str]],
+    },
+)
 CategoricalHyperParameterRangeTypeDef = TypedDict(
     "CategoricalHyperParameterRangeTypeDef",
     {
         "name": NotRequired[str],
         "values": NotRequired[Sequence[str]],
     },
 )
@@ -389,14 +436,26 @@
     "CreateSchemaRequestRequestTypeDef",
     {
         "name": str,
         "schema": str,
         "domain": NotRequired[DomainType],
     },
 )
+DataDeletionJobSummaryTypeDef = TypedDict(
+    "DataDeletionJobSummaryTypeDef",
+    {
+        "dataDeletionJobArn": NotRequired[str],
+        "datasetGroupArn": NotRequired[str],
+        "jobName": NotRequired[str],
+        "status": NotRequired[str],
+        "creationDateTime": NotRequired[datetime],
+        "lastUpdatedDateTime": NotRequired[datetime],
+        "failureReason": NotRequired[str],
+    },
+)
 DatasetExportJobSummaryTypeDef = TypedDict(
     "DatasetExportJobSummaryTypeDef",
     {
         "datasetExportJobArn": NotRequired[str],
         "jobName": NotRequired[str],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
@@ -584,14 +643,20 @@
 )
 DescribeCampaignRequestRequestTypeDef = TypedDict(
     "DescribeCampaignRequestRequestTypeDef",
     {
         "campaignArn": str,
     },
 )
+DescribeDataDeletionJobRequestRequestTypeDef = TypedDict(
+    "DescribeDataDeletionJobRequestRequestTypeDef",
+    {
+        "dataDeletionJobArn": str,
+    },
+)
 DescribeDatasetExportJobRequestRequestTypeDef = TypedDict(
     "DescribeDatasetExportJobRequestRequestTypeDef",
     {
         "datasetExportJobArn": str,
     },
 )
 DescribeDatasetGroupRequestRequestTypeDef = TypedDict(
@@ -802,14 +867,22 @@
     "ListCampaignsRequestRequestTypeDef",
     {
         "solutionArn": NotRequired[str],
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
     },
 )
+ListDataDeletionJobsRequestRequestTypeDef = TypedDict(
+    "ListDataDeletionJobsRequestRequestTypeDef",
+    {
+        "datasetGroupArn": NotRequired[str],
+        "nextToken": NotRequired[str],
+        "maxResults": NotRequired[int],
+    },
+)
 ListDatasetExportJobsRequestRequestTypeDef = TypedDict(
     "ListDatasetExportJobsRequestRequestTypeDef",
     {
         "datasetArn": NotRequired[str],
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
     },
@@ -963,16 +1036,22 @@
 OptimizationObjectiveTypeDef = TypedDict(
     "OptimizationObjectiveTypeDef",
     {
         "itemAttribute": NotRequired[str],
         "objectiveSensitivity": NotRequired[ObjectiveSensitivityType],
     },
 )
-TrainingDataConfigPaginatorTypeDef = TypedDict(
-    "TrainingDataConfigPaginatorTypeDef",
+TrainingDataConfigExtraOutputTypeDef = TypedDict(
+    "TrainingDataConfigExtraOutputTypeDef",
+    {
+        "excludedDatasetColumns": NotRequired[Dict[str, List[str]]],
+    },
+)
+TrainingDataConfigOutputTypeDef = TypedDict(
+    "TrainingDataConfigOutputTypeDef",
     {
         "excludedDatasetColumns": NotRequired[Dict[str, List[str]]],
     },
 )
 TrainingDataConfigTypeDef = TypedDict(
     "TrainingDataConfigTypeDef",
     {
@@ -1013,14 +1092,17 @@
 UpdateDatasetRequestRequestTypeDef = TypedDict(
     "UpdateDatasetRequestRequestTypeDef",
     {
         "datasetArn": str,
         "schemaArn": str,
     },
 )
+BatchInferenceJobConfigUnionTypeDef = Union[
+    BatchInferenceJobConfigTypeDef, BatchInferenceJobConfigOutputTypeDef
+]
 BatchInferenceJobInputTypeDef = TypedDict(
     "BatchInferenceJobInputTypeDef",
     {
         "s3DataSource": S3DataConfigTypeDef,
     },
 )
 BatchInferenceJobOutputTypeDef = TypedDict(
@@ -1055,21 +1137,22 @@
     },
 )
 CampaignUpdateSummaryTypeDef = TypedDict(
     "CampaignUpdateSummaryTypeDef",
     {
         "solutionVersionArn": NotRequired[str],
         "minProvisionedTPS": NotRequired[int],
-        "campaignConfig": NotRequired[CampaignConfigTypeDef],
+        "campaignConfig": NotRequired[CampaignConfigOutputTypeDef],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
     },
 )
+CampaignConfigUnionTypeDef = Union[CampaignConfigTypeDef, CampaignConfigOutputTypeDef]
 UpdateCampaignRequestRequestTypeDef = TypedDict(
     "UpdateCampaignRequestRequestTypeDef",
     {
         "campaignArn": str,
         "solutionVersionArn": NotRequired[str],
         "minProvisionedTPS": NotRequired[int],
         "campaignConfig": NotRequired[CampaignConfigTypeDef],
@@ -1155,14 +1238,21 @@
 CreateCampaignResponseTypeDef = TypedDict(
     "CreateCampaignResponseTypeDef",
     {
         "campaignArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDataDeletionJobResponseTypeDef = TypedDict(
+    "CreateDataDeletionJobResponseTypeDef",
+    {
+        "dataDeletionJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateDatasetExportJobResponseTypeDef = TypedDict(
     "CreateDatasetExportJobResponseTypeDef",
     {
         "datasetExportJobArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1321,26 +1411,51 @@
 UpdateRecommenderResponseTypeDef = TypedDict(
     "UpdateRecommenderResponseTypeDef",
     {
         "recommenderArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDataDeletionJobRequestRequestTypeDef = TypedDict(
+    "CreateDataDeletionJobRequestRequestTypeDef",
+    {
+        "jobName": str,
+        "datasetGroupArn": str,
+        "dataSource": DataSourceTypeDef,
+        "roleArn": str,
+        "tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
 CreateDatasetImportJobRequestRequestTypeDef = TypedDict(
     "CreateDatasetImportJobRequestRequestTypeDef",
     {
         "jobName": str,
         "datasetArn": str,
         "dataSource": DataSourceTypeDef,
         "roleArn": str,
         "tags": NotRequired[Sequence[TagTypeDef]],
         "importMode": NotRequired[ImportModeType],
         "publishAttributionMetricsToS3": NotRequired[bool],
     },
 )
+DataDeletionJobTypeDef = TypedDict(
+    "DataDeletionJobTypeDef",
+    {
+        "jobName": NotRequired[str],
+        "dataDeletionJobArn": NotRequired[str],
+        "datasetGroupArn": NotRequired[str],
+        "dataSource": NotRequired[DataSourceTypeDef],
+        "roleArn": NotRequired[str],
+        "status": NotRequired[str],
+        "numDeleted": NotRequired[int],
+        "creationDateTime": NotRequired[datetime],
+        "lastUpdatedDateTime": NotRequired[datetime],
+        "failureReason": NotRequired[str],
+    },
+)
 DatasetImportJobTypeDef = TypedDict(
     "DatasetImportJobTypeDef",
     {
         "jobName": NotRequired[str],
         "datasetImportJobArn": NotRequired[str],
         "datasetArn": NotRequired[str],
         "dataSource": NotRequired[DataSourceTypeDef],
@@ -1357,14 +1472,22 @@
     "ListMetricAttributionMetricsResponseTypeDef",
     {
         "metrics": List[MetricAttributeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListDataDeletionJobsResponseTypeDef = TypedDict(
+    "ListDataDeletionJobsResponseTypeDef",
+    {
+        "dataDeletionJobs": List[DataDeletionJobSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ListDatasetExportJobsResponseTypeDef = TypedDict(
     "ListDatasetExportJobsResponseTypeDef",
     {
         "datasetExportJobs": List[DatasetExportJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1488,14 +1611,24 @@
     "ListFiltersResponseTypeDef",
     {
         "Filters": List[FilterSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+HyperParameterRangesOutputTypeDef = TypedDict(
+    "HyperParameterRangesOutputTypeDef",
+    {
+        "integerHyperParameterRanges": NotRequired[List[IntegerHyperParameterRangeTypeDef]],
+        "continuousHyperParameterRanges": NotRequired[List[ContinuousHyperParameterRangeTypeDef]],
+        "categoricalHyperParameterRanges": NotRequired[
+            List[CategoricalHyperParameterRangeOutputTypeDef]
+        ],
+    },
+)
 HyperParameterRangesTypeDef = TypedDict(
     "HyperParameterRangesTypeDef",
     {
         "integerHyperParameterRanges": NotRequired[Sequence[IntegerHyperParameterRangeTypeDef]],
         "continuousHyperParameterRanges": NotRequired[
             Sequence[ContinuousHyperParameterRangeTypeDef]
         ],
@@ -1643,20 +1776,29 @@
     "ListSolutionsResponseTypeDef",
     {
         "solutions": List[SolutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-RecommenderConfigPaginatorTypeDef = TypedDict(
-    "RecommenderConfigPaginatorTypeDef",
+RecommenderConfigExtraOutputTypeDef = TypedDict(
+    "RecommenderConfigExtraOutputTypeDef",
+    {
+        "itemExplorationConfig": NotRequired[Dict[str, str]],
+        "minRecommendationRequestsPerSecond": NotRequired[int],
+        "trainingDataConfig": NotRequired[TrainingDataConfigExtraOutputTypeDef],
+        "enableMetadataWithRecommendations": NotRequired[bool],
+    },
+)
+RecommenderConfigOutputTypeDef = TypedDict(
+    "RecommenderConfigOutputTypeDef",
     {
         "itemExplorationConfig": NotRequired[Dict[str, str]],
         "minRecommendationRequestsPerSecond": NotRequired[int],
-        "trainingDataConfig": NotRequired[TrainingDataConfigPaginatorTypeDef],
+        "trainingDataConfig": NotRequired[TrainingDataConfigOutputTypeDef],
         "enableMetadataWithRecommendations": NotRequired[bool],
     },
 )
 RecommenderConfigTypeDef = TypedDict(
     "RecommenderConfigTypeDef",
     {
         "itemExplorationConfig": NotRequired[Mapping[str, str]],
@@ -1755,22 +1897,29 @@
 CampaignTypeDef = TypedDict(
     "CampaignTypeDef",
     {
         "name": NotRequired[str],
         "campaignArn": NotRequired[str],
         "solutionVersionArn": NotRequired[str],
         "minProvisionedTPS": NotRequired[int],
-        "campaignConfig": NotRequired[CampaignConfigTypeDef],
+        "campaignConfig": NotRequired[CampaignConfigOutputTypeDef],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "latestCampaignUpdate": NotRequired[CampaignUpdateSummaryTypeDef],
     },
 )
+DescribeDataDeletionJobResponseTypeDef = TypedDict(
+    "DescribeDataDeletionJobResponseTypeDef",
+    {
+        "dataDeletionJob": DataDeletionJobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeDatasetImportJobResponseTypeDef = TypedDict(
     "DescribeDatasetImportJobResponseTypeDef",
     {
         "datasetImportJob": DatasetImportJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1803,15 +1952,15 @@
         "batchInferenceJobArn": NotRequired[str],
         "filterArn": NotRequired[str],
         "failureReason": NotRequired[str],
         "solutionVersionArn": NotRequired[str],
         "numResults": NotRequired[int],
         "jobInput": NotRequired[BatchInferenceJobInputTypeDef],
         "jobOutput": NotRequired[BatchInferenceJobOutputTypeDef],
-        "batchInferenceJobConfig": NotRequired[BatchInferenceJobConfigTypeDef],
+        "batchInferenceJobConfig": NotRequired[BatchInferenceJobConfigOutputTypeDef],
         "roleArn": NotRequired[str],
         "batchInferenceJobMode": NotRequired[BatchInferenceJobModeType],
         "themeGenerationConfig": NotRequired[ThemeGenerationConfigTypeDef],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
     },
@@ -1828,68 +1977,64 @@
         "numResults": NotRequired[int],
         "batchInferenceJobConfig": NotRequired[BatchInferenceJobConfigTypeDef],
         "tags": NotRequired[Sequence[TagTypeDef]],
         "batchInferenceJobMode": NotRequired[BatchInferenceJobModeType],
         "themeGenerationConfig": NotRequired[ThemeGenerationConfigTypeDef],
     },
 )
-HPOConfigTypeDef = TypedDict(
-    "HPOConfigTypeDef",
+HPOConfigOutputTypeDef = TypedDict(
+    "HPOConfigOutputTypeDef",
     {
         "hpoObjective": NotRequired[HPOObjectiveTypeDef],
         "hpoResourceConfig": NotRequired[HPOResourceConfigTypeDef],
-        "algorithmHyperParameterRanges": NotRequired[HyperParameterRangesTypeDef],
-    },
-)
-RecommenderSummaryPaginatorTypeDef = TypedDict(
-    "RecommenderSummaryPaginatorTypeDef",
-    {
-        "name": NotRequired[str],
-        "recommenderArn": NotRequired[str],
-        "datasetGroupArn": NotRequired[str],
-        "recipeArn": NotRequired[str],
-        "recommenderConfig": NotRequired[RecommenderConfigPaginatorTypeDef],
-        "status": NotRequired[str],
-        "creationDateTime": NotRequired[datetime],
-        "lastUpdatedDateTime": NotRequired[datetime],
+        "algorithmHyperParameterRanges": NotRequired[HyperParameterRangesOutputTypeDef],
     },
 )
-CreateRecommenderRequestRequestTypeDef = TypedDict(
-    "CreateRecommenderRequestRequestTypeDef",
+HPOConfigTypeDef = TypedDict(
+    "HPOConfigTypeDef",
     {
-        "name": str,
-        "datasetGroupArn": str,
-        "recipeArn": str,
-        "recommenderConfig": NotRequired[RecommenderConfigTypeDef],
-        "tags": NotRequired[Sequence[TagTypeDef]],
+        "hpoObjective": NotRequired[HPOObjectiveTypeDef],
+        "hpoResourceConfig": NotRequired[HPOResourceConfigTypeDef],
+        "algorithmHyperParameterRanges": NotRequired[HyperParameterRangesTypeDef],
     },
 )
 RecommenderSummaryTypeDef = TypedDict(
     "RecommenderSummaryTypeDef",
     {
         "name": NotRequired[str],
         "recommenderArn": NotRequired[str],
         "datasetGroupArn": NotRequired[str],
         "recipeArn": NotRequired[str],
-        "recommenderConfig": NotRequired[RecommenderConfigTypeDef],
+        "recommenderConfig": NotRequired[RecommenderConfigOutputTypeDef],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
     },
 )
 RecommenderUpdateSummaryTypeDef = TypedDict(
     "RecommenderUpdateSummaryTypeDef",
     {
-        "recommenderConfig": NotRequired[RecommenderConfigTypeDef],
+        "recommenderConfig": NotRequired[RecommenderConfigOutputTypeDef],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
     },
 )
+CreateRecommenderRequestRequestTypeDef = TypedDict(
+    "CreateRecommenderRequestRequestTypeDef",
+    {
+        "name": str,
+        "datasetGroupArn": str,
+        "recipeArn": str,
+        "recommenderConfig": NotRequired[RecommenderConfigTypeDef],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+RecommenderConfigUnionTypeDef = Union[RecommenderConfigTypeDef, RecommenderConfigExtraOutputTypeDef]
 UpdateRecommenderRequestRequestTypeDef = TypedDict(
     "UpdateRecommenderRequestRequestTypeDef",
     {
         "recommenderArn": str,
         "recommenderConfig": RecommenderConfigTypeDef,
     },
 )
@@ -1931,35 +2076,40 @@
 DescribeBatchInferenceJobResponseTypeDef = TypedDict(
     "DescribeBatchInferenceJobResponseTypeDef",
     {
         "batchInferenceJob": BatchInferenceJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SolutionConfigOutputTypeDef = TypedDict(
+    "SolutionConfigOutputTypeDef",
+    {
+        "eventValueThreshold": NotRequired[str],
+        "hpoConfig": NotRequired[HPOConfigOutputTypeDef],
+        "algorithmHyperParameters": NotRequired[Dict[str, str]],
+        "featureTransformationParameters": NotRequired[Dict[str, str]],
+        "autoMLConfig": NotRequired[AutoMLConfigOutputTypeDef],
+        "optimizationObjective": NotRequired[OptimizationObjectiveTypeDef],
+        "trainingDataConfig": NotRequired[TrainingDataConfigOutputTypeDef],
+        "autoTrainingConfig": NotRequired[AutoTrainingConfigTypeDef],
+    },
+)
 SolutionConfigTypeDef = TypedDict(
     "SolutionConfigTypeDef",
     {
         "eventValueThreshold": NotRequired[str],
         "hpoConfig": NotRequired[HPOConfigTypeDef],
         "algorithmHyperParameters": NotRequired[Mapping[str, str]],
         "featureTransformationParameters": NotRequired[Mapping[str, str]],
         "autoMLConfig": NotRequired[AutoMLConfigTypeDef],
         "optimizationObjective": NotRequired[OptimizationObjectiveTypeDef],
         "trainingDataConfig": NotRequired[TrainingDataConfigTypeDef],
         "autoTrainingConfig": NotRequired[AutoTrainingConfigTypeDef],
     },
 )
-ListRecommendersResponsePaginatorTypeDef = TypedDict(
-    "ListRecommendersResponsePaginatorTypeDef",
-    {
-        "recommenders": List[RecommenderSummaryPaginatorTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListRecommendersResponseTypeDef = TypedDict(
     "ListRecommendersResponseTypeDef",
     {
         "recommenders": List[RecommenderSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1967,49 +2117,35 @@
 RecommenderTypeDef = TypedDict(
     "RecommenderTypeDef",
     {
         "recommenderArn": NotRequired[str],
         "datasetGroupArn": NotRequired[str],
         "name": NotRequired[str],
         "recipeArn": NotRequired[str],
-        "recommenderConfig": NotRequired[RecommenderConfigTypeDef],
+        "recommenderConfig": NotRequired[RecommenderConfigOutputTypeDef],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
         "latestRecommenderUpdate": NotRequired[RecommenderUpdateSummaryTypeDef],
         "modelMetrics": NotRequired[Dict[str, float]],
     },
 )
-CreateSolutionRequestRequestTypeDef = TypedDict(
-    "CreateSolutionRequestRequestTypeDef",
-    {
-        "name": str,
-        "datasetGroupArn": str,
-        "performHPO": NotRequired[bool],
-        "performAutoML": NotRequired[bool],
-        "performAutoTraining": NotRequired[bool],
-        "recipeArn": NotRequired[str],
-        "eventType": NotRequired[str],
-        "solutionConfig": NotRequired[SolutionConfigTypeDef],
-        "tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 SolutionTypeDef = TypedDict(
     "SolutionTypeDef",
     {
         "name": NotRequired[str],
         "solutionArn": NotRequired[str],
         "performHPO": NotRequired[bool],
         "performAutoML": NotRequired[bool],
         "performAutoTraining": NotRequired[bool],
         "recipeArn": NotRequired[str],
         "datasetGroupArn": NotRequired[str],
         "eventType": NotRequired[str],
-        "solutionConfig": NotRequired[SolutionConfigTypeDef],
+        "solutionConfig": NotRequired[SolutionConfigOutputTypeDef],
         "autoMLResult": NotRequired[AutoMLResultTypeDef],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "latestSolutionVersion": NotRequired[SolutionVersionSummaryTypeDef],
     },
 )
@@ -2020,25 +2156,40 @@
         "solutionVersionArn": NotRequired[str],
         "solutionArn": NotRequired[str],
         "performHPO": NotRequired[bool],
         "performAutoML": NotRequired[bool],
         "recipeArn": NotRequired[str],
         "eventType": NotRequired[str],
         "datasetGroupArn": NotRequired[str],
-        "solutionConfig": NotRequired[SolutionConfigTypeDef],
+        "solutionConfig": NotRequired[SolutionConfigOutputTypeDef],
         "trainingHours": NotRequired[float],
         "trainingMode": NotRequired[TrainingModeType],
         "tunedHPOParams": NotRequired[TunedHPOParamsTypeDef],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "trainingType": NotRequired[TrainingTypeType],
     },
 )
+CreateSolutionRequestRequestTypeDef = TypedDict(
+    "CreateSolutionRequestRequestTypeDef",
+    {
+        "name": str,
+        "datasetGroupArn": str,
+        "performHPO": NotRequired[bool],
+        "performAutoML": NotRequired[bool],
+        "performAutoTraining": NotRequired[bool],
+        "recipeArn": NotRequired[str],
+        "eventType": NotRequired[str],
+        "solutionConfig": NotRequired[SolutionConfigTypeDef],
+        "tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+SolutionConfigUnionTypeDef = Union[SolutionConfigTypeDef, SolutionConfigOutputTypeDef]
 DescribeRecommenderResponseTypeDef = TypedDict(
     "DescribeRecommenderResponseTypeDef",
     {
         "recommender": RecommenderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/PKG-INFO` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.34.88
-Summary: Type annotations for boto3.Personalize 1.34.88 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.97
+Summary: Type annotations for boto3.Personalize 1.34.97 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize)](https://pepy.tech/project/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.34.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.34.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
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
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/SOURCES.txt` & `mypy_boto3_personalize-1.34.97/mypy_boto3_personalize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_personalize-1.34.88/setup.py` & `mypy_boto3_personalize-1.34.97/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize",
-    version="1.34.88",
+    version="1.34.97",
     packages=["mypy_boto3_personalize"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Personalize 1.34.88 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Personalize 1.34.97 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

