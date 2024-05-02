# Comparing `tmp/fisspy-1.0.9.tar.gz` & `tmp/fisspy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fisspy-1.0.9.tar", last modified: Sat Apr 27 07:31:22 2024, max compression
+gzip compressed data, was "fisspy-1.1.0.tar", last modified: Thu May  2 00:31:40 2024, max compression
```

## Comparing `fisspy-1.0.9.tar` & `fisspy-1.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.503118 fisspy-1.0.9/
--rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.9/LICENSE.txt
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-27 07:31:22.502918 fisspy-1.0.9/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.0.9/README.md
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.498249 fisspy-1.0.9/fisspy/
--rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-04-27 07:30:23.000000 fisspy-1.0.9/fisspy/__init__.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.499281 fisspy-1.0.9/fisspy/align/
--rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/align/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.0.9/fisspy/align/alignment.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.0.9/fisspy/align/base.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.500110 fisspy-1.0.9/fisspy/analysis/
--rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/analysis/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.0.9/fisspy/analysis/doppler.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/analysis/filter.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.0.9/fisspy/analysis/forecast.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/analysis/ofe.py
--rw-r--r--   0 jhkang     (501) staff       (20)    35498 2024-04-25 11:29:47.000000 fisspy-1.0.9/fisspy/analysis/tdmap.py
--rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.0.9/fisspy/analysis/wavelet.py
--rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.9/fisspy/cm.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.500484 fisspy-1.0.9/fisspy/correction/
--rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/correction/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/correction/correction.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/correction/get_inform.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.500903 fisspy-1.0.9/fisspy/data/
--rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.9/fisspy/data/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.9/fisspy/data/_sample.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.9/fisspy/data/download.py
--rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.9/fisspy/data/sample.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.501225 fisspy-1.0.9/fisspy/image/
--rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.0.9/fisspy/image/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    29769 2024-04-25 11:21:02.000000 fisspy-1.0.9/fisspy/image/interactive_image.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11762 2024-04-26 09:44:52.000000 fisspy-1.0.9/fisspy/image/raster_set.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.501431 fisspy-1.0.9/fisspy/inversion/
--rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/inversion/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/inversion/_mlsi.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.501677 fisspy-1.0.9/fisspy/io/
--rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.9/fisspy/io/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.9/fisspy/io/read.py
--rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/makevideo.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.502255 fisspy-1.0.9/fisspy/preprocess/
--rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/preprocess/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    52752 2024-04-27 05:54:30.000000 fisspy-1.0.9/fisspy/preprocess/proc_base.py
--rw-r--r--   0 jhkang     (501) staff       (20)   146943 2024-04-27 06:00:37.000000 fisspy-1.0.9/fisspy/preprocess/proc_gui.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/preprocess/t_y_sh.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.502613 fisspy-1.0.9/fisspy/read/
--rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.9/fisspy/read/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    49241 2024-04-26 03:08:29.000000 fisspy-1.0.9/fisspy/read/read_factory.py
--rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.0.9/fisspy/read/readbase.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-27 07:31:22.498945 fisspy-1.0.9/fisspy.egg-info/
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-27 07:31:22.000000 fisspy-1.0.9/fisspy.egg-info/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-04-27 07:31:22.000000 fisspy-1.0.9/fisspy.egg-info/SOURCES.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-27 07:31:22.000000 fisspy-1.0.9/fisspy.egg-info/dependency_links.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-27 07:31:22.000000 fisspy-1.0.9/fisspy.egg-info/not-zip-safe
--rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-04-27 07:31:22.000000 fisspy-1.0.9/fisspy.egg-info/requires.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-27 07:31:22.000000 fisspy-1.0.9/fisspy.egg-info/top_level.txt
--rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-27 07:31:22.503159 fisspy-1.0.9/setup.cfg
--rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-04-27 07:30:44.000000 fisspy-1.0.9/setup.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.488764 fisspy-1.1.0/
+-rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.1.0/LICENSE.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-02 00:31:40.488570 fisspy-1.1.0/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.1.0/README.md
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.483226 fisspy-1.1.0/fisspy/
+-rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-04-30 00:20:03.000000 fisspy-1.1.0/fisspy/__init__.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.484455 fisspy-1.1.0/fisspy/align/
+-rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/align/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.1.0/fisspy/align/alignment.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.1.0/fisspy/align/base.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.485333 fisspy-1.1.0/fisspy/analysis/
+-rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/analysis/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.1.0/fisspy/analysis/doppler.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/analysis/filter.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.1.0/fisspy/analysis/forecast.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/analysis/ofe.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    35498 2024-04-25 11:29:47.000000 fisspy-1.1.0/fisspy/analysis/tdmap.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.1.0/fisspy/analysis/wavelet.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.1.0/fisspy/cm.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.485753 fisspy-1.1.0/fisspy/correction/
+-rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/correction/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-05-01 13:33:13.000000 fisspy-1.1.0/fisspy/correction/correction.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-30 00:59:33.000000 fisspy-1.1.0/fisspy/correction/get_inform.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.486181 fisspy-1.1.0/fisspy/data/
+-rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.1.0/fisspy/data/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.1.0/fisspy/data/_sample.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.1.0/fisspy/data/download.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.1.0/fisspy/data/sample.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.486534 fisspy-1.1.0/fisspy/image/
+-rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.1.0/fisspy/image/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    30373 2024-05-01 08:46:52.000000 fisspy-1.1.0/fisspy/image/interactive_image.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12849 2024-05-01 06:38:35.000000 fisspy-1.1.0/fisspy/image/raster_set.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.486736 fisspy-1.1.0/fisspy/inversion/
+-rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/inversion/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/inversion/_mlsi.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.486970 fisspy-1.1.0/fisspy/io/
+-rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.1.0/fisspy/io/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.1.0/fisspy/io/read.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/makevideo.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.487536 fisspy-1.1.0/fisspy/preprocess/
+-rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/preprocess/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    52752 2024-04-27 05:54:30.000000 fisspy-1.1.0/fisspy/preprocess/proc_base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)   146937 2024-04-27 10:55:16.000000 fisspy-1.1.0/fisspy/preprocess/proc_gui.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/preprocess/t_y_sh.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.488274 fisspy-1.1.0/fisspy/read/
+-rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.1.0/fisspy/read/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    50267 2024-05-01 14:11:45.000000 fisspy-1.1.0/fisspy/read/read_factory.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.1.0/fisspy/read/readbase.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-02 00:31:40.484084 fisspy-1.1.0/fisspy.egg-info/
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/not-zip-safe
+-rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/requires.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-05-02 00:31:40.000000 fisspy-1.1.0/fisspy.egg-info/top_level.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-05-02 00:31:40.488810 fisspy-1.1.0/setup.cfg
+-rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-04-30 00:19:57.000000 fisspy-1.1.0/setup.py
```

### Comparing `fisspy-1.0.9/LICENSE.txt` & `fisspy-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/PKG-INFO` & `fisspy-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.0.9
+Version: 1.1.0
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.0.9/README.md` & `fisspy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/align/alignment.py` & `fisspy-1.1.0/fisspy/align/alignment.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/align/base.py` & `fisspy-1.1.0/fisspy/align/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/analysis/doppler.py` & `fisspy-1.1.0/fisspy/analysis/doppler.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/analysis/filter.py` & `fisspy-1.1.0/fisspy/analysis/filter.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/analysis/forecast.py` & `fisspy-1.1.0/fisspy/analysis/forecast.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/analysis/ofe.py` & `fisspy-1.1.0/fisspy/analysis/ofe.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/analysis/tdmap.py` & `fisspy-1.1.0/fisspy/analysis/tdmap.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/analysis/wavelet.py` & `fisspy-1.1.0/fisspy/analysis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/cm.py` & `fisspy-1.1.0/fisspy/cm.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/correction/correction.py` & `fisspy-1.1.0/fisspy/correction/correction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import absolute_import, division
 import numpy as np
 from ..align import alignOffset
-from .get_inform import LineName, centerWV, Pure
+from .get_inform import lineName, centerWV, Pure
 from scipy.signal import savgol_filter
 from scipy.ndimage import gaussian_filter1d
 
 __author__ = "Juhyung Kang"
 __email__ = "jhkang0301@gmail.com"
-__all__ = ["get_InstShift", "get_Linecenter", "wvCalib", "smoothingProf", "CorSLA", "CorStrayLight", "CorAsymmetry"]
+__all__ = ["get_InstShift", "get_Linecenter", "wvCalib", "smoothingProf", "corSLA", "corStrayLight", "corAsymmetry"]
 
 def get_InstShift(data, refSpec, dw):
     """
     Get offsert value of the instrumental shift caused by the seeing and vibration of the spectrograph.
 
     Parameters
     ----------
@@ -120,15 +120,15 @@
     wv: `~numpy.ndarray`
         Wavelength.
     """
     cwv = h['crval1']
     dwv = h['cdelt1']
     nwv = h['naxis1']
     nd = 5
-    name = LineName(cwv)
+    name = lineName(cwv)
 
     line = centerWV(name)
     
     wpix = np.arange(nwv)
     iwv = wvCalib_simple(h)
     w0 = iwv[profile.argmin()]
     wh = abs(iwv - w0) <= 0.3
@@ -151,15 +151,15 @@
     -------
     wv: `~numpy.ndarray`
         Wavelength.
     """
     cwv = h['crval1']
     nwv = h['naxis1']
     nds = [2,5]
-    name = LineName(cwv)
+    name = lineName(cwv)
     
     if name == 'Ha':
         lines = [6559.567, 6562.817]
         nds[1] = 6
     elif name == 'Ca':
         lines = [8536.165, 8542.091]
     elif name == 'Na':
@@ -247,15 +247,15 @@
                             delta=delta, cval=cval, mode=mode, axis=axis)
     elif method == 'gauss':
         sigma = kwargs.pop('sigma', 1)
         return gaussian_filter1d(data, sigma, axis=axis, **kwargs)
     else:
         raise ValueError("Input one of 'savgol' or 'gauss'")
 
-def CorSLA(wv, data, refProf, line, pure=None, eps=0.027, zeta=0.055):
+def corSLA(wv, data, refProf, line, pure=None, eps=0.027, zeta=0.055):
     """
     Correction of spectral line(s) profile for stray linght and far wing red-blue asymmetry.
 
     Parameters
     ----------
     wv: `~numpy.ndarray`, shape (N,)
         Absolute wavelengths in unit of Angstrom.
