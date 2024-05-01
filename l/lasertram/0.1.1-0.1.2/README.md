# Comparing `tmp/lasertram-0.1.1.tar.gz` & `tmp/lasertram-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasertram-0.1.1.tar", last modified: Mon Apr 29 19:30:33 2024, max compression
+gzip compressed data, was "lasertram-0.1.2.tar", last modified: Wed May  1 23:01:30 2024, max compression
```

## Comparing `lasertram-0.1.1.tar` & `lasertram-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-29 19:30:29.000000 lasertram-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-29 19:30:33.096996 lasertram-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-29 19:30:29.000000 lasertram-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/lasertram/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/lasertram/calc/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31599 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/calc/calc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/lasertram/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/helpers/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/helpers/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/lasertram/tram/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/tram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/tram/tram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/lasertram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-29 19:30:33.000000 lasertram-0.1.1/lasertram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-29 19:30:33.000000 lasertram-0.1.1/lasertram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:30:33.000000 lasertram-0.1.1/lasertram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 19:30:33.000000 lasertram-0.1.1/lasertram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 19:30:33.000000 lasertram-0.1.1/lasertram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 19:30:29.000000 lasertram-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-29 19:30:33.100996 lasertram-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    37829 2024-04-29 19:30:29.000000 lasertram-0.1.1/tests/test_lasertram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.568239 lasertram-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 23:01:26.000000 lasertram-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-01 23:01:30.568239 lasertram-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-01 23:01:26.000000 lasertram-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.564239 lasertram-0.1.2/lasertram/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.564239 lasertram-0.1.2/lasertram/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31599 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/calc/calc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.568239 lasertram-0.1.2/lasertram/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/helpers/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/helpers/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.568239 lasertram-0.1.2/lasertram/tram/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/tram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-05-01 23:01:26.000000 lasertram-0.1.2/lasertram/tram/tram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.568239 lasertram-0.1.2/lasertram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-01 23:01:30.000000 lasertram-0.1.2/lasertram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-01 23:01:30.000000 lasertram-0.1.2/lasertram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:01:30.000000 lasertram-0.1.2/lasertram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-01 23:01:30.000000 lasertram-0.1.2/lasertram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 23:01:30.000000 lasertram-0.1.2/lasertram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 23:01:26.000000 lasertram-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-01 23:01:30.568239 lasertram-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:01:30.568239 lasertram-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-05-01 23:01:26.000000 lasertram-0.1.2/tests/test_lasertram.py
```

### Comparing `lasertram-0.1.1/LICENSE` & `lasertram-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.1/PKG-INFO` & `lasertram-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasertram
-Version: 0.1.1
+Version: 0.1.2
 Summary: For processing LA-ICP-MS data
 Home-page: https://github.com/jlubbersgeo/lasertram
 Author: Jordan Lubbers
 Author-email: jelubber@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `lasertram-0.1.1/README.md` & `lasertram-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.1/lasertram/calc/calc.py` & `lasertram-0.1.2/lasertram/calc/calc.py`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.1/lasertram/helpers/batch.py` & `lasertram-0.1.2/lasertram/helpers/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     so a spot can be processed in an efficient and compact way.
 
     Args:
         spot (LaserTRAM spot object): an empty `LaserTRAM` spot object to be processed
         raw_data (pandas DataFrame): the raw counts per second dataframe to be assigned to the spot. Shape is (m x n) where m is the number of cycles through the mass range
         bkgd (tuple): (start, stop) pair of values corresponding to the analysis time where the background signal starts and stops
         keep (tuple): (start, stop) pair of values correpsonding to the analysis time where the interval signal for concentrations starts and stops
