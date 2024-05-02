# Comparing `tmp/ms2pip-4.0.0.dev8.tar.gz` & `tmp/ms2pip-4.0.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2pip-4.0.0.dev8.tar", last modified: Tue Mar  5 17:49:23 2024, max compression
+gzip compressed data, was "ms2pip-4.0.0.dev9.tar", last modified: Wed Mar 27 16:25:44 2024, max compression
```

## Comparing `ms2pip-4.0.0.dev8.tar` & `ms2pip-4.0.0.dev9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:49:23.577971 ms2pip-4.0.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-03-05 17:49:23.577971 ms2pip-4.0.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:49:23.529971 ms2pip-4.0.0.dev8/ms2pip/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:49:23.529971 ms2pip-4.0.0.dev8/ms2pip/_cython_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_cython_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_cython_modules/ms2pip_features_c.c
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_cython_modules/ms2pip_init_c.c
--rw-r--r--   0 runner    (1001) docker     (127)    19526 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_cython_modules/ms2pip_peaks_c.c
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_cython_modules/ms2pip_pyx.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:49:23.533971 ms2pip-4.0.0.dev8/ms2pip/_models_c/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:49:23.553971 ms2pip-4.0.0.dev8/ms2pip/_models_c/HCD-2019/
--rw-r--r--   0 runner    (1001) docker     (127)  8726156 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B.c
--rw-r--r--   0 runner    (1001) docker     (127)  1664299 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B2.c
--rw-r--r--   0 runner    (1001) docker     (127)  9116794 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y.c
--rw-r--r--   0 runner    (1001) docker     (127)  9063001 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y2.c
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_models_c/HCD-2019.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:49:23.569971 ms2pip-4.0.0.dev8/ms2pip/_models_c/TMT/
--rw-r--r--   0 runner    (1001) docker     (127)  2348087 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_models_c/TMT/model_20190107_TMT_train_B.c
--rw-r--r--   0 runner    (1001) docker     (127)  4323734 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_models_c/TMT/model_20190107_TMT_train_Y.c
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_models_c/TMT.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:49:23.573971 ms2pip-4.0.0.dev8/ms2pip/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_utils/dlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_utils/feature_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_utils/psm_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_utils/retention_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/_utils/xgb_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    31121 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/spectrum_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    29694 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/ms2pip/spectrum_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:49:23.577971 ms2pip-4.0.0.dev8/ms2pip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-03-05 17:49:23.000000 ms2pip-4.0.0.dev8/ms2pip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-05 17:49:23.000000 ms2pip-4.0.0.dev8/ms2pip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 17:49:23.000000 ms2pip-4.0.0.dev8/ms2pip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-05 17:49:23.000000 ms2pip-4.0.0.dev8/ms2pip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-05 17:49:23.000000 ms2pip-4.0.0.dev8/ms2pip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-05 17:49:23.000000 ms2pip-4.0.0.dev8/ms2pip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 17:49:23.577971 ms2pip-4.0.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:49:23.577971 ms2pip-4.0.0.dev8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/tests/test_fasta2speclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/tests/test_predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/tests/test_retention_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-03-05 17:49:15.000000 ms2pip-4.0.0.dev8/tests/test_spectrum_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:25:44.166544 ms2pip-4.0.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21479 2024-03-27 16:25:44.166544 ms2pip-4.0.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:25:44.118544 ms2pip-4.0.0.dev9/ms2pip/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:25:44.118544 ms2pip-4.0.0.dev9/ms2pip/_cython_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_cython_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_cython_modules/ms2pip_features_c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_cython_modules/ms2pip_init_c.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19526 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_cython_modules/ms2pip_peaks_c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_cython_modules/ms2pip_pyx.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:25:44.118544 ms2pip-4.0.0.dev9/ms2pip/_models_c/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:25:44.142544 ms2pip-4.0.0.dev9/ms2pip/_models_c/HCD-2019/
+-rw-r--r--   0 runner    (1001) docker     (127)  8726156 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B.c
+-rw-r--r--   0 runner    (1001) docker     (127)  1664299 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B2.c
+-rw-r--r--   0 runner    (1001) docker     (127)  9116794 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y.c
+-rw-r--r--   0 runner    (1001) docker     (127)  9063001 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y2.c
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_models_c/HCD-2019.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:25:44.158544 ms2pip-4.0.0.dev9/ms2pip/_models_c/TMT/
+-rw-r--r--   0 runner    (1001) docker     (127)  2348087 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_models_c/TMT/model_20190107_TMT_train_B.c
+-rw-r--r--   0 runner    (1001) docker     (127)  4323734 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_models_c/TMT/model_20190107_TMT_train_Y.c
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_models_c/TMT.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:25:44.162544 ms2pip-4.0.0.dev9/ms2pip/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_utils/dlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_utils/feature_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_utils/psm_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_utils/retention_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/_utils/xgb_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32200 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/spectrum_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29694 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/ms2pip/spectrum_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:25:44.162544 ms2pip-4.0.0.dev9/ms2pip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21479 2024-03-27 16:25:44.000000 ms2pip-4.0.0.dev9/ms2pip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-27 16:25:44.000000 ms2pip-4.0.0.dev9/ms2pip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 16:25:44.000000 ms2pip-4.0.0.dev9/ms2pip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-27 16:25:44.000000 ms2pip-4.0.0.dev9/ms2pip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-27 16:25:44.000000 ms2pip-4.0.0.dev9/ms2pip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 16:25:44.000000 ms2pip-4.0.0.dev9/ms2pip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 16:25:44.166544 ms2pip-4.0.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:25:44.162544 ms2pip-4.0.0.dev9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/tests/test_fasta2speclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/tests/test_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/tests/test_retention_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-03-27 16:25:35.000000 ms2pip-4.0.0.dev9/tests/test_spectrum_output.py
```

### Comparing `ms2pip-4.0.0.dev8/LICENSE` & `ms2pip-4.0.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/PKG-INFO` & `ms2pip-4.0.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2pip
-Version: 4.0.0.dev8
+Version: 4.0.0.dev9
 Summary: MS2PIP: Accurate and versatile peptide fragmentation spectrum prediction.
 Author: Ana Sílvia C. Silva
 Author-email: Ralf Gabriels <ralf@gabriels.dev>, Sven Degroeve <sven.degroeve@ugent.be>, Arthur Declercq <arthur.declercq@ugent.be>, Kevin Velghe <kevin.velghe@ugent.be>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -235,14 +235,16 @@
 Requires-Dist: rich>=13
 Requires-Dist: pydantic<2,>=1.10
 Requires-Dist: psm_utils>=0.2.0
 Requires-Dist: werkzeug>=2
 Provides-Extra: plotting
 Requires-Dist: matplotlib>=3.0; extra == "plotting"
 Requires-Dist: spectrum-utils>=0.4; extra == "plotting"