@@ -288,20 +288,20 @@
     CorStrayLight: correction for stray light.
     CorAsymmetry: correction for far wing red-blue asymmetry.
     """
     if pure is None:
         pp = Pure(wv, line)
     else:
         pp = pure
-    I = CorStrayLight(wv, data, refProf, line , pp, eps, zeta)
-    I = CorAsymmetry(wv, I, line, pp)
+    I = corStrayLight(wv, data, refProf, line , pp, eps, zeta)
+    I = corAsymmetry(wv, I, line, pp)
 
     return I
 
-def CorStrayLight(wv, data, refProf, line, pure=None, eps=0.027, zeta=0.055):
+def corStrayLight(wv, data, refProf, line, pure=None, eps=0.027, zeta=0.055):
     """
     Correction of spectral line(s) profile for stray linght.
 
     Parameters
     ----------
     wv: `~numpy.ndarray`, shape (N,)
         Absolute wavelengths in unit of Angstrom.
@@ -351,15 +351,15 @@
     # assume I_{c,obs}(0) \sim I_{c}(0)
     # data = I_{lambda,obs} 
     IC = (IC_obs[...,None]/IC_obs0-eps)/(1-eps)*IC_obs0
     I = (data/IC_obs[...,None] - zeta)/(1-zeta)*IC
 
     return I
 
-def CorAsymmetry(wv, data, line, pure=None):
+def corAsymmetry(wv, data, line, pure=None):
     """
     Correction of spectral line(s) profile for far wing red-blue asymmetry.
 
     Parameters
     ----------
     wv: `~numpy.ndarray`, shape (N,)
         Absolute wavelengths in unit of Angstrom.
@@ -390,12 +390,12 @@
     na = int(data.size/nw)
     I = data.reshape((na,nw)).T
 
     # correcting for far blue-red wings asymmetry
     wh_IC_red = pp * (abs(wv-cwv) > 3.9)*(abs(wv-cwv) < 4.5)
     coeff = np.polyfit(wv[wh_IC_red], I[wh_IC_red], 1)
     p = np.polyval(coeff, wv[:,None])
-    p /= np.maximum(p.mean(axis=1), 3e-2)[:,None]
+    p /= np.maximum(p.mean(axis=0), 3e-2)[None,:]
     cI = (I/p).T.reshape(sh)
 
     return cI
```

### Comparing `fisspy-1.0.9/fisspy/correction/get_inform.py` & `fisspy-1.1.0/fisspy/correction/get_inform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import absolute_import, division
 
-__all__ = ["LineName", "centerWV", "Pure"]
+__all__ = ["lineName", "centerWV", "Pure"]
 
-def LineName(cwv):
+def lineName(cwv):
     """
     Get name of the spectrum
 
     Parameter
     ---------
     cwv: `float`
         Centerl wavelength of the spectrum
```

### Comparing `fisspy-1.0.9/fisspy/data/_sample.py` & `fisspy-1.1.0/fisspy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/data/download.py` & `fisspy-1.1.0/fisspy/data/download.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/image/interactive_image.py` & `fisspy-1.1.0/fisspy/image/interactive_image.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,387 +13,414 @@
     """
     Draw interactive FISS raster, spectrogram and profile for single band.
 
     Parameters
     ----------
     fiss: `fisspy.read.FISS`
         FISS class.
-    X : `float`
+    x: `float`
         X position that you draw a spectral profile.
         Default is image center.
-    Y : `float`
+    y: `float`
         Y position that you draw a spectral profile.
         Default is image center.
-    WV : `float`
+    wv: `float`
         Wavelength positin that you draw a raster images.
         Default is central wavelength.
-    scale : `string`
+    scale: `string`
         Scale method of colarbar limit.
         Default is minMax.
         option: 'minMax', 'std', 'log'
-    sigFactor : `float`
+    sigFactor: `float`
         Factor of standard deviation.
         This is worked if scale is set to be 'std'
-    helpBox : `bool`
+    helpBox: `bool`
         Show the interacitve key and simple explanation.
         Default is True
 
     Other Parameters
     ----------------
-    **kwargs : `~matplotlib.pyplot` properties
+    **kwargs: `~matplotlib.pyplot` properties
     """
 
-    def __init__(self, fiss, X=None, Y=None, WV=None, scale='minMax',
-                 sigFactor=3, helpBox=True, **kwargs):
+    def __init__(self, fiss, x=None, y=None, wv=None, scale='log', sigFactor=2, helpBox=True, **kwargs):
 
         try:
             plt.rcParams['keymap.back'].remove('left')
             plt.rcParams['keymap.forward'].remove('right')
         except:
             pass
 
-        if not X:
-            x = fiss.nx//2*fiss.xDelt
-        if not Y:
-            y = fiss.ny//2*fiss.yDelt
-        if not WV:
-            wv = fiss.centralWavelength
+        if not x:
+            X = fiss.nx//2*fiss.xDelt
+        else:
+            X = x
+        if not y:
+            Y = fiss.ny//2*fiss.yDelt
+        else:
+            Y = y
+        if not wv:
+            WV = fiss.centralWavelength
+        else:
+            WV = wv
+
+        self.wave = fiss.wave
+        self.data = fiss.data
+        self.nx = fiss.nx
+        self.ny = fiss.ny
+        self.nwv = fiss.nwv
+        self.band = fiss.band
+        self.cam = fiss.cam
+        self.cwv = fiss.centralWavelength
+        self.dx = fiss.xDelt
+        self.dy = fiss.yDelt
+        self.dwv = fiss.wvDelt
         self.extentRaster = fiss.extentRaster
         self.extentSpectro = fiss.extentSpectro
         self.scale = scale
         self.sigFactor = sigFactor
         self.hw = kwargs.pop('hw', 0.05)
-        self.xpix = round((x-fiss.xDelt/2)/fiss.xDelt)
-        self.x = self.xpix*fiss.xDelt+fiss.xDelt/2
-        self.ypix = round((y-fiss.yDelt/2)/fiss.yDelt)
-        self.y = self.ypix*fiss.yDelt+fiss.yDelt/2
-        self.wv = wv
-        self.x0 = self.x
-        self.y0 = self.y
-        self.wv0 = self.wv
-        self.xH = self.x
-        self.yH = self.y
-        self.wvH = self.wv
-        self.centralWavelength = fiss.centralWavelength
-        self.xDelt = fiss.xDelt
-        self.yDelt = fiss.yDelt
-        self.wvDelt = fiss.wvDelt
-        self.wave = fiss.wave
-        self.data = fiss.data
-        self.band = fiss.band
-        self.cam = fiss.cam
-        self._xMin = self.extentRaster[0]
-        self._xMax = self.extentRaster[1]
-        self._yMin = self.extentRaster[2]
-        self._yMax = self.extentRaster[3]
-        self._wvMin = self.extentSpectro[0]
-        self._wvMax = self.extentSpectro[1]
+        self.xp = int(X/self.dx+0.5)
+        self.x = self.xp*self.dx
+        self.yp = int(Y/self.dy+0.5)
+        self.y = self.yp*self.dy
+        self.mwv = self.wave[0]
+        self.wv = WV
+        self.wvp = int((WV-self.mwv)/self.dwv+0.5)
+        self.xp0 = self.xp
+        self.yp0 = self.yp
+        self.wvp0 = self.wvp
+        self.xpH = self.xp
+        self.ypH = self.yp
+        self.wvpH = self.wvp
 
 
         #Keyboard helpBox
         if helpBox:
             helpFig = plt.figure('Keyboard Help Box', figsize=[3.5,3])
             ax = helpFig.add_subplot(111)
             ax.set_position([0,0,1,1])
             ax.set_axis_off()
-            ax.text(0.05,0.9,'ctrl/cmd+h: Reset to original setting')
-            ax.text(0.05,0.8,'ctrl/cmd+right: Move to right')
-            ax.text(0.05,0.7,'ctrl/cmd+left: Move to left')
-            ax.text(0.05,0.6,'ctrl/cmd+up: Move to up')
-            ax.text(0.05,0.5,'ctrl/cmd+down: Move to down')
-            ax.text(0.05,0.4,'right: Increase the wavelength')
-            ax.text(0.05,0.3,'left: Decrease the wavelength')
+            ax.text(0.05,0.8,'right: Move to right')
+            ax.text(0.05,0.7,'left: Move to left')
+            ax.text(0.05,0.6,'up: Move to up')
+            ax.text(0.05,0.5,'down: Move to down')
             ax.text(0.05,0.2,'spacebar: Change to current mouse point')
+            ax.text(0.05,0.9,'ctrl/cmd+h: Reset to original setting position')
+            ax.text(0.05,0.4,'ctrl/cmd+right: Increase the wavelength')
+            ax.text(0.05,0.3,'ctrl/cmd+left: Decrease the wavelength')
             ax.text(0.05,0.1,'ctrl/cmd+b: Show previous point')
+            helpFig.show()
 
 
         #figure setting
         figsize = kwargs.pop('figsize', [15, 9])
         self.cmap = kwargs.pop('cmap', fiss.cmap)
         self.fig = plt.figure(figsize=figsize)
         # self.fig.canvas.set_window_title(self.band)
-        self.imInterp = kwargs.get('interpolation', fiss.imInterp)
+        kwargs['interpolation'] = kwargs.pop('interpolation', 'bilinear')
         gs = gridspec.GridSpec(2, 3)
         self.axRaster = self.fig.add_subplot(gs[:, 0])
         self.axSpectro = self.fig.add_subplot(gs[0, 1:])
         self.axProfile = self.fig.add_subplot(gs[1, 1:])
         fiss.axRaster = self.axRaster
         fiss.axSpectro = self.axSpectro
         fiss.axProfile = self.axProfile
         self.axRaster.set_xlabel('X (arcsec)')
         self.axRaster.set_ylabel('Y (arcsec)')
         self.axSpectro.set_xlabel(r'Wavelength ($\AA$)')
         self.axSpectro.set_ylabel('Y (arcsec)')
         self.axProfile.set_xlabel(r'Wavelength ($\AA$)')
         self.axProfile.set_ylabel('Intensity (Count)')
         self.axRaster.set_title(fiss.date)
-        self.axSpectro.set_title(r"X = %.2f'', Y = %.2f'' (X$_{pix}$ = %i, Y$_{pix}$ = %i)"%(self.x, self.y, self.xpix, self.ypix))
+        self.axSpectro.set_title(r"X = %.2f'', Y = %.2f'' (X$_{pix}$ = %i, Y$_{pix}$ = %i)"%(self.x, self.y, self.xp, self.yp))
         self.axRaster.set_xlim(fiss.extentRaster[0], fiss.extentRaster[1])
         self.axRaster.set_ylim(fiss.extentRaster[2], fiss.extentRaster[3])
         self.axSpectro.set_xlim(fiss.extentSpectro[0], fiss.extentSpectro[1])
         self.axSpectro.set_ylim(fiss.extentSpectro[2], fiss.extentSpectro[3])
         self.axProfile.set_title(r'%s Band (wv = %.2f $\AA$)'%(fiss.band, self.wv))
         self.axProfile.set_xlim(fiss.wave.min(), fiss.wave.max())
