# Comparing `tmp/rHDPE_Data_Analysis-1.0.4.tar.gz` & `tmp/rHDPE_Data_Analysis-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rHDPE_Data_Analysis-1.0.4.tar", last modified: Thu Apr 25 12:37:32 2024, max compression
+gzip compressed data, was "rHDPE_Data_Analysis-1.0.5.tar", last modified: Wed May  1 17:01:21 2024, max compression
```

## Comparing `rHDPE_Data_Analysis-1.0.4.tar` & `rHDPE_Data_Analysis-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-25 12:37:32.398474 rHDPE_Data_Analysis-1.0.4/
--rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-04-25 12:37:32.397688 rHDPE_Data_Analysis-1.0.4/PKG-INFO
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-25 12:37:32.376143 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-25 12:37:32.390105 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/
--rw-r--r--   0 philsmith   (501) staff       (20)     2704 2024-02-20 12:55:58.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
--rw-r--r--   0 philsmith   (501) staff       (20)     8041 2024-04-25 11:29:42.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
--rw-r--r--   0 philsmith   (501) staff       (20)     1878 2023-12-22 10:54:22.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
--rw-r--r--   0 philsmith   (501) staff       (20)     9887 2024-04-25 11:29:42.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
--rw-r--r--   0 philsmith   (501) staff       (20)    43762 2024-04-25 12:36:53.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)      148 2023-12-22 10:54:51.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-25 12:37:32.395686 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Analysis/
--rw-r--r--   0 philsmith   (501) staff       (20)     2077 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Analysis/Analysis.py
--rw-r--r--   0 philsmith   (501) staff       (20)     1446 2024-01-09 12:15:24.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py
--rw-r--r--   0 philsmith   (501) staff       (20)     3503 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py
--rw-r--r--   0 philsmith   (501) staff       (20)    37968 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Analysis/Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)      120 2024-01-03 12:56:03.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Analysis/__init__.py
--rw-r--r--   0 philsmith   (501) staff       (20)    35883 2024-04-19 16:24:08.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-25 11:22:18.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/__init__.py
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-25 12:37:32.396813 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis.egg-info/
--rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-04-25 12:37:32.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis.egg-info/PKG-INFO
--rw-r--r--   0 philsmith   (501) staff       (20)      813 2024-04-25 12:37:32.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis.egg-info/SOURCES.txt
--rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-25 12:37:32.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis.egg-info/dependency_links.txt
--rw-r--r--   0 philsmith   (501) staff       (20)       20 2024-04-25 12:37:32.000000 rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis.egg-info/top_level.txt
--rw-r--r--   0 philsmith   (501) staff       (20)       38 2024-04-25 12:37:32.398692 rHDPE_Data_Analysis-1.0.4/setup.cfg
--rw-r--r--   0 philsmith   (501) staff       (20)      416 2024-04-25 12:37:27.000000 rHDPE_Data_Analysis-1.0.4/setup.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-01 17:01:21.096659 rHDPE_Data_Analysis-1.0.5/
+-rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-05-01 17:01:21.095802 rHDPE_Data_Analysis-1.0.5/PKG-INFO
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-01 17:01:21.070368 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-01 17:01:21.088947 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/
+-rw-r--r--   0 philsmith   (501) staff       (20)     2698 2024-05-01 14:22:52.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    16419 2023-08-07 12:36:28.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/Deprecated.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     7846 2024-05-01 14:20:16.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     2142 2024-04-25 15:57:34.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     9607 2024-04-29 13:43:44.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    43760 2024-05-01 16:22:46.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)      148 2023-12-22 10:54:51.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-01 17:01:21.094679 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Analysis/
+-rw-r--r--   0 philsmith   (501) staff       (20)     2077 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Analysis/Analysis.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     1446 2024-01-09 12:15:24.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     3503 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    37968 2024-04-25 11:31:49.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Analysis/Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)      120 2024-01-03 12:56:03.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Analysis/__init__.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    35883 2024-04-19 16:24:08.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-25 11:22:18.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/__init__.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-05-01 17:01:21.078993 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis.egg-info/
+-rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-05-01 17:01:20.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis.egg-info/PKG-INFO
+-rw-r--r--   0 philsmith   (501) staff       (20)      861 2024-05-01 17:01:20.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-05-01 17:01:20.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)       20 2024-05-01 17:01:20.000000 rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis.egg-info/top_level.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)       38 2024-05-01 17:01:21.096835 rHDPE_Data_Analysis-1.0.5/setup.cfg
+-rw-r--r--   0 philsmith   (501) staff       (20)      416 2024-05-01 16:30:08.000000 rHDPE_Data_Analysis-1.0.5/setup.py
```

### Comparing `rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py` & `rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,33 +4,30 @@
 from . import Utilities as util
 from . import FTIR_plotting
 import numpy as np
 from scipy.signal import savgol_filter
 
 # Main function definition.
 
-def FTIR_Analysis_Main( directory, ip ):
+def FTIR_Analysis_Main( ip ):
     '''Main function for FTIR data.'''
 
-    input_directory = directory + "FTIR/"
-    output_directory = directory + "FTIR/Output/"
-
     file_data, data, m_peaks, y_peaks, mag_m_peaks, mag_y_peaks, m_peaks_array, y_peaks_array, first_derivative_data, second_derivative_data, third_derivative_data = [], [], [], [], [], [], [], [], [], [], []
 
     if ip.read_files:
 
-        file_data, data = Preprocessing.read_files_and_preprocess( directory, ip.merge_groups )
+        file_data, data = Preprocessing.read_files_and_preprocess( ip.directory, ip.data_directory, ip.merge_groups )
 
     if ip.write_csv:
 
-        Preprocessing.write_csv( input_directory, file_data, data )
+        Preprocessing.write_csv( ip.output_directory, file_data, data )
 
     if ip.read_csv:
 
-        file_data, data = Preprocessing.read_csv( directory, ip.merge_groups )
+        file_data, data = Preprocessing.read_csv( ip.directory, ip.output_directory, ip.merge_groups )
 
     # Data of form [x, [y]]. data[0], data[1][i] all have length 1762.
 
     print( str( len( file_data ) ) + " files have been read." )
 
     if len( file_data ) != 333:
 
@@ -52,36 +49,36 @@
 
                 array = savgol_filter( array, 7, 3 )
 
                 data[1][i] = array.tolist()
 
     if ip.compute_mean:
 
