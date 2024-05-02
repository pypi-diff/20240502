# Comparing `tmp/toulligqc-2.5.7.tar.gz` & `tmp/toulligqc-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toulligqc-2.5.7.tar", last modified: Thu May  2 09:41:48 2024, max compression
+gzip compressed data, was "toulligqc-2.6.tar", last modified: Fri Jan 26 14:36:09 2024, max compression
```

## Comparing `toulligqc-2.5.7.tar` & `toulligqc-2.6.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 09:41:48.737793 toulligqc-2.5.7/
--rw-r--r--   0 root         (0) root         (0)      252 2024-05-02 09:41:25.000000 toulligqc-2.5.7/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    21146 2024-05-02 09:41:25.000000 toulligqc-2.5.7/LICENSE-CeCILL.txt
--rw-r--r--   0 root         (0) root         (0)    35466 2024-05-02 09:41:25.000000 toulligqc-2.5.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-02 09:41:25.000000 toulligqc-2.5.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      941 2024-05-02 09:41:48.737793 toulligqc-2.5.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14814 2024-05-02 09:41:42.000000 toulligqc-2.5.7/README.md
--rw-r--r--   0 root         (0) root         (0)      111 2024-05-02 09:41:48.737793 toulligqc-2.5.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1883 2024-05-02 09:41:42.000000 toulligqc-2.5.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 09:41:48.729793 toulligqc-2.5.7/test/
--rw-r--r--   0 root         (0) root         (0)    15570 2024-05-02 09:41:25.000000 toulligqc-2.5.7/test/test_sequencing_summary_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 09:41:48.733793 toulligqc-2.5.7/toulligqc/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13737 2024-05-02 09:41:42.000000 toulligqc-2.5.7/toulligqc/bam_extractor.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-02 09:41:42.000000 toulligqc-2.5.7/toulligqc/common.py
--rw-r--r--   0 root         (0) root         (0)     1357 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/common_statistics.py
--rw-r--r--   0 root         (0) root         (0)     2339 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/configuration.py
--rw-r--r--   0 root         (0) root         (0)    21561 2024-05-02 09:41:42.000000 toulligqc-2.5.7/toulligqc/extractor_common.py
--rw-r--r--   0 root         (0) root         (0)    10299 2024-05-02 09:41:42.000000 toulligqc-2.5.7/toulligqc/fast5_extractor.py
--rw-r--r--   0 root         (0) root         (0)     1633 2024-05-02 09:41:42.000000 toulligqc-2.5.7/toulligqc/fastq_bam_common.py
--rw-r--r--   0 root         (0) root         (0)    13705 2024-05-02 09:41:42.000000 toulligqc-2.5.7/toulligqc/fastq_extractor.py
--rw-r--r--   0 root         (0) root         (0)    17105 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/html_report_generator.py
--rw-r--r--   0 root         (0) root         (0)    43353 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/plotly_graph_common.py
--rw-r--r--   0 root         (0) root         (0)    31187 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/plotly_graph_generator.py
--rw-r--r--   0 root         (0) root         (0)    16322 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/plotly_graph_onedsquare_generator.py
--rw-r--r--   0 root         (0) root         (0)     1776 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/report_data_file_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 09:41:48.737793 toulligqc-2.5.7/toulligqc/resources/
--rw-r--r--   0 root         (0) root         (0)  3478132 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/resources/plotly-latest.min.js
--rw-r--r--   0 root         (0) root         (0)     2339 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/resources/toulligqc.css
--rw-r--r--   0 root         (0) root         (0)     5548 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/resources/toulligqc.png
--rw-r--r--   0 root         (0) root         (0)    21191 2024-05-02 09:41:42.000000 toulligqc-2.5.7/toulligqc/sequencing_summary_extractor.py
--rw-r--r--   0 root         (0) root         (0)    22743 2024-05-02 09:41:42.000000 toulligqc-2.5.7/toulligqc/sequencing_summary_onedsquare_extractor.py
--rw-r--r--   0 root         (0) root         (0)     7181 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/sequencing_telemetry_extractor.py
--rw-r--r--   0 root         (0) root         (0)    17629 2024-05-02 09:41:42.000000 toulligqc-2.5.7/toulligqc/toulligqc.py
--rw-r--r--   0 root         (0) root         (0)     6203 2024-05-02 09:41:26.000000 toulligqc-2.5.7/toulligqc/toulligqc_info_extractor.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-02 09:41:42.000000 toulligqc-2.5.7/toulligqc/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 09:41:48.733793 toulligqc-2.5.7/toulligqc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      941 2024-05-02 09:41:48.000000 toulligqc-2.5.7/toulligqc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1119 2024-05-02 09:41:48.000000 toulligqc-2.5.7/toulligqc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 09:41:48.000000 toulligqc-2.5.7/toulligqc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-05-02 09:41:48.000000 toulligqc-2.5.7/toulligqc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 09:41:48.000000 toulligqc-2.5.7/toulligqc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      149 2024-05-02 09:41:48.000000 toulligqc-2.5.7/toulligqc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-02 09:41:48.000000 toulligqc-2.5.7/toulligqc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 14:36:09.714009 toulligqc-2.6/
+-rw-r--r--   0 root         (0) root         (0)      252 2024-01-26 14:32:07.000000 toulligqc-2.6/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    21146 2024-01-26 14:32:07.000000 toulligqc-2.6/LICENSE-CeCILL.txt
+-rw-r--r--   0 root         (0) root         (0)    35466 2024-01-26 14:32:07.000000 toulligqc-2.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-01-26 14:32:07.000000 toulligqc-2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      939 2024-01-26 14:36:09.714009 toulligqc-2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14814 2024-01-26 14:32:17.000000 toulligqc-2.6/README.md
+-rw-r--r--   0 root         (0) root         (0)      111 2024-01-26 14:36:09.714009 toulligqc-2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-01-26 14:32:07.000000 toulligqc-2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 14:36:09.706009 toulligqc-2.6/test/
+-rw-r--r--   0 root         (0) root         (0)    15570 2024-01-26 14:32:07.000000 toulligqc-2.6/test/test_sequencing_summary_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 14:36:09.710009 toulligqc-2.6/toulligqc/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15757 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/bam_extractor.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/common.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/common_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/configuration.py
+-rw-r--r--   0 root         (0) root         (0)    21950 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/extractor_common.py
+-rw-r--r--   0 root         (0) root         (0)     9295 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/fast5_extractor.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/fastq_bam_common.py
+-rw-r--r--   0 root         (0) root         (0)    16459 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/fastq_extractor.py
+-rw-r--r--   0 root         (0) root         (0)    17105 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/html_report_generator.py
+-rw-r--r--   0 root         (0) root         (0)    43010 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/plotly_graph_common.py
+-rw-r--r--   0 root         (0) root         (0)    31187 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/plotly_graph_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16322 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/plotly_graph_onedsquare_generator.py
+-rw-r--r--   0 root         (0) root         (0)     9063 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/pod5_extractor.py
+-rw-r--r--   0 root         (0) root         (0)     1776 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/report_data_file_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 14:36:09.714009 toulligqc-2.6/toulligqc/resources/
+-rw-r--r--   0 root         (0) root         (0)  3478132 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/resources/plotly-latest.min.js
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/resources/toulligqc.css
+-rw-r--r--   0 root         (0) root         (0)     5548 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/resources/toulligqc.png
+-rw-r--r--   0 root         (0) root         (0)    21685 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/sequencing_summary_extractor.py
+-rw-r--r--   0 root         (0) root         (0)    22743 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/sequencing_summary_onedsquare_extractor.py
+-rw-r--r--   0 root         (0) root         (0)     7181 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/sequencing_telemetry_extractor.py
+-rw-r--r--   0 root         (0) root         (0)    18123 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/toulligqc.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/toulligqc_info_extractor.py
+-rw-r--r--   0 root         (0) root         (0)       20 2024-01-26 14:32:08.000000 toulligqc-2.6/toulligqc/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 14:36:09.710009 toulligqc-2.6/toulligqc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      939 2024-01-26 14:36:09.000000 toulligqc-2.6/toulligqc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-01-26 14:36:09.000000 toulligqc-2.6/toulligqc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-26 14:36:09.000000 toulligqc-2.6/toulligqc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-01-26 14:36:09.000000 toulligqc-2.6/toulligqc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-26 14:36:09.000000 toulligqc-2.6/toulligqc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      146 2024-01-26 14:36:09.000000 toulligqc-2.6/toulligqc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-01-26 14:36:09.000000 toulligqc-2.6/toulligqc.egg-info/top_level.txt
```

### Comparing `toulligqc-2.5.7/LICENSE-CeCILL.txt` & `toulligqc-2.6/LICENSE-CeCILL.txt`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/LICENSE.txt` & `toulligqc-2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/PKG-INFO` & `toulligqc-2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toulligqc
-Version: 2.5.7
+Version: 2.6
 Summary: A post sequencing QC tool for Oxford Nanopore sequencers
 Home-page: https://github.com/GenomicParisCentre/toulligQC
 Author: Genomic Paris Centre team
 Author-email: toulligqc@biologie.ens.fr
 License: GPL V3
 Keywords: Nanopore MinION QC report
 Platform: ALL
```

