# Comparing `tmp/hippo_plot-0.0.3.tar.gz` & `tmp/hippo_plot-0.0.4.tar.gz`

## Comparing `hippo_plot-0.0.3.tar` & `hippo_plot-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,4 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/hippo-plot/__init__.py
--rwxr-xr-x   0        0        0     1782 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/hippo-plot/cli.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/hippo-plot/draw.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/hippo-plot/io.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/hippo-plot/prep.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/.gitignore
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/README.md
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 hippo_plot-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hippo_plot-0.0.4/.gitignore
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hippo_plot-0.0.4/README.md
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 hippo_plot-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 hippo_plot-0.0.4/PKG-INFO
```

### Comparing `hippo_plot-0.0.3/.gitignore` & `hippo_plot-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hippo_plot-0.0.3/pyproject.toml` & `hippo_plot-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
-name = "hippo-plot"
-version = "0.0.3"
+name = "hippo_plot"
+version = "0.0.4"
 authors = [
     { name = "Max Winokan", email = "max@winokan.com" },
 ]
 description = "Lightweight companion to HIPPO for creating interactive data visualisations of HIPPO outputs"
 readme = "README.md"
 requires-python = ">=3.10"
 requires = []
@@ -24,11 +24,11 @@
     "rdkit",
 ]
 [project.urls]
 "Homepage" = "https://hippo.winokan.com"
 "Bug Tracker" = "https://github.com/mwinokan/HIPPO_plot/issues"
 [tool.hatch.build]
 include = [
-    "hippo-plot/*.py"
+    "hippo_plot/*.py"
 ]
 [project.scripts]
-hippo-plot = "hippo-plot.cli:main"
+hippo_plot = "hippo_plot.cli:main"
```

### Comparing `hippo_plot-0.0.3/PKG-INFO` & `hippo_plot-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
-Name: hippo-plot
-Version: 0.0.3
+Name: hippo_plot
+Version: 0.0.4
 Summary: Lightweight companion to HIPPO for creating interactive data visualisations of HIPPO outputs
 Project-URL: Homepage, https://hippo.winokan.com
 Project-URL: Bug Tracker, https://github.com/mwinokan/HIPPO_plot/issues
 Author-email: Max Winokan <max@winokan.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

