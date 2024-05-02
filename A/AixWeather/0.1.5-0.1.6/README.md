# Comparing `tmp/AixWeather-0.1.5.tar.gz` & `tmp/aixweather-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AixWeather-0.1.5.tar", last modified: Fri Mar  1 11:18:31 2024, max compression
+gzip compressed data, was "aixweather-0.1.6.tar", last modified: Thu May  2 16:25:20 2024, max compression
```

## Comparing `AixWeather-0.1.5.tar` & `aixweather-0.1.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 11:18:31.454935 AixWeather-0.1.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 11:18:31.450935 AixWeather-0.1.5/AixWeather.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8339 2024-03-01 11:18:31.000000 AixWeather-0.1.5/AixWeather.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1526 2024-03-01 11:18:31.000000 AixWeather-0.1.5/AixWeather.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 11:18:31.000000 AixWeather-0.1.5/AixWeather.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      218 2024-03-01 11:18:31.000000 AixWeather-0.1.5/AixWeather.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-01 11:18:31.000000 AixWeather-0.1.5/AixWeather.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2377 2024-03-01 11:09:21.000000 AixWeather-0.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8339 2024-03-01 11:18:31.454935 AixWeather-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6882 2024-03-01 11:09:21.000000 AixWeather-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 11:18:31.450935 AixWeather-0.1.5/aixweather/
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 11:18:31.450935 AixWeather-0.1.5/aixweather/core_data_format_2_output_file/
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/core_data_format_2_output_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27093 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/core_data_format_2_output_file/to_epw_energyplus.py
--rw-rw-rw-   0 root         (0) root         (0)    12087 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/core_data_format_2_output_file/to_mos_TMY3.py
--rw-rw-rw-   0 root         (0) root         (0)     5031 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/core_data_format_2_output_file/unconverted_to_x.py
--rw-rw-rw-   0 root         (0) root         (0)     1703 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/data_quality_checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 11:18:31.450935 AixWeather-0.1.5/aixweather/imports/
--rw-rw-rw-   0 root         (0) root         (0)    12879 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/imports/DWD.py
--rw-rw-rw-   0 root         (0) root         (0)     1701 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/imports/EPW.py
--rw-rw-rw-   0 root         (0) root         (0)     4658 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/imports/ERC.py
--rw-rw-rw-   0 root         (0) root         (0)     5560 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/imports/TRY.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/imports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/imports/custom_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/imports/utils_import.py
--rw-rw-rw-   0 root         (0) root         (0)    15038 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/project_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 11:18:31.450935 AixWeather-0.1.5/aixweather/transformation_functions/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_functions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5321 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_functions/auxiliary.py
--rw-rw-rw-   0 root         (0) root         (0)     9673 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_functions/pass_through_handling.py
--rw-rw-rw-   0 root         (0) root         (0)     4778 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_functions/time_observation_transformations.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_functions/unit_conversions.py
--rw-rw-rw-   0 root         (0) root         (0)    11311 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_functions/variable_transformations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 11:18:31.450935 AixWeather-0.1.5/aixweather/transformation_to_core_data/
--rw-rw-rw-   0 root         (0) root         (0)    13247 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_to_core_data/DWD.py
--rw-rw-rw-   0 root         (0) root         (0)     5770 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_to_core_data/EPW.py
--rw-rw-rw-   0 root         (0) root         (0)     4022 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_to_core_data/ERC.py
--rw-rw-rw-   0 root         (0) root         (0)     4946 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_to_core_data/TRY.py
--rw-rw-rw-   0 root         (0) root         (0)      814 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_to_core_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3095 2024-03-01 11:09:21.000000 AixWeather-0.1.5/aixweather/transformation_to_core_data/custom_file.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-01 11:18:31.454935 AixWeather-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2587 2024-03-01 11:09:22.000000 AixWeather-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 11:18:31.450935 AixWeather-0.1.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3337 2024-03-01 11:09:22.000000 AixWeather-0.1.5/tests/test_DWD_forecast.py
--rw-rw-rw-   0 root         (0) root         (0)     3245 2024-03-01 11:09:22.000000 AixWeather-0.1.5/tests/test_DWD_historical.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2024-03-01 11:09:22.000000 AixWeather-0.1.5/tests/test_EPW.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-03-01 11:09:22.000000 AixWeather-0.1.5/tests/test_ERC.py
--rw-rw-rw-   0 root         (0) root         (0)     2184 2024-03-01 11:09:22.000000 AixWeather-0.1.5/tests/test_TRY.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2024-03-01 11:09:22.000000 AixWeather-0.1.5/tests/test_output_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.808354 aixweather-0.1.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.808354 aixweather-0.1.6/AixWeather.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8385 2024-05-02 16:25:20.000000 aixweather-0.1.6/AixWeather.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-05-02 16:25:20.000000 aixweather-0.1.6/AixWeather.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 16:25:20.000000 aixweather-0.1.6/AixWeather.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      233 2024-05-02 16:25:20.000000 aixweather-0.1.6/AixWeather.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-02 16:25:20.000000 aixweather-0.1.6/AixWeather.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2024-05-02 15:56:22.000000 aixweather-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8385 2024-05-02 16:25:20.808354 aixweather-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6882 2024-05-02 15:56:22.000000 aixweather-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.804354 aixweather-0.1.6/aixweather/
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-02 16:12:55.000000 aixweather-0.1.6/aixweather/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.804354 aixweather-0.1.6/aixweather/core_data_format_2_output_file/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/core_data_format_2_output_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27093 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/core_data_format_2_output_file/to_epw_energyplus.py
+-rw-rw-rw-   0 root         (0) root         (0)    12087 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/core_data_format_2_output_file/to_mos_TMY3.py
+-rw-rw-rw-   0 root         (0) root         (0)     5031 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/core_data_format_2_output_file/unconverted_to_x.py
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/data_quality_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.804354 aixweather-0.1.6/aixweather/imports/
+-rw-rw-rw-   0 root         (0) root         (0)    12879 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/DWD.py
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/EPW.py
+-rw-rw-rw-   0 root         (0) root         (0)     4658 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/ERC.py
+-rw-rw-rw-   0 root         (0) root         (0)     5597 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/TRY.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/custom_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/imports/utils_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    15038 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/project_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.804354 aixweather-0.1.6/aixweather/transformation_functions/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5321 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/auxiliary.py
+-rw-rw-rw-   0 root         (0) root         (0)     9673 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/pass_through_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/time_observation_transformations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/unit_conversions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11311 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_functions/variable_transformations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.808354 aixweather-0.1.6/aixweather/transformation_to_core_data/
+-rw-rw-rw-   0 root         (0) root         (0)    13247 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/DWD.py
+-rw-rw-rw-   0 root         (0) root         (0)     5770 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/EPW.py
+-rw-rw-rw-   0 root         (0) root         (0)     4022 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/ERC.py
+-rw-rw-rw-   0 root         (0) root         (0)     4946 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/TRY.py
+-rw-rw-rw-   0 root         (0) root         (0)      814 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2024-05-02 15:56:22.000000 aixweather-0.1.6/aixweather/transformation_to_core_data/custom_file.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 16:25:20.808354 aixweather-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2024-05-02 15:56:23.000000 aixweather-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 16:25:20.808354 aixweather-0.1.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3337 2024-05-02 15:56:23.000000 aixweather-0.1.6/tests/test_DWD_forecast.py
+-rw-rw-rw-   0 root         (0) root         (0)     3245 2024-05-02 15:56:23.000000 aixweather-0.1.6/tests/test_DWD_historical.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2024-05-02 15:56:23.000000 aixweather-0.1.6/tests/test_EPW.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-02 15:56:23.000000 aixweather-0.1.6/tests/test_ERC.py
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2024-05-02 15:56:23.000000 aixweather-0.1.6/tests/test_TRY.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2024-05-02 15:56:24.000000 aixweather-0.1.6/tests/test_output_functions.py
```

### Comparing `AixWeather-0.1.5/AixWeather.egg-info/PKG-INFO` & `aixweather-0.1.6/AixWeather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: AixWeather
-Version: 0.1.5
+Version: 0.1.6
 Summary: A weather data generation tool for building energy system simulations.Pull, Transform, Export.
 Home-page: https://github.com/RWTH-EBC/AixWeather
