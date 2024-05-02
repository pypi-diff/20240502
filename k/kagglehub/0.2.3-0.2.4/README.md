# Comparing `tmp/kagglehub-0.2.3.tar.gz` & `tmp/kagglehub-0.2.4.tar.gz`

## Comparing `kagglehub-0.2.3.tar` & `kagglehub-0.2.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 kagglehub-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 kagglehub-0.2.3/Dockerfile
--rwxr-xr-x   0        0        0     1683 2020-02-02 00:00:00.000000 kagglehub-0.2.3/docker-hatch
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 kagglehub-0.2.3/integration_tests/test_model_download.py
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 kagglehub-0.2.3/integration_tests/test_model_upload.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/__init__.py
--rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/auth.py
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/cache.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/clients.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/colab_cache_resolver.py
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/config.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/env.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/exceptions.py
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/gcs_upload.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/handle.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/http_resolver.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/integrity.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/kaggle_cache_resolver.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/logging.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/models.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/models_helpers.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/registry.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/resolver.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/fixtures.py
--rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_auth.py
--rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_cache.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_colab_cache_model_download.py
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_config.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_handle.py
--rw-r--r--   0        0        0    12013 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_http_model_download.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_integrity.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_kaggle_api_client.py
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_kaggle_cache_model_download.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_kagglehub_version.py
--rw-r--r--   0        0        0    12928 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_model_upload.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_registry.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_utils.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/utils.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/data/archive.tar.gz
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/data/config.json
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/data/foo.txt
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tools/cicd/Dockerfile
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tools/cicd/cloudbuild.yaml
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tools/cicd/integration-tests.yaml
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tools/release/cloudbuild.yaml
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 kagglehub-0.2.3/.gitignore
--rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 kagglehub-0.2.3/LICENSE
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 kagglehub-0.2.3/README.md
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 kagglehub-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    18069 2020-02-02 00:00:00.000000 kagglehub-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 kagglehub-0.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 kagglehub-0.2.4/Dockerfile
+-rwxr-xr-x   0        0        0     1683 2020-02-02 00:00:00.000000 kagglehub-0.2.4/docker-hatch
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 kagglehub-0.2.4/integration_tests/test_model_download.py
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 kagglehub-0.2.4/integration_tests/test_model_upload.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/__init__.py
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/auth.py
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/cache.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/clients.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/colab_cache_resolver.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/config.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/env.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/exceptions.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/gcs_upload.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/handle.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/http_resolver.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/integrity.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/kaggle_cache_resolver.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/logging.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/models.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/models_helpers.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/registry.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 kagglehub-0.2.4/src/kagglehub/resolver.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/fixtures.py
+-rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_auth.py
+-rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_cache.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_colab_cache_model_download.py
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_config.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_handle.py
+-rw-r--r--   0        0        0    12013 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_http_model_download.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_integrity.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_kaggle_api_client.py
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_kaggle_cache_model_download.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_kagglehub_version.py
+-rw-r--r--   0        0        0    14249 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_model_upload.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_registry.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/test_utils.py
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/utils.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/data/archive.tar.gz
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/data/config.json
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tests/data/foo.txt
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tools/cicd/Dockerfile
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tools/cicd/cloudbuild.yaml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tools/cicd/integration-tests.yaml
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 kagglehub-0.2.4/tools/release/cloudbuild.yaml
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 kagglehub-0.2.4/.gitignore
+-rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 kagglehub-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 kagglehub-0.2.4/README.md
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 kagglehub-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    18069 2020-02-02 00:00:00.000000 kagglehub-0.2.4/PKG-INFO
```

### Comparing `kagglehub-0.2.3/CHANGELOG.md` & `kagglehub-0.2.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## Next (Unreleased)
 