-        internal_std (str): column name for the internal standard analyte (e.g., 29Si)
+        int_std (str): column name for the internal standard analyte (e.g., 29Si)
         omit (tuple): (start, stop) pair of values corresponding to the analysis time to be omitted from the `keep` interval. Defaults to None.
         despike (bool, optional): Whether or not to despike all analyte signals using the standard deviation filter from `LaserTRAM.despike_data()`. Defaults to False
         output_report (bool, optional): Whether or not to create a 1-row pandas DataFrame output report in the following format. Defaults to True.
 
 
     """
     # assign data to the spot
```

### Comparing `lasertram-0.1.1/lasertram/helpers/conversions.py` & `lasertram-0.1.2/lasertram/helpers/conversions.py`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.1/lasertram/tram/tram.py` & `lasertram-0.1.2/lasertram/tram/tram.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 interval to be turned into a concentration, normalizing
 that interval to an internal standard and outputting that value + other
 metadata
 
 
 """
 
+import warnings
+
 import numpy as np
 import pandas as pd
 
 
 class LaserTRAM:
     """
     # LaserTRAM
@@ -285,25 +287,35 @@
                 despiked_signal[spikes] = signal_mean[spikes]
                 signal = despiked_signal
 
             return signal
 
         self.despiked = True
 
+        # analyte_list = "all"  # currently only supports despiking every element
+
         if analyte_list == "all":
             filter_list = self.analytes
         else:
-            if analyte_list is not type(list):
-                filter_list = [analyte_list]
-            else:
-                filter_list = analyte_list
+            warnings.warn(
+                "single element despiking currently not supported, falling back to 'all'"
+            )
+            # # this
+            # if analyte_list is not type(list):
+            #     filter_list = [analyte_list]
+            # else:
+            #     filter_list = analyte_list
+            filter_list = self.analytes
 
         self.despiked_elements = filter_list
         despiked = []
         for analyte in filter_list:
             despiked.append(despike_signal(self.data, analyte))
 
-        despiked = pd.DataFrame(np.array(despiked).T, columns=self.analytes)
+        despiked = pd.DataFrame(
+            np.array(despiked).T, columns=self.analytes, index=self.data.index
+        )
+        despiked.index.name = self.data.index.name
         despiked.insert(0, "Time", self.data["Time"])
 
         self.data = despiked
         self.data_matrix = despiked.to_numpy()
```

### Comparing `lasertram-0.1.1/lasertram.egg-info/PKG-INFO` & `lasertram-0.1.2/lasertram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasertram
-Version: 0.1.1
+Version: 0.1.2
 Summary: For processing LA-ICP-MS data
 Home-page: https://github.com/jlubbersgeo/lasertram
 Author: Jordan Lubbers
 Author-email: jelubber@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `lasertram-0.1.1/setup.cfg` & `lasertram-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.1/tests/test_lasertram.py` & `lasertram-0.1.2/tests/test_lasertram.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,59 @@
                 51.42615343,
                 287.19571818,
             ]
         ),
     ), "detection limits not calculated correctly"
 
 
+def test_despike_data(load_data):
+    """
+    test to make sure data are despiked properly
+    """
+
+    spot = LaserTRAM(name="test")
+
+    samples = load_data.index.unique().dropna().tolist()
+
+    spot.get_data(load_data.loc[samples[0], :])
+
+    spot.assign_int_std("29Si")
+
+    bkgd_interval = (5, 10)
+    keep_interval = (20, 50)
+    omit_interval = (30, 35)
+
+    spot.assign_intervals(bkgd=bkgd_interval, keep=keep_interval, omit=omit_interval)
+    spot.get_bkgd_data()
+    spot.get_detection_limits()
+    spot.despike_data()
+
+    assert np.allclose(
+        spot.data_matrix[100],
+        np.array(
+            [
+                1.50457600e01,
+                8.00256082e03,
+                8.59074455e06,
+                3.89750189e07,
+                3.14335647e06,
+                1.11394144e05,
+                1.49526253e07,
+                4.07430164e06,
+                1.15808129e06,
+                2.17770296e06,
+                8.97208417e04,
+                2.42736116e05,
+                7.20207420e03,
+                3.48485091e04,
+            ]
+        ),
+    ), "data not despiked properly"
+
+
 def test_normalize_interval(load_data):
     """
     check that data are being normalized correctly
     """
     spot = LaserTRAM(name="test")
 
     samples = load_data.index.unique().dropna().tolist()
@@ -1300,7 +1345,115 @@
         check_index_type=False,
     )
     pd.testing.assert_frame_equal(
         test_SRM_concentrations,
         concentrations.SRM_concentrations.iloc[[0, 1, 18, 19], :],
         check_index_type=False,
     )
+
+
+def test_SRM_accuracies(load_SRM_data, load_LTcomplete_data):
+    concentrations = LaserCalc(name="test")
+    concentrations.get_SRM_comps(load_SRM_data)
+    concentrations.get_data(load_LTcomplete_data)
+    concentrations.set_calibration_standard("BCR-2G")
+    concentrations.drift_check()
+    concentrations.get_calibration_std_ratios()
+    concentrations.set_int_std_concentrations(
+        concentrations.data["Spot"],
+        np.full(concentrations.data["Spot"].shape[0], 71.9),
+        np.full(concentrations.data["Spot"].shape[0], 1),
+    )
+    concentrations.calculate_concentrations()
+    concentrations.get_secondary_standard_accuracies()
+
+    test_SRM_accuracies = pd.DataFrame(
+        {
+            "timestamp": [
+                "2021-03-01T22:10:47.999000000",
+                "2021-03-01T22:12:05.000000000",
+                "2021-03-02T02:41:28.000000000",
+                "2021-03-02T02:42:45.999000000",
+            ],
+            "Spot": ["ATHO-G_1", "ATHO-G_2", "BHVO-2G_4", "BHVO-2G_5"],
+            "7Li": [
+                90.2707698781551,
+                90.40056727503291,
+                91.46802760728896,
+                97.2945927279642,
+            ],
+            "24Mg": [
+                93.23275958900813,
+                92.77825774894306,
+                103.18161415638338,
+                103.01753694150116,
+            ],
+            "27Al": [
+                103.10756771923903,
+                102.48851200312427,
+                99.7040383658651,
+                99.45098674583244,
+            ],
+            "29Si": [
+                100.77763624095759,
+                99.7930880605041,
+                105.9608257416244,
+                106.87344282267848,
+            ],
+            "43Ca": [100.0, 100.0, 100.0, 100.0],
+            "48Ti": [
+                101.18478182683648,
+                101.72851950388984,
+                103.24672042436633,
+                102.81441448062434,
+            ],
+            "57Fe": [
+                95.87003025946926,
+                94.96514065655767,
+                100.91422654205039,
+                101.12705638453254,
+            ],
+            "88Sr": [
+                101.94922271980967,
+                101.79345213369966,
+                101.65691193515897,
+                102.53223608014466,
+            ],
+            "138Ba": [
+                100.20043393612958,
+                100.62315209040588,
+                100.72415209391778,
+                100.87285503119428,
+            ],
+            "139La": [
+                102.52598726771596,
+                103.30640634591504,
+                100.55332259697359,
+                99.95834378627933,
+            ],
+            "140Ce": [
+                100.07191920724449,
+                101.58231624812865,
+                99.65017074334447,
+                99.34575547286384,
+            ],
+            "153Eu": [
+                101.18468125418963,
+                102.2406071182077,
+                100.33150971481345,
+                102.23629678402409,
+            ],
+            "208Pb": [
+                99.46689464030175,
+                100.77049884455356,
+                110.39576303999246,
+                114.77739986325912,
+            ],
+        }
+    )
+    test_SRM_accuracies.index = ["ATHO-G", "ATHO-G", "BHVO-2G", "BHVO-2G"]
+    test_SRM_accuracies.index.name = "sample"
+
+    pd.testing.assert_frame_equal(
+        test_SRM_accuracies,
+        concentrations.SRM_accuracies.iloc[[0, 1, 18, 19], :],
+    )
```