-        Preprocessing.compute_mean( input_directory, file_data, data )
+        Preprocessing.compute_mean( ip.output_directory, file_data, data )
 
     if ip.read_mean:
 
-        Preprocessing.read_mean( input_directory, data )
+        Preprocessing.read_mean( ip.output_directory, data )
 
     # Data now of form [x, [y], [m]].
 
     if ip.derivative:
 
         first_derivative_data = util.compute_derivatives( data )
         second_derivative_data = util.compute_derivatives( first_derivative_data )
         third_derivative_data = util.compute_derivatives( second_derivative_data )
 
     if ip.extract_features:
 
-        m_peaks, m_peaks_array, y_peaks, y_peaks_array = util.extract_FTIR_features( output_directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data, ip.peak_threshold_1, ip.peak_threshold_2, ip.peak_spacing, ip.peak_limit )
+        m_peaks, m_peaks_array, y_peaks, y_peaks_array = util.extract_FTIR_features( ip.output_directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data, ip.peak_threshold_1, ip.peak_threshold_2, ip.peak_spacing, ip.peak_limit )
 
     if ip.read_and_analyse_features:
 
-        util.read_and_analyse_FTIR_features( directory, ip, file_data )
+        util.read_and_analyse_FTIR_features( ip, file_data )
 
     if ip.plot_data:
 
-        FTIR_plotting.plot_data( directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data, m_peaks, m_peaks_array, y_peaks, y_peaks_array )
+        FTIR_plotting.plot_data( ip.directory, ip.output_directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data, m_peaks, m_peaks_array, y_peaks, y_peaks_array )
 
     if ip.sandbox:
 
-        util.sandbox( directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data )
+        util.sandbox( ip.directory, ip.output_directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data )
```

### Comparing `rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py` & `rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 # Imports.
 
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib as mpl
-import sys
-from pathlib import Path
-
-# sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
-#
-# from rHDPE_Data_Analysis import Global_Utilities as gu
 
 from .. import Global_Utilities as gu
 
 # Function definitions.
 
-def plot_data( directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data, m_peaks, m_peaks_array, y_peaks, y_peaks_array, savefig = False ):
+def plot_data( directory, output_directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data, m_peaks, m_peaks_array, y_peaks, y_peaks_array, savefig = False ):
 
     # for i in range( len( data[1] ) ):
     #
     #     # data[1][i] = (np.array( data[1][i] ) / np.array( data[1][i] ).max()).tolist()
     #     data[1][i] = ((np.array( data[1][i] ) - np.array( data[1][i] ).min()) / (np.array( data[1][i] ).max() - np.array( data[1][i] ).min())).tolist()
     #
     # for i in range( len( data[2] ) ):
     #
     #     # data[1][i] = (np.array( data[1][i] ) / np.array( data[1][i] ).max()).tolist()
     #     data[2][i] = ((np.array( data[2][i] ) - np.array( data[2][i] ).min()) / (np.array( data[2][i] ).max() - np.array( data[2][i] ).min())).tolist()
 
-    output_directory = directory + "FTIR/Output/"
-
     resin_data = gu.get_list_of_resins_data( directory )
 
     # For overall pipeline figure.
 
     mpl.rcParams['lines.linewidth'] = 3 #4
 
     sample, sample_array, samples_present, samples_present_array = gu.sample_data_from_file_data( file_data )
@@ -184,15 +176,15 @@
         # plt.xlabel( "" )
         # plt.ylabel( "" )
         # plt.tick_params( axis = 'x', which = 'both', bottom = False, top = False, labelbottom = False )
         # plt.tick_params( axis = 'y', which = 'both', left = False, right = False, labelleft = False )
 
         if savefig:
 
-            plt.savefig( output_directory + "Plots/Plot.pdf" )
+            plt.savefig( output_directory + "FTIR/Plots/Plot.pdf" )
 
         else:
 
             plt.show()
 
         plt.close()
 
@@ -200,8 +192,8 @@
 
             array = data_extraction[0][:, np.newaxis]
 
             for i in range( 1, len( data_extraction ) ):
 
                 array = np.hstack( (array, data_extraction[i][:, np.newaxis]) )
 
-            np.savetxt( directory + "Output/Plot_Coords/Unnamed.txt", array )
+            np.savetxt( output_directory + "Plot_Coords/Unnamed.txt", array )
```

### Comparing `rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py` & `rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 # Class definitions.
 
 class Input_Parameters():
 
     def __init__( self ):
 
+        self.directory = ""
+
+        self.data_directory = ""
+
+        self.output_directory = ""
+
         self.read_files = False
 
         self.merge_groups = False
 
         self.write_csv = False
 
         self.read_csv = False
@@ -50,42 +56,48 @@
 
     doc = Document( filename )
 
     sheets = doc.sheets
     tables = sheets[0].tables
     rows = tables[0].rows()
 
-    ip.read_files = bool( rows[0][1].value )
+    ip.directory = str( rows[0][1].value or "" )
+
+    ip.data_directory = str( rows[1][1].value or "" )
+
+    ip.output_directory = str( rows[2][1].value or "" )
+
+    ip.read_files = bool( rows[3][1].value )
 
-    ip.merge_groups = bool( rows[1][1].value )
+    ip.merge_groups = bool( rows[4][1].value )
 
-    ip.write_csv = bool( rows[2][1].value )
+    ip.write_csv = bool( rows[5][1].value )
 
-    ip.read_csv = bool( rows[3][1].value )
+    ip.read_csv = bool( rows[6][1].value )
 
-    ip.remove_files = bool( rows[4][1].value )
+    ip.remove_files = bool( rows[7][1].value )
 
-    ip.compute_mean = bool( rows[5][1].value )
+    ip.compute_mean = bool( rows[8][1].value )
 
-    ip.read_mean = bool( rows[6][1].value )
+    ip.read_mean = bool( rows[9][1].value )
 
-    ip.derivative = bool( rows[7][1].value )
+    ip.derivative = bool( rows[10][1].value )
 
-    ip.extract_features = bool( rows[8][1].value )
+    ip.extract_features = bool( rows[11][1].value )
 
-    ip.peak_threshold_1 = float( rows[9][1].value )
+    ip.peak_threshold_1 = float( rows[12][1].value )
 
-    ip.peak_threshold_2 = float( rows[10][1].value )
+    ip.peak_threshold_2 = float( rows[13][1].value )
 
-    ip.peak_spacing = float( rows[11][1].value )
+    ip.peak_spacing = float( rows[14][1].value )
 
