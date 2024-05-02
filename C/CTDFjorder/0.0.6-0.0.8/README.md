# Comparing `tmp/ctdfjorder-0.0.6.tar.gz` & `tmp/CTDFjorder-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "CTDFjorder-0.0.8.tar", last modified: Thu May  2 00:47:19 2024, max compression
```

## Comparing `ctdfjorder-0.0.6.tar` & `CTDFjorder-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,16 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/CTDFjorder.iml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/build.bat
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/build.sh
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/environment.yml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/meta.yaml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/requirements.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/setup.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/.idea/.gitignore
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/.idea/vcs.xml
--rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/.idea/workspace.xml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/Makefile
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/make.bat
--rw-r--r--   0        0        0    54980 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/CTDFjorder/CTDFjorder.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/CTDFjorder/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/src/CTDFjorder/make.bat
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/LICENSE
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ctdfjorder-0.0.6/PKG-INFO
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-05-02 00:47:19.727766 CTDFjorder-0.0.8/
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-05-02 00:47:19.726408 CTDFjorder-0.0.8/CTDFjorder/
+-rw-r--r--   0 nik        (501) staff       (20)    61105 2024-05-02 00:37:44.000000 CTDFjorder-0.0.8/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0 nik        (501) staff       (20)       54 2024-05-01 23:49:45.000000 CTDFjorder-0.0.8/CTDFjorder/__init__.py
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-05-02 00:47:19.727259 CTDFjorder-0.0.8/CTDFjorder.egg-info/
+-rw-r--r--   0 nik        (501) staff       (20)      949 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (501) staff       (20)      280 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (501) staff       (20)        1 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (501) staff       (20)       51 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/entry_points.txt
+-rw-r--r--   0 nik        (501) staff       (20)      128 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/requires.txt
+-rw-r--r--   0 nik        (501) staff       (20)       11 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/top_level.txt
+-rw-r--r--   0 nik        (501) staff       (20)     1053 2024-05-01 06:24:38.000000 CTDFjorder-0.0.8/LICENSE
+-rw-r--r--   0 nik        (501) staff       (20)      949 2024-05-02 00:47:19.727554 CTDFjorder-0.0.8/PKG-INFO
+-rw-r--r--   0 nik        (501) staff       (20)       47 2024-05-01 06:11:00.000000 CTDFjorder-0.0.8/README.md
+-rw-r--r--   0 nik        (501) staff       (20)       38 2024-05-02 00:47:19.727812 CTDFjorder-0.0.8/setup.cfg
+-rw-r--r--   0 nik        (501) staff       (20)     1200 2024-05-02 00:11:24.000000 CTDFjorder-0.0.8/setup.py
```

### Comparing `ctdfjorder-0.0.6/src/CTDFjorder/CTDFjorder.py` & `CTDFjorder-0.0.8/CTDFjorder/CTDFjorder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,46 @@
+# -*- coding: utf-8 -*-
 import itertools
 import os
 import sys
 import traceback
-
 import numpy as np
 import pandas
 import pandas as pd
 from pyrsktools import RSK
 import gsw
 import matplotlib.pyplot as plt
-from matplotlib.ticker import ScalarFormatter
-from scipy.interpolate import CubicSpline
 import statsmodels.api
 from matplotlib.ticker import ScalarFormatter
-import hashlib
 from tabulate import tabulate
 
+class CTDError(Exception):
+    """Exception raised for CTD related errors.
+
+    Attributes:
+        filename -- input dataset which caused the error
+        message -- explanation of the error
+    """
+    def __init__(self, filename, message=" Unknown, check to make sure your mastersheet is in your current directory."):
+        self.filename = filename
+        self.message = message
+        super().__init__(self.message)
 
 class CTDFjorder:
     """
     CTDFjorder
     ==========
 
     CTDFjorder class for processing and analyzing CTD data.
 
     This class provides methods for reading RSK files, processing CTD data,
     calculating derived quantities, and generating plots.
 
-    Constants
-    ---------
-
-    :master_sheet_path: Path to the master sheet Excel file.
+    :var master_sheet_path: Path to the master sheet Excel file.
 
-    Methods
-    ________
-
-    :run_default(): Run the full pipeline on all rsk files in the current directory.
-
-    Classes
-    --------
-
-    :_Filesystem: Utility class for file system operations.
-    :CTD: Class representing a CTD object for processing and analyzing C
     Usage
     ------
 
     To run the default processing pipeline::
 
         CTDFjorder.run_default()
 
@@ -55,19 +50,20 @@
     Nikolas Yanek-Chrones
 
     Date
     -----
 
     May 1, 2024
     """
-    master_sheet_path = "FjordPhyto MASTER SHEET.xlsx"
+    master_sheet_path = None
 
     @staticmethod
     def run_default():
         filesys = CTDFjorder._Filesystem()
+        CTDFjorder.master_sheet_path = os.path.join(CTDFjorder._Filesystem.get_cwd(), "FjordPhyto MASTER SHEET.xlsx")
         rsk_files_list = CTDFjorder._Filesystem.get_rsk_files_in_working_directory(filesys.get_cwd())
         for file in rsk_files_list:
             try:
                 my_data = CTDFjorder.CTD(file)
                 my_data.add_filename_to_table()
                 my_data.save_to_csv("output.csv")
                 my_data.add_location_to_table()
@@ -83,14 +79,15 @@
                 print(traceback.format_exc())
                 print(e)
                 continue
 
     @staticmethod
     def merge_all_in_folder():
         filesys = CTDFjorder._Filesystem()
