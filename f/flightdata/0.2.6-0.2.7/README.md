# Comparing `tmp/flightdata-0.2.6.tar.gz` & `tmp/flightdata-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightdata-0.2.6.tar", last modified: Thu Apr 18 12:02:58 2024, max compression
+gzip compressed data, was "flightdata-0.2.7.tar", last modified: Wed May  1 08:55:17 2024, max compression
```

## Comparing `flightdata-0.2.6.tar` & `flightdata-0.2.7.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.916330 flightdata-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-18 12:02:27.000000 flightdata-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-18 12:02:58.916330 flightdata-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-18 12:02:27.000000 flightdata-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.908330 flightdata-0.2.6/flightdata/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.912330 flightdata-0.2.6/flightdata/base/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/base/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/base/constructs.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/base/numpy_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15997 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/base/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/coefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.912330 flightdata-0.2.6/flightdata/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/environment/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/environment/wind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.912330 flightdata-0.2.6/flightdata/flight/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/flight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/flight/ardupilot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/flight/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/flight/flight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.912330 flightdata-0.2.6/flightdata/model/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/model/aerodynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/model/thrust.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/origin.py
--rw-r--r--   0 runner    (1001) docker     (127)    21516 2024-04-18 12:02:27.000000 flightdata-0.2.6/flightdata/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.916330 flightdata-0.2.6/flightdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-18 12:02:58.000000 flightdata-0.2.6/flightdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-18 12:02:58.000000 flightdata-0.2.6/flightdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:02:58.000000 flightdata-0.2.6/flightdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 12:02:58.000000 flightdata-0.2.6/flightdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 12:02:58.000000 flightdata-0.2.6/flightdata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.916330 flightdata-0.2.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-18 12:02:27.000000 flightdata-0.2.6/scripts/collect_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-18 12:02:27.000000 flightdata-0.2.6/scripts/flightline.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-18 12:02:58.916330 flightdata-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-18 12:02:27.000000 flightdata-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:02:58.916330 flightdata-0.2.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 12:02:28.000000 flightdata-0.2.6/test/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-18 12:02:28.000000 flightdata-0.2.6/test/test_flight.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-18 12:02:28.000000 flightdata-0.2.6/test/test_origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:17.614077 flightdata-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-01 08:54:51.000000 flightdata-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-01 08:55:17.614077 flightdata-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-01 08:54:51.000000 flightdata-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:17.610077 flightdata-0.2.7/flightdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:17.610077 flightdata-0.2.7/flightdata/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/base/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/base/constructs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/base/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/base/numpy_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/base/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/coefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:17.610077 flightdata-0.2.7/flightdata/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/environment/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/environment/wind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:17.614077 flightdata-0.2.7/flightdata/flight/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/flight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/flight/ardupilot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/flight/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21466 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/flight/flight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/flight/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:17.614077 flightdata-0.2.7/flightdata/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/model/aerodynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/model/thrust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21602 2024-05-01 08:54:51.000000 flightdata-0.2.7/flightdata/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:17.614077 flightdata-0.2.7/flightdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-01 08:55:17.000000 flightdata-0.2.7/flightdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-01 08:55:17.000000 flightdata-0.2.7/flightdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:55:17.000000 flightdata-0.2.7/flightdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 08:55:17.000000 flightdata-0.2.7/flightdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 08:55:17.000000 flightdata-0.2.7/flightdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:17.614077 flightdata-0.2.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-01 08:54:51.000000 flightdata-0.2.7/scripts/collect_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-01 08:54:51.000000 flightdata-0.2.7/scripts/flightline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-01 08:55:17.614077 flightdata-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-01 08:54:51.000000 flightdata-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:55:17.614077 flightdata-0.2.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-01 08:54:52.000000 flightdata-0.2.7/test/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-01 08:54:52.000000 flightdata-0.2.7/test/test_flight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-01 08:54:52.000000 flightdata-0.2.7/test/test_origin.py
```

### Comparing `flightdata-0.2.6/LICENSE` & `flightdata-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/PKG-INFO` & `flightdata-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: flightdata
-Version: 0.2.6
+Version: 0.2.7
 Summary: Module for handling UAV flight log data
 Home-page: https://github.com/PyFlightCoach/FlightData
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: simplejson
-Requires-Dist: pfc-geometry>=0.2.4
-Requires-Dist: ardupilot-log-reader>=0.2.1
+Requires-Dist: pfc-geometry>=0.2.5
+Requires-Dist: ardupilot-log-reader>=0.3.1
 
 ## FlightData
 This repo is contains a set of datastructures and tools for handling flight log data.
 
 ### Flight 
 The Flight object represents the data logged by a flight controller. The class wraps a pandas dataframe which is indexed on a single time axis. Where data is logged at different rates for different sensors it is mapped to the closest time index. Attribute access provides individual columns or sets of columns in the groups defined in Fields. Item access subsets the data in the time axis. 
 