-    ip.peak_limit = float( rows[12][1].value )
+    ip.peak_limit = float( rows[15][1].value )
 
-    ip.read_and_analyse_features = bool( rows[13][1].value )
+    ip.read_and_analyse_features = bool( rows[16][1].value )
 
-    ip.plot_data = bool( rows[14][1].value )
+    ip.plot_data = bool( rows[17][1].value )
 
-    ip.sandbox = bool( rows[15][1].value )
+    ip.sandbox = bool( rows[18][1].value )
 
-    ip.sample_mask = [int( i.value ) for i in rows[16][1:] if i.value != None]
+    ip.sample_mask = [int( i.value ) for i in rows[19][1:] if i.value != None]
 
-    ip.feature_selection = [int( i.value ) for i in rows[17][1:] if i.value != None]
+    ip.feature_selection = [int( i.value ) for i in rows[20][1:] if i.value != None]
```

### Comparing `rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py` & `rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # Imports.
 
 import os
 import glob
 import re
 import numpy as np
 import pandas as pd
-import sys
-from pathlib import Path
-
-# sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
-
-# from rHDPE_Data_Analysis import Global_Utilities as gu
 
 from .. import Global_Utilities as gu
 
 # Function definitions.
 
-def read_raw_data_file_1( filename, r, resin_data, file_data, data ):
-
-    pattern = re.compile( r"^Resin(\d+)" )
-
-    resin = int( pattern.search( r ).groups()[0] )
+def read_raw_data_file_1( filename, f, resin_data, file_data, data ):
 
     pattern = re.compile( r"^Resin(\d+)_(\d+)_" )
 
-    specimen = int( pattern.search( filename ).groups()[1] )
+    resin = int( pattern.search( f ).groups()[0] )
+
+    specimen = int( pattern.search( f ).groups()[1] )
 
     with open( filename, 'r' ) as file:
 
         x, y = [], []
 
         lines = file.readlines()
 
@@ -51,23 +43,21 @@
                 break
 
     data[0].append( np.array( x ) )
     data[1].append( np.array( y ) )
 
     file_data.append( [resin, specimen, resin_data.loc[resin]["Label"] + ".{}".format( specimen ), ""] )
 
-def read_raw_data_file_2( filename, r, resin_data, file_data, data ):
-
-    pattern = re.compile( r"^Resin(\d+)" )
-
-    resin = int( pattern.search( r ).groups()[0] )
+def read_raw_data_file_2( filename, f, resin_data, file_data, data ):
 
     pattern = re.compile( r"^Resin(\d+)_(\d+)_" )
 
-    specimen = int( pattern.search( filename ).groups()[1] )
+    resin = int( pattern.search( f ).groups()[0] )
+
+    specimen = int( pattern.search( f ).groups()[1] )
 
     with open( filename, 'r' ) as file:
 
         x, y = [], []
 
         lines = file.read().splitlines()
 
@@ -90,44 +80,40 @@
                 break
 
     data[0].append( np.array( x ) )
     data[1].append( np.array( y ) )
 
     file_data.append( [resin, specimen, resin_data.loc[resin]["Label"] + ".{}".format( specimen ), ""] )
 
-def extract_raw_data( directory ):
+def extract_raw_data( directory, data_directory ):
     '''Extract the raw data from the files.'''
 
     resin_data = gu.get_list_of_resins_data( directory ) # Obtain the spreadsheet of data for the resins.
 
-    os.chdir( directory + "FTIR/Raw_Data/" )
-
-    resins = sorted( glob.glob( "*" ), key = gu.sort_raw_files_1 )
+    resins = sorted( [os.path.basename( path ) for path in glob.glob( data_directory + "*" )], key = gu.sort_raw_files_1 )
 
     file_data, data = [], [[], []]
 
     pattern = re.compile( r"^Resin(\d+)" )
 
     for r in resins:
 
-        os.chdir( directory + "FTIR/Raw_Data/" + r )
-
-        filenames = sorted( glob.glob( "*" ), key = gu.sort_raw_files_2 )
+        filenames = sorted( [os.path.basename( path ) for path in glob.glob( data_directory + r + "/*" )], key = gu.sort_raw_files_2 )
 
         resin = int( pattern.search( r ).groups()[0] )
 
         for f in filenames:
 
             if resin >= 40 and resin <= 70:
 
-                read_raw_data_file_2( f, r, resin_data, file_data, data )
+                read_raw_data_file_2( data_directory + r + "/" + f, f, resin_data, file_data, data )
 
             else:
 
-                read_raw_data_file_1( f, r, resin_data, file_data, data )
+                read_raw_data_file_1( data_directory + r + "/" + f, f, resin_data, file_data, data )
 
     return file_data, data
 
 def normalise( y ):
     '''Normalise the data.'''
 
     for i in range( len( y ) ):
@@ -261,72 +247,63 @@
 
     for f in file_data:
 
         if f[0] >= 401 and f[0] <= 500:
 
             f[3] = f[3] + "u"
 
-def read_files_and_preprocess( directory, merge_groups ):
+def read_files_and_preprocess( directory, data_directory, merge_groups ):
     '''Read files and preprocess data.'''
 
-    file_data, data = extract_raw_data( directory )
+    file_data, data = extract_raw_data( directory, data_directory )
 
     standardise_data( data )
 
     add_description_to_file_data( file_data )
 
     if merge_groups:
 
         gu.merge( file_data )
 
     return file_data, data
 
-def write_csv( input_directory, file_data, data ):
+def write_csv( output_directory, file_data, data ):
     '''Write read and preprocessed data to a .csv file.'''
 
     array = data[0][:, np.newaxis]
 
     for i in range( len( data[1] ) ):
 
         array = np.hstack( (array, data[1][i][:, np.newaxis]) )
 
-    np.savetxt( input_directory + "Condensed_Data/FTIR_data.csv", array, delimiter = "," )
+    np.savetxt( output_directory + "FTIR/Condensed_Data/FTIR_data.csv", array, delimiter = "," )
 
-def read_csv( directory, merge_groups ):
-    '''Read the preprocessed .csv file.'''
+    array = np.array( file_data )
 
-    resin_data = gu.get_list_of_resins_data( directory ) # Obtain the spreadsheet of data for the resins.
+    np.savetxt( output_directory + "FTIR/Condensed_Data/file_data.csv", array, delimiter = ",", fmt = "%s" )
 