+Provides-Extra: tdf
+Requires-Dist: timsrust_pyo3; extra == "tdf"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort>5; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: numpydoc<2,>=1; extra == "docs"
```

### Comparing `ms2pip-4.0.0.dev8/README.rst` & `ms2pip-4.0.0.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/__main__.py` & `ms2pip-4.0.0.dev9/ms2pip/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import sys
 from pathlib import Path
 from typing import Optional
 
 import click
+from psm_utils.io import READERS
 from rich.console import Console
 from rich.logging import RichHandler
 from werkzeug.utils import secure_filename
 
 import ms2pip.core
 from ms2pip import __version__
 from ms2pip._utils.cli import build_credits, build_prediction_table
@@ -28,14 +29,16 @@
     "DEBUG": logging.DEBUG,
     "INFO": logging.INFO,
     "WARNING": logging.WARNING,
     "ERROR": logging.ERROR,
     "CRITICAL": logging.CRITICAL,
 }
 
+PSM_FILETYPES = list(READERS.keys())
+
 
 def _infer_output_name(
     input_filename: str,
     output_name: Optional[str] = None,
 ) -> Path:
     """Infer output filename from input filename if output_filename was not defined."""
     if output_name:
@@ -111,14 +114,15 @@
 def predict_library(*args, **kwargs):
     ms2pip.core.predict_library(*args, **kwargs)
 
 
 @cli.command(help=ms2pip.core.correlate.__doc__)
 @click.argument("psms", required=True)
 @click.argument("spectrum_file", required=True)
