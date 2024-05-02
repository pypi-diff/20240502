# Comparing `tmp/spc-plotly-0.1.4.1.tar.gz` & `tmp/spc_plotly-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spc-plotly-0.1.4.1.tar", last modified: Thu Mar 28 14:57:35 2024, max compression
+gzip compressed data, was "spc_plotly-0.2.1.tar", last modified: Thu May  2 17:46:24 2024, max compression
```

## Comparing `spc-plotly-0.1.4.1.tar` & `spc_plotly-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-03-28 14:57:35.017240 spc-plotly-0.1.4.1/
--rw-r--r--   0 jeremycolon   (503) staff       (20)     5151 2024-03-28 14:57:35.017017 spc-plotly-0.1.4.1/PKG-INFO
--rw-r--r--   0 jeremycolon   (503) staff       (20)     4355 2024-03-26 18:06:47.000000 spc-plotly-0.1.4.1/README.md
--rw-r--r--   0 jeremycolon   (503) staff       (20)      909 2024-03-28 14:56:46.000000 spc-plotly-0.1.4.1/pyproject.toml
--rw-r--r--   0 jeremycolon   (503) staff       (20)       38 2024-03-28 14:57:35.017278 spc-plotly-0.1.4.1/setup.cfg
--rw-r--r--   0 jeremycolon   (503) staff       (20)       37 2024-03-26 17:10:31.000000 spc-plotly-0.1.4.1/setup.py
-drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-03-28 14:57:35.011849 spc-plotly-0.1.4.1/src/
--rw-r--r--   0 jeremycolon   (503) staff       (20)       32 2024-03-26 18:20:16.000000 spc-plotly-0.1.4.1/src/__init__.py
-drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-03-28 14:57:35.012232 spc-plotly-0.1.4.1/src/spc_plotly/
--rw-r--r--   0 jeremycolon   (503) staff       (20)        0 2024-03-01 18:26:44.000000 spc-plotly-0.1.4.1/src/spc_plotly/__init__.py
-drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-03-28 14:57:35.014509 spc-plotly-0.1.4.1/src/spc_plotly/helpers/
--rw-r--r--   0 jeremycolon   (503) staff       (20)        0 2024-03-01 18:47:17.000000 spc-plotly-0.1.4.1/src/spc_plotly/helpers/__init__.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)     4903 2024-03-28 14:55:49.000000 spc-plotly-0.1.4.1/src/spc_plotly/helpers/annotations.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)     3905 2024-03-20 20:01:14.000000 spc-plotly-0.1.4.1/src/spc_plotly/helpers/axes_formats.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)     1578 2024-03-19 18:58:41.000000 spc-plotly-0.1.4.1/src/spc_plotly/helpers/base_traces.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)     6920 2024-03-28 14:51:05.000000 spc-plotly-0.1.4.1/src/spc_plotly/helpers/limit_lines.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)     3859 2024-03-11 18:48:25.000000 spc-plotly-0.1.4.1/src/spc_plotly/helpers/menus.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)    12484 2024-03-20 20:01:14.000000 spc-plotly-0.1.4.1/src/spc_plotly/helpers/signals.py
-drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-03-28 14:57:35.015805 spc-plotly-0.1.4.1/src/spc_plotly/utils/
--rw-r--r--   0 jeremycolon   (503) staff       (20)        0 2024-03-01 18:55:21.000000 spc-plotly-0.1.4.1/src/spc_plotly/utils/__init__.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)      398 2024-03-14 18:42:01.000000 spc-plotly-0.1.4.1/src/spc_plotly/utils/calc_xmr_func.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)     1925 2024-03-14 18:11:05.000000 spc-plotly-0.1.4.1/src/spc_plotly/utils/combine_paths.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)      555 2024-03-14 18:50:30.000000 spc-plotly-0.1.4.1/src/spc_plotly/utils/endpoints.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)     1016 2024-03-14 19:00:11.000000 spc-plotly-0.1.4.1/src/spc_plotly/utils/rounded_value.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)     1386 2024-03-14 18:58:30.000000 spc-plotly-0.1.4.1/src/spc_plotly/utils/rounding_multiple.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)    13153 2024-03-28 14:30:48.000000 spc-plotly-0.1.4.1/src/spc_plotly/xmr.py
-drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-03-28 14:57:35.016803 spc-plotly-0.1.4.1/src/spc_plotly.egg-info/
--rw-r--r--   0 jeremycolon   (503) staff       (20)     5151 2024-03-28 14:57:35.000000 spc-plotly-0.1.4.1/src/spc_plotly.egg-info/PKG-INFO
--rw-r--r--   0 jeremycolon   (503) staff       (20)      808 2024-03-28 14:57:35.000000 spc-plotly-0.1.4.1/src/spc_plotly.egg-info/SOURCES.txt
--rw-r--r--   0 jeremycolon   (503) staff       (20)        1 2024-03-28 14:57:35.000000 spc-plotly-0.1.4.1/src/spc_plotly.egg-info/dependency_links.txt
--rw-r--r--   0 jeremycolon   (503) staff       (20)       43 2024-03-28 14:57:35.000000 spc-plotly-0.1.4.1/src/spc_plotly.egg-info/requires.txt
--rw-r--r--   0 jeremycolon   (503) staff       (20)       26 2024-03-28 14:57:35.000000 spc-plotly-0.1.4.1/src/spc_plotly.egg-info/top_level.txt
-drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-03-28 14:57:35.016457 spc-plotly-0.1.4.1/src/tests/
--rw-r--r--   0 jeremycolon   (503) staff       (20)        0 2024-03-01 18:27:28.000000 spc-plotly-0.1.4.1/src/tests/__init__.py
--rw-r--r--   0 jeremycolon   (503) staff       (20)     2283 2024-03-21 14:00:03.000000 spc-plotly-0.1.4.1/src/tests/test_xmr.py
+drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-05-02 17:46:24.821769 spc_plotly-0.2.1/
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     5149 2024-05-02 17:46:24.821536 spc_plotly-0.2.1/PKG-INFO
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     4355 2024-03-26 18:06:47.000000 spc_plotly-0.2.1/README.md
+-rw-r--r--   0 jeremycolon   (503) staff       (20)      907 2024-05-02 17:43:44.000000 spc_plotly-0.2.1/pyproject.toml
+-rw-r--r--   0 jeremycolon   (503) staff       (20)       38 2024-05-02 17:46:24.821810 spc_plotly-0.2.1/setup.cfg
+-rw-r--r--   0 jeremycolon   (503) staff       (20)       37 2024-03-26 17:10:31.000000 spc_plotly-0.2.1/setup.py
+drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-05-02 17:46:24.815857 spc_plotly-0.2.1/src/
+-rw-r--r--   0 jeremycolon   (503) staff       (20)       32 2024-03-26 18:20:16.000000 spc_plotly-0.2.1/src/__init__.py
+drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-05-02 17:46:24.816434 spc_plotly-0.2.1/src/spc_plotly/
+-rw-r--r--   0 jeremycolon   (503) staff       (20)        0 2024-03-01 18:26:44.000000 spc_plotly-0.2.1/src/spc_plotly/__init__.py
+drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-05-02 17:46:24.818978 spc_plotly-0.2.1/src/spc_plotly/helpers/
+-rw-r--r--   0 jeremycolon   (503) staff       (20)        0 2024-03-01 18:47:17.000000 spc_plotly-0.2.1/src/spc_plotly/helpers/__init__.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     4903 2024-03-28 14:55:49.000000 spc_plotly-0.2.1/src/spc_plotly/helpers/annotations.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     3905 2024-03-20 20:01:14.000000 spc_plotly-0.2.1/src/spc_plotly/helpers/axes_formats.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     1578 2024-03-19 18:58:41.000000 spc_plotly-0.2.1/src/spc_plotly/helpers/base_traces.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     6920 2024-03-28 14:51:05.000000 spc_plotly-0.2.1/src/spc_plotly/helpers/limit_lines.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     3859 2024-03-11 18:48:25.000000 spc_plotly-0.2.1/src/spc_plotly/helpers/menus.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)    12484 2024-03-20 20:01:14.000000 spc_plotly-0.2.1/src/spc_plotly/helpers/signals.py
+drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-05-02 17:46:24.820685 spc_plotly-0.2.1/src/spc_plotly/utils/
+-rw-r--r--   0 jeremycolon   (503) staff       (20)        0 2024-03-01 18:55:21.000000 spc_plotly-0.2.1/src/spc_plotly/utils/__init__.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)      398 2024-03-14 18:42:01.000000 spc_plotly-0.2.1/src/spc_plotly/utils/calc_xmr_func.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     1925 2024-03-14 18:11:05.000000 spc_plotly-0.2.1/src/spc_plotly/utils/combine_paths.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)      555 2024-03-14 18:50:30.000000 spc_plotly-0.2.1/src/spc_plotly/utils/endpoints.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     1016 2024-03-14 19:00:11.000000 spc_plotly-0.2.1/src/spc_plotly/utils/rounded_value.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     1386 2024-03-14 18:58:30.000000 spc_plotly-0.2.1/src/spc_plotly/utils/rounding_multiple.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)    13619 2024-05-02 17:24:53.000000 spc_plotly-0.2.1/src/spc_plotly/xmr.py
+drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-05-02 17:46:24.821310 spc_plotly-0.2.1/src/spc_plotly.egg-info/
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     5149 2024-05-02 17:46:24.000000 spc_plotly-0.2.1/src/spc_plotly.egg-info/PKG-INFO
+-rw-r--r--   0 jeremycolon   (503) staff       (20)      808 2024-05-02 17:46:24.000000 spc_plotly-0.2.1/src/spc_plotly.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremycolon   (503) staff       (20)        1 2024-05-02 17:46:24.000000 spc_plotly-0.2.1/src/spc_plotly.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremycolon   (503) staff       (20)       43 2024-05-02 17:46:24.000000 spc_plotly-0.2.1/src/spc_plotly.egg-info/requires.txt
+-rw-r--r--   0 jeremycolon   (503) staff       (20)       26 2024-05-02 17:46:24.000000 spc_plotly-0.2.1/src/spc_plotly.egg-info/top_level.txt
+drwxr-xr-x   0 jeremycolon   (503) staff       (20)        0 2024-05-02 17:46:24.821004 spc_plotly-0.2.1/src/tests/
+-rw-r--r--   0 jeremycolon   (503) staff       (20)        0 2024-03-01 18:27:28.000000 spc_plotly-0.2.1/src/tests/__init__.py
+-rw-r--r--   0 jeremycolon   (503) staff       (20)     2537 2024-05-02 17:42:45.000000 spc_plotly-0.2.1/src/tests/test_xmr.py
```

### Comparing `spc-plotly-0.1.4.1/PKG-INFO` & `spc_plotly-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spc-plotly
-Version: 0.1.4.1
+Version: 0.2.1
 Summary: XmR charts with Plotly
 Author-email: Jeremy Colón <jeremycolon24@gmail.com>
 Project-URL: Homepage, https://github.com/JeremyColon/spc_plotly
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spc-plotly-0.1.4.1/README.md` & `spc_plotly-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/pyproject.toml` & `spc_plotly-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=65.3.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spc-plotly"
-version = "0.1.4.1"
+version = "0.2.1"
 description = "XmR charts with Plotly"
 readme = "README.md"
 authors = [{ name = "Jeremy Colón", email = "jeremycolon24@gmail.com" }]
 classifiers = [
      "Intended Audience :: Developers",
      "License :: OSI Approved :: MIT License",
      "Programming Language :: Python",
```

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly/helpers/annotations.py` & `spc_plotly-0.2.1/src/spc_plotly/helpers/annotations.py`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly/helpers/axes_formats.py` & `spc_plotly-0.2.1/src/spc_plotly/helpers/axes_formats.py`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly/helpers/base_traces.py` & `spc_plotly-0.2.1/src/spc_plotly/helpers/base_traces.py`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly/helpers/limit_lines.py` & `spc_plotly-0.2.1/src/spc_plotly/helpers/limit_lines.py`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly/helpers/menus.py` & `spc_plotly-0.2.1/src/spc_plotly/helpers/menus.py`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly/helpers/signals.py` & `spc_plotly-0.2.1/src/spc_plotly/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly/utils/combine_paths.py` & `spc_plotly-0.2.1/src/spc_plotly/utils/combine_paths.py`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly/utils/endpoints.py` & `spc_plotly-0.2.1/src/spc_plotly/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly/utils/rounded_value.py` & `spc_plotly-0.2.1/src/spc_plotly/utils/rounded_value.py`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly/utils/rounding_multiple.py` & `spc_plotly-0.2.1/src/spc_plotly/utils/rounding_multiple.py`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly/xmr.py` & `spc_plotly-0.2.1/src/spc_plotly/xmr.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,33 +55,36 @@
     """
 
     def __init__(
         self,
         data: DataFrame,
         y_ser_name: str,
         x_ser_name: str,
+        x_begin: str = None,
         x_cutoff: str = None,
         date_part_resolution: str = "month",
         custom_date_part: str = "",
         title: str = None,
         sloped: bool = False,
         xmr_function: str = "mean",
-        chart_height: int = 1000,
+        chart_height: int = None,
     ) -> None:
         """
         Initializes an XmR Chart object.
 
         Parameters:
             data (str): Dataframe to use for XmR chart.
             y_ser_name (int): Name of column containing values to plot on y-axis.
             x_ser_name (str): Name of column or index containing values to plot on x-axis.
                 Column or index should represent a date, date/time, or a proxy for such
                 (e.g., increasing integer value)
+            x_begin (str): Value of x_ser_name, before which the data is excluded for purposes
+                of calculating limits. If None, minimum value is set.
             x_cutoff (str): Value of x_ser_name, after which the data is excluded for purposes
-                of calculating limits. If None, all data is included.
+                of calculating limits. If None, maximum value is set.
             date_part_resolution (str): Resolution of your data, for formatting the x-axis. Valid options:
                 - year
                 - month
                 - day
                 - hour
                 - minute
                 - custom
@@ -122,14 +125,21 @@
         test_xmr.test_cutoff_val(x_cutoff, self._x_Ser)
         # Check if cutoff value exists
         if x_cutoff is None:
             self.x_cutoff = self._x_Ser.max()
         else:
             self.x_cutoff = x_cutoff
 
+        test_xmr.test_begin_val(x_begin, self._x_Ser)
+        # Check if cutoff value exists
+        if x_begin is None:
+            self.x_begin = self._x_Ser.min()
+        else:
+            self.x_begin = x_begin
+
         self._title = (
             f"{y_ser_name} XmR Chart by {self._x_Ser.name}" if title is None else title
         )
 
         # Set constant values for mean or median
         self.mR_Upper_Constant = XmR_constants.get(xmr_function).get("mR_Upper")
         self.npl_Constant = XmR_constants.get(xmr_function).get("npl_Constant")
@@ -157,15 +167,17 @@
             tuple: A tuple containing the following;
                 - pd.DataFrame: Data used to calculate limits
                 - pd.Series: Data used for moving range chart
                 - dict: Contains the moving range upper limit and mean/median value
                 - dict: Contains the natural process limits and mean/median value
         """
 
-        data_for_limits = self.data.loc[self._x_Ser <= self.x_cutoff]
+        data_for_limits = self.data.loc[
+            (self._x_Ser >= self.x_begin) & (self._x_Ser <= self.x_cutoff)
+        ]
 
         mR_data_for_limits = abs(
             data_for_limits[self._y_ser_name]
             - data_for_limits[self._y_ser_name].shift(1)
         )
 
         # Calculate mean/median values
```

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly.egg-info/PKG-INFO` & `spc_plotly-0.2.1/src/spc_plotly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spc-plotly
-Version: 0.1.4.1
+Version: 0.2.1
 Summary: XmR charts with Plotly
 Author-email: Jeremy Colón <jeremycolon24@gmail.com>
 Project-URL: Homepage, https://github.com/JeremyColon/spc_plotly
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spc-plotly-0.1.4.1/src/spc_plotly.egg-info/SOURCES.txt` & `spc_plotly-0.2.1/src/spc_plotly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spc-plotly-0.1.4.1/src/tests/test_xmr.py` & `spc_plotly-0.2.1/src/tests/test_xmr.py`

 * *Files 14% similar despite different names*

```diff
@@ -67,11 +67,21 @@
     else:
         print(cutoff_val)
         print(x_Ser)
         e = f"{cutoff_val} not present in {x_Ser.name}"
         raise ValueError(e)
 
 
+def test_begin_val(begin_val, x_Ser):
+    if begin_val is None or begin_val in x_Ser.values:
+        return True
+    else:
+        print(begin_val)
+        print(x_Ser)
+        e = f"{begin_val} not present in {x_Ser.name}"
+        raise ValueError(e)
+
+
 def test_sloped_val(sloped_val):
     if not isinstance(sloped_val, bool):
         e = f"sloped parameter must be a boolean value"
         raise ValueError(e)
```