-
 ### Table
 The Table is the base type for most of the datastructures. It allows attribute access to individual columns. Attribute access is also available to return basic entities subclassed from the base type in the pfc-geometry package. For example in the state object table.x provides the x position, table.pos provides a Point representing the xyz position. columns that are not represented by geometric base types are considered to be labels for the data.
 
 ### State
 The State object is a table representing the position and orientation of the aircraft along with their derivatives, it can be constructed from a Flight or from scratch by extrapolating in lines or around arcs. Many tools are provided to manipulate the data. The position and attitude are in a reference frame (with Z up), the derivatives move with the aircraft in either the body, wind, stability or track (like the wind axis but with no wind) frame.
```

### Comparing `flightdata-0.2.6/README.md` & `flightdata-0.2.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 ## FlightData
 This repo is contains a set of datastructures and tools for handling flight log data.
 
 ### Flight 
 The Flight object represents the data logged by a flight controller. The class wraps a pandas dataframe which is indexed on a single time axis. Where data is logged at different rates for different sensors it is mapped to the closest time index. Attribute access provides individual columns or sets of columns in the groups defined in Fields. Item access subsets the data in the time axis. 
 
-
 ### Table
 The Table is the base type for most of the datastructures. It allows attribute access to individual columns. Attribute access is also available to return basic entities subclassed from the base type in the pfc-geometry package. For example in the state object table.x provides the x position, table.pos provides a Point representing the xyz position. columns that are not represented by geometric base types are considered to be labels for the data.
 
 ### State
 The State object is a table representing the position and orientation of the aircraft along with their derivatives, it can be constructed from a Flight or from scratch by extrapolating in lines or around arcs. Many tools are provided to manipulate the data. The position and attitude are in a reference frame (with Z up), the derivatives move with the aircraft in either the body, wind, stability or track (like the wind axis but with no wind) frame.
```

### Comparing `flightdata-0.2.6/flightdata/base/collection.py` & `flightdata-0.2.7/flightdata/base/collection.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/flightdata/base/constructs.py` & `flightdata-0.2.7/flightdata/base/constructs.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/flightdata/base/table.py` & `flightdata-0.2.7/flightdata/base/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,37 +5,31 @@
 from geometry import Base, Time
 from typing import Self, Tuple
 from .constructs import SVar, Constructs
 from numbers import Number
 from time import time
 
 
-def make_time(tab):
-    return Time.from_t(tab.t)
-    
-    
 class Table:
     constructs = Constructs([
-        SVar("time", Time,        ["t", "dt"]               , make_time )
+        SVar("time", Time, ["t", "dt"], lambda tab: Time.from_t(tab.t))
     ])
 
     def __init__(self, data: pd.DataFrame, fill=True, min_len=1):
         if len(data) < min_len:
             raise Exception(f"State constructor length check failed, data length = {len(data)}, min_len = {min_len}")
         self.base_cols = [c for c in data.columns if c in self.constructs.cols()]
         self.label_cols = [c for c in data.columns if c not in self.constructs.cols()]
     
         self.data = data
-
-        self.data.index = self.data.index - self.data.index[0]
+        #self.data.index = self.data.index - self.data.index[0]
         
         if fill:
             missing = self.constructs.missing(self.data.columns)
-            for svar in missing:
-                
+            for svar in missing:                
                 newdata = svar.builder(self).to_pandas(
                     columns=svar.keys, 
                     index=self.data.index
                 ).loc[:, [key for key in svar.keys if key not in self.data.columns]]
                 
                 self.data = pd.concat([self.data, newdata], axis=1)
             bcs = self.constructs.cols()
@@ -71,23 +65,26 @@
         return len(self.data)
     
     @property
     def duration(self):
         return self.data.index[-1] - self.data.index[0]
     
     def __getitem__(self, sli):
-        if isinstance(sli, Number):
+        if isinstance(sli, slice):
+            return self.__class__(self.data.loc[slice(sli.start + self.data.index[0], sli.stop + self.data.index[0], sli.step)])
+        elif isinstance(sli, Number):
             if sli<0:
                 return self.__class__(self.data.iloc[[int(sli)], :])
 
             return self.__class__(
-                self.data.iloc[self.data.index.get_indexer([sli], method="nearest"), :]
+                self.data.iloc[self.data.index.get_indexer([sli + self.data.index[0]], method="nearest"), :]
             )