-        self.axProfile.set_ylim(self.data[self.ypix, self.xpix].min()-100,
-                                self.data[self.ypix, self.xpix].max()+100)
+        ym = self.data[self.yp, self.xp].min()
+        yM = self.data[self.yp, self.xp].max()
+        margin = (yM-ym)*0.05
+        self.axProfile.set_ylim(ym-margin, yM+margin)
         self.axProfile.minorticks_on()
         self.axProfile.tick_params(which='both', direction='in')
 
 
         # Draw
-        raster = _getRaster(self.data, self.wave, self.wv, self.wvDelt,
-                            hw=self.hw)
-
+        raster = _getRaster(self.data, self.wave, self.wv, self.dwv, hw=self.hw)
+        M = raster.max()
+        if M > 1e2:
+            m = raster[raster > 1e2].min()
+        else:
+            m = raster.min()
         if self.cam == 'A':
-            spectro = self.data[:, self.xpix]
+            spectro = self.data[:, self.xp]
         elif self.cam == 'B':
-            spectro = self.data[:, self.xpix,::-1]
+            spectro = self.data[:, self.xp,::-1]
         if self.scale == 'log':
             raster = np.log10(raster)
             spectro = np.log10(spectro)
-        self.imRaster = self.axRaster.imshow(raster,
-                                             fiss.cmap,
-                                             origin='lower',
-                                             extent=fiss.extentRaster,
-                                             **kwargs)
-        self.imSpectro = self.axSpectro.imshow(spectro,
-                                               fiss.cmap,
-                                               origin='lower',
-                                               extent=fiss.extentSpectro,
-                                               **kwargs)
-        self.plotProfile = self.axProfile.plot(self.wave,
-                                               self.data[self.ypix, self.xpix],
-                                               color='k')[0]
+            M = np.log10(M)
+            m = np.log10(m)
+        self.imRaster = self.axRaster.imshow(raster, fiss.cmap, origin='lower', extent=fiss.extentRaster, **kwargs)
+        self.imSpectro = self.axSpectro.imshow(spectro, fiss.cmap, origin='lower', extent=fiss.extentSpectro, **kwargs)
+        self.plotProfile = self.axProfile.plot(self.wave, self.data[self.yp, self.xp], color='k')[0]
 
         if self.scale == 'std':
-            self.imRaster.set_clim(np.median(raster)-raster.std()*self.sigFactor,
-                                   np.median(raster)+raster.std()*self.sigFactor)
-            self.imSpectro.set_clim(np.median(spectro)-spectro.std()*self.sigFactor,
-                                    np.median(spectro)+spectro.std()*self.sigFactor)
+            self.imRaster.set_clim(np.median(raster)-raster.std()*self.sigFactor, np.median(raster)+raster.std()*self.sigFactor)
+            self.imSpectro.set_clim(spectro.min(), spectro.max())
         else:
-            self.imRaster.set_clim(raster.min(), raster.max())
+            self.imRaster.set_clim(m, M)
             self.imSpectro.set_clim(spectro.min(), spectro.max())
 
         # Reference
-        self.vlineRaster = self.axRaster.axvline(self.x,
-                                                 linestyle='dashed',
-                                                 color='lime')
-        self.vlineProfile = self.axProfile.axvline(self.wv,
-                                                   ls='dashed',
-                                                   c='b')
-        self.vlineSpectro = self.axSpectro.axvline(self.wv,
-                                                   ls='dashed',
-                                                   c='lime')
-        self.hlineSpectro = self.axSpectro.axhline(self.y,
-                                                   ls='dashed',
-                                                   c='lime')
-        self.pointRaster = self.axRaster.scatter(self.x, self.y, 50,
-                                                 marker='x',
-                                                 color='r')
+        self.vlineRaster = self.axRaster.axvline(self.x, linestyle='dashed', color='lime')
+        self.vlineProfile = self.axProfile.axvline(self.wv, ls='dashed', c='b')
+        self.vlineSpectro = self.axSpectro.axvline(self.wv, ls='dashed', c='lime')
+        self.hlineSpectro = self.axSpectro.axhline(self.y, ls='dashed', c='lime')
+        self.pointRaster = self.axRaster.scatter(self.x, self.y, 50, marker='x', color='r')
         self.axSpectro.set_aspect(adjustable='box', aspect='auto')
         self.fig.tight_layout()
-        self.fig.canvas.mpl_connect('key_press_event', self._on_key)
+        self.fig.canvas.mpl_connect('key_press_event', self._onKey)
 
         self.fig.show()
 
-    def _on_key(self, event):
-
-        ### Interactive keyboard input
-        # Position
-        if event.key == 'ctrl+right' or event.key == 'cmd+right':
-            if self.x < self._xMax:
-                self.x += self.xDelt
-            else:
-                self.x = self._xMin
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == 'ctrl+left' or event.key == 'cmd+left':
-            if self.x > self._xMin:
-                self.x -= self.xDelt
+    def _onKey(self, event):
+        if event.key == 'right':
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvp0 = self.wvp
+            if self.xp < self.nx-1:
+                self.xp += 1
             else:
-                self.x = self._xMax
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == 'ctrl+up' or event.key == 'cmd+up':
-            if self.y < self._yMax:
-                self.y += self.yDelt
+                self.xp = 0
+            self.x = self.xp*self.dx
+            self._chSpect()
+        elif event.key == 'left':
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvp0 = self.wvp
+            if self.xp > 0:
+                self.xp -= 1
             else:
-                self.y = self._yMin
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == 'ctrl+down' or event.key == 'cmd+down':
-            if self.y > self._yMin:
-                self.y -= self.yDelt
+                self.xp = self.nx-1
+            self.x = self.xp*self.dx
+            self._chSpect()
+        elif event.key == 'up':
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvp0 = self.wvp
+            if self.yp < self.ny-1:
+                self.yp += 1
             else:
-                self.y = self._yMax
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == 'right':
-            if self.wv < self._wvMax:
-                self.wv += abs(self.wvDelt)
-            else:
-                self.wv = self._wvMin
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
-        elif event.key == 'left':
-            if self.wv > self._wvMin:
-                self.wv -= abs(self.wvDelt)
+                self.yp = 0
+            self.y = self.yp*self.dy
+            self._chSpect()
+        elif event.key == 'down':
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvp0 = self.wvp
+            if self.yp > 0:
+                self.yp -= 1
+            else:
+                self.yp = self.ny-1
+            self.y = self.yp*self.dy
+            self._chSpect()
+        elif event.key == 'ctrl+right' or event.key == 'cmd+right':
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvp0 = self.wvp
+            if self.wvp < self.nwv-1:
+                self.wvp += 1
             else:
-                self.wv = self._wvMax
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
+                self.wvp = 0
+            self.wv = self.wvp*self.dwv+self.mwv
+            self._chRaster()
+        elif event.key == 'ctrl+left' or event.key == 'cmd+left':
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvp0 = self.wvp
+            if self.wvp > 0:
+                self.wvp -= 1
+            else:
+                self.wvp = self.nwv-1
+            self.wv = self.wvp*self.dwv+self.mwv
+            self._chRaster()
         elif event.key == ' ' and event.inaxes == self.axRaster:
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvp0 = self.wvp
             self.x = event.xdata
             self.y = event.ydata
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvb = self.wv0
+            self.xp = int(self.x/self.dx+0.5)
+            self.yp = int(self.y/self.dy+0.5)
+            self.x = self.xp*self.dx
+            self.y = self.yp*self.dy
+            self._chSpect()
         elif event.key == ' ' and event.inaxes == self.axProfile:
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvp0 = self.wvp
             self.wv = event.xdata
-            self.wvb = self.wv0
-            self.xb = self.x0
-            self.yb = self.y0
+            self.wvp = int((self.wv-self.mwv)/self.dwv+0.5)
+            self.wv = self.wvp*self.dwv+self.mwv
+            self._chRaster()
         elif event.key == ' ' and event.inaxes == self.axSpectro:
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvp0 = self.wvp
             self.wv = event.xdata
+            self.wvp = int((self.wv-self.mwv)/self.dwv+0.5)
+            self.wv = self.wvp*self.dwv+self.mwv
             self.y = event.ydata
-            self.wvb = self.wv0
-            self.xb = self.x0
-            self.yb = self.y0
+            self.yp = int(self.y/self.dy+0.5)
+            self.y = self.yp*self.dy
+            self._chRaster()
+            self._chSpect()
         elif event.key == 'ctrl+h' or event.key == 'cmd+h':
-            self.wv = self.wvH
-            self.x = self.xH
-            self.y = self.yH
-        elif event.key == 'ctrl+b' or event.key == 'cmd+b':
-            x = self.x
-            y = self.y
-            wv = self.wv
-            self.x = self.xb
-            self.y = self.yb
-            self.wv = self.wvb
-            self.xb = x
-            self.yb = y
-            self.wvb = wv
-        if self.x != self.x0 or self.y != self.y0:
-            self.xpix = int(round((self.x-self.xDelt/2)/self.xDelt))
-            self.ypix = int(round((self.y-self.yDelt/2)/self.yDelt))
+            self.wvp0 = self.wvp
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvp = self.wvpH
+            self.xp = self.xpH
+            self.yp = self.ypH
+            self.x = self.xp*self.dx
+            self.y = self.yp*self.dy
+            self.wv = self.wvp*self.dwv+self.mwv
+            self._chRaster()
             self._chSpect()
-        if self.wv != self.wv0:
+        elif event.key == 'ctrl+b' or event.key == 'cmd+b':
+            x = self.xp
+            y = self.yp
+            wv = self.wvp
+            self.xp = self.xp0
+            self.yp = self.yp0
+            self.wvp = self.wvp0
+            self.x = self.xp*self.dx
+            self.y = self.yp*self.dy
+            self.wv = self.wvp*self.dwv+self.mwv
             self._chRaster()
-        self.fig.canvas.draw_idle()
-
-
+            self._chSpect()
+            self.xp0 = x
+            self.yp0 = y
+            self.wvp0 = wv
+            
     def _chRaster(self):
-        self.wv0 = self.wv
-        raster = _getRaster(self.data, self.wave, self.wv, self.wvDelt,
-                             hw=self.hw)
+        raster = _getRaster(self.data, self.wave, self.wv, self.dwv, hw=self.hw)
+        M = raster.max()
+        if M > 1e2:
+            m = raster[raster > 1e2].min()
+        else:
+            m = raster.min()
         if self.scale == 'log':
             raster = np.log10(raster)
+            m = np.log10(m)
+            M = np.log10(M)
         self.imRaster.set_data(raster)
         self.vlineProfile.set_xdata(self.wv)
         self.vlineSpectro.set_xdata(self.wv)
         self.axProfile.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.band, self.wv))
         if self.scale == 'std':
-            self.imRaster.set_clim(np.median(raster)-raster.std()*self.sigFactor,
-                                   np.median(raster)+raster.std()*self.sigFactor)
+            self.imRaster.set_clim(np.median(raster)-raster.std()*self.sigFactor, np.median(raster)+raster.std()*self.sigFactor)
         else:
