# Comparing `tmp/mke_sculib-2.4.0.tar.gz` & `tmp/mke_sculib-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.4.0.tar", last modified: Sun Apr 28 20:12:39 2024, max compression
+gzip compressed data, was "mke_sculib-2.4.1.tar", last modified: Thu May  2 12:36:43 2024, max compression
```

## Comparing `mke_sculib-2.4.0.tar` & `mke_sculib-2.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:39.083726 mke_sculib-2.4.0/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.0/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-04-28 20:12:39.083726 mke_sculib-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.0/README.rst
--rw-rw-rw-   0        0        0      921 2024-04-28 20:12:39.084726 mke_sculib-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:39.059681 mke_sculib-2.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:39.078726 mke_sculib-2.4.0/src/mke_sculib/
--rw-rw-rw-   0        0        0       21 2024-04-28 20:12:03.000000 mke_sculib-2.4.0/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.0/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.0/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.0/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.0/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0    95276 2024-04-28 17:00:01.000000 mke_sculib-2.4.0/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.0/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.0/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:39.081727 mke_sculib-2.4.0/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-04-28 20:12:38.000000 mke_sculib-2.4.0/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2024-04-28 20:12:39.000000 mke_sculib-2.4.0/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 20:12:38.000000 mke_sculib-2.4.0/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-28 20:12:38.000000 mke_sculib-2.4.0/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-28 20:12:39.082727 mke_sculib-2.4.0/tests/
--rw-rw-rw-   0        0        0     9759 2023-12-05 16:11:38.000000 mke_sculib-2.4.0/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.0/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:36:43.357651 mke_sculib-2.4.1/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.1/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-02 12:36:43.357651 mke_sculib-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.1/README.rst
+-rw-rw-rw-   0        0        0      921 2024-05-02 12:36:43.363178 mke_sculib-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:36:43.286105 mke_sculib-2.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 12:36:43.331437 mke_sculib-2.4.1/src/mke_sculib/
+-rw-rw-rw-   0        0        0      173 2024-05-02 12:34:26.000000 mke_sculib-2.4.1/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.1/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.1/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.1/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.1/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0    95276 2024-04-28 17:00:01.000000 mke_sculib-2.4.1/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.1/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.1/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-02 12:36:43.348614 mke_sculib-2.4.1/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-02 12:36:42.000000 mke_sculib-2.4.1/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-05-02 12:36:43.000000 mke_sculib-2.4.1/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 12:36:42.000000 mke_sculib-2.4.1/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 12:36:42.000000 mke_sculib-2.4.1/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 12:36:43.355652 mke_sculib-2.4.1/tests/
+-rw-rw-rw-   0        0        0     9759 2023-12-05 16:11:38.000000 mke_sculib-2.4.1/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.1/tests/test_scu.py
```

### Comparing `mke_sculib-2.4.0/LICENSE` & `mke_sculib-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.0/PKG-INFO` & `mke_sculib-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.4.0
+Version: 2.4.1
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.0/README.rst` & `mke_sculib-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.0/setup.cfg` & `mke_sculib-2.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.0/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.4.1/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.0/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.4.1/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.0/src/mke_sculib/helpers.py` & `mke_sculib-2.4.1/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.0/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.4.1/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.0/src/mke_sculib/scu.py` & `mke_sculib-2.4.1/src/mke_sculib/scu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.0/src/mke_sculib/sim.py` & `mke_sculib-2.4.1/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.0/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.4.1/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.0/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.4.1/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.4.0
+Version: 2.4.1
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.0/tests/test_acu_sim.py` & `mke_sculib-2.4.1/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.0/tests/test_scu.py` & `mke_sculib-2.4.1/tests/test_scu.py`

 * *Files identical despite different names*

