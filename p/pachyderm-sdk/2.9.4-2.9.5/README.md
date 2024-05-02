# Comparing `tmp/pachyderm_sdk-2.9.4.tar.gz` & `tmp/pachyderm_sdk-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pachyderm_sdk-2.9.4.tar", max compression
+gzip compressed data, was "pachyderm_sdk-2.9.5.tar", max compression
```

## Comparing `pachyderm_sdk-2.9.4.tar` & `pachyderm_sdk-2.9.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2913 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/README.md
--rw-r--r--   0        0        0      357 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/__init__.py
--rw-r--r--   0        0        0      645 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/__main__.py
--rw-r--r--   0        0        0        8 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/.gitignore
--rw-r--r--   0        0        0       66 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/__init__.py
--rw-r--r--   0        0        0     3172 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/admin/__init__.py
--rw-r--r--   0        0        0     1036 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/admin/extension.py
--rw-r--r--   0        0        0    31384 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/auth/__init__.py
--rw-r--r--   0        0        0    13046 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/debug/__init__.py
--rw-r--r--   0        0        0     1609 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/debug/extension.py
--rw-r--r--   0        0        0     8236 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/enterprise/__init__.py
--rw-r--r--   0        0        0    12315 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/identity/__init__.py
--rw-r--r--   0        0        0    10507 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/license/__init__.py
--rw-r--r--   0        0        0    56747 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/__init__.py
--rw-r--r--   0        0        0     5447 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/_additions.py
--rw-r--r--   0        0        0    25802 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/extension.py
--rw-r--r--   0        0        0     4018 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/file.py
--rw-r--r--   0        0        0    14258 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pjs/__init__.py
--rw-r--r--   0        0        0    75665 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/__init__.py
--rw-r--r--   0        0        0      679 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/_additions.py
--rw-r--r--   0        0        0     4175 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/extension.py
--rw-r--r--   0        0        0     1113 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/taskapi/__init__.py
--rw-r--r--   0        0        0     6822 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/transaction/__init__.py
--rw-r--r--   0        0        0     3614 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/transaction/extension.py
--rw-r--r--   0        0        0     1375 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/version/__init__.py
--rw-r--r--   0        0        0     2866 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/worker/__init__.py
--rw-r--r--   0        0        0     1872 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/worker/extension.py
--rw-r--r--   0        0        0    11519 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/client.py
--rw-r--r--   0        0        0     7114 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/config.py
--rw-r--r--   0        0        0     1083 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/constants.py
--rw-r--r--   0        0        0     1570 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/datum_batching.py
--rw-r--r--   0        0        0     1045 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/errors.py
--rw-r--r--   0        0        0     3439 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/interceptor.py
--rw-r--r--   0        0        0     1490 2024-04-10 16:09:21.369456 pachyderm_sdk-2.9.4/pyproject.toml
--rw-r--r--   0        0        0     4289 1970-01-01 00:00:00.000000 pachyderm_sdk-2.9.4/PKG-INFO
+-rw-r--r--   0        0        0     2913 2024-04-24 19:01:12.229202 pachyderm_sdk-2.9.5/README.md
+-rw-r--r--   0        0        0      357 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/__init__.py
+-rw-r--r--   0        0        0      645 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/__main__.py
+-rw-r--r--   0        0        0        8 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/.gitignore
+-rw-r--r--   0        0        0       66 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/__init__.py
+-rw-r--r--   0        0        0     3172 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/admin/__init__.py
+-rw-r--r--   0        0        0     1036 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/admin/extension.py
+-rw-r--r--   0        0        0    31384 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/auth/__init__.py
+-rw-r--r--   0        0        0    13046 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/debug/__init__.py
+-rw-r--r--   0        0        0     1609 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/debug/extension.py
+-rw-r--r--   0        0        0     8236 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/enterprise/__init__.py
+-rw-r--r--   0        0        0    12315 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/identity/__init__.py
+-rw-r--r--   0        0        0    10507 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/license/__init__.py
+-rw-r--r--   0        0        0    56747 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/__init__.py
+-rw-r--r--   0        0        0     5447 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/_additions.py
+-rw-r--r--   0        0        0    25802 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/extension.py
+-rw-r--r--   0        0        0     4018 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/file.py
+-rw-r--r--   0        0        0    14258 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pjs/__init__.py
+-rw-r--r--   0        0        0    75621 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/__init__.py
+-rw-r--r--   0        0        0      679 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/_additions.py
+-rw-r--r--   0        0        0     4175 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/extension.py
+-rw-r--r--   0        0        0     1113 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/taskapi/__init__.py
+-rw-r--r--   0        0        0     6822 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/transaction/__init__.py
+-rw-r--r--   0        0        0     3614 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/transaction/extension.py
+-rw-r--r--   0        0        0     1375 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/version/__init__.py
+-rw-r--r--   0        0        0     2866 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/worker/__init__.py
+-rw-r--r--   0        0        0     1872 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/worker/extension.py
+-rw-r--r--   0        0        0    11519 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/client.py
+-rw-r--r--   0        0        0     7114 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/config.py
+-rw-r--r--   0        0        0     1083 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/constants.py
+-rw-r--r--   0        0        0     1570 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/datum_batching.py
+-rw-r--r--   0        0        0     1045 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/errors.py
+-rw-r--r--   0        0        0     3439 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/interceptor.py
+-rw-r--r--   0        0        0     1490 2024-04-24 19:01:51.973537 pachyderm_sdk-2.9.5/pyproject.toml
+-rw-r--r--   0        0        0     4289 1970-01-01 00:00:00.000000 pachyderm_sdk-2.9.5/PKG-INFO
```

### Comparing `pachyderm_sdk-2.9.4/README.md` & `pachyderm_sdk-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/__main__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/admin/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/admin/extension.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/admin/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/auth/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/debug/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/debug/extension.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/debug/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/enterprise/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/enterprise/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/identity/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/license/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/license/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/_additions.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/_additions.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/extension.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/file.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/file.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pjs/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pjs/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,17 +186,15 @@
 
 @dataclass(eq=False, repr=False)
 class Egress(betterproto.Message):
     url: str = betterproto.string_field(1)
     object_storage: "_pfs__.ObjectStorageEgress" = betterproto.message_field(
         2, group="target"
     )
