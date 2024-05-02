# Comparing `tmp/hippo_plot-0.0.1.tar.gz` & `tmp/hippo_plot-0.0.2.tar.gz`

## Comparing `hippo_plot-0.0.1.tar` & `hippo_plot-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hippo_plot-0.0.1/hipplot/__init__.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hippo_plot-0.0.1/hipplot/draw.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hippo_plot-0.0.1/hipplot/io.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 hippo_plot-0.0.1/hipplot/prep.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hippo_plot-0.0.1/.gitignore
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hippo_plot-0.0.1/README.md
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 hippo_plot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 hippo_plot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/hipplot/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/hipplot/draw.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/hipplot/io.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/hipplot/prep.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/.gitignore
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/README.md
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 hippo_plot-0.0.2/PKG-INFO
```

### Comparing `hippo_plot-0.0.1/.gitignore` & `hippo_plot-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hippo_plot-0.0.1/pyproject.toml` & `hippo_plot-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "hippo-plot"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Max Winokan", email = "max@winokan.com" },
 ]
 description = "Lightweight companion to HIPPO for creating interactive data visualisations of HIPPO outputs"
 readme = "README.md"
 requires-python = ">=3.10"
 requires = []
```

### Comparing `hippo_plot-0.0.1/PKG-INFO` & `hippo_plot-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hippo-plot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Lightweight companion to HIPPO for creating interactive data visualisations of HIPPO outputs
 Project-URL: Homepage, https://hippo.winokan.com
 Project-URL: Bug Tracker, https://github.com/mwinokan/HIPPO_plot/issues
 Author-email: Max Winokan <max@winokan.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

