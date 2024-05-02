# Comparing `tmp/imgw_pib-1.0.0.tar.gz` & `tmp/imgw_pib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgw_pib-1.0.0.tar", last modified: Tue Apr 30 09:24:59 2024, max compression
+gzip compressed data, was "imgw_pib-1.0.1.tar", last modified: Thu May  2 14:40:17 2024, max compression
```

## Comparing `imgw_pib-1.0.0.tar` & `imgw_pib-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:24:59.519933 imgw_pib-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-30 09:24:59.519933 imgw_pib-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:24:59.515933 imgw_pib-1.0.0/imgw_pib/
--rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/imgw_pib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:24:59.519933 imgw_pib-1.0.0/imgw_pib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-30 09:24:59.000000 imgw_pib-1.0.0/imgw_pib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 09:24:59.000000 imgw_pib-1.0.0/imgw_pib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:24:59.000000 imgw_pib-1.0.0/imgw_pib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 09:24:59.000000 imgw_pib-1.0.0/imgw_pib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 09:24:59.000000 imgw_pib-1.0.0/imgw_pib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:24:59.519933 imgw_pib-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:24:59.515933 imgw_pib-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-30 09:24:51.000000 imgw_pib-1.0.0/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:17.784837 imgw_pib-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-02 14:40:17.784837 imgw_pib-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:17.780837 imgw_pib-1.0.1/imgw_pib/
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/imgw_pib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/imgw_pib/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/imgw_pib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/imgw_pib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/imgw_pib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/imgw_pib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:17.784837 imgw_pib-1.0.1/imgw_pib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-02 14:40:17.000000 imgw_pib-1.0.1/imgw_pib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-02 14:40:17.000000 imgw_pib-1.0.1/imgw_pib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:40:17.000000 imgw_pib-1.0.1/imgw_pib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 14:40:17.000000 imgw_pib-1.0.1/imgw_pib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 14:40:17.000000 imgw_pib-1.0.1/imgw_pib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:40:17.784837 imgw_pib-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:17.784837 imgw_pib-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-05-02 14:40:09.000000 imgw_pib-1.0.1/tests/test_init.py
```

### Comparing `imgw_pib-1.0.0/LICENSE` & `imgw_pib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imgw_pib-1.0.0/PKG-INFO` & `imgw_pib-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgw_pib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python wrapper for IMGW-PIB API.
 Home-page: https://github.com/bieniu/imgw-pib
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
 
 You can install the library with pip:
 
 ```
 pip install imgw-pib
 ```
 
-## How to use package
+## How to use the library
 
 ```python
 """Example of usage IMGW-PIB."""
 
 import asyncio
 import logging
 
@@ -78,15 +78,15 @@
 
 
 loop = asyncio.new_event_loop()
 loop.run_until_complete(main())
 loop.close()
 ```
 
-## Error Handling
+## Error handling
 
 The library raises `ApiError` when the IMGW-PIB API returns an error, `ClientError` for network-related errors, and `TimeoutError` when a request times out.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `imgw_pib-1.0.0/README.md` & `imgw_pib-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 You can install the library with pip:
 
 ```
 pip install imgw-pib
 ```
 
-## How to use package
+## How to use the library
 
 ```python
 """Example of usage IMGW-PIB."""
 
 import asyncio
 import logging
 
@@ -58,15 +58,15 @@
 
 
 loop = asyncio.new_event_loop()
 loop.run_until_complete(main())
 loop.close()
 ```
 
-## Error Handling
+## Error handling
 
 The library raises `ApiError` when the IMGW-PIB API returns an error, `ClientError` for network-related errors, and `TimeoutError` when a request times out.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `imgw_pib-1.0.0/imgw_pib/__init__.py` & `imgw_pib-1.0.1/imgw_pib/__init__.py`

 * *Files identical despite different names*

### Comparing `imgw_pib-1.0.0/imgw_pib/model.py` & `imgw_pib-1.0.1/imgw_pib/model.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,21 +55,21 @@
 
     flood_alarm: bool | None = None
     flood_warning: bool | None = None
 
     def __post_init__(self: Self) -> None:
         """Call after initialization."""
         if self.water_level.value is not None:
-            if self.flood_warning_level.value is not None:
+            if self.flood_alarm_level.value is not None:
                 self.flood_alarm = (
-                    self.water_level.value >= self.flood_warning_level.value
+                    self.water_level.value >= self.flood_alarm_level.value
                 )
-            if self.flood_alarm_level.value is not None:
+            if self.flood_warning_level.value is not None:
                 self.flood_warning = (
-                    self.water_level.value >= self.flood_alarm_level.value
+                    self.water_level.value >= self.flood_warning_level.value
                 )
 
 
 class ApiNames(StrEnum):
     """Names type for API."""
 
     HUMIDITY = "wilgotnosc_wzgledna"
