# Comparing `tmp/license_manager_agent-3.2.0.tar.gz` & `tmp/license_manager_agent-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_agent-3.2.0.tar", max compression
+gzip compressed data, was "license_manager_agent-3.2.1.tar", max compression
```

## Comparing `license_manager_agent-3.2.0.tar` & `license_manager_agent-3.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1911 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/backend_utils/__init__.py
--rw-r--r--   0        0        0      288 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/backend_utils/constants.py
--rw-r--r--   0        0        0     1808 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/backend_utils/models.py
--rw-r--r--   0        0        0     9582 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/backend_utils/utils.py
--rw-r--r--   0        0        0     3473 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/config.py
--rw-r--r--   0        0        0     1150 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/exceptions.py
--rw-r--r--   0        0        0     2519 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/logs.py
--rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/__init__.py
--rw-r--r--   0        0        0     4942 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/flexlm.py
--rw-r--r--   0        0        0     3953 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/lmx.py
--rw-r--r--   0        0        0     4521 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/lsdyna.py
--rw-r--r--   0        0        0     4860 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/olicense.py
--rw-r--r--   0        0        0     3405 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/parsing/rlm.py
--rwxr-xr-x   0        0        0     1063 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/reconcile.py
--rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/__init__.py
--rw-r--r--   0        0        0     3002 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/flexlm.py
--rw-r--r--   0        0        0     1871 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/license_server_interface.py
--rw-r--r--   0        0        0     2844 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/lmx.py
--rw-r--r--   0        0        0     2810 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/lsdyna.py
--rw-r--r--   0        0        0     2802 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/olicense.py
--rw-r--r--   0        0        0     2737 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/server_interfaces/rlm.py
--rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/services/__init__.py
--rw-r--r--   0        0        0     9881 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/services/clean_jobs_and_bookings.py
--rw-r--r--   0        0        0     4721 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/services/license_report.py
--rw-r--r--   0        0        0      496 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/services/models.py
--rw-r--r--   0        0        0     6323 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/services/reconciliation.py
--rw-r--r--   0        0        0     1269 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/utils.py
--rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/__init__.py
--rw-r--r--   0        0        0     8894 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/cmd_utils.py
--rw-r--r--   0        0        0     1036 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/common.py
--rw-r--r--   0        0        0     3732 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/reservations.py
--rw-r--r--   0        0        0     1610 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/slurmctld_epilog.py
--rw-r--r--   0        0        0     3939 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/slurmctld_prolog.py
--rw-r--r--   0        0        0     1825 2024-04-29 19:53:22.544947 license_manager_agent-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 license_manager_agent-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1911 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/backend_utils/__init__.py
+-rw-r--r--   0        0        0      288 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/backend_utils/constants.py
+-rw-r--r--   0        0        0     1808 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/backend_utils/models.py
+-rw-r--r--   0        0        0     9582 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/backend_utils/utils.py
+-rw-r--r--   0        0        0     3473 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/config.py
+-rw-r--r--   0        0        0     1150 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/exceptions.py
+-rw-r--r--   0        0        0     2519 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/logs.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/__init__.py
+-rw-r--r--   0        0        0     4942 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/flexlm.py
+-rw-r--r--   0        0        0     3953 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/lmx.py
+-rw-r--r--   0        0        0     4521 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/lsdyna.py
+-rw-r--r--   0        0        0     4860 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/olicense.py
+-rw-r--r--   0        0        0     3405 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/parsing/rlm.py
+-rwxr-xr-x   0        0        0     1063 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/reconcile.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/__init__.py
+-rw-r--r--   0        0        0     3002 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/flexlm.py
+-rw-r--r--   0        0        0     1871 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/license_server_interface.py
+-rw-r--r--   0        0        0     2844 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/lmx.py
+-rw-r--r--   0        0        0     2810 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/lsdyna.py
+-rw-r--r--   0        0        0     2802 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/olicense.py
+-rw-r--r--   0        0        0     2737 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/server_interfaces/rlm.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/services/__init__.py
+-rw-r--r--   0        0        0     9881 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/services/clean_jobs_and_bookings.py
+-rw-r--r--   0        0        0     4721 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/services/license_report.py
+-rw-r--r--   0        0        0      496 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/services/models.py
+-rw-r--r--   0        0        0     6323 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/services/reconciliation.py
+-rw-r--r--   0        0        0     1269 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/utils.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/workload_managers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/__init__.py
+-rw-r--r--   0        0        0     9717 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/cmd_utils.py
+-rw-r--r--   0        0        0      990 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/common.py
+-rw-r--r--   0        0        0     3735 2024-05-02 17:08:19.576136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/reservations.py
+-rw-r--r--   0        0        0     1616 2024-05-02 17:08:19.580136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/slurmctld_epilog.py
+-rw-r--r--   0        0        0     3945 2024-05-02 17:08:19.580136 license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/slurmctld_prolog.py
+-rw-r--r--   0        0        0     1825 2024-05-02 17:08:19.580136 license_manager_agent-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 license_manager_agent-3.2.1/PKG-INFO
```

### Comparing `license_manager_agent-3.2.0/README.md` & `license_manager_agent-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/backend_utils/models.py` & `license_manager_agent-3.2.1/lm_agent/backend_utils/models.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/backend_utils/utils.py` & `license_manager_agent-3.2.1/lm_agent/backend_utils/utils.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/config.py` & `license_manager_agent-3.2.1/lm_agent/config.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/exceptions.py` & `license_manager_agent-3.2.1/lm_agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/logs.py` & `license_manager_agent-3.2.1/lm_agent/logs.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/parsing/flexlm.py` & `license_manager_agent-3.2.1/lm_agent/parsing/flexlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/parsing/lmx.py` & `license_manager_agent-3.2.1/lm_agent/parsing/lmx.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/parsing/lsdyna.py` & `license_manager_agent-3.2.1/lm_agent/parsing/lsdyna.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/parsing/olicense.py` & `license_manager_agent-3.2.1/lm_agent/parsing/olicense.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/parsing/rlm.py` & `license_manager_agent-3.2.1/lm_agent/parsing/rlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/reconcile.py` & `license_manager_agent-3.2.1/lm_agent/reconcile.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/server_interfaces/flexlm.py` & `license_manager_agent-3.2.1/lm_agent/server_interfaces/flexlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/server_interfaces/license_server_interface.py` & `license_manager_agent-3.2.1/lm_agent/server_interfaces/license_server_interface.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/server_interfaces/lmx.py` & `license_manager_agent-3.2.1/lm_agent/server_interfaces/lmx.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/server_interfaces/lsdyna.py` & `license_manager_agent-3.2.1/lm_agent/server_interfaces/lsdyna.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/server_interfaces/olicense.py` & `license_manager_agent-3.2.1/lm_agent/server_interfaces/olicense.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/server_interfaces/rlm.py` & `license_manager_agent-3.2.1/lm_agent/server_interfaces/rlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/services/clean_jobs_and_bookings.py` & `license_manager_agent-3.2.1/lm_agent/services/clean_jobs_and_bookings.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/services/license_report.py` & `license_manager_agent-3.2.1/lm_agent/services/license_report.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/services/reconciliation.py` & `license_manager_agent-3.2.1/lm_agent/services/reconciliation.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/utils.py` & `license_manager_agent-3.2.1/lm_agent/utils.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/cmd_utils.py` & `license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/cmd_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import re
 import shlex
 import subprocess
 from typing import Dict, List, Optional, Union
 
 from lm_agent.backend_utils.models import LicenseBooking
 from lm_agent.logs import logger
