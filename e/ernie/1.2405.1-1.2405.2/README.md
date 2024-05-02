# Comparing `tmp/ernie-1.2405.1-py3-none-any.whl.zip` & `tmp/ernie-1.2405.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 18167 bytes, number of entries: 17
--rw-r--r--  2.0 unx     1064 b- defN 24-May-01 11:54 ernie/__init__.py
+Zip file size: 17802 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      254 b- defN 24-May-01 12:17 ernie/__init__.py
 -rw-r--r--  2.0 unx     2068 b- defN 24-Apr-30 23:17 ernie/aggregation_strategies.py
 -rw-r--r--  2.0 unx    13857 b- defN 24-May-01 11:49 ernie/ernie.py
 -rw-r--r--  2.0 unx     3076 b- defN 24-May-01 11:49 ernie/helper.py
 -rw-r--r--  2.0 unx     1913 b- defN 24-May-01 11:50 ernie/models.py
 -rw-r--r--  2.0 unx     4512 b- defN 24-May-01 11:49 ernie/split_strategies.py
 -rw-r--r--  2.0 unx       87 b- defN 24-Apr-25 15:26 test/__init__.py
 -rw-r--r--  2.0 unx     1414 b- defN 24-Apr-25 15:26 test/dump_load.py
 -rw-r--r--  2.0 unx      775 b- defN 24-Apr-25 15:26 test/load_csv.py
 -rw-r--r--  2.0 unx      973 b- defN 24-Apr-25 15:26 test/load_model.py
 -rw-r--r--  2.0 unx      714 b- defN 24-Apr-25 15:26 test/predict.py
 -rw-r--r--  2.0 unx    18131 b- defN 24-Apr-25 15:26 test/split_aggregate.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-May-01 11:58 ernie-1.2405.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      957 b- defN 24-May-01 11:58 ernie-1.2405.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-01 11:58 ernie-1.2405.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 24-May-01 11:58 ernie-1.2405.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1294 b- defN 24-May-01 11:58 ernie-1.2405.1.dist-info/RECORD
-17 files, 62296 bytes uncompressed, 16081 bytes compressed:  74.2%
+-rw-rw-r--  2.0 unx    11358 b- defN 24-May-02 12:16 ernie-1.2405.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      931 b- defN 24-May-02 12:16 ernie-1.2405.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 12:16 ernie-1.2405.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 24-May-02 12:16 ernie-1.2405.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1293 b- defN 24-May-02 12:16 ernie-1.2405.2.dist-info/RECORD
+17 files, 61459 bytes uncompressed, 15716 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: test/predict.py
 Comment: 
 
 Filename: test/split_aggregate.py
 Comment: 
 
-Filename: ernie-1.2405.1.dist-info/LICENSE
+Filename: ernie-1.2405.2.dist-info/LICENSE
 Comment: 
 
-Filename: ernie-1.2405.1.dist-info/METADATA
+Filename: ernie-1.2405.2.dist-info/METADATA
 Comment: 
 
-Filename: ernie-1.2405.1.dist-info/WHEEL
+Filename: ernie-1.2405.2.dist-info/WHEEL
 Comment: 
 
-Filename: ernie-1.2405.1.dist-info/top_level.txt
+Filename: ernie-1.2405.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ernie-1.2405.1.dist-info/RECORD
+Filename: ernie-1.2405.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ernie/__init__.py

```diff
@@ -1,50 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 
-from tensorflow.python.client import device_lib
-
 from .ernie import *  # noqa: F401, F403
 
-__version__ = '1.2405.1'
+__version__ = '1.2405.2'
 
 logging.getLogger().setLevel(logging.WARNING)
 logging.getLogger('transformers.tokenization_utils').setLevel(logging.ERROR)
-logging.basicConfig(
-    format='%(asctime)-15s [%(levelname)s] %(message)s',
-    datefmt='%Y-%m-%d %H:%M:%S'
-)
-
-
-def _get_cpu_name():
-    import cpuinfo
-    cpu_info = cpuinfo.get_cpu_info()
-    cpu_name = f"{cpu_info['brand_raw']}, {cpu_info['count']} vCores"
-    return cpu_name
-
-
-def _get_gpu_name():
-    gpu_name = (
-        device_lib
-        .list_local_devices()[3]
-        .physical_device_desc
-        .split(',')[1]
-        .split('name:')[1]
-        .strip()
-    )
-    return gpu_name
-
-
-device_name = _get_cpu_name()
-device_type = 'CPU'
-
-try:
-    device_name = _get_gpu_name()
-    device_type = 'GPU'
-except IndexError:
-    # Detect TPU
-    pass
-
-logging.info(f'ernie v{__version__}')
-logging.info(f'target device: [{device_type}] {device_name}\n')
```