+        else:
+            raise TypeError(f"Expected Number or slice, got {sli.__class__.__name__}")
         
-        return self.__class__(self.data.loc[sli])
 
     def slice_raw_t(self, sli):
         inds = self.data.reset_index(names="t2").set_index("t").loc[sli].t2.to_numpy()#set_index("t", drop=False).columns
 
         return self.__class__(self.data.loc[inds])
 
     @classmethod
@@ -172,21 +169,15 @@
         return self.label_cols
     
     @property
     def labels(self) -> dict[str, npt.NDArray]:
         return self.data.loc[:, self.label_cols]
 
     def remove_labels(self) -> Self:
-        return self.__class__(
-            self.data.drop(
-                self.label_keys, 
-                axis=1, 
-                errors="ignore"
-            )
-        )
+        return self.__class__(self.data.drop(self.label_keys, axis=1, errors="ignore"))
     
     def get_subset_df(self, **kwargs) -> pd.DataFrame:
         dfo = self.data
         for k, v in kwargs.items():
             dfo = dfo.loc[dfo[k] == v, :]            
         return dfo
 
@@ -338,15 +329,14 @@
         for i, nl in enumerate(new_labels):
             uls.append(sum(new_labels.iloc[:i] == nl))
         
         df = pd.DataFrame(labs).assign(indexer = np.array(uls)[changes.cumsum() - 1])
         strdf = df.copy()
         strdf['indexer'] = strdf['indexer'].astype(int).astype(str)
         strdf  = strdf.stack().groupby(level=0).apply('_'.join)
-        strdf.loc[df.indexer==0] = df[0]
         return strdf.values
 
     @staticmethod
     def copy_labels(template: Self, flown: Self, path=None, min_len=0) -> Self:
         """Copy the labels from along the index warping path"""
 
         flown = flown.remove_labels()
```

### Comparing `flightdata-0.2.6/flightdata/coefficients.py` & `flightdata-0.2.7/flightdata/coefficients.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/flightdata/environment/environment.py` & `flightdata-0.2.7/flightdata/environment/environment.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/flightdata/environment/wind.py` & `flightdata-0.2.7/flightdata/environment/wind.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/flightdata/flight/fields.py` & `flightdata-0.2.7/flightdata/flight/fields.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/flightdata/flight/flight.py` & `flightdata-0.2.7/flightdata/flight/flight.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,119 +17,160 @@
 from geometry import GPS, Point
 from geometry.testing import assert_almost_equal
 from pathlib import Path
 from time import time
 from json import load, dump
 from ardupilot_log_reader.reader import Ardupilot
 from flightdata.base.numpy_encoder import NumpyEncoder
-from flightdata.flight.fields import Fields
 from .ardupilot import flightmodes 
 from flightdata import Origin
-from scipy.signal import butter, filtfilt
+from numbers import Number
 
 
 class Flight:
     ardupilot_types = [
         'XKF1', 'XKF2', 'NKF1', 'NKF2', 
         'POS', 'ATT', 'RATE', 'ACC', 'GYRO', 'IMU', 
         'ARSP', 'GPS', 'RCIN', 'RCOU', 'BARO', 'MODE', 
         'RPM', 'MAG', 'BAT', 'BAT2', 'VEL', 'ORGN', 'ESC', 'CURRENT']
     
-    def __init__(self, data: pd.DataFrame, parameters: list = None, origin: Origin = None, primary_pos_source='gps'):
+    def __init__(self, data: pd.DataFrame, parameters: pd.DataFrame = None, origin: Origin = None, primary_pos_source='gps'):
         self.data = data
         self.parameters = parameters
-        self.data.index = self.data.index - self.data.index[0]
-        self.data.index.name = 'time_index'
         self.origin = origin
         self.primary_pos_source = primary_pos_source
         
     def __getattr__(self, name):
+        if self.parameters is not None:
+            if name in self.parameters.parameter.unique():
+                df =  self.parameters.loc[self.parameters.parameter==name]
+                return df.loc[df.value != df.value.shift()]
         cols = getattr(fields, name)
         if cols is None:
             cols = [f for f in self.data.columns if f.startswith(name)]
             if len(cols) > 0:
                 return self.data[cols]