### Comparing `toulligqc-2.5.7/README.md` & `toulligqc-2.6/README.md`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/setup.py` & `toulligqc-2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,18 +42,18 @@
     packages=['toulligqc'],
     package_dir={'toulligqc': "toulligqc"},
     package_data={'toulligqc': ['resources/*.css', 'resources/*.js', 'resources/*.png']},
     zip_safe=False,
     include_package_data=True,
 
     python_requires='>=3.11.0',
-    install_requires=['matplotlib>=3.6.3',   'plotly==4.5.0', 'h5py>=3.7.0',
+    install_requires=['matplotlib>=3.6.3',   'plotly>=5.15.0', 'h5py>=3.7.0',
                       'pandas>=1.5.3',       'numpy>=1.24.2',  'scipy>=1.10.1',
                       'scikit-learn>=1.2.1', 'tqdm>=4.64.1',   'pysam>=0.21.0',
-                      'ezcharts==0.7.6'],
+                      'pod5>=0.3.6'],
 
     entry_points={
         'console_scripts': [
             'toulligqc=toulligqc.toulligqc:main',
         ],
     },
 )
```

### Comparing `toulligqc-2.5.7/test/test_sequencing_summary_extractor.py` & `toulligqc-2.6/test/test_sequencing_summary_extractor.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/bam_extractor.py` & `toulligqc-2.6/toulligqc/bam_extractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 from math import log
 import os
 import numpy as np
 import pandas as pd
 import time
 import pysam
-from datetime import datetime
+from collections import defaultdict
 from toulligqc.extractor_common import log_task
 from toulligqc.extractor_common import describe_dict
 from toulligqc.extractor_common import set_result_value
 from toulligqc.extractor_common import add_image_to_result
 from toulligqc.extractor_common import check_result_values
 from toulligqc.extractor_common import count_boolean_elements
 from toulligqc.extractor_common import get_result_value
 from toulligqc.extractor_common import set_result_dict_telemetry_value
 from toulligqc.extractor_common import fill_series_dict
 from toulligqc.extractor_common import timeISO_to_float
+from toulligqc.extractor_common import extract_barcode_info
 from toulligqc.common_statistics import compute_NXX, compute_LXX, occupancy_channel, avg_qual
 from toulligqc.fastq_bam_common import multiprocessing_submit, extract_headerTag
 from toulligqc.fastq_bam_common import batch_iterator
 from toulligqc.common import is_numpy_1_24
 from toulligqc import plotly_graph_generator as pgg
 
 
 class uBAM_Extractor:
     def __init__(self, config_dictionary):
-        self.config_file_dictionary = config_dictionary
+        self.config_dictionary = config_dictionary
         self.ubam = config_dictionary['bam'].split('\t')
         self.images_directory = config_dictionary['images_directory']
         self.threshold_Qscore = int(config_dictionary['threshold'])
         self.batch_size = int(config_dictionary['batch_size'])
         self.thread = int(config_dictionary['thread'])
         self.header = dict()
+        self.is_barcode = False
+        if config_dictionary['barcoding'] == 'True':
+            self.is_barcode = True
         if 'quiet' not in config_dictionary or config_dictionary['quiet'].lower() != 'true':
             self.quiet = False
         else:
             self.quiet = True
 
     def check_conf(self):
         """
@@ -49,41 +53,52 @@
 
     def init(self):
         """
         Creation of the dataframe containing all info from uBAM
         :return: Panda's Dataframe object
         """
         start_time = time.time()
-        self.dataframe_1d = self._load_uBAM_data()
-        if self.dataframe_1d.empty:
+        self.dataframe = self._load_uBAM_file()
+        if self.dataframe.empty:
             raise pd.errors.EmptyDataError("Dataframe is empty")
         self.dataframe_dict = {}
+        
+        # Add missing categories
+        if 'barcode_arrangement' in self.dataframe.columns:
+           self.dataframe['barcode_arrangement'].cat.add_categories([0, 'other barcodes', 'passes_filtering'],
+                                                                       inplace=True)
+        
+        # Replace all NaN values by 0 to avoid data manipulation errors when columns are not the same length
+        self.dataframe = self.dataframe.fillna(0)
+            
+        self.barcode_selection = self.config_dictionary['barcode_selection']
+
         log_task(self.quiet,
-                 'Load BAM file ({:,.2f} MB used)'.format(self.dataframe_1d.memory_usage(deep=True).sum()/1024/1024),
+                 'Load BAM file ({:,.2f} MB used)'.format(self.dataframe.memory_usage(deep=True).sum()/1024/1024),
                  start_time,
                  time.time())
 
 
     def clean(self, result_dict):
         """
         Removing dictionary entries that will not be kept in the report.data file
         :return:
         """
         check_result_values(self, result_dict)
         self.dataframe_dict.clear()
-        self.dataframe_1d.iloc[0:0]
+        self.dataframe.iloc[0:0]
 
 
     @staticmethod
     def get_name() -> str:
         """
         Get the name of the extractor.
         :return: the name of the extractor
         """
-        return 'ubam'
+        return 'uBAM'
 
 
     @staticmethod
     def get_report_data_file_id() -> str:
         """
         Get the report.data id of the extractor.
         :return: the report.data id