+@click.option("--psm-filetype", "-t", type=click.Choice(PSM_FILETYPES), default=None)
 @click.option("--output-name", "-o", type=str)
 @click.option("--spectrum-id-pattern", "-p")
 @click.option("--compute-correlations", "-x", is_flag=True)
 @click.option("--add-retention-time", "-r", is_flag=True)
 @click.option("--model", type=click.Choice(MODELS), default="HCD")
 @click.option("--model-dir")
 @click.option("--ms2-tolerance", type=float, default=0.02)
@@ -144,14 +148,15 @@
         logger.info(f"Writing correlations to {output_name_corr}")
         correlations_to_csv(results, output_name_corr)
 
 
 @cli.command(help=ms2pip.core.get_training_data.__doc__)
 @click.argument("psms", required=True)
 @click.argument("spectrum_file", required=True)
+@click.option("--psm-filetype", "-t", type=click.Choice(PSM_FILETYPES), default=None)
 @click.option("--output-name", "-o", type=str)
 @click.option("--spectrum-id-pattern", "-p")
 @click.option("--model", type=click.Choice(MODELS), default="HCD")
 @click.option("--ms2-tolerance", type=float, default=0.02)
 @click.option("--processes", "-n", type=int)
 def get_training_data(*args, **kwargs):
     # Parse arguments
@@ -165,14 +170,15 @@
     logger.info(f"Writing training data to {output_name}")
     training_data.to_feather(output_name)
 
 
 @cli.command(help=ms2pip.core.annotate_spectra.__doc__)
 @click.argument("psms", required=True)
 @click.argument("spectrum_file", required=True)
+@click.option("--psm-filetype", "-t", type=click.Choice(PSM_FILETYPES), default=None)
 @click.option("--output-name", "-o", type=str)
 @click.option("--spectrum-id-pattern", "-p")
 @click.option("--model", type=click.Choice(MODELS), default="HCD")
 @click.option("--ms2-tolerance", type=float, default=0.02)
 @click.option("--processes", "-n", type=int)
 def annotate_spectra(*args, **kwargs):
     # Parse arguments
@@ -204,15 +210,15 @@
             f"Unknown output format: `{o}` (supported formats: `{SUPPORTED_OUTPUT_FORMATS}`)"
         )
         sys.exit(1)
     except UnknownModelError as f:
         logger.critical(f"Unknown model: `{f}` (supported models: {set(MODELS.keys())})")
         sys.exit(1)
     except InvalidXGBoostModelError:
-        logger.critical(f"Could not download XGBoost model properly\nTry a manual download.")
+        logger.critical("Could not correctly download XGBoost model\nTry a manual download.")
         sys.exit(1)
     except Exception:
         logger.exception("An unexpected error occurred in MS²PIP.")
         sys.exit(1)
 
 
 if __name__ == "__main__":