-        try:
-            if isinstance(cols, Field):
-                return self.data[cols.col]
-            else:
-                return self.data.loc[:, [f.col for f in cols if f.col in self.data.columns]]
-        except KeyError:
-            if isinstance(cols, Field):
-                cols = [cols]
-            return pd.DataFrame(data=np.empty((len(self), len(cols))),columns=[f.col for f in cols])
-        
+        else:
+            try:
+                if isinstance(cols, Field):
+                    return self.data[cols.col]
+                else:
+                    return self.data.loc[:, [f.col for f in cols if f.col in self.data.columns]]
+            except KeyError:
+                if isinstance(cols, Field):
+                    cols = [cols]
+                return pd.DataFrame(data=np.empty((len(self), len(cols))),columns=[f.col for f in cols])
+        raise AttributeError(f"'Flight' object has no attribute '{name}'")
+    
+    def make_param_labels(self, pname: str, prefix:str=None, suffix:str=None, unknown=''):
+        '''Make a series with the parameter values at the correct times.'''
+        ser = pd.Series(np.nan, index=self.data.index, name=pname)
+        param = getattr(self, pname)
+        ser.iloc[ser.index.get_indexer(param.index, 'nearest')] = param.value
+        ser = ser.ffill()
+        
+        if prefix or suffix:
+            sout = pd.Series(unknown, index=self.data.index, name=pname)
+            sout[~np.isnan(ser)] = (prefix or '') + ser[~np.isnan(ser)].astype(str) + (suffix or '')
+            return sout
+        else:
+            return ser
+
+    def make_param_df(self, pnames: list[str]):
+        '''Make a dataframe of parameter values'''
+        return pd.DataFrame([self.make_param_labels(p) for p in pnames]).T
+
     def contains(self, name: Union[str, list[str]]):
         cols = getattr(fields, name)
         if isinstance(cols, Field):
             return name in self.data.columns
         else:
             return [f.column in self.data.columns for f in cols]
                 
-    def __getitem__(self, sli) -> Self:
-        if isinstance(sli, int) or isinstance(sli, float):
-            return self.data.iloc[self.data.index.get_loc(sli)]
+    def __getitem__(self, sli: Number | slice) -> Flight:
+        if isinstance(sli, Number):
+            if sli < 0:
+                return self.data.iloc[sli]
+            else:
+                gl = self.data.index.get_loc(sli + self.data.index[0])
+                return Flight(
+                    self.data.iloc[gl],
+                    self.parameters.loc[:gl],
+                )
+        elif isinstance(sli, slice):
+            return Flight(
+                self.data.loc[slice(
+                    None if sli.start is None else sli.start + self.data.index[0],
+                    None if sli.stop is None else sli.stop + self.data.index[0],
+                    sli.step
+                )], 
+                self.parameters.loc[:None if sli.stop is None else sli.stop + self.data.index[0]], 
+                self.origin, self.primary_pos_source
+            )
         else:
-            return Flight(self.data.loc[sli], self.parameters, self.origin, self.primary_pos_source)
+            raise TypeError(f'Expected a number or a slice, got a {sli.__class__.__name__}')
 
     def __len__(self):
         return len(self.data)
 
-    def slice_raw_t(self, sli):
+    def slice_raw_t(self, sli: Number | slice) -> Flight:
+        def opp(df: pd.DataFrame, indexer: Number | slice):
+            return df.reset_index(drop=True) \
+                .set_index('time_actual', drop=False) \
+                    .loc[indexer].set_index("time_flight", drop=False)
+            
         return Flight(
-            self.data.reset_index(drop=True)
-                .set_index('time_actual', drop=False)
-                    .loc[sli].set_index("time_flight", drop=False), 
-            self.parameters, self.origin, self.primary_pos_source
+            opp(self.data, sli),
+            opp(self.parameters, slice(None, sli if isinstance(sli, Number) else sli.stop, None)),
+            self.origin, self.primary_pos_source
         )
         
-    def slice_time_flight(self, sli):
+    def slice_time_flight(self, sli) -> Flight:
         return Flight(
-            self.data.reset_index(drop=True)
-                .set_index('time_flight', drop=False)
-                    .loc[sli], 
-            self.parameters, self.origin, self.primary_pos_source
+            self.data.loc[sli], 
+            self.parameters.loc[:sli if isinstance(sli, Number) else sli.stop], 
+            self.origin, self.primary_pos_source
         )
         