@@ -96,47 +111,63 @@
         Generation of the different graphs containing in the plotly_graph_generator module
         :return: images array containing the title and the path toward the images
         """
         images = list()
 
         add_image_to_result(self.quiet, images, time.time(), pgg.read_count_histogram(result_dict, self.images_directory))
         add_image_to_result(self.quiet, images, time.time(), pgg.read_length_scatterplot(self.dataframe_dict, self.images_directory))
-        add_image_to_result(self.quiet, images, time.time(), pgg.yield_plot(self.dataframe_1d, self.images_directory))
+        add_image_to_result(self.quiet, images, time.time(), pgg.yield_plot(self.dataframe, self.images_directory))
         add_image_to_result(self.quiet, images, time.time(), pgg.read_quality_multiboxplot(self.dataframe_dict, self.images_directory))
         add_image_to_result(self.quiet, images, time.time(), pgg.allphred_score_frequency(self.dataframe_dict, self.images_directory))
-        add_image_to_result(self.quiet, images, time.time(), pgg.plot_performance(self.dataframe_1d, self.images_directory))
+        add_image_to_result(self.quiet, images, time.time(), pgg.plot_performance(self.dataframe, self.images_directory))
         add_image_to_result(self.quiet, images, time.time(), pgg.twod_density(self.dataframe_dict, self.images_directory))
         add_image_to_result(self.quiet, images, time.time(), pgg.sequence_length_over_time(self.dataframe_dict, self.images_directory))
         add_image_to_result(self.quiet, images, time.time(), pgg.phred_score_over_time(self.dataframe_dict, result_dict, self.images_directory))
         add_image_to_result(self.quiet, images, time.time(), pgg.speed_over_time(self.dataframe_dict, self.images_directory))
+        if self.is_barcode:
+            add_image_to_result(self.quiet, images, time.time(), pgg.barcode_percentage_pie_chart_pass(self.dataframe_dict,
+                                                                                                       self.barcode_selection,
+                                                                                                       self.images_directory))
+
+            read_fail = self.dataframe_dict["read.fail.barcoded"]
+            if not (len(read_fail) == 1 and read_fail["other barcodes"] == 0):
+                add_image_to_result(self.quiet, images, time.time(), pgg.barcode_percentage_pie_chart_fail(self.dataframe_dict,
+                                                                                                      self.barcode_selection,
+                                                                                                      self.images_directory))
+
+            add_image_to_result(self.quiet, images, time.time(), pgg.barcode_length_boxplot(self.dataframe_dict,
+                                                                                            self.images_directory))
+
+            add_image_to_result(self.quiet, images, time.time(), pgg.barcoded_phred_score_frequency(self.dataframe_dict,
+                                                                                                    self.images_directory))
         return images
 
 
     def extract(self, result_dict):
         """
         Get Phred score (Qscore) and Length details (frequencies, ratios, yield and statistics) per type read (pass or fail)
         :param result_dict:
         """
         start_time = time.time()
-        fill_series_dict(self.dataframe_dict, self.dataframe_1d)
+        fill_series_dict(self.dataframe_dict, self.dataframe)
 
         set_result_dict_telemetry_value(result_dict, "run.id", self.header["run_id"])
         set_result_dict_telemetry_value(result_dict, "sample.id", self.header["sample_id"])
         set_result_dict_telemetry_value(result_dict, "model.file", self.header["model_version_id"])
         set_result_dict_telemetry_value(result_dict, "software.name", self.header["basecaller"])
         set_result_dict_telemetry_value(result_dict, "software.version", self.header["basecaller_version"])
         set_result_dict_telemetry_value(result_dict, "flowcell.id", self.header["flow_cell_id"])
         set_result_dict_telemetry_value(result_dict, "basecalling.date", self.header["run_date"])
         set_result_dict_telemetry_value(result_dict, "pass.threshold.qscore", str(self.threshold_Qscore))
 
-        set_result_value(self, result_dict, "read.count", len(self.dataframe_1d))
+        set_result_value(self, result_dict, "read.count", len(self.dataframe))
         set_result_value(self, result_dict, "read.pass.count",
-                         count_boolean_elements(self.dataframe_1d, 'passes_filtering', True))
+                         count_boolean_elements(self.dataframe, 'passes_filtering', True))
         set_result_value(self, result_dict, "read.fail.count",
-                         count_boolean_elements(self.dataframe_1d, 'passes_filtering', False))
+                         count_boolean_elements(self.dataframe, 'passes_filtering', False))
         total_reads = get_result_value(self, result_dict, "read.count")
 
         # Ratios
         set_result_value(self, result_dict, "read.pass.ratio",
                          (get_result_value(self, result_dict, "read.pass.count") / total_reads))
         set_result_value(self, result_dict, "read.fail.ratio",
                          (get_result_value(self, result_dict, "read.fail.count") / total_reads))
@@ -156,17 +187,17 @@
 
         # Yield, n50, run time
         set_result_value(self, result_dict, "yield", sum(self.dataframe_dict["all.reads.sequence.length"]))
 
         set_result_value(self, result_dict, "n50", compute_NXX(self.dataframe_dict, 50))
         set_result_value(self, result_dict, "l50", compute_LXX(self.dataframe_dict, 50))
 
-        set_result_value(self, result_dict, "run.time", max(self.dataframe_1d['start_time']))
+        set_result_value(self, result_dict, "run.time", max(self.dataframe['start_time']))
         # Get channel occupancy statistics and store each value into result_dict
-        for index, value in occupancy_channel(self.dataframe_1d).items():
+        for index, value in occupancy_channel(self.dataframe).items():
             set_result_value(self,
                             result_dict, "channel.occupancy.statistics." + index, value)
         
         # Get statistics about all reads length and store each value into result_dict
         sequence_length_statistics = self.dataframe_dict["all.reads.sequence.length"].describe()
 
         for index, value in sequence_length_statistics.items():
@@ -176,69 +207,76 @@
         # Add statistics (without count) about read pass/fail length in the result_dict
         describe_dict(self, result_dict, self.dataframe_dict["pass.reads.sequence.length"],
                       "pass.reads.sequence.length")
         describe_dict(self, result_dict, self.dataframe_dict["fail.reads.sequence.length"],
                       "fail.reads.sequence.length")
 
         # Get Qscore statistics without count value and store them into result_dict
-        qscore_statistics = self.dataframe_1d['mean_qscore'].describe().drop(
+        qscore_statistics = self.dataframe['mean_qscore'].describe().drop(
             "count")
 
         for index, value in qscore_statistics.items():
             set_result_value(self,
                              result_dict, "all.read.qscore." + index, value)
 
         # Add statistics (without count) about read pass/fail qscore in the result_dict
         describe_dict(self, result_dict, self.dataframe_dict["pass.reads.mean.qscore"], "pass.reads.mean.qscore")
         describe_dict(self, result_dict, self.dataframe_dict["fail.reads.mean.qscore"], "fail.reads.mean.qscore")
-
+        if self.is_barcode:
+            extract_barcode_info(self, result_dict,
+                                 self.barcode_selection,
+                                 self.dataframe_dict,
+                                 self.dataframe)
+                                 
         log_task(self.quiet, 'Extract info from uBAM file', start_time, time.time())       
 
 
-    def _load_uBAM_data(self):
+    def _load_uBAM_file(self):
         """
         Load uBAM dataframe
         :return: a Pandas Dataframe object
         """  
         self._get_header()
         uBAM_chunks = self._uBAM_batch_generator()
         rst_futures = multiprocessing_submit(self._uBAM_batch_reader,
                                                         uBAM_chunks, 
                                                         n_process=self.thread, 
                                                         pbar_update=self.batch_size)
-        uBAM_data = []
+        uBAM_df = []
         
         for _, f in enumerate(rst_futures):
-            uBAM_data.extend(f.result())
+            uBAM_df.extend(f.result())
 
         columns = ['sequence_length', 'mean_qscore', 'passes_filtering', 'start_time', 'channel', 'duration']
-        
-        uBAM_data = pd.DataFrame(uBAM_data, columns=columns)
+        if self.is_barcode:
+            columns.append('barcode_arrangement')
+
+        uBAM_df = pd.DataFrame(uBAM_df, columns=columns)
 
-        uBAM_data['sequence_length'] = uBAM_data['sequence_length'].astype(np.uint32)
-        uBAM_data['mean_qscore'] = uBAM_data['mean_qscore'].astype(np.float32)
-        uBAM_data['passes_filtering'] = uBAM_data['passes_filtering'].astype(np.bool_ if is_numpy_1_24 else np.bool)
-        uBAM_data["start_time"] = uBAM_data["start_time"] - uBAM_data["start_time"].min()
-        uBAM_data['channel'] = uBAM_data['channel'].astype(np.int16)
-        uBAM_data['start_time'] = uBAM_data['start_time'].astype(np.float64)
-        uBAM_data['duration'] = uBAM_data['duration'].astype(np.float32)
-        return uBAM_data 
+        uBAM_df['sequence_length'] = uBAM_df['sequence_length'].astype(np.uint32)
+        uBAM_df['mean_qscore'] = uBAM_df['mean_qscore'].astype(np.float32)
+        uBAM_df['passes_filtering'] = uBAM_df['passes_filtering'].astype(np.bool_ if is_numpy_1_24 else np.bool)
+        uBAM_df["start_time"] = uBAM_df["start_time"] - uBAM_df["start_time"].min()
+        uBAM_df['channel'] = uBAM_df['channel'].astype(np.int16)
+        uBAM_df['start_time'] = uBAM_df['start_time'].astype(np.float64)
+        uBAM_df['duration'] = uBAM_df['duration'].astype(np.float32)
+        if self.is_barcode:
+            uBAM_df['barcode_arrangement'] = uBAM_df['barcode_arrangement'].astype("category")
+        return uBAM_df 
 
 
     def _uBAM_batch_reader(self, uBAM_chunk):
         """
         parse each line of uBAM quality line:
         return: [read length, mean Qscore, type of read (pass or fail)]
         """
         #def process_bam_chunk(bam_chunk):
         rec_data = []
-        record_count = 0
         for rec in uBAM_chunk:
-            record_count += 1
-            rec_dict = self._process_record(rec, record_count)
+            rec_dict = self._process_record(rec)
             rec_data.append(rec_dict)
         return rec_data
 
 
     def _uBAM_batch_generator(self):
         """
         read uBAM file in small chunk
@@ -247,56 +285,46 @@
         for ubam in self.ubam:
             samfile = pysam.AlignmentFile(ubam, "rb", check_sq=False)
             bam_batch = batch_iterator(samfile, batch_size=self.batch_size)
             for batch in bam_batch:
                 yield batch
 
 
-    def _timeISO_to_float(self, iso_datetime, format):
-        """
-        """
-        dt = datetime.strptime(iso_datetime, format)
-        unix_timestamp = dt.timestamp()
-        return unix_timestamp
-
-
     def _get_header(self):
