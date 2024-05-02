# Comparing `tmp/cas-tools-0.0.1.dev8.tar.gz` & `tmp/cas-tools-0.0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cas-tools-0.0.1.dev8.tar", last modified: Mon Dec 11 15:07:40 2023, max compression
+gzip compressed data, was "cas-tools-0.0.1.dev9.tar", last modified: Mon Dec 11 15:35:15 2023, max compression
```

## Comparing `cas-tools-0.0.1.dev8.tar` & `cas-tools-0.0.1.dev9.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:07:40.533678 cas-tools-0.0.1.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-12-11 15:07:40.533678 cas-tools-0.0.1.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 15:07:40.533678 cas-tools-0.0.1.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:07:40.529678 cas-tools-0.0.1.dev8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:07:40.529678 cas-tools-0.0.1.dev8/src/cas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:07:40.529678 cas-tools-0.0.1.dev8/src/cas/accession/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/accession/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/accession/base_accession_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/accession/hash_accession_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/accession/incremental_accession_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/anndata_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/flatten_data_to_anndata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/flatten_data_to_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:07:40.533678 cas-tools-0.0.1.dev8/src/cas/ingest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/ingest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/ingest/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/ingest/ingest_user_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:07:40.533678 cas-tools-0.0.1.dev8/src/cas/matrix_file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/matrix_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/matrix_file/base_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/matrix_file/cxg_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/matrix_file/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2023-12-11 15:07:14.000000 cas-tools-0.0.1.dev8/src/cas/populate_cell_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:07:40.533678 cas-tools-0.0.1.dev8/src/cas_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-12-11 15:07:40.000000 cas-tools-0.0.1.dev8/src/cas_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-12-11 15:07:40.000000 cas-tools-0.0.1.dev8/src/cas_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 15:07:40.000000 cas-tools-0.0.1.dev8/src/cas_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-11 15:07:40.000000 cas-tools-0.0.1.dev8/src/cas_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-11 15:07:40.000000 cas-tools-0.0.1.dev8/src/cas_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-11 15:07:40.000000 cas-tools-0.0.1.dev8/src/cas_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:35:15.073545 cas-tools-0.0.1.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-12-11 15:35:15.073545 cas-tools-0.0.1.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 15:35:15.073545 cas-tools-0.0.1.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:35:15.069545 cas-tools-0.0.1.dev9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:35:15.073545 cas-tools-0.0.1.dev9/src/cas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:35:15.073545 cas-tools-0.0.1.dev9/src/cas/accession/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/accession/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/accession/base_accession_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/accession/hash_accession_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/accession/incremental_accession_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/anndata_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/flatten_data_to_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/flatten_data_to_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:35:15.073545 cas-tools-0.0.1.dev9/src/cas/ingest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/ingest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/ingest/config_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/ingest/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/ingest/ingest_user_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:35:15.073545 cas-tools-0.0.1.dev9/src/cas/matrix_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/matrix_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/matrix_file/base_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/matrix_file/cxg_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/matrix_file/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2023-12-11 15:34:51.000000 cas-tools-0.0.1.dev9/src/cas/populate_cell_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:35:15.073545 cas-tools-0.0.1.dev9/src/cas_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-12-11 15:35:14.000000 cas-tools-0.0.1.dev9/src/cas_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2023-12-11 15:35:14.000000 cas-tools-0.0.1.dev9/src/cas_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 15:35:14.000000 cas-tools-0.0.1.dev9/src/cas_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-11 15:35:14.000000 cas-tools-0.0.1.dev9/src/cas_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-11 15:35:14.000000 cas-tools-0.0.1.dev9/src/cas_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-11 15:35:14.000000 cas-tools-0.0.1.dev9/src/cas_tools.egg-info/top_level.txt
```

### Comparing `cas-tools-0.0.1.dev8/PKG-INFO` & `cas-tools-0.0.1.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cas-tools
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: Cell Annotation Schema tools.
 Home-page: https://github.com/cellannotation/cas-tools
 Author: 
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `cas-tools-0.0.1.dev8/README.md` & `cas-tools-0.0.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/setup.py` & `cas-tools-0.0.1.dev9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="cas-tools",
-    version="0.0.1.dev8",
+    version="0.0.1.dev9",
     description="Cell Annotation Schema tools.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/cellannotation/cas-tools",
     author="",
     license="Apache-2.0 license",
     classifiers=[
```

### Comparing `cas-tools-0.0.1.dev8/src/cas/__main__.py` & `cas-tools-0.0.1.dev9/src/cas/__main__.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/accession/base_accession_manager.py` & `cas-tools-0.0.1.dev9/src/cas/accession/base_accession_manager.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/accession/hash_accession_manager.py` & `cas-tools-0.0.1.dev9/src/cas/accession/hash_accession_manager.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/accession/incremental_accession_manager.py` & `cas-tools-0.0.1.dev9/src/cas/accession/incremental_accession_manager.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/anndata_conversion.py` & `cas-tools-0.0.1.dev9/src/cas/anndata_conversion.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/file_utils.py` & `cas-tools-0.0.1.dev9/src/cas/file_utils.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/flatten_data_to_anndata.py` & `cas-tools-0.0.1.dev9/src/cas/flatten_data_to_anndata.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/flatten_data_to_tables.py` & `cas-tools-0.0.1.dev9/src/cas/flatten_data_to_tables.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/ingest/config_validator.py` & `cas-tools-0.0.1.dev9/src/cas/ingest/config_validator.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/ingest/ingest_user_table.py` & `cas-tools-0.0.1.dev9/src/cas/ingest/ingest_user_table.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/matrix_file/base_resolver.py` & `cas-tools-0.0.1.dev9/src/cas/matrix_file/base_resolver.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/matrix_file/cxg_resolver.py` & `cas-tools-0.0.1.dev9/src/cas/matrix_file/cxg_resolver.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/matrix_file/resolver.py` & `cas-tools-0.0.1.dev9/src/cas/matrix_file/resolver.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/model.py` & `cas-tools-0.0.1.dev9/src/cas/model.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas/populate_cell_ids.py` & `cas-tools-0.0.1.dev9/src/cas/populate_cell_ids.py`

 * *Files identical despite different names*

### Comparing `cas-tools-0.0.1.dev8/src/cas_tools.egg-info/PKG-INFO` & `cas-tools-0.0.1.dev9/src/cas_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cas-tools
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: Cell Annotation Schema tools.
 Home-page: https://github.com/cellannotation/cas-tools
 Author: 
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `cas-tools-0.0.1.dev8/src/cas_tools.egg-info/SOURCES.txt` & `cas-tools-0.0.1.dev9/src/cas_tools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 README.md
 setup.py
 src/cas/__init__.py
 src/cas/__main__.py
 src/cas/anndata_conversion.py
 src/cas/file_utils.py
 src/cas/flatten_data_to_anndata.py
@@ -9,14 +10,15 @@
 src/cas/model.py
 src/cas/populate_cell_ids.py
 src/cas/accession/__init__.py
 src/cas/accession/base_accession_manager.py
 src/cas/accession/hash_accession_manager.py
 src/cas/accession/incremental_accession_manager.py
 src/cas/ingest/__init__.py
+src/cas/ingest/config_schema.yaml
 src/cas/ingest/config_validator.py
 src/cas/ingest/ingest_user_table.py
 src/cas/matrix_file/__init__.py
 src/cas/matrix_file/base_resolver.py
 src/cas/matrix_file/cxg_resolver.py
 src/cas/matrix_file/resolver.py
 src/cas_tools.egg-info/PKG-INFO
```