-    def copy(self, **kwargs):
+    def copy(self, **kwargs) -> Flight:
         return Flight(
             kwargs['data'] if 'data' in kwargs else self.data.copy() ,
-            kwargs['parameters'] if 'parameters' in kwargs else self.parameters.copy() if self.parameters else None,
+            kwargs['parameters'] if 'parameters' in kwargs else self.parameters.copy() if self.parameters is not None else None,
             kwargs['origin'] if 'origin' in kwargs else self.origin.copy(),
             kwargs['primary_pos_source'] if 'primary_pos_source' in kwargs else self.primary_pos_source
         )
 
     def to_dict(self):
         return {
             'data': self.data.to_dict('list'),
-            'parameters': self.parameters,
+            'parameters': self.parameters.to_dict('list'),
             'origin': self.origin.to_dict(),
             'primary_pos_source': self.primary_pos_source
         }
     
     @staticmethod
-    def from_dict(data: dict):
+    def from_dict(data: dict) -> Flight:
         return Flight(
             data=pd.DataFrame.from_dict(data['data']).set_index('time_flight', drop=False),
-            parameters=data['parameters'],
+            parameters=pd.DataFrame.from_dict(data['parameters']).set_index('time_flight', drop=False),
             origin=Origin.from_dict(data['origin']),
             primary_pos_source=data['primary_pos_source']
         )
     
     def to_json(self, file: str) -> str:
         with open(file, 'w') as f:
             dump(self.to_dict(), f, cls=NumpyEncoder, indent=2)
         return file
 
     @staticmethod
     def from_json(file: str) -> Self:
         return Flight.from_dict(load(open(file, 'r')))
 
     @staticmethod
-    def build_cols(**kwargs):
+    def build_cols(**kwargs) -> pd.DataFrame:
         df = pd.DataFrame(columns=list(fields.data.keys()))
         for k, v in kwargs.items():
             df[k] = v
         return df.dropna(axis=1, how='all')
     
     @staticmethod
     def synchronise(fls: list[Self]) -> list[Self]:
