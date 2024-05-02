# Comparing `tmp/lsst-ctrl-bps-htcondor-26.2024.900.tar.gz` & `tmp/lsst_ctrl_bps_htcondor-27.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-ctrl-bps-htcondor-26.2024.900.tar", last modified: Thu Feb 29 10:20:31 2024, max compression
+gzip compressed data, was "lsst_ctrl_bps_htcondor-27.0.0rc1.tar", last modified: Wed May  1 21:16:50 2024, max compression
```

## Comparing `lsst-ctrl-bps-htcondor-26.2024.900.tar` & `lsst_ctrl_bps_htcondor-27.0.0rc1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.059387 lsst-ctrl-bps-htcondor-26.2024.900/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-29 10:20:31.059387 lsst-ctrl-bps-htcondor-26.2024.900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.051387 lsst-ctrl-bps-htcondor-26.2024.900/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.055387 lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.051387 lsst-ctrl-bps-htcondor-26.2024.900/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.051387 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.051387 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.051387 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.055387 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74496 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/htcondor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    53700 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/lssthtc.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:30.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.059387 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-29 10:20:31.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-29 10:20:31.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:31.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-29 10:20:31.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:20:31.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:30.000000 lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-29 10:20:31.059387 lsst-ctrl-bps-htcondor-26.2024.900/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:31.059387 lsst-ctrl-bps-htcondor-26.2024.900/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/tests/test_htcondor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-02-29 10:20:17.000000 lsst-ctrl-bps-htcondor-26.2024.900/tests/test_lssthtc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:50.331132 lsst_ctrl_bps_htcondor-27.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-01 21:16:50.331132 lsst_ctrl_bps_htcondor-27.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:50.323132 lsst_ctrl_bps_htcondor-27.0.0rc1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:50.327132 lsst_ctrl_bps_htcondor-27.0.0rc1/doc/lsst.ctrl.bps.htcondor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/doc/lsst.ctrl.bps.htcondor/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/doc/lsst.ctrl.bps.htcondor/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/doc/lsst.ctrl.bps.htcondor/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:50.323132 lsst_ctrl_bps_htcondor-27.0.0rc1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:50.323132 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:50.323132 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/ctrl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:50.323132 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/ctrl/bps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:50.327132 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/ctrl/bps/htcondor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/ctrl/bps/htcondor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/ctrl/bps/htcondor/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74636 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/ctrl/bps/htcondor/htcondor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54062 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/ctrl/bps/htcondor/lssthtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:16:50.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/ctrl/bps/htcondor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:50.331132 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst_ctrl_bps_htcondor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-01 21:16:50.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-01 21:16:50.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:50.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst_ctrl_bps_htcondor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-01 21:16:50.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst_ctrl_bps_htcondor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:16:50.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst_ctrl_bps_htcondor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:49.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst_ctrl_bps_htcondor.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-01 21:16:50.331132 lsst_ctrl_bps_htcondor-27.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:50.331132 lsst_ctrl_bps_htcondor-27.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/tests/test_htcondor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-01 21:16:44.000000 lsst_ctrl_bps_htcondor-27.0.0rc1/tests/test_lssthtc.py
```

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/PKG-INFO` & `lsst_ctrl_bps_htcondor-27.0.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-htcondor
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: HTCondor plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_htcondor
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/README.rst` & `lsst_ctrl_bps_htcondor-27.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/bsd_license.txt` & `lsst_ctrl_bps_htcondor-27.0.0rc1/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/CHANGES.rst` & `lsst_ctrl_bps_htcondor-27.0.0rc1/doc/lsst.ctrl.bps.htcondor/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/index.rst` & `lsst_ctrl_bps_htcondor-27.0.0rc1/doc/lsst.ctrl.bps.htcondor/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/doc/lsst.ctrl.bps.htcondor/userguide.rst` & `lsst_ctrl_bps_htcondor-27.0.0rc1/doc/lsst.ctrl.bps.htcondor/userguide.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/gpl-v3.0.txt` & `lsst_ctrl_bps_htcondor-27.0.0rc1/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/pyproject.toml` & `lsst_ctrl_bps_htcondor-27.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/__init__.py` & `lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/ctrl/bps/htcondor/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/htcondor_service.py` & `lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/ctrl/bps/htcondor/htcondor_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,22 +139,24 @@
 
         with time_this(
             log=_LOG, level=logging.INFO, prefix=None, msg="Completed writing out HTCondor workflow"
         ):
             workflow.write(out_prefix)
         return workflow
 
-    def submit(self, workflow):
+    def submit(self, workflow, **kwargs):
         """Submit a single HTCondor workflow.
 
         Parameters
         ----------
         workflow : `lsst.ctrl.bps.BaseWorkflow`
             A single HTCondor workflow to submit.  run_id is updated after
             successful submission to WMS.
+        **kwargs : `~typing.Any`
+            Keyword arguments for the options.
         """
         dag = workflow.dag
 
         ver = version.parse(htc_version())
         if ver >= version.parse("8.9.3"):
             sub = htc_create_submit_from_dag(dag.graph["dag_filename"], {})
         else:
@@ -1022,15 +1024,15 @@
         # If the provided workflow id does not correspond to the one extracted
         # from the DAGMan log file in the submit directory, rerun the query
         # with the id found in the file.
         #
         # This is to cover the situation in which the user provided the old job
         # id of a restarted run.
         try:
-            path_dag_id, path_dag_ad = read_dag_log(dag_ad["Iwd"])
+            path_dag_id, _ = read_dag_log(dag_ad["Iwd"])
         except FileNotFoundError as exc:
             # At the moment missing DAGMan log is pretty much a fatal error.
             # So empty the DAG info to finish early (see the if statement
             # below).
             schedd_dag_info.clean()
             messages.append(f"Cannot create the report for '{dag_id}': {exc}")
         else:
@@ -1428,28 +1430,26 @@
     for job_id, job_ad in jobs.items():
         job_label = job_ad["bps_job_label"]
         summary.setdefault(job_label, [])
         try:
             exit_code = 0
             job_status = job_ad["JobStatus"]
             match job_status:
-                case JobStatus.COMPLETED:
+                case JobStatus.COMPLETED | JobStatus.HELD:
                     exit_code = job_ad["ExitSignal"] if job_ad["ExitBySignal"] else job_ad["ExitCode"]
-                case JobStatus.HELD:
-                    exit_code = job_ad["ExitSignal"] if job_ad["ExitBySignal"] else job_ad["HoldReasonCode"]
                 case (
                     JobStatus.IDLE
                     | JobStatus.RUNNING
                     | JobStatus.REMOVED
                     | JobStatus.TRANSFERRING_OUTPUT
                     | JobStatus.SUSPENDED
                 ):
                     pass
                 case _:
-                    _LOG.debug("Unknown 'JobStatus' value ('%d') in classad for job '%d'", job_status, job_id)
+                    _LOG.debug("Unknown 'JobStatus' value ('%d') in classad for job '%s'", job_status, job_id)
             if exit_code != 0:
                 summary[job_label].append(exit_code)
         except KeyError as ex:
             _LOG.debug("Attribute '%s' not found in the classad for job '%s'", ex, job_id)
     return summary
 
 
@@ -1509,25 +1509,27 @@
     if "DAG_NodesReady" in job:
         state_counts = {
             WmsStates.UNREADY: job.get("DAG_NodesUnready", 0),
             WmsStates.READY: job.get("DAG_NodesReady", 0),
             WmsStates.HELD: job.get("JobProcsHeld", 0),
             WmsStates.SUCCEEDED: job.get("DAG_NodesDone", 0),
             WmsStates.FAILED: job.get("DAG_NodesFailed", 0),
+            WmsStates.PRUNED: job.get("DAG_NodesFutile", 0),
             WmsStates.MISFIT: job.get("DAG_NodesPre", 0) + job.get("DAG_NodesPost", 0),
         }
         total_jobs = job.get("DAG_NodesTotal")
         _LOG.debug("_get_state_counts_from_dag_job: from DAG_* keys, total_jobs = %s", total_jobs)
     elif "NodesFailed" in job:
         state_counts = {
             WmsStates.UNREADY: job.get("NodesUnready", 0),
             WmsStates.READY: job.get("NodesReady", 0),
             WmsStates.HELD: job.get("JobProcsHeld", 0),
             WmsStates.SUCCEEDED: job.get("NodesDone", 0),
             WmsStates.FAILED: job.get("NodesFailed", 0),
+            WmsStates.PRUNED: job.get("NodesFutile", 0),
             WmsStates.MISFIT: job.get("NodesPre", 0) + job.get("NodesPost", 0),
         }
         try:
             total_jobs = job.get("NodesTotal")
         except KeyError as ex:
             _LOG.error("Job missing %s. job = %s", str(ex), job)
             raise
@@ -1591,65 +1593,64 @@
         wms_state = WmsStates.DELETED
     elif job_status == JobStatus.COMPLETED:
         if (
             job.get("ExitBySignal", False)
             or job.get("ExitCode", 0)
             or job.get("ExitSignal", 0)
             or job.get("DAG_Status", 0)
-            or job.get("ReturnValue", 0)
         ):
             wms_state = WmsStates.FAILED
         else:
             wms_state = WmsStates.SUCCEEDED
     elif job_status == JobStatus.HELD:
         wms_state = WmsStates.HELD
 
     return wms_state
 
 
 def _htc_node_status_to_wms_state(job):
-    """Convert HTCondor status to generic wms state.
+    """Convert HTCondor node status to generic wms state.
 
     Parameters
     ----------
     job : `dict` [`str`, `Any`]
         HTCondor job information.
 
     Returns
     -------
     wms_state : `lsst.ctrl.bps.WmsStates`
         The equivalent WmsState to given node's status.
     """
     wms_state = WmsStates.MISFIT
-
-    status = job["NodeStatus"]
-    if status == NodeStatus.NOT_READY:
-        wms_state = WmsStates.UNREADY
-    elif status == NodeStatus.READY:
-        wms_state = WmsStates.READY
-    elif status == NodeStatus.PRERUN:
-        wms_state = WmsStates.MISFIT
-    elif status == NodeStatus.SUBMITTED:
-        if job["JobProcsHeld"]:
-            wms_state = WmsStates.HELD
-        elif job["StatusDetails"] == "not_idle":
-            wms_state = WmsStates.RUNNING
-        elif job["JobProcsQueued"]:
-            wms_state = WmsStates.PENDING
-    elif status == NodeStatus.POSTRUN:
-        wms_state = WmsStates.MISFIT
-    elif status == NodeStatus.DONE:
-        wms_state = WmsStates.SUCCEEDED
-    elif status == NodeStatus.ERROR:
-        # Use job exist instead of post script exit
-        if "DAGMAN error 0" in job["StatusDetails"]:
+    match job["NodeStatus"]:
+        case NodeStatus.NOT_READY:
+            wms_state = WmsStates.UNREADY
+        case NodeStatus.READY:
+            wms_state = WmsStates.READY
+        case NodeStatus.PRERUN:
+            wms_state = WmsStates.MISFIT
+        case NodeStatus.SUBMITTED:
+            if job["JobProcsHeld"]:
+                wms_state = WmsStates.HELD
+            elif job["StatusDetails"] == "not_idle":
+                wms_state = WmsStates.RUNNING
+            elif job["JobProcsQueued"]:
+                wms_state = WmsStates.PENDING
+        case NodeStatus.POSTRUN:
+            wms_state = WmsStates.MISFIT
+        case NodeStatus.DONE:
             wms_state = WmsStates.SUCCEEDED
-        else:
-            wms_state = WmsStates.FAILED
-
+        case NodeStatus.ERROR:
+            # Use job exit status instead of post script exit status.
+            if "DAGMAN error 0" in job["StatusDetails"]:
+                wms_state = WmsStates.SUCCEEDED
+            else:
+                wms_state = WmsStates.FAILED
+        case NodeStatus.FUTILE:
+            wms_state = WmsStates.PRUNED
     return wms_state
 
 
 def _update_jobs(jobs1, jobs2):
     """Update jobs1 with info in jobs2.
 
     (Basically an update for nested dictionaries.)
```

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/python/lsst/ctrl/bps/htcondor/lssthtc.py` & `lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst/ctrl/bps/htcondor/lssthtc.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
 from pathlib import Path
 
 import classad
 import htcondor
 import networkx
 from packaging import version
 