-        sam_file = pysam.AlignmentFile(self.ubam[0], "rb", check_sq=False)
-        header = sam_file.header.to_dict()
-        run_id, model_version_id = extract_headerTag(header, 'RG','ID',
-                                                     'Unknown_Unknown').split('_', 1)
+        samfile = pysam.AlignmentFile(self.ubam[0], "rb", check_sq=False)
+        header = samfile.header.to_dict()
+        run_id, model_version_id =  extract_headerTag(header,'RG','ID').split('_', 1)
         self.header = {
-            "run_id": run_id,
-            "run_date": extract_headerTag(header, 'RG', 'DT', 'Unknown'),
-            "sample_id": extract_headerTag(header, 'RG', 'SM', 'Unknown'),
-            "basecaller": extract_headerTag(header, 'PG', 'PN', 'Unknown'),
-            "basecaller_version": extract_headerTag(header, 'PG', 'VN', 'Unknown'),
-            "model_version_id": model_version_id,
-            "flow_cell_id": extract_headerTag(header, 'RG', 'PU', 'Unknown')
+        "run_id" : run_id,
+        "run_date" : extract_headerTag(header, 'RG', 'DT'),
+        "sample_id" : extract_headerTag(header,'RG','SM'),
+        "basecaller" : extract_headerTag(header,'PG','PN'),
+        "basecaller_version" : extract_headerTag(header,'PG','VN'),
+        "model_version_id" : model_version_id,
+        "flow_cell_id" : extract_headerTag(header,'RG','PU')
         }
 
-
-    def _process_record(self, rec, record_count):
+    
+    
+    def _process_record(self, rec):
         """
         extract QC info from BAM record
         return : dict of QC info
         """
-        fields = rec.split("\t")
-
-        # Parse optional fields
-        attributes = {}
-        for t in fields[11:]:
-            k, t, v = t.split(':', 2)
-            attributes[k] = v
-
-        iso_start_time = attributes.get('st', None)
-        qual = avg_qual(fields[10])
+        tags = rec.split("\t")
+        tag_dict = defaultdict(lambda:'unclassified')
+        tag_dict.update({key : value for key,_, value in [item.split(':',2) for item in tags[11:]]})
+        start_time = timeISO_to_float(tag_dict['st'], '%Y-%m-%dT%H:%M:%S.%f%z')
+        qual = avg_qual(tags[10]) 
         passes_filtering = True if qual > self.threshold_Qscore else False
         data = [
-            len(fields[9]), # read length
-            qual, # AVG Qscore
-            passes_filtering, # Passing filter
-            float(record_count) if iso_start_time is None else timeISO_to_float(iso_start_time, '%Y-%m-%dT%H:%M:%S.%f%z'), # start time
-            attributes.get('ch', '1'),  # Channel
-            attributes.get('du', '1')  # Duration
+            len(tags[9]),
+            qual,
+            passes_filtering,
+            start_time,
+            tag_dict['ch'],
+            tag_dict['du']
         ]
-        return data
+        if self.is_barcode:
+            bc = tag_dict['BC'].split('_')[-1]
+            data.append(bc)
+        return data
```

### Comparing `toulligqc-2.5.7/toulligqc/common_statistics.py` & `toulligqc-2.6/toulligqc/common_statistics.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/configuration.py` & `toulligqc-2.6/toulligqc/configuration.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/extractor_common.py` & `toulligqc-2.6/toulligqc/extractor_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,22 +443,34 @@
                 return f.readline()
         else:
             with open(filename, 'r') as f:
                 return f.readline()
     except IOError:
         raise FileNotFoundError
 
+
 def set_result_dict_telemetry_value(result_dict, key, new_value):
     """
     """
     final_key = "sequencing.telemetry.extractor." + key
     current_value = None
 
     if final_key in result_dict:
         current_value = result_dict[final_key]
         if len(current_value) == 0:
             current_value = None
 
     if new_value is None:
         new_value = current_value
 
-    result_dict[final_key] = new_value
+    result_dict[final_key] = new_value
+
+
+def pd_read_sequencing_summary(file, cols, data_type):
+        try:
+            return pd.read_csv(file, sep="\t", usecols=cols,
+                            dtype=data_type)
+        except:
+            del data_type['passes_filtering']
+            cols.remove('passes_filtering')
+            return pd.read_csv(file, sep="\t", usecols=cols,
+                            dtype=data_type)
```

### Comparing `toulligqc-2.5.7/toulligqc/fast5_extractor.py` & `toulligqc-2.6/toulligqc/fast5_extractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 #
 # First author: Lionel Ferrato-Berberian
 # Maintainer: Bérengère Laffay
 # Since version 0.1
 
 # Extraction of the information about the FAST5 files
 
-import glob
 import os
 import shutil
 import sys
 import tarfile
 import tempfile
-
 import h5py
 
+from toulligqc.common import find_file_in_directory
+from toulligqc.common import set_result_dict_value
 
 class Fast5Extractor:
     """
     Extraction of different information from a FAST5 file
     param fast5_source: FAST5 file directory
     param result_directory: dictionary which gathers all the extracted
     information that will be reported in the report.data file
@@ -60,60 +60,65 @@
         :return:
         """
 
         if not os.path.exists(self.fast5_source):
             return False, 'The input file or directory for Fast5 file does not exists: ' + self.fast5_source
 
         if os.path.isdir(self.fast5_source):
-            file_found = self._find_file_in_directory()
+            file_found = find_file_in_directory(self.fast5_source, "fast5")
             if file_found is None:
                 return False, 'No Fast5 file found in directory: ' + self.fast5_source
             self.file_to_process = file_found
         else:
             self.file_to_process = self.fast5_source
 
-        if self.file_to_process.endswith('.tar.gz'):
-            self.fast5_file_extension = 'tar.gz'
+        if self.file_to_process.endswith('.tar'):
+            self.fast5_file_extension = 'tar'
 
-        elif self.file_to_process.endswith('.fast5'):
-            self.fast5_file_extension = 'fast5'
+        elif self.file_to_process.endswith('.tar.gz'):
+            self.fast5_file_extension = 'tar.gz'
 
         elif self.file_to_process.endswith('.tar.bz2'):
             self.fast5_file_extension = 'tar.bz2'
 
+        elif self.file_to_process.endswith('.fast5'):
+            self.fast5_file_extension = 'fast5'
+
         else:
-            return False, 'The fast5 extension is not supported (fast5, tar.bz2 or tar.gz format): ' + self.fast5_source
+            return (False, 'The file extension for FAST5 input is not supported '
+                           '(only .fast5, .tar, .tar.gz or .tar.bz2 are supported): ' + self.fast5_source)
 
         return True, ""
 
 
-
-
     def init(self):
         """
         Determination of the fast5 file extension
         """
         return
 
+
     @staticmethod
     def get_name():
         """
         Get the name of the extractor.
         :return: the name of the extractor
         """
         return 'Fast5'
 
+
     @staticmethod
     def get_report_data_file_id():
         """
         Get the report.data id of the extractor
         :return: the report.data id
         """
         return 'fast5.extractor'
 
+
     def extract(self, result_dict):
         """
         Extraction of the different information about the fast5 files
         :param result_dict: Dictionary which gathers all the extracted
         information that will be reported in the report.data file
         :return: result_dict filled
         """
@@ -121,110 +126,104 @@
         tracking_id_dict = self._get_fast5_items(h5py_file, 'tracking_id')
 
         if len(tracking_id_dict) == 0:
             return
 
         prefix = 'sequencing.telemetry.extractor'
         result_dict[prefix + '.source'] = self.fast5_source