-            self.imRaster.set_clim(raster.min(), raster.max())
+            self.imRaster.set_clim(m, M)
+        self.fig.canvas.draw_idle()
 
     def _chSpect(self):
-        self.x0 = self.x
-        self.y0 = self.y
-
         if self.cam == 'A':
-            spectro = self.data[:, self.xpix]
+            spectro = self.data[:, self.xp]
         elif self.cam == 'B':
-            spectro = self.data[:, self.xpix,::-1]
+            spectro = self.data[:, self.xp,::-1]
         if self.scale == 'log':
             spectro = np.log10(spectro)
-        self.plotProfile.set_ydata(self.data[self.ypix, self.xpix])
+        self.plotProfile.set_ydata(self.data[self.yp, self.xp])
         self.imSpectro.set_data(spectro)
         self.hlineSpectro.set_ydata(self.y)
         self.vlineRaster.set_xdata(self.x)
         self.pointRaster.set_offsets([self.x, self.y])
 
-        self.axProfile.set_ylim(self.data[self.ypix, self.xpix].min()-100,
-                                self.data[self.ypix, self.xpix].max()+100)
-        self.axSpectro.set_title(r"X = %.2f'', Y = %.2f'' (X$_{pix}$ = %i, Y$_{pix}$ = %i)"%(self.x, self.y, self.xpix, self.ypix))
-        if self.scale == 'std':
-            self.imSpectro.set_clim(np.median(spectro)-spectro.std()*self.sigFactor,
-                                    np.median(spectro)+spectro.std()*self.sigFactor)
-        else:
-            self.imSpectro.set_clim(spectro.min(), spectro.max())
+        ym = self.data[self.yp, self.xp].min()
+        yM = self.data[self.yp, self.xp].max()
+        margin = (yM-ym)*0.05
+        self.axProfile.set_ylim(ym-margin, yM+margin)
+        self.axSpectro.set_title(r"X = %.2f'', Y = %.2f'' (X$_{pix}$ = %i, Y$_{pix}$ = %i)"%(self.x, self.y, self.xp, self.yp))
+        self.imSpectro.set_clim(spectro.min(), spectro.max())
+        self.fig.canvas.draw_idle()
 
     def chRasterClim(self, cmin, cmax):
         self.imRaster.set_clim(cmin, cmax)
+        self.fig.canvas.draw_idle()
 
     def chSpectroClim(self, cmin, cmax):
         self.imSpectro.set_clim(cmin, cmax)
+        self.fig.canvas.draw_idle()
 
     def chcmap(self, cmap):
         self.imRaster.set_cmap(cmap)
         self.imSpectro.set_cmap(cmap)
+        self.fig.canvas.draw_idle()
 
 class dualBand:
     """
     Draw interactive FISS raster, spectrogram and profile for dual band.
 
     Parameters
     ----------
     fissA: `fisspy.read.FISS`
         FISS class.
     fissB: `fisspy.read.FISS`
         FISS class.
-    x : `float`
+    x: `float`
         X position that you draw a spectral profile.
         Default is image center.
-    y : `float`
+    y: `float`
         Y position that you draw a spectral profile.
         Default is image center.
-    wvA : `float`
+    wvA: `float`
         Wavelength positin that you draw a raster images.
         Default is central wavelength.
-    wvB : `float`
+    wvB: `float`
         Wavelength positin that you draw a raster images.
         Default is central wavelength.
-    scale : `string`
+    scale: `string`
         Scale method of colarbar limit.
         Default is minMax.
         option: 'minMax', 'std', 'log'
-    sigFactor : `float`
+    sigFactor: `float`
         Factor of standard deviation.
         This is worked if scale is set to be 'std'
-    helpBox : `bool`
+    helpBox: `bool`
         Show the interacitve key and simple explanation.
         Default is True
 
     Other Parameters
     ----------------
     **kwargs : `~matplotlib.pyplot` properties
     """
-    def __init__(self, fissA, fissB, X=None, Y=None, WVA=None, WVB=None,
+    def __init__(self, fissA, fissB, x=None, y=None, wvA=None, wvB=None,
                  scale='minMax', sigFactor=3, helpBox=True, **kwargs):
 
         try:
             plt.rcParams['keymap.back'].remove('left')
             plt.rcParams['keymap.forward'].remove('right')
         except:
             pass
         from ..align import alignOffset, shiftImage3D
         kwargs['interpolation'] = kwargs.pop('interpolation', 'bilinear')
         self.fissA = fissA
         self.fissB = fissB
         self.nx = self.fissA.nx
-        self.xDelt = self.fissA.xDelt
-        self.yDelt = self.fissA.yDelt
+        self.nwvA = self.fissA.nwv
+        self.nwvB = self.fissB.nwv
+        self.dx = self.fissA.xDelt
+        self.dy = self.fissA.yDelt
+        self.dwvA = self.fissA.wvDelt
+        self.dwvB = self.fissB.wvDelt
         if self.fissA.ny >= self.fissB.ny:
             self.fissA.data = self.fissA.data[:self.fissB.ny]
             self.ny = self.fissB.ny
             self.extentRaster = self.fissB.extentRaster
         elif fissA.ny < fissB.ny:
             self.fissB.data = self.fissB.data[:self.fissA.ny]
             self.ny = self.fissA.ny
@@ -403,69 +430,79 @@
         self._yMin = self.extentRaster[2]
         self._yMax = self.extentRaster[3]
 
         sh = alignOffset(self.fissB.data[:,:,50], self.fissA.data[:,:,-50])
         tmp = shiftImage3D(fissB.data.transpose(2, 0, 1), -sh).transpose(1,2,0)
         self.fissB.data = tmp
         tmp[tmp<10]=1
-        del tmp
 
-        if not X:
-            x = self.nx//2*self.xDelt
-        if not Y:
-            y = self.ny//2*self.yDelt
-        if not WVA:
-            wvA = self.fissA.centralWavelength
-        if not WVB:
-            wvB = self.fissB.centralWavelength
-        xpix = round((x-self.xDelt/2)/self.xDelt)
-        ypix = round((y-self.yDelt/2)/self.yDelt)
-        self.x = xpix*self.xDelt+self.xDelt/2
-        self.y = ypix*self.yDelt+self.yDelt/2
+        if not x:
+            X = self.nx//2*self.dx
+        else:
+            X = x
+        if not y:
+            Y = self.ny//2*self.dy
+        else:
+            Y = y
+        if not wvA:
+            WVA = self.fissA.centralWavelength
+        else:
+            WVA = wvA
+        if not wvB:
+            WVB = self.fissB.centralWavelength
+        else:
+            WVB = wvB
+        self.xp = xp = int(X/self.dx+0.5)
+        self.yp = yp = int(Y/self.dy+0.5)
+        self.x = xp*self.dx
+        self.y = yp*self.dy
         self.scale = scale
         self.sigFactor = sigFactor
         self.hw = kwargs.pop('hw', 0.05)
-        self.wvA = wvA
-        self.wvB = wvB
-        self.x0 = self.x
-        self.y0 = self.y
-        self.wvA0 = self.wvA
-        self.wvB0 = self.wvB
-        self.xH = self.x
-        self.yH = self.y
-        self.wvAH = self.wvA
-        self.wvBH = self.wvB
+        self.wvA = WVA
+        self.wvB = WVB
+        self.mwvA = self.fissA.wave[0]
+        self.mwvB = self.fissB.wave[0]
+        self.wvpA = int((WVA-self.mwvA)/self.dwvA+0.5)
+        self.wvpB = int((WVB-self.mwvB)/self.dwvB+0.5)
+        self.xp0 = self.xp
+        self.yp0 = self.yp
+        self.wvpA0 = self.wvpA
+        self.wvpB0 = self.wvpB
+        self.xpH = self.xp
+        self.ypH = self.yp
+        self.wvpAH = self.wvpA
+        self.wvpBH = self.wvpB
 
         #Keyboard helpBox
         if helpBox:
-            helpFig = plt.figure('Keyboard Help Box', figsize=[3.5,3])
+            helpFig = plt.figure('Keyboard Help Box', figsize=[5,3])
             ax = helpFig.add_subplot(111)
             ax.set_position([0,0,1,1])
             ax.set_axis_off()
             ax.text(0.05,0.92,'ctrl+h: Reset to original setting')
-            ax.text(0.05,0.82,'ctrl+right: Move to right')
-            ax.text(0.05,0.72,'ctrl+left: Move to left')
-            ax.text(0.05,0.62,'ctrl+up: Move to up')
-            ax.text(0.05,0.52,'ctrl+down: Move to down')
-            ax.text(0.05,0.42,'right: Increase the wavelength of the fissA')
-            ax.text(0.05,0.32,'left: Decrease the wavelength of the fissA')
-            ax.text(0.05,0.22,'up: Increase the wavelength of the fissB')
-            ax.text(0.05,0.12,'down: Decrease the wavelength of the fissB')
+            ax.text(0.05,0.82,'right: Move to right')
+            ax.text(0.05,0.72,'left: Move to left')
+            ax.text(0.05,0.62,'up: Move to up')
+            ax.text(0.05,0.52,'down: Move to down')
+            ax.text(0.05,0.42,'ctrl/cmd+right: Increase the wavelength of the fissA')
+            ax.text(0.05,0.32,'ctrl/cmd+left: Decrease the wavelength of the fissA')
+            ax.text(0.05,0.22,'ctrl/cmd+up: Increase the wavelength of the fissB')
+            ax.text(0.05,0.12,'ctrl/cmd+down: Decrease the wavelength of the fissB')
             ax.text(0.05,0.02,'spacebar: Change to current mouse point')
+            helpFig.show()
 
         #figure setting
         figsize = kwargs.pop('figsize', [12, 6])
         self.fig = plt.figure(figsize=figsize)
         # self.fig.canvas.set_window_title('Dual Band Image')
         self.imInterp = kwargs.get('interpolation', 'bilinear')
         gs = gridspec.GridSpec(2,4)
         self.axRasterA = self.fig.add_subplot(gs[:,0])
-        self.axRasterB = self.fig.add_subplot(gs[:,1],
-                                              sharex=self.axRasterA,
-                                              sharey=self.axRasterA)
+        self.axRasterB = self.fig.add_subplot(gs[:,1], sharex=self.axRasterA, sharey=self.axRasterA)
         self.axProfileA = self.fig.add_subplot(gs[0,2:])
         self.axProfileB = self.fig.add_subplot(gs[1,2:])
         self.axRasterA.set_xlabel('X (arcsec)')
         self.axRasterA.set_ylabel('Y (arcsec)')
         self.axRasterB.set_xlabel('X (arcsec)')
         self.axRasterB.set_ylabel('Y (arcsec)')
         self.axProfileA.set_xlabel(r'Wavelength ($\AA$)')
@@ -478,246 +515,276 @@
         self.axProfileB.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissB.band, self.wvB))
         self.axRasterA.set_xlim(self.extentRaster[0], self.extentRaster[1])
         self.axRasterB.set_xlim(self.extentRaster[0], self.extentRaster[1])
         self.axRasterA.set_ylim(self.extentRaster[2], self.extentRaster[3])
         self.axRasterB.set_ylim(self.extentRaster[2], self.extentRaster[3])
         self.axProfileA.set_xlim(self.fissA.wave.min(), self.fissA.wave.max())
         self.axProfileB.set_xlim(self.fissB.wave.min(), self.fissB.wave.max())