-    sql_database: "_pfs__.SqlDatabaseEgress" = betterproto.message_field(
-        3, group="target"
-    )
+    sql_database: "_pfs__.SqlDatabaseEgress" = betterproto.message_field(3, group="target")
 
 
 @dataclass(eq=False, repr=False)
 class Determined(betterproto.Message):
     workspaces: List[str] = betterproto.string_field(1)
 
 
@@ -1036,17 +1034,15 @@
     """
     Projects to filter on. Empty list means no filter, so return all pipelines.
     """
 
     def __post_init__(self) -> None:
         super().__post_init__()
         if self.is_set("details"):
-            warnings.warn(
-                "ListPipelineRequest.details is deprecated", DeprecationWarning
-            )
+            warnings.warn("ListPipelineRequest.details is deprecated", DeprecationWarning)
 
 
 @dataclass(eq=False, repr=False)
 class DeletePipelineRequest(betterproto.Message):
     """
     Delete a pipeline.  If the deprecated all member is true, then delete all
     pipelines in the default project.
@@ -1544,15 +1540,15 @@
         pipeline: "Pipeline" = None,
         input_commit: Optional[List["_pfs__.Commit"]] = None,
         history: int = 0,
         details: bool = False,
         jq_filter: str = "",
         pagination_marker: datetime = None,
         number: int = 0,
-        reverse: bool = False
+        reverse: bool = False,
     ) -> Iterator["JobInfo"]:
         projects = projects or []
         input_commit = input_commit or []
 
         request = ListJobRequest()
         if projects is not None:
             request.projects = projects
@@ -1575,15 +1571,15 @@
         self,
         *,
         details: bool = False,
         projects: Optional[List["_pfs__.Project"]] = None,
         pagination_marker: datetime = None,
         number: int = 0,
         reverse: bool = False,
-        jq_filter: str = ""
+        jq_filter: str = "",
     ) -> Iterator["JobSetInfo"]:
         projects = projects or []
 
         request = ListJobSetRequest()
         request.details = details
         if projects is not None:
             request.projects = projects
@@ -1604,17 +1600,15 @@
         if pipeline is not None:
             request.pipeline = pipeline
         request.details = details
 
         for response in self.__rpc_subscribe_job(request):
             yield response
 
-    def delete_job(
-        self, *, job: "Job" = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
+    def delete_job(self, *, job: "Job" = None) -> "betterproto_lib_google_protobuf.Empty":
 
         request = DeleteJobRequest()
         if job is not None:
             request.job = job
 
         return self.__rpc_delete_job(request)
 
@@ -1641,15 +1635,15 @@
         self,
         *,
         job: "Job" = None,
         input: "Input" = None,
         filter: "ListDatumRequestFilter" = None,
         pagination_marker: str = "",
         number: int = 0,
-        reverse: bool = False
+        reverse: bool = False,
     ) -> Iterator["DatumInfo"]:
 
         request = ListDatumRequest()
         if job is not None:
             request.job = job
         if input is not None:
             request.input = input
@@ -1726,15 +1720,15 @@
         metadata: "Metadata" = None,
         reprocess_spec: str = "",
         autoscaling: bool = False,
         tolerations: Optional[List["Toleration"]] = None,
         sidecar_resource_requests: "ResourceSpec" = None,
         dry_run: bool = False,
         determined: "Determined" = None,
-        maximum_expected_uptime: timedelta = None
+        maximum_expected_uptime: timedelta = None,
     ) -> "betterproto_lib_google_protobuf.Empty":
         tolerations = tolerations or []
 
         request = CreatePipelineRequest()
         if pipeline is not None:
             request.pipeline = pipeline
         if tf_job is not None:
@@ -1794,15 +1788,15 @@
 
     def create_pipeline_v2(
         self,
         *,
         create_pipeline_request_json: str = "",
         dry_run: bool = False,
         update: bool = False,
-        reprocess: bool = False
+        reprocess: bool = False,
     ) -> "CreatePipelineV2Response":
 
         request = CreatePipelineV2Request()
         request.create_pipeline_request_json = create_pipeline_request_json
         request.dry_run = dry_run
         request.update = update
         request.reprocess = reprocess
@@ -1824,15 +1818,15 @@
         self,
         *,
         pipeline: "Pipeline" = None,
         history: int = 0,
         details: bool = False,
         jq_filter: str = "",
         commit_set: "_pfs__.CommitSet" = None,
-        projects: Optional[List["_pfs__.Project"]] = None
+        projects: Optional[List["_pfs__.Project"]] = None,
     ) -> Iterator["PipelineInfo"]:
         projects = projects or []
 
         request = ListPipelineRequest()
         if pipeline is not None:
             request.pipeline = pipeline
         request.history = history
@@ -1849,15 +1843,15 @@
     def delete_pipeline(
         self,
         *,
         pipeline: "Pipeline" = None,
         all: bool = False,
         force: bool = False,
         keep_repo: bool = False,
-        must_exist: bool = False
+        must_exist: bool = False,
     ) -> "betterproto_lib_google_protobuf.Empty":
 
         request = DeletePipelineRequest()
         if pipeline is not None:
             request.pipeline = pipeline
         request.all = all
         request.force = force
@@ -1868,15 +1862,15 @@
 
     def delete_pipelines(
         self,
         *,
         projects: Optional[List["_pfs__.Project"]] = None,
         force: bool = False,
         keep_repo: bool = False,
-        all: bool = False
+        all: bool = False,
     ) -> "DeletePipelinesResponse":
         projects = projects or []
 
         request = DeletePipelinesRequest()
         if projects is not None:
             request.projects = projects
         request.force = force
@@ -1907,15 +1901,15 @@
         return self.__rpc_stop_pipeline(request)
 
     def run_pipeline(
         self,
         *,
         pipeline: "Pipeline" = None,
         provenance: Optional[List["_pfs__.Commit"]] = None,
-        job_id: str = ""
+        job_id: str = "",
     ) -> "betterproto_lib_google_protobuf.Empty":
         provenance = provenance or []
 
         request = RunPipelineRequest()
         if pipeline is not None:
             request.pipeline = pipeline
         if provenance is not None:
@@ -1992,15 +1986,15 @@
         job: "Job" = None,
         data_filters: Optional[List[str]] = None,
         datum: "Datum" = None,
         master: bool = False,
         follow: bool = False,
         tail: int = 0,
         use_loki_backend: bool = False,
-        since: timedelta = None
+        since: timedelta = None,
     ) -> Iterator["LogMessage"]:
         data_filters = data_filters or []
 
         request = GetLogsRequest()
         if pipeline is not None:
             request.pipeline = pipeline
         if job is not None:
@@ -2032,15 +2026,15 @@
         reason: str = "",
         restart: int = 0,
         data_processed: int = 0,
         data_skipped: int = 0,
         data_failed: int = 0,
         data_recovered: int = 0,
         data_total: int = 0,
-        stats: "ProcessStats" = None
+        stats: "ProcessStats" = None,
     ) -> "betterproto_lib_google_protobuf.Empty":
 
         request = UpdateJobStateRequest()
         if job is not None:
             request.job = job
         request.state = state
         request.reason = reason
@@ -2059,15 +2053,15 @@
         self,
         *,
         dag_spec: str = "",
         load_spec: str = "",
         seed: int = 0,
         parallelism: int = 0,
         pod_patch: str = "",
-        state_id: str = ""
+        state_id: str = "",
     ) -> "RunLoadTestResponse":
 
         request = RunLoadTestRequest()
         request.dag_spec = dag_spec
         request.load_spec = load_spec
         request.seed = seed
         request.parallelism = parallelism
@@ -2133,15 +2127,15 @@
 
     def set_cluster_defaults(
         self,
         *,
         regenerate: bool = False,
         reprocess: bool = False,
         dry_run: bool = False,
-        cluster_defaults_json: str = ""
+        cluster_defaults_json: str = "",
     ) -> "SetClusterDefaultsResponse":
 
         request = SetClusterDefaultsRequest()
         request.regenerate = regenerate
         request.reprocess = reprocess
         request.dry_run = dry_run
         request.cluster_defaults_json = cluster_defaults_json
@@ -2161,15 +2155,15 @@
     def set_project_defaults(
         self,
         *,
         project: "_pfs__.Project" = None,
         regenerate: bool = False,
         reprocess: bool = False,
         dry_run: bool = False,
-        project_defaults_json: str = ""
+        project_defaults_json: str = "",
     ) -> "SetProjectDefaultsResponse":
 
         request = SetProjectDefaultsRequest()
         if project is not None:
             request.project = project
         request.regenerate = regenerate
         request.reprocess = reprocess
```

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/_additions.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/_additions.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/extension.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/taskapi/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/taskapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/transaction/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/transaction/extension.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/transaction/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/version/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/worker/__init__.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/api/worker/extension.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/api/worker/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/client.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/client.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/config.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/config.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/constants.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/datum_batching.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/datum_batching.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/errors.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pachyderm_sdk/interceptor.py` & `pachyderm_sdk-2.9.5/pachyderm_sdk/interceptor.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.4/pyproject.toml` & `pachyderm_sdk-2.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pachyderm_sdk"
-version = "2.9.4"
+version = "2.9.5"
 description = "Python Pachyderm Client"
 authors = ["Pachyderm Integrations <integrations@pachyderm.io>"]
 license = "Apache 2.0"
 documentation = "https://docs.pachyderm.com/latest/sdk/python/"
 readme = 'README.md'
 repository = "https://github.com/pachyderm/pachyderm/tree/master/python-sdk"
 keywords = ["pachyderm"]
```

### Comparing `pachyderm_sdk-2.9.4/PKG-INFO` & `pachyderm_sdk-2.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pachyderm-sdk
-Version: 2.9.4
+Version: 2.9.5
 Summary: Python Pachyderm Client
 Home-page: https://github.com/pachyderm/pachyderm/tree/master/python-sdk
 License: Apache 2.0
 Keywords: pachyderm
 Author: Pachyderm Integrations
 Author-email: integrations@pachyderm.io
 Requires-Python: >=3.8,<4.0
```

