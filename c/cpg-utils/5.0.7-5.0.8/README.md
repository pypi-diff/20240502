# Comparing `tmp/cpg-utils-5.0.7.tar.gz` & `tmp/cpg-utils-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpg-utils-5.0.7.tar", last modified: Fri Apr 19 03:50:40 2024, max compression
+gzip compressed data, was "cpg-utils-5.0.8.tar", last modified: Thu May  2 01:13:42 2024, max compression
```

## Comparing `cpg-utils-5.0.7.tar` & `cpg-utils-5.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:50:40.780823 cpg-utils-5.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-19 03:50:40.780823 cpg-utils-5.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:50:40.780823 cpg-utils-5.0.7/cpg_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/cromwell_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/dataproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/hail_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/membership.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/cpg_utils/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:50:40.780823 cpg-utils-5.0.7/cpg_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-19 03:50:40.000000 cpg-utils-5.0.7/cpg_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-19 03:50:40.000000 cpg-utils-5.0.7/cpg_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:50:40.000000 cpg-utils-5.0.7/cpg_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 03:50:40.000000 cpg-utils-5.0.7/cpg_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 03:50:40.000000 cpg-utils-5.0.7/cpg_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:50:40.780823 cpg-utils-5.0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:50:40.780823 cpg-utils-5.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/test/test_cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-19 03:50:39.000000 cpg-utils-5.0.7/test/test_doctests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/cpg_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27898 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/cromwell_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/hail_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/cpg_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-02 01:13:42.000000 cpg-utils-5.0.8/cpg_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-02 01:13:42.000000 cpg-utils-5.0.8/cpg_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:13:42.000000 cpg-utils-5.0.8/cpg_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-02 01:13:42.000000 cpg-utils-5.0.8/cpg_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 01:13:42.000000 cpg-utils-5.0.8/cpg_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/test/test_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/test/test_doctests.py
```

### Comparing `cpg-utils-5.0.7/LICENSE` & `cpg-utils-5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/PKG-INFO` & `cpg-utils-5.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.7
+Version: 5.0.8
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.7/README.md` & `cpg-utils-5.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils/__init__.py` & `cpg-utils-5.0.8/cpg_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils/cloud.py` & `cpg-utils-5.0.8/cpg_utils/cloud.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils/cloudpath_hail_az.py` & `cpg-utils-5.0.8/cpg_utils/cloudpath_hail_az.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils/config.py` & `cpg-utils-5.0.8/cpg_utils/config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils/constants.py` & `cpg-utils-5.0.8/cpg_utils/constants.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils/cromwell.py` & `cpg-utils-5.0.8/cpg_utils/cromwell.py`

 * *Files 3% similar despite different names*

```diff
@@ -283,14 +283,15 @@
     commit: str | None = None,
     cwd: str | None = None,
     driver_image: str | None = None,
     project: str | None = None,
     copy_outputs_to_gcp: bool = True,
     min_watch_poll_interval: int = 5,
     max_watch_poll_interval: int = 60,
+    time_limit_seconds: int | None = None,
 ) -> tuple[Job, dict[str, Resource | list[Resource]]]:
     """
     This function needs to know the structure of the outputs you
     want to collect. It currently only supports:
         - a single value, or
         - a list of values
 
@@ -305,14 +306,17 @@
     If copy_outputs_to_gcp is True, the outputs will be copied to GCS.
     Workflows may then choose to copy these outputs to a final destination.
 
     Returns a submit Job object, and a dict of output Resource objects.
 
     Optionally override min/max poll interval for the watch job.
     This alters how often the Watch job pings Cromwell for Status updates
+
+    time_limit_seconds is optional, and will cause the workflow to be aborted if
+    the time limit is exceeded
     """
 
     _driver_image = driver_image or get_driver_image()
     access_level = get_access_level()
 
     submit_job = b.new_job(f'{job_prefix}_submit')
     submit_job.image(_driver_image)
@@ -342,33 +346,45 @@
         b,
         job_prefix=job_prefix,
         workflow_id_file=workflow_id_file,
         outputs_to_collect=outputs_to_collect,
         driver_image=_driver_image,
         max_poll_interval=max_watch_poll_interval,
         min_poll_interval=min_watch_poll_interval,
+        time_limit_seconds=time_limit_seconds,
     )
 
     return submit_job, outputs_dict
 
 
 def watch_workflow(  # noqa: C901
     workflow_id_file: str,
     max_sequential_exception_count: int,
     min_poll_interval: int,
     max_poll_interval: int,
     exponential_decrease_seconds: int,
     output_json_path: str,
+    time_limit_seconds: int | None = None,
 ):
     """
     INNER Python function to watch workflow status, and write
     output paths to output_json_path on success.
+
+    Re-importing dependencies here so the function is self-contained
+    and can be run in a Hail bash job.
+
+    Args:
+        workflow_id_file (str): file containing the Cromwell WF ID only
+        max_sequential_exception_count (int): Fail after X consecutive errors
+        min_poll_interval (int): minimum polling wait
+        max_poll_interval (int): maximum polling wait
+        exponential_decrease_seconds (int): expo curve for interval generation
+        output_json_path (str): where to write output results file
+        time_limit_seconds (int): kill if not completed before X seconds pass
     """