+        CTDFjorder.master_sheet_path = os.path.join(CTDFjorder._Filesystem.get_cwd(), "FjordPhyto MASTER SHEET.xlsx")
         rsk_files_list = CTDFjorder._Filesystem.get_rsk_files_in_working_directory(filesys.get_cwd())
         for file in rsk_files_list:
             try:
                 my_data = CTDFjorder.CTD(file)
                 my_data.add_filename_to_table()
                 my_data.add_location_to_table()
                 my_data.save_to_csv("output.csv")
@@ -101,22 +98,14 @@
 
     class _Filesystem:
         """
         _Filesystem
         -----------
         
         Utility class for file system operations.
-        
-        Methods
-        ~~~~~~~
-        
-        :get_rsk_files_in_working_directory(working_directory): Get a list of RSK files in the working directory.
-        :get_cwd(): Get the current working directory.
-        :get_filename(filepath): Extract the filename from a file path.
-        :reset_file_environment(): Reset the file environment by removing output files and creating necessary directories.
         """
 
         @staticmethod
         def get_rsk_files_in_working_directory(working_directory):
             rsk_files_list = []
             rsk_filenames_no_path = []
             for filename in os.listdir(working_directory):
@@ -133,39 +122,35 @@
         @staticmethod
         def get_cwd():
             working_directory_path = None
             # determine if application is a script file or frozen exe
             if getattr(sys, 'frozen', False):
                 working_directory_path = os.path.dirname(sys.executable)
             elif __file__:
-                working_directory_path = os.path.dirname(__file__)
+                working_directory_path = os.getcwd()
+            else:
+                working_directory_path = os.getcwd()
             return working_directory_path
 
         @staticmethod
         def get_filename(filepath):
             return '_'.join(filepath.split("/")[-1].split("_")[0:3]).split('.rsk')[0]
 
         @staticmethod
         def reset_file_environment():
-            CTDFjorder.master_sheet_path = "FjordPhyto MASTER SHEET.xlsx"
+            CTDFjorder.master_sheet_path = os.path.join(CTDFjorder._Filesystem.get_cwd(), "FjordPhyto MASTER SHEET.xlsx")
             output_file_csv = "output.csv"
             output_file_csv_clean = "output_clean.csv"
             output_plots_dir = "plots"
-            working_directory_path = None
-            # determine if application is a script file or frozen exe
-            if getattr(sys, 'frozen', False):
-                working_directory_path = os.path.dirname(sys.executable)
-            elif __file__:
-                working_directory_path = os.path.dirname(__file__)
-            cwd = working_directory_path
+            cwd = CTDFjorder.CTD.get_cwd()
             CTDFjorder.master_sheet_path = os.path.join(cwd, CTDFjorder.master_sheet_path)
             output_file_csv = os.path.join(cwd, output_file_csv)
             output_file_csv_clean = os.path.join(cwd, output_file_csv_clean)
             if cwd is None:
-                raise RuntimeError("Couldn't get working dir")
+                raise CTDError("", "Couldn't get working directory.")
             if os.path.isfile(output_file_csv):
                 os.remove(output_file_csv)
             if os.path.isfile(output_file_csv_clean):
                 os.remove(output_file_csv_clean)
             if os.path.isdir("./plots.gif"):
                 os.remove("./plots/gif")
             if not os.path.isdir("./plots"):
@@ -176,49 +161,21 @@
     class CTD():
         """
         CTD
         ---
         
         Class representing a CTD object for processing and analyzing CTD data.
         
-        Attributes
-        ~~~~~~~~~~
-        
-        :_ctd_array: DataFrame containing CTD data.
-        :_rsk: RSK object for reading RSK files.
-        :_filename: Filename of the RSK file.
-        :_utils: Utility object for CTD data processing.
-        :_calculator: Calculator object for CTD data calculations.
-        :_plotter: Placeholder for plotter object.
-        :_cwd: Current working directory.
-        
-        Methods
-        ~~~~~~~
-        
-        :__init__(self, rskfilepath): Initialize a CTD object with the specified RSK file path.
-        :view_table(): Print the CTD data table.
-        :add_filename_to_table(): Add the filename to the CTD data table.
-        :add_location_to_table(): Add location information to the CTD data table.
-        :remove_non_positive_samples(): Remove samples with non-positive values.
-        :run_complex_cleaner(feature, method): Run complex data cleaning on the specified feature using the specified method.
-        :add_absolute_salinity(): Add absolute salinity to the CTD data table.
-        :add_density(): Add density to the CTD data table.
-        :add_overturns(): Add overturns to the CTD data table.
-        :addMeanSurfaceDensity(): Add mean surface density to the CTD data table.
-        :add_mld(reference, method): Add mixed layer depth (MLD) to the CTD data table.
-        :save_to_csv(output_file): Save the CTD data table to a CSV file.
-        :plot_depth_salinity_density_mld_line(): Generate a line plot of depth vs. salinity, density, and MLD.
-        :plot_depth_density_salinity_mld_scatter(): Generate a scatter plot of depth vs. density, salinity, and MLD.
-        :plot_depth_temperature_scatter(): Generate a scatter plot of depth vs. temperature.
-        
-        Classes
-        ~~~~~~~
-        
-        :_Utility: Utility class for CTD data processing.
-        :_Calculate: Class for CTD data calculations.
+        :var _ctd_array: DataFrame containing CTD data.
+        :var _rsk: RSK object for reading RSK files.
+        :var _filename: Filename of the RSK file.
+        :var _utils: Utility object for CTD data processing.
+        :var _calculator: Calculator object for CTD data calculations.
+        :var _plotter: Placeholder for plotter object.
+        :var _cwd: Current working directory.
         """
         _ctd_array = pandas.DataFrame()
         _rsk = None
         _filename = None
         _utils = None
         _calculator = None
         _plotter = None