+from .handlers import HTC_JOB_AD_HANDLERS
+
 _LOG = logging.getLogger(__name__)
 
 MISSING_ID = -99999
 
 
 class DagStatus(IntEnum):
     """HTCondor DAGMan's statuses for a DAG."""
@@ -143,14 +145,17 @@
     # (STATUS_DONE): The node has completed successfully.
     DONE = 5
 
     # (STATUS_ERROR): The node has failed. StatusDetails has info (e.g.,
     # ULOG_JOB_ABORTED for deleted job).
     ERROR = 6
 
+    # (STATUS_FUTILE): The node will never run because ancestor node failed.
+    FUTILE = 7
+
 
 HTC_QUOTE_KEYS = {"environment"}
 HTC_VALID_JOB_KEYS = {
     "universe",
     "executable",
     "arguments",
     "environment",
@@ -1359,15 +1364,20 @@
     ----------
     wms_path : `str`
         Path that includes node status file for a run.
 
     Returns
     -------
     jobs : `dict` [`str`, Any]
-        DAG summary information.
+        DAG summary information compiled from the node status file combined
+        with the information found in the node event log.
+
+        Currently, if the same job attribute is found in both files, its value
+        from the event log takes precedence over the value from the node status
+        file.
     """
     # Get jobid info from other places to fill in gaps in info from node_status
     _, job_name_to_pipetask = summary_from_dag(wms_path)
     wms_workflow_id, loginfo = read_dag_log(wms_path)
     loginfo = read_dag_nodes_log(wms_path)
     _LOG.debug("loginfo = %s", loginfo)
     job_name_to_id = {}
@@ -1407,26 +1417,30 @@
                     elif "_" in jclassad["Node"]:
                         label = jclassad["Node"].split("_")[1]
                     else:
                         label = jclassad["Node"]
 
                     # Make job info as if came from condor_q
                     if jclassad["Node"] in job_name_to_id:
-                        job_id = job_name_to_id[jclassad["Node"]]
+                        job_id = str(job_name_to_id[jclassad["Node"]])
                     else:
                         job_id = str(fake_id)
                         fake_id -= 1
 
                     job = dict(jclassad)
                     job["ClusterId"] = int(float(job_id))
                     job["DAGManJobID"] = wms_workflow_id
                     job["DAGNodeName"] = jclassad["Node"]
                     job["bps_job_label"] = label
 
-                    jobs[str(job_id)] = job
+                    jobs[job_id] = job
+                    try:
+                        jobs[job_id] |= loginfo[job_id]
+                    except KeyError:
+                        pass
     except (OSError, PermissionError):
         pass
 
     return jobs
 
 
 def read_dag_log(wms_path):
@@ -1585,43 +1599,45 @@
     filename : `pathlib.Path`
         Name of the DAGMan log.
     job : `dict` [ `str`, Any ]
         A mapping between HTCondor job id and job information read from
         the log.
     """
     _LOG.debug("_tweak_log_info: %s %s", filename, job)
+
     try:
         job["ClusterId"] = job["Cluster"]
         job["ProcId"] = job["Proc"]
         job["Iwd"] = str(filename.parent)
         job["Owner"] = filename.owner()
-        if job["MyType"] == "ExecuteEvent":
-            job["JobStatus"] = JobStatus.RUNNING
-        elif job["MyType"] == "JobTerminatedEvent" or job["MyType"] == "PostScriptTerminatedEvent":
-            job["JobStatus"] = JobStatus.COMPLETED
-            try:
-                if not job["TerminatedNormally"]:
-                    if "ReturnValue" in job:
-                        job["ExitCode"] = job["ReturnValue"]
-                        job["ExitBySignal"] = False
-                    elif "TerminatedBySignal" in job:
-                        job["ExitBySignal"] = True
-                        job["ExitSignal"] = job["TerminatedBySignal"]
-                    else:
-                        _LOG.warning("Could not determine exit status for completed job: %s", job)
-            except KeyError as ex:
-                _LOG.error("Could not determine exit status for job (missing %s): %s", str(ex), job)
-        elif job["MyType"] == "SubmitEvent":
-            job["JobStatus"] = JobStatus.IDLE
-        elif job["MyType"] == "JobAbortedEvent":
-            job["JobStatus"] = JobStatus.REMOVED
-        else:
-            _LOG.debug("Unknown log event type: %s", job["MyType"])
-    except KeyError:
-        _LOG.error("Missing key in job: %s", job)
+
+        match job["MyType"]:
+            case "ExecuteEvent":
+                job["JobStatus"] = JobStatus.RUNNING
+            case "JobTerminatedEvent" | "PostScriptTerminatedEvent":
+                job["JobStatus"] = JobStatus.COMPLETED
+            case "SubmitEvent":
+                job["JobStatus"] = JobStatus.IDLE
+            case "JobAbortedEvent":
+                job["JobStatus"] = JobStatus.REMOVED
+            case "JobHeldEvent":
+                job["JobStatus"] = JobStatus.HELD
+            case _:
+                _LOG.debug("Unknown log event type: %s", job["MyType"])
+                job["JobStatus"] = JobStatus.UNEXPANDED
+
+        if job["JobStatus"] in {JobStatus.COMPLETED, JobStatus.HELD}:
+            new_job = HTC_JOB_AD_HANDLERS.handle(job)
+            if new_job is not None:
+                job = new_job
+            else:
+                _LOG.error("Could not determine exit status for job '%s.%s'", job["ClusterId"], job["ProcId"])
+
+    except KeyError as e:
+        _LOG.error("Missing key %s in job: %s", str(e), job)
         raise
 
 
 def htc_check_dagman_output(wms_path):
     """Check the DAGMan output for error messages.
 
     Parameters
```

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO` & `lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-htcondor
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: HTCondor plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_htcondor
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt` & `lsst_ctrl_bps_htcondor-27.0.0rc1/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 gpl-v3.0.txt
 pyproject.toml
 setup.cfg
 doc/lsst.ctrl.bps.htcondor/CHANGES.rst
 doc/lsst.ctrl.bps.htcondor/index.rst
 doc/lsst.ctrl.bps.htcondor/userguide.rst
 python/lsst/ctrl/bps/htcondor/__init__.py
+python/lsst/ctrl/bps/htcondor/handlers.py
 python/lsst/ctrl/bps/htcondor/htcondor_service.py
 python/lsst/ctrl/bps/htcondor/lssthtc.py
 python/lsst/ctrl/bps/htcondor/version.py
 python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO
 python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt
 python/lsst_ctrl_bps_htcondor.egg-info/dependency_links.txt
 python/lsst_ctrl_bps_htcondor.egg-info/requires.txt
 python/lsst_ctrl_bps_htcondor.egg-info/top_level.txt
 python/lsst_ctrl_bps_htcondor.egg-info/zip-safe
+tests/test_handlers.py
 tests/test_htcondor_service.py
 tests/test_lssthtc.py
```

### Comparing `lsst-ctrl-bps-htcondor-26.2024.900/tests/test_lssthtc.py` & `lsst_ctrl_bps_htcondor-27.0.0rc1/tests/test_lssthtc.py`

 * *Files identical despite different names*

