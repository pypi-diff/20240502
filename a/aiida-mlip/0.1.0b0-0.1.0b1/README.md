# Comparing `tmp/aiida_mlip-0.1.0b0.tar.gz` & `tmp/aiida_mlip-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_mlip-0.1.0b0.tar", max compression
+gzip compressed data, was "aiida_mlip-0.1.0b1.tar", max compression
```

## Comparing `aiida_mlip-0.1.0b0.tar` & `aiida_mlip-0.1.0b1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1533 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/LICENSE
--rw-r--r--   0        0        0     8039 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/README.md
--rw-r--r--   0        0        0       87 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/__init__.py
--rw-r--r--   0        0        0       34 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/calculations/__init__.py
--rw-r--r--   0        0        0     9272 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/calculations/base.py
--rw-r--r--   0        0        0     4497 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/calculations/geomopt.py
--rw-r--r--   0        0        0     4409 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/calculations/md.py
--rw-r--r--   0        0        0     3496 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/calculations/singlepoint.py
--rw-r--r--   0        0        0       43 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/data/__init__.py
--rw-r--r--   0        0        0     4349 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/data/config.py
--rw-r--r--   0        0        0     8231 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/data/model.py
--rw-r--r--   0        0        0       40 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/helpers/__init__.py
--rw-r--r--   0        0        0     2826 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/helpers/converters.py
--rw-r--r--   0        0        0     2650 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/helpers/help_load.py
--rw-r--r--   0        0        0       34 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/parsers/__init__.py
--rw-r--r--   0        0        0     2332 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/parsers/base_parser.py
--rw-r--r--   0        0        0     3643 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/parsers/md_parser.py
--rw-r--r--   0        0        0     2563 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/parsers/opt_parser.py
--rw-r--r--   0        0        0     2891 2024-04-28 20:47:33.737152 aiida_mlip-0.1.0b0/aiida_mlip/parsers/sp_parser.py
--rw-r--r--   0        0        0     3344 2024-04-28 20:47:33.741153 aiida_mlip-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0     9132 1970-01-01 00:00:00.000000 aiida_mlip-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/LICENSE
+-rw-r--r--   0        0        0     8039 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/README.md
+-rw-r--r--   0        0        0       87 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/aiida_mlip/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/aiida_mlip/calculations/__init__.py
+-rw-r--r--   0        0        0     9272 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/aiida_mlip/calculations/base.py
+-rw-r--r--   0        0        0     4497 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/aiida_mlip/calculations/geomopt.py
+-rw-r--r--   0        0        0     4409 2024-05-02 17:21:52.820970 aiida_mlip-0.1.0b1/aiida_mlip/calculations/md.py
+-rw-r--r--   0        0        0     3496 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/calculations/singlepoint.py
+-rw-r--r--   0        0        0       43 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/data/__init__.py
+-rw-r--r--   0        0        0     4349 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/data/config.py
+-rw-r--r--   0        0        0     8231 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/data/model.py
+-rw-r--r--   0        0        0       40 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/helpers/__init__.py
+-rw-r--r--   0        0        0     2826 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/helpers/converters.py
+-rw-r--r--   0        0        0     2650 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/helpers/help_load.py
+-rw-r--r--   0        0        0       34 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/parsers/__init__.py
+-rw-r--r--   0        0        0     2409 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/parsers/base_parser.py
+-rw-r--r--   0        0        0     3719 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/parsers/md_parser.py
+-rw-r--r--   0        0        0     2583 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/parsers/opt_parser.py
+-rw-r--r--   0        0        0     2912 2024-05-02 17:21:52.824970 aiida_mlip-0.1.0b1/aiida_mlip/parsers/sp_parser.py
+-rw-r--r--   0        0        0     3344 2024-05-02 17:21:52.828970 aiida_mlip-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     9132 1970-01-01 00:00:00.000000 aiida_mlip-0.1.0b1/PKG-INFO
```

### Comparing `aiida_mlip-0.1.0b0/LICENSE` & `aiida_mlip-0.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b0/README.md` & `aiida_mlip-0.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/calculations/base.py` & `aiida_mlip-0.1.0b1/aiida_mlip/calculations/base.py`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/calculations/geomopt.py` & `aiida_mlip-0.1.0b1/aiida_mlip/calculations/geomopt.py`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/calculations/md.py` & `aiida_mlip-0.1.0b1/aiida_mlip/calculations/md.py`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/calculations/singlepoint.py` & `aiida_mlip-0.1.0b1/aiida_mlip/calculations/singlepoint.py`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/data/config.py` & `aiida_mlip-0.1.0b1/aiida_mlip/data/config.py`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/data/model.py` & `aiida_mlip-0.1.0b1/aiida_mlip/data/model.py`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/helpers/converters.py` & `aiida_mlip-0.1.0b1/aiida_mlip/helpers/converters.py`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/helpers/help_load.py` & `aiida_mlip-0.1.0b1/aiida_mlip/helpers/help_load.py`

 * *Files identical despite different names*

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/parsers/base_parser.py` & `aiida_mlip-0.1.0b1/aiida_mlip/parsers/base_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,11 +76,13 @@
 
         # Add output file to the outputs
 
         with (
             self.retrieved.open(log_output, "rb") as log,
             self.retrieved.open(output_filename, "rb") as output,
         ):
