# Comparing `tmp/env_canada-0.6.1.tar.gz` & `tmp/env_canada-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_canada-0.6.1.tar", last modified: Tue Dec 19 14:04:41 2023, max compression
+gzip compressed data, was "env_canada-0.6.2.tar", last modified: Thu May  2 20:40:18 2024, max compression
```

## Comparing `env_canada-0.6.1.tar` & `env_canada-0.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:04:41.257851 env_canada-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-19 14:04:31.000000 env_canada-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-19 14:04:31.000000 env_canada-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2023-12-19 14:04:41.257851 env_canada-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2023-12-19 14:04:31.000000 env_canada-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:04:41.253852 env_canada-0.6.1/env_canada/
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2023-12-19 14:04:31.000000 env_canada-0.6.1/env_canada/10x20.pbm
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2023-12-19 14:04:31.000000 env_canada-0.6.1/env_canada/10x20.pil
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-19 14:04:31.000000 env_canada-0.6.1/env_canada/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-19 14:04:31.000000 env_canada-0.6.1/env_canada/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2023-12-19 14:04:31.000000 env_canada-0.6.1/env_canada/ec_aqhi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-12-19 14:04:31.000000 env_canada-0.6.1/env_canada/ec_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-19 14:04:31.000000 env_canada-0.6.1/env_canada/ec_exc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15901 2023-12-19 14:04:31.000000 env_canada-0.6.1/env_canada/ec_historical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2023-12-19 14:04:31.000000 env_canada-0.6.1/env_canada/ec_hydro.py
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2023-12-19 14:04:31.000000 env_canada-0.6.1/env_canada/ec_radar.py
--rw-r--r--   0 runner    (1001) docker     (127)    17358 2023-12-19 14:04:31.000000 env_canada-0.6.1/env_canada/ec_weather.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:04:41.257851 env_canada-0.6.1/env_canada.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2023-12-19 14:04:41.000000 env_canada-0.6.1/env_canada.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-12-19 14:04:41.000000 env_canada-0.6.1/env_canada.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 14:04:41.000000 env_canada-0.6.1/env_canada.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-19 14:04:41.000000 env_canada-0.6.1/env_canada.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-19 14:04:41.000000 env_canada-0.6.1/env_canada.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 14:04:41.257851 env_canada-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-12-19 14:04:31.000000 env_canada-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:04:41.257851 env_canada-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-12-19 14:04:31.000000 env_canada-0.6.1/tests/test_ec_aqhi.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-19 14:04:31.000000 env_canada-0.6.1/tests/test_ec_historical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-12-19 14:04:31.000000 env_canada-0.6.1/tests/test_ec_hydro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-12-19 14:04:31.000000 env_canada-0.6.1/tests/test_ec_radar.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-19 14:04:31.000000 env_canada-0.6.1/tests/test_ec_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:40:18.389431 env_canada-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-02 20:40:02.000000 env_canada-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 20:40:02.000000 env_canada-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-05-02 20:40:18.389431 env_canada-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-05-02 20:40:02.000000 env_canada-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:40:18.389431 env_canada-0.6.2/env_canada/
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-02 20:40:02.000000 env_canada-0.6.2/env_canada/10x20.pbm
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-02 20:40:02.000000 env_canada-0.6.2/env_canada/10x20.pil
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 20:40:02.000000 env_canada-0.6.2/env_canada/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 20:40:02.000000 env_canada-0.6.2/env_canada/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-02 20:40:02.000000 env_canada-0.6.2/env_canada/ec_aqhi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-02 20:40:02.000000 env_canada-0.6.2/env_canada/ec_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 20:40:02.000000 env_canada-0.6.2/env_canada/ec_exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15901 2024-05-02 20:40:02.000000 env_canada-0.6.2/env_canada/ec_historical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-02 20:40:02.000000 env_canada-0.6.2/env_canada/ec_hydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-05-02 20:40:02.000000 env_canada-0.6.2/env_canada/ec_radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-02 20:40:02.000000 env_canada-0.6.2/env_canada/ec_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:40:18.389431 env_canada-0.6.2/env_canada.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-05-02 20:40:18.000000 env_canada-0.6.2/env_canada.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-02 20:40:18.000000 env_canada-0.6.2/env_canada.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:40:18.000000 env_canada-0.6.2/env_canada.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 20:40:18.000000 env_canada-0.6.2/env_canada.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 20:40:18.000000 env_canada-0.6.2/env_canada.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:40:18.389431 env_canada-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-02 20:40:02.000000 env_canada-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:40:18.389431 env_canada-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 20:40:02.000000 env_canada-0.6.2/tests/test_ec_aqhi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-02 20:40:02.000000 env_canada-0.6.2/tests/test_ec_historical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-02 20:40:02.000000 env_canada-0.6.2/tests/test_ec_hydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-02 20:40:02.000000 env_canada-0.6.2/tests/test_ec_radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-02 20:40:02.000000 env_canada-0.6.2/tests/test_ec_weather.py
```

### Comparing `env_canada-0.6.1/LICENSE` & `env_canada-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/PKG-INFO` & `env_canada-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env_canada
-Version: 0.6.1
+Version: 0.6.2
 Summary: A package to access meteorological data from Environment Canada
 Home-page: https://github.com/michaeldavie/env_canada
 Author: Michael Davie
 Author-email: michael.davie@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 Requires-Dist: Pillow>=10.0.1
 Requires-Dist: python-dateutil
 Requires-Dist: voluptuous
 
 # Environment Canada (env_canada)
 
 [![PyPI version](https://badge.fury.io/py/env-canada.svg)](https://badge.fury.io/py/env-canada)
-[![Snyk rating](https://snyk-widget.herokuapp.com/badge/pip/env-canada/badge.svg)](https://snyk.io/vuln/pip:env-canada@0.6.1?utm_source=badge)
+[![Snyk rating](https://snyk-widget.herokuapp.com/badge/pip/env-canada/badge.svg)](https://snyk.io/vuln/pip:env-canada@0.6.2?utm_source=badge)
 
 This package provides access to various data sources published by [Environment and Climate Change Canada](https://www.canada.ca/en/environment-climate-change.html).
 
 ## Weather Observations and Forecasts
 
 `ECWeather` provides current conditions and forecasts. It automatically determines which weather station to use based on latitude/longitude provided. It is also possible to specify a specific station code of the form `AB/s0000123` based on those listed in [this CSV file](https://dd.weather.gc.ca/citypage_weather/docs/site_list_towns_en.csv). For example:
 
@@ -112,15 +112,16 @@
 `ECHistorical` provides historical daily weather data.
 The ECHistorical object is instantiated with a station ID, year, language, format (one of xml or csv) and granularity (hourly, daily data).
 Once updated asynchronously, historical weather data is contained with the `station_data` property. If `xml` is requested, `station_data` will appear in a dictionary form. If `csv` is requested, `station_data` will contain a CSV-readable buffer. For example:
 
 ```python
 import asyncio
 
-from env_canada import ECHistorical, get_historical_stations
+from env_canada import ECHistorical
+from env_canada.ec_historical import get_historical_stations
 
 # search for stations, response contains station_ids
 coordinates = [53.916944, -122.749444] # [lat, long]
 
 # coordinates: [lat, long]
 # radius: km
 # limit: response limit, value one of [10, 25, 50, 100]
@@ -161,15 +162,16 @@
 The data can then be used as pandas DataFrame, XML (requires pandas >=1.3.0) and csv
 
 For example :
 
 ```python
 import pandas as pd
 import asyncio
-from env_canada import ECHistoricalRange, get_historical_stations
+from env_canada import ECHistoricalRange
+from env_canada.ec_historical import get_historical_stations
 from datetime import datetime
 
 coordinates = ['48.508333', '-68.467667']
 
 stations = pd.DataFrame(asyncio.run(get_historical_stations(coordinates, start_year=2022,
                                                 end_year=2022, radius=200, limit=100))).T
```

### Comparing `env_canada-0.6.1/README.md` & `env_canada-0.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Environment Canada (env_canada)
 
 [![PyPI version](https://badge.fury.io/py/env-canada.svg)](https://badge.fury.io/py/env-canada)
-[![Snyk rating](https://snyk-widget.herokuapp.com/badge/pip/env-canada/badge.svg)](https://snyk.io/vuln/pip:env-canada@0.6.1?utm_source=badge)
+[![Snyk rating](https://snyk-widget.herokuapp.com/badge/pip/env-canada/badge.svg)](https://snyk.io/vuln/pip:env-canada@0.6.2?utm_source=badge)
 
 This package provides access to various data sources published by [Environment and Climate Change Canada](https://www.canada.ca/en/environment-climate-change.html).
 
 ## Weather Observations and Forecasts
 
 `ECWeather` provides current conditions and forecasts. It automatically determines which weather station to use based on latitude/longitude provided. It is also possible to specify a specific station code of the form `AB/s0000123` based on those listed in [this CSV file](https://dd.weather.gc.ca/citypage_weather/docs/site_list_towns_en.csv). For example:
 
@@ -88,15 +88,16 @@
 `ECHistorical` provides historical daily weather data.
 The ECHistorical object is instantiated with a station ID, year, language, format (one of xml or csv) and granularity (hourly, daily data).
 Once updated asynchronously, historical weather data is contained with the `station_data` property. If `xml` is requested, `station_data` will appear in a dictionary form. If `csv` is requested, `station_data` will contain a CSV-readable buffer. For example:
 
 ```python
 import asyncio
 
-from env_canada import ECHistorical, get_historical_stations
+from env_canada import ECHistorical
+from env_canada.ec_historical import get_historical_stations
 
 # search for stations, response contains station_ids
 coordinates = [53.916944, -122.749444] # [lat, long]
 
 # coordinates: [lat, long]
 # radius: km
 # limit: response limit, value one of [10, 25, 50, 100]
@@ -137,15 +138,16 @@
 The data can then be used as pandas DataFrame, XML (requires pandas >=1.3.0) and csv
 
 For example :
 
 ```python
 import pandas as pd
 import asyncio
-from env_canada import ECHistoricalRange, get_historical_stations
+from env_canada import ECHistoricalRange
+from env_canada.ec_historical import get_historical_stations
 from datetime import datetime
 
 coordinates = ['48.508333', '-68.467667']
 
 stations = pd.DataFrame(asyncio.run(get_historical_stations(coordinates, start_year=2022,
                                                 end_year=2022, radius=200, limit=100))).T
```

### Comparing `env_canada-0.6.1/env_canada/10x20.pbm` & `env_canada-0.6.2/env_canada/10x20.pbm`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/env_canada/10x20.pil` & `env_canada-0.6.2/env_canada/10x20.pil`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/env_canada/ec_aqhi.py` & `env_canada-0.6.2/env_canada/ec_aqhi.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/env_canada/ec_cache.py` & `env_canada-0.6.2/env_canada/ec_cache.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/env_canada/ec_historical.py` & `env_canada-0.6.2/env_canada/ec_historical.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/env_canada/ec_hydro.py` & `env_canada-0.6.2/env_canada/ec_hydro.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/env_canada/ec_radar.py` & `env_canada-0.6.2/env_canada/ec_radar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from aiohttp.client_exceptions import ClientConnectorError
 import asyncio
 import datetime
-from io import BytesIO
 import logging
 import math
 import os
-from PIL import Image, ImageDraw, ImageFont
+from io import BytesIO
 
-from .ec_cache import CacheClientSession as ClientSession
 import dateutil.parser
 import defusedxml.ElementTree as et
 import imageio.v2 as imageio
 import voluptuous as vol
+from aiohttp.client_exceptions import ClientConnectorError
+from PIL import Image, ImageDraw, ImageFont
+
+from .ec_cache import CacheClientSession as ClientSession
 
 ATTRIBUTION = {
     "english": "Data provided by Environment Canada",
     "french": "Données fournies par Environnement Canada",
 }
 
 __all__ = ["ECRadar"]
@@ -327,14 +328,25 @@
             self._auto_precip_type()
 
         self.image = await self.get_loop()
 
     async def get_loop(self, fps=5):
         """Build an animated GIF of recent radar images."""
 
+        def build_image():
+            gif_frames = [imageio.imread(f, mode="RGBA") for f in frames]
+            gif_bytes = imageio.mimwrite(
+                imageio.RETURN_BYTES,
+                gif_frames,
+                format="GIF",
+                duration=duration,
+                subrectangles=True,
+            )
+            return gif_bytes
+
         """Build list of frame timestamps."""
         start, end = await self._get_dimensions()
         frame_times = [start]
 
         while True:
             next_frame = frame_times[-1] + datetime.timedelta(minutes=radar_interval)
             if next_frame > end:
@@ -357,16 +369,10 @@
 
         for f in range(3):
             frames.append(frames[-1])
 
         """Assemble animated GIF."""
         duration = 1000 / fps
 
-        gif_frames = [imageio.imread(f, mode="RGBA") for f in frames]
-        gif_bytes = imageio.mimwrite(
-            imageio.RETURN_BYTES,
-            gif_frames,
-            format="GIF",
-            duration=duration,
-            subrectangles=True,
-        )
+        loop = asyncio.get_running_loop()
+        gif_bytes = await loop.run_in_executor(None, build_image)
         return gif_bytes
```

### Comparing `env_canada-0.6.1/env_canada/ec_weather.py` & `env_canada-0.6.2/env_canada/ec_weather.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/env_canada.egg-info/PKG-INFO` & `env_canada-0.6.2/env_canada.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: env-canada
-Version: 0.6.1
+Name: env_canada
+Version: 0.6.2
 Summary: A package to access meteorological data from Environment Canada
 Home-page: https://github.com/michaeldavie/env_canada
 Author: Michael Davie
 Author-email: michael.davie@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 Requires-Dist: Pillow>=10.0.1
 Requires-Dist: python-dateutil
 Requires-Dist: voluptuous
 
 # Environment Canada (env_canada)
 
 [![PyPI version](https://badge.fury.io/py/env-canada.svg)](https://badge.fury.io/py/env-canada)
-[![Snyk rating](https://snyk-widget.herokuapp.com/badge/pip/env-canada/badge.svg)](https://snyk.io/vuln/pip:env-canada@0.6.1?utm_source=badge)
+[![Snyk rating](https://snyk-widget.herokuapp.com/badge/pip/env-canada/badge.svg)](https://snyk.io/vuln/pip:env-canada@0.6.2?utm_source=badge)
 
 This package provides access to various data sources published by [Environment and Climate Change Canada](https://www.canada.ca/en/environment-climate-change.html).
 
 ## Weather Observations and Forecasts
 
 `ECWeather` provides current conditions and forecasts. It automatically determines which weather station to use based on latitude/longitude provided. It is also possible to specify a specific station code of the form `AB/s0000123` based on those listed in [this CSV file](https://dd.weather.gc.ca/citypage_weather/docs/site_list_towns_en.csv). For example:
 
@@ -112,15 +112,16 @@
 `ECHistorical` provides historical daily weather data.
 The ECHistorical object is instantiated with a station ID, year, language, format (one of xml or csv) and granularity (hourly, daily data).
 Once updated asynchronously, historical weather data is contained with the `station_data` property. If `xml` is requested, `station_data` will appear in a dictionary form. If `csv` is requested, `station_data` will contain a CSV-readable buffer. For example:
 
 ```python
 import asyncio
 
-from env_canada import ECHistorical, get_historical_stations
+from env_canada import ECHistorical
+from env_canada.ec_historical import get_historical_stations
 
 # search for stations, response contains station_ids
 coordinates = [53.916944, -122.749444] # [lat, long]
 
 # coordinates: [lat, long]
 # radius: km
 # limit: response limit, value one of [10, 25, 50, 100]
@@ -161,15 +162,16 @@
 The data can then be used as pandas DataFrame, XML (requires pandas >=1.3.0) and csv
 
 For example :
 
 ```python
 import pandas as pd
 import asyncio
-from env_canada import ECHistoricalRange, get_historical_stations
+from env_canada import ECHistoricalRange
+from env_canada.ec_historical import get_historical_stations
 from datetime import datetime
 
 coordinates = ['48.508333', '-68.467667']
 
 stations = pd.DataFrame(asyncio.run(get_historical_stations(coordinates, start_year=2022,
                                                 end_year=2022, radius=200, limit=100))).T
```

### Comparing `env_canada-0.6.1/env_canada.egg-info/SOURCES.txt` & `env_canada-0.6.2/env_canada.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/setup.py` & `env_canada-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="env_canada",
-    version="0.6.1",
+    version="0.6.2",
     author="Michael Davie",
     author_email="michael.davie@gmail.com",
     description="A package to access meteorological data from Environment Canada",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/michaeldavie/env_canada",
```

### Comparing `env_canada-0.6.1/tests/test_ec_aqhi.py` & `env_canada-0.6.2/tests/test_ec_aqhi.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/tests/test_ec_historical.py` & `env_canada-0.6.2/tests/test_ec_historical.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/tests/test_ec_hydro.py` & `env_canada-0.6.2/tests/test_ec_hydro.py`

 * *Files identical despite different names*

### Comparing `env_canada-0.6.1/tests/test_ec_radar.py` & `env_canada-0.6.2/tests/test_ec_radar.py`

 * *Files identical despite different names*

