# Comparing `tmp/np_aind_metadata-0.1.8.tar.gz` & `tmp/np_aind_metadata-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_aind_metadata-0.1.8.tar", last modified: Wed May  1 21:18:31 2024, max compression
+gzip compressed data, was "np_aind_metadata-0.1.9.tar", last modified: Thu May  2 01:10:05 2024, max compression
```

## Comparing `np_aind_metadata-0.1.8.tar` & `np_aind_metadata-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.615282 np_aind_metadata-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-01 21:18:31.615282 np_aind_metadata-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-01 21:18:29.000000 np_aind_metadata-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:18:31.615282 np_aind_metadata-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.607282 np_aind_metadata-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.611282 np_aind_metadata-0.1.8/src/np_aind_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-01 21:18:25.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/dynamic_routing_task_etl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.611282 np_aind_metadata-0.1.8/src/np_aind_metadata/init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22049 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/init/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/np.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-01 21:18:25.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/np_codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.611282 np_aind_metadata-0.1.8/src/np_aind_metadata/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-01 21:18:26.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-05-01 21:18:25.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-01 21:18:26.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.615282 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.615282 np_aind_metadata-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/tests/test_np.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/tests/test_np_codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:10:05.510041 np_aind_metadata-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-02 01:10:05.510041 np_aind_metadata-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-02 01:10:02.000000 np_aind_metadata-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:10:05.514041 np_aind_metadata-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:10:05.506041 np_aind_metadata-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:10:05.510041 np_aind_metadata-0.1.9/src/np_aind_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/dynamic_routing_task_etl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:10:05.510041 np_aind_metadata-0.1.9/src/np_aind_metadata/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22049 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/init/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/np_codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:10:05.510041 np_aind_metadata-0.1.9/src/np_aind_metadata/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/src/np_aind_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:10:05.510041 np_aind_metadata-0.1.9/src/np_aind_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-02 01:10:05.000000 np_aind_metadata-0.1.9/src/np_aind_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-02 01:10:05.000000 np_aind_metadata-0.1.9/src/np_aind_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:10:05.000000 np_aind_metadata-0.1.9/src/np_aind_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-02 01:10:05.000000 np_aind_metadata-0.1.9/src/np_aind_metadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-02 01:10:05.000000 np_aind_metadata-0.1.9/src/np_aind_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 01:10:05.000000 np_aind_metadata-0.1.9/src/np_aind_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:10:05.510041 np_aind_metadata-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/tests/test_np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/tests/test_np_codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-02 01:09:26.000000 np_aind_metadata-0.1.9/tests/test_storage.py
```

### Comparing `np_aind_metadata-0.1.8/LICENSE` & `np_aind_metadata-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/PKG-INFO` & `np_aind_metadata-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-aind-metadata
-Version: 0.1.8
+Version: 0.1.9
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-aind-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/np-aind-metadata/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `np_aind_metadata-0.1.8/README.md` & `np_aind_metadata-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/pyproject.toml` & `np_aind_metadata-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dependencies = [
     "h5py>=3.10.0",
     "pyyaml>=6.0.1",
     "np-session>=0.6.40",
     "np-config>=0.4.27",
     "aind-metadata-mapper==0.6.2",
 ]
-version = "0.1.8"
+version = "0.1.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `np_aind_metadata-0.1.8/src/np_aind_metadata/__init__.py` & `np_aind_metadata-0.1.9/src/np_aind_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/src/np_aind_metadata/dynamic_routing_task_etl.py` & `np_aind_metadata-0.1.9/src/np_aind_metadata/dynamic_routing_task_etl.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/src/np_aind_metadata/init/neuropixels_rig.py` & `np_aind_metadata-0.1.9/src/np_aind_metadata/init/neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/src/np_aind_metadata/np.py` & `np_aind_metadata-0.1.9/src/np_aind_metadata/np.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/src/np_aind_metadata/np_codeocean.py` & `np_aind_metadata-0.1.9/src/np_aind_metadata/np_codeocean.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/src/np_aind_metadata/scripts/main.py` & `np_aind_metadata-0.1.9/src/np_aind_metadata/scripts/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,14 @@
         )
         rig_model.write_standard_file(temp_dir)
         rig_model_path = pathlib.Path(temp_dir) / "rig.json"
         added_path = storage.update_item(
             storage_directory,
             rig_model_path,
             rig_name,
-            "dynamic-routing",
         )
         logger.debug("Stored rig model at: %s" % added_path)
 
     click.echo("Initialized rig storage for: %s" % rig_name)
 
 
 # @cli.command()
```

### Comparing `np_aind_metadata-0.1.8/src/np_aind_metadata/storage.py` & `np_aind_metadata-0.1.9/src/np_aind_metadata/storage.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/src/np_aind_metadata/update.py` & `np_aind_metadata-0.1.9/src/np_aind_metadata/update.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/src/np_aind_metadata/utils.py` & `np_aind_metadata-0.1.9/src/np_aind_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/PKG-INFO` & `np_aind_metadata-0.1.9/src/np_aind_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-aind-metadata
-Version: 0.1.8
+Version: 0.1.9
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-aind-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/np-aind-metadata/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/SOURCES.txt` & `np_aind_metadata-0.1.9/src/np_aind_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/tests/test_np_codeocean.py` & `np_aind_metadata-0.1.9/tests/test_np_codeocean.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.8/tests/test_storage.py` & `np_aind_metadata-0.1.9/tests/test_storage.py`

 * *Files identical despite different names*