-        _set_result_dict_value(result_dict, prefix + '.flowcell.id', tracking_id_dict, 'flow_cell_id')
-        _set_result_dict_value(result_dict, prefix + '.minknow.version', tracking_id_dict, 'version')
-        _set_result_dict_value(result_dict, prefix + '.hostname', tracking_id_dict, 'hostname')
-        _set_result_dict_value(result_dict, prefix + '.operating.system', tracking_id_dict, 'operating_system')
-        _set_result_dict_value(result_dict, prefix + '.run.id', tracking_id_dict, 'run_id')
-        _set_result_dict_value(result_dict, prefix + '.protocol.run.id', tracking_id_dict, 'protocol_run_id')
-        _set_result_dict_value(result_dict, prefix + '.protocol.group.id', tracking_id_dict, 'protocol_group_id')
-        _set_result_dict_value(result_dict, prefix + '.sample.id', tracking_id_dict, 'sample_id')
-        _set_result_dict_value(result_dict, prefix + '.exp.start.time', tracking_id_dict, 'exp_start_time')
-        _set_result_dict_value(result_dict, prefix + '.device.id', tracking_id_dict, 'device_id')
-        _set_result_dict_value(result_dict, prefix + '.device.type', tracking_id_dict, 'device_type')
-        _set_result_dict_value(result_dict, prefix + '.distribution.version', tracking_id_dict, 'distribution_version')
-        _set_result_dict_value(result_dict, prefix + '.flow.cell.product.code', tracking_id_dict,
+        set_result_dict_value(result_dict, prefix + '.flowcell.id', tracking_id_dict, 'flow_cell_id')
+        set_result_dict_value(result_dict, prefix + '.minknow.version', tracking_id_dict, 'version')
+        set_result_dict_value(result_dict, prefix + '.hostname', tracking_id_dict, 'hostname')
+        set_result_dict_value(result_dict, prefix + '.operating.system', tracking_id_dict, 'operating_system')
+        set_result_dict_value(result_dict, prefix + '.run.id', tracking_id_dict, 'run_id')
+        set_result_dict_value(result_dict, prefix + '.protocol.run.id', tracking_id_dict, 'protocol_run_id')
+        set_result_dict_value(result_dict, prefix + '.protocol.group.id', tracking_id_dict, 'protocol_group_id')
+        set_result_dict_value(result_dict, prefix + '.sample.id', tracking_id_dict, 'sample_id')
+        set_result_dict_value(result_dict, prefix + '.exp.start.time', tracking_id_dict, 'exp_start_time')
+        set_result_dict_value(result_dict, prefix + '.device.id', tracking_id_dict, 'device_id')
+        set_result_dict_value(result_dict, prefix + '.device.type', tracking_id_dict, 'device_type')
+        set_result_dict_value(result_dict, prefix + '.distribution.version', tracking_id_dict, 'distribution_version')
+        set_result_dict_value(result_dict, prefix + '.flow.cell.product.code', tracking_id_dict,
                                'flow_cell_product_code')
 
         context_tags_dict = self._get_fast5_items(h5py_file, 'context_tags')
         if len(context_tags_dict) != 0:
-            _set_result_dict_value(result_dict, prefix + '.selected.speed.bases.per.second', context_tags_dict, 'selected_speed_bases_per_second')
-            _set_result_dict_value(result_dict, prefix + '.sample.frequency', context_tags_dict, 'sample_frequency')
-            _set_result_dict_value(result_dict, prefix + '.sequencing.kit.version', context_tags_dict, 'sequencing_kit')
+            set_result_dict_value(result_dict, prefix + '.selected.speed.bases.per.second', context_tags_dict, 'selected_speed_bases_per_second')
+            set_result_dict_value(result_dict, prefix + '.sample.frequency', context_tags_dict, 'sample_frequency')
+            set_result_dict_value(result_dict, prefix + '.sequencing.kit.version', context_tags_dict, 'sequencing_kit')
 
 
     def graph_generation(self, result_dict):
         """
         Graph generation
         :return: nothing
         """
         return []
 
+
     def clean(self, result_dict):
         """
         Deleting the temporary fast5 file extracted from the tar archive if used
         and removing dictionary entries that will not be kept in the report.data file
         :param result_dict: dictionary which gathers all the extracted
         information that will be reported in the report.data file
         :return:
         """
         if self.temporary_directory:
             shutil.rmtree(self.temporary_directory, ignore_errors=True)
 
-    def _fast5_tar_bz2_extraction(self, tar_bz2_file, output_directory):
-        """
-        Extraction of the FAST5 file stored in tar_bz2 format
-        :param tar_bz2_file: tar bz2 file containing the set of the raw FAST5 files
-        :param output_directory:dictionary which gathers all the extracted
-        information that will be reported in the report.data file
-        :return: a FAST5 file
-        """
-        tar_bz2 = tarfile.open(tar_bz2_file, 'r:bz2')
-        while True:
-            member = tar_bz2.next()
-            if member.name.endswith('.fast5'):
-                tar_bz2.extract(member, path=output_directory)
-                break
-        return output_directory + '/' + member.name
 
-    def _fast5_tar_gz_extraction(self, tar_gz_file, output_directory):
+    def _fast5_tar_extraction(self, tar_file, extension, output_directory):
         """
-        Extraction of a FAST5 file stored in tar_gz format
-        :param tar_gz_file: tar gz file containing the set of the raw FAST5 files
+        Extraction of a FAST5 file stored in a tar file,
+        :param tar_file: tar file containing the set of the raw FAST5 files
+        :param extension of the file
         :param output_directory: dictionary which gathers all the extracted
         information that will be reported in the report.data file
         :return: a FAST5 file
         """
-        tar_gz = tarfile.open(self, tar_gz_file, 'r:gz')
+
+        if extension == 'tar.gz':
+            tar_mode = 'r:gz'
+        elif extension == 'tar.bz2':
+            tar_mode = 'r:bz2'
+        else:
+            tar_mode = 'r'
+
+        tf = tarfile.open(name=tar_file, mode=tar_mode)
         while True:
-            member = tar_gz.next()
+            member = tf.next()
             if member.name.endswith('.fast5'):
-                tar_gz.extract(member, path=output_directory)
+                tf.extract(member, path=output_directory)
                 break
         return output_directory + '/' + member.name
 
+
     def _read_fast5(self):
         """
         Extraction of one fast5 file from the archive and stores
         it in a h5py object for next retrieving information
         :return: h5py_file: h5py file
         """
         self.temporary_directory = tempfile.mkdtemp()
-        if self.fast5_file_extension == 'tar.bz2':
-            tar_bz2_file = self.file_to_process
-            self.fast5_file = self._fast5_tar_bz2_extraction(tar_bz2_file, self.temporary_directory)
-
-        elif self.fast5_file_extension == 'tar.gz':
-            tar_gz_file = self.file_to_process
-            self.fast5_file = self._fast5_tar_gz_extraction(tar_gz_file, self.temporary_directory)
-
+        if self.fast5_file_extension == 'tar' or \
+                self.fast5_file_extension == 'tar.gz' or \
+                self.fast5_file_extension == 'tar.bz2':
+            self.fast5_file = self._fast5_tar_extraction(self.file_to_process, self.fast5_file_extension,
+                                                         self.temporary_directory)
         elif self.fast5_file_extension == 'fast5' or self.fast5_file_extension == '.fast5':
             self.fast5_file = self.file_to_process
         else:
             err_msg = 'There is a problem with the fast5 file or the tar file'
             sys.exit(err_msg)
         h5py_file = h5py.File(self.fast5_file)
 
         return h5py_file
 
+
     def _get_fast5_items(self, h5py_file, group):
         """
         Global function to extract run information stores in h5py format
         :param h5py_file: fast5 file store in a h5py object
         :param key:  required h5py attributes
         :return: h5py value, for example flow_cell_id : FAE22827
         """
@@ -233,29 +232,7 @@
             new_group = '/' + k + '/' + group
             if new_group in h5py_file:
                 tracking_id_items = list(h5py_file[new_group].attrs.items())
                 tracking_id_dict = {key: value.decode('utf-8') for key, value in tracking_id_items}
                 return tracking_id_dict
 
         return {}
-
-    def _find_file_in_directory(self):
-        """
-        Method that looking for a suitable Fast5 file in the source directory.
-        :return: The path to the first suitable file in the source directory
-        """
-
-        for ext in ('fast5', 'tar.bz2', 'tar.gz'):
-            if glob.glob(self.fast5_source + '/*.' + ext):
-                files_found = os.listdir(self.fast5_source)
-                if len(files_found) > 0:
-                    return self.fast5_source + files_found[0]
-
-        return None
-
-
-def _set_result_dict_value(result_dict, key, tracking_id_dict, dict_key):
-    value = ''
-    if dict_key in tracking_id_dict:
-        value = tracking_id_dict[dict_key]
-
-    result_dict[key] = value
```

### Comparing `toulligqc-2.5.7/toulligqc/fastq_bam_common.py` & `toulligqc-2.6/toulligqc/fastq_bam_common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,13 @@
 import multiprocessing as mp
 from tqdm import tqdm
 from concurrent.futures import ProcessPoolExecutor, as_completed
 
-def extract_headerTag(header, tagGroup, tag, defaultValue = None):
-
-    if tagGroup not in header:
-        if defaultValue is not None:
-            return defaultValue
-        else:
-            raise KeyError(tagGroup)
-
-    first_entry = header[tagGroup][0]
-
-    if tag not in first_entry:
-        if defaultValue is not None:
-            return defaultValue
-        else:
-            raise KeyError(tag)
-
-    return first_entry[tag]
+def extract_headerTag(header, tagGroup, tag):
+        return header[tagGroup][0][tag]
 
 
 def batch_iterator(iterator, batch_size):
     batch = []
     i=0
     for entry in iterator:
         i += 1
```

### Comparing `toulligqc-2.5.7/toulligqc/fastq_extractor.py` & `toulligqc-2.6/toulligqc/fastq_extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,31 +10,35 @@
 from toulligqc.extractor_common import check_result_values
 from toulligqc.extractor_common import add_image_to_result
 from toulligqc.extractor_common import count_boolean_elements
 from toulligqc.extractor_common import get_result_value
 from toulligqc.extractor_common import fill_series_dict
 from toulligqc.extractor_common import set_result_dict_telemetry_value
 from toulligqc.extractor_common import timeISO_to_float
+from toulligqc.extractor_common import extract_barcode_info
 from toulligqc.common_statistics import compute_NXX, compute_LXX, occupancy_channel, avg_qual
 from toulligqc.fastq_bam_common import multiprocessing_submit
 from toulligqc.common import is_numpy_1_24
 from toulligqc import plotly_graph_generator as pgg
 
 
 class fastqExtractor:
 
     def __init__(self, config_dictionary):
-        self.config_file_dictionary = config_dictionary
+        self.config_dictionary = config_dictionary
         self.fastq = config_dictionary['fastq'].split('\t')
         self.images_directory = config_dictionary['images_directory']
         self.threshold_Qscore = int(config_dictionary['threshold'])
         self.batch_size = int(config_dictionary['batch_size'])
         self.thread = int(config_dictionary['thread'])
         self.rich = False
         self.runid, self.sampleid, self.model_version_id = ['Unknow']*3
+        self.is_barcode = False
+        if config_dictionary['barcoding'] == 'True':
+            self.is_barcode = True
         if 'quiet' not in config_dictionary or config_dictionary['quiet'].lower() != 'true':
             self.quiet = False
         else:
             self.quiet = True
 
     def check_conf(self):
         """
@@ -53,14 +57,23 @@
         :return: Panda's Dataframe object
         """
         start_time = time.time()
         self.dataframe_1d = self._load_fastq_data()
         if self.dataframe_1d.empty:
             raise pd.errors.EmptyDataError("Dataframe is empty")
         self.dataframe_dict = {}
+
+        # Add missing categories
+        if 'barcode_arrangement' in self.dataframe_1d.columns:
+           self.dataframe_1d['barcode_arrangement'].cat.add_categories([0, 'other barcodes', 'passes_filtering'],
+                                                                       inplace=True)
+        self.dataframe_1d = self.dataframe_1d.fillna(0)
+        self.barcode_selection = self.config_dictionary['barcode_selection']
+        
+
         log_task(self.quiet,
                  'Load FASTQ file ({:,.2f} MB used)'.format(self.dataframe_1d.memory_usage(deep=True).sum()/1024/1024),
                  start_time,
                  time.time())
     
     def clean(extractor, result_dict):
         """
@@ -111,14 +124,30 @@
         add_image_to_result(self.quiet, images, time.time(), pgg.allphred_score_frequency(self.dataframe_dict, self.images_directory))
         if self.rich:
             add_image_to_result(self.quiet, images, time.time(), pgg.plot_performance(self.dataframe_1d, self.images_directory))
         add_image_to_result(self.quiet, images, time.time(), pgg.twod_density(self.dataframe_dict, self.images_directory))
         if self.rich:
             add_image_to_result(self.quiet, images, time.time(), pgg.sequence_length_over_time(self.dataframe_dict, self.images_directory))
             add_image_to_result(self.quiet, images, time.time(), pgg.phred_score_over_time(self.dataframe_dict, result_dict, self.images_directory))
+        if self.is_barcode:
+            add_image_to_result(self.quiet, images, time.time(), pgg.barcode_percentage_pie_chart_pass(self.dataframe_dict,
+                                                                                                       self.barcode_selection,
+                                                                                                       self.images_directory))
+
+            read_fail = self.dataframe_dict["read.fail.barcoded"]
+            if not (len(read_fail) == 1 and read_fail["other barcodes"] == 0):
+                add_image_to_result(self.quiet, images, time.time(), pgg.barcode_percentage_pie_chart_fail(self.dataframe_dict,
+                                                                                                      self.barcode_selection,
+                                                                                                      self.images_directory))
+
+            add_image_to_result(self.quiet, images, time.time(), pgg.barcode_length_boxplot(self.dataframe_dict,
+                                                                                            self.images_directory))
+
+            add_image_to_result(self.quiet, images, time.time(), pgg.barcoded_phred_score_frequency(self.dataframe_dict,
+                                                                                                    self.images_directory))
         return images
 
 
     def extract(self, result_dict):
         """
         Get Phred score (Qscore) and Length details (frequencies, ratios, yield and statistics) per type read (pass or fail)
         :param result_dict:
@@ -177,14 +206,19 @@
                              result_dict, "all.read.length." + index, value)
 
         # Add statistics (without count) about read pass/fail length in the result_dict
         describe_dict(self, result_dict, self.dataframe_dict["pass.reads.sequence.length"],
                       "pass.reads.sequence.length")
         describe_dict(self, result_dict, self.dataframe_dict["fail.reads.sequence.length"],
                       "fail.reads.sequence.length")
