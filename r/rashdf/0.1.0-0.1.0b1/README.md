# Comparing `tmp/rashdf-0.1.0.tar.gz` & `tmp/rashdf-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rashdf-0.1.0.tar", last modified: Thu May  2 14:08:59 2024, max compression
+gzip compressed data, was "rashdf-0.1.0b1.tar", last modified: Fri Apr 19 16:34:41 2024, max compression
```

## Comparing `rashdf-0.1.0.tar` & `rashdf-0.1.0b1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:08:59.391690 rashdf-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-02 14:08:49.000000 rashdf-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-02 14:08:59.391690 rashdf-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-02 14:08:49.000000 rashdf-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-02 14:08:49.000000 rashdf-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:08:59.391690 rashdf-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:08:59.387690 rashdf-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:08:59.391690 rashdf-0.1.0/src/rashdf/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-02 14:08:49.000000 rashdf-0.1.0/src/rashdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-02 14:08:49.000000 rashdf-0.1.0/src/rashdf/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14846 2024-05-02 14:08:49.000000 rashdf-0.1.0/src/rashdf/geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-02 14:08:49.000000 rashdf-0.1.0/src/rashdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-05-02 14:08:49.000000 rashdf-0.1.0/src/rashdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:08:59.391690 rashdf-0.1.0/src/rashdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-02 14:08:59.000000 rashdf-0.1.0/src/rashdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 14:08:59.000000 rashdf-0.1.0/src/rashdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:08:59.000000 rashdf-0.1.0/src/rashdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 14:08:59.000000 rashdf-0.1.0/src/rashdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 14:08:59.000000 rashdf-0.1.0/src/rashdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:08:59.391690 rashdf-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-02 14:08:49.000000 rashdf-0.1.0/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-02 14:08:49.000000 rashdf-0.1.0/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-02 14:08:49.000000 rashdf-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:34:41.551280 rashdf-0.1.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 16:34:32.000000 rashdf-0.1.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-19 16:34:41.551280 rashdf-0.1.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-19 16:34:32.000000 rashdf-0.1.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-19 16:34:32.000000 rashdf-0.1.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 16:34:41.551280 rashdf-0.1.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:34:41.547280 rashdf-0.1.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:34:41.547280 rashdf-0.1.0b1/src/rashdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 16:34:32.000000 rashdf-0.1.0b1/src/rashdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-19 16:34:32.000000 rashdf-0.1.0b1/src/rashdf/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-04-19 16:34:32.000000 rashdf-0.1.0b1/src/rashdf/geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 16:34:32.000000 rashdf-0.1.0b1/src/rashdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-19 16:34:32.000000 rashdf-0.1.0b1/src/rashdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:34:41.547280 rashdf-0.1.0b1/src/rashdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-19 16:34:41.000000 rashdf-0.1.0b1/src/rashdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-19 16:34:41.000000 rashdf-0.1.0b1/src/rashdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:34:41.000000 rashdf-0.1.0b1/src/rashdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-19 16:34:41.000000 rashdf-0.1.0b1/src/rashdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 16:34:41.000000 rashdf-0.1.0b1/src/rashdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:34:41.547280 rashdf-0.1.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-19 16:34:32.000000 rashdf-0.1.0b1/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-19 16:34:32.000000 rashdf-0.1.0b1/tests/test_utils.py
```

### Comparing `rashdf-0.1.0/LICENSE` & `rashdf-0.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `rashdf-0.1.0/pyproject.toml` & `rashdf-0.1.0b1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "0.1.0"
+version = "0.1.0-beta.1"
 dependencies = ["h5py", "geopandas"]
 
 [project.optional-dependencies]
-dev = ["pre-commit", "ruff", "pytest"]
+dev = ["pytest"]
 
 [project.urls]
 repository = "https://github.com/fema-ffrd/rashdf"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 testpaths = "tests"
```

### Comparing `rashdf-0.1.0/tests/test_utils.py` & `rashdf-0.1.0b1/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 import numpy as np
 import pytest
 
 from datetime import datetime
 
 
 def test_convert_ras_hdf_value():
-    assert utils.convert_ras_hdf_value(b"True") is True
-    assert utils.convert_ras_hdf_value(b"False") is False
+    assert utils.convert_ras_hdf_value(b"True") == True
+    assert utils.convert_ras_hdf_value(b"False") == False
     assert utils.convert_ras_hdf_value(np.float32(1.23)) == pytest.approx(1.23)
     assert utils.convert_ras_hdf_value(np.int32(123)) == 123
-    assert utils.convert_ras_hdf_value(b"15Mar2024 16:39:01") == datetime(
-        2024, 3, 15, 16, 39, 1
-    )
+    assert utils.convert_ras_hdf_value(b"15Mar2024 16:39:01") == datetime(2024, 3, 15, 16, 39, 1)
     assert utils.convert_ras_hdf_value(b"15Mar2024 16:39:01 to 16Mar2024 16:39:01") == [
         datetime(2024, 3, 15, 16, 39, 1),
         datetime(2024, 3, 16, 16, 39, 1),
     ]
```