@@ -228,144 +185,228 @@
         _DENSITY_CALCULATION_ERROR = "Could not calculate density on this dataset."
         _SALINITYABS_CALCULATION_ERROR = "Could not calculate density on this dataset."
         _DATA_CLEANING_ERROR = "No data remains after data cleaning, reverting to previous CTD"
         _REMOVE_NEGATIVES_ERROR = "No data remains after removing non-positive samples."
         _MLD_ERROR = "No data remains after calculating MLD."
 
         def __init__(self, rskfilepath):
+            """
+            Initialize a new CTD object.
+
+            :param rskfilepath: The file path to the RSK file.
+            """
             self._rsk = RSK(rskfilepath)
             self._filename = ('_'.join(rskfilepath.split("/")[-1].split("_")[0:3]).split(".rsk")[0])
             print("New CTDFjorder Object Created from : " + self._filename)
             self._ctd_array = np.array(self._rsk.npsamples())
             self._ctd_array = pd.DataFrame(self._ctd_array)
             self._utils = self._Utility(self._filename, )
             self._calculator = self._Calculate
-            self._cwd = self._get_cwd()
+            self._cwd = self.get_cwd()
 
         @staticmethod
-        def _get_cwd():
+        def get_cwd():
             working_directory_path = None
             # determine if application is a script file or frozen exe
             if getattr(sys, 'frozen', False):
                 working_directory_path = os.path.dirname(sys.executable)
             elif __file__:
-                working_directory_path = os.path.dirname(__file__)
+                working_directory_path = os.getcwd()
+            else:
+                working_directory_path = os.getcwd()
             return working_directory_path
 
         def view_table(self):
+            """
+            Print the CTD data table.
+            """
             print(tabulate(self._ctd_array, headers='keys', tablefmt='psql'))
 
         def add_filename_to_table(self):
+            """
+            Add the filename to the CTD data table.
+            """
             self._ctd_array.assign(filename=self._filename)
 
         def add_location_to_table(self):
+            """
+            Add latitude and longitude information to the CTD data table.
+
+            Retrieves the sample location data from the RSK file and adds it to the CTD data table.
+            If no location data is found, it attempts to estimate the location using the master sheet.
+            """
             self._ctd_array = self._utils.remove_sample_timezone_indicator(self._ctd_array)
             location_data = self._utils.get_sample_location(self._rsk, self._filename)
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._NO_SAMPLES_ERROR
+            if self._utils.no_values_in_object(self._ctd_array):
+                raise CTDError(self._filename, self._NO_SAMPLES_ERROR)
             try:
                 self._ctd_array = self._ctd_array.assign(latitude=location_data[0],
                                                          longitude=location_data[1])
             except Exception:
                 self._ctd_array.loc['latitude'] = None
                 self._ctd_array.loc['longitude'] = None
                 self._ctd_array.loc['filename'] = None
-                raise Exception(self._NO_LOCATION_ERROR)
+                raise CTDError(self._filename, self._NO_LOCATION_ERROR)
 
         def remove_non_positive_samples(self):
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._NO_SAMPLES_ERROR
+            """
+            Remove samples with non-positive depth, pressure, salinity, absolute salinity, or density.
+
+            Iterates through the columns of the CTD data table and removes rows with non-positive values
+            for depth, pressure, salinity, absolute salinity, or density.
+            """
+            if self._utils.no_values_in_object(self._ctd_array):
+                raise CTDError(self._filename, self._NO_SAMPLES_ERROR)
             for column in self._ctd_array.columns:
                 match column:
                     case 'depth_00':
                         self._ctd_array = self._utils.remove_rows_with_negative_depth(self._ctd_array)
                     case 'pressure_00':
                         self._ctd_array = self._utils.remove_rows_with_negative_pressure(self._ctd_array)
                     case 'salinity_00':
                         self._ctd_array = self._utils.remove_rows_with_negative_salinity(self._ctd_array)
                     case 'salinityabs':
                         self._ctd_array = self._utils.remove_rows_with_negative_salinityabs(self._ctd_array)
                     case 'density':
                         self._ctd_array = self._utils.remove_rows_with_negative_density(self._ctd_array)
             if self._utils.no_values_in_object(self._ctd_array):