```

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_cython_modules/ms2pip_features_c.c` & `ms2pip-4.0.0.dev9/ms2pip/_cython_modules/ms2pip_features_c.c`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_cython_modules/ms2pip_init_c.c` & `ms2pip-4.0.0.dev9/ms2pip/_cython_modules/ms2pip_init_c.c`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_cython_modules/ms2pip_peaks_c.c` & `ms2pip-4.0.0.dev9/ms2pip/_cython_modules/ms2pip_peaks_c.c`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_cython_modules/ms2pip_pyx.pyx` & `ms2pip-4.0.0.dev9/ms2pip/_cython_modules/ms2pip_pyx.pyx`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B.c` & `ms2pip-4.0.0.dev9/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B.c`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B2.c` & `ms2pip-4.0.0.dev9/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_B2.c`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y.c` & `ms2pip-4.0.0.dev9/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y.c`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y2.c` & `ms2pip-4.0.0.dev9/ms2pip/_models_c/HCD-2019/model_20190107_HCD_train_Y2.c`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_models_c/TMT/model_20190107_TMT_train_B.c` & `ms2pip-4.0.0.dev9/ms2pip/_models_c/TMT/model_20190107_TMT_train_B.c`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_models_c/TMT/model_20190107_TMT_train_Y.c` & `ms2pip-4.0.0.dev9/ms2pip/_models_c/TMT/model_20190107_TMT_train_Y.c`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_utils/cli.py` & `ms2pip-4.0.0.dev9/ms2pip/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_utils/dlib.py` & `ms2pip-4.0.0.dev9/ms2pip/_utils/dlib.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_utils/encoder.py` & `ms2pip-4.0.0.dev9/ms2pip/_utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_utils/feature_names.py` & `ms2pip-4.0.0.dev9/ms2pip/_utils/feature_names.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_utils/retention_time.py` & `ms2pip-4.0.0.dev9/ms2pip/_utils/retention_time.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/_utils/xgb_models.py` & `ms2pip-4.0.0.dev9/ms2pip/_utils/xgb_models.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/constants.py` & `ms2pip-4.0.0.dev9/ms2pip/constants.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/core.py` & `ms2pip-4.0.0.dev9/ms2pip/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,25 +68,29 @@
 
     return result
 
 
 def predict_batch(
     psms: Union[PSMList, str, Path],
     add_retention_time: bool = False,
+    psm_filetype: Optional[str] = None,
     model: Optional[str] = "HCD",
     model_dir: Optional[Union[str, Path]] = None,
     processes: Optional[int] = None,
 ) -> List[ProcessingResult]:
     """
     Predict fragmentation spectra for a batch of peptides.\f
 
     Parameters
     ----------
     psms
         PSMList or path to PSM file that is supported by psm_utils.
+    psm_filetype
+        Filetype of the PSM file. By default, None. Should be one of the supported psm_utils
+        filetypes. See https://psm-utils.readthedocs.io/en/stable/#supported-file-formats.
     add_retention_time
         Add retention time predictions with DeepLC (Requires optional DeepLC dependency).
     model
         Model to use for prediction. Default: "HCD".
     model_dir
         Directory where XGBoost model files are stored. Default: `~/.ms2pip`.
     processes
@@ -94,15 +98,15 @@
 
     Returns
     -------
     predictions: List[ProcessingResult]
         Predicted spectra with theoretical m/z and predicted intensity values.
 
     """
-    psm_list = read_psms(psms)
+    psm_list = read_psms(psms, filetype=psm_filetype)
 
     if add_retention_time:
         logger.info("Adding retention time predictions")
         rt_predictor = RetentionTime(processes=processes)
         rt_predictor.add_rt_predictions(psm_list)
 
     with Encoder.from_psm_list(psm_list) as encoder:
@@ -122,14 +126,15 @@
     """Predict spectral library from protein FASTA file."""
     raise NotImplementedError
 
 
 def correlate(
     psms: Union[PSMList, str, Path],
     spectrum_file: Union[str, Path],
+    psm_filetype: Optional[str] = None,
     spectrum_id_pattern: Optional[str] = None,
     compute_correlations: bool = False,
     add_retention_time: bool = False,
     model: Optional[str] = "HCD",
     model_dir: Optional[Union[str, Path]] = None,
     ms2_tolerance: float = 0.02,
     processes: Optional[int] = None,
@@ -139,14 +144,17 @@
 
     Parameters
     ----------
     psms
         PSMList or path to PSM file that is supported by psm_utils.
     spectrum_file
         Path to spectrum file with target intensities.
+    psm_filetype
+        Filetype of the PSM file. By default, None. Should be one of the supported psm_utils
+        filetypes. See https://psm-utils.readthedocs.io/en/stable/#supported-file-formats.
     spectrum_id_pattern
         Regular expression pattern to apply to spectrum titles before matching to
         peptide file ``spec_id`` entries.
     compute_correlations
         Compute correlations between predictions and targets.
     add_retention_time
         Add retention time predictions with DeepLC (Requires optional DeepLC dependency).
@@ -162,15 +170,15 @@
     Returns
     -------
     results: List[ProcessingResult]
         Predicted spectra with theoretical m/z and predicted intensity values, and optionally,
         correlations.
 
     """
-    psm_list = read_psms(psms)
+    psm_list = read_psms(psms, filetype=psm_filetype)
     spectrum_id_pattern = spectrum_id_pattern if spectrum_id_pattern else "(.*)"
 
     if add_retention_time:
         logger.info("Adding retention time predictions")
         rt_predictor = RetentionTime(processes=processes)
         rt_predictor.add_rt_predictions(psm_list)
 
@@ -193,28 +201,32 @@
 
     return results
 
 
 def get_training_data(
     psms: Union[PSMList, str, Path],
     spectrum_file: Union[str, Path],
+    psm_filetype: Optional[str] = None,
     spectrum_id_pattern: Optional[str] = None,
     model: Optional[str] = "HCD",
     ms2_tolerance: float = 0.02,
     processes: Optional[int] = None,
 ):
     """
     Extract feature vectors and target intensities from observed spectra for training.\f
 
     Parameters
     ----------
     psms
         PSMList or path to PSM file that is supported by psm_utils.
     spectrum_file
         Path to spectrum file with target intensities.
+    psm_filetype
+        Filetype of the PSM file. By default, None. Should be one of the supported psm_utils
+        filetypes. See https://psm-utils.readthedocs.io/en/stable/#supported-file-formats.
     spectrum_id_pattern
         Regular expression pattern to apply to spectrum titles before matching to
         peptide file ``spec_id`` entries.
     model
         Model to use as reference for the ion types that are extracted from the observed spectra.
         Default: "HCD", which results in the extraction of singly charged b- and y-ions.
     ms2_tolerance
@@ -224,15 +236,15 @@
 
     Returns
     -------
     features
         :py:class:`pandas.DataFrame` with feature vectors and targets.
 
     """
-    psm_list = read_psms(psms)
+    psm_list = read_psms(psms, filetype=psm_filetype)
     spectrum_id_pattern = spectrum_id_pattern if spectrum_id_pattern else "(.*)"
 
     with Encoder.from_psm_list(psm_list) as encoder:
         ms2pip_parallelized = _Parallelized(
             encoder=encoder,
             model=model,
             ms2_tolerance=ms2_tolerance,
@@ -248,28 +260,32 @@
 
     return training_data
 
 
 def annotate_spectra(
     psms: Union[PSMList, str, Path],
     spectrum_file: Union[str, Path],
+    psm_filetype: Optional[str] = None,
     spectrum_id_pattern: Optional[str] = None,
     model: Optional[str] = "HCD",
     ms2_tolerance: float = 0.02,
     processes: Optional[int] = None,
 ):
     """
     Annotate observed spectra.\f
 
     Parameters
     ----------
     psms
         PSMList or path to PSM file that is supported by psm_utils.
     spectrum_file
         Path to spectrum file with target intensities.
+    psm_filetype
+        Filetype of the PSM file. By default, None. Should be one of the supported psm_utils
+        filetypes. See https://psm-utils.readthedocs.io/en/stable/#supported-file-formats.
     spectrum_id_pattern
         Regular expression pattern to apply to spectrum titles before matching to
         peptide file ``spec_id`` entries.
     model
         Model to use as reference for the ion types that are extracted from the observed spectra.
         Default: "HCD", which results in the extraction of singly charged b- and y-ions.
     ms2_tolerance
@@ -279,15 +295,15 @@
 
     Returns
     -------
     results: List[ProcessingResult]
         List of ProcessingResult objects with theoretical m/z and observed intensity values.
 
     """
-    psm_list = read_psms(psms)
+    psm_list = read_psms(psms, filetype=psm_filetype)
     spectrum_id_pattern = spectrum_id_pattern if spectrum_id_pattern else "(.*)"
 
     with Encoder.from_psm_list(psm_list) as encoder:
         ms2pip_parallelized = _Parallelized(
             encoder=encoder,
             model=model,
             ms2_tolerance=ms2_tolerance,
@@ -462,24 +478,25 @@
 
             # Add jobs to pool
             mp_results = []
             for psm_list_chunk in chunks:
                 mp_results.append(pool.apply_async(func, args=(psm_list_chunk, *args)))
 
             # Gather results
-            results = [
-                r.get()
-                for r in track(
-                    mp_results,
-                    disable=len(chunks) == 1,
-                    description="Processing chunks...",
-                    transient=True,
-                    show_speed=False,
-                )
-            ]
+            # results = [
+            #     r.get()
+            #     for r in track(
+            #         mp_results,
+            #         disable=len(chunks) == 1,
+            #         description="Processing chunks...",
+            #         transient=True,
+            #         show_speed=False,
+            #     )
+            # ]
+            results = [r.get() for r in mp_results]
 
         # Sort results by input order
         results = list(
             sorted(
                 itertools.chain.from_iterable(results),
                 key=lambda result: result.psm_index,
             )
@@ -748,15 +765,14 @@
         spectrum_id_regex = re.compile(r"(.*)")
 
     # Restructure PeptideRecord entries as spec_id -> [(id, psm_1), (id, psm_2), ...]
     psms_by_specid = defaultdict(list)
     for psm_index, psm in enumerated_psm_list:
         psms_by_specid[str(psm.spectrum_id)].append((psm_index, psm))
 
-    # Track progress for only one worker (good approximation of all workers' progress)
     for spectrum in read_spectrum_file(spec_file):
         # Match spectrum ID with provided regex, use first match group as new ID
         match = spectrum_id_regex.search(spectrum.identifier)
         try:
             spectrum_id = match[1]
         except (TypeError, IndexError):
             raise exceptions.TitlePatternError(
@@ -780,16 +796,16 @@
             except exceptions.InvalidAminoAcidError:
                 result = ProcessingResult(psm_index=psm_index, psm=psm)
                 results.append(result)
                 continue
 
             targets = ms2pip_pyx.get_targets(
                 enc_peptidoform,
-                spectrum.mz,
-                spectrum.intensity,
+                spectrum.mz.astype(np.float32),
+                spectrum.intensity.astype(np.float32),
                 float(ms2_tolerance),
                 MODELS[model]["peaks_version"],
             )
             targets = {i: np.array(t, dtype=np.float32) for i, t in zip(ion_types, targets)}
 
             if not psm.peptidoform.precursor_charge:
                 psm.peptidoform.precursor_charge = spectrum.precursor_charge
```

