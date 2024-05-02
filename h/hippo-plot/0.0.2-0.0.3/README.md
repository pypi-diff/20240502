# Comparing `tmp/hippo_plot-0.0.2.tar.gz` & `tmp/hippo_plot-0.0.3.tar.gz`

## Comparing `hippo_plot-0.0.2.tar` & `hippo_plot-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/hipplot/__init__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/hipplot/draw.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/hipplot/io.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/hipplot/prep.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/.gitignore
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/README.md
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/hippo-plot/__init__.py
+-rwxr-xr-x   0        0        0     1782 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/hippo-plot/cli.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/hippo-plot/draw.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/hippo-plot/io.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/hippo-plot/prep.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/.gitignore
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/README.md
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/PKG-INFO
```

### Comparing `hippo_plot-0.0.2/.gitignore` & `hippo_plot-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hippo_plot-0.0.2/pyproject.toml` & `hippo_plot-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "hippo-plot"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Max Winokan", email = "max@winokan.com" },
 ]
 description = "Lightweight companion to HIPPO for creating interactive data visualisations of HIPPO outputs"
 readme = "README.md"
 requires-python = ">=3.10"
 requires = []
@@ -17,16 +17,18 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "mpytools >= 0.0.10",
     "plotly",
     "pandas",
     "dash",
-    "molparse",
+    "rdkit",
 ]
 [project.urls]
 "Homepage" = "https://hippo.winokan.com"
 "Bug Tracker" = "https://github.com/mwinokan/HIPPO_plot/issues"
 [tool.hatch.build]
 include = [
-    "hipplot/*.py"
+    "hippo-plot/*.py"
 ]
+[project.scripts]
+hippo-plot = "hippo-plot.cli:main"
```

### Comparing `hippo_plot-0.0.2/PKG-INFO` & `hippo_plot-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.3
 Name: hippo-plot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Lightweight companion to HIPPO for creating interactive data visualisations of HIPPO outputs
 Project-URL: Homepage, https://hippo.winokan.com
 Project-URL: Bug Tracker, https://github.com/mwinokan/HIPPO_plot/issues
 Author-email: Max Winokan <max@winokan.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: dash
-Requires-Dist: molparse
 Requires-Dist: mpytools>=0.0.10
 Requires-Dist: pandas
 Requires-Dist: plotly
+Requires-Dist: rdkit
 Description-Content-Type: text/markdown
 
 # HIPPO_plot
 Lightweight companion to HIPPO for creating interactive data visualisations of HIPPO outputs
```