-        self.axProfileA.set_ylim(self.fissA.data[ypix, xpix].min()-100,
-                                 self.fissA.data[ypix, xpix].max()+100)
-        self.axProfileB.set_ylim(self.fissB.data[ypix, xpix].min()-100,
-                                 self.fissB.data[ypix, xpix].max()+100)
+        ym = self.fissA.data[self.yp, self.xp].min()
+        yM = self.fissA.data[self.yp, self.xp].max()
+        margin = (yM-ym)*0.05
+        self.axProfileA.set_ylim(ym-margin, yM+margin)
+        ym = self.fissB.data[self.yp, self.xp].min()
+        yM = self.fissB.data[self.yp, self.xp].max()
+        margin = (yM-ym)*0.05
+        self.axProfileB.set_ylim(ym-margin, yM+margin)
         self.axProfileA.minorticks_on()
         self.axProfileA.tick_params(which='both', direction='in')
         self.axProfileB.minorticks_on()
         self.axProfileB.tick_params(which='both', direction='in')
 
         #Draw
-        rasterA = _getRaster(self.fissA.data, self.fissA.wave, self.wvA,
-                             self.fissA.wvDelt, hw=self.hw)
-        rasterB = _getRaster(self.fissB.data, self.fissB.wave, self.wvB,
-                             self.fissB.wvDelt, hw=self.hw)
+        rasterA = _getRaster(self.fissA.data, self.fissA.wave, self.wvA, self.dwvA, hw=self.hw)
+        rasterB = _getRaster(self.fissB.data, self.fissB.wave, self.wvB, self.dwvB, hw=self.hw)
+
+        MA = rasterA.max()
+        if MA > 1e2:
+            mA = rasterA[rasterA > 1e2].min()
+        else:
+            mA = rasterA.min()
+        MB = rasterB.max()
+        if MB > 1e2:
+            mB = rasterB[rasterB > 1e2].min()
+        else:
+            mB = rasterB.min()
 
-        whA = rasterA > 5
-        whB = rasterB > 5
         if self.scale == 'log':
             rasterA = np.log10(rasterA)
             rasterB = np.log10(rasterB)
-        cminA = rasterB[whA].min()
-        cminB = rasterB[whB].min()
-        self.imRasterA = self.axRasterA.imshow(rasterA,
-                                               self.fissA.cmap,
-                                               origin='lower',
-                                               extent=self.extentRaster,
-                                               **kwargs)
-        self.imRasterB = self.axRasterB.imshow(rasterB,
-                                               self.fissB.cmap,
-                                               origin='lower',
-                                               extent=self.extentRaster,
-                                               **kwargs)
-        self.plotProfileA = self.axProfileA.plot(self.fissA.wave,
-                                                 self.fissA.data[ypix, xpix],
-                                                 color='k')[0]
-        self.plotProfileB = self.axProfileB.plot(self.fissB.wave,
-                                                 self.fissB.data[ypix, xpix],
-                                                 color='k')[0]
+            MA = np.log10(MA)
+            mA = np.log10(mA)
+            MB = np.log10(MB)
+            mB = np.log10(mB)
+        
+        self.imRasterA = self.axRasterA.imshow(rasterA, self.fissA.cmap, origin='lower', extent=self.extentRaster, **kwargs)
+        self.imRasterB = self.axRasterB.imshow(rasterB, self.fissB.cmap, origin='lower', extent=self.extentRaster, **kwargs)
+        self.plotProfileA = self.axProfileA.plot(self.fissA.wave, self.fissA.data[yp, xp], color='k')[0]
+        self.plotProfileB = self.axProfileB.plot(self.fissB.wave, self.fissB.data[yp, xp], color='k')[0]
 
         if self.scale == 'std':
-            self.imRasterA.set_clim(np.median(rasterA)-rasterA.std()*self.sigFactor,
-                                    np.median(rasterA)+rasterA.std()*self.sigFactor)
-            self.imRasterB.set_clim(np.median(rasterB)-rasterB.std()*self.sigFactor,
-                                    np.median(rasterB)+rasterB.std()*self.sigFactor)
+            self.imRasterA.set_clim(np.median(rasterA)-rasterA.std()*self.sigFactor, np.median(rasterA)+rasterA.std()*self.sigFactor)
+            self.imRasterB.set_clim(np.median(rasterB)-rasterB.std()*self.sigFactor, np.median(rasterB)+rasterB.std()*self.sigFactor)
         else:
-            self.imRasterA.set_clim(cminA, rasterA.max())
-            self.imRasterB.set_clim(cminB, rasterB.max())
+            self.imRasterA.set_clim(mA, MA)
+            self.imRasterB.set_clim(mB, MB)
 
         #Reference
-        self.vlineProfileA = self.axProfileA.axvline(self.wvA,
-                                                     ls='dashed',
-                                                     c='b')
-        self.vlineProfileB = self.axProfileB.axvline(self.wvB,
-                                                     ls='dashed',
-                                                     c='b')
-        self.pointRasterA = self.axRasterA.scatter(self.x, self.y, 50,
-                                                   marker='x',
-                                                   color='r')
-        self.pointRasterB = self.axRasterB.scatter(self.x, self.y, 50,
-                                                   marker='x',
-                                                   color='r')
+        self.vlineProfileA = self.axProfileA.axvline(self.wvA, ls='dashed', c='b')
+        self.vlineProfileB = self.axProfileB.axvline(self.wvB, ls='dashed', c='b')
+        self.pointRasterA = self.axRasterA.scatter(self.x, self.y, 50, marker='x', color='r')
+        self.pointRasterB = self.axRasterB.scatter(self.x, self.y, 50, marker='x', color='r')
         self.fig.tight_layout()
-        self.fig.canvas.mpl_connect('key_press_event', self._on_key)
+        self.fig.canvas.mpl_connect('key_press_event', self._onKey)
         self.fig.show()
 
-    def _on_key(self, event):
+    def _onKey(self, event):
 
-        if event.key == 'ctrl+right' or event.key == 'cmd+right':
-            if self.x < self._xMax:
-                self.x += self.xDelt
-            else:
-                self.x = self._xMin+self.xDelt//2
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'ctrl+left' or event.key == 'cmd+left':
-            if self.x > self._xMin:
-                self.x -= self.xDelt
-            else:
-                self.x = self._xMax-self.xDelt//2
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'ctrl+up' or event.key == 'cmd+up':
-            if self.y < self._yMax:
-                self.y += self.yDelt
+        if event.key == 'right':
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
+            if self.xp < self.nx-1:
+                self.xp += 1
             else:
-                self.y = self._yMin+self.yDelt//2
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'ctrl+down' or event.key == 'cmd+down':
-            if self.y > self._yMin:
-                self.y -= self.yDelt
-            else:
-                self.y = self._yMax-self.yDelt//2
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == 'right':
-            if self.wvA < self.fissA.wave.max():
-                self.wvA += abs(self.fissA.wvDelt)
-            else:
-                self.wvA = self.fissA.wave.min()
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
+                self.xp = 0
+            self.x = self.xp*self.dx
+            self._chSpect()
         elif event.key == 'left':
-            if self.wvA > self.fissA.wave.min():
-                self.wvA -= abs(self.fissA.wvDelt)
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
+            if self.xp > 0:
+                self.xp -= 1
             else:
-                self.wvA = self.fissA.wave.max()
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
+                self.xp = self.nx-1
+            self.x = self.xp*self.dx
+            self._chSpect()
         elif event.key == 'up':
-            if self.wvB < self.fissB.wave.max():
-                self.wvB += abs(self.fissB.wvDelt)
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
+            if self.yp < self.ny-1:
+                self.yp += 1
             else:
-                self.wvB = self.fissB.wave.min()
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
+                self.yp = 0
+            self.y = self.yp*self.dy
+            self._chSpect()
         elif event.key == 'down':
-            if self.wvB > self.fissB.wave.min():
-                self.wvB -= abs(self.fissB.wvDelt)
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
+            if self.yp > 0:
+                self.yp -= 1
+            else:
+                self.yp = self.ny-1
+            self.y = self.yp*self.dy
+            self._chSpect()
+        elif event.key == 'ctrl+right' or event.key == 'cmd+right':
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
+            if self.wvpA < self.nwvA-1:
+                self.wvpA += 1
+            else:
+                self.wvpA = 0
+            self.wvA = self.wvpA*self.dwvA+self.mwvA
+            self._chRasterA()
+        elif event.key == 'ctrl+left' or event.key == 'cmd+left':
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
+            if self.wvpA > 0:
+                self.wvpA -= 1
+            else:
+                self.wvpA = self.nwvA-1
+            self.wvA = self.wvpA*self.dwvA+self.mwvA
+            self._chRasterA()
+        elif event.key == 'ctrl+up' or event.key == 'cmd+up':
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
+            if self.wvpB < self.nwvB-1:
+                self.wvpB += 1
+            else:
+                self.wvpB = 0
+            self.wvB = self.wvpB*self.dwvB+self.mwvB
+            self._chRasterB()
+        elif event.key == 'ctrl+down' or event.key == 'cmd+down':
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
+            if self.wvpB > 0:
+                self.wvpB -= 1
             else:
-                self.wvB = self.fissB.wave.max()
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
-        elif event.key == ' ' and (event.inaxes == self.axRasterA or
-                                        event.inaxes == self.axRasterB) :
+                self.wvpB = self.nwvB-1
+            self.wvB = self.wvpB*self.dwvB+self.mwvB
+            self._chRasterB()
+        elif event.key == ' ' and (event.inaxes == self.axRasterA or event.inaxes == self.axRasterB):
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
             self.x = event.xdata
             self.y = event.ydata
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
+            self.xp = int(self.x/self.dx+0.5)
+            self.yp = int(self.y/self.dy+0.5)
+            self.x = self.xp*self.dx
+            self.y = self.yp*self.dy
+            self._chSpect()
         elif event.key == ' ' and event.inaxes == self.axProfileA:
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
             self.wvA = event.xdata
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
+            self.wvpA = int((self.wvA-self.mwvA)/self.dwvA+0.5)
+            self.wvA = self.wvpA*self.dwvA+self.mwvA
+            self._chRasterA()
         elif event.key == ' ' and event.inaxes == self.axProfileB:
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
             self.wvB = event.xdata