+## v0.2.4 (April 26th, 2024)
+
+* Remove zipping in upload ([#105]((https://github.com/Kaggle/kagglehub/pull/105)))
+
 ## v0.2.3 (April 16th, 2024)
 
 * Improve upload speed ([#100](https://github.com/Kaggle/kagglehub/pull/100))
 
 ## v0.2.2 (March 27th, 2024)
 
 * Add support for single file upload ([#97](https://github.com/Kaggle/kagglehub/pull/97))
```

### Comparing `kagglehub-0.2.3/docker-hatch` & `kagglehub-0.2.4/docker-hatch`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/integration_tests/test_model_download.py` & `kagglehub-0.2.4/integration_tests/test_model_download.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/integration_tests/test_model_upload.py` & `kagglehub-0.2.4/integration_tests/test_model_upload.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from functools import wraps
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Callable, Type, TypeVar
 
 from kagglehub import model_upload, models_helpers
 from kagglehub.config import get_kaggle_credentials
-from kagglehub.exceptions import BackendError
 
 LICENSE_NAME = "MIT"
 
 logger = logging.getLogger(__name__)
 
 
 ReturnType = TypeVar("ReturnType")
@@ -42,27 +41,14 @@
             raise RuntimeError(runtime_error_message)
 
         return wrapper
 
     return decorator
 
 
-@retry(times=5, delay_seconds=10, exception_to_check=BackendError)
-def upload_with_retries(handle: str, temp_dir: str, license_name: str) -> None:
-    """
-    Uploads a model with retries on BackendError indicating the instance slug is already in use.
-
-    Args:
-        handle: The model handle.
-        temp_dir: Temporary directory where the model is stored.
-        license_name: License name for the model.
-    """
-    model_upload(handle, temp_dir, license_name)
-
-
 class TestModelUpload(unittest.TestCase):
     def setUp(self) -> None:
         self.temp_dir = tempfile.mkdtemp()
         self.dummy_files = ["dummy_model.h5", "config.json", "metadata.json"]
         for file in self.dummy_files:
             with open(os.path.join(self.temp_dir, file), "w") as f:
                 f.write("dummy content")
@@ -75,29 +61,29 @@
         self.handle = f"{self.owner_slug}/{self.model_slug}/pyTorch/new-variation"
 
     def test_model_upload_and_versioning(self) -> None:
         # Create Instance
         model_upload(self.handle, self.temp_dir, LICENSE_NAME)
 
         # Create Version
-        upload_with_retries(self.handle, self.temp_dir, LICENSE_NAME)
+        model_upload(self.handle, self.temp_dir, LICENSE_NAME)
 
         # If delete model does not raise an error, then the upload was successful.
 
     def test_model_upload_and_versioning_zip(self) -> None:
         with TemporaryDirectory() as temp_dir:
             for i in range(60):
                 test_filepath = Path(temp_dir) / f"temp_test_file_{i}"
                 test_filepath.touch()
 
             # Create Instance
             model_upload(self.handle, temp_dir, LICENSE_NAME)
 
             # Create Version
-            upload_with_retries(self.handle, temp_dir, LICENSE_NAME)
+            model_upload(self.handle, temp_dir, LICENSE_NAME)
 
     def test_model_upload_directory(self) -> None:
         with TemporaryDirectory() as temp_dir:
             # Create the new folder within temp_dir
             inner_folder_path = Path(temp_dir) / "inner_folder"
             inner_folder_path.mkdir()
 
@@ -110,15 +96,31 @@
                 test_filepath_inner = inner_folder_path / f"temp_test_file_{i}"
                 test_filepath_inner.touch()
 
             # Create Instance
             model_upload(self.handle, temp_dir, LICENSE_NAME)
 
             # Create Version
-            upload_with_retries(self.handle, temp_dir, LICENSE_NAME)
+            model_upload(self.handle, temp_dir, LICENSE_NAME)
+
+    def test_model_upload_directory_structure(self) -> None:
+        nested_dir = Path(self.temp_dir) / "nested"
+        nested_dir.mkdir()
+
+        with open(Path(self.temp_dir) / "file1.txt", "w") as f:
+            f.write("dummy content in nested file")
+
+        # Create dummy files in the nested directory
+        nested_dummy_files = ["nested_model.h5", "nested_config.json", "nested_metadata.json"]
+        for file in nested_dummy_files:
+            with open(nested_dir / file, "w") as f:
+                f.write("dummy content in nested file")
+
+        # Call the model upload function with the base directory
+        model_upload(self.handle, self.temp_dir, LICENSE_NAME)
 
     def test_model_upload_nested_dir(self) -> None:
         # Create a nested directory within self.temp_dir
         nested_dir = Path(self.temp_dir) / "nested"
         nested_dir.mkdir()
 
         # Create dummy files in the nested directory
```

### Comparing `kagglehub-0.2.3/src/kagglehub/__init__.py` & `kagglehub-0.2.4/src/kagglehub/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 import kagglehub.logging  # configures the library logger.
 from kagglehub import colab_cache_resolver, http_resolver, kaggle_cache_resolver, registry
 from kagglehub.auth import login
 from kagglehub.models import model_download, model_upload
 
 registry.model_resolver.add_implementation(http_resolver.ModelHttpResolver())
```

### Comparing `kagglehub-0.2.3/src/kagglehub/auth.py` & `kagglehub-0.2.4/src/kagglehub/auth.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/src/kagglehub/cache.py` & `kagglehub-0.2.4/src/kagglehub/cache.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/src/kagglehub/clients.py` & `kagglehub-0.2.4/src/kagglehub/clients.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/src/kagglehub/colab_cache_resolver.py` & `kagglehub-0.2.4/src/kagglehub/colab_cache_resolver.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/src/kagglehub/config.py` & `kagglehub-0.2.4/src/kagglehub/config.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/src/kagglehub/env.py` & `kagglehub-0.2.4/src/kagglehub/env.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/src/kagglehub/exceptions.py` & `kagglehub-0.2.4/src/kagglehub/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 
 class ColabEnvironmentError(Exception):
     pass
 
 
 class BackendError(Exception):
-    pass
+    def __init__(self, message: str, error_code: Optional[int] = None) -> None:
+        self.error_code = error_code
+        super().__init__(message)
 
 
 class NotFoundError(Exception):
     pass
 
 
 class DataCorruptionError(Exception):
@@ -98,8 +100,9 @@
     """
     Postprocesses the API response to check for errors.
     """
     if not (200 <= response.get("code", 200) < 300):  # noqa: PLR2004
         error_message = response.get("message", "No error message provided")
         raise BackendError(error_message)
     elif "error" in response and response["error"] != "":
-        raise BackendError(response["error"])
+        error_code = int(response["errorCode"]) if "errorCode" in response else None
+        raise BackendError(response["error"], error_code)
```

### Comparing `kagglehub-0.2.3/src/kagglehub/handle.py` & `kagglehub-0.2.4/src/kagglehub/handle.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Functions to parse resource handles."""
 
 import abc
 from dataclasses import dataclass
 from typing import Optional
 
+from kagglehub.config import get_kaggle_api_endpoint
+
 NUM_VERSIONED_MODEL_PARTS = 5  # e.g.: <owner>/<model>/<framework>/<variation>/<version>
 NUM_UNVERSIONED_MODEL_PARTS = 4  # e.g.: <owner>/<model>/<framework>/<variation>
 
 # TODO(b/313706281): Implement a DatasetHandle class & parse_dataset_handle method.
 
 
 @dataclass
@@ -33,18 +35,19 @@
     def __str__(self) -> str:
         handle_str = f"{self.owner}/{self.model}/{self.framework}/{self.variation}"
         if self.is_versioned():
             return f"{handle_str}/{self.version}"
         return handle_str
 
     def to_url(self) -> str:
+        endpoint = get_kaggle_api_endpoint()
         if self.is_versioned():
-            return f"https://www.kaggle.com/models/{self.owner}/{self.model}/{self.framework}/{self.variation}/{self.version}"
+            return f"{endpoint}/models/{self.owner}/{self.model}/{self.framework}/{self.variation}/{self.version}"
         else:
-            return f"https://www.kaggle.com/models/{self.owner}/{self.model}/{self.framework}/{self.variation}"
+            return f"{endpoint}/models/{self.owner}/{self.model}/{self.framework}/{self.variation}"
 
 
 @dataclass
 class DatasetHandle:
     owner: str
     dataset_name: str
     version: Optional[int] = None
@@ -55,15 +58,16 @@
     def __str__(self) -> str:
         handle_str = f"{self.owner}/{self.dataset_name}"
         if self.is_versioned():
             return f"{handle_str}/{self.version}"
         return handle_str
 
     def to_url(self) -> str:
-        base_url = f"https://www.kaggle.com/datasets/{self.owner}/{self.dataset_name}"
+        endpoint = get_kaggle_api_endpoint()
+        base_url = f"{endpoint}/datasets/{self.owner}/{self.dataset_name}"
         if self.is_versioned():
             return f"{base_url}/versions/{self.version}"
         return base_url
 
 
 def parse_model_handle(handle: str) -> ModelHandle:
     parts = handle.split("/")
```

### Comparing `kagglehub-0.2.3/src/kagglehub/http_resolver.py` & `kagglehub-0.2.4/src/kagglehub/http_resolver.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/src/kagglehub/integrity.py` & `kagglehub-0.2.4/src/kagglehub/integrity.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/src/kagglehub/kaggle_cache_resolver.py` & `kagglehub-0.2.4/src/kagglehub/kaggle_cache_resolver.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/src/kagglehub/logging.py` & `kagglehub-0.2.4/src/kagglehub/logging.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/src/kagglehub/models.py` & `kagglehub-0.2.4/src/kagglehub/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Optional
 
 from kagglehub import registry
-from kagglehub.gcs_upload import upload_files
+from kagglehub.gcs_upload import upload_files_and_directories
 from kagglehub.handle import parse_model_handle
 from kagglehub.models_helpers import create_model_if_missing, create_model_instance_or_version
 
 logger = logging.getLogger(__name__)
 
 
 def model_download(handle: str, path: Optional[str] = None, *, force_download: Optional[bool] = False) -> str:
@@ -43,11 +43,11 @@
         is_versioned_exception = "The model handle should not include the version"
         raise ValueError(is_versioned_exception)
 
     # Create the model if it doesn't already exist
     create_model_if_missing(h.owner, h.model)
 
     # Upload the model files to GCS
-    tokens = upload_files(local_model_dir, "model")
+    tokens = upload_files_and_directories(local_model_dir, "model")
 
     # Create a model instance if it doesn't exist, and create a new instance version if an instance exists
     create_model_instance_or_version(h, tokens, license_name, version_notes)
```

### Comparing `kagglehub-0.2.3/src/kagglehub/models_helpers.py` & `kagglehub-0.2.4/src/kagglehub/models_helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,72 @@
 import logging
 from http import HTTPStatus
-from typing import List, Optional
+from typing import Optional
 
-from kagglehub.clients import KaggleApiV1Client
+from kagglehub.clients import BackendError, KaggleApiV1Client
 from kagglehub.exceptions import KaggleApiHTTPError
+from kagglehub.gcs_upload import UploadDirectoryInfo
 from kagglehub.handle import ModelHandle
 
 logger = logging.getLogger(__name__)
 
 
 def _create_model(owner_slug: str, model_slug: str) -> None:
     data = {"ownerSlug": owner_slug, "slug": model_slug, "title": model_slug, "isPrivate": True}
     api_client = KaggleApiV1Client()
     api_client.post("/models/create/new", data)
     logger.info(f"Model '{model_slug}' Created.")
 
 
-def _create_model_instance(model_handle: ModelHandle, files: List[str], license_name: Optional[str] = None) -> None:
+def _create_model_instance(
+    model_handle: ModelHandle, files_and_directories: UploadDirectoryInfo, license_name: Optional[str] = None
+) -> None:
+    serialized_data = files_and_directories.serialize()
     data = {
         "instanceSlug": model_handle.variation,
         "framework": model_handle.framework,
-        "files": [{"token": file_token} for file_token in files],
+        "files": [{"token": file_token} for file_token in files_and_directories.files],
+        "directories": serialized_data["directories"],
     }
     if license_name is not None:
         data["licenseName"] = license_name
 
     api_client = KaggleApiV1Client()
     api_client.post(f"/models/{model_handle.owner}/{model_handle.model}/create/instance", data)
     logger.info(f"Your model instance has been created.\nFiles are being processed...\nSee at: {model_handle.to_url()}")
 
 
-def _create_model_instance_version(model_handle: ModelHandle, files: List[str], version_notes: str = "") -> None:
-    data = {"versionNotes": version_notes, "files": [{"token": file_token} for file_token in files]}
+def _create_model_instance_version(
+    model_handle: ModelHandle, files_and_directories: UploadDirectoryInfo, version_notes: str = ""
+) -> None:
+    serialized_data = files_and_directories.serialize()
+    data = {
+        "versionNotes": version_notes,
+        "files": [{"token": file_token} for file_token in files_and_directories.files],
+        "directories": serialized_data["directories"],
+    }
     api_client = KaggleApiV1Client()
     api_client.post(
         f"/models/{model_handle.owner}/{model_handle.model}/{model_handle.framework}/{model_handle.variation}/create/version",
         data,
     )
     logger.info(
         f"Your model instance version has been created.\nFiles are being processed...\nSee at: {model_handle.to_url()}"
     )
 
 
 def create_model_instance_or_version(
-    model_handle: ModelHandle, files: List[str], license_name: Optional[str], version_notes: str = ""
+    model_handle: ModelHandle, files: UploadDirectoryInfo, license_name: Optional[str], version_notes: str = ""
 ) -> None:
     try:
-        api_client = KaggleApiV1Client()
-        api_client.get(f"/models/{model_handle}/get", model_handle)
-        # the instance exist, create a new version.
-        _create_model_instance_version(model_handle, files, version_notes)
-    except KaggleApiHTTPError as e:
-        if e.response is not None and (
-            e.response.status_code == HTTPStatus.NOT_FOUND  # noqa: PLR1714
-            or e.response.status_code == HTTPStatus.FORBIDDEN
-        ):
-            _create_model_instance(model_handle, files, license_name)
+        _create_model_instance(model_handle, files, license_name)
+    except BackendError as e:
+        if e.error_code == HTTPStatus.CONFLICT:
+            # Instance already exist, creating a new version instead.
+            _create_model_instance_version(model_handle, files, version_notes)
         else:
             raise (e)
 
 
 def create_model_if_missing(owner_slug: str, model_slug: str) -> None:
     try:
         api_client = KaggleApiV1Client()
```

### Comparing `kagglehub-0.2.3/src/kagglehub/registry.py` & `kagglehub-0.2.4/src/kagglehub/registry.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/src/kagglehub/resolver.py` & `kagglehub-0.2.4/src/kagglehub/resolver.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/test_auth.py` & `kagglehub-0.2.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/test_cache.py` & `kagglehub-0.2.4/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/test_colab_cache_model_download.py` & `kagglehub-0.2.4/tests/test_colab_cache_model_download.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/test_config.py` & `kagglehub-0.2.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/test_handle.py` & `kagglehub-0.2.4/tests/test_handle.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/test_http_model_download.py` & `kagglehub-0.2.4/tests/test_http_model_download.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/test_integrity.py` & `kagglehub-0.2.4/tests/test_integrity.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/test_kaggle_api_client.py` & `kagglehub-0.2.4/tests/test_kaggle_api_client.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/test_kaggle_cache_model_download.py` & `kagglehub-0.2.4/tests/test_kaggle_cache_model_download.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/test_model_upload.py` & `kagglehub-0.2.4/tests/test_model_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         with create_test_http_server(KaggleAPIHandler):
             with create_test_http_server(GcsAPIHandler, "http://localhost:7778"):
                 with TemporaryDirectory() as temp_dir:
                     test_filepath = Path(temp_dir) / TEMP_TEST_FILE
                     test_filepath.touch()  # Create a temporary file in the temporary directory
                     model_upload("metaresearch/new-model/pyTorch/new-variation", temp_dir, APACHE_LICENSE, "model_type")
                     self.assertEqual(len(KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES), 1)
-                    self.assertIn(TEMP_ARCHIVE_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
+                    self.assertIn(TEMP_TEST_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
 
     def test_model_upload_instance_with_nested_directories(self) -> None:
         # execution path: get_model -> create_model -> get_instance -> create_version
         with create_test_http_server(KaggleAPIHandler):
             with create_test_http_server(GcsAPIHandler, "http://localhost:7778"):
                 with TemporaryDirectory() as temp_dir:
                     # Create a nested directory structure
@@ -152,27 +152,27 @@
                     nested_dir.mkdir()
 
                     # Create a temporary file in the nested directory
                     test_filepath = nested_dir / TEMP_TEST_FILE
                     test_filepath.touch()
                     model_upload("metaresearch/new-model/pyTorch/new-variation", temp_dir, APACHE_LICENSE, "model_type")
                     self.assertEqual(len(KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES), 1)
-                    self.assertIn(TEMP_ARCHIVE_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
+                    self.assertIn(TEMP_TEST_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
 
     def test_model_upload_version_with_valid_handle(self) -> None:
         # execution path: get_model -> get_instance -> create_instance
 
         with create_test_http_server(KaggleAPIHandler):
             with create_test_http_server(GcsAPIHandler, "http://localhost:7778"):
                 with TemporaryDirectory() as temp_dir:
                     test_filepath = Path(temp_dir) / TEMP_TEST_FILE
                     test_filepath.touch()  # Create a temporary file in the temporary directory
                     model_upload("metaresearch/llama-2/pyTorch/7b", temp_dir, APACHE_LICENSE, "model_type")
                     self.assertEqual(len(KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES), 1)
-                    self.assertIn(TEMP_ARCHIVE_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
+                    self.assertIn(TEMP_TEST_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
 
     def test_model_upload_with_too_many_files(self) -> None:
         with create_test_http_server(KaggleAPIHandler):
             with create_test_http_server(GcsAPIHandler, "http://localhost:7778"):
                 with TemporaryDirectory() as temp_dir:
                     # Create more than 50 temporary files in the directory
                     for i in range(MAX_FILES_TO_UPLOAD + 1):
@@ -195,35 +195,35 @@
                         f.write(os.urandom(1000))
 
                     model_upload("metaresearch/new-model/pyTorch/new-variation", temp_dir, APACHE_LICENSE, "model_type")
 
                     # Check that GcsAPIHandler received two PUT requests
                     self.assertEqual(GcsAPIHandler.put_requests_count, 2)
                     self.assertEqual(len(KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES), 1)
-                    self.assertIn(TEMP_ARCHIVE_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
+                    self.assertIn(TEMP_TEST_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
 
     def test_model_upload_with_none_license(self) -> None:
         with create_test_http_server(KaggleAPIHandler):
             with create_test_http_server(GcsAPIHandler, "http://localhost:7778"):
                 with TemporaryDirectory() as temp_dir:
                     test_filepath = Path(temp_dir) / TEMP_TEST_FILE
                     test_filepath.touch()  # Create a temporary file in the temporary directory
                     model_upload("metaresearch/new-model/pyTorch/new-variation", temp_dir, None, "model_type")
                     self.assertEqual(len(KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES), 1)
-                    self.assertIn(TEMP_ARCHIVE_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
+                    self.assertIn(TEMP_TEST_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
 
     def test_model_upload_without_license(self) -> None:
         with create_test_http_server(KaggleAPIHandler):
             with create_test_http_server(GcsAPIHandler, "http://localhost:7778"):
                 with TemporaryDirectory() as temp_dir:
                     test_filepath = Path(temp_dir) / TEMP_TEST_FILE
                     test_filepath.touch()  # Create a temporary file in the temporary directory
                     model_upload("metaresearch/new-model/pyTorch/new-variation", temp_dir, version_notes="model_type")
                     self.assertEqual(len(KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES), 1)
-                    self.assertIn(TEMP_ARCHIVE_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
+                    self.assertIn(TEMP_TEST_FILE, KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
 
     def test_model_upload_with_invalid_license_fails(self) -> None:
         with create_test_http_server(KaggleAPIHandler):
             with create_test_http_server(GcsAPIHandler, "http://localhost:7778"):
                 with TemporaryDirectory() as temp_dir:
                     test_filepath = Path(temp_dir) / TEMP_TEST_FILE
                     test_filepath.touch()  # Create a temporary file in the temporary directory
@@ -240,7 +240,33 @@
 
                     model_upload(
                         "metaresearch/new-model/pyTorch/new-variation", str(test_filepath), APACHE_LICENSE, "model_type"
                     )
 
                     self.assertEqual(len(KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES), 1)
                     self.assertIn("single_dummy_file.txt", KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES)
+
+    def test_model_upload_with_directory_structure(self) -> None:
+        with create_test_http_server(KaggleAPIHandler):
+            with create_test_http_server(GcsAPIHandler, "http://localhost:7778"):
+                with TemporaryDirectory() as temp_dir:
+                    base_path = Path(temp_dir)
+                    (base_path / "dir1").mkdir()
+                    (base_path / "dir2").mkdir()
+
+                    (base_path / "file1.txt").touch()
+
+                    (base_path / "dir1" / "file2.txt").touch()
+                    (base_path / "dir1" / "file3.txt").touch()
+
+                    (base_path / "dir1" / "subdir1").mkdir()
+                    (base_path / "dir1" / "subdir1" / "file4.txt").touch()
+
+                    model_upload("metaresearch/new-model/pyTorch/new-variation", temp_dir, APACHE_LICENSE, "model_type")
+
+                    self.assertEqual(len(KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES), 4)
+                    expected_files = {"file1.txt", "file2.txt", "file3.txt", "file4.txt"}
+                    self.assertTrue(set(KaggleAPIHandler.UPLOAD_BLOB_FILE_NAMES).issubset(expected_files))
+
+                    # TODO: Add assertions on CreateModelInstanceRequest.Directories and
+                    # CreateModelInstanceRequest.Files to verify the expected structure
+                    # is sent.
```

### Comparing `kagglehub-0.2.3/tests/test_registry.py` & `kagglehub-0.2.4/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/test_utils.py` & `kagglehub-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tests/utils.py` & `kagglehub-0.2.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tools/cicd/cloudbuild.yaml` & `kagglehub-0.2.4/tools/cicd/cloudbuild.yaml`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tools/cicd/integration-tests.yaml` & `kagglehub-0.2.4/tools/cicd/integration-tests.yaml`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/tools/release/cloudbuild.yaml` & `kagglehub-0.2.4/tools/release/cloudbuild.yaml`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/.gitignore` & `kagglehub-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/LICENSE` & `kagglehub-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/README.md` & `kagglehub-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/pyproject.toml` & `kagglehub-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.3/PKG-INFO` & `kagglehub-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kagglehub
-Version: 0.2.3
+Version: 0.2.4
 Summary: Access Kaggle resources anywhere
 Project-URL: Homepage, https://github.com/Kaggle/kagglehub
 Project-URL: Bug Tracker, https://github.com/Kaggle/kagglehub/issues
 Author-email: Kaggle <support@kaggle.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