-    os.chdir( directory + "FTIR/Raw_Data/" )
+def read_csv( directory, output_directory, merge_groups ):
+    '''Read the preprocessed .csv file.'''
 
-    resins = sorted( glob.glob( "*" ), key = gu.sort_raw_files_1 )
+    resin_data = gu.get_list_of_resins_data( directory ) # Obtain the spreadsheet of data for the resins.
 
     file_data = []
 
-    for r in resins:
-
-        os.chdir( directory + "FTIR/Raw_Data/" + r )
-
-        filenames = sorted( glob.glob( "*" ), key = gu.sort_raw_files_2 )
-
-        for f in filenames:
-
-            pattern = re.compile( r"^Resin(\d+)" )
-
-            resin = int( pattern.search( r ).groups()[0] )
+    df = pd.read_csv( output_directory + "FTIR/Condensed_Data/file_data.csv", sep = ",", header = None )
 
-            pattern = re.compile( r"^Resin(\d+)_(\d+)_" )
+    for i in range( len( df.index ) ):
 
-            specimen = int( pattern.search( f ).groups()[1] )
+        resin = df.iloc[i, 0]
+        specimen = df.iloc[i, 1]
 
-            file_data.append( [resin, specimen, resin_data.loc[resin]["Label"] + ".{}".format( specimen ), ""] )
+        file_data.append( [resin, specimen, resin_data.loc[resin]["Label"] + ".{}".format( specimen ), ""] )
 
     data = []
 
-    df = pd.read_csv( directory + "FTIR/Condensed_Data/FTIR_data.csv", sep = ",", header = None )
+    df = pd.read_csv( output_directory + "FTIR/Condensed_Data/FTIR_data.csv", sep = ",", header = None )
 
     data.append( df.iloc[:, 0].tolist() )
 
     y = []
 
     for i in range( 1, len( df.columns ) ):
 
@@ -391,32 +368,32 @@
     files_to_remove.reverse()
 
     for r in files_to_remove:
 
         file_data.pop( r )
         data[1].pop( r )
 
-def compute_mean( input_directory, file_data, data ):
+def compute_mean( output_directory, file_data, data ):
     '''Compute the mean data for each resin.'''
 
     m = gu.sample_mean( file_data, data[1] )
 
     array = m[0][:, np.newaxis]
 
     for i in range( 1, len( m ) ):
 
         array = np.hstack( (array, m[i][:, np.newaxis]) )
 
-    np.savetxt( input_directory + "Condensed_Data/Means.csv", array, delimiter = "," )
+    np.savetxt( output_directory + "FTIR/Condensed_Data/Means.csv", array, delimiter = "," )
 
-def read_mean( input_directory, data ):
+def read_mean( output_directory, data ):
     '''Read the computed means for each resin from a file.'''
 
     m = []
 
-    df = pd.read_csv( input_directory + "Condensed_Data/Means.csv", sep = ",", header = None )
+    df = pd.read_csv( output_directory + "FTIR/Condensed_Data/Means.csv", sep = ",", header = None )
 
     for i in range( len( df.columns ) ):
 
         m.append( df.iloc[:, i].tolist() )
 
     data.append( m )
```

### Comparing `rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py` & `rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Imports.
 
 import numpy as np
 import pandas as pd
 from scipy.stats import pearsonr
-import sys
-from pathlib import Path
-
-# sys.path.append( Path( __file__ ).absolute().parents[3].as_posix() )
+from sklearn.preprocessing import StandardScaler
 
+from . import Preprocessing
+from ..Global_Analysis import Utilities as util2
 from .. import Global_Utilities as gu
 
 # Function definitions.
 
 def compute_derivatives( data, width = 1 ):
     '''Compute the derivatives.'''
 
@@ -277,15 +276,15 @@
         m_peaks, m_peaks_array = remove_identical_columns( m_peaks_array, m_peaks )
         m_peaks_array = remove_wavenumbers( m_peaks, m_peaks_array )
 
         feature_names = ["FTIR_{}".format( int( i ) ) for i in m_peaks]
 
         df = gu.array_with_column_titles_to_df( m_peaks_array, feature_names )
 
-        df.to_csv( output_directory + "Features/Features.csv" )
+        df.to_csv( output_directory + "FTIR/Features/Features.csv" )
 
     if y_peak_analysis:
 
         peaks_specified_by_m_peak_analysis = True
 
         linear_filter( mag_y_peaks, peak_threshold_2, peak_threshold_1 )
 
@@ -314,36 +313,34 @@
             y_peaks, y_peaks_array = remove_identical_columns( y_peaks_array, y_peaks )
             y_peaks_array = remove_wavenumbers( y_peaks, y_peaks_array )
 
         feature_names = ["FTIR_{}".format( int( i ) ) for i in y_peaks]
 
         df = gu.array_with_column_titles_to_df( y_peaks_array, feature_names )
 
-        df.to_csv( output_directory + "Features/Specimen_Features.csv" )
+        df.to_csv( output_directory + "FTIR/Features/Specimen_Features.csv" )
 
     return m_peaks, m_peaks_array, y_peaks, y_peaks_array
 
-def read_and_analyse_FTIR_features( directory, ip, file_data ):
+def read_and_analyse_FTIR_features( ip, file_data ):
 
     precomputed_means = False
 
     plot_specimen_bars = False
     plot_mean_bars = False
     plot_specimen_features = True
     plot_mean_features = True
     plot_specimen_distance_matrix = True
     plot_mean_distance_matrix = True
     plot_specimen_dendrogram = True
     plot_mean_dendrogram = True
 
-    output_directory = directory + "FTIR/Output/"
+    resin_data = gu.get_list_of_resins_data( ip.directory )
 
-    resin_data = gu.get_list_of_resins_data( directory )
-
-    feature_names, features = gu.csv_to_df_to_array_and_column_titles( output_directory + "Features/Specimen_Features.csv" )
+    feature_names, features = gu.csv_to_df_to_array_and_column_titles( ip.output_directory + "FTIR/Features/Specimen_Features.csv" )
 
     sample, sample_array, samples_present, samples_present_array = gu.sample_data_from_file_data( file_data )
 
     if not ip.sample_mask:
 
         ip.sample_mask = [11, 14, 10, 4, 13, 21, 23, 18, 22, 20, 2, 3, 17, 16, 19, 1, 15, 12, 6, 5, 7, 9, 8, 24]
         # ip.sample_mask = [301, 303, 306, 308, 309, 312, 313, 315, 318, 320, 324, 325]
