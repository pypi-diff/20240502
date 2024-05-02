# Comparing `tmp/np_aind_metadata-0.1.7.tar.gz` & `tmp/np_aind_metadata-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_aind_metadata-0.1.7.tar", last modified: Tue Apr 30 00:32:52 2024, max compression
+gzip compressed data, was "np_aind_metadata-0.1.8.tar", last modified: Wed May  1 21:18:31 2024, max compression
```

## Comparing `np_aind_metadata-0.1.7.tar` & `np_aind_metadata-0.1.8.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-30 00:32:50.000000 np_aind_metadata-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.955531 np_aind_metadata-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/src/np_aind_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/src/np_aind_metadata/init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22049 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/init/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/np.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-30 00:32:47.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/np_codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/src/np_aind_metadata/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/src/np_aind_metadata/update/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/update/dynamic_routing_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/update/dynamic_routing_task_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/tests/test_np.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/tests/test_np_codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.615282 np_aind_metadata-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-01 21:18:31.615282 np_aind_metadata-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-01 21:18:29.000000 np_aind_metadata-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:18:31.615282 np_aind_metadata-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.607282 np_aind_metadata-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.611282 np_aind_metadata-0.1.8/src/np_aind_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-01 21:18:25.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/dynamic_routing_task_etl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.611282 np_aind_metadata-0.1.8/src/np_aind_metadata/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22049 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/init/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-01 21:18:25.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/np_codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.611282 np_aind_metadata-0.1.8/src/np_aind_metadata/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-01 21:18:26.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-05-01 21:18:25.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-01 21:18:26.000000 np_aind_metadata-0.1.8/src/np_aind_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.615282 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 21:18:31.000000 np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:31.615282 np_aind_metadata-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/tests/test_np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/tests/test_np_codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-01 21:17:50.000000 np_aind_metadata-0.1.8/tests/test_storage.py
```

### Comparing `np_aind_metadata-0.1.7/LICENSE` & `np_aind_metadata-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.7/PKG-INFO` & `np_aind_metadata-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-aind-metadata
-Version: 0.1.7
+Version: 0.1.8
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-aind-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/np-aind-metadata/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `np_aind_metadata-0.1.7/README.md` & `np_aind_metadata-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.7/pyproject.toml` & `np_aind_metadata-0.1.8/pyproject.toml`

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
-version = "0.1.7"
+version = "0.1.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `np_aind_metadata-0.1.7/src/np_aind_metadata/__init__.py` & `np_aind_metadata-0.1.8/src/np_aind_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.7/src/np_aind_metadata/init/neuropixels_rig.py` & `np_aind_metadata-0.1.8/src/np_aind_metadata/init/neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.7/src/np_aind_metadata/np.py` & `np_aind_metadata-0.1.8/src/np_aind_metadata/np.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.7/src/np_aind_metadata/np_codeocean.py` & `np_aind_metadata-0.1.8/src/np_aind_metadata/np_codeocean.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,35 @@
 import datetime
 import logging
 import pathlib
-import shutil
-import tempfile
 
 from aind_data_schema.core import rig, session
 
-from np_aind_metadata import storage
-from np_aind_metadata.update import dynamic_routing_task as dynamic_routing_task_update
+from np_aind_metadata import storage, update
 
 logger = logging.getLogger(__name__)
 
 
 def scrape_session_model_path(session_directory: pathlib.Path) -> pathlib.Path:
     """Scrapes aind-metadata session json from dynamic routing session
     directory.
     """
     matches = list(session_directory.glob("*session.json"))
     logger.debug("Scraped session model paths: %s" % matches)
     return matches[0]
 
 
-def _update_rig_modification_date(
-    current: rig.Rig,
-    modification_date: datetime.date,
-    output_path: pathlib.Path,
-) -> pathlib.Path:
-    id_parts = current.rig_id.split("_")
-    id_parts[-1] = modification_date.strftime("%y%m%d")
-    current.rig_id = "_".join(id_parts)
-    current.modification_date = modification_date
-    with tempfile.TemporaryDirectory() as temp_dir:
-        current.write_standard_file(temp_dir)
-        temp_path = pathlib.Path(temp_dir) / current.default_filename()
-        assert temp_path.exists()
-        return pathlib.Path(shutil.copy2(temp_path, output_path))
-
+# def parse_rig_id(rig_id: str) -> tuple[str, str]:
+#     """Parses rig id, returning rig name and date.
 
