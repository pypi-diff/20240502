# Comparing `tmp/pluma-analysis-0.4.7.tar.gz` & `tmp/pluma_analysis-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluma-analysis-0.4.7.tar", last modified: Tue Aug 29 14:20:01 2023, max compression
+gzip compressed data, was "pluma_analysis-0.5.0.tar", last modified: Thu May  2 09:16:39 2024, max compression
```

## Comparing `pluma-analysis-0.4.7.tar` & `pluma_analysis-0.5.0.tar`

### file list

```diff
@@ -1,54 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.327792 pluma-analysis-0.4.7/
--rw-rw-rw-   0        0        0       68 2023-08-12 12:33:04.000000 pluma-analysis-0.4.7/.gitignore
--rw-rw-rw-   0        0        0     1092 2022-11-21 15:02:54.000000 pluma-analysis-0.4.7/LICENSE
--rw-rw-rw-   0        0        0       34 2023-08-12 12:33:04.000000 pluma-analysis-0.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2126 2023-08-29 14:20:01.326787 pluma-analysis-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2022-11-21 15:04:08.000000 pluma-analysis-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.052212 pluma-analysis-0.4.7/pluma/
--rw-rw-rw-   0        0        0        0 2023-08-12 12:33:04.000000 pluma-analysis-0.4.7/pluma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.074723 pluma-analysis-0.4.7/pluma/export/
--rw-rw-rw-   0        0        0     2146 2023-08-12 10:41:12.000000 pluma-analysis-0.4.7/pluma/export/maps.py
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.091723 pluma-analysis-0.4.7/pluma/export/ogcapi/
--rw-rw-rw-   0        0        0     3254 2023-08-28 11:09:16.000000 pluma-analysis-0.4.7/pluma/export/ogcapi/features.py
--rw-rw-rw-   0        0        0     2465 2023-08-29 06:48:59.000000 pluma-analysis-0.4.7/pluma/export/ogcapi/records.py
--rw-rw-rw-   0        0        0     6426 2023-08-28 12:32:57.000000 pluma-analysis-0.4.7/pluma/export/streams.py
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.152725 pluma-analysis-0.4.7/pluma/io/
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.161723 pluma-analysis-0.4.7/pluma/io/_nepy/
--rw-rw-rw-   0        0        0    18315 2023-08-12 10:41:12.000000 pluma-analysis-0.4.7/pluma/io/_nepy/NedfReader.py
--rw-rw-rw-   0        0        0     2006 2023-08-28 11:09:16.000000 pluma-analysis-0.4.7/pluma/io/accelerometer.py
--rw-rw-rw-   0        0        0     4605 2023-08-12 10:41:12.000000 pluma-analysis-0.4.7/pluma/io/eeg.py
--rw-rw-rw-   0        0        0     3317 2023-08-12 10:41:12.000000 pluma-analysis-0.4.7/pluma/io/empatica.py
--rw-rw-rw-   0        0        0     3494 2023-08-12 10:41:12.000000 pluma-analysis-0.4.7/pluma/io/harp.py
--rw-rw-rw-   0        0        0     1442 2023-08-12 10:41:12.000000 pluma-analysis-0.4.7/pluma/io/microphone.py
--rw-rw-rw-   0        0        0     3777 2023-08-12 10:41:12.000000 pluma-analysis-0.4.7/pluma/io/path_helper.py
--rw-rw-rw-   0        0        0     6800 2023-08-12 13:39:17.000000 pluma-analysis-0.4.7/pluma/io/ubx.py
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.187268 pluma-analysis-0.4.7/pluma/preprocessing/
--rw-rw-rw-   0        0        0     2107 2022-11-21 14:38:38.000000 pluma-analysis-0.4.7/pluma/preprocessing/ecg.py
--rw-rw-rw-   0        0        0     2401 2022-11-21 14:38:38.000000 pluma-analysis-0.4.7/pluma/preprocessing/resampling.py
--rw-rw-rw-   0        0        0      511 2022-11-21 14:38:38.000000 pluma-analysis-0.4.7/pluma/preprocessing/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.205262 pluma-analysis-0.4.7/pluma/schema/
--rw-rw-rw-   0        0        0    10132 2023-08-24 11:56:44.000000 pluma-analysis-0.4.7/pluma/schema/__init__.py
--rw-rw-rw-   0        0        0     9591 2023-08-12 10:41:12.000000 pluma-analysis-0.4.7/pluma/schema/outdoor.py
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.279791 pluma-analysis-0.4.7/pluma/stream/
--rw-rw-rw-   0        0        0     2926 2023-08-23 06:05:29.000000 pluma-analysis-0.4.7/pluma/stream/__init__.py
--rw-rw-rw-   0        0        0     1857 2023-08-23 06:05:29.000000 pluma-analysis-0.4.7/pluma/stream/accelerometer.py
--rw-rw-rw-   0        0        0     1733 2023-08-23 06:05:29.000000 pluma-analysis-0.4.7/pluma/stream/eeg.py
--rw-rw-rw-   0        0        0      947 2023-08-23 06:05:29.000000 pluma-analysis-0.4.7/pluma/stream/empatica.py
--rw-rw-rw-   0        0        0     6626 2023-08-23 06:05:29.000000 pluma-analysis-0.4.7/pluma/stream/georeference.py
--rw-rw-rw-   0        0        0     2298 2023-08-23 06:05:29.000000 pluma-analysis-0.4.7/pluma/stream/harp.py
--rw-rw-rw-   0        0        0     1097 2023-08-23 06:05:29.000000 pluma-analysis-0.4.7/pluma/stream/microphone.py
--rw-rw-rw-   0        0        0     1578 2022-11-21 14:38:38.000000 pluma-analysis-0.4.7/pluma/stream/siconversion.py
--rw-rw-rw-   0        0        0     3023 2023-08-23 06:05:29.000000 pluma-analysis-0.4.7/pluma/stream/ubx.py
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.296803 pluma-analysis-0.4.7/pluma/sync/
--rw-rw-rw-   0        0        0     2049 2023-08-23 06:05:29.000000 pluma-analysis-0.4.7/pluma/sync/__init__.py
--rw-rw-rw-   0        0        0     7370 2023-08-12 10:41:12.000000 pluma-analysis-0.4.7/pluma/sync/ubx2harp.py
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.298792 pluma-analysis-0.4.7/pluma/templates/
--rw-rw-rw-   0        0        0     2909 2023-08-29 14:19:16.000000 pluma-analysis-0.4.7/pluma/templates/metadata_template.j2
-drwxrwxrwx   0        0        0        0 2023-08-29 14:20:01.325787 pluma-analysis-0.4.7/pluma_analysis.egg-info/
--rw-rw-rw-   0        0        0     2126 2023-08-29 14:20:00.000000 pluma-analysis-0.4.7/pluma_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      990 2023-08-29 14:20:01.000000 pluma-analysis-0.4.7/pluma_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-29 14:20:00.000000 pluma-analysis-0.4.7/pluma_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-08-29 14:20:00.000000 pluma-analysis-0.4.7/pluma_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-29 14:20:00.000000 pluma-analysis-0.4.7/pluma_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1477 2023-08-27 14:55:28.000000 pluma-analysis-0.4.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-29 14:20:01.327792 pluma-analysis-0.4.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.566853 pluma_analysis-0.5.0/
+-rw-rw-rw-   0        0        0       78 2024-01-04 11:17:02.000000 pluma_analysis-0.5.0/.gitignore
+-rw-rw-rw-   0        0        0     1092 2022-11-21 15:02:54.000000 pluma_analysis-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-08-12 12:33:04.000000 pluma_analysis-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2554 2024-05-02 09:16:39.565854 pluma_analysis-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2024-05-02 08:57:11.000000 pluma_analysis-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.367099 pluma_analysis-0.5.0/pluma/
+-rw-rw-rw-   0        0        0        0 2023-08-12 12:33:04.000000 pluma_analysis-0.5.0/pluma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.379641 pluma_analysis-0.5.0/pluma/export/
+-rw-rw-rw-   0        0        0     2146 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/export/maps.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.383488 pluma_analysis-0.5.0/pluma/export/ogcapi/
+-rw-rw-rw-   0        0        0     3254 2024-04-05 03:04:27.000000 pluma_analysis-0.5.0/pluma/export/ogcapi/features.py
+-rw-rw-rw-   0        0        0     2465 2024-04-05 03:03:44.000000 pluma_analysis-0.5.0/pluma/export/ogcapi/records.py
+-rw-rw-rw-   0        0        0     6426 2024-04-05 03:04:11.000000 pluma_analysis-0.5.0/pluma/export/streams.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.429244 pluma_analysis-0.5.0/pluma/io/
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.439538 pluma_analysis-0.5.0/pluma/io/_nepy/
+-rw-rw-rw-   0        0        0    18315 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/_nepy/NedfReader.py
+-rw-rw-rw-   0        0        0     2006 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/accelerometer.py
+-rw-rw-rw-   0        0        0     4605 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/eeg.py
+-rw-rw-rw-   0        0        0     3317 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/empatica.py
+-rw-rw-rw-   0        0        0     3494 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/harp.py
+-rw-rw-rw-   0        0        0     1442 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/microphone.py
+-rw-rw-rw-   0        0        0     3777 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/path_helper.py
+-rw-rw-rw-   0        0        0     6800 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/io/ubx.py
+-rw-rw-rw-   0        0        0     1046 2024-05-02 08:42:57.000000 pluma_analysis-0.5.0/pluma/io/zeromq.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.445538 pluma_analysis-0.5.0/pluma/preprocessing/
+-rw-rw-rw-   0        0        0     2107 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/preprocessing/ecg.py
+-rw-rw-rw-   0        0        0     2401 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/preprocessing/resampling.py
+-rw-rw-rw-   0        0        0      511 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/preprocessing/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.457545 pluma_analysis-0.5.0/pluma/schema/
+-rw-rw-rw-   0        0        0    10132 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/schema/__init__.py
+-rw-rw-rw-   0        0        0    11160 2024-05-02 08:42:57.000000 pluma_analysis-0.5.0/pluma/schema/outdoor.py
+-rw-rw-rw-   0        0        0    12228 2024-05-02 08:42:57.000000 pluma_analysis-0.5.0/pluma/schema/vr.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.522901 pluma_analysis-0.5.0/pluma/stream/
+-rw-rw-rw-   0        0        0     3016 2024-05-02 08:42:57.000000 pluma_analysis-0.5.0/pluma/stream/__init__.py
+-rw-rw-rw-   0        0        0     1857 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/accelerometer.py
+-rw-rw-rw-   0        0        0     1468 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/csv.py
+-rw-rw-rw-   0        0        0     1733 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/eeg.py
+-rw-rw-rw-   0        0        0      947 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/empatica.py
+-rw-rw-rw-   0        0        0     6626 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/georeference.py
+-rw-rw-rw-   0        0        0     2298 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/harp.py
+-rw-rw-rw-   0        0        0     1097 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/microphone.py
+-rw-rw-rw-   0        0        0     1578 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/siconversion.py
+-rw-rw-rw-   0        0        0     3023 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/stream/ubx.py
+-rw-rw-rw-   0        0        0     6408 2024-05-02 08:42:57.000000 pluma_analysis-0.5.0/pluma/stream/zeromq.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.526452 pluma_analysis-0.5.0/pluma/sync/
+-rw-rw-rw-   0        0        0     2049 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/sync/__init__.py
+-rw-rw-rw-   0        0        0     7370 2024-04-05 03:07:52.000000 pluma_analysis-0.5.0/pluma/sync/ubx2harp.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.528452 pluma_analysis-0.5.0/pluma/templates/
+-rw-rw-rw-   0        0        0     2980 2024-01-04 11:17:02.000000 pluma_analysis-0.5.0/pluma/templates/metadata_template.j2
+drwxrwxrwx   0        0        0        0 2024-05-02 09:16:39.563853 pluma_analysis-0.5.0/pluma_analysis.egg-info/
+-rw-rw-rw-   0        0        0     2554 2024-05-02 09:16:39.000000 pluma_analysis-0.5.0/pluma_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1071 2024-05-02 09:16:39.000000 pluma_analysis-0.5.0/pluma_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 09:16:39.000000 pluma_analysis-0.5.0/pluma_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2024-05-02 09:16:39.000000 pluma_analysis-0.5.0/pluma_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-02 09:16:39.000000 pluma_analysis-0.5.0/pluma_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1545 2024-05-02 08:55:22.000000 pluma_analysis-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 09:16:39.567855 pluma_analysis-0.5.0/setup.cfg
```

### Comparing `pluma-analysis-0.4.7/LICENSE` & `pluma_analysis-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/README.md` & `pluma_analysis-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/export/maps.py` & `pluma_analysis-0.5.0/pluma/export/maps.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/export/ogcapi/features.py` & `pluma_analysis-0.5.0/pluma/export/ogcapi/features.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/export/ogcapi/records.py` & `pluma_analysis-0.5.0/pluma/export/ogcapi/records.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/export/streams.py` & `pluma_analysis-0.5.0/pluma/export/streams.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/io/_nepy/NedfReader.py` & `pluma_analysis-0.5.0/pluma/io/_nepy/NedfReader.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/io/accelerometer.py` & `pluma_analysis-0.5.0/pluma/io/accelerometer.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/io/eeg.py` & `pluma_analysis-0.5.0/pluma/io/eeg.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/io/empatica.py` & `pluma_analysis-0.5.0/pluma/io/empatica.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/io/harp.py` & `pluma_analysis-0.5.0/pluma/io/harp.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/io/microphone.py` & `pluma_analysis-0.5.0/pluma/io/microphone.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/io/path_helper.py` & `pluma_analysis-0.5.0/pluma/io/path_helper.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/io/ubx.py` & `pluma_analysis-0.5.0/pluma/io/ubx.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/preprocessing/ecg.py` & `pluma_analysis-0.5.0/pluma/preprocessing/ecg.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/preprocessing/resampling.py` & `pluma_analysis-0.5.0/pluma/preprocessing/resampling.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/schema/__init__.py` & `pluma_analysis-0.5.0/pluma/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/schema/outdoor.py` & `pluma_analysis-0.5.0/pluma/schema/outdoor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from dotmap import DotMap
 from typing import Union