@@ -381,65 +378,65 @@
 
     mean_distance_matrix = gu.distance_matrix_from_features( mean_features )
 
     mean_features_plus_sample_mask = np.hstack( (np.array( sample_mask )[:, np.newaxis], mean_features) )
 
     df = gu.array_with_column_titles_to_df( mean_features_plus_sample_mask, ["sample"] + mean_feature_names )
 
-    df.to_csv( output_directory + "Features/Mean_Features.csv" )
+    df.to_csv( ip.output_directory + "FTIR/Features/Mean_Features.csv" )
 
     std_of_features_plus_sample_mask = np.hstack( (np.array( sample_mask )[:, np.newaxis], std_of_features) )
 
     df = gu.array_with_column_titles_to_df( std_of_features_plus_sample_mask, ["sample"] + mean_feature_names )
 
-    df.to_csv( output_directory + "Features/Std_of_Features.csv" )
+    df.to_csv( ip.output_directory + "FTIR/Features/Std_of_Features.csv" )
 
     df = gu.array_with_column_titles_and_label_titles_to_df( mean_distance_matrix, sample_mask, sample_mask )
 
-    df.to_csv( output_directory + "Features/Distance_Matrix.csv" )
+    df.to_csv( ip.output_directory + "FTIR/Features/Distance_Matrix.csv" )
 
     if plot_specimen_bars:
 
         for i in range( len( features[0] ) ):
 
-            gu.plot_barchart_of_feature( features[:, i], [f[2] for f in file_data_mask], colour = True, colour_mask = sample_array, filename = output_directory + "Feature_Bars/Specimen/" + feature_names[i] + ".pdf", savefig = True )
+            gu.plot_barchart_of_feature( features[:, i], [f[2] for f in file_data_mask], colour = True, colour_mask = sample_array, filename = ip.output_directory + "FTIR/Feature_Bars/Specimen/" + feature_names[i] + ".pdf", savefig = True )
 
     if plot_mean_bars:
 
         for i in range( len( mean_features[0] ) ):
 
-            gu.plot_barchart_of_feature( mean_features[:, i], [resin_data.loc[i]["Label"] for i in sample_mask], errorbars = True, std = std_of_features[:, i], colour = True, colour_mask = sample_mask, filename = output_directory + "Feature_Bars/Mean/" + mean_feature_names[i] + ".pdf", savefig = True )
+            gu.plot_barchart_of_feature( mean_features[:, i], [resin_data.loc[i]["Label"] for i in sample_mask], errorbars = True, std = std_of_features[:, i], colour = True, colour_mask = sample_mask, filename = ip.output_directory + "FTIR/Feature_Bars/Mean/" + mean_feature_names[i] + ".pdf", savefig = True )
 
     if plot_specimen_features:
 
-        gu.plot_features( output_directory, features, [f[5:] for f in feature_names], [f[2] for f in file_data_mask], specimen = True, subdirectory = "Features/", title = "Specimen_Features.pdf" )
+        gu.plot_features( ip.output_directory, features, [f[5:] for f in feature_names], [f[2] for f in file_data_mask], specimen = True, subdirectory = "FTIR/Features/", title = "Specimen_Features.pdf" )
 
     if plot_mean_features:
 