-Download-URL: https://github.com/RWTH-EBC/AixWeather/archive/refs/tags/0.1.5.tar.gz
+Download-URL: https://github.com/RWTH-EBC/AixWeather/archive/refs/tags/0.1.6.tar.gz
 Author: RWTH Aachen University, E.ON Energy Research Center, Institute of Energy Efficient Buildings and Indoor Climate
 Author-email: ebc-abos@eonerc.rwth-aachen.de
 License: BSD 3-Clause
 Keywords: weather,BES,converter,simulation,building,energy
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
@@ -20,14 +20,15 @@
 Requires-Dist: unidecode~=1.3.7
 Requires-Dist: pvlib~=0.10.2
 Requires-Dist: matplotlib~=3.8.1
 Requires-Dist: seaborn~=0.13.0
 Provides-Extra: try
 Requires-Dist: geopandas~=0.14.0; extra == "try"
 Requires-Dist: geopy~=2.4.0; extra == "try"
+Requires-Dist: shapely~=2.0.3; extra == "try"
 Provides-Extra: dwd-forecast
 Requires-Dist: wetterdienst<=0.72.0,>=0.65.0; extra == "dwd-forecast"
 Provides-Extra: full
 Requires-Dist: wetterdienst<=0.72.0,>=0.65.0; extra == "full"
 Requires-Dist: geopandas~=0.14.0; extra == "full"
 Requires-Dist: geopy~=2.4.0; extra == "full"