+        if self.is_barcode:
+            extract_barcode_info(self, result_dict,
+                                 self.barcode_selection,
+                                 self.dataframe_dict,
+                                 self.dataframe_1d)
 
         # Get Qscore statistics without count value and store them into result_dict
         qscore_statistics = self.dataframe_1d['mean_qscore'].describe().drop(
             "count")
 
         for index, value in qscore_statistics.items():
             set_result_value(self,
@@ -202,42 +236,47 @@
         Load FASTQ dataframe
         :return: a Pandas Dataframe object
         """
         run_info = self.check_fastq()
 
         if run_info:
             self.rich = True
-            self.runid, self.sampleid, self.model_version_id = run_info   
+            self.runid, self.sampleid, self.model_version_id = run_info
         else:
             self.rich = False
 
         read_batchs = self._fastq_batch_generator()
         rst_futures = multiprocessing_submit(self._fastq_batch_reader,
                                                         read_batchs, 
                                                         n_process=self.thread, 
                                                         pbar_update=self.batch_size)
-        fq_data = []
+        fq_df = []
         
         for _, f in enumerate(rst_futures):
-            fq_data.extend(f.result())
-
-        columns = ['sequence_length', 'mean_qscore', 'passes_filtering', 'start_time', 'channel'] if self.rich \
-                else ['sequence_length', 'mean_qscore', 'passes_filtering']
+            fq_df.extend(f.result())
 
-        fq_data = pd.DataFrame(fq_data, columns=columns)
-
-        fq_data['sequence_length'] = fq_data['sequence_length'].astype(np.uint32)
-        fq_data['mean_qscore'] = fq_data['mean_qscore'].astype(np.float32)
-        fq_data['passes_filtering'] = fq_data['passes_filtering'].astype(np.bool_ if is_numpy_1_24 else np.bool)
+        columns = ['sequence_length', 'mean_qscore', 'passes_filtering']
+        if self.rich:
+            columns.extend(['start_time', 'channel'])
+        if self.is_barcode:
+            columns.append('barcode_arrangement')
+
+        fq_df = pd.DataFrame(fq_df, columns=columns)
+
+        fq_df['sequence_length'] = fq_df['sequence_length'].astype(np.uint32)
+        fq_df['mean_qscore'] = fq_df['mean_qscore'].astype(np.float32)
+        fq_df['passes_filtering'] = fq_df['passes_filtering'].astype(np.bool_ if is_numpy_1_24 else np.bool)
 
         if self.rich:
-            fq_data["start_time"] = fq_data["start_time"] - fq_data["start_time"].min()
-            fq_data['start_time'] = fq_data['start_time'].astype(np.float64)
-            fq_data['channel'] = fq_data['channel'].astype(np.int16)
-        return fq_data 
+            fq_df["start_time"] = fq_df["start_time"] - fq_df["start_time"].min()
+            fq_df['start_time'] = fq_df['start_time'].astype(np.float64)
+            fq_df['channel'] = fq_df['channel'].astype(np.int16)
+        if self.is_barcode:
+            fq_df['barcode_arrangement'] = fq_df['barcode_arrangement'].astype("category")
+        return fq_df 
 
 
     def _fastq_batch_generator(self):
         """
         read FASTQ file in small batch
         yield : list of lines (quality line): batch of n size
         """
@@ -275,40 +314,47 @@
         """
         fastq_lines = []
         if self.rich:
             for read in read_batch:
                 name = read[0]
                 qscore = avg_qual(read[1])
                 passes_filtering = True if qscore > self.threshold_Qscore else False
-                start_time, ch = self._extract_info_from_name(name)
-                fastq_lines.append((len(read[1]), qscore, passes_filtering, start_time, ch))
+                if self.is_barcode:
+                    start_time, ch, barcode = self._extract_info_from_name(name)
+                    fastq_lines.append((len(read[1]), qscore, passes_filtering, start_time, ch, barcode))
+                else:
+                    start_time, ch = self._extract_info_from_name(name)
+                    fastq_lines.append((len(read[1]), qscore, passes_filtering, start_time, ch))
         else:
             for read in read_batch:
-                if len(read)>0:
-                    qscore = avg_qual(read)
-                    passes_filtering = True if qscore > self.threshold_Qscore else False
-                    fastq_lines.append((len(read), qscore, passes_filtering))
+                qscore = avg_qual(read)
+                passes_filtering = True if qscore > self.threshold_Qscore else False
+                fastq_lines.append((len(read), qscore, passes_filtering))
         return fastq_lines
 
 
     def check_fastq(self):
         """
         """
         open_fn = gzip.open if self.fastq[0].endswith('.gz') else open
 
         with open_fn(self.fastq[0], 'rt') as fq:
             first_line = fq.readline().strip('\n')
-        try:
-            metadata = dict(x.split("=") for x in first_line.split(" ")[1:])
-            if 'model_version_id' not in metadata:
+        metadata = dict(x.split("=") for x in first_line.split(" ")[1:])
+        if 'barcode' not in metadata:
+            self.is_barcode = False
+        if 'model_version_id' not in metadata:
                 metadata['model_version_id'] = 'Unknow'
+        try:
             return metadata['runid'] , metadata['sampleid'] , metadata['model_version_id'] 
         except:
             return None
 
 
     def _extract_info_from_name(self, name):
         """
         """
         metadata = dict(x.split("=") for x in name.split(" ")[1:])
         start_time = timeISO_to_float(metadata['start_time'], '%Y-%m-%dT%H:%M:%SZ')
+        if self.is_barcode:
+            return  start_time, metadata['ch'], metadata['barcode']
         return  start_time, metadata['ch']
```

### Comparing `toulligqc-2.5.7/toulligqc/html_report_generator.py` & `toulligqc-2.6/toulligqc/html_report_generator.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/plotly_graph_common.py` & `toulligqc-2.6/toulligqc/plotly_graph_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 # Maintainer: Karine Dias
 # Since version 2.0
 
 # This module contains common methods for plotly modules.
 
 from collections import defaultdict
 
-import pkgutil
 import numpy as np
 import pandas as pd
 import plotly.graph_objs as go
 import plotly.offline as py
 from scipy.interpolate import interp1d
 from scipy.ndimage.filters import gaussian_filter1d
 from sklearn.utils import resample
@@ -298,35 +297,29 @@
     v = (1 - a) * c + a * b
     r = hex(int(v))[2:]
 
     if len(r) == 1:
         return '0' + r
     return r
 
-def _copy_latest_minjs(result_directory, js_file):
-    with open(result_directory + '/' + js_file , 'w+') as f:
-        plotly_min_js = pkgutil.get_data(__name__, "resources/plotly-latest.min.js").decode('utf8')
-        f.write(plotly_min_js) 
 
 def _create_and_save_div(fig, result_directory, main):
     div = py.plot(fig,
                   include_plotlyjs=False,
                   output_type='div',
                   auto_open=False,
                   show_link=False)
 
     if result_directory is not None:
         output_file = result_directory + '/' + '_'.join(main.split())
-        js_file="plotly.min.js"
         py.plot(fig,
                 filename=output_file,
                 output_type="file",
-                include_plotlyjs= js_file, 
+                include_plotlyjs="directory",
                 auto_open=False)
-        _copy_latest_minjs(result_directory, js_file)
     else:
         output_file = None
 
     return div, output_file
 
 
 def _over_time_graph(data_series,
@@ -625,33 +618,33 @@
                               {'xaxis': {'visible': False},
                                'yaxis': {'visible': False},
                                'plot_bgcolor': 'white'}],
                         label="Reads Pie chart",
                         method="update"
                     ),
                     dict(
-                        args=[{'visible': [False, False, True, False]},
+                        args=[{'visible': [False, False, False, True]},
                               {**_xaxis('Barcodes', dict(visible=True)),
-                               **_yaxis('Read count', dict(visible=True)),
+                               **_yaxis('Base count', dict(visible=True)),
                                'plot_bgcolor': plotly_background_color}],
                         label="Reads Histogram",
                         method="update"
                     ),
                     dict(
                         args=[{'visible': [True, False, False, False]},
                               {'xaxis': {'visible': False},
                                'yaxis': {'visible': False},
                                'plot_bgcolor': 'white'}],
                         label="Bases Pie chart",
                         method="update"
                     ),
                     dict(
-                        args=[{'visible': [False, False, False, True]},
+                        args=[{'visible': [False, False, True, False]},
                               {**_xaxis('Barcodes', dict(visible=True)),
-                               **_yaxis('Base count', dict(visible=True)),
+                               **_yaxis('Read count', dict(visible=True)),
                                'plot_bgcolor': plotly_background_color}],
                         label="Bases Histogram",
                         method="update"
                     )
                 ]),
                 pad={"r": 20, "t": 20, "l": 40, "b": 20},
                 showactive=True,