## Comparing `ernie-1.2405.1.dist-info/LICENSE` & `ernie-1.2405.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ernie-1.2405.1.dist-info/METADATA` & `ernie-1.2405.2.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ernie
-Version: 1.2405.1
+Version: 1.2405.2
 Summary: An Accessible Python Library for State-of-the-art Natural Language Processing. Built with HuggingFace's Transformers.
 Home-page: https://github.com/labteral/ernie
 Author: Rodrigo Martínez Castaño
 Author-email: dev@brunneis.com
 License: Apache License (Version 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -17,9 +17,8 @@
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: tf-keras
 Requires-Dist: huggingface-hub
 Requires-Dist: transformers
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
-Requires-Dist: py-cpuinfo
```

## Comparing `ernie-1.2405.1.dist-info/RECORD` & `ernie-1.2405.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-ernie/__init__.py,sha256=AOtojRK06bMwPOKXgEhwHCDFBia4YCj2AM24QJKcu-M,1064
+ernie/__init__.py,sha256=cCA40MmJRpQqQ4W5qfeDZ02MDwGewsV1KTcmOr5pKfc,254
 ernie/aggregation_strategies.py,sha256=AYp4QG4xh0ZgPGtpWgoGpwYsdgpnzZzPdda-pC7GQDA,2068
 ernie/ernie.py,sha256=tfWtwxsXlt7enVNmZn6joHm1MYPvl6LhV6sCUDYf-ig,13857
 ernie/helper.py,sha256=YfLYeGgyi3BA3wiQNko2p7383rjAqtYXs62OugDyhFs,3076
 ernie/models.py,sha256=UMqtGQIPOACKow0uf5fqA35ISVvFqHFyHS26OHwjJP8,1913
 ernie/split_strategies.py,sha256=3A1x92SquI7e3qS6r64mmo69xLl0mWPyc1xoXdMG8v0,4512
 test/__init__.py,sha256=Vy72ITAa99WGby_RFX9sxvC-QUj3J3FrgDTOAovqAOM,87
 test/dump_load.py,sha256=tdd_OLWidDZtDEqGeWABPqP6Wi9D0VSUw7olebX2Ytg,1414
 test/load_csv.py,sha256=Z7Ka3PH44axCV4Ll44bSr7hLKr5n-h5mx-N_yYDOucs,775
 test/load_model.py,sha256=oN9mKif0GrvTdjmeOS4ReJJCCw12DfaWRqJR4ZpCoag,973
 test/predict.py,sha256=Me2bBayH-nHGfxEGcUo2jrlTNq5-IOS-OxONnQqOfrE,714
 test/split_aggregate.py,sha256=6l_318O8SO1Jt2nMvxQTskznd6aS1xGWX1cqr4Yj_84,18131
-ernie-1.2405.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-ernie-1.2405.1.dist-info/METADATA,sha256=xHiN9r0sJugGNuLU1sl5nsQzTbC3Gzj5jkgU3Uq2s4Y,957
-ernie-1.2405.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ernie-1.2405.1.dist-info/top_level.txt,sha256=IHK6af4HA-M8LcMpdIUJTH0DG1QRIai_1zA3kGcbwqI,11
-ernie-1.2405.1.dist-info/RECORD,,
+ernie-1.2405.2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+ernie-1.2405.2.dist-info/METADATA,sha256=zidsz4zoJrJudW4PntWhlzj08VC2a1BSdXbofoJkmlw,931
+ernie-1.2405.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ernie-1.2405.2.dist-info/top_level.txt,sha256=IHK6af4HA-M8LcMpdIUJTH0DG1QRIai_1zA3kGcbwqI,11
+ernie-1.2405.2.dist-info/RECORD,,
```