-    # Re-importing dependencies here so the function is self-contained
-    # and can be run in a Hail bash job.
 
     import json
     import logging
     import math
     import subprocess
     import time
     from datetime import datetime
@@ -425,29 +441,47 @@
     logger.info(f'Received workflow ID: {workflow_id}')
 
     failed_statuses = {'failed', 'aborted'}
     terminal_statuses = {'succeeded'} | failed_statuses
     status_reported = False
     subprocess.check_output(GCLOUD_ACTIVATE_AUTH_BASE)  # noqa: S603
     cromwell_workflow_root = f'{CROMWELL_URL}/api/workflows/v1/{workflow_id}'
+    abort_url = f'{cromwell_workflow_root}/abort'
     metadata_url = f'{cromwell_workflow_root}/metadata'
     outputs_url = f'{cromwell_workflow_root}/outputs'
     status_url = f'{cromwell_workflow_root}/status'
     _remaining_exceptions = max_sequential_exception_count
     start = datetime.now()
 
     while True:
+        # kill the workflow if the maximum wait has elapsed
+        if (
+            time_limit_seconds
+            and (datetime.now() - start).total_seconds() >= time_limit_seconds
+        ):
+            # time to die, Mr. Cromwell
+            auth_header = {'Authorization': f'Bearer {_get_cromwell_oauth_token()}'}
+            r = requests.post(abort_url, headers=auth_header, timeout=10)
+            if not r.ok:
+                logger.info(
+                    f"Abort failed, error code {r.status_code}, WF ID: {workflow_id}",
+                )
+                _remaining_exceptions -= 1
+                continue
+
         if _remaining_exceptions <= 0:
             raise CromwellError('Unreachable')
+
         wait_time = _get_wait_interval(
             start,
             min_poll_interval,
             max_poll_interval,
             exponential_decrease_seconds,
         )
+
         try:
             auth_header = {'Authorization': f'Bearer {_get_cromwell_oauth_token()}'}
             r = requests.get(status_url, headers=auth_header, timeout=60)
             if not r.ok:
                 _remaining_exceptions -= 1
                 logger.warning(
                     f'Received "not okay" (status={r.status_code}) from cromwell '
@@ -509,14 +543,15 @@
     workflow_id_file: Resource,
     outputs_to_collect: dict[str, CromwellOutputType],
     driver_image: str | None = None,
     min_poll_interval: int = 5,  # 5 seconds
     max_poll_interval: int = 60,  # 1 minute
     exponential_decrease_seconds: int = 1200,  # 20 minutes
     max_sequential_exception_count: int = 25,
+    time_limit_seconds: int | None = None,
 ):
     """
     This is a little bit tricky, but the process is:
 
     - Wait for a cromwell workflow to finish,
     - If it succeeds, get the outputs (as a json)
     - (Hard) Get the value of the output back into Hail Batch as a resource file.
@@ -537,14 +572,15 @@
     :param b: Batch object
     :param job_prefix: Prefix for the job name
     :param workflow_id_file: File containing the workflow ID
     :param outputs_to_collect: dict of output name -> CromwellOutputType
     :param max_poll_interval: Maximum time to wait between polls
     :param exponential_decrease_seconds: Exponential decrease in wait time
     :param max_sequential_exception_count: Maximum number of exceptions before giving up
+    :param time_limit_seconds: a maximum runtime before abort is triggered
     """
 
     driver_image = driver_image or get_driver_image()
 
     watch_job = b.new_job(job_prefix + '_watch')
     watch_job.cpu(0.25)
 
@@ -558,14 +594,15 @@
             watch_workflow.__name__,
             str(workflow_id_file),
             max_sequential_exception_count,
             min_poll_interval,
             max_poll_interval,
             exponential_decrease_seconds,
             str(watch_job.output_json_path),
+            time_limit_seconds,
             setup_gcp=True,
             setup_hail=False,
         ),
     )
 
     rdict = watch_job.output_json_path
```

### Comparing `cpg-utils-5.0.7/cpg_utils/cromwell_model.py` & `cpg-utils-5.0.8/cpg_utils/cromwell_model.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils/dataproc.py` & `cpg-utils-5.0.8/cpg_utils/dataproc.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils/git.py` & `cpg-utils-5.0.8/cpg_utils/git.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils/hail_batch.py` & `cpg-utils-5.0.8/cpg_utils/hail_batch.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils/membership.py` & `cpg-utils-5.0.8/cpg_utils/membership.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils/slack.py` & `cpg-utils-5.0.8/cpg_utils/slack.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/cpg_utils.egg-info/PKG-INFO` & `cpg-utils-5.0.8/cpg_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.7
+Version: 5.0.8
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.7/cpg_utils.egg-info/SOURCES.txt` & `cpg-utils-5.0.8/cpg_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/pyproject.toml` & `cpg-utils-5.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/setup.py` & `cpg-utils-5.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='cpg-utils',
     # This tag is automatically updated by bumpversion
-    version='5.0.7',
+    version='5.0.8',
     description='Library of convenience functions specific to the CPG',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/populationgenomics/cpg-utils',
     license='MIT',
     packages=find_packages(),
     package_data={
```

### Comparing `cpg-utils-5.0.7/test/test_config.py` & `cpg-utils-5.0.8/test/test_config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.7/test/test_cromwell.py` & `cpg-utils-5.0.8/test/test_cromwell.py`

 * *Files identical despite different names*