```

### Comparing `toulligqc-2.5.7/toulligqc/plotly_graph_generator.py` & `toulligqc-2.6/toulligqc/plotly_graph_generator.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/plotly_graph_onedsquare_generator.py` & `toulligqc-2.6/toulligqc/plotly_graph_onedsquare_generator.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/report_data_file_generator.py` & `toulligqc-2.6/toulligqc/report_data_file_generator.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/resources/plotly-latest.min.js` & `toulligqc-2.6/toulligqc/resources/plotly-latest.min.js`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/resources/toulligqc.css` & `toulligqc-2.6/toulligqc/resources/toulligqc.css`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/resources/toulligqc.png` & `toulligqc-2.6/toulligqc/resources/toulligqc.png`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/sequencing_summary_extractor.py` & `toulligqc-2.6/toulligqc/sequencing_summary_extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from toulligqc.extractor_common import describe_dict
 from toulligqc.extractor_common import extract_barcode_info
 from toulligqc.extractor_common import get_result_value
 from toulligqc.extractor_common import set_result_value
 from toulligqc.extractor_common import log_task
 from toulligqc.extractor_common import add_image_to_result
 from toulligqc.extractor_common import read_first_line_file
+from toulligqc.extractor_common import pd_read_sequencing_summary
 from toulligqc.extractor_common import fill_series_dict
 from toulligqc.common_statistics import compute_NXX, compute_LXX, occupancy_channel
 from toulligqc.common import is_numpy_1_24
 
 class SequencingSummaryExtractor:
     """
     Extraction of data from sequencing_summary.txt and optional barcoding files.
@@ -58,14 +59,15 @@
         and _load_sequencing_summary_data methods
         :param config_dictionary: dictionary containing all files or directories paths for sequencing_summary.txt and barcoding files
         """
         self.config_dictionary = config_dictionary
         self.sequencing_summary_source = config_dictionary['sequencing_summary_source']
         self.images_directory = config_dictionary['images_directory']
         self.sequencing_summary_files = self.sequencing_summary_source.split('\t')
+        self.threshold_Qscore = int(config_dictionary['threshold'])
         if 'quiet' not in config_dictionary or config_dictionary['quiet'].lower() != 'true':
             self.quiet = False
         else:
             self.quiet = True
 
         self.is_barcode = False
         if config_dictionary['barcoding'] == 'True':
@@ -110,16 +112,21 @@
 
         # Rename 'sequence_length_template' and 'mean_qscore_template'
         self.dataframe_1d.rename(columns={'sequence_length_template': 'sequence_length',
                                           'mean_qscore_template': 'mean_qscore'}, inplace=True)
 
         # Add missing categories
         if 'barcode_arrangement' in self.dataframe_1d.columns:
+            #self.dataframe_1d['barcode_arrangement'].cat.add_categories([0, 'other barcodes', 'passes_filtering'],
+            #                                                            inplace=True)
             self.dataframe_1d['barcode_arrangement'] = self.dataframe_1d['barcode_arrangement'].cat.add_categories(
                                                                         [0, 'other barcodes', 'passes_filtering'])
+        if 'passes_filtering' not in self.dataframe_1d.columns:
+            self.dataframe_1d['passes_filtering'] = np.where(self.dataframe_1d['mean_qscore'] > self.threshold_Qscore, True, False)
+
 
         # Replace all NaN values by 0 to avoid data manipulation errors when columns are not the same length
         self.dataframe_1d = self.dataframe_1d.fillna(0)
 
         # Dictionary for storing all pd.Series and pd.Dataframe entries
         self.dataframe_dict = {}
 
@@ -326,58 +333,56 @@
             'read_id': object,
             'barcode_arrangement': 'category'
         }
 
         try:
             # If 1 file and it's a sequencing_summary.txt
             if len(files) == 1 and self._is_sequencing_summary_file(files[0]):
-                return pd.read_csv(files[0], sep="\t", usecols=sequencing_summary_columns,
-                                   dtype=sequencing_summary_datatypes)
+                return pd_read_sequencing_summary(files[0], cols=sequencing_summary_columns, data_type=sequencing_summary_datatypes)
 
             # If 1 file and it's a sequencing_summary.txt with barcode info, load column barcode_arrangement
             elif len(files) == 1 and self._is_sequencing_summary_with_barcodes(files[0]):
                 sequencing_summary_columns.append('barcode_arrangement')
                 sequencing_summary_datatypes.update(
                     {'barcode_arrangement': 'category'})
 
-                return pd.read_csv(files[0], sep="\t", usecols=sequencing_summary_columns,
-                                   dtype=sequencing_summary_datatypes)
+                return pd_read_sequencing_summary(files[0], cols=sequencing_summary_columns, data_type=sequencing_summary_datatypes)
 
             # If multiple files, check if there's a barcoding one and a sequencing one :
             for f in files:
                 # check for presence of barcoding files
                 if self._is_barcode_file(f):
-                    dataframe = pd.read_csv(
-                        f, sep="\t", usecols=barcoding_summary_columns, dtype=barcoding_summary_datatypes)
+                    dataframe = pd_read_sequencing_summary(
+                        f, cols=barcoding_summary_columns, data_type=barcoding_summary_datatypes)
                     if barcode_dataframe is None:
                         barcode_dataframe = dataframe
                     # if a barcoding file has already been read, append the 2 dataframes
                     else:
                         barcode_dataframe = barcode_dataframe.append(
                             dataframe, ignore_index=True)
 
                 # check for presence of sequencing_summary file with barcode info, if true load column barcode_arrangement and ignore barcoding files.
                 elif self._is_sequencing_summary_with_barcodes(f):
                     sequencing_summary_columns.append('barcode_arrangement')
                     sequencing_summary_datatypes.update(
                         {'barcode_arrangement': 'category'})
                     sys.stderr.write('Warning: The sequencing summary file {} contains barcode information.'
                                      ' The barcoding summary files will be skipped.\n'.format(f))
-                    return pd.read_csv(f, sep="\t", usecols=sequencing_summary_columns,
-                                    dtype=sequencing_summary_datatypes)
+                    return pd_read_sequencing_summary(f, cols=sequencing_summary_columns,
+                                    data_type=sequencing_summary_datatypes)
 
                 # check for presence of sequencing_summary file, if True add column read_id for merging with barcode dataframe
                 else:
                     if self._is_sequencing_summary_file(f):
                         sequencing_summary_columns.append('read_id')
                         sequencing_summary_datatypes.update(
                             {'read_id': object})
 
-                        dataframe = pd.read_csv(f, sep="\t", usecols=sequencing_summary_columns,
-                                                dtype=sequencing_summary_datatypes)
+                        dataframe = pd_read_sequencing_summary(f, cols=sequencing_summary_columns,
+                                                data_type=sequencing_summary_datatypes)
                         if summary_dataframe is None:
                             summary_dataframe = dataframe
                         else:
                             summary_dataframe = summary_dataframe.append(
                                 dataframe, ignore_index=True)
 
             if barcode_dataframe is None:
```

