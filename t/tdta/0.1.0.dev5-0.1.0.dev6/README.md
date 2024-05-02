# Comparing `tmp/tdta-0.1.0.dev5.tar.gz` & `tmp/tdta-0.1.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdta-0.1.0.dev5.tar", last modified: Wed Mar 13 13:30:46 2024, max compression
+gzip compressed data, was "tdta-0.1.0.dev6.tar", last modified: Thu May  2 10:31:32 2024, max compression
```

## Comparing `tdta-0.1.0.dev5.tar` & `tdta-0.1.0.dev6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:30:46.969408 tdta-0.1.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-13 13:30:23.000000 tdta-0.1.0.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:30:23.000000 tdta-0.1.0.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-13 13:30:46.969408 tdta-0.1.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-13 13:30:23.000000 tdta-0.1.0.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 13:30:46.969408 tdta-0.1.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-13 13:30:23.000000 tdta-0.1.0.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:30:46.969408 tdta-0.1.0.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:30:46.969408 tdta-0.1.0.dev5/src/tdta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:30:23.000000 tdta-0.1.0.dev5/src/tdta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-03-13 13:30:23.000000 tdta-0.1.0.dev5/src/tdta/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-13 13:30:23.000000 tdta-0.1.0.dev5/src/tdta/anndata_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-03-13 13:30:23.000000 tdta-0.1.0.dev5/src/tdta/purl_publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-03-13 13:30:23.000000 tdta-0.1.0.dev5/src/tdta/tdt_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-13 13:30:23.000000 tdta-0.1.0.dev5/src/tdta/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:30:46.969408 tdta-0.1.0.dev5/src/tdta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-13 13:30:46.000000 tdta-0.1.0.dev5/src/tdta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-13 13:30:46.000000 tdta-0.1.0.dev5/src/tdta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 13:30:46.000000 tdta-0.1.0.dev5/src/tdta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-13 13:30:46.000000 tdta-0.1.0.dev5/src/tdta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-13 13:30:46.000000 tdta-0.1.0.dev5/src/tdta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-13 13:30:46.000000 tdta-0.1.0.dev5/src/tdta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:31:32.452557 tdta-0.1.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 10:31:32.452557 tdta-0.1.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:31:32.452557 tdta-0.1.0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:31:32.448557 tdta-0.1.0.dev6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:31:32.448557 tdta-0.1.0.dev6/src/tdta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/anndata_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/purl_publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/tdt_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-02 10:30:43.000000 tdta-0.1.0.dev6/src/tdta/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:31:32.452557 tdta-0.1.0.dev6/src/tdta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 10:31:32.000000 tdta-0.1.0.dev6/src/tdta.egg-info/top_level.txt
```

### Comparing `tdta-0.1.0.dev5/LICENSE` & `tdta-0.1.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev5/PKG-INFO` & `tdta-0.1.0.dev6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdta
-Version: 0.1.0.dev5
+Version: 0.1.0.dev6
 Summary: The aim of this project is to provide taxonomy development tools custom actions.
 Home-page: https://github.com/hkir-dev/taxonomy-development-tools-actions
 Author: 
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tdta-0.1.0.dev5/setup.py` & `tdta-0.1.0.dev6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="tdta",
-    version="0.1.0.dev5",
+    version="0.1.0.dev6",
     description="The aim of this project is to provide taxonomy development tools custom actions.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/hkir-dev/taxonomy-development-tools-actions",
     author="",
     license="Apache-2.0 license",
     classifiers=[
```

### Comparing `tdta-0.1.0.dev5/src/tdta/__main__.py` & `tdta-0.1.0.dev6/src/tdta/__main__.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev5/src/tdta/anndata_export.py` & `tdta-0.1.0.dev6/src/tdta/anndata_export.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev5/src/tdta/purl_publish.py` & `tdta-0.1.0.dev6/src/tdta/purl_publish.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev5/src/tdta/tdt_export.py` & `tdta-0.1.0.dev6/src/tdta/tdt_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,22 @@
             parse__annotation_transfer_data(cta, sqlite_db, table_name)
 
     project_config = read_project_config(Path(output_file).parent.absolute())
 
     if "matrix_file_id" in project_config:
         matrix_file_id = str(project_config["matrix_file_id"]).strip()
         anndata = resolve_matrix_file(matrix_file_id, dataset_cache_folder)
-        cas_json = add_cell_ids(cta.to_dict(), anndata)
+        labelsets = cta.labelsets.copy()
+        labelsets.sort(key=lambda x: x.rank)
+        labelset_names = [labelset.name for labelset in labelsets]
+
+        cas_json = add_cell_ids(cta.to_dict(), anndata, labelsets=labelset_names)
+        if cas_json is None:
+            print("WARN: Cell IDs population operation failed, skipping cell_id population")
+            cas_json = cta.to_dict()
         with open(output_file, "w") as json_file:
             json.dump(cas_json, json_file, indent=2)
     else:
         print("WARN: 'matrix_file_id' not specified in the project configuration. Skipping cell_id population")
         write_json_file(cta, output_file, False)
 
     print("CAS json successfully created at: {}".format(output_file))
```

### Comparing `tdta-0.1.0.dev5/src/tdta/utils.py` & `tdta-0.1.0.dev6/src/tdta/utils.py`

 * *Files identical despite different names*

### Comparing `tdta-0.1.0.dev5/src/tdta.egg-info/PKG-INFO` & `tdta-0.1.0.dev6/src/tdta.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdta
-Version: 0.1.0.dev5
+Version: 0.1.0.dev6
 Summary: The aim of this project is to provide taxonomy development tools custom actions.
 Home-page: https://github.com/hkir-dev/taxonomy-development-tools-actions
 Author: 
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