@@ -146,15 +187,15 @@
         flos = []
         for fl in fls:
             flos.append(fl.copy(
                 data=pd.merge_asof(
                     otf, 
                     fl.data.reset_index(), 
                     on='time_actual'
-                ).set_index('time_index', drop=False)
+                ).set_index('time_flight', drop=False)
             ))
 
         return flos
 
     def split_modes(self):
         """Split the flight into segments of the same flight mode.
 
@@ -168,15 +209,15 @@
         for mode in modechanges.unique():
             _fl = self.data.loc[modechanges == mode, :]
             flights[flightmodes[_fl.flightmode_a.iloc[0]]].append(Flight(_fl, self.parameters, self.origin, self.primary_pos_source))
         return flights
 
     @property
     def duration(self):
-        return self.data.tail(1).index.item()
+        return self.data.iloc[-1].name - self.data.iloc[0].name
 
     def flying_only(self, minalt=5, minv=10):
         vs = abs(Point(self.velocity))
         above_ground = self.data.loc[(self.gps_altitude >= minalt) & (vs > minv)]
 
         return self[above_ground.index[0]:above_ground.index[-1]]
 
@@ -190,37 +231,44 @@
         return "{}_{:.8f}_{:.6f}_{:.6f}".format(len(_ftemp.data), _ftemp.duration, *self.origin.data[0])
 
     def __eq__(self, other):
         try:
             pd.testing.assert_frame_equal(self.data, other.data)
             assert_almost_equal(self.origin.pos, other.origin.pos)
             assert self.origin.heading == other.origin.heading
+            pd.testing.assert_frame_equal(self.parameters, other.parameters)
             return True
-        except Exception as ex:
+        except Exception:
             return False
         
     @staticmethod
     def from_log(log:Union[Ardupilot, str], extra_types: list[str] = None, **kwargs) -> Flight:
         """Constructor from an ardupilot bin file."""
-        
         extra_types = [] if extra_types is None else extra_types
         
         if isinstance(log, str) or isinstance(log, Path):
-            parser = Ardupilot(str(log), types=list(set(Flight.ardupilot_types + extra_types)))
+            parser = Ardupilot.parse(str(log), types=list(set(Flight.ardupilot_types + extra_types)))
         else:
             parser = log
-
-        if parser.parms['AHRS_EKF_TYPE'] == 2:
+        
+        params = Flight.build_cols(
+            time_actual = parser.PARM.timestamp,
+            time_flight = parser.PARM.TimeUS / 1e6,
+            parameter = parser.PARM.Name,
+            value = parser.PARM.Value
+        ).set_index('time_flight', drop=False)
+       
+        if params.loc[params.parameter=='AHRS_EKF_TYPE'].iloc[0].value == 2:
             ekf1 = 'NKF1'
             ekf2 = 'NKF2'
         else:
             ekf1 = 'XKF1'
             ekf2 = 'XKF2'
 
-        ekf1 = parser.dfs[ekf1] if ekf1 in parser.dfs else  None
+        ekf1 = parser.dfs[ekf1] if ekf1 in parser.dfs else None
         ekf2 = parser.dfs[ekf2] if ekf2 in parser.dfs else None
 
         dfs = []
 
         if 'ATT' in parser.dfs:
             att=parser.ATT.iloc[1:, :]
             dfs.append(Flight.build_cols(
@@ -258,21 +306,21 @@
         if ekf2 is not None:
             dfs = dfs + Flight.parse_instances(ekf2, {
                 'wind_N': 'VWN',
                 'wind_E': 'VWE',
             }, 'C')
         if 'RATE' in parser.dfs:
             dfs.append(Flight.build_cols(
-                time_actual = parser.rate.timestamp,
-                axisrate_roll = parser.rate.R,
-                axisrate_pitch = parser.rate.P,
-                axisrate_yaw = parser.rate.Y,
-                desrate_roll = parser.rate.RDes,
-                desrate_pitch = parser.rate.PDes,
-                desrate_yaw = parser.rate.YDes,
+                time_actual = parser.RATE.timestamp,
+                axisrate_roll = parser.RATE.R,
+                axisrate_pitch = parser.RATE.P,
+                axisrate_yaw = parser.RATE.Y,
+                desrate_roll = parser.RATE.RDes,
+                desrate_pitch = parser.RATE.PDes,
+                desrate_yaw = parser.RATE.YDes,
             ))
         
         if 'IMU' in parser.dfs:
             imu = parser.IMU
             if 'I' in imu:
                 imu = imu.loc[imu.I==0, :]
             
@@ -379,15 +427,15 @@
             dfout = pd.merge_asof(
                 dfout, df, on='time_actual', direction='nearest', 
                 tolerance=min(max(dt, df.time_actual.diff().max()), 0.1)
             )
         
         origin = Origin('ekf_origin', GPS(parser.ORGN.iloc[:,-3:]), 0)
         
-        return Flight(dfout.set_index('time_flight', drop=False), parser.parms, origin, ppsorce)
+        return Flight(dfout.set_index('time_flight', drop=False), params, origin, ppsorce)
 
     @staticmethod
     def parse_instances(indf: pd.DataFrame, colmap:dict[str, str], instancecol='Instance'):
             '''Where an instance column exists in an input df split the values into two columns'''
             instances = indf[instancecol].unique() if instancecol in indf.columns else [0]
             dfs = []
             for i in instances:
@@ -447,14 +495,15 @@
             data=pd.concat([
                 pd.DataFrame(np.array(avcols).T, columns=time_cols, index=self.data.index),
                 self.data.loc[:,[c for c in self.data.columns if c not in time_cols]],
             ], axis=1).reset_index(drop=True).set_index('time_flight', drop=False)
         )
 
     def filter(self, b, a):
+        from scipy.signal import filtfilt
         dont_filter = [c for c in fields.get_cols(['time', 'flightmode', 'rcin', 'rcout']) if c in self.data.columns]
         unwrap_cols = [c for c in fields.get_cols(['attitude']) if c in self.data.columns]
 
         filter_cols = [c for c in self.data.columns if c not in dont_filter + unwrap_cols]
         
         filtdf = filtfilt(b, a, self.data.loc[:, filter_cols], axis=0)
         unwfiltdf = filtfilt(b, a, np.unwrap(self.data.loc[:, unwrap_cols], axis=0), axis=0)
@@ -464,13 +513,14 @@
                 self.data.loc[:,dont_filter],
                 pd.DataFrame(unwfiltdf, columns=unwrap_cols, index=self.data.index) % (2*np.pi),
                 pd.DataFrame(filtdf, columns=filter_cols, index=self.data.index),
             ], axis=1)
         )
     
     def butter_filter(self, cutoff, order=5):
+        from scipy.signal import butter
         ts = self.time_flight.to_numpy()
         N = len(self)
         T = (ts[-1] - ts[0]) / N
         fs = 1/T
         return self.filter(*butter(order, cutoff, fs=fs, btype='low', analog=False))
```

### Comparing `flightdata-0.2.6/flightdata/flow.py` & `flightdata-0.2.7/flightdata/flow.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/flightdata/model/aerodynamic.py` & `flightdata-0.2.7/flightdata/model/aerodynamic.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/flightdata/origin.py` & `flightdata-0.2.7/flightdata/origin.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/flightdata/state.py` & `flightdata-0.2.7/flightdata/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,35 +99,35 @@
                 origin = Origin.from_json(origin)
         elif origin is None:
             origin = flight.origin
 
         time = g.Time.from_t(np.array(flight.data.time_flight))
 
         if all(flight.contains('gps')) and flight.primary_pos_source == 'gps':
-            pos = origin.rotation.transform_point(g.GPS(flight.gps) - origin.pos[0])
+            pos = origin.rotation.transform_point(g.GPS(flight.gps.ffill().bfill()) - origin.pos[0])
         else: 
             pos = origin.rotation.transform_point(
-                flight.origin.pos.offset(g.Point(flight.position)) - origin.pos[0]
+                flight.origin.pos.offset(g.Point(flight.position.ffill().bfill())) - origin.pos[0]
             )
         
-        att = origin.rotation * g.Euler(flight.attitude) 
-        vel =  att.inverse().transform_point(origin.rotation.transform_point(g.Point(flight.velocity))) if all(flight.contains('velocity')) else None
-        rvel = g.Point(flight.axisrate) if all(flight.contains('axisrate')) else None
-        acc = g.Point(flight.acceleration) if all(flight.contains('acceleration')) else None
+        att = origin.rotation * g.Euler(flight.attitude.ffill().bfill()) 
+        vel =  att.inverse().transform_point(origin.rotation.transform_point(g.Point(flight.velocity.ffill().bfill()))) if all(flight.contains('velocity')) else None
+        rvel = g.Point(flight.axisrate.ffill().bfill()) if all(flight.contains('axisrate')) else None
+        acc = g.Point(flight.acceleration.ffill().bfill()) if all(flight.contains('acceleration')) else None
         
         return State.from_constructs(time, pos, att, vel, rvel, acc)
 
     @staticmethod
     def align(
         flown: State, 
         template: State, 
         radius=5, mirror=True,
         weights = g.Point(1,1.2,0.5),
         tp_weights = g.Point(0.6,0.6,0.6),
-    ) -> Tuple(float, Self):
+    ) -> Tuple[float, Self]:
         """Perform a temporal alignment between two sections. return the flown section with labels 
         copied from the template along the warped path. 
         """
         from fastdtw import fastdtw
         from scipy.spatial.distance import euclidean
         def get_brv(brv):
             if mirror:
@@ -143,16 +143,14 @@
             fl.data,
             radius=radius,
             dist=euclidean
         )
 
         return distance, State.copy_labels(template, flown, path, 3)
 
-    
-    
     def splitter_labels(self: State, mans: List[dict], better_names: List[str]=None) -> State:
             """label the manoeuvres in a State based on the flight coach splitter information
 
             TODO this assumes the state only contains the dataset contained in the json
 
             Args:
                 mans (list): the mans field of a flight coach json
