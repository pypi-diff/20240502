# Comparing `tmp/edgeimpulse-1.0.8.tar.gz` & `tmp/edgeimpulse-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse-1.0.8.tar", max compression
+gzip compressed data, was "edgeimpulse-1.0.9.tar", max compression
```

## Comparing `edgeimpulse-1.0.8.tar` & `edgeimpulse-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,29 @@
--rw-r--r--   0        0        0     1581 2024-01-15 17:31:46.289664 edgeimpulse-1.0.8/README.md
--rw-r--r--   0        0        0     6148 2023-09-21 17:24:42.483379 edgeimpulse-1.0.8/edgeimpulse/.DS_Store
--rw-r--r--   0        0        0      550 2024-01-16 00:13:40.206598 edgeimpulse-1.0.8/edgeimpulse/__init__.py
--rw-r--r--   0        0        0        0 2024-01-15 16:35:43.288229 edgeimpulse-1.0.8/edgeimpulse/data/__init__.py
--rw-r--r--   0        0        0     6103 2024-01-15 16:35:43.288784 edgeimpulse-1.0.8/edgeimpulse/data/_functions/delete.py
--rw-r--r--   0        0        0    12509 2024-01-15 23:50:13.485253 edgeimpulse-1.0.8/edgeimpulse/data/_functions/download.py
--rw-r--r--   0        0        0     8668 2024-01-15 16:35:43.289505 edgeimpulse-1.0.8/edgeimpulse/data/_functions/upload.py
--rw-r--r--   0        0        0     6880 2024-01-15 16:35:43.289803 edgeimpulse-1.0.8/edgeimpulse/data/_functions/upload_files.py
--rw-r--r--   0        0        0     5039 2024-01-15 17:52:09.306171 edgeimpulse-1.0.8/edgeimpulse/data/_functions/upload_numpy.py
--rw-r--r--   0        0        0    23550 2024-01-15 22:06:39.460397 edgeimpulse-1.0.8/edgeimpulse/data/_functions/upload_pandas.py
--rw-r--r--   0        0        0     8496 2024-01-11 18:56:08.742517 edgeimpulse-1.0.8/edgeimpulse/data/_functions/util.py
--rw-r--r--   0        0        0    11084 2024-01-11 18:56:08.742958 edgeimpulse-1.0.8/edgeimpulse/data/sample_type.py
--rw-r--r--   0        0        0     1601 2024-01-15 16:35:43.290441 edgeimpulse-1.0.8/edgeimpulse/datasets.py
--rw-r--r--   0        0        0     3869 2023-12-21 15:35:52.210726 edgeimpulse-1.0.8/edgeimpulse/exceptions.py
--rw-r--r--   0        0        0      113 2024-01-15 16:35:43.290746 edgeimpulse-1.0.8/edgeimpulse/experimental/__init__.py
--rw-r--r--   0        0        0     1413 2024-01-15 16:35:43.291125 edgeimpulse-1.0.8/edgeimpulse/experimental/data/__init__.py
--rw-r--r--   0        0        0      358 2023-11-16 18:16:15.790403 edgeimpulse-1.0.8/edgeimpulse/model/__init__.py
--rw-r--r--   0        0        0        0 2023-10-27 22:43:16.512444 edgeimpulse-1.0.8/edgeimpulse/model/_functions/__init__.py
--rw-r--r--   0        0        0    18837 2023-11-16 18:15:37.107748 edgeimpulse-1.0.8/edgeimpulse/model/_functions/deploy.py
--rw-r--r--   0        0        0     7995 2023-11-16 18:17:34.502623 edgeimpulse-1.0.8/edgeimpulse/model/_functions/profile.py
--rw-r--r--   0        0        0     2163 2023-11-16 18:13:45.088595 edgeimpulse-1.0.8/edgeimpulse/model/input_type.py
--rw-r--r--   0        0        0      753 2023-11-16 18:13:45.088862 edgeimpulse-1.0.8/edgeimpulse/model/model_info.py
--rw-r--r--   0        0        0     2264 2023-11-16 18:13:45.089094 edgeimpulse-1.0.8/edgeimpulse/model/output_type.py
--rw-r--r--   0        0        0    19651 2024-01-15 16:35:43.291518 edgeimpulse-1.0.8/edgeimpulse/util.py
--rw-r--r--   0        0        0     1558 2024-01-16 00:13:40.200637 edgeimpulse-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 edgeimpulse-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1581 2024-04-25 10:59:24.597281 edgeimpulse-1.0.9/README.md
+-rw-r--r--   0        0        0      858 2024-04-25 10:59:24.597281 edgeimpulse-1.0.9/edgeimpulse/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-25 10:59:24.601281 edgeimpulse-1.0.9/edgeimpulse/data/__init__.py
+-rw-r--r--   0        0        0     6192 2024-04-25 10:59:24.601281 edgeimpulse-1.0.9/edgeimpulse/data/_functions/delete.py
+-rw-r--r--   0        0        0    12690 2024-04-25 10:59:24.605281 edgeimpulse-1.0.9/edgeimpulse/data/_functions/download.py
+-rw-r--r--   0        0        0     9233 2024-04-25 10:59:24.609281 edgeimpulse-1.0.9/edgeimpulse/data/_functions/upload.py
+-rw-r--r--   0        0        0     7141 2024-04-25 10:59:24.609281 edgeimpulse-1.0.9/edgeimpulse/data/_functions/upload_files.py
+-rw-r--r--   0        0        0     4853 2024-04-25 10:59:24.613281 edgeimpulse-1.0.9/edgeimpulse/data/_functions/upload_numpy.py
+-rw-r--r--   0        0        0    22642 2024-04-25 10:59:24.617281 edgeimpulse-1.0.9/edgeimpulse/data/_functions/upload_pandas.py
+-rw-r--r--   0        0        0     8556 2024-04-25 10:59:24.617281 edgeimpulse-1.0.9/edgeimpulse/data/_functions/util.py
+-rw-r--r--   0        0        0    11573 2024-04-25 10:59:24.621281 edgeimpulse-1.0.9/edgeimpulse/data/sample_type.py
+-rw-r--r--   0        0        0    13723 2024-04-25 10:59:24.625281 edgeimpulse-1.0.9/edgeimpulse/datasets.py
+-rw-r--r--   0        0        0     3860 2024-04-25 10:59:24.625281 edgeimpulse-1.0.9/edgeimpulse/exceptions.py
+-rw-r--r--   0        0        0      169 2024-04-25 10:59:24.629281 edgeimpulse-1.0.9/edgeimpulse/experimental/__init__.py
+-rw-r--r--   0        0        0    10240 2024-04-25 10:59:24.633281 edgeimpulse-1.0.9/edgeimpulse/experimental/api.py
+-rw-r--r--   0        0        0     1557 2024-04-25 10:59:24.637281 edgeimpulse-1.0.9/edgeimpulse/experimental/data/__init__.py
+-rw-r--r--   0        0        0      471 2024-04-25 10:59:24.637281 edgeimpulse-1.0.9/edgeimpulse/experimental/tuner/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-25 10:59:24.641281 edgeimpulse-1.0.9/edgeimpulse/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 10:59:24.641281 edgeimpulse-1.0.9/edgeimpulse/model/_functions/__init__.py
+-rw-r--r--   0        0        0    18817 2024-04-25 10:59:24.645281 edgeimpulse-1.0.9/edgeimpulse/model/_functions/deploy.py
+-rw-r--r--   0        0        0     8039 2024-04-25 10:59:24.645281 edgeimpulse-1.0.9/edgeimpulse/model/_functions/profile.py
+-rw-r--r--   0        0        0     2184 2024-04-25 10:59:24.649281 edgeimpulse-1.0.9/edgeimpulse/model/input_type.py
+-rw-r--r--   0        0        0      785 2024-04-25 10:59:24.653281 edgeimpulse-1.0.9/edgeimpulse/model/model_info.py
+-rw-r--r--   0        0        0     2287 2024-04-25 10:59:24.653281 edgeimpulse-1.0.9/edgeimpulse/model/output_type.py
+-rw-r--r--   0        0        0       50 2024-04-25 10:59:24.657281 edgeimpulse-1.0.9/edgeimpulse/tuner/__init__.py
+-rw-r--r--   0        0        0    16598 2024-04-25 10:59:24.661281 edgeimpulse-1.0.9/edgeimpulse/tuner/_functions/tuner.py
+-rw-r--r--   0        0        0    27670 2024-04-25 10:59:24.665281 edgeimpulse-1.0.9/edgeimpulse/util.py
+-rw-r--r--   0        0        0     1716 2024-04-25 10:59:38.661156 edgeimpulse-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 edgeimpulse-1.0.9/PKG-INFO
```

### Comparing `edgeimpulse-1.0.8/README.md` & `edgeimpulse-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.8/edgeimpulse/__init__.py` & `edgeimpulse-1.0.9/edgeimpulse/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,36 @@
-import os
-
 # Import the subpackages here to expose them to the user
-# ruff: noqa: F401
+# ruff: noqa: F401,D104
+# mypy: ignore-errors
+import os
 import edgeimpulse.model
 import edgeimpulse.exceptions
 import edgeimpulse.experimental
+from edgeimpulse.util import configure_generic_client, default_project_id_for
+
+import edgeimpulse_api
 
 __version__ = "1.0.8"
 
 try:
     API_KEY = os.environ["EI_API_KEY"]
 except KeyError:
     API_KEY = None
 
 try:
+    EI_USERNAME = os.environ["EI_USERNAME"]
+except KeyError:
+    EI_USERNAME = None
+
+try:
+    EI_PASSWORD = os.environ["EI_PASSWORD"]
+except KeyError:
+    EI_PASSWORD = None
+
+try:
     API_ENDPOINT = os.environ["EI_API_ENDPOINT"]
 except KeyError:
     API_ENDPOINT = "https://studio.edgeimpulse.com/v1"
 
 try:
     INGESTION_ENDPOINT = os.environ["EI_INGESTION_ENDPOINT"]
 except KeyError:
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/data/_functions/delete.py` & `edgeimpulse-1.0.9/edgeimpulse/data/_functions/delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+# ruff: noqa: D100
 import logging
