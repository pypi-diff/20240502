# Comparing `tmp/deadline_cloud_for_cinema_4d-0.3.0.tar.gz` & `tmp/deadline_cloud_for_cinema_4d-0.3.1.tar.gz`

## Comparing `deadline_cloud_for_cinema_4d-0.3.0.tar` & `deadline_cloud_for_cinema_4d-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/_version.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/_version.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/Cinema4DAdaptor.json
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__init__.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__main__.py
--rw-r--r--   0        0        0    17059 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/adaptor.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DClient/__init__.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_client.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_handler.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DClient/plugin/DeadlineCloudClient.pyp
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/_version.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/adaptor_cinema4d_job_template.yaml
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/adaptor_override_environment.yaml
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/assets.py
--rw-r--r--   0        0        0    14924 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/cinema4d_render_submitter.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/data_classes.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/default_cinema4d_job_template.yaml
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/scene.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/style.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/takes.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/ui/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/ui/components/__init__.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/ui/components/scene_settings_tab.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/NOTICE
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/README.md
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/hatch.toml
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/_version.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/_version.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/Cinema4DAdaptor.json
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__init__.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__main__.py
+-rw-r--r--   0        0        0    17059 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/adaptor.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/__init__.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_client.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_handler.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/plugin/DeadlineCloudClient.pyp
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/_version.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/adaptor_cinema4d_job_template.yaml
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/assets.py
+-rw-r--r--   0        0        0    14924 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/cinema4d_render_submitter.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/data_classes.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/default_cinema4d_job_template.yaml
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/scene.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/style.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/takes.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/ui/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/ui/components/__init__.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/ui/components/scene_settings_tab.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/NOTICE
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/README.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/hatch.toml
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/PKG-INFO
```

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__main__.py` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/adaptor.py` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_client.py` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_handler.py` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_adaptor/Cinema4DClient/plugin/DeadlineCloudClient.pyp` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/plugin/DeadlineCloudClient.pyp`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/adaptor_cinema4d_job_template.yaml` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/adaptor_cinema4d_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/adaptor_override_environment.yaml` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/assets.py` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/assets.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/cinema4d_render_submitter.py` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/cinema4d_render_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/data_classes.py` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/data_classes.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/default_cinema4d_job_template.yaml` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/default_cinema4d_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/scene.py` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/scene.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/style.py` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/style.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/src/deadline/cinema4d_submitter/ui/components/scene_settings_tab.py` & `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/ui/components/scene_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/LICENSE` & `deadline_cloud_for_cinema_4d-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/README.md` & `deadline_cloud_for_cinema_4d-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/hatch.toml` & `deadline_cloud_for_cinema_4d-0.3.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/pyproject.toml` & `deadline_cloud_for_cinema_4d-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

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
 Homepage = "https://github.com/aws-deadline/deadline-cloud-for-cinema-4d"
 Source = "https://github.com/aws-deadline/deadline-cloud-for-cinimema-4d"
```

### Comparing `deadline_cloud_for_cinema_4d-0.3.0/PKG-INFO` & `deadline_cloud_for_cinema_4d-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-cinema-4d
-Version: 0.3.0
+Version: 0.3.1
 Summary: AWS Deadline Cloud for Cinema 4D
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-cinema-4d
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-cinimema-4d
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
 
 # AWS Deadline Cloud for Cinema 4D
 
 [![pypi](https://img.shields.io/pypi/v/deadline-cloud-for-cinema-4d.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-cinema-4d)
 [![python](https://img.shields.io/pypi/pyversions/deadline-cloud-for-cinema-4d.svg?style=flat)](https://pypi.python.org/pypi/deadline-cloud-for-cinema-4d)
```