-def _update_session_rig_id(
-    session: session.Session,
-    rig_id: str,
-    output_path: pathlib.Path,
-) -> pathlib.Path:
-    """Updates session rig id and copies it to `output_path`."""
-    session.rig_id = rig_id
-    with tempfile.TemporaryDirectory() as temp_dir:
-        session.write_standard_file(temp_dir)
-        temp_session_path = pathlib.Path(temp_dir) / session.default_filename()
-        assert temp_session_path.exists()
-        return pathlib.Path(shutil.copy2(temp_session_path, output_path))
+#     >>> parse_rig_id("323_NP3_210101")
+#     ('NP3', '210101')
+#     """
+#     split = rig_id.split("_")
+#     return split[-2], split[-1]
 
 
 def add_rig_to_dynamic_routing_session_dir(
     session_dir: pathlib.Path,
     rig_model_dir: pathlib.Path,
     modification_date: datetime.date,
 ) -> pathlib.Path:
@@ -61,60 +38,48 @@
      will update the associated session json.
 
     Notes
     -----
     - An aind metadata session json must exist and be ending with filename
     session.json (pattern: `*session.json`) in the root directory.
     """
-    scraped_session_model_path = scrape_session_model_path(session_dir)
+    matches = list(session_dir.glob("*session.json"))
+    logger.debug("Scraped session model paths: %s" % matches)
+    scraped_session_model_path = matches[0]
+    logger.debug("Scraped session model path: %s" % scraped_session_model_path)
     scraped_session = session.Session.model_validate_json(
         scraped_session_model_path.read_text()
     )
     scraped_rig_id = scraped_session.rig_id
     logger.info("Scraped rig id: %s" % scraped_rig_id)
     _, rig_name, _ = scraped_rig_id.split("_")
     logger.info("Parsed rig name: %s" % rig_name)
     current_model_path = storage.get_item(
         rig_model_dir,
         rig_name,
-        "dynamic-routing",
     )
     logger.info("Current model path: %s" % current_model_path)
     settings_sources = list(session_dir.glob("**/settings.xml"))
     logger.info("Scraped open ephys settings: %s" % settings_sources)
-
-    if settings_sources:
-        logger.debug("Updating model.")
-        current_model = rig.Rig.model_validate_json(current_model_path.read_text())
-        current_model.write_standard_file(session_dir)
-        session_rig_path = session_dir / "rig.json"
-        assert (
-            session_rig_path.exists()
-        ), "Session rig path should exist where we expect."
-        updated_model_path = dynamic_routing_task_update.update_rig(
-            session_rig_path,
-            open_ephys_settings_sources=settings_sources,
-            output_path=session_rig_path,
-        )
-        updated_model_path = _update_rig_modification_date(
-            rig.Rig.model_validate_json(updated_model_path.read_text()),
-            modification_date,
-            updated_model_path,
-        )
-        updated_model = rig.Rig.model_validate_json(updated_model_path.read_text())
-        if updated_model.rig_id != scraped_rig_id:
-            logger.debug("Rig model rig_id has changed. Updating session rig_id.")
-            _update_session_rig_id(
-                scraped_session,
-                updated_model.rig_id,
-                scraped_session_model_path,
-            )
-        if current_model != updated_model:
-            logger.debug("Current rig model has changed. Updating storage.")
-            storage.update_item(
-                rig_model_dir,
-                updated_model_path,
-                rig_name,
-                "dynamic-routing",
-            )
+    current_model = rig.Rig.model_validate_json(current_model_path.read_text())
+    current_model.write_standard_file(session_dir)
+    rig_model_path = session_dir / "rig.json"
+    updated_model_path = update.update_neuropixels_rig(
+        rig_model_path,
+        open_ephys_settings_sources=settings_sources,
+        output_path=rig_model_path,
+    )
+    updated_model_path = update.update_rig_modification_date(
+        updated_model_path,
+        modification_date,
+    )
+    update.update_session_modification_date(
+        scraped_session_model_path,
+        modification_date,
+    )
+    storage.update_item(
+        rig_model_dir,
+        updated_model_path,
+        rig_name,
+    )
 
     return updated_model_path
```

### Comparing `np_aind_metadata-0.1.7/src/np_aind_metadata/scripts/main.py` & `np_aind_metadata-0.1.8/src/np_aind_metadata/scripts/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import os
 import pathlib
 import tempfile
 import typing
 
 import click
 
-from np_aind_metadata import common, np, storage, utils
-from np_aind_metadata.update import dynamic_routing_task as dynamic_routing_task_update
+from np_aind_metadata import common, np, storage, update, utils
 
 logger = logging.getLogger(__name__)
 
 
 NPEXP_PATH_ROOT = os.getenv("NPEXP_PATH_ROOT")
 now = datetime.datetime.now()
 
@@ -21,30 +20,30 @@
 @click.option("--debug/--no-debug", default=False)
 @click.option("--log-file", default=False, is_flag=True)
 def cli(debug: bool, log_file: bool) -> None:
     click.echo(f"Debug mode is {'on' if debug else 'off'}")
     if debug:
         np.logger.setLevel(logging.DEBUG)
         storage.logger.setLevel(logging.DEBUG)
-        dynamic_routing_task_update.logger.setLevel(logging.DEBUG)
+        update.logger.setLevel(logging.DEBUG)
         utils.logger.setLevel(logging.DEBUG)
         logger.setLevel(logging.DEBUG)
 
     if log_file:
         handler = logging.FileHandler(
             now.strftime("np-aind-metadata_%Y-%m-%d-%H-%M-%S") + ".log"
         )
         handler.setLevel(logging.DEBUG)
         handler.setFormatter(
             logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
         )
         logger.addHandler(handler)
         np.logger.addHandler(handler)
         storage.logger.addHandler(handler)
-        dynamic_routing_task_update.logger.addHandler(handler)
+        update.logger.addHandler(handler)
         utils.logger.addHandler(handler)
 
 
 modification_date_format_0 = "%Y-%m-%d"
 modification_date_format_1 = "%Y/%m/%d"
 
 
@@ -91,9 +90,33 @@
             "dynamic-routing",
         )
         logger.debug("Stored rig model at: %s" % added_path)
 
     click.echo("Initialized rig storage for: %s" % rig_name)
 
 
+# @cli.command()
+# @click.argument("storage-directory", type=pathlib.Path)
+# def list_rigs(storage_directory: pathlib.Path) -> None:
+#     items = storage.list_items(storage_directory)
+#     for item in items:
+#         click.echo(item)
+
+
+@cli.command()
+@click.argument("storage-directory", type=pathlib.Path)
+@click.argument("rig-name", type=click.Choice(["NP1", "NP2", "NP3"]))
+@click.argument("rig-source", type=pathlib.Path)
+def update_stored_rig(
+    storage_directory: pathlib.Path, rig_name: str, rig_source: pathlib.Path
+) -> None:
+    added_path = storage.update_item(
+        storage_directory,
+        rig_source,
+        rig_name,
+    )
+    logger.debug("Stored rig model at: %s" % added_path)
+    click.echo("Updated stored rig model for: %s" % rig_name)
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `np_aind_metadata-0.1.7/src/np_aind_metadata/storage.py` & `np_aind_metadata-0.1.8/src/np_aind_metadata/storage.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.7/src/np_aind_metadata/update/dynamic_routing_task_etl.py` & `np_aind_metadata-0.1.8/src/np_aind_metadata/dynamic_routing_task_etl.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.7/src/np_aind_metadata/utils.py` & `np_aind_metadata-0.1.8/src/np_aind_metadata/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import logging
+import shutil
+import tempfile
 from pathlib import Path
 from typing import Any, Union
 
+from aind_data_schema import base
 from h5py import Dataset, File
 
 logger = logging.getLogger(__name__)
 
 
 def load_hdf5(h5_path: Path) -> File:
     """Load hdf5 file from path."""
@@ -52,7 +55,25 @@
 
 def fix_allen_path(path: Path) -> Path:
     """Fix Allen path for Windows."""
     if path.parts[0] == "\x07llen":
         logger.debug(f"Fixing Allen path: {path}")
         return Path(r"\\allen", *path.parts[1:])
     return path
+
+
+def save_aind_model(
+    model: base.AindCoreModel,
+    output_path: Path,
+) -> Path:
+    """Save aind models to a specified output path.
+
+    Notes
+    -----
+    - Gets around awkward `write_standard_file` method. to write to a determined
+    output path.
+    """
+    with tempfile.TemporaryDirectory() as temp_dir:
+        model.write_standard_file(temp_dir)
+        return Path(
+            shutil.copy2(Path(temp_dir) / model.default_filename(), output_path)
+        )
```

### Comparing `np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/PKG-INFO` & `np_aind_metadata-0.1.8/src/np_aind_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-aind-metadata
-Version: 0.1.7
+Version: 0.1.8
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-aind-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/np-aind-metadata/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `np_aind_metadata-0.1.7/tests/test_np_codeocean.py` & `np_aind_metadata-0.1.8/tests/test_np_codeocean.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import pathlib
 import shutil
+import datetime
 
-import pytest
+# import pytest
 from aind_data_schema.core import rig, session
 
-from np_aind_metadata import np_codeocean, storage
-from np_aind_metadata.update import (
-    dynamic_routing_task as dynamic_routing_task_update
-)
+from np_aind_metadata import np_codeocean, storage, update
 
 
 def _copy_resource_files(
     source: pathlib.Path,
     dest: pathlib.Path,
 ) -> pathlib.Path:
     """Test utility. Copies all files from source to dest. Recursively