-                raise Exception(self._REMOVE_NEGATIVES_ERROR)
+                raise CTDError(self._filename, self._REMOVE_NEGATIVES_ERROR)
 
         def run_complex_cleaner(self, feature, method='salinitydiff'):
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._NO_SAMPLES_ERROR
+            """
+            Run complex data cleaning methods on the specified feature.
+
+            :param feature: The feature to clean (e.g., 'practicalsalinity').
+            :param method: The cleaning method to apply (default: 'salinitydiff').
+
+            Applies complex data cleaning methods to the specified feature based on the selected method.
+            Currently supports cleaning practical salinity using the 'salinitydiff' method.
+            """
+            if self._utils.no_values_in_object(self._ctd_array):
+                raise CTDError(self._filename, self._NO_SAMPLES_ERROR)
             supported_features = {
                 "practicalsalinity": "salinity_00"
             }
             supported_methods = {
-                "salinitydiff": self._calculator.calculate_and_drop_salinity_spikes(self._ctd_array, self._filename)
+                "salinitydiff": self._calculator.calculate_and_drop_salinity_spikes(self._ctd_array)
             }
             if feature in supported_features.keys():
                 if method in supported_methods.keys():
                     self._ctd_array.loc[self._ctd_array.index, 'salinity_00'] = supported_methods[method]
                 else:
                     print(f"run_complex_cleaner: Invalid method \"{method}\" not in {supported_methods.keys()}")
             else:
                 print(f"run_complex_cleaner: Invalid feature \"{feature}\" not in {supported_features.keys()}.")
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._DATA_CLEANING_ERROR
+            if self._utils.no_values_in_object(self._ctd_array):
+                raise CTDError(self._filename, self._DATA_CLEANING_ERROR)
 
         def add_absolute_salinity(self):
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._NO_SAMPLES_ERROR
+            """
+            Calculate and add absolute salinity to the CTD data table.
+
+            Calculates the absolute salinity using the TEOS-10 equations and adds it as a new column
+            to the CTD data table. Removes rows with negative absolute salinity values.
+            """
+            if self._utils.no_values_in_object(self._ctd_array):
+                raise CTDError(self._filename, self._NO_SAMPLES_ERROR)
             self._ctd_array.loc[self._ctd_array.index, 'salinityabs'] = self._calculator.calculate_absolute_salinity(
                 self._ctd_array)
             self._ctd_array = self._utils.remove_rows_with_negative_salinityabs(self._ctd_array)
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._SALINITYABS_CALCULATION_ERROR
+            if self._utils.no_values_in_object(self._ctd_array):
+                raise CTDError(self._filename, self._SALINITYABS_CALCULATION_ERROR)
 
         def add_density(self):
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._NO_SAMPLES_ERROR
+            """
+            Calculate and add density to the CTD data table.
+
+            Calculates the density using the TEOS-10 equations and adds it as a new column to the CTD
+            data table. If absolute salinity is not present, it is calculated first.
+            """
+            if self._utils.no_values_in_object(self._ctd_array):
+                raise CTDError(self._filename, self._NO_SAMPLES_ERROR)
             if 'salinityabs' in self._ctd_array.columns:
                 self._ctd_array.loc[self._ctd_array.index, 'density'] = self._calculator.calculate_absolute_density(
                     self._ctd_array)
             else:
                 self._ctd_array.loc[self._ctd_array.index, 'salinityabs'] = self.add_absolute_salinity()
                 self._ctd_array = self._calculator.calculate_absolute_density(self._ctd_array)
                 self._ctd_array.loc[self._ctd_array.index, 'density'] = self._calculator.calculate_absolute_density(
                     self._ctd_array)
                 self._ctd_array.drop('salinityabs')
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._DENSITY_CALCULATION_ERROR
+                if self._utils.no_values_in_object(self._ctd_array):
+                    raise CTDError(self._filename, self._DENSITY_CALCULATION_ERROR)
 
         def add_overturns(self):
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._NO_SAMPLES_ERROR
+            """
+            Identify and add density overturns to the CTD data table.
+
+            Calculates density changes between consecutive measurements and identifies overturns where
+            denser water lies above less dense water. Adds an 'overturn' column to the CTD data table.
+            """
+            if self._utils.no_values_in_object(self._ctd_array):
+                raise CTDError(self._filename, self._NO_SAMPLES_ERROR)
             self._ctd_array = self._calculator.calculate_overturns(self._ctd_array.copy())
 
         def addMeanSurfaceDensity(self):
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._NO_SAMPLES_ERROR
+            """
+            Calculate and add mean surface density to the CTD data table.
+
+            Calculates the mean surface density from the density values and adds it as a new column
+            to the CTD data table.
+            """
+            if self._utils.no_values_in_object(self._ctd_array):
+                raise CTDError(self._filename, self._NO_SAMPLES_ERROR)
             mean_surface_density = self._calculator.calculate_mean_surface_density(self._ctd_array.copy())
             self._ctd_array = self._ctd_array.assign(mean_surface_density=mean_surface_density)
 
         def add_mld(self, reference, method="default"):
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._NO_SAMPLES_ERROR
+            """
+            Calculate and add mixed layer depth (MLD) to the CTD data table.
+
+            :param reference: The reference depth for MLD calculation.
+            :param method: The MLD calculation method (default: "default").
+
+            Calculates the mixed layer depth using the specified method and reference depth.
+            Adds the MLD and the actual reference depth used as new columns to the CTD data table.
+            """
+            if self._utils.no_values_in_object(self._ctd_array):
+                raise CTDError(self._filename, self._NO_SAMPLES_ERROR)
             copy_ctd_array = self._ctd_array.copy()
             supported_methods = [
-                "LOESS",
                 "default"
             ]
             unpack = None
-            if method == "LOESS":
-                unpack = self._calculator.calculate_mld_LOESS(copy_ctd_array['density'], copy_ctd_array['depth_00'],
-                                                              reference)
+
             if method == "default":
                 unpack = self._calculator.calculate_mld(copy_ctd_array['density'], copy_ctd_array['depth_00'],
                                                         reference)
             else:
                 print(f"add_mld: Invalid method \"{method}\" not in {supported_methods}")
                 unpack = [None, None]
             if unpack is None:
                 unpack = [None, None]
-                raise RuntimeWarning("MLD could not be calculated.")
+                raise CTDError("MLD could not be calculated.")
             MLD = unpack[0]
             depth_used_as_reference = unpack[1]
             self._ctd_array.loc[self._ctd_array.index, f'MLD {reference}'] = MLD
             self._ctd_array.loc[
                 self._ctd_array.index, f'MLD {reference} Actual Reference Depth'] = depth_used_as_reference
             self._ctd_array = copy_ctd_array.merge(self._ctd_array)