-            self.xb = self.x0
-            self.yb = self.y0
-            self.wvAb = self.wvA0
-            self.wvBb = self.wvB0
+            self.wvpB = int((self.wvB-self.mwvB)/self.dwvB+0.5)
+            self.wvB = self.wvpB*self.dwvB+self.mwvB
+            self._chRasterB()
         elif event.key == 'ctrl+h' or event.key == 'cmd+h':
-            self.wvA = self.wvAH
-            self.wvB = self.wvBH
-            self.x = self.xH
-            self.y = self.yH
-        elif event.key == 'ctrl+b' or event.key == 'cmd+b':
-            x = self.x
-            y = self.y
-            wvA = self.wvA
-            wvB = self.wvB
-            self.x = self.xb
-            self.y = self.yb
-            self.wvA = self.wvAb
-            self.wvB = self.wvBb
-            self.xb = x
-            self.yb = y
-            self.wvAb = wvA
-            self.wvBb = wvB
-
-        if self.x != self.x0 or self.y != self.y0:
+            self.xp0 = self.xp
+            self.yp0 = self.yp
+            self.wvpA0 = self.wvpA
+            self.wvpB0 = self.wvpB
+            self.wvpA = self.wvpAH
+            self.wvpB = self.wvpBH
+            self.xp = self.xpH
+            self.yp = self.ypH
+            self.x = self.xp*self.dx
+            self.y = self.yp*self.dy
+            self.wvA = self.wvpA*self.dwvA+self.mwvA
+            self.wvB = self.wvpB*self.dwvB+self.mwvB
+            self._chRasterA()
+            self._chRasterB()
             self._chSpect()
-        if self.wvA != self.wvA0:
+        elif event.key == 'ctrl+b' or event.key == 'cmd+b':
+            x = self.xp
+            y = self.yp
+            wvA = self.wvpA
+            wvB = self.wvpB
+            self.xp = self.xp0
+            self.yp = self.yp0
+            self.wvpA = self.wvpA0
+            self.wvpB = self.wvpB0
+            self.x = self.xp*self.dx
+            self.y = self.yp*self.dy
+            self.wvA = self.wvpA*self.dwvA+self.mwvA
+            self.wvB = self.wvpB*self.dwvB+self.mwvB
             self._chRasterA()
-        if self.wvB != self.wvB0:
             self._chRasterB()
-        self.fig.canvas.draw_idle()
+            self._chSpect()
+            self.xp0 = x
+            self.yp0 = y
+            self.wvpA0 = wvA
+            self.wvpB0 = wvB
 
     def _chSpect(self):
-        self.x0 = self.x
-        self.y0 = self.y
-        xpix = int(round((self.x-self.xDelt/2)/self.xDelt))
-        ypix = int(round((self.y-self.yDelt/2)/self.yDelt))
-
-        self.plotProfileA.set_ydata(self.fissA.data[ypix, xpix])
-        self.plotProfileB.set_ydata(self.fissB.data[ypix, xpix])
+        self.plotProfileA.set_ydata(self.fissA.data[self.yp, self.xp])
+        self.plotProfileB.set_ydata(self.fissB.data[self.yp, self.xp])
         self.pointRasterA.set_offsets([self.x, self.y])
         self.pointRasterB.set_offsets([self.x, self.y])
 
-        self.axProfileA.set_ylim(self.fissA.data[ypix, xpix].min()-100,
-                                 self.fissA.data[ypix, xpix].max()+100)
-        self.axProfileB.set_ylim(self.fissB.data[ypix, xpix].min()-100,
-                                 self.fissB.data[ypix, xpix].max()+100)
+        ym = self.fissA.data[self.yp, self.xp].min()
+        yM = self.fissA.data[self.yp, self.xp].max()
+        margin = (yM-ym)*0.05
+        self.axProfileA.set_ylim(ym-margin, yM+margin)
+        ym = self.fissB.data[self.yp, self.xp].min()
+        yM = self.fissB.data[self.yp, self.xp].max()
+        margin = (yM-ym)*0.05
+        self.axProfileB.set_ylim(ym-margin, yM+margin)
+        self.fig.canvas.draw_idle()
 
     def _chRasterA(self):
-        self.wvA0 = self.wvA
-        rasterA = _getRaster(self.fissA.data, self.fissA.wave, self.wvA,
-                             self.fissA.wvDelt,
-                             hw=self.hw)
-        wh = rasterA > 5
+        rasterA = _getRaster(self.fissA.data, self.fissA.wave, self.wvA, self.fissA.wvDelt, hw=self.hw)
+        M = rasterA.max()
+        if M > 1e2:
+            m = rasterA[rasterA > 1e2].min()
+        else:
+            m = rasterA.min()
         if self.scale == 'log':
             rasterA = np.log10(rasterA)
-        cmin = rasterA[wh].min()
+            m = np.log10(m)
+            M = np.log10(M)
         self.imRasterA.set_data(rasterA)
         self.vlineProfileA.set_xdata(self.wvA)
-        self.axProfileA.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissA.band,
-                                                                self.wvA))
+        self.axProfileA.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissA.band, self.wvA))
         if self.scale == 'std':
-            self.imRasterA.set_clim(np.median(rasterA)-rasterA.std()*self.sigFactor,
-                                    np.median(rasterA)+rasterA.std()*self.sigFactor)
+            self.imRasterA.set_clim(np.median(rasterA)-rasterA.std()*self.sigFactor, np.median(rasterA)+rasterA.std()*self.sigFactor)
         else:
-            self.imRasterA.set_clim(cmin, rasterA.max())
+            self.imRasterA.set_clim(m, M)
+        self.fig.canvas.draw_idle()
 
     def _chRasterB(self):
-        self.wvB0 = self.wvB
-        rasterB = _getRaster(self.fissB.data, self.fissB.wave, self.wvB,
-                             self.fissB.wvDelt,
-                             hw=self.hw)
-        wh = rasterB > 5
+        rasterB = _getRaster(self.fissB.data, self.fissB.wave, self.wvB, self.fissB.wvDelt, hw=self.hw)
+        M = rasterB.max()
+        if M > 1e2:
+            m = rasterB[rasterB > 1e2].min()
+        else:
+            m = rasterB.min()
         if self.scale == 'log':
             rasterB = np.log10(rasterB)
-        cmin = rasterB[wh].min()
+            m = np.log10(m)
+            M = np.log10(M)
         self.imRasterB.set_data(rasterB)
         self.vlineProfileB.set_xdata(self.wvB)
-        self.axProfileB.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissB.band,
-                                                                self.wvB))
+        self.axProfileB.set_title(r'%s Band (wv = %.2f $\AA$)'%(self.fissB.band, self.wvB))
         if self.scale == 'std':
-            self.imRasterB.set_clim(np.median(rasterB)-rasterB.std()*self.sigFactor,
-                                    np.median(rasterB)+rasterB.std()*self.sigFactor)
+            self.imRasterB.set_clim(np.median(rasterB)-rasterB.std()*self.sigFactor, np.median(rasterB)+rasterB.std()*self.sigFactor)
         else:
-            self.imRasterB.set_clim(cmin, rasterB.max())
+            self.imRasterB.set_clim(m, M)
+        self.fig.canvas.draw_idle()
```

### Comparing `fisspy-1.0.9/fisspy/image/raster_set.py` & `fisspy-1.1.0/fisspy/image/raster_set.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         Please set this value to False to save the image or animation.
     
     Other parameters
     ----------------
     **kwargs:
         `~fisspy.read.FISS` keyword arguments.
     """
-    def __init__(self, flistA, flistB, wvset=None, ii=0, show=True, **kwargs):
+    def __init__(self, flistA, flistB, wvset=None, ii=None, show=True, **kwargs):
 
         
         self.show = show
         if show:
             plt.ion()
         else:
             plt.ioff()
@@ -59,15 +59,18 @@
         bgcolor = "#212529"
         bg_second = "#484c4f"
         fontcolor = "#adb5bd"
         titlecolor = "#ffda6a"
         self.time = np.zeros(self.nf, dtype=float)
         self.anx = np.zeros(self.nf, dtype=int)
 
-        A, B, time = self.loadData(ii)
+        if ii is None:
+            idx = self.nf//2
+
+        A, B, time = self.loadData(idx)
         self.rh = A.header
         cwvA = A.centralWavelength
         cwvB = B.centralWavelength
 
         if wvset is None:
             wvSet = np.array([-4, -0.7, -0.5, -0.2, 0, 0.2, 0.5, 0.7])
         else:
@@ -120,16 +123,34 @@
             if i == nwv//2:
                 self.ax[0, i].text(0.5, 0.5, f'{cwvB:.1f} $\\AA$', transform=self.ax[0, i].transAxes, ha='center', va='center', weight='bold', size=12, c=fontcolor)
                 self.ax[2, i].text(0.5, 0.5, f'{cwvA:.1f} $\\AA$', transform=self.ax[2, i].transAxes, ha='center', va='center', weight='bold', size=12, c=fontcolor)
             else:
                 self.ax[0, i].text(0.5, 0.5, f'{wvSet[i]:.1f} $\\AA$', transform=self.ax[0, i].transAxes, ha='center', va='center', weight='bold', size=12, c=fontcolor)
                 self.ax[2, i].text(0.5, 0.5, f'{wvSet[i]:.1f} $\\AA$', transform=self.ax[2, i].transAxes, ha='center', va='center', weight='bold', size=12, c=fontcolor)
 
-            self.imRasterA[i] = self.ax[3, i].imshow(A.getRaster(self.wvA[i]), cm.ha, origin='lower')
-            self.imRasterB[i] = self.ax[1, i].imshow(B.getRaster(self.wvB[i]), cm.ca, origin='lower')
+            aa = A.getRaster(self.wvA[i])
+            M = aa.max()
+            if M > 1e2:
+                m = aa[aa>1e2].min()
+            else:
+                m = aa.min()
+            aa = np.log10(aa)
+            m = np.log10(m)
+            M = np.log10(M)
+            self.imRasterA[i] = self.ax[3, i].imshow(aa, cm.ha, origin='lower', clim=[m, M])
+            bb = B.getRaster(self.wvB[i])
+            M = bb.max()
+            if M > 1e2:
+                m = bb[bb>1e2].min()
+            else:
+                m = bb.min()
+            bb = np.log10(bb)
+            m = np.log10(m)
+            M = np.log10(M)
+            self.imRasterB[i] = self.ax[1, i].imshow(bb, cm.ca, origin='lower', clim=[m, M])
             for j in range(4):
                 self.ax[j, i].set_axis_off()
                 self.ax[j, i].set_facecolor(bgcolor)
         if show:
             self.fig.show()
 
     def loadData(self, i):
@@ -180,16 +201,16 @@
             self.fig.set_figwidth(self.figy/2.3*self.nx/self.ny*self.nwv)
             for i in range(self.nwv):
                 self.imRasterA[i].set_extent([-0.5, self.nx-0.5,-0.5, self.ny-0.5])
                 self.imRasterB[i].set_extent([-0.5, self.nx-0.5,-0.5, self.ny-10-0.5])
 
 
         for i in range(self.nwv):
-            self.imRasterA[i].set_data(A.getRaster(self.wvA[i]))
-            self.imRasterB[i].set_data(B.getRaster(self.wvB[i]))
+            self.imRasterA[i].set_data(np.log10(A.getRaster(self.wvA[i])))
+            self.imRasterB[i].set_data(np.log10(B.getRaster(self.wvB[i])))
 
         self.fig.canvas.draw_idle()
 
     def saveAllImages(self, dirn, dpi=100):
         """
         Save all images
         