### Comparing `ms2pip-4.0.0.dev8/ms2pip/correlation.py` & `ms2pip-4.0.0.dev9/ms2pip/correlation.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/exceptions.py` & `ms2pip-4.0.0.dev9/ms2pip/exceptions.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/result.py` & `ms2pip-4.0.0.dev9/ms2pip/result.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/spectrum.py` & `ms2pip-4.0.0.dev9/ms2pip/spectrum.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip/spectrum_input.py` & `ms2pip-4.0.0.dev9/ms2pip/spectrum_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,16 @@
                 precursor_charge = None
             try:
                 precursor_mz = spectrum["params"]["pepmass"][0]
             except KeyError:
                 precursor_mz = None
             spectrum = ObservedSpectrum(
                 identifier=spectrum["params"]["title"],
-                mz=spectrum["m/z array"],
-                intensity=spectrum["intensity array"],
+                mz=spectrum["m/z array"].astype(np.float32),
+                intensity=spectrum["intensity array"].astype(np.float32),
                 precursor_mz=precursor_mz,
                 precursor_charge=precursor_charge,
             )
             yield spectrum
 
 
 def read_mzml(spectrum_file: str) -> Generator[ObservedSpectrum, None, None]:
@@ -76,16 +76,16 @@
                 ][0]
                 try:
                     precursor_charge = precursor["charge state"]
                 except KeyError:
                     precursor_charge = None
                 spectrum = ObservedSpectrum(
                     identifier=spectrum["id"],
-                    mz=spectrum["m/z array"],
-                    intensity=spectrum["intensity array"],
+                    mz=spectrum["m/z array"].astype(np.float32),
+                    intensity=spectrum["intensity array"].astype(np.float32),
                     precursor_mz=precursor["selected ion m/z"],
                     precursor_charge=precursor_charge,
                 )
                 yield spectrum
 
 
 def read_tdf(spectrum_file: str) -> Generator[ObservedSpectrum, None, None]:
@@ -95,21 +95,24 @@
     Parameters
     ----------
     spectrum_file
         Path to .d folder.
 
     """
     if not _has_timsrust:
-        raise ImportError("Optional dependency timsrust_pyo3 required for .d spectrum file support.")
+        raise ImportError(
+            "Optional dependency timsrust_pyo3 required for .d spectrum file support. Reinstall "
+            "ms2pip with `pip install ms2pip[tdf]` and try again."
+        )
     reader = timsrust.TimsReader(spectrum_file)
     for spectrum in reader.read_all_spectra():
         spectrum = ObservedSpectrum(
             identifier=spectrum.index,
-            mz=np.asarray(spectrum.mz_values),
-            intensity=np.asarray(spectrum.intensities),
+            mz=np.asarray(spectrum.mz_values, dtype=np.float32),
+            intensity=np.asarray(spectrum.intensities, dtype=np.float32),
             precursor_mz=spectrum.precursor.mz,
             precursor_charge=spectrum.precursor.charge
             )
         yield spectrum
 
 
 def read_spectrum_file(spectrum_file: str) -> Generator[ObservedSpectrum, None, None]:
```

### Comparing `ms2pip-4.0.0.dev8/ms2pip/spectrum_output.py` & `ms2pip-4.0.0.dev9/ms2pip/spectrum_output.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/ms2pip.egg-info/PKG-INFO` & `ms2pip-4.0.0.dev9/ms2pip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2pip
-Version: 4.0.0.dev8
+Version: 4.0.0.dev9
 Summary: MS2PIP: Accurate and versatile peptide fragmentation spectrum prediction.
 Author: Ana Sílvia C. Silva
 Author-email: Ralf Gabriels <ralf@gabriels.dev>, Sven Degroeve <sven.degroeve@ugent.be>, Arthur Declercq <arthur.declercq@ugent.be>, Kevin Velghe <kevin.velghe@ugent.be>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -235,14 +235,16 @@
 Requires-Dist: rich>=13
 Requires-Dist: pydantic<2,>=1.10
 Requires-Dist: psm_utils>=0.2.0
 Requires-Dist: werkzeug>=2
 Provides-Extra: plotting
 Requires-Dist: matplotlib>=3.0; extra == "plotting"
 Requires-Dist: spectrum-utils>=0.4; extra == "plotting"
+Provides-Extra: tdf
+Requires-Dist: timsrust_pyo3; extra == "tdf"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort>5; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: numpydoc<2,>=1; extra == "docs"
```

### Comparing `ms2pip-4.0.0.dev8/ms2pip.egg-info/SOURCES.txt` & `ms2pip-4.0.0.dev9/ms2pip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/pyproject.toml` & `ms2pip-4.0.0.dev9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "pydantic>=1.10,<2",
     "psm_utils>=0.2.0",
     "werkzeug>=2",
 ]
 
 [project.optional-dependencies]
 plotting = ["matplotlib>=3.0", "spectrum-utils>=0.4"]
-# tdf = ["timsrust_pyo3@git+https://github.com/jspaezp/timsrust_pyo3#egg=0f40c31"]
+tdf = ["timsrust_pyo3"]
 dev = ["black", "isort>5", "pytest"]
 docs = [
     "sphinx",
     "numpydoc>=1,<2",
     "recommonmark",
     "toml",
     "semver>=2",
```

### Comparing `ms2pip-4.0.0.dev8/setup.py` & `ms2pip-4.0.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/tests/test_encoder.py` & `ms2pip-4.0.0.dev9/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/tests/test_fasta2speclib.py` & `ms2pip-4.0.0.dev9/tests/test_fasta2speclib.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/tests/test_predictions.py` & `ms2pip-4.0.0.dev9/tests/test_predictions.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/tests/test_retention_time.py` & `ms2pip-4.0.0.dev9/tests/test_retention_time.py`

 * *Files identical despite different names*

### Comparing `ms2pip-4.0.0.dev8/tests/test_spectrum_output.py` & `ms2pip-4.0.0.dev9/tests/test_spectrum_output.py`

 * *Files identical despite different names*

