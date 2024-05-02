# Comparing `tmp/xplotlib-0.0.4.tar.gz` & `tmp/xplotlib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplotlib-0.0.4.tar", last modified: Wed May  1 01:01:25 2024, max compression
+gzip compressed data, was "xplotlib-0.0.5.tar", last modified: Thu May  2 21:41:56 2024, max compression
```

## Comparing `xplotlib-0.0.4.tar` & `xplotlib-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:01:25.039464 xplotlib-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 01:01:20.000000 xplotlib-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-01 01:01:25.039464 xplotlib-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-01 01:01:20.000000 xplotlib-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 01:01:20.000000 xplotlib-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-01 01:01:25.039464 xplotlib-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:01:25.035464 xplotlib-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:01:25.035464 xplotlib-0.0.4/src/XPlotLib/
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-01 01:01:20.000000 xplotlib-0.0.4/src/XPlotLib/BandgapAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18473 2024-05-01 01:01:20.000000 xplotlib-0.0.4/src/XPlotLib/DOSAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-01 01:01:20.000000 xplotlib-0.0.4/src/XPlotLib/XPlotLibUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 01:01:20.000000 xplotlib-0.0.4/src/XPlotLib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:01:25.039464 xplotlib-0.0.4/src/XPlotLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-01 01:01:25.000000 xplotlib-0.0.4/src/XPlotLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 01:01:25.000000 xplotlib-0.0.4/src/XPlotLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:01:25.000000 xplotlib-0.0.4/src/XPlotLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 01:01:25.000000 xplotlib-0.0.4/src/XPlotLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 01:01:25.000000 xplotlib-0.0.4/src/XPlotLib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:41:56.400501 xplotlib-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-02 21:41:51.000000 xplotlib-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-02 21:41:56.400501 xplotlib-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 21:41:51.000000 xplotlib-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 21:41:51.000000 xplotlib-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-02 21:41:56.400501 xplotlib-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:41:56.396501 xplotlib-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:41:56.396501 xplotlib-0.0.5/src/XPlotLib/
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-02 21:41:51.000000 xplotlib-0.0.5/src/XPlotLib/BandgapAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18473 2024-05-02 21:41:51.000000 xplotlib-0.0.5/src/XPlotLib/DOSAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-02 21:41:51.000000 xplotlib-0.0.5/src/XPlotLib/XPlotLibUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:41:51.000000 xplotlib-0.0.5/src/XPlotLib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:41:56.400501 xplotlib-0.0.5/src/XPlotLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-02 21:41:56.000000 xplotlib-0.0.5/src/XPlotLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-02 21:41:56.000000 xplotlib-0.0.5/src/XPlotLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:41:56.000000 xplotlib-0.0.5/src/XPlotLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 21:41:56.000000 xplotlib-0.0.5/src/XPlotLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 21:41:56.000000 xplotlib-0.0.5/src/XPlotLib.egg-info/top_level.txt
```

### Comparing `xplotlib-0.0.4/LICENSE` & `xplotlib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xplotlib-0.0.4/PKG-INFO` & `xplotlib-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XPlotLib
-Version: 0.0.4
+Version: 0.0.5
 Summary: Libary to plot experimental and theoretical XRay data.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xplotlib-0.0.4/setup.cfg` & `xplotlib-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = XPlotLib
-version = 0.0.4
+version = 0.0.5
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = Libary to plot experimental and theoretical XRay data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers =
```

### Comparing `xplotlib-0.0.4/src/XPlotLib/BandgapAnalyzer.py` & `xplotlib-0.0.5/src/XPlotLib/BandgapAnalyzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -312,8 +312,39 @@
     -------
     float
         Core hole shift
     """
     def calc_core_hole_shift(self):
         return min(self.es_onsets) - min(self.gs_onsets)
 
+
+    """
+    Export 2nd derivative of XES and XAS spectra to csv files
+
+    Parameters
+    ----------
+    path : str
+        Path to the directory where the files will be saved
+    name : str
+        Name of the files (without extension)
+    """
+
+    def export_2nd_derivative(self, path, name):
+        xes_2nd = pd.DataFrame()
+        for xes_exp_name in self.xes_exp_spectra.keys():
+            if f'{xes_exp_name}_smoothed_2nd' not in self.xes_exp_spectra[xes_exp_name].columns:
+                print(f'No 2nd derivative found for {xes_exp_name}. Run smoothen method first, if you want to export the 2nd derivative.')
+                continue
+            xes_2nd[f'{xes_exp_name}_energy'] = self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_energy']
+            xes_2nd[f'{xes_exp_name}_2nd'] = self.xes_exp_spectra[xes_exp_name][f'{xes_exp_name}_smoothed_2nd']
+        xes_2nd.to_csv(f'{path}/{name}_XES_2nd.csv', index=False)
+
+        xas_2nd = pd.DataFrame()
+        for xas_exp_name in self.xas_exp_spectra.keys():
+            if f'{xas_exp_name}_smoothed_2nd' not in self.xas_exp_spectra[xas_exp_name].columns:
+                print(f'No 2nd derivative found for {xas_exp_name}. Run smoothen method first, if you want to export the 2nd derivative.')
+                continue
+            xas_2nd[f'{xas_exp_name}_energy'] = self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_energy']
+            xas_2nd[f'{xas_exp_name}_2nd'] = self.xas_exp_spectra[xas_exp_name][f'{xas_exp_name}_smoothed_2nd']
+        xas_2nd.to_csv(f'{path}/{name}_XAS_2nd.csv', index=False)
+
```

### Comparing `xplotlib-0.0.4/src/XPlotLib/DOSAnalyzer.py` & `xplotlib-0.0.5/src/XPlotLib/DOSAnalyzer.py`

 * *Files identical despite different names*

### Comparing `xplotlib-0.0.4/src/XPlotLib/XPlotLibUtils.py` & `xplotlib-0.0.5/src/XPlotLib/XPlotLibUtils.py`

 * *Files identical despite different names*

### Comparing `xplotlib-0.0.4/src/XPlotLib.egg-info/PKG-INFO` & `xplotlib-0.0.5/src/XPlotLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XPlotLib
-Version: 0.0.4
+Version: 0.0.5
 Summary: Libary to plot experimental and theoretical XRay data.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