-            assert (not self._utils.no_values_in_object(self._ctd_array)), self._MLD_ERROR
+            if self._utils.no_values_in_object(self._ctd_array):
+                raise CTDError(self._filename, self._MLD_ERROR)
 
         def save_to_csv(self, output_file):
+            """
+            Save the CTD data table to a CSV file.
+
+            :param output_file: The output CSV file path.
+
+            Renames the columns of the CTD data table based on a predefined mapping and saves the
+            data to the specified CSV file. If the file already exists, the data is appended to it.
+            """
             rsk_labels = {
                 "temperature_00": "Temperature (°C)",
                 "pressure_00": "Pressure (dbar)",
                 "chlorophyll_00": "Chlorophyll a (µg/l)",
                 "seapressure_00": "Sea Pressure (dbar)",
                 "depth_00": "Depth (m)",
                 "salinity_00": "Salinity (PSU)",
@@ -404,14 +445,21 @@
 
             return merged_df
 
         # =============================================================================
         # Section: Plotting Functions
         # =============================================================================
         def plot_depth_salinity_density_mld_line(self):
+            """
+            Plot depth vs. salinity and density with MLD lines using LOESS smoothing.
+
+            Generates a plot of depth vs. salinity and density, applying LOESS smoothing to the data.
+            Adds horizontal lines indicating the mixed layer depth (MLD) at different reference depths.
+            Saves the plot as an image file.
+            """
             df = self._ctd_array.copy()
             filename = self._filename
             plt.rcParams.update({'font.size': 16})
             df_filtered = df
             if df_filtered.isnull().values.any():
                 df_filtered.dropna(inplace=True)  # Drop rows with NaNs
             df_filtered = df_filtered.reset_index(drop=True)
@@ -462,14 +510,21 @@
             ax2_legend = ax2.get_legend_handles_labels()
             ax1.legend(lines + ax2_legend[0], labels + ax2_legend[1], loc='lower center', bbox_to_anchor=(0.5, -0.15),
                        ncol=3)
             plt.savefig(os.path.join(self._cwd, f"plots/{filename}_salinity_density_depth_plot_dual_x_axes_line.png"))
             plt.close(fig)
 
         def plot_depth_density_salinity_mld_scatter(self):
+            """
+            Plot depth vs. salinity and density with MLD lines using scatter points.
+
+            Generates a scatter plot of depth vs. salinity and density.
+            Adds horizontal lines indicating the mixed layer depth (MLD) at different reference depths.
+            Saves the plot as an image file.
+            """
             df = self._ctd_array.copy()
             filename = self._filename
             plt.rcParams.update({'font.size': 16})
             df_filtered = df
             if df_filtered.empty:
                 plt.close()
                 return
@@ -515,14 +570,21 @@
             ax2_legend = ax2.get_legend_handles_labels()
             ax1.legend(lines + ax2_legend[0], labels + ax2_legend[1], loc='upper center', bbox_to_anchor=(0.5, -0.15),
                        ncol=3)
             plt.savefig(os.path.join(self._cwd, f"plots/{filename}_salinity_density_depth_plot_dual_x_axes.png"))
             plt.close(fig)
 
         def plot_depth_temperature_scatter(self):
+            """
+            Plot depth vs. temperature with MLD lines using scatter points.
+
+            Generates a scatter plot of depth vs. temperature.
+            Adds horizontal lines indicating the mixed layer depth (MLD) at different reference depths.
+            Saves the plot as an image file.
+            """
             df = self._ctd_array.copy()
             filename = self._filename
             plt.rcParams.update({'font.size': 16})
             df_filtered = df
             if df_filtered.empty:
                 plt.close()
                 return
@@ -568,49 +630,58 @@
         class _Utility:
             """
             _Utility
             --------
 
             Utility class for CTD data processing.
 
-            Attributes
-            ~~~~~~~~~~
-
-            :filename: Filename of the RSK file.
-            :mastersheet: Path to the master sheet Excel file.
-
-            Methods
-            ~~~~~~~
-
-            :__init__(self, filename): Initialize a _Utility object with the specified filename.
-            :no_values_in_object(object_to_check): Check if an object has no values.
-            :process_master_sheet(master_sheet_path, filename): Process the master sheet to extract location information.
-            :get_sample_location(rsk, filename): Get the sample location from the RSK file or master sheet.
-            :remove_sample_timezone_indicator(df): Remove the timezone indicator from the timestamp column.
-            :remove_rows_with_negative_depth(df): Remove rows with negative depth values.
-            :remove_rows_with_negative_salinity(df): Remove rows with negative salinity values.
-            :remove_rows_with_negative_pressure(df): Remove rows with negative pressure values.
-            :remove_rows_with_negative_salinityabs(df): Remove rows with negative absolute salinity values.
-            :remove_rows_with_negative_density(df): Remove rows with negative density values.
-            :find_stratification(depth, stratification_dict): Find the stratification value for a given depth.
+            :var filename: Filename of the RSK file.
+            :var mastersheet: Path to the master sheet Excel file.
             """
 
             def __init__(self, filename):
+                """
+                Initialize a new _Utility object.
+
+                :param filename: The filename of the RSK file.
+                """
                 self.filename = filename
-                self.mastersheet = CTDFjorder.master_sheet_path
+                self.mastersheet = os.path.join(CTDFjorder._Filesystem.get_cwd(), CTDFjorder.master_sheet_path)
 
             def no_values_in_object(self, object_to_check):
+                """
+                Check if an object has no values.
+
+                :param object_to_check: The object to check for values.
+                :return: True if the object has no values, False otherwise.
+
+                Checks if the given object is None, empty, or has a length greater than 0.
+                Returns True if the object has no values, False otherwise.
+                """
                 if isinstance(object_to_check, type(None)):
                     return True
                 if object_to_check.empty:
                     return True
                 if len(object_to_check) > 0:
                     return False
 
             def process_master_sheet(self, master_sheet_path, filename):
+                """
+                Process the master sheet to find the closest location and time for a given filename.
+
+                :param master_sheet_path: The path to the master sheet Excel file.
+                :param filename: The filename of the RSK file.
+                :return: A tuple containing the estimated latitude, longitude, and updated filename.
+
+                Extracts the date and time components from the filename and compares them with the data
+                in the master sheet. Calculates the absolute differences between the dates and times to
+                find the closest match. Returns the estimated latitude, longitude, and updated filename
+                based on the closest match.
+                """
+
                 def get_date_from_string(filename):
                     try:
                         year = filename.split('_')[1][:4]
                         month = filename.split('_')[1][4:6]
                         day = filename.split('_')[1][6:]
                         hour = filename.split('_')[2][0:2]
                         minute = filename.split('_')[2][2:4]
@@ -676,14 +747,25 @@
                 print("Long: " + str(longitude))
                 if closest_time_time:
                     print("Closest Time:", closest_time_time)
                 print("====================")
                 return latitude, longitude, RBRfilename
 
             def get_sample_location(self, rsk, filename):
+                """
+                Get the sample location from the RSK file or estimate it using the master sheet.
+
+                :param rsk: The RSK object.
+                :param filename: The filename of the RSK file.
+                :return: A tuple containing the latitude, longitude, and updated filename.
+
+                Retrieves the sample location data from the RSK file. If no location data is found,
+                it attempts to estimate the location using the master sheet. Returns the latitude,
+                longitude, and updated filename.
+                """
                 # Adding geo data, assumes no drift and uses the first lat long in the file if there is one
                 geo_data_length = len(list(itertools.islice(rsk.geodata(), None)))
                 if geo_data_length < 1:
                     latitude_intermediate, longitude_intermediate, filename = self.process_master_sheet(
                         self.mastersheet, filename)
                     return latitude_intermediate, longitude_intermediate, filename
                 else:
@@ -706,106 +788,141 @@
                                 latitude_intermediate, longitude_intermediate, filename = self.process_master_sheet(
                                     self.mastersheet, filename)
                                 return latitude_intermediate, longitude_intermediate, filename
                         else:
                             return None, None, filename + 'gpserror'
 
             def remove_sample_timezone_indicator(self, df):
+                """
+                Remove the timezone indicator from the 'timestamp' column of a DataFrame.
+
+                :param df: The DataFrame to process.
+                :return: The updated DataFrame with the timezone indicator removed.
+
+                Removes the timezone indicator (e.g., '+00:00') from the 'timestamp' column of the
+                given DataFrame. Returns the updated DataFrame.
+                """
                 if self.no_values_in_object(df):
                     return None
                 if 'timestamp' in df.columns:
                     df['timestamp'] = df['timestamp'].astype(str).str.split('+').str[0]
                     return df
                 else:
                     return df
 
             def remove_rows_with_negative_depth(self, df):
+                """
+                Remove rows with negative depth values from a DataFrame.
+
+                :param df: The DataFrame to process.
+                :return: The updated DataFrame with rows containing negative depth values removed.
+
+                Removes rows from the given DataFrame where the 'depth_00' column has negative values.
+                Returns the updated DataFrame.
+                """
                 if self.no_values_in_object(df):
                     return None
                 if 'depth_00' in df.columns:
                     df = df[df['depth_00'] >= 0].reset_index(drop=True)
                 else:
                     return None
                 if self.no_values_in_object(df):
                     return None
                 return df.copy()
 
             def remove_rows_with_negative_salinity(self, df):
+                """
+                Remove rows with negative salinity values from a DataFrame.
+
+                :param df: The DataFrame to process.
+                :return: The updated DataFrame with rows containing negative salinity values removed.
+
+                Removes rows from the given DataFrame where the 'salinity_00' column has negative values.
+                Returns the updated DataFrame.
+                """
                 if self.no_values_in_object(df):
                     return None
                 if 'salinity_00' in df.columns:
                     df = df[df['salinity_00'] >= 0].reset_index(drop=True)
                 else:
                     return None
                 if self.no_values_in_object(df):
                     return None
                 return df.copy()
 
             def remove_rows_with_negative_pressure(self, df):
+                """
+                Remove rows with negative pressure values from a DataFrame.
+
+                :param df: The DataFrame to process.
+                :return: The updated DataFrame with rows containing negative pressure values removed.
+
+                Removes rows from the given DataFrame where the 'pressure_00' column has negative values.
+                Returns the updated DataFrame.
+                """
                 if self.no_values_in_object(df):
                     return None
                 if 'pressure_00' in df.columns:
                     df = df[df['pressure_00'] >= 0].reset_index(drop=True)
                 else:
                     return None
                 if self.no_values_in_object(df):
                     return None
                 return df.copy()
 
             def remove_rows_with_negative_salinityabs(self, df):
+                """
+                Remove rows with negative absolute salinity values from a DataFrame.
+
+                :param df: The DataFrame to process.
+                :return: The updated DataFrame with rows containing negative absolute salinity values removed.
+
+                Removes rows from the given DataFrame where the 'salinityabs' column has negative values.
+                Returns the updated DataFrame.
+                """
                 if self.no_values_in_object(df):
                     return None
                 if 'salinityabs' in df.columns:
                     df = df[df['salinityabs'] >= 0].reset_index(drop=True)
                 else:
                     return None
                 if self.no_values_in_object(df):
                     return None
                 return df.copy()
 
             def remove_rows_with_negative_density(self, df):
+                """
+                Remove rows with negative density values from a DataFrame.
+
+                :param df: The DataFrame to process.
+                :return: The updated DataFrame with rows containing negative density values removed.
+
+                Removes rows from the given DataFrame where the 'density' column has negative values.
+                Returns the updated DataFrame.
+                """
                 if self.no_values_in_object(df):
                     return None
                 if 'density' in df.columns:
                     df = df[df['density'] >= 0].reset_index(drop=True)
                 else:
                     return None
                 if self.no_values_in_object(df):
                     return None
                 return df.copy()
 
-            def find_stratification(self, depth, stratification_dict):
-                for depth_range, value in stratification_dict.items():
-                    lower, upper = map(int, depth_range.replace('m', '').split('-'))
-                    if lower <= depth < upper:
-                        return value
-                return np.nan  # In case no range matches
-
         # =============================================================================
         # Section: Calculation Functions
         # =============================================================================
 
         class _Calculate:
             """
             _Calculate
             ----------
 
             Class for CTD data calculations.
-
-            Methods
-            ~~~~~~~
-
-            :gsw_infunnel(SA, CT, p): Check if Absolute Salinity, Conservative Temperature, and pressure are within the "oceanographic funnel" for the TEOS-10 75-term equation.
-            :calculate_and_drop_salinity_spikes(df, filename): Calculate and drop salinity spikes from the CTD data.
-            :calculate_overturns(ctd_array): Calculate overturns in the CTD data.
-            :calculate_absolute_density(ctd_array): Calculate absolute density from the CTD data.
-            :calculate_absolute_salinity(ctd_array): Calculate absolute salinity from the CTD data.
-            :calculate_mld(densities, depths, reference_depth): Calculate the mixed layer depth (MLD) using the density threshold method.
-            :calculate_mld_LOESS(densities, depths, reference_depth): Calculate the mixed layer depth (MLD) using the LOESS smoothing method.
-            :calculate_mean_surface_density(df): Calculate the mean surface density from the CTD data.
             """
 
             @staticmethod
             def gsw_infunnel(SA, CT, p):
                 """
                 .. staticmethod:: gsw_infunnel(SA, CT, p)
                     :param SA: Absolute Salinity [g/kg]
@@ -814,18 +931,18 @@
                     :returns: A boolean series where True indicates the values are inside the "oceanographic funnel".
 
                 Checks if the given Absolute Salinity (SA), Conservative Temperature (CT), and pressure (p) are within the "oceanographic funnel" for the TEOS-10 75-term equation.
                 """
                 # Ensure all inputs are Series and aligned
                 if not (isinstance(SA, pd.Series) and isinstance(CT, pd.Series) and (
                         isinstance(p, pd.Series) or np.isscalar(p))):
-                    raise ValueError("SA, CT, and p must be pandas Series or p a scalar")
+                    raise CTDError("","SA, CT, and p must be pandas Series or p a scalar")
 
                 if isinstance(p, pd.Series) and (SA.index.equals(CT.index) and SA.index.equals(p.index)) is False:
-                    raise ValueError("Indices of SA, CT, and p must be aligned")
+                    raise CTDError("","Indices of SA, CT, and p must be aligned")
 
                 if np.isscalar(p):
                     p = pd.Series(p, index=SA.index)
 
                 # Define the funnel conditions
                 CT_freezing_p = gsw.CT_freezing(SA, p, 0)
                 CT_freezing_500 = gsw.CT_freezing(SA, 500, 0)
@@ -843,19 +960,18 @@
                         SA.isna() | CT.isna() | p.isna()
                 )
                 in_funnel[condition] = False
 
                 return in_funnel
 
             @staticmethod