```

### Comparing `flightdata-0.2.6/flightdata.egg-info/PKG-INFO` & `flightdata-0.2.7/flightdata.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: flightdata
-Version: 0.2.6
+Version: 0.2.7
 Summary: Module for handling UAV flight log data
 Home-page: https://github.com/PyFlightCoach/FlightData
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: simplejson
-Requires-Dist: pfc-geometry>=0.2.4
-Requires-Dist: ardupilot-log-reader>=0.2.1
+Requires-Dist: pfc-geometry>=0.2.5
+Requires-Dist: ardupilot-log-reader>=0.3.1
 
 ## FlightData
 This repo is contains a set of datastructures and tools for handling flight log data.
 
 ### Flight 
 The Flight object represents the data logged by a flight controller. The class wraps a pandas dataframe which is indexed on a single time axis. Where data is logged at different rates for different sensors it is mapped to the closest time index. Attribute access provides individual columns or sets of columns in the groups defined in Fields. Item access subsets the data in the time axis. 
 
-
 ### Table
 The Table is the base type for most of the datastructures. It allows attribute access to individual columns. Attribute access is also available to return basic entities subclassed from the base type in the pfc-geometry package. For example in the state object table.x provides the x position, table.pos provides a Point representing the xyz position. columns that are not represented by geometric base types are considered to be labels for the data.
 
 ### State
 The State object is a table representing the position and orientation of the aircraft along with their derivatives, it can be constructed from a Flight or from scratch by extrapolating in lines or around arcs. Many tools are provided to manipulate the data. The position and attitude are in a reference frame (with Z up), the derivatives move with the aircraft in either the body, wind, stability or track (like the wind axis but with no wind) frame.
```

### Comparing `flightdata-0.2.6/flightdata.egg-info/SOURCES.txt` & `flightdata-0.2.7/flightdata.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 flightdata.egg-info/SOURCES.txt
 flightdata.egg-info/dependency_links.txt
 flightdata.egg-info/requires.txt
 flightdata.egg-info/top_level.txt
 flightdata/base/__init__.py
 flightdata/base/collection.py
 flightdata/base/constructs.py
