# Comparing `tmp/liveisstracker-1.1.7.tar.gz` & `tmp/liveisstracker-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/liveisstracker-1.1.7.tar", last modified: Sun Feb  4 11:27:39 2024, max compression
+gzip compressed data, was "dist/liveisstracker-1.1.8.tar", last modified: Thu May  2 10:02:17 2024, max compression
```

## Comparing `liveisstracker-1.1.7.tar` & `liveisstracker-1.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/
--rw-r--r--   0 root         (0) root         (0)       56 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3304 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2287 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/PlotMap/
--rw-r--r--   0 root         (0) root         (0)     2903 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/PlotMap/MapBasePlot.py
--rw-r--r--   0 root         (0) root         (0)     2020 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/PlotMap/PlotlyFig.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/PlotMap/__init__.py
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3365 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/command_line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/dbsql/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/dbsql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2271 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/dbsql/dbconnections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/issTrack/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/issTrack/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5481 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/issTrack/issTracking.py
--rw-r--r--   0 root         (0) root         (0)     3242 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/issTrack/page_information.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/mylogger/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/mylogger/__init__.py
--rw-r--r--   0 root         (0) root         (0)      350 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/mylogger/iss_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/tests/
--rw-r--r--   0 root         (0) root         (0)      749 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2929 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/tests/test_iss.py
--rw-r--r--   0 root         (0) root         (0)     2794 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker/track_iss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3304 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      170 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/liveisstracker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      232 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1315 2024-02-04 11:27:39.000000 liveisstracker-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3304 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2287 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker/PlotMap/
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/PlotMap/MapBasePlot.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/PlotMap/PlotlyFig.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/PlotMap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/command_line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker/dbsql/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/dbsql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/dbsql/dbconnections.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker/issTrack/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/issTrack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/issTrack/issTracking.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/issTrack/page_information.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker/mylogger/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/mylogger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      350 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/mylogger/iss_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker/tests/
+-rw-r--r--   0 root         (0) root         (0)      749 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/tests/test_iss.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/liveisstracker/track_iss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3304 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/liveisstracker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 10:02:17.000000 liveisstracker-1.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1315 2024-05-02 10:02:16.000000 liveisstracker-1.1.8/setup.py
```

### Comparing `liveisstracker-1.1.7/PKG-INFO` & `liveisstracker-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: liveisstracker
-Version: 1.1.7
+Version: 1.1.8
 Summary: A CLI to get the current position, speed, passing country and image of the location of International Space Station on a map [#liveisstracker]. Source: LiveIssTracker Project from https://gitlab.com/manojm18/liveisstracker.
 Home-page: https://github.com/manojmanivannan
 Author: Manoj Manivannan
 Author-email: manojm18@live.in
 License: UNKNOWN
 Description: Live ISS Tracker
         ================
```

### Comparing `liveisstracker-1.1.7/README.rst` & `liveisstracker-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `liveisstracker-1.1.7/liveisstracker/PlotMap/MapBasePlot.py` & `liveisstracker-1.1.8/liveisstracker/PlotMap/MapBasePlot.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             format(\
                 round(self.gps_location['latitude'],2),\
                 round(self.gps_location['longitude'],2)))
 
         distance_to_home = TrackerISS.get_distance_btwn_locations(location_1 = (self.home_latitude, self.home_longitude),\
                                                                     location_2 = iss)
          
-        location = Nominatim(user_agent="my-application",timeout=3)\
+        location = Nominatim(user_agent="liveiss-application",timeout=3)\
         .reverse('{},{}'.format(self.gps_location['latitude'],\
             self.gps_location['longitude']), language='en')
         try:
             country = location.raw['address']['country']
         except KeyError:
             country = 'the ocean'
```

### Comparing `liveisstracker-1.1.7/liveisstracker/PlotMap/PlotlyFig.py` & `liveisstracker-1.1.8/liveisstracker/PlotMap/PlotlyFig.py`

 * *Files identical despite different names*

### Comparing `liveisstracker-1.1.7/liveisstracker/command_line.py` & `liveisstracker-1.1.8/liveisstracker/command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         except  Exception as e:
             speed = 99999999999
 
         print(f'Ground Speed of International Space Station is ~ {round(speed,2)} Km/h')
 
     if get_country:
 
-        geolocator = Nominatim(user_agent="my-application",timeout=3).reverse(f'{location["latitude"]},{location["longitude"]}',language='en')
+        geolocator = Nominatim(user_agent="liveiss-application",timeout=3).reverse(f'{location["latitude"]},{location["longitude"]}',language='en')
         
         try:
             country = geolocator.raw['address']['country']
         except KeyError:
             country = 'the ocean'
 
         print(f'Internaionl Space Station is currently above {country}')
```

### Comparing `liveisstracker-1.1.7/liveisstracker/dbsql/dbconnections.py` & `liveisstracker-1.1.8/liveisstracker/dbsql/dbconnections.py`

 * *Files identical despite different names*

### Comparing `liveisstracker-1.1.7/liveisstracker/issTrack/issTracking.py` & `liveisstracker-1.1.8/liveisstracker/issTrack/issTracking.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     from dbsql.dbconnections import *
 except ModuleNotFoundError:
     try:
         from liveisstracker.dbsql.dbconnections import *
     except:
         logger.debug('No DB connection capabilities imported')
 
-geolocator = Nominatim(user_agent="my-application",timeout=3)
+geolocator = Nominatim(user_agent="my-app",timeout=3)
 
 
 def get_city_location(city_name):
     try:
         location = geolocator.geocode(city_name)
         if not location:
             logger.error(f'"{city_name}" is not a valid city name')
```

### Comparing `liveisstracker-1.1.7/liveisstracker/issTrack/page_information.py` & `liveisstracker-1.1.8/liveisstracker/issTrack/page_information.py`

 * *Files identical despite different names*

### Comparing `liveisstracker-1.1.7/liveisstracker/tests/__init__.py` & `liveisstracker-1.1.8/liveisstracker/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `liveisstracker-1.1.7/liveisstracker/tests/test_iss.py` & `liveisstracker-1.1.8/liveisstracker/tests/test_iss.py`

 * *Files identical despite different names*

### Comparing `liveisstracker-1.1.7/liveisstracker/track_iss.py` & `liveisstracker-1.1.8/liveisstracker/track_iss.py`

 * *Files identical despite different names*

### Comparing `liveisstracker-1.1.7/liveisstracker.egg-info/PKG-INFO` & `liveisstracker-1.1.8/liveisstracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: liveisstracker
-Version: 1.1.7
+Version: 1.1.8
 Summary: A CLI to get the current position, speed, passing country and image of the location of International Space Station on a map [#liveisstracker]. Source: LiveIssTracker Project from https://gitlab.com/manojm18/liveisstracker.
 Home-page: https://github.com/manojmanivannan
 Author: Manoj Manivannan
 Author-email: manojm18@live.in
 License: UNKNOWN
 Description: Live ISS Tracker
         ================
```

### Comparing `liveisstracker-1.1.7/liveisstracker.egg-info/SOURCES.txt` & `liveisstracker-1.1.8/liveisstracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveisstracker-1.1.7/setup.py` & `liveisstracker-1.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with io.open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='liveisstracker',
     url='https://github.com/manojmanivannan',
-    version='1.1.7',
+    version='1.1.8',
     author='Manoj Manivannan',
     author_email='manojm18@live.in',
     description='A CLI to get the current position, speed, passing country and image of the location of International Space Station on a map [#liveisstracker]. Source: LiveIssTracker Project from https://gitlab.com/manojm18/liveisstracker.',
     long_description=long_description,
     packages=find_packages(),
     entry_points={
     'console_scripts': ['liveisstracker=liveisstracker.command_line:main'],
```