-            def calculate_and_drop_salinity_spikes(df, filename):
+            def calculate_and_drop_salinity_spikes(df):
                 """
                 .. staticmethod:: calculate_and_drop_salinity_spikes(df, filename)
                     :param df: DataFrame containing depth and salinity data
-                    :param filename: Filename for output
                     :returns: DataFrame after removing salinity spikes
 
                 Calculates and removes salinity spikes from the CTD data based on predefined thresholds for acceptable changes in salinity with depth.
                 """
                 acceptable_delta_salinity_per_depth = [
                     (0.0005, 0.001),
                     (0.005, 0.01),
@@ -890,20 +1006,18 @@
                     groups = df.groupby(pd.cut(df['depth_00'], ranges), observed=True)
 
                     # Calculate the min and max salinity for each range and filter ranges where the difference is <= 1
                     filtered_groups = groups.filter(
                         lambda x: abs(x['salinity_00'].max() - x['salinity_00'].min()) <= acceptable_delta)
                     # Get the indices of the filtered groups
                     filtered_indices = filtered_groups.index
-                    # plot_salinity_spike_gif(df, i, filename, filtered_indices)
                     return filtered_groups
 
                 for i, deltas in enumerate(acceptable_delta_salinity_per_depth):
                     df = recursively_drop(df, deltas[0], deltas[1], i)
-                # plot_salinity_spike_gif(df, 10, filename, df.index)
                 return df
 
             @staticmethod
             def calculate_overturns(ctd_array):
                 """
                 .. staticmethod:: calculate_overturns(ctd_array)
                     :param ctd_array: DataFrame containing depth, density, and timestamp data
@@ -933,15 +1047,15 @@
                 SA = ctd_array['salinity_00']
                 t = ctd_array['temperature_00']
                 p = ctd_array['pressure_00']
                 CT = gsw.CT_from_t(SA, t, p)
                 if CTDFjorder.CTD._Calculate.gsw_infunnel(SA, CT, p).all():
                     return gsw.density.rho_t_exact(SA, t, p)
                 else:
-                    raise ValueError("Sample not in funnel, could not calculate density.")
+                    raise CTDError("","Sample not in funnel, could not calculate density.")
 
             @staticmethod
             def calculate_absolute_salinity(ctd_array):
                 """
                 .. staticmethod:: calculate_absolute_salinity(ctd_array)
                     :param ctd_array: DataFrame containing practical salinity, pressure, longitude, and latitude data
                     :returns: Series with calculated absolute salinity
@@ -986,15 +1100,15 @@
                             # Linear interpolation
                             try:
                                 reference_density = sorted_densities[i - 1] + (
                                         (sorted_densities[i] - sorted_densities[i - 1]) * (
                                         (reference_depth - sorted_depths[i - 1]) /
                                         (sorted_depths[i] - sorted_depths[i - 1])))
                             except:
-                                raise ValueError(
+                                raise CTDError("",
                                     f"Insufficient depth range to calculate MLD. Maximum sample depth is {depths.max()}, minimum is {depths.min()}")
                         break
                 if reference_density is None:
                     return None
                 # Find the depth where density exceeds the reference density by more than 0.05 kg/m³
                 for depth, density in zip(sorted_depths, sorted_densities):
                     if density > reference_density + 0.05 and depth >= reference_depth:
@@ -1058,21 +1172,67 @@
                   :param df: DataFrame containing density data
                   :returns: Mean surface density
 
                 Calculates the mean surface density from the CTD data, includes all depth ranges in profile.
                 """
                 return df['density'].mean()
 
+def main():
+    if len(sys.argv) < 2:
+        print("Usage: ctdfjorder <command> [arguments]")
+        print("Commands:")
+        print("  process <file>          Process a single RSK file")
+        print("  merge                   Merge all RSK files in the current folder")
+        print("  default                 Run the default processing pipeline")
+        print("CWD:")
+        print(CTDFjorder.CTD.get_cwd())
+        sys.exit(1)
 
-if __name__ == "__main__":
-    if len(sys.argv) > 1:
-        print("Wrong Usage")
+    command = sys.argv[1]
+
+    if command == "process":
+        if len(sys.argv) < 3:
+            print("Usage: ctdfjorder process <file>")
+            sys.exit(1)
+
+        file_path = sys.argv[2]
+        try:
+            ctd = CTDFjorder.CTD(file_path)
+            ctd.add_filename_to_table()
+            ctd.save_to_csv("output.csv")
+            ctd.add_location_to_table()
+            ctd.remove_non_positive_samples()
+            ctd.run_complex_cleaner("practicalsalinity", 'salinitydiff')
+            ctd.add_absolute_salinity()
+            ctd.add_density()
+            ctd.add_overturns()
+            ctd.add_mld(0)
+            ctd.add_mld(10)
+            ctd.save_to_csv("outputclean.csv")
+            print("Processing completed successfully.")
+        except Exception as e:
+            print(f"Error processing file: {file_path}")
+            print(traceback.format_exc())
+            print(e)
+
+    elif command == "merge":
+        CTDFjorder.merge_all_in_folder()
+        print("Merging completed successfully.")
+
+    elif command == "default":
+        CTDFjorder.run_default()
+        print("Default processing completed successfully.")
+
+    else:
+        print(f"Unknown command: {command}")
+        print("Usage: ctdfjorder <command> [arguments]")
+        print("Commands:")
+        print("  process <file>          Process a single RSK file")
+        print("  merge                   Merge all RSK files in the current folder")
+        print("  default                 Run the default processing pipeline")
+        print("CWD:")
+        print(CTDFjorder.CTD.get_cwd())
         sys.exit(1)
-    data = CTDFjorder.CTD("208040_20211217_1628.rsk")
-    data.add_density()
-    data.add_location_to_table()
-    data.run_complex_cleaner('salinity', 'salinitydiff')
-    data.add_absolute_salinity()
-    data.add_overturns()
-    data.add_mld('default')
-    data.plot_depth_salinity_density_mld_line()
-    CTDFjorder
+
+if __name__ == "__main__":
+    main()
+
```

### Comparing `ctdfjorder-0.0.6/LICENSE` & `CTDFjorder-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.6/PKG-INFO` & `CTDFjorder-0.0.8/CTDFjorder.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.6
+Version: 0.0.8
 Summary: A package for processing and analyzing CTD data.
+Home-page: https://github.com/nikothomas/CTDFjorder
+Author: Nikolas Yanek-Chrones
+Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
-Author-email: Nikolas Yanek-Chrones <nikojb1001@gmail.com>
-License-File: LICENSE
 Keywords: CTD
 Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
-Requires-Dist: gsw>=3.6.17
-Requires-Dist: matplotlib>=3.8.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.1
-Requires-Dist: pyrsktools>=0.1.9
-Requires-Dist: scipy>=1.11.4
+Requires-Dist: gsw>=3.6.17
+Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: statsmodels>=0.14.0
 Requires-Dist: tabulate>=0.9.0
-Description-Content-Type: text/markdown
+Requires-Dist: pyrsktools>=0.1.9
+Requires-Dist: openpyxl>=3.1.2
 
 # CTDFjorder
 
-Package for processing CTD files.
+Package for processing CTD files.
```