### Comparing `toulligqc-2.5.7/toulligqc/sequencing_summary_onedsquare_extractor.py` & `toulligqc-2.6/toulligqc/sequencing_summary_onedsquare_extractor.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/sequencing_telemetry_extractor.py` & `toulligqc-2.6/toulligqc/sequencing_telemetry_extractor.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc/toulligqc.py` & `toulligqc-2.6/toulligqc/toulligqc.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 import warnings
 from toulligqc import toulligqc_info_extractor
 from toulligqc import report_data_file_generator
 from toulligqc import html_report_generator
 from toulligqc import version
 from toulligqc import configuration
 from toulligqc import fast5_extractor
+from toulligqc import pod5_extractor
 from toulligqc import sequencing_summary_extractor
 from toulligqc import sequencing_summary_onedsquare_extractor
 from toulligqc import sequencing_telemetry_extractor
 from toulligqc import common
 from toulligqc import fastq_extractor
 from toulligqc import bam_extractor
 
@@ -79,14 +80,18 @@
                                'can be compressed with gzip (.gz) or bzip2 (.bz2)',
                           default=False)
 
     required.add_argument('-f', '--fast5-source', action='store', dest='fast5_source',
                           help='Fast5 file source (necessary if no telemetry file), ' +
                                'can also be in a tar.gz/tar.bz2 archive or a directory')
     
+    required.add_argument('-p', '--pod5-source', action='store', dest='pod5_source',
+                          help='pod5 file source (necessary if no telemetry file), ' +
+                               'can also be in a tar.gz/tar.bz2 archive or a directory')
+
     required.add_argument('-q', '--fastq', action='append', dest='fastq',
                           help='FASTQ file (necessary if no sequencing summary file), ' +
                                'can also be in a tar.gz archive')
     
     required.add_argument('-u', '--bam', action='append', dest='bam',
                           help='uBAM file (necessary if no sequencing summary file), ' +
                                'can also be in SAM format')
@@ -137,14 +142,15 @@
         config_dictionary['report_name'] = "Toulligqc-report-" + str((timestamp.strftime("%Y-%m-%d-%H%M%S")))
     else:
         config_dictionary['report_name'] = report_name
 
     # Rewrite the configuration file value if argument option is present
     args_dict = {
         ('fast5_source', args.fast5_source),
+        ('pod5_source', args.pod5_source),
         ('sequencing_summary_source', _join_parameter_arguments(args.sequencing_summary_source)),
         ('sequencing_summary_1dsqr_source', _join_parameter_arguments(args.sequencing_summary_1dsqr_source)),
         ('sequencing_telemetry_source', args.telemetry_source),
         ('fastq', _join_parameter_arguments(args.fastq)),
         ('bam', _join_parameter_arguments(args.bam)), 
         ('thread', args.thread),
         ('batch_size', args.batch_size),
@@ -291,14 +297,17 @@
     if 'sequencing_telemetry_source' in config_dictionary and \
             config_dictionary['sequencing_telemetry_source']:
         result.append(sequencing_telemetry_extractor.SequencingTelemetryExtractor(config_dictionary))
 
     if 'fast5_source' in config_dictionary and config_dictionary['fast5_source']:
         result.append(fast5_extractor.Fast5Extractor(config_dictionary))
 
+    if 'pod5_source' in config_dictionary and config_dictionary['pod5_source']:
+        result.append(pod5_extractor.Pod5Extractor(config_dictionary))
+
     if 'sequencing_summary_1dsqr_source' in config_dictionary and \
             config_dictionary['sequencing_summary_1dsqr_source']:
         result.append(sequencing_summary_onedsquare_extractor.
                       OneDSquareSequencingSummaryExtractor(config_dictionary))
     if 'fastq' in config_dictionary and \
             config_dictionary['fastq']:
         result.append(fastq_extractor.fastqExtractor(config_dictionary))
```

### Comparing `toulligqc-2.5.7/toulligqc/toulligqc_info_extractor.py` & `toulligqc-2.6/toulligqc/toulligqc_info_extractor.py`

 * *Files identical despite different names*

### Comparing `toulligqc-2.5.7/toulligqc.egg-info/PKG-INFO` & `toulligqc-2.6/toulligqc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toulligqc
-Version: 2.5.7
+Version: 2.6
 Summary: A post sequencing QC tool for Oxford Nanopore sequencers
 Home-page: https://github.com/GenomicParisCentre/toulligQC
 Author: Genomic Paris Centre team
 Author-email: toulligqc@biologie.ens.fr
 License: GPL V3
 Keywords: Nanopore MinION QC report
 Platform: ALL
```

### Comparing `toulligqc-2.5.7/toulligqc.egg-info/SOURCES.txt` & `toulligqc-2.6/toulligqc.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 toulligqc/fast5_extractor.py
 toulligqc/fastq_bam_common.py
 toulligqc/fastq_extractor.py
 toulligqc/html_report_generator.py
 toulligqc/plotly_graph_common.py
 toulligqc/plotly_graph_generator.py
 toulligqc/plotly_graph_onedsquare_generator.py
+toulligqc/pod5_extractor.py
 toulligqc/report_data_file_generator.py
 toulligqc/sequencing_summary_extractor.py
 toulligqc/sequencing_summary_onedsquare_extractor.py
 toulligqc/sequencing_telemetry_extractor.py
 toulligqc/toulligqc.py
 toulligqc/toulligqc_info_extractor.py
 toulligqc/version.py
```