-from lm_agent.workload_managers.slurm.common import (
-    CMD_TIMEOUT,
-    ENCODING,
-    SACCTMGR_PATH,
-    SCONTROL_PATH,
-    SQUEUE_PATH,
-)
+from buzz import require_condition
+
+
+SCONTROL_PATH = "/usr/bin/scontrol"
+SACCTMGR_PATH = "/usr/bin/sacctmgr"
+SQUEUE_PATH = "/usr/bin/squeue"
+CMD_TIMEOUT = 5
+ENCODING = "UTF8"
 
 
 class SqueueParserUnexpectedInputError(ValueError):
     """Unexpected squeue output."""
 
 
 class ScontrolRetrievalFailure(Exception):
@@ -141,14 +142,44 @@
 
     stdout, _ = await asyncio.wait_for(proc.communicate(), CMD_TIMEOUT)
     output = str(stdout, encoding=ENCODING)
     logger.debug("##### scontrol show lic #####")
     return output
 
 
+async def get_lead_host(nodelist):
+    """
+    Get the job's lead host from the nodelist.
+
+    The lead host is the first node in the nodelist.
+    The nodelist can contain multiple lists of nodes inside square brackets.
+    """
+    cmd = [
+        SCONTROL_PATH,
+        "show",
+        "hostnames",
+        nodelist,
+    ]
+
+    proc = await asyncio.create_subprocess_shell(
+        shlex.join(cmd), stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.STDOUT
+    )
+
+    stdout, _ = await asyncio.wait_for(proc.communicate(), CMD_TIMEOUT)
+    output = str(stdout, encoding=ENCODING)
+
+    lead_host = output.split("\n")[0]
+
+    require_condition(
+        lead_host != "", "Could not get lead host from nodelist.", raise_exc_class=ScontrolRetrievalFailure
+    )
+
+    return lead_host
+
+
 async def get_cluster_name() -> str:
     cmd = [
         SACCTMGR_PATH,
         "list",
         "cluster",
         "-nP",
         "format=Cluster",
```

### Comparing `license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/common.py` & `license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """
 Common utilities for slurm commands.
 """
 import os
 
 from lm_agent.logs import logger
+from lm_agent.workload_managers.slurm.cmd_utils import get_lead_host
 
-SCONTROL_PATH = "/usr/bin/scontrol"
-SACCTMGR_PATH = "/usr/bin/sacctmgr"
-SQUEUE_PATH = "/usr/bin/squeue"
-CMD_TIMEOUT = 5
-ENCODING = "UTF8"
 
-
-def get_job_context():
-    """Get and return variables from the job environment."""
+async def get_job_context():
+    """
+    Get and return variables from the job environment.
+    """
     ctxt = dict()
     try:
         ctxt = {
             "cluster_name": os.environ["SLURM_CLUSTER_NAME"],
             "job_id": os.environ["SLURM_JOB_ID"],
-            "lead_host": os.environ["SLURM_JOB_NODELIST"].split(",")[0],
+            "lead_host": await get_lead_host(os.environ["SLURM_JOB_NODELIST"]),
             "user_name": os.environ["SLURM_JOB_USER"],
             "job_licenses": os.environ.get("SLURM_JOB_LICENSES", ""),
         }
+
     except KeyError as e:
         # If not all keys could be assigned, then return non 0 exit status
         logger.error(
             f"All required environment variables were not set, missing: {e}. "
             "Expecting: SLURM_CLUSTER_NAME, SLURM_JOB_ID, SLURM_JOB_NODELIST, "
             "SLURM_JOB_USER, SLURM_JOB_LICENSES"
         )
```

### Comparing `license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/reservations.py` & `license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/reservations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Slurm reservation CRUD module."""
 from typing import Union
 
 from lm_agent.config import settings
 from lm_agent.exceptions import CommandFailedToExecute
 from lm_agent.logs import logger
 from lm_agent.utils import run_command
-from lm_agent.workload_managers.slurm.common import SCONTROL_PATH
+from lm_agent.workload_managers.slurm.cmd_utils import SCONTROL_PATH
 
 
 async def scontrol_create_reservation(licenses: str, duration: str) -> bool:
     """
     Create the reservation for licenses with the specified duration.
 
     Duration format: [days-]hours:minutes:seconds
```

### Comparing `license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/slurmctld_epilog.py` & `license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/slurmctld_epilog.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from lm_agent.workload_managers.slurm.cmd_utils import get_required_licenses_for_job
 from lm_agent.workload_managers.slurm.common import get_job_context
 
 
 async def epilog():
     # Initialize the logger
     init_logging("slurmctld-epilog")
-    job_context = get_job_context()
+    job_context = await get_job_context()
     job_id = job_context["job_id"]
     job_licenses = job_context["job_licenses"]
 
     # Check if reconciliation should be triggered.
     if settings.USE_RECONCILE_IN_PROLOG_EPILOG:
         # Force a reconciliation before we attempt to remove bookings.
         try:
```

### Comparing `license_manager_agent-3.2.0/lm_agent/workload_managers/slurm/slurmctld_prolog.py` & `license_manager_agent-3.2.1/lm_agent/workload_managers/slurm/slurmctld_prolog.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 async def prolog():
     """The PrologSlurmctld for the license-manager-agent."""
     # Initialize the logger
     init_logging("slurmctld-prolog")
     # Acqure the job context
-    job_context = get_job_context()
+    job_context = await get_job_context()
     job_id = job_context.get("job_id", "")
     user_name = job_context.get("user_name")
     lead_host = job_context.get("lead_host")
     job_licenses = job_context.get("job_licenses")
 
     logger.info(f"Prolog started for job id: {job_id}")
```

### Comparing `license_manager_agent-3.2.0/pyproject.toml` & `license_manager_agent-3.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-agent"
-version = "3.2.0"
+version = "3.2.1"
 description = "Provides an agent for interacting with license manager"
 authors = ["OmniVector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [{ include = "lm_agent" }]
```

### Comparing `license_manager_agent-3.2.0/PKG-INFO` & `license_manager_agent-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-manager-agent
-Version: 3.2.0
+Version: 3.2.1
 Summary: Provides an agent for interacting with license manager
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: OmniVector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