@@ -250,53 +271,63 @@
         -------
         None
         """
         self.ani = FuncAnimation(self.fig, self.chData, frames=np.arange(self.nf), interval=interval)
         self.fig.canvas.draw_idle()
             
 
-    def saveAnimation(self, dirn):
+    def saveAnimation(self, dirn, interval=100):
         """
         Save animation
         
         Parameters
         ----------
         dirn: `str`
             Save Directory
-        
+        interval: `int`, (optional)
+            Frame interval in unit of ms.
+            Default is 100.
+
         Returns
         -------
         None
         """
         if self.ani is None:
-            self.animation()
+            self.animation(interval=interval)
         tmp = self.rh['target'].replace(' ', '')
         mname = join(dirn, tmp+'_01.mp4')
         if isfile(mname):
             lf = len(glob(join(dirn, tmp+'*.mp4')))
             mname = mname.replace("01.mp4", f"{lf+1:02}.mp4")
         self.ani.save(mname)
         self.fname_movie = mname
         if not self.show:
             plt.close(self.fig)
 
-    def makeCatalogFiles(self, dirn):
+    def makeCatalogFiles(self, dirn, interval=100, incdata=True):
         """
         Make JSON file for the data catalog
 
         Parameters
         ----------
-        None
+        dirn: `str`
+            Save directory.
+        interval: `int`, (optional)
+            Frame interval in unit of ms.
+            Default is 100.
+        incdata: `bool`
+            If true include data in the JSON file.
+            Default is True.
 
         Returns
         -------
         None
         """
         if self.fname_movie is None:
-            self.saveAnimation(dirn)
+            self.saveAnimation(dirn, interval=interval)
         
         bdir = dirn
         date = self.stT.isot[:10].replace('-','')
         mdir = join(bdir, 'movie')
         idir = join(bdir, 'img')
         ddir = join(bdir, 'data')
         if not isdir(mdir):
@@ -364,10 +395,13 @@
         opn.write(f"""  "target": "{target}",\n""")
         opn.write(f"""  "position": {position},\n""")
         opn.write(f"""  "cadence": "{dt:.2f}",\n""")
         opn.write(f"""  "obsarea": ["{ax:.0f}", "{ay:.0f}"],\n""")
         opn.write(f"""  "imgA": "{ifname}",\n""")
         opn.write(f"""  "imgB": "",\n""")
         opn.write(f"""  "movie": ["{amname}"],\n""")
-        opn.write(f"""  "data": ["{basename(zipname)}"]\n""")
+        if incdata:
+            opn.write(f"""  "data": ["{basename(zipname)}"]\n""")
+        else:
+            opn.write(f"""  "data": [""]\n""")
         opn.write('}')
         opn.close()
```

### Comparing `fisspy-1.0.9/fisspy/io/read.py` & `fisspy-1.1.0/fisspy/io/read.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/makevideo.py` & `fisspy-1.1.0/fisspy/makevideo.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/preprocess/proc_base.py` & `fisspy-1.1.0/fisspy/preprocess/proc_base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/preprocess/proc_gui.py` & `fisspy-1.1.0/fisspy/preprocess/proc_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -2085,19 +2085,19 @@
                 fF0 = 1 - bF0
                 bF = (1-bskip)*(bF0 + fskip*fF0)
                 fF = (1-fskip)*(fF0 + bskip*bF0)
                 
                 for l in range(s1.shape[1]):
                     # foreward
                     if not fskip:
-                        fm = AutoReg(s1[i,l,:x1[kk[j]]],lags=flag).fit()
+                        fm = AutoReg(s1[i,l,:x1[kk[j]]],lags=5).fit()
                         fp = fm.forecast(npredict)
                     # backward
                     if not bskip:
-                        bm = AutoReg(s1[i,l,bst:][::-1],lags=blag).fit()
+                        bm = AutoReg(s1[i,l,bst:][::-1],lags=5).fit()
                         bp = bm.forecast(npredict)
                     pred = fF*fp + bF*bp[::-1]
                     if j != nsp-1:
                         self.ms1[i,l,x1[kk[j]]+5:x1[kk[j+1]-1]+1+5] = pred
                         # s1[i,l,x1[kk[j]]:x1[kk[j+1]-1]+1] = pred
                     else:
                         self.ms1[i,l,x1[kk[j]]+5:x1[-1]+1+5] = pred
```

### Comparing `fisspy-1.0.9/fisspy/preprocess/t_y_sh.py` & `fisspy-1.1.0/fisspy/preprocess/t_y_sh.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy/read/read_factory.py` & `fisspy-1.1.0/fisspy/read/read_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 from matplotlib import ticker
 from .. import cm
 from .readbase import getRaster, getHeader, readFrame
 from ..analysis import lambdameter
 from ..image.interactive_image import singleBand
-from ..correction import LineName, wvCalib, smoothingProf, CorSLA
+from ..correction import lineName, wvCalib, smoothingProf, corSLA
 from ..analysis import FourierFilter, Wavelet, makeTDmap
 
 __author__= "Juhyung Kang"
 __email__ = "jhkang0301@gmail.com"
-__all__ = ["rawData", "FISS", "FD", "calibData", "AlignCube"]
+__all__ = ["FISS", "FD", "AlignCube"]
 
 class rawData:
     """
     Read a raw file of the FISS.
 
     Parameters
     ----------
@@ -131,18 +131,24 @@
             plt.rcParams['keymap.back'].remove('left')
             plt.rcParams['keymap.forward'].remove('right')
         except:
             pass
 
         if not x:
             X = self.nx//2*self.xDelt
+        else:
+            X = x
         if not y:
             Y = self.ny//2*self.yDelt
+        else:
+            Y = y
         if not wv:
             WV = self.centralWavelength