-            self.out("log_output", SinglefileData(file=log))
-            self.out("std_output", SinglefileData(file=output))
+            self.out("log_output", SinglefileData(file=log, filename=log_output))
+            self.out(
+                "std_output", SinglefileData(file=output, filename=output_filename)
+            )
 
         return ExitCode(0)
```

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/parsers/md_parser.py` & `aiida_mlip-0.1.0b1/aiida_mlip/parsers/md_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,31 +81,31 @@
             return exit_code
 
         md_dictionary = self.node.inputs.md_kwargs.get_dict()
 
         # Process trajectory file saving both the file and trajectory as aiida data
         traj_filepath = md_dictionary.get("traj-file", MD.DEFAULT_TRAJ_FILE)
         with self.retrieved.open(traj_filepath, "rb") as handle:
-            self.out("traj_file", SinglefileData(file=handle))
+            self.out("traj_file", SinglefileData(file=handle, filename=traj_filepath))
         final_str, traj_output = xyz_to_aiida_traj(
             Path(self.node.get_remote_workdir(), traj_filepath)
         )
         self.out("traj_output", traj_output)
         self.out("final_structure", final_str)
 
         # Process stats file as singlefiledata
         stats_filepath = md_dictionary.get("stats-file", MD.DEFAULT_STATS_FILE)
         with self.retrieved.open(stats_filepath, "rb") as handle:
-            self.out("stats_file", SinglefileData(file=handle))
+            self.out("stats_file", SinglefileData(file=handle, filename=stats_filepath))
 
         # Process summary as both singlefiledata and results dictionary
         summary_filepath = md_dictionary.get("summary", MD.DEFAULT_SUMMARY_FILE)
         print(self.node.get_remote_workdir(), summary_filepath)
         with self.retrieved.open(summary_filepath, "rb") as handle:
-            self.out("summary", SinglefileData(file=handle))
+            self.out("summary", SinglefileData(file=handle, filename=summary_filepath))
 
         with self.retrieved.open(summary_filepath, "r") as handle:
             try:
                 res_dict = yaml.safe_load(handle.read())
             except yaml.YAMLError as exc:
                 print("Error loading YAML:", exc)
             if res_dict is None:
```

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/parsers/opt_parser.py` & `aiida_mlip-0.1.0b1/aiida_mlip/parsers/opt_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         exit_code = super().parse(**kwargs)
 
         if exit_code == ExitCode(0):
             traj_file = (self.node.inputs.traj).value
 
             # Parse the trajectory file and save it as `SingleFileData`
             with self.retrieved.open(traj_file, "rb") as handle:
-                self.out("traj_file", SinglefileData(file=handle))
+                self.out("traj_file", SinglefileData(file=handle, filename=traj_file))
             # Parse trajectory and save it as `TrajectoryData`
             opt, traj_output = xyz_to_aiida_traj(
                 Path(self.node.get_remote_workdir(), traj_file)
             )
             self.out("traj_output", traj_output)
 
             # Parse the final structure of the trajectory to obtain the opt structure
```

### Comparing `aiida_mlip-0.1.0b0/aiida_mlip/parsers/sp_parser.py` & `aiida_mlip-0.1.0b1/aiida_mlip/parsers/sp_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             )
             return self.exit_codes.ERROR_MISSING_OUTPUT_FILES
 
         # Add output file to the outputs
         self.logger.info(f"Parsing '{xyz_output}'")
 
         with self.retrieved.open(xyz_output, "rb") as handle:
-            self.out("xyz_output", SinglefileData(file=handle))
+            self.out("xyz_output", SinglefileData(file=handle, filename=xyz_output))
 
         content = read(Path(self.node.get_remote_workdir(), xyz_output))
         results = convert_numpy(content.todict())
         results_node = Dict(results)
         self.out("results_dict", results_node)
 
         return ExitCode(0)
```

### Comparing `aiida_mlip-0.1.0b0/pyproject.toml` & `aiida_mlip-0.1.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiida-mlip"
-version = "0.1.0b0"
+version = "0.1.0b1"
 description = "machine learning interatomic potentials aiida plugin"
 authors = [
     "Federica Zanca",
     "Elliott Kasoar",
     "Jacob Wilkins",
     "Alin M. Elena",
 ]
```

### Comparing `aiida_mlip-0.1.0b0/PKG-INFO` & `aiida_mlip-0.1.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-mlip
-Version: 0.1.0b0
+Version: 0.1.0b1
 Summary: machine learning interatomic potentials aiida plugin
 Home-page: https://github.com/stfc/aiida-mlip/
 Keywords: aiida,plugin
 Author: Federica Zanca
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AiiDA
```

