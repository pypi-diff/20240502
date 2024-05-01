# Comparing `tmp/deadline_cloud_for_nuke-0.18.1.tar.gz` & `tmp/deadline_cloud_for_nuke-0.18.2.tar.gz`

## Comparing `deadline_cloud_for_nuke-0.18.1.tar` & `deadline_cloud_for_nuke-0.18.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/_version.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/hatch_custom_hook.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/menu.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/_version.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeAdaptor/NukeAdaptor.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeAdaptor/__init__.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeAdaptor/__main__.py
--rw-r--r--   0        0        0    19258 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeAdaptor/adaptor.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeAdaptor/py.typed
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeClient/__init__.py
--rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeClient/nuke_client.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeClient/nuke_handler.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeClient/py.typed
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/__init__.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/_logging.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/_version.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/adaptor_override_environment.yaml
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/assets.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/data_classes.py
--rw-r--r--   0        0        0    14625 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/deadline_submitter_for_nuke.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/default_nuke_job_template.yaml
--rw-r--r--   0        0        0    13097 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/job_bundle_output_test_runner.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/py.typed
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/ui/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/ui/components/__init__.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/ui/components/scene_settings_tab.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_util/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_util/_version.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_util/ocio.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/NOTICE
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/README.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/hatch.toml
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/pyproject.toml
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.1/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/_version.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/hatch_custom_hook.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/menu.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/_version.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/NukeAdaptor.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/__init__.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/__main__.py
+-rw-r--r--   0        0        0    19258 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/adaptor.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/py.typed
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/__init__.py
+-rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/nuke_client.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/nuke_handler.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/py.typed
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/__init__.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/_logging.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/_version.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/assets.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/data_classes.py
+-rw-r--r--   0        0        0    14467 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/deadline_submitter_for_nuke.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/default_nuke_job_template.yaml
+-rw-r--r--   0        0        0    13097 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/job_bundle_output_test_runner.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/py.typed
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/ui/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/ui/components/__init__.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/ui/components/scene_settings_tab.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_util/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_util/_version.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_util/ocio.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/NOTICE
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/README.md
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/hatch.toml
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/pyproject.toml
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 deadline_cloud_for_nuke-0.18.2/PKG-INFO
```

### Comparing `deadline_cloud_for_nuke-0.18.1/hatch_custom_hook.py` & `deadline_cloud_for_nuke-0.18.2/hatch_custom_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/menu.py` & `deadline_cloud_for_nuke-0.18.2/src/menu.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeAdaptor/__main__.py` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeAdaptor/adaptor.py` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeAdaptor/schemas/init_data.schema.json` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeAdaptor/schemas/init_data.schema.json`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeClient/nuke_client.py` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/nuke_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_adaptor/NukeClient/nuke_handler.py` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_adaptor/NukeClient/nuke_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/_logging.py` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/_logging.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/adaptor_override_environment.yaml` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/assets.py` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/assets.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/data_classes.py` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/data_classes.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/deadline_submitter_for_nuke.py` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/deadline_submitter_for_nuke.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,42 +116,38 @@
         job_template["parameterDefinitions"].extend(override_environment["parameterDefinitions"])
 
         # Add the environment to the end of the template's job environments
         if "jobEnvironments" not in job_template:
             job_template["jobEnvironments"] = []
         job_template["jobEnvironments"].append(override_environment["environment"])
 
-        # Determine whether this is a movie render. If it is, we want to ensure that the entire Nuke
-        # evaluation is placed on one task.
-        write_node, _ = _get_write_node(settings)
-        movie_render = "file_type" in write_node.knobs() and write_node["file_type"].value() in [
-            "mov",
-            "mxf",
-        ]
-        if movie_render:
-            frame_list = (
-                settings.frame_list
-                if settings.override_frame_range
-                else str(write_node.frameRange())
+    # Determine whether this is a movie render. If it is, we want to ensure that the entire Nuke
+    # evaluation is placed on one task.
+    write_node, _ = _get_write_node(settings)
+    movie_render = "file_type" in write_node.knobs() and write_node["file_type"].value() in [
+        "mov",
+        "mxf",
+    ]
+    if movie_render:
+        frame_list = (
+            settings.frame_list if settings.override_frame_range else str(write_node.frameRange())
+        )
+        match = re.match(r"(\d+)-(\d+)", frame_list)
+        if not match:
+            raise DeadlineOperationError(
+                f"Invalid frame range {frame_list} for evaluating a MOV render. Frame range must follow the format 'startFrame - endFrame'"
             )
-            match = re.match(r"(\d+)-(\d+)", frame_list)
-            if not match:
-                raise DeadlineOperationError(
-                    f"Invalid frame range {frame_list} for evaluating a MOV render. Frame range must follow the format 'startFrame - endFrame'"
-                )
-
-            start_frame = match.group(1)
-            end_frame = match.group(2)
-
-            # Remove the Frame parameter space and update the script data with the desired start and end frame
-            for step in job_template["steps"]:
-                del step["parameterSpace"]
-                step["script"]["embeddedFiles"][0][
-                    "data"
-                ] = f"frameRange: {start_frame}-{end_frame}\n"
+
+        start_frame = match.group(1)
+        end_frame = match.group(2)
+
+        # Remove the Frame parameter space and update the script data with the desired start and end frame
+        for step in job_template["steps"]:
+            del step["parameterSpace"]
+            step["script"]["embeddedFiles"][0]["data"] = f"frameRange: {start_frame}-{end_frame}\n"
 
     return job_template
 
 
 def _get_parameter_values(
     settings: RenderSubmitterUISettings,
     queue_parameters: list[dict[str, Any]],
```

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/default_nuke_job_template.yaml` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/default_nuke_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/job_bundle_output_test_runner.py` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/job_bundle_output_test_runner.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_submitter/ui/components/scene_settings_tab.py` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_submitter/ui/components/scene_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/src/deadline/nuke_util/ocio.py` & `deadline_cloud_for_nuke-0.18.2/src/deadline/nuke_util/ocio.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/LICENSE` & `deadline_cloud_for_nuke-0.18.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/README.md` & `deadline_cloud_for_nuke-0.18.2/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/hatch.toml` & `deadline_cloud_for_nuke-0.18.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_nuke-0.18.1/pyproject.toml` & `deadline_cloud_for_nuke-0.18.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   "Operating System :: MacOS",
   "License :: OSI Approved :: Apache Software License",
   "Intended Audience :: Developers",
   "Intended Audience :: End Users/Desktop",
 ]
 
 dependencies = [
-    "deadline == 0.47.*",
+    "deadline == 0.48.*",
     "openjd-adaptor-runtime == 0.7.*",
 ]
 
 [project.urls]
 Homepage = "https://github.com/aws-deadline/deadline-cloud-for-nuke"
 Source = "https://github.com/aws-deadline/deadline-cloud-for-nuke"
```

### Comparing `deadline_cloud_for_nuke-0.18.1/PKG-INFO` & `deadline_cloud_for_nuke-0.18.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-nuke
-Version: 0.18.1
+Version: 0.18.2
 Summary: The submitter and adaptor to enable Nuke support for AWS Deadline Cloud
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-nuke
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-nuke
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
-Requires-Dist: deadline==0.47.*
+Requires-Dist: deadline==0.48.*
 Requires-Dist: openjd-adaptor-runtime==0.7.*
 Description-Content-Type: text/markdown
 
 [![pypi](https://img.shields.io/pypi/v/deadline-cloud-for-nuke.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-nuke)
 [![python](https://img.shields.io/pypi/pyversions/deadline-cloud-for-nuke.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-nuke)
 [![license](https://img.shields.io/pypi/l/deadline-cloud-for-nuke.svg?style=flat)](https://github.com/aws-deadline/deadline-cloud-for-nuke/blob/mainline/LICENSE)
```