-from typing import Optional, Tuple
+from typing import Any, Optional, Tuple
 
 import edgeimpulse
 from edgeimpulse.data._functions.util import (
     get_sample_ids,
 )
 from edgeimpulse.util import (
     configure_generic_client,
@@ -16,17 +17,17 @@
 
 
 def delete_all_samples(
     category: Optional[str] = None,
     api_key: Optional[str] = None,
     timeout_sec: Optional[float] = None,
 ) -> Optional[GenericApiResponse]:
-    """
-    Deletes all samples in a given category. If category is set to `None`, all samples
-    in the project are deleted.
+    """Delete all samples in a given category.
+
+    If category is set to `None`, all samples in the project are deleted.
 
     Args:
         category (Optional[str]): Category ("training", "testing", "anomaly") from which
             the samples should be deleted. Set to 'None' to delete all samples from all
             categories.
         api_key (Optional[str]): The API key for an Edge Impulse project.
             This can also be set via the module-level variable `edgeimpulse.API_KEY`, or
@@ -35,15 +36,14 @@
 
     Raises:
         e: Unhandled exception from api
 
     Returns:
         Optional[GenericApiResponse]: API response
     """
-
     # Create API clients
     client = configure_generic_client(
         key=api_key if api_key else edgeimpulse.API_KEY,
         host=edgeimpulse.API_ENDPOINT,
     )
     raw_data_api = RawDataApi(client)
 
@@ -71,16 +71,15 @@
 
 
 def delete_sample_by_id(
     sample_id: int,
     api_key: Optional[str] = None,
     timeout_sec: Optional[float] = None,
 ) -> Optional[GenericApiResponse]:
-    """
-    Delete a particular sample from a project given the sample ID.
+    """Delete a particular sample from a project given the sample ID.
 
     Args:
         sample_id (id): ID of the sample to delete
         api_key (Optional[str]): The API key for an Edge Impulse project.
             This can also be set via the module-level variable `edgeimpulse.API_KEY`, or
             the environment variable `EI_API_KEY`.
         timeout_sec (Optional[float], optional): Optional timeout (in seconds) for API calls.
@@ -88,15 +87,14 @@
     Raises:
         e: Unhandled exception from api
 
     Returns:
         Optional[GenericApiResponse]: API response, None if no sample is found
 
     Examples:
-
         .. code-block:: python
 
             # Example of filename that has been uploaded to Studio
             filename = "my-image.01.png"
 
             # Remove extension on the filename when querying the dataset in Studio
             filename_no_ext = os.path.splitext(filename)[0]
@@ -106,15 +104,14 @@
 
             # Delete the IDs
             for info in infos:
                 resp = ei.experimental.data.delete_sample_by_id(info.sample_id)
                 if resp is None:
                     logging.warning(f"Could not delete sample {filename_no_ext}")
     """
-
     # Create API clients
     client = configure_generic_client(
         key=api_key if api_key else edgeimpulse.API_KEY,
         host=edgeimpulse.API_ENDPOINT,
     )
     raw_data_api = RawDataApi(client)
 
@@ -143,17 +140,16 @@
 
 # Delete sample from project
 def delete_samples_by_filename(
     filename: str,
     category: Optional[str] = None,
     api_key: Optional[str] = None,
     timeout_sec: Optional[float] = None,
-) -> Optional[Tuple[GenericApiResponse]]:
-    """
-    Delete any samples from an Edge Impulse project that match the given filename.
+) -> Tuple[Optional[Any], ...]:
+    """Delete any samples from an Edge Impulse project that match the given filename.
 
     Note: the `filename` argument must not include the original extension. For example,
     if you uploaded a file named `my-image.01.png`, you must provide the `filename` as
     `my-image.01`.
 
     Args:
         filename (str): Filename of the sample to delete. You should not include any
@@ -163,25 +159,27 @@
             categories.
         api_key (Optional[str]): The API key for an Edge Impulse project.
             This can also be set via the module-level variable `edgeimpulse.API_KEY`, or
             the environment variable `EI_API_KEY`.
         timeout_sec (Optional[float], optional): Optional timeout (in seconds) for API
             calls.
     """
-
     # Get list of IDs that match the given sample filename
     infos = get_sample_ids(
         filename=filename,
         category=category,
         timeout_sec=timeout_sec,
     )
 
     # Delete the IDs
     resps = []
     for info in infos:
+        if info.sample_id is None:
+            raise Exception("Can't find the id in infos")
+
         resp = delete_sample_by_id(
             sample_id=info.sample_id, api_key=api_key, timeout_sec=timeout_sec
         )
         if resp is None:
             logging.warning(f"Could not delete sample {filename}")
         resps.append(resp)
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/data/_functions/download.py` & `edgeimpulse-1.0.9/edgeimpulse/data/_functions/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# mypy: ignore-errors
+# ruff: noqa: D100
 import json
 import logging
 import os
 from io import BytesIO
 from typing import Optional, Sequence, Union, List
 from urllib.parse import urljoin
 from concurrent.futures import ThreadPoolExecutor
@@ -33,18 +35,15 @@
     session: Session,
     project_id: int,
     sample_id: int,
     api_key: str,
     endpoint: str,
     timeout_sec: Optional[float] = None,
 ) -> Optional[BytesIO]:
-    """
-    Downloads a sample by ID from an Edge Impulse project as an image.
-    """
-
+    """Download a sample by ID from an Edge Impulse project as an image."""
     data = None
 
     # Workaround: Use raw request for now
     resource_path = f"/v1/api/{project_id}/raw-data/{sample_id}/image"
     url = urljoin(endpoint, resource_path)
     headers = {
         "accept": "application/json",
@@ -65,18 +64,15 @@
     session: Session,
     project_id: int,
     sample_id: int,
     api_key: str,
     endpoint: str,
     timeout_sec: Optional[float] = None,
 ) -> Optional[BytesIO]:
-    """
-    Downloads a sample by ID from an Edge Impulse project as a video.
-    """
-
+    """Download a sample by ID from an Edge Impulse project as a video."""
     data = None
 
     # Workaround: Use raw request for now
     resource_path = f"/v1/api/{project_id}/raw-data/{sample_id}/video"
     url = urljoin(endpoint, resource_path)
     headers = {
         "accept": "application/json",
@@ -97,18 +93,15 @@
     session: Session,
     project_id: int,
     sample_id: int,
     api_key: str,
     endpoint: str,
     timeout_sec: Optional[float] = None,
 ) -> Optional[BytesIO]:
-    """
-    Downloads a sample by ID from an Edge Impulse project as a .WAV file.
-    """
-
+    """Download a sample by ID from an Edge Impulse project as a .WAV file."""
     data = None
 
     # Workaround: Use raw request for now
     resource_path = f"/v1/api/{project_id}/raw-data/{sample_id}/wav?axisIx=0"
     url = urljoin(endpoint, resource_path)
     headers = {
         "accept": "application/json",
@@ -124,18 +117,15 @@
 
     return data
 
 
 def _convert_timeseries_to_json(
     resp: dict,
 ) -> BytesIO:
-    """
-    Parse time series response from Edge Impulse API and convert to CBOR buffer.
-    """
-
+    """Parse time series response from Edge Impulse API and convert to CBOR buffer."""
     # Parse response
     data = DataAcquisition(
         protected=Protected(),
         payload=Payload(
             device_type=resp["payload"]["device_type"],
             sensors=[
                 Sensor(
@@ -161,18 +151,15 @@
     project_id: int,
     sample_id: int,
     api_key: str,
     endpoint: str,
     timeout_sec: Optional[float] = None,
     progress_callback: Optional[callable] = None,
 ) -> Optional[Sample]:
-    """
-    Downloads a sample by ID from an Edge Impulse project with progress info.
-    """
-
+    """Download a sample by ID from an Edge Impulse project with progress info."""
     # Define headers
     headers = {
         "x-api-key": api_key,
         "accept": "application/json",
         "User-Agent": get_user_agent(add_platform_info=True),
     }
 
@@ -185,15 +172,14 @@
     # Make request
     resp = session.get(url, headers=headers, timeout=timeout_sec)
     if resp.status_code != 200:
         raise HTTPError(f"HTTP error occurred: {resp.status_code} - {resp.reason}")
 
     # Convert JSON response to dictionary
     resp = resp.json()
-
     if isinstance(resp, str):
         resp = json.loads(resp)
 
     # Check for unsuccessful response
     if resp["success"] is False:
         logging.info(f"Could not get sample with ID {sample_id}")
         return None
@@ -265,22 +251,22 @@
     if data is None:
         return None
 
     # Wrap sample
     sample = Sample(
         data=data,
         filename=filename,
-        category=resp["sample"]["category"],
+        sample_id=sample_id,
         label=resp["sample"]["label"],
+        category=resp["sample"]["category"],
         bounding_boxes=resp["sample"]["boundingBoxes"],
-        metadata=resp.get("sample", {}).get("metadata", None),
-        sample_id=sample_id,
+        metadata=resp["sample"].get("metadata", None),
+        structured_labels=resp["sample"].get("structuredLabels", None),
     )
 
-    # Update progress
     if progress_callback:
         progress_callback()
 
     return sample
 
 
 def download_samples_by_ids(
@@ -288,52 +274,52 @@
     api_key: Optional[str] = None,
     timeout_sec: Optional[float] = None,
     max_workers: Optional[int] = None,
     show_progress: Optional[bool] = False,
     pool_maxsize: Optional[int] = 20,
     pool_connections: Optional[int] = 20,
 ) -> List[Sample]:
-    """
-    Downloads samples by their associated IDs from an Edge Impulse project. Downloaded
-    sample data is returned as a `DownloadSample` object, which contains the raw data in
+    """Download samples by their associated IDs from an Edge Impulse project.
+
+    Downloaded sample data is returned as a `DownloadSample` object, which contains the raw data in
     a BytesIO object along with associated metadata.
 
     **Important!** All time series data is returned as a JSON file (in BytesIO format)
     with a timestamp column. This includes files originally uploaded as CSV, JSON, and
     CBOR. Edge Impulse Studio removes the timestamp column in any uploaded CSV
     files and computes an estimated sample rate. The timestamps are computed based on
     the sample rate, will always start at 0, and will be in milliseconds. These
     timestamps may not be the same as the original timestamps in the uploaded file.
 
     Args:
         sample_ids (Union[int, Sequence[int]]): IDs of the samples to download
         api_key (Optional[str]): The API key for an Edge Impulse project.
             This can also be set via the module-level variable `edgeimpulse.API_KEY`, or
             the env var `EI_API_KEY`.
-        timeout_sec (Optional[float], optional): Number of seconds to wait for profile
+        timeout_sec (float, optional): Number of seconds to wait for profile
             job to complete on the server. `None` is considered "infinite timeout" and
             will wait forever.
-        max_workers (Optional[int]): The maximum number of subprocesses to use when
+        max_workers (int, optional): The maximum number of subprocesses to use when
             making concurrent requests. If `None`, the number of workers will be set to
             the number of processors on the machine multiplied by 5.
-        show_progress=False: Show progress bar while uploading samples.
+        show_progress: Show progress bar while uploading samples.
+        pool_maxsize: (int, optional) Maxium size of the upload pool. Defaults to 20.
+        pool_connections: (int, optional) Maxium size of the pool connections. Defaults to 20.
 
     Returns:
         List[Sample]: List of Sample objects with data and metadata as downloaded from
             the Edge Impulse project. Will be an empty list `[]` if no samples
             with the matching IDs are found.
 
     Example:
-
         .. code-block:: python
 
             sample = ei.data.download_samples_by_ids(12345)
             print(sample)
     """
-
     # Turn single or multiple IDs into list
     if isinstance(sample_ids, int):
         sample_ids = [sample_ids]
     sample_ids = list(sample_ids)
 
     # Type check to ensure all IDs are integers
     if not all(isinstance(sample_id, int) for sample_id in sample_ids):
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/data/_functions/upload.py` & `edgeimpulse-1.0.9/edgeimpulse/data/_functions/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# mypy: ignore-errors
+# ruff: noqa: D100
 from typing import Union, Optional, Sequence, List
 from urllib.parse import urljoin
 from requests import Response, Session
 from requests.adapters import HTTPAdapter
 
 from concurrent.futures import ThreadPoolExecutor
 import json
@@ -33,22 +35,26 @@
         "x-api-key": api_key,
         "x-upload-source": "EDGE_IMPULSE_PYTHON_SDK",
     }
 
     # Construct headers
     if not allow_duplicates:
         headers["x-disallow-duplicates"] = "1"
+
     if sample.label:
         headers["x-label"] = str(sample.label)
+
     if sample.bounding_boxes:
         if isinstance(sample.bounding_boxes, list):
             sample.bounding_boxes = json.dumps(sample.bounding_boxes)
         headers["x-bounding-boxes"] = sample.bounding_boxes
+
     if sample.metadata:
         headers["x-metadata"] = json.dumps(sample.metadata)
+
     if sample.category is None:
         sample.category = "split"
 
     # Construct URL
     resource_path = f"/api/{sample.category}/files"
     url = urljoin(endpoint, resource_path)
 
@@ -67,28 +73,45 @@
                     "application/cbor",
                 ),
             )
         ]
     else:
         files = [("data", (sample.filename, sample.data, "multipart/form-data"))]
 
+    if sample.structured_labels:
+        # append the structured labels to the file upload
+        structured_labels = {
+            "version": 1,
+            "type": "structured-labels",
+            "structuredLabels": {sample.filename: sample.structured_labels},
+        }
+
+        files.append(
+            (
+                "data",
+                (
+                    "structured_labels.labels",
+                    json.dumps(structured_labels),
+                    "application/json",
+                ),
+            )
+        )
+
     # Make request
     response = session.post(url, headers=headers, files=files, timeout=timeout_sec)
 
     # Call progress callback
     if progress_callback:
         progress_callback()
 
     return (response, sample)
 
 
 def _report_results(results: List[Response]) -> UploadSamplesResponse:
-    """
-    Converts http reponses to a type with success and error samples
-    """
+    """Convert http responses to a type with success and error samples."""
     successes = []
     fails = []
 
     # Sort results into successes and failures
     for result, sample in results:
         if result.status_code == 200:
             files = result.json().get("files", [])
@@ -127,16 +150,15 @@
     api_key: Optional[str] = None,
     timeout_sec: Optional[float] = None,
     max_workers: Optional[int] = None,
     show_progress: Optional[bool] = False,
     pool_maxsize: Optional[int] = 20,
     pool_connections: Optional[int] = 20,
 ) -> UploadSamplesResponse:
-    """
-    Uploads one or more samples to an Edge Impulse project using the ingestion service.
+    """Upload one or more samples to an Edge Impulse project using the ingestion service.
 
     Each sample must be wrapped in a `Sample` object, which contains metadata about that sample.
     Give this function a single `Sample` or a sequence of `Sample` objects to upload to your
     project. The `data` field of the `Sample` must be a raw binary stream, such as a BufferedIOBase
     object (which you can create with the `open(..., "rb")` function).
 
     Args:
@@ -164,15 +186,14 @@
     Returns:
         UploadSamplesResponse: A response object that contains the results of the upload. The
             response object contains two tuples: the first tuple contains the samples that were
             successfully uploaded, and the second tuple contains the samples that failed to upload
             along with the error message.
 
     Examples:
-
         .. code-block:: python
 
             # Create a dataset (with a single Sample)
             samples = (
                 Sample(
                     filename="wave.01.csv",
                     data=open("path/to/wave.01.csv", "rb"),
@@ -182,15 +203,14 @@
             )
 
             # Upload samples and print responses
             response = ei.data.upload_samples(samples)
             print(response.successes)
             print(response.fails)
     """
-
     # Turn a single sample into a 1-element list
     if isinstance(samples, Sample):
         samples = [samples]
 
     api_key = api_key if api_key is not None else ei.API_KEY
     endpoint = ei.INGESTION_ENDPOINT
     samples = list(samples)  # TODO: support iterators?
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/data/_functions/upload_files.py` & `edgeimpulse-1.0.9/edgeimpulse/data/_functions/upload_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# mypy: ignore-errors
+# ruff: noqa: D100
 from edgeimpulse.data.sample_type import Sample
 from typing import Optional
 from glob import glob
 import os
 import json
 from fnmatch import fnmatch
 import logging
@@ -23,52 +25,67 @@
     "*.cbor",
     "*.json",
     "*.csv",
     "info.labels",
 ]
 
 
+def infer_category_and_label_from_filename(sample, file) -> None:
+    """Extract label and category information from the filename and assigns them to the sample object.
+
+    Files should look like this myfiles/training/wave.1.cbor where wave is label and training is the category.
+
+    Args:
+        sample (object): The sample object to which label and category will be assigned.
+        file (str): The filename from which label and category information will be extracted.
+
+    Returns:
+        None
+    """
+    sample.label = os.path.basename(file).split(".")[0]
+    if "testing" in file:
+        sample.category = "testing"
+    elif "training" in file:
+        sample.category = "training"
+
+
 def upload_directory(
     directory: str,
-    category: str = None,
-    label: str = None,
-    metadata: dict = None,
+    category: Optional[str] = None,
+    label: Optional[str] = None,
+    metadata: Optional[dict] = None,
     transform: Optional[callable] = None,
 ) -> UploadSamplesResponse:
-    """
-    Uploads a directory of samples to Edge Impulse. The samples can be in CBOR, JSON,
-    image, or WAV file formats. You can read more about the different file formats
+    """Upload a directory of files to Edge Impulse.
+
+    The files can be in CBOR, JSON, image, or WAV file formats. You can read more about the different file formats
     accepted by the Edge Impulse ingestion service here:
+
     https://docs.edgeimpulse.com/reference/ingestion-api
 
     Args:
-        directory (str): The path to the directory containing the files to upload.
-        category (str): Category for the samples
+        directory (str): The path to the directory containing the files to upload
+        category (str): Category for the samples (train or split)
         label (str): Label for the files
-        metadata (dict): Metadatada dictionary
-        transform (Optional[Callable[[str], str]]): A function to manipulate sample before uploading
+        metadata (dict): Metadata to add to the file (visible in studio)
+        transform (callable): A function to manipulate the sample and properties before uploading
 
     Returns:
-        UploadSamplesResponse: A response object that contains the results of the upload. The
-            response object contains two tuples: the first tuple contains the samples that were
-            successfully uploaded, and the second tuple contains the samples that failed to upload
-            along with the error message.
+        UploadSamplesResponse: A response object that contains the results of the upload.
 
     Raises:
         FileNotFoundError: If the specified directory does not exist.
 
     Examples:
-
         .. code-block:: python
 
             response = ei.experimental.data.upload_directory(directory="tests/sample_data/gestures")
             self.assertEqual(len(response.successes), 8)
             self.assertEqual(len(response.fails), 0)
     """
-
     if not os.path.exists(directory) or not os.path.isdir(directory):
         raise FileNotFoundError(f"directory '{directory}' not found.")
 
     label_path = os.path.join(directory, LABEL_FILE)
     has_labels = os.path.exists(label_path)
 
     if has_labels:
@@ -83,57 +100,52 @@
             metadata=metadata,
             transform=transform,
         )
 
 
 def upload_plain_directory(
     directory: str,
-    category: str = None,
-    label: str = None,
-    metadata: dict = None,
+    category: Optional[str] = None,
+    label: Optional[str] = None,
+    metadata: Optional[dict] = None,
     transform: Optional[callable] = None,
 ) -> UploadSamplesResponse:
-    """
-    Uploads a directory of samples to Edge Impulse. The samples can be in CBOR, JSON, image, or WAV
-    file formats.
+    """Upload a directory of files to Edge Impulse.
 
-    Args:
+    The samples can be in CBOR, JSON, image, or WAV file formats.
 
+    Args:
         directory (str): The path to the directory containing the files to upload.
         category (str): Category for the samples
         label (str): Label for the files
-        metadata (dict): Metadatada dictionary
-        callback (Optional[Callable[[str], str]]): A function to manipulate sample before uploading
+        metadata (dict): Metadata to add to the file (visible in studio)
+        transform (callable): A function to manipulate the sample and properties before uploading
 
     Returns:
-        UploadSamplesResponse: A response object that contains the results of the upload. The
-            response object contains two tuples: the first tuple contains the samples that were
-            successfully uploaded, and the second tuple contains the samples that failed to upload
-            along with the error message.
+        UploadSamplesResponse: A response object that contains the results of the upload.
 
     Raises:
         FileNotFoundError: If the specified directory does not exist.
 
     Examples:
-
         .. code-block:: python
 
             response = ei.experimental.data.upload_directory(directory="tests/sample_data/gestures")
             self.assertEqual(len(response.successes), 8)
             self.assertEqual(len(response.fails), 0)
     """
     if not os.path.exists(directory) or not os.path.isdir(directory):
         raise FileNotFoundError(f"directory '{directory}' not found.")
 
     files = glob(os.path.join(directory, "**", "*"), recursive=True)
-    files = [f for f in files if os.path.isfile(f)]
+    files = [file for file in files if os.path.isfile(file)]
     files = [
-        f
-        for f in files
-        if any(fnmatch(os.path.basename(f), pattern) for pattern in ALLOWED_FILES)
+        file
+        for file in files
+        if any(fnmatch(os.path.basename(file), pattern) for pattern in ALLOWED_FILES)
     ]
 
     samples = []
     for file in files:
         sample = Sample(
             data=open(file, "rb"),
             filename=os.path.basename(file),
@@ -154,31 +166,28 @@
 
     return res
 
 
 def upload_exported_dataset(
     directory: str, transform: Optional[callable] = None
 ) -> UploadSamplesResponse:
-    """
-    Uploads samples from a downloaded Edge Impulse dataset and preserving the info.labels information.
+    """Upload samples from a downloaded Edge Impulse dataset and preserving the `info.labels` information.
+
+    Use this when you've exported your data in the studio.
 
     Args:
         directory (str): Path to the directory containing the dataset.
-        transform (Optional[callable]): A function to manipulate sample before uploading
+        transform (callable): A function to manipulate sample before uploading
 
     Returns:
-        UploadSamplesResponse: A response object that contains the results of the upload. The
-            response object contains two tuples: the first tuple contains the samples that were
-            successfully uploaded, and the second tuple contains the samples that failed to upload
-            along with the error message.
+        UploadSamplesResponse: A response object that contains the results of the upload.
 
     Raises:
         FileNotFoundError: If the labels file (info.labels) is not found in the specified directory.
     """
-
     if not os.path.exists(directory) or not os.path.isdir(directory):
         raise FileNotFoundError(f"directory '{directory}' not found.")
 
     label_path = os.path.join(directory, LABEL_FILE)
     if not os.path.exists(label_path):
         raise FileNotFoundError(
             f"Labels file '{LABEL_FILE}' not found in the specified directory."
@@ -192,19 +201,20 @@
         }
 
     samples = []
 
     for file, file_info in labels.items():
         sample = Sample(
             data=open(file, "rb"),
-            label=file_info["label"]["label"],
             bounding_boxes=file_info["boundingBoxes"],
             filename=os.path.basename(file),
+            structured_labels=file_info["label"].get("labels", None),
             metadata=file_info.get("metadata", None),
             category=file_info.get("category", None),
+            label=file_info["label"].get("label", None),
         )
 
         if transform:
             transform(sample, file)
 
         samples.append(sample)
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/data/_functions/upload_numpy.py` & `edgeimpulse-1.0.9/edgeimpulse/data/_functions/upload_numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,59 @@
+# mypy: ignore-errors
+# ruff: noqa: D100
 from edgeimpulse.data.sample_type import (
     Sample,
     DataAcquisition,
     Sensor,
     Protected,
     Payload,
     UploadSamplesResponse,
 )
 from edgeimpulse.data._functions.upload import (
     upload_samples,
 )
-from typing import Literal, Sequence
+from typing import Optional, Literal, Sequence
 import random
 import json
 from dataclasses import asdict
 
 DEVICE_TYPE = "EDGE_IMPULSE_PYTHON_SDK"
 
 
-def numpy_timeseries_to_sample(
-    values, sensors: Sequence[Sensor], sample_rate_ms: int
-) -> Sample:
-    """
-    Converts numpy values to a sample that can be uploaded to Edge Impulse
-
-    Args:
-        data (array): Numpy array containing the timeseries data. The shape should be (num_samples, time_point, num_sensors)
-        sensors (Sequence[Sensor]): List of sensor objects representing the sensors used in the data.
-        sample_rate_ms (int): Time interval in milliseconds between consecutive data points. Default is 50ms.
-
-    Returns:
-        Sample: Sample object that can be uploaded to Edge Impulse
-    """
-    data = DataAcquisition(
-        protected=Protected(),
-        payload=Payload(
-            device_type=DEVICE_TYPE,
-            interval_ms=sample_rate_ms,
-            values=values,
-            sensors=sensors,
-        ),
-    )
-    sample = Sample(
-        filename="%08x.json" % random.getrandbits(64), data=json.dumps(asdict(data))
-    )
-    return sample
-
-
 def upload_numpy(
     data,
     labels: Sequence[str],
     sensors: Sequence[Sensor],
     sample_rate_ms: int,
-    metadata: dict = None,
+    metadata: Optional[dict] = None,
     category: Literal["training", "testing", "split"] = "split",
 ) -> UploadSamplesResponse:
-    """
-    Uploads numpy arrays as timeseries using the Edge Impulse data acquisition format.
+    """Upload numpy arrays as timeseries using the Edge Impulse data acquisition format.
 
     Args:
-        data (any): Numpy array containing the timeseries data.
-            The shape should be (num_samples, time_point, num_sensors)
+        data (array): Numpy array containing the timeseries data. The shape should be (num_samples, time_point, num_sensors)
         labels (Sequence[str]): List of labels for the data samples can also be a numpy array.
         sensors (Sequence[Sensor]): List of Sensor objects representing the sensors used in the data.
         sample_rate_ms (int): Time interval in milliseconds between consecutive data points.
         metadata (dict, optional): Metadata for all samples being uploaded. Default is None.
         category (str or None, optional): Category or class label for the entire dataset. Default is split.
 
     Returns:
-        UploadSamplesResponse: A response object that contains the results of the upload. The
-            response object contains two tuples: the first tuple contains the samples that were
-            successfully uploaded, and the second tuple contains the samples that failed to upload
-            along with the error message.
+        UploadSamplesResponse: A response object that contains the results of the upload.
 
     Raises:
-        ValueError: If the length of labels doesn't match the number of samples.
-        ValueError: If the number of sensors doesn't match the number of axis in the data.
+        ValueError: If the length of labels doesn't match the number of samples or if the number of sensors
+            doesn't match the number of axis in the data.
 
     Examples:
-
         .. code-block:: python
 
             import numpy as np
             import edgeimpulse as ei