```

### Comparing `AixWeather-0.1.5/AixWeather.egg-info/SOURCES.txt` & `aixweather-0.1.6/AixWeather.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/LICENSE` & `aixweather-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/PKG-INFO` & `aixweather-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: AixWeather
-Version: 0.1.5
+Version: 0.1.6
 Summary: A weather data generation tool for building energy system simulations.Pull, Transform, Export.
 Home-page: https://github.com/RWTH-EBC/AixWeather
-Download-URL: https://github.com/RWTH-EBC/AixWeather/archive/refs/tags/0.1.5.tar.gz
+Download-URL: https://github.com/RWTH-EBC/AixWeather/archive/refs/tags/0.1.6.tar.gz
 Author: RWTH Aachen University, E.ON Energy Research Center, Institute of Energy Efficient Buildings and Indoor Climate
 Author-email: ebc-abos@eonerc.rwth-aachen.de
 License: BSD 3-Clause
 Keywords: weather,BES,converter,simulation,building,energy
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
@@ -20,14 +20,15 @@
 Requires-Dist: unidecode~=1.3.7
 Requires-Dist: pvlib~=0.10.2
 Requires-Dist: matplotlib~=3.8.1
 Requires-Dist: seaborn~=0.13.0
 Provides-Extra: try
 Requires-Dist: geopandas~=0.14.0; extra == "try"
 Requires-Dist: geopy~=2.4.0; extra == "try"
+Requires-Dist: shapely~=2.0.3; extra == "try"
 Provides-Extra: dwd-forecast
 Requires-Dist: wetterdienst<=0.72.0,>=0.65.0; extra == "dwd-forecast"
 Provides-Extra: full
 Requires-Dist: wetterdienst<=0.72.0,>=0.65.0; extra == "full"
 Requires-Dist: geopandas~=0.14.0; extra == "full"
 Requires-Dist: geopy~=2.4.0; extra == "full"