```

### Comparing `imgw_pib-1.0.0/imgw_pib/utils.py` & `imgw_pib-1.0.1/imgw_pib/utils.py`

 * *Files identical despite different names*

### Comparing `imgw_pib-1.0.0/imgw_pib.egg-info/PKG-INFO` & `imgw_pib-1.0.1/imgw_pib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgw_pib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python wrapper for IMGW-PIB API.
 Home-page: https://github.com/bieniu/imgw-pib
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
 
 You can install the library with pip:
 
 ```
 pip install imgw-pib
 ```
 
-## How to use package
+## How to use the library
 
 ```python
 """Example of usage IMGW-PIB."""
 
 import asyncio
 import logging
 
@@ -78,15 +78,15 @@
 
 
 loop = asyncio.new_event_loop()
 loop.run_until_complete(main())
 loop.close()
 ```
 
-## Error Handling
+## Error handling
 
 The library raises `ApiError` when the IMGW-PIB API returns an error, `ClientError` for network-related errors, and `TimeoutError` when a request times out.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `imgw_pib-1.0.0/setup.py` & `imgw_pib-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 setup(
     name="imgw_pib",
     version=VERSION,
     author="Maciej Bieniek",
     description="Python wrapper for IMGW-PIB API.",
     long_description=README_FILE.read_text(encoding="utf-8"),
```

### Comparing `imgw_pib-1.0.0/tests/test_init.py` & `imgw_pib-1.0.1/tests/test_init.py`

 * *Files 26% similar despite different names*

```diff
@@ -257,7 +257,85 @@
 
         imgwpib = await ImgwPib.create(session, hydrological_station_id="154190050")
         hydrological_data = await imgwpib.get_hydrological_data()
 
     await session.close()
 
     assert hydrological_data.water_level_measurement_date is None
+
+
+@pytest.mark.parametrize(
+    ("water_level", "flood_warning_level", "expected"),
+    [(100.0, 200.0, False), (100.0, 100.0, True), (100.0, 50.0, True)],
+)
+@pytest.mark.asyncio()
+async def test_flood_warning(
+    hydrological_stations: list[dict[str, Any]],
+    hydrological_station: dict[str, Any],
+    hydrological_details: dict[str, Any],
+    water_level: float,
+    flood_warning_level: float,
+    expected: bool,
+) -> None:
+    """Test flood warning value."""
+    session = aiohttp.ClientSession()
+
+    hydrological_station[ApiNames.WATER_LEVEL] = water_level
+    hydrological_details["status"]["warningValue"] = flood_warning_level
+
+    with aioresponses() as session_mock:
+        session_mock.get(API_HYDROLOGICAL_ENDPOINT, payload=hydrological_stations)
+        session_mock.get(
+            f"{API_HYDROLOGICAL_ENDPOINT}/id/154190050", payload=hydrological_station
+        )
+        session_mock.get(
+            API_HYDROLOGICAL_DETAILS_ENDPOINT.format(
+                hydrological_station_id="154190050"
+            ),
+            payload=hydrological_details,
+        )
+
+        imgwpib = await ImgwPib.create(session, hydrological_station_id="154190050")
+        result = await imgwpib.get_hydrological_data()
+
+    await session.close()
+
+    assert result.flood_warning == expected
+
+
+@pytest.mark.parametrize(
+    ("water_level", "flood_alarm_level", "expected"),
+    [(100.0, 200.0, False), (100.0, 100.0, True), (100.0, 50.0, True)],
+)
+@pytest.mark.asyncio()
+async def test_flood_alarm(
+    hydrological_stations: list[dict[str, Any]],
+    hydrological_station: dict[str, Any],
+    hydrological_details: dict[str, Any],
+    water_level: float,
+    flood_alarm_level: float,
+    expected: bool,
+) -> None:
+    """Test flood alarm value."""
+    session = aiohttp.ClientSession()
+
+    hydrological_station[ApiNames.WATER_LEVEL] = water_level
+    hydrological_details["status"]["alarmValue"] = flood_alarm_level
+
+    with aioresponses() as session_mock:
+        session_mock.get(API_HYDROLOGICAL_ENDPOINT, payload=hydrological_stations)
+        session_mock.get(
+            f"{API_HYDROLOGICAL_ENDPOINT}/id/154190050", payload=hydrological_station
+        )
+        session_mock.get(
+            API_HYDROLOGICAL_DETAILS_ENDPOINT.format(
+                hydrological_station_id="154190050"
+            ),
+            payload=hydrological_details,
+        )
+
+        imgwpib = await ImgwPib.create(session, hydrological_station_id="154190050")
+        result = await imgwpib.get_hydrological_data()
+
+    await session.close()
+
+    assert result.flood_alarm == expected
```