+import numpy as np
 
 from pluma.stream.harp import HarpStream
 from pluma.stream.accelerometer import AccelerometerStream
 from pluma.stream.empatica import EmpaticaStream
 from pluma.stream.ubx import UbxStream, _UBX_MSGIDS
 from pluma.stream.microphone import MicrophoneStream
 from pluma.stream.eeg import EegStream
+from pluma.stream.zeromq import PupilGazeStream, PupilWorldCameraStream
 
 from pluma.io.path_helper import ComplexPath, ensure_complexpath
 
 
 def build_schema(root: Union[str, ComplexPath],
                  parent_dataset = None,
                  autoload: bool = False) -> DotMap:
@@ -21,29 +23,41 @@
         autoload (bool, optional): If True it will automatically attempt to load data from disk. Defaults to False.
 
     Returns:
         DotMap: DotMap with all the created data streams.
     """
     root = ensure_complexpath(root)
     streams = DotMap()
+
+    # Pupil streams
+    streams.PupilLabs.Counter.DecodedFrames =     HarpStream(209, device='PupilLabs', streamlabel='Counter_DecodedFrames', root=root, autoload=autoload, parent_dataset=parent_dataset)
+    streams.PupilLabs.Counter.RawFrames =         HarpStream(210, device='PupilLabs', streamlabel='Counter_RawFrames', root=root, autoload=autoload, parent_dataset=parent_dataset)
+    streams.PupilLabs.Data.RawFrames =            PupilWorldCameraStream(device='PupilLabs',
+                                                                        streamlabel='PupilLabs.WorldCamera.Data',
+                                                                        root=root, autoload=True,
+                                                                        parent_dataset=None)
+    streams.PupilLabs.Counter.IMU =               HarpStream(211, device='PupilLabs', streamlabel='Counter_IMU', root=root, autoload=autoload, parent_dataset=parent_dataset)
+    streams.PupilLabs.Counter.Gaze =              HarpStream(212, device='PupilLabs', streamlabel='Counter_Gaze', root=root, autoload=autoload, parent_dataset=parent_dataset)
+    streams.PupilLabs.Data.Gaze =                 PupilGazeStream(device='PupilLabs',
+                                                                streamlabel='PupilLabs.Gaze.Data',
+                                                                root=root, autoload=True,
+                                                                parent_dataset=None)
+    streams.PupilLabs.Counter.Audio =             HarpStream(213, device='PupilLabs', streamlabel='Counter_Audio', root=root, autoload=autoload, parent_dataset=parent_dataset)
+    streams.PupilLabs.Counter.Key =               HarpStream(214, device='PupilLabs', streamlabel='Counter_Key', root=root, autoload=autoload, parent_dataset=parent_dataset)
+
     # BioData streams
     streams.BioData.EnableStreams =               HarpStream(32, device='BioData', streamlabel='EnableStreams', root=root, autoload=autoload, parent_dataset=parent_dataset)
     streams.BioData.DisableStreams =              HarpStream(33, device='BioData', streamlabel='DisableStreams', root=root, autoload=autoload, parent_dataset=parent_dataset)
     streams.BioData.ECG =                         HarpStream(35, device='BioData', streamlabel='ECG', root=root, autoload=autoload, parent_dataset=parent_dataset)
     streams.BioData.GSR =                         HarpStream(36, device='BioData', streamlabel='GSR', root=root, autoload=autoload, parent_dataset=parent_dataset)
     streams.BioData.Accelerometer =               HarpStream(37, device='BioData', streamlabel='Accelerometer', root=root, autoload=autoload, parent_dataset=parent_dataset)
     streams.BioData.DigitalIn =                   HarpStream(38, device='BioData', streamlabel='DigitalIn', root=root, autoload=autoload, parent_dataset=parent_dataset)
     streams.BioData.Set =                         HarpStream(39, device='BioData', streamlabel='Set', root=root, autoload=autoload, parent_dataset=parent_dataset)
     streams.BioData.Clear =                       HarpStream(40, device='BioData', streamlabel='Clear', root=root, autoload=autoload, parent_dataset=parent_dataset)
 
-    # PupilLabs streams
-    streams.PupilLabs.LSLSampleTime =             HarpStream(220, device='PupilLabs', streamlabel='LSLSampleTime', root=root, autoload=autoload, parent_dataset=parent_dataset)
-    streams.PupilLabs.LSLSampleArray =            HarpStream(221, device='PupilLabs', streamlabel='LSLSampleArray', root=root, autoload=autoload, parent_dataset=parent_dataset)
-
-
     # TinkerForge streams
     streams.TK.AmbientLight.AmbientLight =        HarpStream(223, device='TK', streamlabel='AmbientLight.AmbientLight', root=root, autoload=autoload, parent_dataset=parent_dataset)
 
     streams.TK.CO2V2.CO2Conc =                    HarpStream(224, device='TK', streamlabel='CO2V2.CO2Conc', root=root, autoload=autoload, parent_dataset=parent_dataset)
     streams.TK.CO2V2.Temperature =                HarpStream(225, device='TK', streamlabel='CO2V2.Temperature', root=root, autoload=autoload, parent_dataset=parent_dataset)
     streams.TK.CO2V2.Humidity =                   HarpStream(226, device='TK', streamlabel='CO2V2.Humidity', root=root, autoload=autoload, parent_dataset=parent_dataset)
```

### Comparing `pluma-analysis-0.4.7/pluma/stream/__init__.py` & `pluma_analysis-0.5.0/pluma/stream/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 	NONE = None
 	UBX = 'UbxStream'
 	HARP = 'HarpStream'
 	ACCELEROMETER = 'AccelerometerStream'
 	MICROPHONE = 'MicrophoneStream'
 	EMPATICA = 'EmpaticaStream'
 	EEG = 'EegStream'
+	GLIA = 'GliaStream'
+	CSV = 'CsvStream'
+	PUPIL = 'PupilStream'
+	UNITY = 'UnityStream'
 
 
 class Stream:
 	"""Based class for all stream types
 	"""
 	def __init__(self,
               device: str,
```

### Comparing `pluma-analysis-0.4.7/pluma/stream/accelerometer.py` & `pluma_analysis-0.5.0/pluma/stream/accelerometer.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/stream/eeg.py` & `pluma_analysis-0.5.0/pluma/stream/eeg.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/stream/empatica.py` & `pluma_analysis-0.5.0/pluma/stream/empatica.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/stream/georeference.py` & `pluma_analysis-0.5.0/pluma/stream/georeference.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/stream/harp.py` & `pluma_analysis-0.5.0/pluma/stream/harp.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/stream/microphone.py` & `pluma_analysis-0.5.0/pluma/stream/microphone.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/stream/siconversion.py` & `pluma_analysis-0.5.0/pluma/stream/siconversion.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/stream/ubx.py` & `pluma_analysis-0.5.0/pluma/stream/ubx.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/sync/__init__.py` & `pluma_analysis-0.5.0/pluma/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/sync/ubx2harp.py` & `pluma_analysis-0.5.0/pluma/sync/ubx2harp.py`

 * *Files identical despite different names*

### Comparing `pluma-analysis-0.4.7/pluma/templates/metadata_template.j2` & `pluma_analysis-0.5.0/pluma/templates/metadata_template.j2`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,19 @@
   "properties": {
     "created": "{{ created_timestamp }}",
     "updated": "{{ updated_timestamp }}",
     "type": "dataset",
     "title": "{{ title }}",
     "description": "{{ description }}",
     "keywords": {{ keywords | tojson(indent=2) | indent(width=4) }},
-    "language": "en",
+    "language": {
+      "code": "en",
+      "name": "English",
+      "dir": "ltr"
+    },
     "contacts": [
       {%- for contact in contacts %}
       {
         "name": "{{ contact.name }}",
         "organization": "{{ contact.institution }}",
         "email": [
           {"value" : "{{ contact.email }}"}
```

### Comparing `pluma-analysis-0.4.7/pluma_analysis.egg-info/SOURCES.txt` & `pluma_analysis-0.5.0/pluma_analysis.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,29 +11,33 @@
 pluma/io/accelerometer.py
 pluma/io/eeg.py
 pluma/io/empatica.py
 pluma/io/harp.py
 pluma/io/microphone.py
 pluma/io/path_helper.py
 pluma/io/ubx.py
+pluma/io/zeromq.py
 pluma/io/_nepy/NedfReader.py
 pluma/preprocessing/ecg.py
 pluma/preprocessing/resampling.py
 pluma/preprocessing/utils.py
 pluma/schema/__init__.py
 pluma/schema/outdoor.py
+pluma/schema/vr.py
 pluma/stream/__init__.py
 pluma/stream/accelerometer.py
+pluma/stream/csv.py
 pluma/stream/eeg.py
 pluma/stream/empatica.py
 pluma/stream/georeference.py
 pluma/stream/harp.py
 pluma/stream/microphone.py
 pluma/stream/siconversion.py
 pluma/stream/ubx.py
+pluma/stream/zeromq.py
 pluma/sync/__init__.py
 pluma/sync/ubx2harp.py
 pluma/templates/metadata_template.j2
 pluma_analysis.egg-info/PKG-INFO
 pluma_analysis.egg-info/SOURCES.txt
 pluma_analysis.egg-info/dependency_links.txt
 pluma_analysis.egg-info/requires.txt
```

### Comparing `pluma-analysis-0.4.7/pyproject.toml` & `pluma_analysis-0.5.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [project]
 name = "pluma-analysis"
 authors = [
     {name = "Goncalo Lopes", email = "g.lopes@neurogears.org"},
     {name = "Bruno Cruz", email = "b.cruz@neurogears.org"},
+    {name = "Andrew Erskine", email = "a.erskine@neurogears.org"},
 ]
 description = "A low-level interface to data collected with the pluma urban data acquisition system"
 readme = "README.md"
 requires-python = ">=3.9.0"
 dynamic = ["version"]
 license = {text = "MIT License"}
```