```

### Comparing `AixWeather-0.1.5/README.md` & `aixweather-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/core_data_format_2_output_file/to_epw_energyplus.py` & `aixweather-0.1.6/aixweather/core_data_format_2_output_file/to_epw_energyplus.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/core_data_format_2_output_file/to_mos_TMY3.py` & `aixweather-0.1.6/aixweather/core_data_format_2_output_file/to_mos_TMY3.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/core_data_format_2_output_file/unconverted_to_x.py` & `aixweather-0.1.6/aixweather/core_data_format_2_output_file/unconverted_to_x.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/data_quality_checks.py` & `aixweather-0.1.6/aixweather/data_quality_checks.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/definitions.py` & `aixweather-0.1.6/aixweather/definitions.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/imports/DWD.py` & `aixweather-0.1.6/aixweather/imports/DWD.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/imports/EPW.py` & `aixweather-0.1.6/aixweather/imports/EPW.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/imports/ERC.py` & `aixweather-0.1.6/aixweather/imports/ERC.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/imports/TRY.py` & `aixweather-0.1.6/aixweather/imports/TRY.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import DWD TRY data
 """
 
 import re
 import pandas as pd
 import random
 
-from shapely.geometry import Point
-
 from aixweather.imports.utils_import import MetaData
 
 
 def _handle_TRY_type(path: str) -> tuple:
     """
     Determine the TRY format type based on the provided file path.
 
@@ -98,16 +96,18 @@
     # Extract Höhenlage (altitude)
     hoehenlage_line = next(line for line in header_lines if "Hoehenlage" in line)
     hoehenlage = int(re.search(r":\s*(\d+) Meter", hoehenlage_line).group(1))
 
     try:
         import geopandas as gpd
         from geopy.geocoders import Nominatim
