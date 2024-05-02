# Comparing `tmp/las_geoh5-0.2.0rc1.tar.gz` & `tmp/las_geoh5-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "las_geoh5-0.2.0rc1.tar", max compression
+gzip compressed data, was "las_geoh5-0.2.0rc2.tar", max compression
```

## Comparing `las_geoh5-0.2.0rc1.tar` & `las_geoh5-0.2.0rc2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      702 2024-04-27 20:37:43.194475 las_geoh5-0.2.0rc1/las_geoh5/__init__.py
--rw-r--r--   0        0        0      240 2024-04-23 21:10:39.081155 las_geoh5-0.2.0rc1/las_geoh5/export_files/__init__.py
--rw-r--r--   0        0        0     1734 2024-04-23 21:10:39.082255 las_geoh5-0.2.0rc1/las_geoh5/export_files/driver.py
--rw-r--r--   0        0        0     1264 2024-04-23 21:11:17.349111 las_geoh5-0.2.0rc1/las_geoh5/export_files/uijson.py
--rw-r--r--   0        0        0     6748 2024-04-23 21:11:17.349111 las_geoh5-0.2.0rc1/las_geoh5/export_las.py
--rw-r--r--   0        0        0      240 2024-04-23 21:10:39.083315 las_geoh5-0.2.0rc1/las_geoh5/import_directories/__init__.py
--rw-r--r--   0        0        0     2104 2024-04-23 21:10:39.083315 las_geoh5-0.2.0rc1/las_geoh5/import_directories/driver.py
--rw-r--r--   0        0        0     1057 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc1/las_geoh5/import_directories/uijson.py
--rw-r--r--   0        0        0      240 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc1/las_geoh5/import_files/__init__.py
--rw-r--r--   0        0        0     4632 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc1/las_geoh5/import_files/driver.py
--rw-r--r--   0        0        0     1468 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc1/las_geoh5/import_files/params.py
--rw-r--r--   0        0        0     3080 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc1/las_geoh5/import_files/uijson.py
--rw-r--r--   0        0        0    13319 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc1/las_geoh5/import_las.py
--rw-r--r--   0        0        0      122 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc1/las_geoh5/uijson/__init__.py
--rw-r--r--   0        0        0     2119 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc1/las_geoh5/uijson/write_uijson.py
--rw-r--r--   0        0        0      122 2024-04-23 21:10:39.087480 las_geoh5-0.2.0rc1/las_geoh5-assets/__init__.py
--rw-r--r--   0        0        0     1112 2024-04-23 21:11:17.350225 las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/export_las_files.ui.json
--rw-r--r--   0        0        0      974 2024-04-23 21:10:39.088503 las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/import_las_directories.ui.json
--rw-r--r--   0        0        0     2656 2024-04-23 21:11:17.350225 las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/import_las_files.ui.json
--rw-r--r--   0        0        0     1093 2024-04-23 21:10:39.080154 las_geoh5-0.2.0rc1/LICENSE.txt
--rw-r--r--   0        0        0     2591 2024-04-27 20:40:58.445160 las_geoh5-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4992 2024-04-26 06:14:29.001844 las_geoh5-0.2.0rc1/README.rst
--rw-r--r--   0        0        0     6011 1970-01-01 00:00:00.000000 las_geoh5-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      702 2024-05-02 20:02:14.201504 las_geoh5-0.2.0rc2/las_geoh5/__init__.py
+-rw-r--r--   0        0        0      240 2024-04-23 21:10:39.081155 las_geoh5-0.2.0rc2/las_geoh5/export_files/__init__.py
+-rw-r--r--   0        0        0     1734 2024-04-23 21:10:39.082255 las_geoh5-0.2.0rc2/las_geoh5/export_files/driver.py
+-rw-r--r--   0        0        0     1264 2024-04-23 21:11:17.349111 las_geoh5-0.2.0rc2/las_geoh5/export_files/uijson.py
+-rw-r--r--   0        0        0     6748 2024-04-23 21:11:17.349111 las_geoh5-0.2.0rc2/las_geoh5/export_las.py
+-rw-r--r--   0        0        0      240 2024-04-23 21:10:39.083315 las_geoh5-0.2.0rc2/las_geoh5/import_directories/__init__.py
+-rw-r--r--   0        0        0     2104 2024-04-23 21:10:39.083315 las_geoh5-0.2.0rc2/las_geoh5/import_directories/driver.py
+-rw-r--r--   0        0        0     1057 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc2/las_geoh5/import_directories/uijson.py
+-rw-r--r--   0        0        0      240 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc2/las_geoh5/import_files/__init__.py
+-rw-r--r--   0        0        0     4632 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc2/las_geoh5/import_files/driver.py
+-rw-r--r--   0        0        0     1468 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc2/las_geoh5/import_files/params.py
+-rw-r--r--   0        0        0     3080 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc2/las_geoh5/import_files/uijson.py
+-rw-r--r--   0        0        0    13319 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc2/las_geoh5/import_las.py
+-rw-r--r--   0        0        0      122 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc2/las_geoh5/uijson/__init__.py
+-rw-r--r--   0        0        0     2119 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc2/las_geoh5/uijson/write_uijson.py
+-rw-r--r--   0        0        0      122 2024-04-23 21:10:39.087480 las_geoh5-0.2.0rc2/las_geoh5-assets/__init__.py
+-rw-r--r--   0        0        0     1114 2024-05-02 03:50:51.043275 las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/export_las_files.ui.json
+-rw-r--r--   0        0        0      976 2024-05-02 03:50:51.044307 las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/import_las_directories.ui.json
+-rw-r--r--   0        0        0     2656 2024-05-02 03:50:51.045439 las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/import_las_files.ui.json
+-rw-r--r--   0        0        0     1093 2024-04-27 22:59:02.102762 las_geoh5-0.2.0rc2/LICENSE
+-rw-r--r--   0        0        0     2742 2024-05-02 20:02:14.185918 las_geoh5-0.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4992 2024-04-26 06:14:29.001844 las_geoh5-0.2.0rc2/README.rst
+-rw-r--r--   0        0        0     6327 1970-01-01 00:00:00.000000 las_geoh5-0.2.0rc2/PKG-INFO
```

### Comparing `las_geoh5-0.2.0rc1/las_geoh5/__init__.py` & `las_geoh5-0.2.0rc2/las_geoh5/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # flake8: noqa
 
 from __future__ import annotations
 
 from pathlib import Path
 