+        else:
+            WV = wv
         self.x = X
         self.y = Y
         self.wv = wv
         self.imInterp = kwargs.get('interpolation', 'bilinear')
         kwargs['interpolation'] = self.imInterp
         self.iIm = singleBand(self, X, Y, WV,
                                   scale=scale, sigFactor=sigFactor,
@@ -204,20 +210,14 @@
     ----------------
     **kwargs : `~scipy.signal.savgol_filter` properties or `~scipy.ndimage.gaussian_filter1d` properties.
 
     See also
     --------
     `~scipy.signal.savgol_filter`.
     `~scipy.ndimage.gaussian_filter1d`
-
-    Examples
-    --------
-    >>> from fisspy import read
-    >>> import fisspy.data.sample
-    >>> fiss = read.FISS(fisspy.data.sample.FISS_IMAGE)
     """
 
     def __init__(self, file, x1=0, x2=None, y1=0, y2=None, ncoeff=False, smoothingMethod=None, wvCalibMethod='simple', **kwargs):
         if file.find('1.fts') != -1:
             self.ftype = 'proc'
         elif file.find('c.fts') != -1:
             self.ftype = 'comp'
@@ -235,32 +235,39 @@
 
         self.header = getHeader(file)
         self.pfile = self.header.pop('pfile', False)
         self.data = readFrame(file, self.pfile, x1=x1, x2=x2, y1=y1, y2=y2, ncoeff=ncoeff)
         self.ndim = self.header['naxis']
         self.ny, self.nx, self.nwv = self.data.shape
         self.wvDelt = self.header['cdelt1']
+        self.dx = self.xDelt
+        self.dy = self.yDelt
+        self.dwv = self.wvDelt
         self.date = self.header['date']
         try:
-            self.band = self.header['wavelen'][:4]
+            wvln = self.header['wavelen']
+            if type(wvln) == str:
+                self.band = wvln[:4]
+            else:
+                wvln = str(wvln)
         except:
             self.band = str(self.header['gratwvln'])[:4]
 
         self.refProfile = self.data.mean((0,1))
         self.wave = self.wvCalib(method=wvCalibMethod)
         self.cwv = self.centralWavelength = cwv = self.header['crval1']
 
         self.smoothing = False
         if smoothingMethod is not None:
             self.smoothing = True
         if self.smoothing:
             self.smoothingProf(method=smoothingMethod, **kwargs)
         
 
-        self.line = LineName(cwv)
+        self.line = lineName(cwv)
         if self.line == 'Ha':
             self.cam = 'A'
             self.set = '1'
             self.cmap = cm.ha
         elif self.line == 'Ca':
             self.cam = 'B'
             self.set = '1'
@@ -270,19 +277,19 @@
             self.set = '2'
             self.cmap = cm.na
         elif self.line == 'Fe':
             self.cam = 'B'
             self.set = '2'
             self.cmap = cm.fe
 
-        self.extentRaster = [0, self.nx*self.xDelt,
-                             0, self.ny*self.yDelt]
+        self.extentRaster = [-self.xDelt/2, (self.nx-0.5)*self.xDelt,
+                             -self.yDelt/2, (self.ny-0.5)*self.yDelt]
         self.extentSpectro = [self.wave.min()-self.wvDelt/2,
                               self.wave.max()+self.wvDelt/2,
-                              0, self.ny*self.yDelt]
+                              -self.yDelt/2, (self.ny-0.5)*self.yDelt]
         self.lv = None
 
     def reload(self, x1=0, x2=None, y1=0, y2=None, ncoeff=False, smoothingMethod=None, **kwargs):
         """
         Reload the FISS data.
 
         Parameters
@@ -358,15 +365,15 @@
             pf = profile
         try:
             wv = wvCalib(pf, self.header, method=method)
         except:
             raise ValueError(f"Please change the wvCalibMethod among 'simple', 'center', and 'photo'. Current: {method}")
         return wv
 
-    def CorSLA(self, refProf=None, pure=None, eps=0.027, zeta=0.055):
+    def corSLA(self, refProf=None, pure=None, eps=0.027, zeta=0.055):
         """
         Correction of spectral line(s) profile for stray linght and far wing red-blue asymmetry.
 
         Parameters
         ----------
         refProf: `numpy.ndarray`, shape (N,), (optional)
             (Spatially averaged) Reference line profile.
@@ -391,15 +398,15 @@
         if refProf is None:
             ndim = self.data.ndim
             axes = tuple([i for i in range(ndim-1)])
             rp = self.data.mean(axes)
         else:
             rp = refProf
 
-        self.data = CorSLA(self.wave, self.data, rp, self.line, pure=pure, eps=eps, zeta=zeta)
+        self.data = corSLA(self.wave, self.data, rp, self.line, pure=pure, eps=eps, zeta=zeta)
 
 
     def smoothingProf(self, method='savgol', **kwargs):
         """
         Parameters
         ----------
         method: `str`, optional
@@ -455,16 +462,15 @@
             n dimensional array of intensies of the line segment.
 
         """
         self.hw = kw.get('hw', 0.05)
         self.lwc, self.lic = lambdameter(self.wave, self.data, **kw)
         self.lv = (self.lwc-self.centralWavelength)/self.centralWavelength * ac.c.to('km/s').value
         
-    def imshow(self, x=None, y=None, wv=None, scale='minMax',
-               sigFactor=3, helpBox=True, **kwargs):
+    def imshow(self, x=None, y=None, wv=None, scale='log', sigFactor=2, helpBox=True, **kwargs):
         """
         Draw interactive FISS raster, spectrogram and profile for single band.
 
         Parameters
         ----------
         x : `float`
             X position that you draw a spectral profile.
@@ -494,18 +500,24 @@
             plt.rcParams['keymap.back'].remove('left')
             plt.rcParams['keymap.forward'].remove('right')
         except:
             pass
 
         if x is None:
             X = self.nx//2*self.xDelt
+        else:
+            X = x
         if y is None:
             Y = self.ny//2*self.yDelt
+        else:
+            Y = y
         if wv is None:
             WV = self.centralWavelength
+        else:
+            WV = wv
         self.x = X
         self.y = Y
         self.wv = WV
         self.imInterp = kwargs.get('interpolation', 'bilinear')
         self.cmap = kwargs.pop('cmap', self.cmap)
         kwargs['interpolation'] = self.imInterp
         self.iIm = singleBand(self, X, Y, WV,
@@ -535,21 +547,27 @@
             plt.rcParams['keymap.back'].remove('left')
             plt.rcParams['keymap.forward'].remove('right')
         except:
             pass
 
         if x is None:
             X = self.nx//2*self.xDelt
+        else:
+            X = x
         if y is None:
             Y = self.ny//2*self.yDelt
+        else:
+            Y = y
 
-        self.xpix = round((X-self.xDelt/2)/self.xDelt)
-        self.x = self.xpix*self.xDelt+self.xDelt/2
-        self.ypix = round((Y-self.yDelt/2)/self.yDelt)
-        self.y = self.ypix*self.yDelt+self.yDelt/2
+        self.xpix = int(X/self.dx+0.5)
+        self.x = self.xpix*self.dx
+        self.ypix = int(Y/self.dy+0.5)
+        self.y = self.ypix*self.dy
+        self.xp0 = self.xpix
+        self.yp0 = self.ypix
 
         self.lambdameter(**kw)
         
         # figure setting
         self.fig = plt.figure(figsize=[18,7])
         gs = gridspec.GridSpec(1, 5)
         self.axI = self.fig.add_subplot(gs[0,0])
@@ -561,16 +579,18 @@
         self.axSpec.set_ylabel('Intensity (Count)')
         self.axI.set_title("Intensity")
         self.axV.set_title("Velocity (km/s)")
         self.axSpec.set_title(r"X = %.2f'', Y = %.2f'' (X$_{pix}$ = %i, Y$_{pix}$ = %i), $\Delta\lambda$ = %.2f"%(self.x, self.y, self.xpix, self.ypix, self.hw))
         self.axI.set_xlim(self.extentRaster[0], self.extentRaster[1])
         self.axI.set_ylim(self.extentRaster[2], self.extentRaster[3])
         self.axSpec.set_xlim(self.wave.min(), self.wave.max())
-        self.axSpec.set_ylim(self.data[self.ypix, self.xpix].min()-100,
-                                self.data[self.ypix, self.xpix].max()+100)
+        ym = self.data[self.ypix, self.xpix].min()
+        yM = self.data[self.ypix, self.xpix].max()
+        margin = (yM-ym)*0.05
+        self.axSpec.set_ylim(ym-margin, yM+margin)
         self.axSpec.minorticks_on()
         self.axSpec.tick_params(which='both', direction='in')
 
         # Draw
         self.imI = self.axI.imshow(self.lic, self.cmap, origin='lower', extent=self.extentRaster)
         tmp = self.lic.copy().flatten()
         tmp.sort()
@@ -591,58 +611,80 @@
         self.pointV = self.axV.scatter(self.x, self.y, 50, marker='x', color='r')
 
         self.fig.tight_layout()
         self.fig.canvas.mpl_connect('key_press_event', self._onKey_vs)
         self.fig.show()
 
     def _onKey_vs(self, event):
-        if event.key == 'left' or event.key == 'ctrl+left' or event.key == 'cmd+left':
+        if event.key == 'left':
+            self.xp0 = self.xpix
+            self.yp0 = self.ypix
             if self.xpix > 0:
                 self.xpix -= 1
             else:
                 self.xpix = self.nx-1
-            self.x = self.xpix*self.xDelt+self.xDelt/2
+            self.x = self.xpix*self.dx
             self._chPos()
-        elif event.key == 'right' or event.key == 'ctrl+right' or event.key == 'cmd+right':
+        elif event.key == 'right':
+            self.xp0 = self.xpix
+            self.yp0 = self.ypix
             if self.xpix < self.nx-1:
                 self.xpix += 1
             else:
                 self.xpix = 0
-            self.x = self.xpix*self.xDelt+self.xDelt/2
+            self.x = self.xpix*self.dx
             self._chPos()
-        elif event.key == 'down' or event.key == 'ctrl+down' or event.key == 'cmd+down':
+        elif event.key == 'down':
+            self.xp0 = self.xpix
             if self.ypix > 0:
                 self.ypix -= 1
             else:
                 self.ypix = self.ny-1
-            self.y = self.ypix*self.yDelt+self.yDelt/2
+            self.y = self.ypix*self.dy
             self._chPos()
-        elif event.key == 'up' or event.key == 'ctrl+up' or event.key == 'cmd+up':
+        elif event.key == 'up':
+            self.yp0 = self.ypix
             if self.ypix < self.ny-1:
                 self.ypix += 1
             else:
                 self.ypix = 0
-            self.y = self.ypix*self.yDelt+self.yDelt/2
+            self.y = self.ypix*self.dy
             self._chPos()
         elif event.key == ' ' and (event.inaxes == self.axI or event.inaxes == self.axV):
+            self.xp0 = self.xpix
+            self.yp0 = self.ypix
             self.x = event.xdata
             self.y = event.ydata
-            self.xpix = int(round((self.x-self.xDelt/2)/self.xDelt))
-            self.ypix = int(round((self.y-self.yDelt/2)/self.yDelt))
+            self.xpix = int(self.x/self.dx+0.5)
+            self.ypix = int(self.y/self.dy+0.5)
+            self.x = self.xpix*self.dx
+            self.y = self.ypix*self.dy
             self._chPos()
+        elif event.key == 'ctrl+b' or event.key == 'cmd+b':
+            x = self.xpix
+            y = self.ypix
+            self.xp = self.xp0
+            self.yp = self.yp0
+            self.x = self.xpix*self.dx
+            self.y = self.ypix*self.dy
+            self._chPos()
+            self.xp0 = x
+            self.yp0 = y
+
 
     def _chPos(self):
         self.pSpec.set_ydata(self.data[self.ypix, self.xpix])
         self.pHL.set_xdata([self.lwc[self.ypix, self.xpix]-self.hw, self.lwc[self.ypix, self.xpix]+self.hw])
         self.pHL.set_ydata([self.lic[self.ypix, self.xpix], self.lic[self.ypix, self.xpix]])
         self.pVL.set_xdata([self.lwc[self.ypix, self.xpix], self.lwc[self.ypix, self.xpix]])
         self.pointI.set_offsets([self.x, self.y])
         self.pointV.set_offsets([self.x, self.y])
         self.axSpec.set_ylim(self.data[self.ypix, self.xpix].min()-100,
                                 self.data[self.ypix, self.xpix].max()+100)
+        self.axSpec.set_title(r"X = %.2f'', Y = %.2f'' (X$_{pix}$ = %i, Y$_{pix}$ = %i), $\Delta\lambda$ = %.2f"%(self.x, self.y, self.xpix, self.ypix, self.hw))
         self.fig.canvas.draw_idle()
     
     def chIclim(self, cmin, cmax):
         self.imI.set_clim(cmin, cmax)
         self.fig.canvas.draw_idle()
     
     def chVclim(self, cmin, cmax):
@@ -1304,36 +1346,46 @@
         if self.num != self.num0:
             self.image.set_data(self.data[self.num])
             self.num0 = self.num
         self.fig.canvas.draw_idle()
 
 class AlignCube:
     """
-    Show align cube and make Time-Distance map.
+    Read align cube.
 
     Parameters
     ----------
     fname: `str`
         File name of the align data cube.
-
-    Other Parameters
-    ----------------
-    **kwargs: `.makeTDmap` properties (optional)
-        Keyword arguments 
+        
     Returns
     -------
+    None
     """
-    def __init__(self, fname, **kwargs):
+    def __init__(self, fname):
         res = np.load(fname)
         self.data = res['data']
         self.time = res['time']
         self.dt = res['dt']
         self.dx = res['dx']
         self.dy = res['dy']
 
+    def imshow(self, **kwargs):
+        """
+        Show align cube and make Time-Distance map.
+
+        Other Parameters
+        ----------------
+        **kwargs: `.makeTDmap` properties (optional)
+            Keyword arguments
+            
+        Returns
+        -------
+        None
+        """
         self.td = makeTDmap(self.data, dx=self.dx, dy=self.dy, dt=self.dt, **kwargs)
 
 def _isoRefTime(refTime):
     year = refTime[:4]
     month = refTime[4:6]
     day = refTime[6:8]
     hour = refTime[9:11]
```

### Comparing `fisspy-1.0.9/fisspy/read/readbase.py` & `fisspy-1.1.0/fisspy/read/readbase.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/fisspy.egg-info/PKG-INFO` & `fisspy-1.1.0/fisspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.0.9
+Version: 1.1.0
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.0.9/fisspy.egg-info/SOURCES.txt` & `fisspy-1.1.0/fisspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.9/setup.py` & `fisspy-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fisspy',
-    version='1.0.9',
+    version='1.1.0',
     description='fisspy: Python analysis tools for GST/FISS',
     url='http://fiss.snu.ac.kr',
     author='Juhyung Kang',
     author_email='jhkang@astro.snu.ac.kr',
     license='BSD-2',
     python_requires='>=3.6',
     packages=find_packages(exclude=['docs', 'logo']),
```