+flightdata/base/labeling.py
 flightdata/base/numpy_encoder.py
 flightdata/base/table.py
 flightdata/environment/__init__.py
 flightdata/environment/environment.py
 flightdata/environment/wind.py
 flightdata/flight/__init__.py
 flightdata/flight/ardupilot.py
 flightdata/flight/fields.py
 flightdata/flight/flight.py
+flightdata/flight/parameters.py
 flightdata/model/__init__.py
 flightdata/model/aerodynamic.py
 flightdata/model/thrust.py
 scripts/collect_logs.py
 scripts/flightline.py
 test/test_fields.py
 test/test_flight.py
```

### Comparing `flightdata-0.2.6/scripts/collect_logs.py` & `flightdata-0.2.7/scripts/collect_logs.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/scripts/flightline.py` & `flightdata-0.2.7/scripts/flightline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from flightdata import Flight, Origin
 from geometry import GPS
 from pathlib import Path
-import numpy as np
 import argparse
 
 
 def box_from_log(log: Flight, channel: int):
     c6on = Flight(log.data.loc[log.data[f'rcin_c{channel}']>=1500])
-    groups = np.cumsum(c6on.time_flight.diff() >=1)
-    return Origin.from_points("new", GPS(c6on.gps[groups==0])[-1], GPS(c6on.gps[groups==1])[-1])
+    groups = (c6on.time_flight.diff() > 1).cumsum()
+    pilot = Flight(c6on.data.loc[groups==0])
+    centre = Flight(c6on.data.loc[groups==1])
+
+    return Origin.from_points("new", GPS(pilot.gps)[-1], GPS(centre.gps)[-1])
 
 def box_from_logs(pilot: Flight, centre: Flight):
     return Origin.from_points("new", GPS(*pilot.gps.iloc[-1]), GPS(*centre.gps.iloc[-1]))
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description='A tool for creating a flightline .f3a file from bin logs')
```

### Comparing `flightdata-0.2.6/setup.py` & `flightdata-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `flightdata-0.2.6/test/test_flight.py` & `flightdata-0.2.7/test/test_flight.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,38 +5,36 @@
 import numpy as np
 import pandas as pd
 from ardupilot_log_reader import Ardupilot
 
 
 @fixture(scope='session')
 def parser():
-    return Ardupilot('test/test_inputs/00000137.BIN',
-                     types=Flight.ardupilot_types)
+    return Ardupilot.parse('test/data/p23.BIN',types=Flight.ardupilot_types)
 
 @fixture(scope='session')
-def fl():
-    return Flight.from_log('test/test_inputs/00000137.BIN')
+def fl(parser):
+    return Flight.from_log(parser)
 
 @fixture(scope='session')
 def fcj():
-    return Flight.from_fc_json('test/test_inputs/00000137.json')
+    return Flight.from_fc_json('test/data/p23_fc.json')
 
 def test_duration(fl):
-    assert fl.duration == approx(685, rel=1e-3)
+    assert fl.duration == approx(687, rel=1e-3)
 
 def test_slice(fl):
     short_flight = fl[100:200]
     assert short_flight.duration == approx(100, 0.01)
 
 def test_to_from_dict(fl):
     data = fl.to_dict()
     fl2 = Flight.from_dict(data)
     assert fl == fl2
-    assert fl2.parameters == approx(fl.parameters)
-
+    
 def test_from_fc_json(fcj):
     assert isinstance(fcj, Flight)
     assert fcj.duration > 200
     assert fcj.position_D.max() < -10
   
 @mark.skip
 def test_unique_identifier():
@@ -97,7 +95,23 @@
     xf, yf = _fft(filtered.acceleration_x)
 
     assert np.all(yf[xf>1]<0.025)
 
 def test_remove_time_flutter(fl: Flight):
     flf = fl.remove_time_flutter()
     assert np.gradient(np.gradient(flf.data.index)) == approx(0)
+
+
+def test_get_parameter_attr(fl: Flight):
+    assert fl.AHRS_EKF_TYPE.iloc[0].value == 3
+
+def test_make_param_labels(fl: Flight):
+    col = fl.make_param_labels('AHRS_EKF_TYPE')
+
+    assert len(col) == len(fl)  
+    assert np.all(col.loc[~np.isnan(col)] == 3)
+
+
+    col = fl.make_param_labels('AHRS_EKF_TYPE', 'Test')
+
+    assert np.all(col.loc[col!=''] == 'Test3.0')
+
```