-        gu.plot_features( output_directory, mean_features, [f[5:] for f in mean_feature_names], [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "Features/", title = "Means_Features.pdf" )
+        gu.plot_features( ip.output_directory, mean_features, [f[5:] for f in mean_feature_names], [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "FTIR/Features/", title = "Means_Features.pdf" )
 
     if plot_specimen_distance_matrix:
 
-        gu.plot_distance_matrix( output_directory, distance_matrix, [f[2] for f in file_data_mask], specimen = True, file_data = file_data_mask, sample_mask = sample_mask, subdirectory = "Features/", title = "Specimen_Distance_Matrix.pdf" )
+        gu.plot_distance_matrix( ip.output_directory, distance_matrix, [f[2] for f in file_data_mask], specimen = True, file_data = file_data_mask, sample_mask = sample_mask, subdirectory = "FTIR/Features/", title = "Specimen_Distance_Matrix.pdf" )
 
     if plot_mean_distance_matrix:
 
-        gu.plot_distance_matrix( output_directory, mean_distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "Features/", title = "Means_Distance_Matrix.pdf" )
+        gu.plot_distance_matrix( ip.output_directory, mean_distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "FTIR/Features/", title = "Means_Distance_Matrix.pdf" )
 
     if plot_specimen_dendrogram:
 
-        gu.plot_dendrogram( output_directory, distance_matrix, [f[2] for f in file_data_mask], specimen = True, subdirectory = "Features/", title = "Specimen_Dendrogram.pdf" )
+        gu.plot_dendrogram( ip.output_directory, distance_matrix, [f[2] for f in file_data_mask], specimen = True, subdirectory = "FTIR/Features/", title = "Specimen_Dendrogram.pdf" )
 
     if plot_mean_dendrogram:
 
-        gu.plot_dendrogram( output_directory, mean_distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "Features/", title = "Means_Dendrogram.pdf" )
+        gu.plot_dendrogram( ip.output_directory, mean_distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "FTIR/Features/", title = "Means_Dendrogram.pdf" )
 
     if precomputed_means:
 
-        feature_names, features = gu.csv_to_df_to_array_and_column_titles( output_directory + "Features/Features.csv" )
+        feature_names, features = gu.csv_to_df_to_array_and_column_titles( ip.output_directory + "FTIR/Features/Features.csv" )
 
         feature_selection = [i for i in range( len( feature_names ) )]
 
         features = features[:, feature_selection]
         feature_names = list( np.array( feature_names )[feature_selection] )
 
         samples_present_mask = gu.produce_mask( samples_present_array, sample_mask )
@@ -452,48 +449,46 @@
 
         distance_matrix = gu.distance_matrix_from_features( features )
 
         mean_features_plus_sample_mask = np.hstack( (np.array( sample_mask )[:, np.newaxis], features) )
 
         df = gu.array_with_column_titles_to_df( mean_features_plus_sample_mask, ["sample"] + feature_names )
 
-        df.to_csv( output_directory + "Features/Mean_Features.csv" )
+        df.to_csv( ip.output_directory + "FTIR/Features/Mean_Features.csv" )
 
         df = gu.array_with_column_titles_and_label_titles_to_df( distance_matrix, sample_mask, sample_mask )
 
-        df.to_csv( output_directory + "Features/Distance_Matrix.csv" )
+        df.to_csv( ip.output_directory + "FTIR/Features/Distance_Matrix.csv" )
 
         if plot_mean_bars:
 
             for i in range( len( features[0] ) ):
 
-                gu.plot_barchart_of_feature( features[:, i], [resin_data.loc[i]["Label"] for i in sample_mask], colour = True, colour_mask = sample_mask, filename = output_directory + "Feature_Bars/Mean/" + feature_names[i] + ".pdf", savefig = True )
+                gu.plot_barchart_of_feature( features[:, i], [resin_data.loc[i]["Label"] for i in sample_mask], colour = True, colour_mask = sample_mask, filename = ip.output_directory + "FTIR/Feature_Bars/Mean/" + feature_names[i] + ".pdf", savefig = True )
 
         if plot_mean_features:
 
-            gu.plot_features( output_directory, features, [f[5:] for f in feature_names], [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "Features/", title = "Means_Features.pdf" )
+            gu.plot_features( ip.output_directory, features, [f[5:] for f in feature_names], [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "FTIR/Features/", title = "Means_Features.pdf" )
 
         if plot_mean_distance_matrix:
 
-            gu.plot_distance_matrix( output_directory, distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "Features/", title = "Means_Distance_Matrix.pdf" )
+            gu.plot_distance_matrix( ip.output_directory, distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "FTIR/Features/", title = "Means_Distance_Matrix.pdf" )
 
         if plot_mean_dendrogram:
 
-            gu.plot_dendrogram( output_directory, distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "Features/", title = "Means_Dendrogram.pdf" )
+            gu.plot_dendrogram( ip.output_directory, distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "FTIR/Features/", title = "Means_Dendrogram.pdf" )
 
-def integral_analysis( directory, file_data, data ):
+def integral_analysis( directory, output_directory, file_data, data ):
     '''Perform an analysis on the data that focuses on integrals.'''
 
     plot_specimen_distance_matrix = True
     plot_mean_distance_matrix = True
     plot_specimen_dendrogram = True
     plot_mean_dendrogram = True
 
-    output_directory = directory + "FTIR/Output/"
-
     resin_data = gu.get_list_of_resins_data( directory )
 
     sample, sample_array, samples_present, samples_present_array = gu.sample_data_from_file_data( file_data )
 
     sample_mask = [11, 14, 10, 4, 13, 21, 23, 18, 22, 20, 2, 3, 17, 16, 19, 1, 15, 12, 6, 5, 7, 9, 8]
 
     sample_mask = gu.remove_redundant_samples( sample_mask, samples_present )
@@ -552,51 +547,49 @@
 
     mean_distance_matrix = gu.distance_matrix_from_features( mean_features )
 
     mean_features_plus_sample_mask = np.hstack( (np.array( sample_mask )[:, np.newaxis], mean_features) )
 
     df = gu.array_with_column_titles_to_df( mean_features_plus_sample_mask, ["sample"] + mean_feature_names )
 
-    df.to_csv( output_directory + "Integral_Analysis/Mean_Features.csv" )
+    df.to_csv( output_directory + "FTIR/Integral_Analysis/Mean_Features.csv" )
 
     std_of_features_plus_sample_mask = np.hstack( (np.array( sample_mask )[:, np.newaxis], std_of_features) )
 
     df = gu.array_with_column_titles_to_df( std_of_features_plus_sample_mask, ["sample"] + mean_feature_names )
 
-    df.to_csv( output_directory + "Integral_Analysis/Std_of_Features.csv" )
+    df.to_csv( output_directory + "FTIR/Integral_Analysis/Std_of_Features.csv" )
 
     df = gu.array_with_column_titles_and_label_titles_to_df( mean_distance_matrix, sample_mask, sample_mask )
 
-    df.to_csv( output_directory + "Integral_Analysis/Distance_Matrix.csv" )
+    df.to_csv( output_directory + "FTIR/Integral_Analysis/Distance_Matrix.csv" )
 
     if plot_specimen_distance_matrix:
 
-        gu.plot_distance_matrix( output_directory, distance_matrix, [f[2] for f in file_data_mask], specimen = True, file_data = file_data_mask, sample_mask = sample_mask, subdirectory = "Integral_Analysis/", title = "Specimen_Distance_Matrix.pdf" )
+        gu.plot_distance_matrix( output_directory, distance_matrix, [f[2] for f in file_data_mask], specimen = True, file_data = file_data_mask, sample_mask = sample_mask, subdirectory = "FTIR/Integral_Analysis/", title = "Specimen_Distance_Matrix.pdf" )
 
     if plot_mean_distance_matrix:
 
-        gu.plot_distance_matrix( output_directory, mean_distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "Integral_Analysis/", title = "Means_Distance_Matrix.pdf" )
+        gu.plot_distance_matrix( output_directory, mean_distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "FTIR/Integral_Analysis/", title = "Means_Distance_Matrix.pdf" )
 
     if plot_specimen_dendrogram:
 
-        gu.plot_dendrogram( output_directory, distance_matrix, [f[2] for f in file_data_mask], specimen = True, subdirectory = "Integral_Analysis/", title = "Specimen_Dendrogram.pdf" )
+        gu.plot_dendrogram( output_directory, distance_matrix, [f[2] for f in file_data_mask], specimen = True, subdirectory = "FTIR/Integral_Analysis/", title = "Specimen_Dendrogram.pdf" )
 
     if plot_mean_dendrogram:
 
-        gu.plot_dendrogram( output_directory, mean_distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "Integral_Analysis/", title = "Means_Dendrogram.pdf" )
+        gu.plot_dendrogram( output_directory, mean_distance_matrix, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "FTIR/Integral_Analysis/", title = "Means_Dendrogram.pdf" )
 
-def component_analysis( directory, file_data, data ):
+def component_analysis( directory, output_directory, file_data, data ):
 
     plot_specimen_bars = False
     plot_mean_bars = False
     plot_specimen_features = True
     plot_mean_features = True
 
-    output_directory = directory + "FTIR/Output/"
-
     resin_data = gu.get_list_of_resins_data( directory )
 
     sample, sample_array, samples_present, samples_present_array = gu.sample_data_from_file_data( file_data )
 
     # sample_mask = [11, 14, 10, 4, 13, 21, 23, 18, 22, 20, 2, 3, 17, 16, 19, 1, 15, 12, 6, 5, 7, 9, 8]
     sample_mask = [11, 14, 10, 4, 13, 21, 23, 18, 22, 20, 2, 3, 17, 16, 19, 1, 15, 12, 6, 5, 7, 9, 8, 401, 402, 403, 404, 405, 406, 407, 408, 409, 410, 411, 412, 413, 414, 415, 416]
 
@@ -850,47 +843,45 @@
 
     std_of_features = gu.extract_std_of_features( mean_integral, sample_array, sample_mask )
 
     mean_features_plus_sample_mask = np.hstack( (np.array( sample_mask )[:, np.newaxis], mean_features) )
 
     df = gu.array_with_column_titles_to_df( mean_features_plus_sample_mask, ["sample"] + mean_feature_names )
 
-    df.to_csv( output_directory + "Component_Analysis/Features/Mean_Features.csv" )
+    df.to_csv( output_directory + "FTIR/Component_Analysis/Features/Mean_Features.csv" )
 
     std_of_features_plus_sample_mask = np.hstack( (np.array( sample_mask )[:, np.newaxis], std_of_features) )
 
     df = gu.array_with_column_titles_to_df( std_of_features_plus_sample_mask, ["sample"] + mean_feature_names )
 
-    df.to_csv( output_directory + "Component_Analysis/Features/Std_of_Features.csv" )
+    df.to_csv( output_directory + "FTIR/Component_Analysis/Features/Std_of_Features.csv" )
 
     if plot_specimen_bars:
 
         for i in range( len( mean_integral[0] ) ):
 
-            gu.plot_barchart_of_feature( mean_integral[:, i], [f[2] for f in file_data_mask], colour = True, colour_mask = sample_array, filename = output_directory + "Component_Analysis/Feature_Bars/Specimen/" + feature_names[i] + ".pdf", savefig = True )
+            gu.plot_barchart_of_feature( mean_integral[:, i], [f[2] for f in file_data_mask], colour = True, colour_mask = sample_array, filename = output_directory + "FTIR/Component_Analysis/Feature_Bars/Specimen/" + feature_names[i] + ".pdf", savefig = True )
 
     if plot_mean_bars:
 
         for i in range( len( mean_features[0] ) ):
 
-            gu.plot_barchart_of_feature( mean_features[:, i], [resin_data.loc[i]["Label"] for i in sample_mask], errorbars = True, std = std_of_features[:, i], colour = True, colour_mask = sample_mask, filename = output_directory + "Component_Analysis/Feature_Bars/Mean/" + mean_feature_names[i] + ".pdf", savefig = True )
+            gu.plot_barchart_of_feature( mean_features[:, i], [resin_data.loc[i]["Label"] for i in sample_mask], errorbars = True, std = std_of_features[:, i], colour = True, colour_mask = sample_mask, filename = output_directory + "FTIR/Component_Analysis/Feature_Bars/Mean/" + mean_feature_names[i] + ".pdf", savefig = True )
 
     if plot_specimen_features:
 
-        gu.plot_features( output_directory, mean_integral, feature_names, [f[2] for f in file_data_mask], specimen = True, subdirectory = "Component_Analysis/Features/", title = "Specimen_Features.pdf" )
+        gu.plot_features( output_directory, mean_integral, feature_names, [f[2] for f in file_data_mask], specimen = True, subdirectory = "FTIR/Component_Analysis/Features/", title = "Specimen_Features.pdf" )
 
     if plot_mean_features:
 
-        gu.plot_features( output_directory, mean_features, mean_feature_names, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "Component_Analysis/Features/", title = "Means_Features.pdf" )
-
-def specimen_feature_correlation( directory, file_data ):
+        gu.plot_features( output_directory, mean_features, mean_feature_names, [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "FTIR/Component_Analysis/Features/", title = "Means_Features.pdf" )
 
-    output_directory = directory + "FTIR/Output/"
+def specimen_feature_correlation( directory, output_directory, file_data ):
 
-    df = pd.read_csv( output_directory + "Features/Specimen_Features.csv" )
+    df = pd.read_csv( output_directory + "FTIR/Features/Specimen_Features.csv" )
 
     df.drop( columns = df.columns[0], inplace = True )
 
     # feature_1 = "FTIR_667"
     # feature_2 = "FTIR_2349"
     #
     # pearson, _ = pearsonr( df[feature_1].to_list(), df[feature_2].to_list() )
@@ -925,20 +916,20 @@
 
         if abs( pearson ) > 0.75:
 
             print( pearson, feature_1, feature_2 )
 
             gu.plot_scatterplot_of_two_specimen_features_with_hover_annotation( df[feature_1].to_list(), df[feature_2].to_list(), file_data )
 
-def correlation_with_external_data( directory, file_data, data ):
+def correlation_with_external_data( directory, output_directory, file_data, data ):
     '''Find correlations with external data.'''
 
     resin_data = gu.get_list_of_resins_data( directory )
 
-    external_data = pd.read_csv( directory + "DSC/Output/Features/Mean_Features.csv" )
+    external_data = pd.read_csv( output_directory + "DSC/Output/Features/Mean_Features.csv" )
 
     external_data.drop( columns = [external_data.columns[0]], inplace = True )
 
     samples_present_external_data = external_data.iloc[:, 0].tolist()
 
     sample, sample_array, samples_present, samples_present_array = gu.sample_data_from_file_data( file_data )
 
@@ -993,42 +984,35 @@
 
         wavenumber_values.append( data[2][j][index_pearson] )
 
     wavenumber_values_array = np.array( wavenumber_values )
 
     gu.plot_scatterplot_of_two_features( feature, wavenumber_values_array, sample_mask, [resin_data.loc[i]["Label"] for i in sample_mask] )
 
-from . import Preprocessing
-# from rHDPE_Data_Analysis.Global.Global_Analysis import Utilities as util2
-from ..Global_Analysis import Utilities as util2
-from sklearn.preprocessing import StandardScaler
-
-def normalisation_experimentation( directory, file_data, data ):
+def normalisation_experimentation( directory, output_directory, file_data, data ):
     '''Experimenting to find best preprocessing for PCA.'''
 
     for i in range( len( data[1] ) ):
 
         # data[1][i] = (np.array( data[1][i] ) / np.array( data[1][i] ).max()).tolist()
         data[1][i] = ((np.array( data[1][i] ) - np.array( data[1][i] ).min()) / (np.array( data[1][i] ).max() - np.array( data[1][i] ).min())).tolist()
 
-    Preprocessing.compute_mean( directory + "FTIR/", file_data, data )
+    Preprocessing.compute_mean( output_directory, file_data, data )
 
-    Preprocessing.read_mean( directory + "FTIR/", data )
+    Preprocessing.read_mean( output_directory, data )
 
     first_derivative_data = compute_derivatives( data )
     second_derivative_data = compute_derivatives( first_derivative_data )
     third_derivative_data = compute_derivatives( second_derivative_data )
 
-    m_peaks, m_peaks_array, y_peaks, y_peaks_array = extract_FTIR_features( directory + "FTIR/Output/", file_data, data, first_derivative_data, second_derivative_data, third_derivative_data, -0.00008, 0.0002, 6, 3400 )
-
-    output_directory = directory + "FTIR/Output/"
+    m_peaks, m_peaks_array, y_peaks, y_peaks_array = extract_FTIR_features( output_directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data, -0.00008, 0.0002, 6, 3400 )
 
     resin_data = gu.get_list_of_resins_data( directory )
 
-    feature_names, features = gu.csv_to_df_to_array_and_column_titles( output_directory + "Features/Specimen_Features.csv" )
+    feature_names, features = gu.csv_to_df_to_array_and_column_titles( output_directory + "FTIR/Features/Specimen_Features.csv" )
 
     ###
 
     features = np.array( first_derivative_data[1] )
     feature_names = [str( i ) for i in first_derivative_data[0]]
 
     ###
@@ -1064,27 +1048,27 @@
 
     mean_distance_matrix = gu.distance_matrix_from_features( mean_features )
 
     mean_features_plus_sample_mask = np.hstack( (np.array( sample_mask )[:, np.newaxis], mean_features) )
 
     df = gu.array_with_column_titles_to_df( mean_features_plus_sample_mask, ["sample"] + mean_feature_names )
 
-    df.to_csv( output_directory + "Features/Mean_Features.csv" )
+    df.to_csv( output_directory + "FTIR/Features/Mean_Features.csv" )
 
     std_of_features_plus_sample_mask = np.hstack( (np.array( sample_mask )[:, np.newaxis], std_of_features) )
 
     df = gu.array_with_column_titles_to_df( std_of_features_plus_sample_mask, ["sample"] + mean_feature_names )
 
-    df.to_csv( output_directory + "Features/Std_of_Features.csv" )
+    df.to_csv( output_directory + "FTIR/Features/Std_of_Features.csv" )
 
     df = gu.array_with_column_titles_and_label_titles_to_df( mean_distance_matrix, sample_mask, sample_mask )
 
-    df.to_csv( output_directory + "Features/Distance_Matrix.csv" )
+    df.to_csv( output_directory + "FTIR/Features/Distance_Matrix.csv" )
 
-    # gu.plot_features( output_directory, mean_features, [f[5:] for f in mean_feature_names], [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "Features/", title = "Means_Features.pdf" )
+    # gu.plot_features( output_directory, mean_features, [f[5:] for f in mean_feature_names], [resin_data.loc[i]["Label"] for i in sample_mask], subdirectory = "FTIR/Features/", title = "Means_Features.pdf" )
 
     features_df = gu.array_with_column_titles_and_label_titles_to_df( mean_features, [str( i ) for i in mean_feature_names], sample_mask )
 
     # features_df = StandardScaler().fit_transform( features_df )
 
     features_df = gu.array_with_column_titles_and_label_titles_to_df( features_df, [str( i ) for i in mean_feature_names], sample_mask )
 
@@ -1103,38 +1087,38 @@
 
     # Max-min normalisation, all in:
     # [0.0, 0.519424198453715, 0.7109133621521699, 0.8403923836430574, 0.9029294068088906, 0.9354452996364587, 0.9563529416662541, 0.9693791609314283, 0.9812628941776536, 0.987887135278509, 0.9918010241419203]
 
     # Max-min normalisation, all in, first derivative:
     # [0.0, 0.43051277477178207, 0.8298189845995849, 0.9090705223769208, 0.9442834667082102, 0.959899984490423, 0.9692436649075102, 0.9761112933461358, 0.9817540207900024, 0.9857847801988655, 0.9894756652385638]
 
-def sandbox( directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data ):
+def sandbox( directory, output_directory, file_data, data, first_derivative_data, second_derivative_data, third_derivative_data ):
 
     perform_integral_analysis = False # Perform a second kind of analysis on the spectrums focusing on integrals.
 
     perform_component_analysis = True
 
     perform_specimen_feature_correlation = False
 
     perform_correlation_with_external_data = False # Try to find correlations between external data and FTIR data.
 
     perform_normalisation_experimentation = False
 
     if perform_integral_analysis:
 
-        integral_analysis( directory, file_data, data )
+        integral_analysis( directory, output_directory, file_data, data )
 
     if perform_component_analysis:
 
-        component_analysis( directory, file_data, data )
+        component_analysis( directory, output_directory, file_data, data )
 
     if perform_specimen_feature_correlation:
 
-        specimen_feature_correlation( directory, file_data )
+        specimen_feature_correlation( directory, output_directory, file_data )
 
     if perform_correlation_with_external_data:
 
-        correlation_with_external_data( directory, file_data, data )
+        correlation_with_external_data( directory, output_directory, file_data, data )
 
     if perform_normalisation_experimentation:
 
-        normalisation_experimentation( directory, file_data, data )
+        normalisation_experimentation( directory, output_directory, file_data, data )
```

### Comparing `rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Analysis/Analysis.py` & `rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Analysis/Analysis.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py` & `rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py` & `rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Analysis/Utilities.py` & `rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Analysis/Utilities.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis/Global_Utilities.py` & `rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis/Global_Utilities.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.4/rHDPE_Data_Analysis.egg-info/SOURCES.txt` & `rHDPE_Data_Analysis-1.0.5/rHDPE_Data_Analysis.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 rHDPE_Data_Analysis/Global_Utilities.py
 rHDPE_Data_Analysis/__init__.py
 rHDPE_Data_Analysis.egg-info/PKG-INFO
 rHDPE_Data_Analysis.egg-info/SOURCES.txt
 rHDPE_Data_Analysis.egg-info/dependency_links.txt
 rHDPE_Data_Analysis.egg-info/top_level.txt
 rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
+rHDPE_Data_Analysis/FTIR_Analysis/Deprecated.py
 rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
 rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
 rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
 rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
 rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
 rHDPE_Data_Analysis/Global_Analysis/Analysis.py
 rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py
```