+            from ei.experimental.data import upload_numpy
 
             ei.API_KEY = "your-api-key" # set your key
 
             # Create 2 samples, each with 3 axes of accelerometer data
             samples = np.array(
                 [
                     [  # sample 1
@@ -110,15 +78,15 @@
             sensors = [
                 {"name": "accelX", "units": "ms/s"},
                 {"name": "accelY", "units": "ms/s"},
                 {"name": "accelZ", "units": "ms/s"},
             ]
 
             # Upload samples to your Edge Impulse project
-            resp = ei.experimental.data.upload_numpy(
+            resp = upload_numpy(
                 sample_rate_ms=100,
                 data=samples,
                 labels=labels,
                 category="training",
                 sensors=sensors,
             )
             print(resp)
@@ -141,7 +109,35 @@
         )
         sample.label = labels[i]
         sample.metadata = metadata
         sample.category = category
         samples.append(sample)
 
     return upload_samples(samples)
+
+
+def numpy_timeseries_to_sample(
+    values, sensors: Sequence[Sensor], sample_rate_ms: int
+) -> Sample:
+    """Convert numpy values to a sample that can be uploaded to Edge Impulse.
+
+    Args:
+        values (array): Numpy array containing the timeseries data. The shape should be (num_samples, time_point, num_sensors)
+        sensors (Sequence[Sensor]): List of sensor objects representing the sensors used in the data.
+        sample_rate_ms (int): Time interval in milliseconds between consecutive data points.
+
+    Returns:
+        Sample: Sample object that can be uploaded to Edge Impulse
+    """
+    data = DataAcquisition(
+        protected=Protected(),
+        payload=Payload(
+            device_type=DEVICE_TYPE,
+            interval_ms=sample_rate_ms,
+            values=values,
+            sensors=sensors,
+        ),
+    )
+    sample = Sample(
+        filename="%08x.json" % random.getrandbits(64), data=json.dumps(asdict(data))
+    )
+    return sample
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/data/_functions/upload_pandas.py` & `edgeimpulse-1.0.9/edgeimpulse/data/_functions/upload_pandas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# mypy: ignore-errors
+# ruff: noqa: D100
 # NOTE: We're not importing pandas here because we want to be compatible with pandas like
 # frameworks. I.e. Dask, Modin, Polars etc.
 # Please try to rely on duck typing where possible and don't make any dependencies towards
 # specific frameworks
 #
 # In the end we'll adopt something like this https://data-apis.org/dataframe-protocol/latest/purpose_and_scope.html
 
@@ -24,70 +26,63 @@
 MSG_NO_DF_MODULE = (
     "DataFrame methods on input object not found. DataFrame support "
     "requires pandas (or similar) to be installed."
 )
 
 
 def row_metadata(row, metadata_col):
-    """
-    Get the metadata from a dataframe row for a single sample.
-    """
+    """Get the metadata from a dataframe row for a single sample."""
     metadata = None
     if metadata_col is not None:
         metadata = {k: str(row[k]) for k in metadata_col}
     return metadata
 
 
 def ts_to_ms(timestamp):
-    """
-    Helper to convert timestamps to miliseconds for the EI data aquisition format
-    """
+    """Convert timestamps to milliseconds for the EI data aquisition format."""
     if isinstance(timestamp, (int, float)):
         return int(timestamp * 1000)
     elif hasattr(timestamp, "timestamp"):
         return int(timestamp.timestamp() * 1000)
     else:
         raise Exception(f"Error: Unsupported timestamp format - {type(timestamp)}")
 
 
 def upload_pandas_sample(
     df,
-    label: str = None,
-    sample_rate_ms: int = None,
-    filename: str = None,
+    label: Optional[str] = None,
+    sample_rate_ms: Optional[int] = None,
+    filename: Optional[str] = None,
     axis_columns: Optional[List[str]] = None,
     metadata: Optional[dict] = None,
     category: Literal["training", "testing", "split"] = "split",
 ) -> UploadSamplesResponse:
-    """
-    Upload a single dataframe sample.
+    """Upload a single dataframe sample.
+
+    Upload a single dataframe sample to Edge Impulse.
 
     Args:
         df (DataFrame): The input DataFrame containing data.
         label (str, optional): The label for the sample. Default is None.
         sample_rate_ms (int, optional): The sampling rate of the time series data (in milliseconds)
         filename (str, optional): The filename for the sample. Default is None.
         axis_columns (List[str], optional): List of column names representing axis if the data is
             multi-dimensional. Default is None.
         metadata (dict, optional): Dictionary containing metadata information. Default is None.
         category (str or None, optional): Category or class label for the entire dataset. Default is split.
 
     Returns:
-        UploadSamplesResponse: A response object that contains the results of the upload. The
-            response object contains two tuples: the first tuple contains the samples that were
-            successfully uploaded, and the second tuple contains the samples that failed to upload
-            along with the error message.
+        UploadSamplesResponse: A response object that contains the results of the upload.
 
     Raises:
         AttributeError: If the input object does not have a `reset_index` method.
         ValueError: If the `axis_columns` argument is not a list of strings or if the `metadata`
             argument is not a dictionary.
 
     Examples:
-
         .. code-block:: python
 
             import edgeimpulse as ei
             ei.API_KEY = "your-api-key" # set your key
 
             # Uncomment one of the following
             # import pandas as pd
@@ -142,40 +137,37 @@
     sample_rate_ms: Optional[int] = None,
     label: Optional[str] = None,
     filename: Optional[str] = None,
     axis_columns: Optional[List[str]] = None,
     metadata: Optional[dict] = None,
     category: Literal["training", "testing", "split"] = "split",
 ) -> Sample:
-    """
-    Converts a dataframe to a single sample. Can both handle timeseries and non-timeseries data.
+    """Convert a dataframe to a single sample. Can handle both *timeseries* and *non-timeseries* data.
 
-    In order to be a determiend to be a timeseries it must have:
+    In order to be inferred as timeseries it must have:
 
     - More than one row
     - A sample rate or an index from which the sample rate can be inferred
-        - Therefore must be monotonically inreasing
+        - Therefore must be monotonically increasing
         - And int or a date
 
     Args:
         df (DataFrame): The input DataFrame containing data.
         sample_rate_ms (int): The sampling rate of the time series data (in milliseconds).
         label (str, optional): The label for the sample. Default is None.
         filename (str, optional): The filename for the sample. Default is None.
-        axis_columns (List[str], optional): List of column names representing axis if the data is
-            multi-dimensional. Default is None.
-        metadata (dict, optional): Dictionary containing metadata information. Default is None.
-        category (str or None, optional): Category or class label for the entire dataset. Default is split.
+        axis_columns (List[str], optional): List of column names representing axis if the data is multi-dimensional. Default is None.
+        metadata (dict, optional): Dictionary containing metadata information for the sample. Default is None.
+        category (str or None, optional): To which category this sample belongs (training/testing/split) default is spit.
 
     Returns:
         Sample: A sample object containing the data from the dataframe.
     """
-
     # Check to make sure dataframe operations are supported
-    if not hasattr(df, "reset_index") or not callable(getattr(df, "reset_index")):
+    if not hasattr(df, "reset_index") or not callable(df.reset_index):
         raise AttributeError(MSG_NO_DF_MODULE)
 
     if axis_columns is not None:
         if not isinstance(axis_columns, list) or not all(
             isinstance(col, str) for col in axis_columns
         ):
             raise ValueError("The 'axis_columns' argument must be a list of strings.")
@@ -200,30 +192,30 @@
             df.reset_index(drop=True, inplace=True)
             df.index = df.index * int(sample_rate_ms)
         else:
             logging.debug("Trying to infer sample rate")
 
             if not hasattr(df.index, "is_monotonic_increasing"):
                 raise ValueError(
-                    "Index should be monotonicly increasing in order to detect sample rate. Or specify sample_rate_ms argument."
+                    "Index should be monotonically increasing in order to detect sample rate. Or specify sample_rate_ms argument."
                 )
 
             if hasattr(df.index, "seconds"):
                 # the csv ingestion services requires the timestamp to be specified
                 # in milliseconds. See here: https://docs.edgeimpulse.com/reference/importing-csv-data
                 # So here we convert the index when its timedelta index.
-                # Because we're duck typeing we can't check for
+                # Because we're duck typing we can't check for
                 # explicit TimeDeltaIndex
                 df.index = df.index.seconds * 1000
             else:
                 # Must be a normal range based index, so we can use that.
                 pass
 
     # We convert here to a csv since its a little bit more easy to use than the JSON ei data
-    # We don't need sensors here (they are automatically infered)
+    # We don't need sensors here (they are automatically inferred)
     # And we can both support timeseries and non-time series.
 
     csv = io.StringIO()
     df.to_csv(csv, index=is_time_series, index_label="timestamp")
 
     # Print the first 2000 characters of the csv to the log
     max_chars = 2000
@@ -253,53 +245,44 @@
 
 def upload_pandas_dataframe_wide(
     df,
     sample_rate_ms: int,
     data_col_start: Optional[int] = None,
     label_col: Optional[str] = None,
     category_col: Optional[str] = None,
-    metadata_cols: List[str] = None,
+    metadata_cols: Optional[List[str]] = None,
     data_col_length: Optional[int] = None,
-    data_axis_cols: List[str] = None,
+    data_axis_cols: Optional[List[str]] = None,
 ) -> UploadSamplesResponse:
-    """
-    Uploads a dataframe to Edge Impulse where each of columns represent a value in the
-    timeseries data and the rows become the individual samples.
+    """Upload a dataframe to Edge Impulse where each of columns represent a value in the timeseries data and the rows become the individual samples.
 
     Args:
-        df (DataFrame):
-            The input DataFrame containing time series data.
-        data_col_start (int):
-            The index of the column from which the time series data begins.
-        sample_rate_ms (int):
-            The sampling rate of the time series data (in milliseconds).
+        df (DataFrame): The input DataFrame containing time series data.
+        data_col_start (int): The index of the column from which the time series data begins.
+        sample_rate_ms (int): The sampling rate of the time series data (in milliseconds).
         label_col (str, optional): The column name containing labels for each
             time series. Default is None.
         category_col (str, optional): The column name containing the category for the
             data. Default is None.
         metadata_cols (List[str], optional): List of column names containing metadata
             information. Default is None.
         data_col_length (int, optional): The number of columns that represent a single
             time series. Default is None.
         data_axis_cols (List[str], optional): List of column names representing axis if the data is
             multi-dimensional. Default is None.
 
     Returns:
-        UploadSamplesResponse: A response object that contains the results of the upload. The
-            response object contains two tuples: the first tuple contains the samples that were
-            successfully uploaded, and the second tuple contains the samples that failed to upload
-            along with the error message.
+        UploadSamplesResponse: A response object that contains the results of the upload.
 
     Raises:
         AttributeError: If the input object does not have a `iterrows` method.
         ValueError: If the `data_col_length` argument is not an integer or if the `data_col_start`
             argument is not an integer.
 
     Examples:
-
         .. code-block:: python
 
             import edgeimpulse as ei
             ei.API_KEY = "your-api-key" # set your key
 
             # Uncomment one of the following
             # import pandas as pd
@@ -319,27 +302,26 @@
                 df,
                 label_col="label",
                 metadata_col=["id"],
                 data_col_start=2,
                 sample_rate_ms=100,
             )
             self.assertEqual(len(response.successes), 2)
-            self.assertEqual(len(resonse.fails), 0)
+            self.assertEqual(len(response.fails), 0)
     """
-
     # Check to make sure dataframe operations are supported
-    if not hasattr(df, "iterrows") or not callable(getattr(df, "iterrows")):
+    if not hasattr(df, "iterrows") or not callable(df.iterrows):
         raise AttributeError(MSG_NO_DF_MODULE)
 
     samples = []
     is_single_axis = data_axis_cols is None
     if is_single_axis:
         for _, row in df.iterrows():
             # We need to transpose the single wide row to a timeseries long dataframe
-            # We reset the index in order to make it compatible. After toframe, the column names are the index
+            # We reset the index in order to make it compatible. After to frame, the column names are the index
             # so if that is text it will break the upload
 
             row_df = row[data_col_start:].to_frame()  # transforms from wide to long.
             row_df.reset_index(
                 drop=True, inplace=True
             )  # the index becomes to column names so lets drop them and convert to a standard range
 
@@ -398,39 +380,34 @@
 
     return upload_samples(samples)
 
 
 def upload_pandas_dataframe(
     df,
     feature_cols: List[str],
-    label_col: str = None,
+    label_col: Optional[str] = None,
     category_col: Optional[str] = None,
     metadata_cols: Optional[List[str]] = None,
 ) -> UploadSamplesResponse:
-    """
-    Upload non-timeseries data to Edge Impulse where each dataframe row becomes a sample.
+    """Upload non-timeseries data to Edge Impulse where each dataframe row becomes a sample.
 
     Args:
         df (dataframe): The DataFrame to be uploaded.
         feature_cols (List[str]): A list of column names containing features
         label_col (str, optional): The name of the column containing labels for the data.
         category_col (str, optional): The name of the column containing the category for the data.
         metadata_cols (List[str], optional): Optional list of column names containing metadata
 
     Returns:
-        UploadSamplesResponse: A response object that contains the results of the upload. The
-            response object contains two tuples: the first tuple contains the samples that were
-            successfully uploaded, and the second tuple contains the samples that failed to upload
-            along with the error message.
+        UploadSamplesResponse: A response object that contains the results of the upload.
 
     Raises:
         AttributeError: If the input object does not have a `iterrows` method.
 
     Examples:
-
         .. code-block:: python
 
             import edgeimpulse as ei
             ei.API_KEY = "your-api-key" # set your key
 
             # Uncomment one of the following
             # import pandas as pd
@@ -453,17 +430,16 @@
                 feature_col=["accX", "accY", "accZ"],
                 label_col="label",
                 category_col="category",
                 metadata_col=["loc"],
             )
             assert len(response.fails) == 0, "Could not upload some files"
     """
-
     # Check to make sure dataframe operations are supported
-    if not hasattr(df, "iterrows") or not callable(getattr(df, "iterrows")):
+    if not hasattr(df, "iterrows") or not callable(df.iterrows):
         raise AttributeError(MSG_NO_DF_MODULE)
 
     samples = []
     for index, row in df.iterrows():
         row_df = row.to_frame().transpose()[feature_cols]
         sample = pandas_dataframe_to_sample(row_df)
 
@@ -481,39 +457,39 @@
     timestamp_col: str,
     group_by: str,
     feature_cols: List[str],
     label_col: Optional[str] = None,
     category_col: Optional[str] = None,
     metadata_cols: Optional[List[str]] = None,
 ) -> UploadSamplesResponse:
-    """
-    Uploads a dataframe where the rows contain multiple samples and timeseries data for
-    those samples. It uses a `group_by` in order to detect what timeseries value belongs
+    """Upload a dataframe where the rows contain multiple samples and timeseries data for those samples.
+
+    It uses a `group_by` in order to detect what timeseries value belongs
     to which sample.
 
     Args:
-        df (dataframe): The DataFrame to be uploaded.
-        timestamp_col (str): The name of the column containing the timestamp for the data (in seconds).
-        group_by (str): The name of the column containing the group for the data.
-        feature_cols (List[str]): A list of column names containing features.
+        df (dataframe):
+            The DataFrame to be uploaded.
+        timestamp_col (str):
+            The name of the column containing the timestamp for the data (in seconds).
+        group_by (str):
+            The name of the column containing the group for the data.
+        feature_cols (List[str]):
+            A list of column names containing features.
         label_col (str, optional): The name of the column containing labels for the data. Each group
             must have the same label. Default is None (derived from group name).
         category_col (str, optional): The name of the column containing the category for the data.
             Each group must have the same category. Default is None (random training/test split).
         metadata_cols (List[str], optional): A list of column names containing metadata information.
             Each group must have the same metadata. Default is None.
 
     Returns:
-        UploadSamplesResponse: A response object that contains the results of the upload. The
-            response object contains two tuples: the first tuple contains the samples that were
-            successfully uploaded, and the second tuple contains the samples that failed to upload
-            along with the error message.
+        UploadSamplesResponse: A response object that contains the results of the upload.
 
     Examples:
-
         .. code-block:: python
 
             import edgeimpulse as ei
             ei.API_KEY = "your-api-key" # set your key
 
             # Uncomment one of the following
             # import pandas as pd
@@ -545,19 +521,16 @@
                 feature_cols=["accX", "accY", "accZ"],
                 label_col="label",
                 category_col="category",
                 metadata_cols=["loc"]
             )
             assert len(response.fails) == 0, "Could not upload some files"
     """
-
     # Check to make sure dataframe operations are supported
-    if not hasattr(df[timestamp_col], "apply") or not callable(
-        getattr(df[timestamp_col], "apply")
-    ):
+    if not hasattr(df[timestamp_col], "apply") or not callable(df[timestamp_col].apply):
         raise AttributeError(MSG_NO_DF_MODULE)
 
     samples = []
     df[timestamp_col] = df[timestamp_col].apply(ts_to_ms)
     groups = df[group_by].unique()
 
     for group in groups:
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/data/_functions/util.py` & `edgeimpulse-1.0.9/edgeimpulse/data/_functions/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# mypy: ignore-errors
+"""Use this module to do various tasks within Edge Impulse SDK."""
 import json
 import logging
 import math
 from typing import Optional, List
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 import edgeimpulse
@@ -18,17 +20,15 @@
 
 
 def get_filename_by_id(
     sample_id: int,
     api_key: Optional[str] = None,
     timeout_sec: Optional[float] = None,
 ) -> Optional[str]:
-    """
-    Given an ID for a sample in a project, return the filename associated with that
-    sample.
+    """Given an ID for a sample in a project, return the filename associated with that sample.
 
     Note that while multiple samples can have the same filename, each sample has a
     unique sample ID that is provided by Studio when the sample is uploaded.
 
     Args:
         sample_id (int): Sample ID to look up
         api_key (Optional[str]): The API key for an Edge Impulse project.
@@ -39,15 +39,14 @@
     Raises:
         e: Unhandled exception from api
 
     Returns:
         Optional[str]: Filename (string) if sample is found. None if no sample is found
             matching the ID given.
     """
-
     # Create API clients
     client = configure_generic_client(
         key=api_key if api_key else edgeimpulse.API_KEY,
         host=edgeimpulse.API_ENDPOINT,
     )
     raw_data_api = RawDataApi(client)
 
@@ -83,18 +82,15 @@
     labels: List[str],
     filename: str,
     offset: int,
     samples_per_thread: int,
     chunk_size: int = 1000,
     timeout_sec=None,
 ):
-    """
-    Make API calls to get sample info from a project
-    """
-
+    """Make API calls to get sample info from a project."""
     # Determine how many times to make API call
     num_chunks = int(math.ceil(samples_per_thread / chunk_size))
 
     # Make API calls to list sample information
     resps = []
     for i in range(num_chunks):
         # Determine offset and limit for this chunk
@@ -134,22 +130,20 @@
     filename: Optional[str] = None,
     category: Optional[str] = None,
     labels: Optional[str] = None,
     api_key: Optional[str] = None,
     num_workers: Optional[int] = 4,
     timeout_sec: Optional[float] = None,
 ) -> List[SampleInfo]:
-    """
-    Get the sample IDs and filenames for all samples in a project, filtered by category,
-    labels, and/or filename.
+    """Get the sample IDs and filenames for all samples in a project, filtered by category, labels, and/or filename.
 
     Note that filenames are given by the root of the filename when uploaded.
     For example, if you upload `my-image.01.png`, it will be stored in your project with
     a hash, such as `my-image.01.png.4f262n1b.json`. To find the ID(s) that match this
-    sample, you must provide the argument `filename=my-image.01`. Notic the lack of
+    sample, you must provide the argument `filename=my-image.01`. Notice the lack of
     extension and hash.
 
     Because of the possibility for multiple samples (i.e. different sample IDs) with the
     same filename, we recommend providing unique filenames for your samples when
     uploading.
 
     Args:
@@ -172,15 +166,14 @@
     Raises:
         e: Unhandled exception from api
 
     Returns:
         List[SampleInfo]: List of `SampleInfo` objects containing the sample ID,
             filename, category, and label for each sample matching the criteria given.
     """
-
     # Recursively get info from all categories if no category given
     if category == "all" or category is None:
         resp_samples = []
         for category in edgeimpulse.util.DATA_CATEGORIES:
             resp_samples.extend(
                 get_sample_ids(
                     category=category,
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/data/sample_type.py` & `edgeimpulse-1.0.9/edgeimpulse/data/sample_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+# ruff: noqa: D100, D101
 from dataclasses import dataclass
-from io import BufferedIOBase
-from typing import Optional, Sequence, Literal, List
+from io import BufferedIOBase, StringIO
+from typing import Optional, Sequence, Literal, List, Union
 
 
 @dataclass
 class Sensor:
-    """
-    Represents a sensor in the Edge Impulse data acquisition format.
+    """Represents a sensor in the Edge Impulse data acquisition format.
 
     Note:
         The units must comply with the SenML units list:
         https://www.iana.org/assignments/senml/senml.xhtml
 
     Attributes:
         name (str): Name of the sensor.
@@ -94,17 +94,17 @@
         "NTU",
         "rgba",
     ] = "m/s"
 
 
 @dataclass
 class Payload:
-    """
-    Wrapper class for the sensor data. Information about the data acquisition format
-    can be found here: https://docs.edgeimpulse.com/reference/data-acquisition-format
+    """Wrapper class for the sensor data.
+
+    Information about the data acquisition format can be found here: https://docs.edgeimpulse.com/reference/data-acquisition-format.
 
     Attributes:
         device_type (str): - Device type, for example the exact model of the device.
             Should be the same for all similar devices. For example
             "DISCO-L475VG-IOT01A"
         sensors (List[Sensor]): List of Sensor objects representing the data acquisition
             sensors, such as `"accX"`, `"accY"`, `"accZ"` for a three-axis
@@ -114,15 +114,14 @@
         interval_ms (Optional[int]): Interval in milliseconds between data samples.
             Default is 0.
         device_name (Optional[str]): Unique identifier for this device. Only set this
             when the device has a globally unique identifier (e.g. MAC address). If this
             field is set the device shows up on the 'Devices' page in the studio.
 
     Example:
-
         .. code-block:: python
 
             from edgeimpulse.data.sample_type import Payload, Sensor
 
             payload = Payload(
                 device_type="DISCO-L475VG-IOT01A",
                 sensors=[
@@ -138,35 +137,34 @@
                 ],
                 interval_ms=10,
                 device_name="ac:87:a3:0a:2d:1b"
             )
     """
 
     device_type: str
-    sensors: List[Sensor]
-    values: List[List[float]]
+    sensors: Sequence[Sensor]
+    values: Sequence[Sequence[float]]
     interval_ms: Optional[int] = 0
     device_name: Optional[str] = None
 
 
 @dataclass
 class Protected:
-    """
-    Wrapper class for information about the signature format. More information can be
-    found here: https://docs.edgeimpulse.com/reference/data-acquisition-format
+    """Wrapper class for information about the signature format.
+
+    More information can be found here: https://docs.edgeimpulse.com/reference/data-acquisition-format.
 
     Attributes:
         ver (str): Version of the signature format. Default is `"v1"`.
         alg (str): Algorithm used to generate the signature. Default is `"none"`.
         iat (Optional[int]): Date and time when the file was created in seconds since
             epoch. Only set this when the device creating the file has an accurate
             clock. Default is `None`.
 
     Example:
-
         .. code-block:: python
 
             from edgeimpulse.data.sample_type import Protected
 
             protected = Protected(
                 ver="v1",
                 alg="none",
@@ -177,35 +175,35 @@
     ver: str = "v1"
     alg: Literal["HS256", "none"] = "none"
     iat: Optional[int] = None
 
 
 @dataclass
 class DataAcquisition:
-    """
-    Wrapper class for the Edge Impulse data acquisition format. See here for more
-    information: https://docs.edgeimpulse.com/reference/data-acquisition-format
+    """Wrapper class for the Edge Impulse data acquisition format.
+
+    See here for more information: https://docs.edgeimpulse.com/reference/data-acquisition-format.
 
     Attributes:
         protected (Protected): Information about the signature format.
         payload (Payload): Sensor data.
         signature (Optional[str]): Cryptographic signature of the data. Default is
             `None`.
     """
 
     protected: Protected
     payload: Payload
-    signature: str = None
+    signature: Optional[str] = None
 
 
 @dataclass
 class Sample:
-    """
-    Wrapper class for sample data, labels, and associated metadata. Sample data should be contained
-    in a file or file-like object, for example, as the return from `open(..., "rb")`. The
+    """Wrapper class for sample data, labels, and associated metadata.
+
+    Sample data should be contained in a file or file-like object, for example, as the return from `open(..., "rb")`. The
     `upload_samples()` function expects Sample objects as input.
 
     Attributes:
         filename (str): Name to give the sample when stored in the Edge Impulse project
         data (BufferedIOBase): IO stream of data to be read during the upload process. This can be
             a BytesIO object, such as the return from `open(..., "rb")`.
         category (Optional[Literal["training", "testing", "anomaly", "split"]]): Which dataset to
@@ -220,39 +218,44 @@
             format bounding box dictionaries.
         metadata (Optional[dict]): Dictionary of optional metadata that you would like to include
             for your particular sample (example: `{"source": "microphone", "timestamp": "120"}`)
         sample_id (Optional[int]): Unique ID of the sample. This is automatically assigned by the
             Edge Impulse server when the sample is uploaded. You can use this ID to retrieve the
             sample later. This value is ignored when uploading samples and should not be set by the
             user.
+        structured_labels (Optional[Sequence[dict]]): Array of dictionary objects that define the labels
+            in this sample at various intervals.
+            <https://edge-impulse.gitbook.io/docs/edge-impulse-studio/data-acquisition/multi-label>`_ to
+            read more. Example: `[{"label": "noise","startIndex": 0,"endIndex": 5000},
+            {"label": "water","startIndex": 5000,"endIndex": 10000}]`
+
     """
 
-    data: BufferedIOBase
+    data: Union[BufferedIOBase, StringIO, str]
     filename: Optional[str] = None
     category: Optional[Literal["training", "testing", "anomaly", "split"]] = "split"
     label: Optional[str] = None
     bounding_boxes: Optional[Sequence[dict]] = None
     metadata: Optional[dict] = None
     sample_id: Optional[int] = None
+    structured_labels: Optional[Sequence[dict]] = None
 
 
 class SampleIngestionResponse:
     def __init__(
         self,
         sample: Sample,
         response: dict,
     ):
-        """
-        Wrapper for the response from the Edge Impulse ingestion service when uploading
-        a sample along with the sample that was uploaded.
+        """Wrapper for the response from the Edge Impulse ingestion service when uploading a sample along with the sample that was uploaded.
 
         Args:
             sample (Sample): The sample that was uploaded.
             response (dict): The response from the server.
-        """
+        """  # noqa: D401
         self.sample = sample
         self.success = False
         self.error = None
         self.sample_id = None
         self.project_id = None
         self.filename = None
 
@@ -265,16 +268,15 @@
             self.sample_id = response["sampleId"]
         if "projectId" in response:
             self.project_id = response["projectId"]
         if "fileName" in response:
             self.filename = response["fileName"]
 
     def __repr__(self) -> str:
-        """
-        Returns a string providing an overview of the response.
+        """Return a string providing an overview of the response.
 
         Returns:
             str: Response from the server.
         """
         msg = f"SampleIngestionResponse(success={self.success}, error={self.error}, "
         msg += f"sampleId={self.sample_id}, projectId={self.project_id}, "
         msg += f"fileName={self.filename}, sample={self.sample})"
@@ -284,50 +286,45 @@
 
 class UploadSamplesResponse:
     def __init__(
         self,
         successes: List[SampleIngestionResponse],
         fails: List[SampleIngestionResponse],
     ):
-        """
-        Response from the Edge Impulse server when uploading multiple samples.
+        """Response from the Edge Impulse server when uploading multiple samples.
 
         Args:
             success (bool): `True` if all samples were uploaded successfully.
             successes (List[SampleIngestionResponse]): List of
                 SampleIngestionResponse objects for each sample that were successfully
                 uploaded.
             fails (List[SampleIngestionResponse]): List of SampleIngestionResponse
                 objects for each sample that failed to upload.
         """
         self.successes = successes
         self.fails = fails
         self.success = len(fails) == 0
 
     def __repr__(self) -> str:
-        """
-        Returns a string providing an overview of the number of successes and fails from
-        the responses.
+        """Return a string providing an overview of the number of successes and fails from the responses.
 
         Returns:
             str: Successful upload along with number of successes and fails.
         """
         msg = "UploadSamplesResponse\r\n"
         msg += f"  success: {self.success}\r\n"
         msg += f"  number of successes: {len(self.successes)}\r\n"
         msg += f"  number of fails: {len(self.fails)}"
 
         return msg
 
 
 @dataclass
 class SampleInfo:
-    """
-    Wrapper for the response from the Edge Impulse ingestion service when retrieving
-    sample information.
+    """Wrapper for the response from the Edge Impulse ingestion service when retrieving sample information.
 
     Attributes:
         sample_id (Optional[int]): The sample ID.
         filename (Optional[str]): The filename of the sample.
         category (Optional[str]): The category of the sample.
         label (Optional[str]): The label of the sample.
     """
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/exceptions.py` & `edgeimpulse-1.0.9/edgeimpulse/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# ruff: noqa: D100, D101, D107
 from typing import List, Optional
 
 
 class EdgeImpulseException(Exception):
     def __init__(self, message):
         super().__init__(
             message
@@ -9,47 +10,47 @@
             + " or ask a question at https://forum.edgeimpulse.com/"
         )
 
 
 class InvalidDeviceException(EdgeImpulseException):
     """Exception raised when an invalid device is passed.
 
-    Atrributes:
+    Attributes:
         device (str): device type to profile
         profile devices (List[str]): List of devices for a project as strings.
 
     """
 
     def __init__(self, device: str, profile_devices: List[str]):
         self.device = device
         self.profile_devices = profile_devices
         self.message = f"Invalid device: [{device}] valid types are: {profile_devices}"
         super().__init__(self.message)
 
 
 class InvalidTargetException(EdgeImpulseException):
-    """
-        Exception raised when an invalid target is passed.
-        For a list of valid targets use `edgeimpulse.model.list_deployment_targets()`.
+    """Exception raised when an invalid target is passed.
+
+    For a list of valid targets use `edgeimpulse.model.list_deployment_targets()`.
 
-    Atrributes:
+    Attributes:
         deploy_target (str): Target to deploy to.
         target_names (List[str]): List of targets for a project as strings.
     """
 
     def __init__(self, deploy_target: str, target_names: List[str]):
         self.deploy_target = deploy_target
         self.target_names = target_names
         self.message = f"deploy_target: [{deploy_target}] not in {target_names}"
         super().__init__(self.message)
 
 
 class InvalidEngineException(EdgeImpulseException):
-    """
-    Exception raised when an invalid engine is passed.
+    """Exception raised when an invalid engine is passed.
+
     For a list of valid engines use `edgeimpulse.model.list_engines()`.
 
     """
 
     def __init__(self, validation_error):
         super().__init__(str(validation_error))
 
@@ -92,27 +93,22 @@
                 if error is not None
                 else "There was no error message included."
             )
         )
 
 
 class TimeoutException(EdgeImpulseException):
-    """
-    Exception raised when a timeout has been reached.
-    """
+    """Exception raised when a timeout has been reached."""
 
     def __init__(self, msg: str):
         super().__init__(msg)
 
 
 class UnsupportedSampleType(EdgeImpulseException):
-    """
-    Exception raised when attempting to upload or download a data type that is
-    not supported by Edge Impulse.
-    """
+    """Exception raised when attempting to upload or download a data type that is not supported by Edge Impulse."""
 
     def __init__(self, error: Optional[str]):
         self.error = error
         super().__init__(
             (
                 "Unsupported sample type. See here to learn more about the "
                 "supported sample types: "
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/experimental/data/__init__.py` & `edgeimpulse-1.0.9/edgeimpulse/experimental/data/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+"""Use this module to upload data to Edge Impulse."""
 from edgeimpulse.data._functions.delete import (
     delete_all_samples,
     delete_sample_by_id,
     delete_samples_by_filename,
 )
 
 from edgeimpulse.data._functions.download import (
     download_samples_by_ids,
 )
 
 from edgeimpulse.data._functions.upload_files import (
     upload_plain_directory,
     upload_exported_dataset,
     upload_directory,
+    infer_category_and_label_from_filename,
 )
 
 from edgeimpulse.data._functions.upload import upload_samples
 
 from edgeimpulse.data._functions.upload_pandas import (
     upload_pandas_dataframe,
     upload_pandas_dataframe_wide,
@@ -50,9 +52,10 @@
     "upload_pandas_dataframe_wide",
     "upload_pandas_sample",
     "upload_pandas_dataframe_with_group",
     "pandas_dataframe_to_sample",
     "upload_numpy",
     "numpy_timeseries_to_sample",
     "download_samples_by_ids",
+    "infer_category_and_label_from_filename",
     "Sample",
 ]
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/model/_functions/deploy.py` & `edgeimpulse-1.0.9/edgeimpulse/model/_functions/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     deploy_model_type: Optional[str] = None,
     engine: str = "tflite",
     deploy_target: str = "zip",
     output_directory: Optional[str] = None,
     api_key: Optional[str] = None,
     timeout_sec: Optional[float] = None,
 ) -> io.BytesIO:
-    """Transforms a machine learning model into a library for an edge device
+    """Transform a machine learning model into a library for an edge device.
 
     Transforms a trained model into a library, package, or firmware ready to deploy on an embedded
     device. Can optionally apply post-training quantization if a representative data sample is
     uploaded.
 
     Supported model formats:
 
@@ -93,15 +93,15 @@
     not deploy: deploy_target: ...`.
 
     Args:
         model (Union[Path, str, bytes, Any]): A machine learning model, or similarly represented
             computational graph. Can be `Path` or `str` denoting file path, Python `bytes`
             containing a model, or a Keras model instance.
         model_output_type (Union[Classification, Regression, ObjectDetection]): Describe your
-            model's type:Classification, Regression, or ObjectDetection. The types are available in
+            model's type: Classification, Regression, or ObjectDetection. The types are available in
             the module `edgeimpulse.model.output_type`.
         model_input_type (Union[ImageInput, AudioInput, TimeSeriesInput, OtherInput], optional):
             Determines any input preprocessing (windowing, downsampling) that should be performed by
             the resulting library. The types are available in `edgeimpulse.model.input_type`. The
             default is `OtherInput` (no preprocessing).
         representative_data_for_quantization: A numpy representative input dataset. Accepts either
             an in memory numpy array or the Path/str filename of a np.save .npy file.
@@ -131,15 +131,14 @@
         InvalidEngineException: Unacceptable engine for this target.
         InvalidTargetException: Unacceptable deploy_target for this project.
         FileNotFoundError: Model file could not be loaded.
         TimeoutException: Timeout waiting for result
         Exception: Unhandled exception from API
 
     Examples:
-
         .. code-block:: python
 
             # Turn a Keras model into a C++ library and write to disk
             ei.model.deploy(model=keras_model,
                             model_output_type=ei.model.output_type.Classification(),
                             model_input_type=ei.model.input_type.OtherInput(),
                             output_directory=".")
@@ -161,15 +160,14 @@
             # The function returns a BytesIO which can be written as desired
             output = ei.model.deploy(model=keras_model,
                                      model_output_type=ei.model.output_type.Classification())
             with open('destination.zip', 'wb') as f:
                 f.write(output.read())
 
     """
-
     if model_input_type is None:
         model_input_type = OtherInput()
 
     if deploy_model_type is not None and deploy_model_type not in list_model_types():
         raise InvalidDeployParameterException(
             "deploy_model_type must be None, or one of the following:\n"
             f"{list_model_types()}\n"
@@ -317,18 +315,16 @@
         except Exception as e:
             logging.debug(f"Exception saving output to '{output_path}' [{str(e)}]")
             raise e
 
     return io.BytesIO(response.data)
 
 
-def list_deployment_targets(api_key: Optional[str] = None) -> "List[str]":
-    """
-    Lists suitable deployment targets for the project associated with configured or provided api
-    key.
+def list_deployment_targets(api_key: Optional[str] = None) -> List[str]:
+    """List suitable deployment targets for the project associated with configured or provided api key.
 
     Args:
         api_key (str, optional): The API key for an Edge Impulse project.
             This can also be set via the module-level variable `edgeimpulse.API_KEY`, or the env var
             `EI_API_KEY`.
 
     Returns:
@@ -338,26 +334,25 @@
     client = configure_generic_client(
         key=api_key if api_key else edgeimpulse.API_KEY,
         host=edgeimpulse.API_ENDPOINT,
     )
     return get_project_deploy_targets(client)
 
 
-def list_engines() -> "List[str]":
-    """Lists all the engines that can be passed to `deploy()`'s `engine` parameter.
+def list_engines() -> List[str]:
+    """List all the engines that can be passed to `deploy()`'s `engine` parameter.
 
     Returns:
         List[str]: List of engines
-
     """
     return [e.value for e in DeploymentTargetEngine]
 
 
-def list_model_types() -> "List[str]":
-    """Lists all the model types that can passed to `deploy()`'s `deploy_model_type` parameter.
+def list_model_types() -> List[str]:
+    """List all the model types that can passed to `deploy()`'s `deploy_model_type` parameter.
 
     Returns:
         List[str]: List of model types
 
     """
     return [t.value for t in KerasModelTypeEnum]
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/model/_functions/profile.py` & `edgeimpulse-1.0.9/edgeimpulse/model/_functions/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: ignore-errors
 import logging
 import json
 from pathlib import Path
 from typing import Union, Optional, Any, List
 import tempfile
 
 import edgeimpulse
@@ -23,15 +24,15 @@
     LearnApi,
     GetPretrainedModelResponse,
 )
 
 
 class ProfileResponse(GetPretrainedModelResponse):
     def summary(self) -> None:
-        """Returns a summary of the profiling results"""
+        """Return a summary of the profiling results."""
         output = []
         if self.specific_device_selected and self.model and self.model.profile_info:
             if self.model.profile_info.float32:
                 output.append("Target results for float32:")
                 output.append("===========================")
                 output.append(
                     json.dumps(
@@ -60,27 +61,25 @@
                 )
             )
 
         print("\n".join(output))
 
     @classmethod
     def from_dict(cls, obj: dict):
-        """Create an instance of ProfileResponse from a dict"""
+        """Create an instance of ProfileResponse from a dict."""
         return cls(**obj)
 
 
 def profile(
     model: Union[Path, str, bytes, Any],
     device: Optional[str] = None,
     api_key: Optional[str] = None,
     timeout_sec: Optional[float] = None,
 ) -> ProfileResponse:
-    """
-    Profiles the performance of a trained model on a range of embedded targets, or a specific
-    device.
+    """Profile the performance of a trained model on a range of embedded targets, or a specific device.
 
     The response includes estimates of memory usage and latency for the model across a range of
     targets, including low-end MCU, high-end MCU, high-end MCU with accelerator, microprocessor unit
     (MPU), and a GPU or neural network accelerator. It will also include details of any conditions
     that preclude operation on a given type of device.
 
     If you request a specific `device`, the results will also include estimates for that specific
@@ -110,37 +109,41 @@
     Raises:
         Exception: Unhandled exception from API
         InvalidAuthTypeException: Incorrect authentication type was provided.
         InvalidDeviceException: Device is not valid.
         TimeoutException: Timeout waiting for result
 
     Examples:
-
         .. code-block:: python
 
             # Profile a Keras model across a range of devices
             result = ei.model.profile(model=keras_model)
             result.summary()
 
             # Profile different types of models on specific devices
+
+            # ONNX
             result = ei.model.profile(
-                model="heart_rate.onnx",  # ONNX
+                model="heart_rate.onnx",
                 device="cortex-m4f-80mhz"
             )
+
+            # TensorFlow SavedModel (can also be a zip)
             result = ei.model.profile(
-                model="heart_rate",  # TensorFlow SavedModel (can also be a zip)
+                model="heart_rate",
                 device="nordic-nrf9160-dk"
             )
+
+            # TensorFlow Lite (float32 or int8)
             result = ei.model.profile(
-                model="heart_rate.lite",  # TensorFlow Lite (float32 or int8)
+                model="heart_rate.lite",
                 device="synaptics-ka10000"
             )
 
     """
-
     client = configure_generic_client(
         key=api_key if api_key else edgeimpulse.API_KEY,
         host=edgeimpulse.API_ENDPOINT,
     )
     jobs = JobsApi(client)
     learn = LearnApi(client)
 
@@ -202,16 +205,16 @@
     profile_response = ProfileResponse.from_dict(
         get_pretrained_model_response.to_dict()
     )
     logging.info(f"profile_response = {profile_response}")
     return profile_response
 
 
-def list_profile_devices(api_key: Optional[str] = None) -> "List[str]":
-    """Lists possible values for the `device` field when calling `edgeimpulse.model.profile()`.
+def list_profile_devices(api_key: Optional[str] = None) -> List[str]:
+    """List possible values for the `device` field when calling `edgeimpulse.model.profile()`.
 
     Args:
         api_key (str, optional): The API key for an Edge Impulse project. This can also be set via
         the module-level variable `edgeimpulse.API_KEY`, or the env var `EI_API_KEY`.
 
     Returns:
         List[str]: List of profile targets for project
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/model/input_type.py` & `edgeimpulse-1.0.9/edgeimpulse/model/input_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+# ruff: noqa: D100, D101
 from typing import Literal
 
 
 class ImageInput(dict):
     def __init__(self, scaling_range: Literal["0..1", "0..255", "torch"] = "0..1"):
-        """Describes an image input, and specifies how it should be processed.
+        """Describe an image input, and specifies how it should be processed.
 
         Args:
             scaling_range (Literal['0..1', '0..255', 'torch']): Describes any scaling or
                 normalization that is applied to images. If no value is set then "0..1" is used.
                 "0..1" gives you non-normalized pixels between 0 and 1. "0..255" gives you
                 non-normalized pixels between 0 and 255. "torch" first scales pixels between 0 and
                 1, then applies normalization using the ImageNet dataset as a reference (same as
@@ -15,26 +16,26 @@
         """
         self["inputType"] = "image"
         self["inputScaling"] = scaling_range
 
 
 class AudioInput(dict):
     def __init__(self, frequency_hz: float):
-        """Describes an audio input, and specifies how it should be processed.
+        """Describe an audio input, and specifies how it should be processed.
 
         Args:
             frequency_hz (float): The frequency of the audio signal in Hz (samples per second).
         """
         self["inputType"] = "audio"
         self["frequencyHz"] = frequency_hz
 
 
 class TimeSeriesInput(dict):
     def __init__(self, frequency_hz: float, windowlength_ms: int):
-        """Describes a time series input, and specifies how it should be processed.
+        """Describe a time series input, and specifies how it should be processed.
 
         A stream of time series data is windowed into chunks of `windowlength_ms` according to the
         signal's frequency (`frequency_hz`). The window length represents how much data
         is fed into the model per inference.
 
         Args:
             frequency_hz (float): The frequency of the signal in Hz (samples per second).
@@ -44,9 +45,9 @@
         self["inputType"] = "time-series"
         self["frequencyHz"] = frequency_hz
         self["windowLengthMs"] = windowlength_ms
 
 
 class OtherInput(dict):
     def __init__(self):
-        """Describes an input that is passed into the model without any changes."""
+        """Describe an input that is passed into the model without any changes."""
         self["inputType"] = "other"
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/model/output_type.py` & `edgeimpulse-1.0.9/edgeimpulse/model/output_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+# ruff: noqa:  D100, D101
 from typing import Optional, List, Union, Literal
 
 
 class Classification(dict):
     def __init__(self, labels: Optional[List[str]] = None):
-        """Describes a classifier output with an optional list of label names.
+        """Describe a classifier output with an optional list of label names.
 
         If no list is provided then numeric labels will be assigned according to the
         order of outputs.
 
         Args:
             labels (Optional[List[str]]): A list of label names, one per index in the
                 output tensor. If no list is provided then numeric labels will be
@@ -15,15 +16,15 @@
         """
         self["modelType"] = "classification"
         self["labels"] = labels
 
 
 class Regression(dict):
     def __init__(self):
-        """Describes a regression output with a single value."""
+        """Describe a regression output with a single value."""
         self["modelType"] = "regression"
 
 
 class ObjectDetection(dict):
     def __init__(
         self,
         labels: List[str],
@@ -31,15 +32,15 @@
             Literal[
                 "mobilenet-ssd", "fomo", "yolov5", "yolo5v5-drpai", "yolox", "yolov7"
             ],
             str,
         ],
         minimum_confidence: float,
     ):
-        """Describes an object detection output with a specific format and labels.
+        """Describe an object detection output with a specific format and labels.
 
         Args:
             labels (Optional[List[str]]): A list of label names, one per index in the
                 output tensor. If no list is provided then numeric labels will be
                 assigned according to the order of outputs.
             last_layer (Union[Literal, str]): The output type of the model, depending on
                 the type of object detection model this is. Many common formats are
```

### Comparing `edgeimpulse-1.0.8/edgeimpulse/util.py` & `edgeimpulse-1.0.9/edgeimpulse/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,75 @@
+"""Various Edge Impulse functions for working with the SDK."""
+# mypy: ignore-errors
+# noqa: D100
 import logging
-import tempfile
 import time
 import base64
 from typing import Union, Optional, List, Tuple, Any
 from pathlib import Path
 import shutil
 import os
-from urllib3.exceptions import ReadTimeoutError
 import zipfile
+import socketio
 import platform
+import re
 
 import edgeimpulse as ei
+import edgeimpulse
 
 from edgeimpulse.exceptions import (
     InvalidAuthTypeException,
     MissingApiKeyException,
     InvalidModelException,
     UnsuccessfulRequestException,
     TimeoutException,
 )
 
 from edgeimpulse_api import (
     ApiClient,
     JobsApi,
     DeploymentApi,
+    OrganizationJobsApi,
     Configuration,
     ProjectsApi,
     GetJobResponse,
     LearnApi,
-    RawDataApi,
 )
 
 DATA_CATEGORIES = ["training", "testing", "anomaly"]
 
 
 def get_user_agent(add_platform_info=False):
-    """
-    Helper function to get user agent string for API calls.
-    """
+    """Get user agent string for API calls so we can track usage."""
     user_agent = f"edgeimpulse-sdk/{ei.__version__}"
     if add_platform_info:
         user_agent += (
             f" (python {platform.python_version()} {platform.system().lower()})"
         )
     return user_agent
 
 
 def configure_generic_client(
     key: str,
-    key_type: str = "api",
-    host: str = "https://studio.edgeimpulse.com/v1",
+    key_type: Optional[str] = "api",
+    host: Optional[str] = "https://studio.edgeimpulse.com/v1",
 ) -> ApiClient:
-    """Helper funtion to configure generic api client
+    """Configure generic api client which the right key.
 
     Args:
         key (str): api, jwt or jwt_http key.
-        key_type (str, optional): Type of key. Defaults to 'api'.
+        key_type (str, optional): Type of key. Defaults to `api`.
         host (str): API host url. Defaults to "https://studio.edgeimpulse.com/v1".
 
     Raises:
         Exception: Unrecognized key_type
 
     Returns:
         ApiClient: Generic API client used in other generated APIs
     """
-
     if key is None:
         raise MissingApiKeyException()
 
     logging.debug(f"Using API host [{host}]")
 
     config = Configuration(host=host)
     if key_type == "api":
@@ -95,15 +96,15 @@
 
 def poll(
     jobs_client: JobsApi,
     project_id: int,
     job_id: int,
     timeout_sec: Optional[float] = None,
 ) -> GetJobResponse:
-    """Helper function to syncronously poll a specific job within a project
+    """Poll a specific job within a project until done or timmeout is reached.
 
     Args:
         jobs_client (JobsApi): JobsApi client
         project_id (int): Project id number
         job_id (int): Job id to poll
         timeout_sec (float, optional): Optional timeout for polling.
 
@@ -176,124 +177,159 @@
                     raise e
 
             raise TimeoutException(err_msg)
 
 
 # Try importing numpy (even if it isn't used, which triggers F401 in linting)
 # ruff: noqa: F401
-def numpy_installed():
+def numpy_installed() -> bool:
+    """Check if numpy is installed returns true or false."""
     try:
         import numpy as np
 
         return True
     except ModuleNotFoundError:
         return False
 
 
 # Try importing tensorflow (even if it isn't used, which triggers F401 in linting)
 # ruff: noqa: F401
-def tensorflow_installed():
+def tensorflow_installed() -> bool:
+    """Check if tensorflow is installed returns true or false."""
     try:
-        import tensorflow as tf
+        import tensorflow as tf  # type: ignore # noqa: F401
 
         return True
     except ModuleNotFoundError:
         return False
 
 
 # Try importing onnx (even if it isn't used, which triggers F401 in linting)
 # ruff: noqa: F401
-def onnx_installed():
+def onnx_installed() -> bool:
+    """Check if onnx is installed returns true or false."""
     try:
         import onnx
 
         return True
     except ModuleNotFoundError:
-        return
+        return False
 
 
 # Try importing pandas
 # ruff: noqa: F401
-def pandas_installed():
+def pandas_installed() -> bool:
+    """Check if pandas is installed returns true or false."""
     try:
         import pandas
 
         return True
     except ModuleNotFoundError:
-        return
+        return False
 
 
-def is_path_to_numpy_file(data):
-    return is_type_accepted_by_open(data) and str(data).endswith(".npy")
+def is_path_to_numpy_file(path):
+    """Check if given path is a numpy file."""
+    return is_type_accepted_by_open(path) and str(path).endswith(".npy")
 
 
-def is_path_to_onnx_model(model):
-    return is_type_accepted_by_open(model) and str(model).endswith(".onnx")
+def is_path_to_onnx_model(path):
+    """Check if given path is a onnx file."""
+    return is_type_accepted_by_open(path) and str(path).endswith(".onnx")
 
 
-def is_type_accepted_by_open(model):
-    return (isinstance(model, str)) or (issubclass(type(model), Path))
+def is_type_accepted_by_open(path):
+    """Check if given path is a. string or a `Path`."""
+    return (isinstance(path, str)) or (issubclass(type(path), Path))
 
 
 def is_path_to_tf_saved_model_zipped(model):
+    """Check if path is poiting to a zipped model."""
     if not is_type_accepted_by_open(model):
         return False
     if not os.path.exists(model):
         return False
     try:
         zip_file = zipfile.ZipFile(model)
         return "saved_model/saved_model.pb" in zip_file.namelist()
     except (zipfile.BadZipFile, IsADirectoryError):
         return False
 
 
 def is_path_to_tf_saved_model_directory(model_dir):
+    """Check if directory contains a saved model."""
     return os.path.exists(f"{model_dir}/saved_model.pb")
 
 
 def encode_file_as_base64(filename: str):
+    """Envode a file as base64."""
     with open(filename, "rb") as f:
         return base64.b64encode(f.read()).decode("utf-8")
 
 
 def is_keras_model(model):
+    """Check if model is a keras model."""
     if not tensorflow_installed():
         return False
-    import tensorflow as tf
+    import tensorflow as tf  # type: ignore # noqa: F401
 
     return issubclass(type(model), tf.keras.Model)
 
 
 def is_onnx_model(model):
+    """Check if given model is an onnx model."""
     if not onnx_installed():
         return False
     import onnx
 
     return issubclass(type(model), onnx.ModelProto)
 
 
 def is_numpy_array(array):
+    """Check if array is a numpy array."""
     if not numpy_installed():
         return False
     import numpy as np
 
     return type(array) == np.ndarray
 
 
 def make_zip_archive(saved_model_path):
+    """Create zip archive from a model path."""
     zip_path = shutil.make_archive(
         saved_model_path,
         "zip",
         root_dir=os.path.dirname(saved_model_path),
         base_dir="saved_model",
     )
     return zip_path
 
 
 def save_model(model: Union[Path, str, bytes], directory: str) -> str:
+    """Save a machine learning model to the specified directory.
+
+    Args:
+        model (Union[Path, str, bytes]): The machine learning model to be saved.
+            It can be either a file path pointing to the location of the model file,
+            a bytes object representing the model, or the model object itself.
+        directory (str): The directory where the model will be saved.
+
+    Returns:
+        str: The path to the saved model or archive.
+
+    Raises:
+        Exception: If the model is already located at the provided path.
+        InvalidModelException: If the model is of an unexpected type and cannot be processed.
+
+    Note:
+        The function supports saving TensorFlow/Keras models in TensorFlow's
+        SavedModel format if TensorFlow is installed and the model is a Keras model.
+        It also supports saving ONNX models if ONNX is installed and the model is in ONNX format.
+
+    """
     if isinstance(model, str) or isinstance(model, Path):
         raise Exception(f"Model is already located at path {model}")
 
     if tensorflow_installed() and is_keras_model(model):
         # Note: this needs to exactly match the format studio
         # expects for unpacking
         saved_model_path = os.path.join(directory, "saved_model")
@@ -314,25 +350,25 @@
 
     raise InvalidModelException(
         f"Model was unexpected type {type(model)} and could not be processed"
     )
 
 
 def inspect_model(model: Union[Path, str, bytes, Any], tempdir: str) -> Tuple[str, str]:
-    """
-    Helper function to load tflite model
+    """Load tflite model.
 
     Args:
         model: Supports a number of ways of representing a model including
                1) A Path / str filename of an onnx file, a Keras
                saved_model.zip, a TensorFlow saved_model directory or saved
                tflite model. 2) a Keras model instance. 3) an ONNX model
                instance
         tempdir: temp dir used to write saved form of any in memory
                  model passed
+
     Returns:
         Tuple(str): (model type suitable for API,
                      path to model saved suitable for API)
     """
     try:
         if is_path_to_onnx_model(model):
             logging.info(f"Model parsed as ONNX (by path) [{model}]")
@@ -430,14 +466,15 @@
 
     raise Exception(
         f"Can't parse representative data. Expecting file ending in .npy but received {type(data)}."
     )
 
 
 def save_representative_data(data: Union[Path, str, bytes], directory: str) -> str:
+    """Save the representive data to a directory."""
     if numpy_installed():
         import numpy as np
 
         if type(data) == np.ndarray:
             if directory is None:
                 raise Exception(
                     "Directory must be specified if a numpy array is provided"
@@ -446,19 +483,19 @@
             np.save(tmp_filename, data)
             return tmp_filename
 
     raise Exception(f"Can't parse representative data. Unknown type {type(data)}")
 
 
 def default_project_id_for(client: ApiClient) -> int:
-    """Derive project id from api_key used to configure generic client
+    """Derive project id from api_key used to configure generic client.
 
     Args:
         client (ApiClient): Generic api client configured with a project api key. For jwt or
-            jwt_http key use get_project_id_list().
+            jwt_http key use `get_project_id_list()`.
 
     Returns:
         int: Project id
     """
     projects = ProjectsApi(client)
     if any("JWT" in s for s in client.configuration.api_key.keys()):
         msg = (
@@ -478,18 +515,19 @@
     logging.debug(f"Derived project_id={project_id} based on api key")
     return project_id
 
 
 def get_project_deploy_targets(
     client: ApiClient, project_id: Optional[int] = None
 ) -> List[str]:
-    """Pull a list of deploy targets
+    """Pull a list of deploy targets.
 
     Args:
         client (ApiClient): Generic api client configured with a project api key
+        project_id: (int, Optional) Project id to get the targets for. Defaults to None.
 
     Returns:
         List[str]: List of deploy targets for project
     """
     if project_id is None:
         project_id = default_project_id_for(client)
     try:
@@ -502,18 +540,19 @@
         raise e
     return [x.to_dict()["format"] for x in targets]
 
 
 def get_profile_devices(
     client: ApiClient, project_id: Optional[int] = None
 ) -> List[str]:
-    """Pull a list of profile devices
+    """Pull a list of profile devices.
 
     Args:
         client (ApiClient): Generic api client configured with a project api key
+        project_id: (int, Optional) Project id to get the targets for. Defaults to None.
 
     Returns:
         List[str]: List of profile targets for project
     """
     if project_id is None:
         project_id = default_project_id_for(client)
     try:
@@ -532,23 +571,22 @@
     client: ApiClient,
     project_id: int,
     model: Union[Path, str, bytes, Any],
     representative_data: Optional[Union[Path, str, bytes, Any]] = None,
     device: Optional[str] = None,
     timeout_sec: Optional[float] = None,
 ) -> GetJobResponse:
-    """
-    Upload a model and data to Edge Impulse servers.
+    """Upload a model and data to Edge Impulse servers.
 
     Args:
         tempdir (str): Temporary directory to hold saved form of any model passed in
         client (ApiClient): Generic api client configured with a project api key. For jwt or
-            jwt_http key use get_project_id_list().
+            jwt_http key use `get_project_id_list()`.
         project_id (int): Project id number
-        model (Union[Path, str, bytes, Any], op): A machine learning model, or similarly represented
+        model (Union[Path, str, bytes, Any]): A machine learning model, or similarly represented
             computational graph. Can be `Path` or `str` denoting file path, Python `bytes`
             containing a model, or a Keras model instance.
         representative_data (Optional[Union[Path, str, bytes, Any]], optional): A numpy
             representative input dataset. Accepts either an in memory numpy array or the Path/str
             filename of a np.save .npy file.
         device (Optional[str], optional): An embedded processor for which to profile the model.
             A comprehensive list can be obtained via `edgeimpulse.model.list_profile_devices()`.
@@ -558,15 +596,14 @@
         e: Unhandled exception from api
         FileNotFoundError: File or directory not found
         TimeoutException: Timeout waiting for result from server
 
     Returns:
         GetJobResponse: Structure containing job information
     """
-
     # Determine the type of model we have and make sure it is present on disk
     model_file_type, model_path = inspect_model(model, tempdir)
 
     # Determine the type of representative features we have and make sure they are
     # present on disk
     representative_features_path = inspect_representative_data(representative_data)
     if representative_data is not None and not representative_features_path:
@@ -610,15 +647,194 @@
     # Write out response
     logging.info(job_response)
 
     return job_response
 
 
 def check_response_errors(request):
-    """Checks for standard errors and raises an exception with the details if found."""
+    """Check for standard errors and raise an exception with the details if found."""
     if hasattr(request, "success"):
         success = request.success
         error = None
         if hasattr(request, "error"):
             error = request.error
         if success is not True:
             raise UnsuccessfulRequestException(error)
+
+
+def run_organization_job_until_completion(
+    organization_id: int,
+    job_id: int,
+    data_cb=None,
+    client=None,
+    timeout_sec: Optional[int] = None,
+) -> None:
+    """Runs an organization job until completion.
+
+    Args:
+        organization_id (int): The ID of the organization.
+        job_id (int): The ID of the job to run.
+        data_cb (callable, optional): Callback function to handle job data.
+        client (object, optional): An API client object. If None, a generic client will be configured.
+        timeout_sec (int, optional): Number of seconds before timeing out the job with an exception. Default is None.
+
+    Returns:
+        None
+    """
+    if client is None:
+        client = configure_generic_client(
+            key=ei.API_KEY,
+            host=ei.API_ENDPOINT,
+        )
+
+    api = OrganizationJobsApi(client)
+    status = api.get_organization_job_status(
+        organization_id=organization_id, job_id=job_id
+    )
+    if status.job.finished is not None:
+        logging.debug(f"Organization job {job_id} is already finished")
+        return
+
+    ws = get_organization_websocket(client=client, organization_id=organization_id)
+    run_job_until_completion(ws, job_id, data_cb, timeout_sec=timeout_sec)
+
+
+def run_project_job_until_completion(
+    job_id: int,
+    data_cb=None,
+    client=None,
+    project_id: Optional[int] = None,
+    timeout_sec: Optional[int] = None,
+) -> None:
+    """Runs a project job until completion.
+
+    Args:
+        job_id (int): The ID of the job to run.
+        data_cb (callable, optional): Callback function to handle job data.
+        client (object, optional): An API client object. If None, a generic client will be configured.
+        project_id (int, optional): The ID of the project. If not provided, a default project ID will be used.
+        timeout_sec (int, optional): Number of seconds before timeing out the job with an exception. Default is None
+
+    Returns:
+        None
+    """
+    if client is None:
+        client = configure_generic_client(
+            key=ei.API_KEY,
+            host=ei.API_ENDPOINT,
+        )
+
+    if project_id is None:
+        project_id = default_project_id_for(client)
+
+    api = JobsApi(client)
+    status = api.get_job_status(project_id=project_id, job_id=job_id)
+    if status.job.finished is not None:
+        logging.debug(f"Job {job_id} is already finished")
+        return
+
+    ws = get_project_websocket(client=client, project_id=project_id)
+    run_job_until_completion(
+        ws=ws, job_id=job_id, data_cb=data_cb, timeout_sec=timeout_sec
+    )
+
+
+def run_job_until_completion(
+    ws, job_id: int, data_cb=None, timeout_sec: Optional[int] = None
+):
+    """Runs a project or organization job until completion.
+
+    Args:
+        ws (object): Websocket object.
+        job_id (int): The ID of the job to run.
+        data_cb (callable, optional): Callback function to handle job data.
+        timeout_sec (int, optional): Number of seconds before timeing out the job with an exception. Default is None.
+
+    Returns:
+        None
+    """
+    finished = [False]  # python hack for scoping
+
+    def handle_any(event, data):
+        if event == f"job-data-{job_id}":
+            line = data["data"].strip()
+            if data_cb is None:
+                logging.info(f"[{job_id}] {line}")
+            else:
+                data_cb(line)
+
+    def handle_finished(data):
+        if job_id == data.get("jobId"):
+            # TODO: Should we disconnect?
+            finished[0] = True
+            ws.disconnect()
+
+    logging.info(f"Watching job: {job_id}")
+    ws.on("*", handle_any)
+    ws.on("job-finished", handle_finished)
+    while not finished[0]:
+        if isinstance(timeout_sec, int):
+            if timeout_sec <= 0:
+                raise Exception(f"Timeout reached while waiting for job {job_id}")
+        time.sleep(1)
+        if isinstance(timeout_sec, int):
+            timeout_sec = timeout_sec - 1
+
+
+def get_organization_websocket(
+    client, organization_id: int, host: str = None
+) -> socketio.Client:
+    """Gets a websocket to listen to organization events.
+
+    Args:
+        client (object): An API client object.
+        organization_id (int): The ID of the organization.
+        host (str, optional): The hostname. If None, API_ENDPOINT will be used.
+
+    Returns:
+        object: Websocket object.
+    """
+    organization = OrganizationJobsApi(client)
+    token_res = organization.get_organization_socket_token(organization_id)
+    return connect_websocket(token_res.token.socket_token, host=host)
+
+
+def get_project_websocket(client, project_id: int, host: str = None) -> socketio.Client:
+    """Gets a websocket to listen to project events.
+
+    Args:
+        client (object): An API client object.
+        project_id (int): The ID of the project.
+        host (str, optional): The hostname. If None, API_ENDPOINT will be used.
+
+    Returns:
+        object: Websocket object.
+    """
+    projects = ProjectsApi(client)
+    token_res = projects.get_socket_token(project_id)
+    return connect_websocket(token_res.token.socket_token, host=host)
+
+
+def connect_websocket(token, host: str = None) -> socketio.Client:
+    """Connects to the websocket server.
+
+    Parameters:
+        token (str): The authentication token.
+        host (str, optional): The hostname. If None, API_ENDPOINT will be used.
+
+    Returns:
+        object: Websocket object.
+    """
+    if not host:
+        host = ei.API_ENDPOINT
+        host = host.replace("https://", "wss://")
+        host = host.replace("http://", "ws://")
+        host = host.replace("/v1", "/")
+
+    sio = socketio.Client(ssl_verify="wss://" in host)
+    sio.on("error", lambda: logging.info("Error"))
+    sio.on("connect", lambda: logging.info("Websocket connected to server"))
+    sio.on("disconnect", lambda: logging.info("Websocket disconnected from server"))
+
+    host = f"{host}/socket.io/?token={token}"
+    sio.connect(host, transports=["websocket"])
+    return sio
```

### Comparing `edgeimpulse-1.0.8/pyproject.toml` & `edgeimpulse-1.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 [tool.poetry]
 name = "edgeimpulse"
-version = "1.0.8"
+version = "1.0.9"
 description = "Python SDK for Edge Impulse."
 authors = ["EdgeImpulse Inc. <hello@edgeimpulse.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://edgeimpulse.com"
 repository = "https://github.com/edgeimpulse/python-sdk"
 documentation = "https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Embedded Systems"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-edgeimpulse-api = "1.40.11"
+edgeimpulse-api = "^1.49.9"
 requests = "^2.23.0"
+python-socketio = {extras = ["client"], version = "^5.8.0"}
 
 [tool.poetry.dev-dependencies]
 pandas = "^2.0.3"
 numpy = "^1.22"
 onnx = "^1.12"
 sphinx = "7.1.2"
 furo = "2023.7.26"
 myst-parser = "2.0.0"
 m2r2 = "0.3.3.post2"
 pyYAML = "6.0.1"
+sphinx-copybutton = "^0.5.2"
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.3"
 black = "^23.10.1"
+mypy = "^1.9.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "pypi-test"
 url = "https://test.pypi.org/simple"
 secondary = true
 
 [tool.ruff]
-target-version = "1.0.8"
+target-version = "py38"
 indent-width = 4
 
 [tool.ruff.lint]
 select = [
+    "B006",
     "A",    # flake8-builtins: prevent keywords that clobber python builtins
     "E4",   # (default) flake8: listing imports
     "E7",   # (default) flake8: multiple lines, comparisons, naming
     "E9",   # (default) flake8: Python syntax errors
     "F",    # (default) pyflakes: https://www.flake8rules.com/
     "W",    # flake8: whitespace rules
+    "D",
 ]
 ignore = []
+pydocstyle.convention = "google"
 
 [tool.black]
 target-version = ["py38"]
 line-length = 88
```

### Comparing `edgeimpulse-1.0.8/PKG-INFO` & `edgeimpulse-1.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: edgeimpulse
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python SDK for Edge Impulse.
 Home-page: https://edgeimpulse.com
 License: Apache-2.0
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Embedded Systems
-Requires-Dist: edgeimpulse-api (==1.40.11)
+Requires-Dist: edgeimpulse-api (>=1.49.9,<2.0.0)
+Requires-Dist: python-socketio[client] (>=5.8.0,<6.0.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Project-URL: Documentation, https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview
 Project-URL: Repository, https://github.com/edgeimpulse/python-sdk
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://edgeimpulse.com/"><img src="https://cdn.edgeimpulse.com/images/edge-impulse-primary-logo-black-text-white-bg.png" alt="Edge Impulse logo"/></a>
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: edgeimpulse Version: 1.0.8 Summary: Python SDK for
+Metadata-Version: 2.1 Name: edgeimpulse Version: 1.0.9 Summary: Python SDK for
 Edge Impulse. Home-page: https://edgeimpulse.com License: Apache-2.0 Author:
 EdgeImpulse Inc. Author-email: hello@edgeimpulse.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Software Development :: Embedded
-Systems Requires-Dist: edgeimpulse-api (==1.40.11) Requires-Dist: requests
-(>=2.23.0,<3.0.0) Project-URL: Documentation, https://docs.edgeimpulse.com/
-docs/edge-impulse-python-sdk/overview Project-URL: Repository, https://
-github.com/edgeimpulse/python-sdk Description-Content-Type: text/markdown
+Systems Requires-Dist: edgeimpulse-api (>=1.49.9,<2.0.0) Requires-Dist: python-
+socketio[client] (>=5.8.0,<6.0.0) Requires-Dist: requests (>=2.23.0,<3.0.0)
+Project-URL: Documentation, https://docs.edgeimpulse.com/docs/edge-impulse-
+python-sdk/overview Project-URL: Repository, https://github.com/edgeimpulse/
+python-sdk Description-Content-Type: text/markdown
                               _[_E_d_g_e_ _I_m_p_u_l_s_e_ _l_o_g_o_]
 # Edge Impulse SDK The official Python SDK for Edge Impulse is designed to help
 machine learning practitioners build and deploy models for embedded hardware
 and edge AI applications. - Profile your model to estimate RAM, ROM, and
 inference speed - Convert your model to C++ to deploy on edge hardware -
 Interact with Edge Impulse projects to collect data, train models, and deploy
 them to edge devices [Sign up for a free account â](https://
```