@@ -26,73 +24,49 @@
             shutil.copy2(file, dest / file.name)
     return dest
 
 
 RESOURCES_DIRECTORY = pathlib.Path("tests") / "resources"
 
 
-@pytest.mark.onprem
-def test_update_session_and_rig(tmp_path: pathlib.Path) -> None:
-    """Runs two tests to ensure order is correct.
-    """
+def test_add_rig_to_dynamic_routing_session_dir(
+    tmp_path: pathlib.Path,
+) -> None:
     np_codeocean.logger.setLevel("DEBUG")
     storage.logger.setLevel("DEBUG")
-    dynamic_routing_task_update.logger.setLevel("DEBUG")
+    update.logger.setLevel("DEBUG")
     # setup temporary test directories
     rig_directory_temp = tmp_path / "rig"
     rig_directory_temp.mkdir()
     rig_directory = _copy_resource_files(
         RESOURCES_DIRECTORY / "rig-directory",
         rig_directory_temp,
     )
     session_directory_0_temp = tmp_path / "session-0"
     session_directory_0_temp.mkdir()
     session_directory_0 = _copy_resource_files(
         RESOURCES_DIRECTORY / "session-directory-0",
         session_directory_0_temp,
     )
-    session_directory_1_temp = tmp_path / "session-1"
-    session_directory_1_temp.mkdir()
-    session_directory_1 = _copy_resource_files(
-        RESOURCES_DIRECTORY / "session-directory-1",
-        session_directory_1_temp,
-    )
 
     def get_current_rig_model() -> rig.Rig:
         return rig.Rig.model_validate_json(
             storage.get_item(
                 rig_directory,
                 "NP3",
-                "dynamic-routing",
             ).read_text()
         )
 
     initial_rig_model = get_current_rig_model()
 
