# Comparing `tmp/midori-0.1.0.tar.gz` & `tmp/midori-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midori-0.1.0.tar", max compression
+gzip compressed data, was "midori-1.0.0.tar", max compression
```

## Comparing `midori-0.1.0.tar` & `midori-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      522 2024-05-02 17:02:44.003201 midori-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-02 17:02:44.003201 midori-0.1.0/midori/__init__.py
--rw-r--r--   0        0        0     4193 2024-05-02 17:02:44.003201 midori-0.1.0/midori/core.py
--rw-r--r--   0        0        0     1886 2024-05-02 17:02:44.003201 midori-0.1.0/midori/plugins/base.py
--rw-r--r--   0        0        0      926 2024-05-02 17:02:44.003201 midori-0.1.0/midori/plugins/example_plugins.py
--rw-r--r--   0        0        0     5471 2024-05-02 17:02:44.003201 midori-0.1.0/midori/plugins/helpers.py
--rw-r--r--   0        0        0      484 2024-05-02 17:02:44.003201 midori-0.1.0/midori/treatments_helper.py
--rw-r--r--   0        0        0      370 2024-05-02 17:02:44.003201 midori-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 midori-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6670 2024-05-02 20:19:41.986739 midori-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 20:19:41.990738 midori-1.0.0/midori/__init__.py
+-rw-r--r--   0        0        0     4640 2024-05-02 20:19:41.990738 midori-1.0.0/midori/core.py
+-rw-r--r--   0        0        0     1886 2024-05-02 20:19:41.990738 midori-1.0.0/midori/plugins/base.py
+-rw-r--r--   0        0        0      928 2024-05-02 20:19:41.990738 midori-1.0.0/midori/plugins/example_plugins.py
+-rw-r--r--   0        0        0     5473 2024-05-02 20:19:41.990738 midori-1.0.0/midori/plugins/helpers.py
+-rw-r--r--   0        0        0      484 2024-05-02 20:19:41.990738 midori-1.0.0/midori/treatments_helper.py
+-rw-r--r--   0        0        0      425 2024-05-02 20:19:41.990738 midori-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7059 1970-01-01 00:00:00.000000 midori-1.0.0/PKG-INFO
```

### Comparing `midori-0.1.0/midori/core.py` & `midori-1.0.0/midori/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import paramiko
+import random
 from typing import List, Dict, Type
 from .plugins.helpers import PluginHelper
 from .treatments_helper import get_treatments
 from .plugins.base import (
     checkout_branch_based_on_treatment,
     is_a_branch_exist,
     pause,
@@ -12,24 +13,26 @@
 
 class Orchestrator:
     def __init__(
         self,
         hostname: str,
         username: str,
         password: str,
+        repetitions: int,
         before_trial_cooling_time: int,
         trial_timespan: int,
         after_trial_cooling_time: int,
         variables: Dict[str, List[str]],
         subject_path: str,
         before_experiment_plugins: List[Type[PluginHelper]] = [],
         setup_plugins: List[Type[PluginHelper]] = [],
         end_trial_plugins: List[Type[PluginHelper]] = [],
         end_experiment_plugins: List[Type[PluginHelper]] = [],
     ) -> None:
+        self.__repetitions: int = repetitions
         self.__before_experiment_plugins: List[Type[PluginHelper]] = (
             before_experiment_plugins
         )
         self.__subject_path: str = subject_path
         self.__before_trial_cooling_time: int = before_trial_cooling_time
         self.__trial_timespan: int = trial_timespan
         self.__setup_plugins: List[Type[PluginHelper]] = setup_plugins
@@ -58,54 +61,61 @@
                 subject_path=self.__subject_path,
                 treatment="",
                 previous_output=output,
             )
             output = plugin.execute()
 
         print(f"Treatments: {self.treatments}")
-        for treatment in self.treatments:
-            if not is_a_branch_exist(
-                branch=treatment, subject_path=self.__subject_path, ssh=self.__ssh
-            ):
-                print(f"Branch {treatment} does not exist.")
-                continue
-            checkout_branch_based_on_treatment(
-                treatment=treatment, ssh=self.__ssh, subject_path=self.__subject_path
-            )
 
-            # Before Trial Cooling time
-            pause(interval=self.__before_trial_cooling_time)
+        for i in range(self.__repetitions):
+            print(f"Repetition {i+1}")
 