-    except ImportError:
-        print("Optional dependency 'TRY' not installed, skipping metadata of TRY.")
+        from shapely.geometry import Point
+    except ImportError as err:
+        print("Optional dependency 'TRY' not installed, "
+              "skipping metadata of TRY. ImportError:", err)
         return meta
 
     ### convert latitude and longitude
     # Create a GeoDataFrame with the provided coordinates
     # (using pyproj directly led to wrong calculation)
     gdf = gpd.GeoDataFrame(
         {"geometry": [Point(rechtswert, hochwert)]},
@@ -170,15 +170,15 @@
 
     TRY_year, header_row = _handle_TRY_type(path)
 
     ### load file to Dataframe
     weather_df = pd.read_table(
         filepath_or_buffer=path,
         header=header_row,
-        delim_whitespace=True,
+        sep='\s+',
         skip_blank_lines=False,
         encoding="latin",
     )
     # drop first row cause empty
     weather_df = weather_df.iloc[1:]
 
     return weather_df
```

### Comparing `AixWeather-0.1.5/aixweather/imports/custom_file.py` & `aixweather-0.1.6/aixweather/imports/custom_file.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/imports/utils_import.py` & `aixweather-0.1.6/aixweather/imports/utils_import.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/project_class.py` & `aixweather-0.1.6/aixweather/project_class.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/transformation_functions/auxiliary.py` & `aixweather-0.1.6/aixweather/transformation_functions/auxiliary.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/transformation_functions/pass_through_handling.py` & `aixweather-0.1.6/aixweather/transformation_functions/pass_through_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,22 +179,22 @@
         if core_name in output_format:
             suffix = col[len(core_name) :]
             if (
                 suffix in suffix_mapping_forward
                 and output_format[core_name]["time_of_meas_shift"]
                 == suffix_mapping_forward[suffix]
             ):
-                df.loc[:, col] = df[col].shift(periods=1, freq="H", axis=0)
+                df.loc[:, col] = df[col].shift(periods=1, freq="h", axis=0)
                 selected_columns.append(col)
             elif (
                 suffix in suffix_mapping_backward
                 and output_format[core_name]["time_of_meas_shift"]
                 == suffix_mapping_backward[suffix]
             ):
-                df.loc[:, col] = df[col].shift(periods=-1, freq="H", axis=0)
+                df.loc[:, col] = df[col].shift(periods=-1, freq="h", axis=0)
                 selected_columns.append(col)
 
     return selected_columns, df
 
 
 def pass_through_measurements_with_back_and_forth_interpolating(
     core2output_df: pd.DataFrame, format_outputter: dict
```

### Comparing `AixWeather-0.1.5/aixweather/transformation_functions/time_observation_transformations.py` & `aixweather-0.1.6/aixweather/transformation_functions/time_observation_transformations.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/transformation_functions/unit_conversions.py` & `aixweather-0.1.6/aixweather/transformation_functions/unit_conversions.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/transformation_functions/variable_transformations.py` & `aixweather-0.1.6/aixweather/transformation_functions/variable_transformations.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/transformation_to_core_data/DWD.py` & `aixweather-0.1.6/aixweather/transformation_to_core_data/DWD.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,18 +156,18 @@
 
     # delete dummy values from DWD
     df = auxiliary.replace_dummy_with_nan(df, format_DWD_historical)
 
     # resample some via sum some via mean -> results in average of following hour
     for var in df.columns:
         if var in variables_to_sum_DWD_historical:
-            df[var] = df[var].resample("H").sum(min_count=1)  # fills nan only if 1 value in interval
+            df[var] = df[var].resample("h").sum(min_count=1)  # fills nan only if 1 value in interval
         else:
-            df[var] = df[var].resample("H").mean()  # fills nan only if all nan in interval
-    df = df.resample("H").first()  # only keep the previously resampled value
+            df[var] = df[var].resample("h").mean()  # fills nan only if all nan in interval
+    df = df.resample("h").first()  # only keep the previously resampled value
 
     # rename available variables to core data format
     df = auxiliary.rename_columns(df, format_DWD_historical)
 
     ### convert timezone to UTC
     # the data is for most stations and datasets, as well as for more recent
     # data (several years) in UTC. For more sophisticated handling pull meta
@@ -224,15 +224,15 @@
     auxiliary.evaluate_transformations(
         core_format=definitions.format_core_data, other_format=format_DWD_forecast
     )
 
     ### format raw data for further operations
     df = df_import.copy()
     # Resample the DataFrame to make the DatetimeIndex complete and monotonic
-    df = df.resample('H').asfreq()
+    df = df.resample('h').asfreq()
     # delete timezone information
     df = df.tz_localize(None)
     # rename available variables to core data format
     df = auxiliary.rename_columns(df, format_DWD_forecast)
 
     ### convert timezone to UTC
     # the data pulled by Wetterdienst is already UTC
```

### Comparing `AixWeather-0.1.5/aixweather/transformation_to_core_data/EPW.py` & `aixweather-0.1.6/aixweather/transformation_to_core_data/EPW.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,24 +105,24 @@
         return df
 
     ### preprocessing raw data for further operations
     df = df_import.copy()
     df = if_TMY_convert_to_one_year(df)
     df = epw_to_datetimeindex(df)
     # Resample the DataFrame to make the DatetimeIndex complete and monotonic
-    df = df.resample("H").asfreq()
+    df = df.resample("h").asfreq()
     # give names to columns according to documentation of import data
     df.columns = [key for key in format_epw.keys()]
     # rename available variables to core data format
     df = auxiliary.rename_columns(df, format_epw)
     # delete dummy values from EPW
     df = auxiliary.replace_dummy_with_nan(df, format_epw)
 
     ### convert timezone to UTC+0
-    df = df.shift(periods=-meta.timezone, freq="H", axis=0)
+    df = df.shift(periods=-meta.timezone, freq="h", axis=0)
 
     ### shift and interpolate data forward 30mins or backward -30mins
     df_no_shift = df.copy()
     df = time_observation_transformations.shift_time_by_dict(format_epw, df)
 
     def transform(df):
         ### force variable naming format_core_data
```

### Comparing `AixWeather-0.1.5/aixweather/transformation_to_core_data/ERC.py` & `aixweather-0.1.6/aixweather/transformation_to_core_data/ERC.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     auxiliary.evaluate_transformations(
         core_format=definitions.format_core_data, other_format=format_ERC
     )
 
     ### format raw data for further operations
     df = df_import.copy()
     # Resample the DataFrame to make the DatetimeIndex complete and monotonic
-    df = df.resample('H').asfreq()
+    df = df.resample('h').asfreq()
     # Remove timezone awareness
     df.index = df.index.tz_localize(None)
     # rename available variables to core data format
     df = auxiliary.rename_columns(df, format_ERC)
 
     ### convert timezone to UTC
     # data is UTC
```

### Comparing `AixWeather-0.1.5/aixweather/transformation_to_core_data/TRY.py` & `aixweather-0.1.6/aixweather/transformation_to_core_data/TRY.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,28 +69,28 @@
         )
         # data is shifted by -1 H to satisfy pandas timestamp
         # hours in pandas only between 0 and 23, in TRY between 1 and 24
         # converts to pandas timestamps if desired
         df.index = pd.to_datetime(time_index)
         # data is shifted back to original to start: back to
         # 2017-01-01 01:00:00 instead of the temporary 2017-01-01 00:00:00
-        df = df.shift(periods=1, freq="H", axis=0)
+        df = df.shift(periods=1, freq="h", axis=0)
 
         return df
 
     ### preprocessing raw data for further operations
     df = df_import.copy()
     df = TRY_to_datetimeindex(df, meta)
     # Resample the DataFrame to make the DatetimeIndex complete and monotonic
-    df = df.resample('H').asfreq()
+    df = df.resample('h').asfreq()
     # rename available variables to core data format
     df = auxiliary.rename_columns(df, format_TRY_15_45)
 
     ### convert timezone to UTC+0
-    df = df.shift(periods=-1, freq="H", axis=0)
+    df = df.shift(periods=-1, freq="h", axis=0)
 
     ### shift and interpolate data forward 30mins or backward -30mins
     df_no_shift = df.copy()
     df = time_observation_transformations.shift_time_by_dict(format_TRY_15_45, df)
 
     def transform_TRY(df):
         # drop unnecessary variables
```

### Comparing `AixWeather-0.1.5/aixweather/transformation_to_core_data/__init__.py` & `aixweather-0.1.6/aixweather/transformation_to_core_data/__init__.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/aixweather/transformation_to_core_data/custom_file.py` & `aixweather-0.1.6/aixweather/transformation_to_core_data/custom_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,20 +36,20 @@
     auxiliary.evaluate_transformations(
         core_format=definitions.format_core_data, other_format=format_costum
     )
 
     ### preprocessing raw data for further operations
     df = df_import.copy()
     # Resample the DataFrame to make the DatetimeIndex complete and monotonic
-    df = df.resample('H').asfreq()
+    df = df.resample('h').asfreq()
     # rename available variables to core data format
     df = auxiliary.rename_columns(df, format_costum)
 
     ### convert timezone to UTC+0 -> change periods accordingly
-    df = df.shift(periods=0, freq="H", axis=0)
+    df = df.shift(periods=0, freq="h", axis=0)
 
     ### shift and interpolate data forward 30mins or backward -30mins
     df_no_shift = df.copy()
     df = time_observation_transformations.shift_time_by_dict(
         format_costum, df
     )
```

### Comparing `AixWeather-0.1.5/setup.py` & `aixweather-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "matplotlib~=3.8.1",
     "seaborn~=0.13.0",
 ]
 EXTRAS_REQUIRE = {
     'TRY': [
         "geopandas~=0.14.0",
         "geopy~=2.4.0",
+        "shapely~=2.0.3"
     ],
     "DWD_forecast": ["wetterdienst>=0.65.0,<=0.72.0"],
     "full": [
         "wetterdienst>=0.65.0,<=0.72.0",
         "geopandas~=0.14.0",
         "geopy~=2.4.0",
     ]
```

### Comparing `AixWeather-0.1.5/tests/test_DWD_forecast.py` & `aixweather-0.1.6/tests/test_DWD_forecast.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/tests/test_DWD_historical.py` & `aixweather-0.1.6/tests/test_DWD_historical.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/tests/test_EPW.py` & `aixweather-0.1.6/tests/test_EPW.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/tests/test_ERC.py` & `aixweather-0.1.6/tests/test_ERC.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/tests/test_TRY.py` & `aixweather-0.1.6/tests/test_TRY.py`

 * *Files identical despite different names*

### Comparing `AixWeather-0.1.5/tests/test_output_functions.py` & `aixweather-0.1.6/tests/test_output_functions.py`

 * *Files identical despite different names*