-    # Test no update
     np_codeocean.add_rig_to_dynamic_routing_session_dir(
         session_directory_0,
         rig_directory,
+        datetime.date(2024, 4, 1),
     )
     updated_session_0 = session.Session.model_validate_json(
         next(session_directory_0.glob("*session.json")).read_text()
     )
 
-    non_updated_rig_model = get_current_rig_model()
-    assert initial_rig_model == non_updated_rig_model
-    assert updated_session_0.rig_id == non_updated_rig_model.rig_id
-
-    # Test update
-    np_codeocean.add_rig_to_dynamic_routing_session_dir(
-        session_directory_1,
-        rig_directory,
-    )
-
     updated_rig_model = get_current_rig_model()
     assert initial_rig_model != updated_rig_model
-    assert updated_rig_model.rig_id != initial_rig_model.rig_id
-
-    updated_session_1 = session.Session.model_validate_json(
-        next(session_directory_1.glob("*session.json")).read_text()
-    )
-
-    assert updated_session_1.rig_id == updated_rig_model.rig_id
+    assert updated_session_0.rig_id == updated_rig_model.rig_id
```

### Comparing `np_aind_metadata-0.1.7/tests/test_storage.py` & `np_aind_metadata-0.1.8/tests/test_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     tmp_path: pathlib.Path
 ) -> None:
     item_0 = {
         "rig_id": "327_NP1_240401",
     }
     item_0_path = tmp_path / "item-0.json"
     item_0_path.write_text(json.dumps(item_0))
-    tags = ("NP1", "dynamic-routing")
+    tags = ("NP1", )
     storage.update_item(
         tmp_path,
         item_0_path,
         *tags,
     )
     stored_item = json.loads(storage.get_item(
         tmp_path,
```