-            # Setup plugins
-            output = None
-            for Plugin in self.__setup_plugins:
-                plugin = Plugin(
+            randomized_treatments = random.sample(self.treatments, len(self.treatments))
+            for treatment in randomized_treatments:
+                if not is_a_branch_exist(
+                    branch=treatment, subject_path=self.__subject_path, ssh=self.__ssh
+                ):
+                    print(f"Branch {treatment} does not exist.")
+                    continue
+                checkout_branch_based_on_treatment(
+                    treatment=treatment,
                     ssh=self.__ssh,
                     subject_path=self.__subject_path,
-                    treatment=treatment,
-                    previous_output=output,
                 )
-                output = plugin.execute()
 
-            # Each trial runs for a specific timespan
-            pause(interval=self.__trial_timespan)
+                # Before Trial Cooling time
+                pause(interval=self.__before_trial_cooling_time)
 
-            # End Trial plugins
-            output = None
-            for Plugin in self.__end_trial_plugins:
-                plugin = Plugin(
-                    ssh=self.__ssh,
-                    subject_path=self.__subject_path,
-                    treatment=treatment,
-                    previous_output=output,
-                )
-                output = plugin.execute()
+                # Setup plugins
+                output = None
+                for Plugin in self.__setup_plugins:
+                    plugin = Plugin(
+                        ssh=self.__ssh,
+                        subject_path=self.__subject_path,
+                        treatment=treatment,
+                        previous_output=output,
+                    )
+                    output = plugin.execute()
+
+                # Each trial runs for a specific timespan
+                pause(interval=self.__trial_timespan)
+
+                # End Trial plugins
+                output = None
+                for Plugin in self.__end_trial_plugins:
+                    plugin = Plugin(
+                        ssh=self.__ssh,
+                        subject_path=self.__subject_path,
+                        treatment=treatment,
+                        previous_output=output,
+                    )
+                    output = plugin.execute()
 
-            # After Trial Cooling time
-            pause(interval=self.__after_trial_cooling_time)
+                # After Trial Cooling time
+                pause(interval=self.__after_trial_cooling_time)
 
         # End Experiment plugins
         output = None
         for Plugin in self.__end_experiment_plugins:
             plugin = Plugin(
                 ssh=self.__ssh,
                 subject_path=self.__subject_path,
```

### Comparing `midori-0.1.0/midori/plugins/base.py` & `midori-1.0.0/midori/plugins/base.py`

 * *Files identical despite different names*

### Comparing `midori-0.1.0/midori/plugins/example_plugins.py` & `midori-1.0.0/midori/plugins/example_plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
     def action(self) -> str:
         return f"cd {self.subject_path} && skaffold delete && skaffold run"
 
 
 class EnergyDataCollection(PluginHelper):
     def action(self) -> None:
         energy_collector: PodHelper = PodHelper(
-            self.ssh, "prometheus-server", "default"
+            self._ssh, "prometheus-server", "default"
         )
         energy_node_save_path = f"~/research/results/{self.treatment}/energy.json"
         energy_collector.execute_query_in_pod(
             node_saving_path=energy_node_save_path,
             query_cmd=energy_collector.construct_query_cmd(),
         )
 
 
 class LoadTestingDataCollection(PluginHelper):
     def action(self) -> None:
         treatment_node_save_path = f"~/research/results/{self.treatment}"
-        pft: PodHelper = PodHelper(self.ssh, "loadgenerator", "default")
+        pft: PodHelper = PodHelper(self._ssh, "loadgenerator", "default")
         pft.transfer_file_from_pod("/loadgen", treatment_node_save_path)
```

### Comparing `midori-0.1.0/midori/plugins/helpers.py` & `midori-1.0.0/midori/plugins/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     def __init__(
         self,
         ssh: paramiko.SSHClient,
         subject_path: str,
         treatment: str,
         previous_output: Optional[str] = None,
     ):
-        self.ssh = ssh
+        self._ssh = ssh
         self.subject_path = subject_path
         self.previous_output = previous_output
         self.treatment = treatment
 
     @final
     def execute(self) -> Optional[str]:
         command = self.action()
         if command:
-            return execute(command, self.ssh)
+            return execute(command, self._ssh)
         return None
 
     def action(self) -> Optional[str]:
         raise NotImplementedError("Subclasses must implement this method")
 
 
 class PodHelper:
```