-__version__ = "0.2.0-rc.1"
+__version__ = "0.2.0-rc.2"
 
 
 def assets_path() -> Path:
     """Return the path to the assets folder."""
 
     parent = Path(__file__).parent
     folder_name = f"{parent.name}-assets"
```

### Comparing `las_geoh5-0.2.0rc1/las_geoh5/export_files/driver.py` & `las_geoh5-0.2.0rc2/las_geoh5/export_files/driver.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/las_geoh5/export_files/uijson.py` & `las_geoh5-0.2.0rc2/las_geoh5/export_files/uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/las_geoh5/export_las.py` & `las_geoh5-0.2.0rc2/las_geoh5/export_las.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/las_geoh5/import_directories/driver.py` & `las_geoh5-0.2.0rc2/las_geoh5/import_directories/driver.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/las_geoh5/import_directories/uijson.py` & `las_geoh5-0.2.0rc2/las_geoh5/import_directories/uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/las_geoh5/import_files/driver.py` & `las_geoh5-0.2.0rc2/las_geoh5/import_files/driver.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/las_geoh5/import_files/params.py` & `las_geoh5-0.2.0rc2/las_geoh5/import_files/params.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/las_geoh5/import_files/uijson.py` & `las_geoh5-0.2.0rc2/las_geoh5/import_files/uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/las_geoh5/import_las.py` & `las_geoh5-0.2.0rc2/las_geoh5/import_las.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/las_geoh5/uijson/write_uijson.py` & `las_geoh5-0.2.0rc2/las_geoh5/uijson/write_uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/export_las_files.ui.json` & `las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/export_las_files.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,19 +1,19 @@
 {
     "title": "Drillhole group to LAS files",
-    "geoh5": "",
+    "conda_environment": "las-geoh5",
     "run_command": "las_geoh5.export_files.driver",
+    "geoh5": "",
+    "monitoring_directory": "",
     "run_command_boolean": {
         "value": false,
         "label": "Run python module ",
         "tooltip": "Warning: launches process to run python model on save",
         "main": true
     },
-    "monitoring_directory": "",
-    "conda_environment": "las-geoh5",
     "conda_environment_boolean": false,
     "workspace": "",
     "drillhole_group": {
         "main": true,
         "label": "Drillhole group",
         "value": "",
         "groupType": [
```

### Comparing `las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/import_las_directories.ui.json` & `las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/import_las_directories.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,19 +1,19 @@
 {
     "title": "LAS file directories to Drillhole group",
-    "geoh5": "",
+    "conda_environment": "las-geoh5",
     "run_command": "las_geoh5.import_directories.driver",
+    "geoh5": "",
+    "monitoring_directory": "",
     "run_command_boolean": {
         "value": false,
         "label": "Run python module ",
         "tooltip": "Warning: launches process to run python model on save",
         "main": true
     },
-    "monitoring_directory": "",
-    "conda_environment": "las-geoh5",
     "conda_environment_boolean": false,
     "workspace": "",
     "drillhole_group": {
         "main": true,
         "label": "Drillhole group",
         "value": "",
         "groupType": [
```

### Comparing `las_geoh5-0.2.0rc1/las_geoh5-assets/uijson/import_las_files.ui.json` & `las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/import_las_files.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,19 +1,19 @@
 {
     "title": "LAS files to Drillhole group",
-    "geoh5": "",
+    "conda_environment": "las-geoh5",
     "run_command": "las_geoh5.import_files.driver",
+    "geoh5": "",
+    "monitoring_directory": "",
     "run_command_boolean": {
         "value": false,
         "label": "Run python module",
         "main": true,
         "tooltip": "Warning: launches process to run python model on save"
     },
-    "monitoring_directory": "",
-    "conda_environment": "las-geoh5",
     "conda_environment_boolean": false,
     "workspace": "",
     "drillhole_group": {
         "main": true,
         "label": "Drillhole group",
         "value": "",
         "groupType": [
```

### Comparing `las_geoh5-0.2.0rc1/LICENSE.txt` & `las_geoh5-0.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/pyproject.toml` & `las_geoh5-0.2.0rc2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [tool.poetry]
 name = "las-geoh5"
-version = "0.2.0-rc.1"
+version = "0.2.0-rc.2"
 description = "Las/Geoh5 conversion"
 license = "MIT"
 readme = "README.rst"
-homepage = "https://mirageoscience.com"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
+maintainers = ["Benjamin Kary <benjamink@mirageoscience.com>"]
 keywords = ["geology", "geophysics", "earth sciences", "io", "data", "interoperability"]
+repository = "https://github.com/MiraGeoscience/las-geoh5"
+documentation  = "https://mirageoscience-las-geoh5.readthedocs-hosted.com/"
+homepage = "https://www.mirageoscience.com/mining-industry-software/python-integration/"
 
 packages = [
     { include = "las_geoh5" },
     { include = "las_geoh5-assets" },
 ]
 
 include = [
@@ -35,14 +38,15 @@
     "Natural Language :: English",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10, <3.11"
 
 lasio = "~0.31"
+numpy = "~1.23.5"  # also in geoh5py
 pydantic = "~2.5.2"
 tqdm = "^4.66.1"
 
 ## dependencies from Git repositories
 #------------------------------------
 geoh5py = {version ="~0.9.0rc1", allow-prereleases = true}
 #geoh5py = {git = "https://github.com/MiraGeoscience/geoh5py.git", branch = "release/0.9.0"}
@@ -56,34 +60,30 @@
 pytest-cov = "*"
 tomli = "*"
 sphinx = "*"
 sphinx-autodoc-typehints = "*"
 sphinx-rtd-theme = "*"
 
 [tool.isort]
-# settings for compatibility between ``isort`` and ``black`` formatting
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-line_length = 88
+profile = "black"
 
 [tool.black]
 # defaults are just fine
 
 [tool.mypy]
 warn_unused_configs = true
 ignore_missing_imports = true
 scripts_are_modules = true
 show_error_context = true
 show_column_numbers = true
 check_untyped_defs = true
 
 plugins = [
-    "pydantic.mypy"
+    "numpy.typing.mypy_plugin",
+    "pydantic.mypy",
 ]
 
 [tool.coverage.run]
 branch = true
 source = ["las_geoh5"]
 omit = []
```

### Comparing `las_geoh5-0.2.0rc1/README.rst` & `las_geoh5-0.2.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc1/PKG-INFO` & `las_geoh5-0.2.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: las-geoh5
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: Las/Geoh5 conversion
-Home-page: https://mirageoscience.com
+Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Keywords: geology,geophysics,earth sciences,io,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
+Maintainer: Benjamin Kary
+Maintainer-email: benjamink@mirageoscience.com
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -20,16 +22,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: lasio (>=0.31,<0.32)
+Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: pydantic (>=2.5.2,<2.6.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
+Project-URL: Documentation, https://mirageoscience-las-geoh5.readthedocs-hosted.com/
+Project-URL: Repository, https://github.com/MiraGeoscience/las-geoh5
 Description-Content-Type: text/x-rst
 
 |coverage| |maintainability| |precommit_ci| |docs| |style| |version| |status| |pyversions|
 
 
 .. |docs| image:: https://readthedocs.com/projects/mirageoscience-las-geoh5/badge/?version=latest
     :alt: Documentation Status
```

