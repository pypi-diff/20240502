# Comparing `tmp/eprime_data-0.2.dev1.tar.gz` & `tmp/eprime_data-0.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eprime_data-0.2.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eprime_data-0.2.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eprime_data-0.2.dev1.tar` & `eprime_data-0.2.dev2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2729 2024-04-29 14:07:21.506799 eprime_data-0.2.dev1/.gitignore
--rw-r--r--   0        0        0     1073 2024-04-29 13:50:49.074138 eprime_data-0.2.dev1/LICENSE
--rw-r--r--   0        0        0      125 2024-04-29 13:51:53.987008 eprime_data-0.2.dev1/README.md
--rw-r--r--   0        0        0      459 2024-04-29 16:18:01.861145 eprime_data-0.2.dev1/eprime_data/__init__.py
--rw-r--r--   0        0        0     3186 2024-04-29 16:05:49.600798 eprime_data-0.2.dev1/eprime_data/__main__.py
--rw-r--r--   0        0        0      357 2024-04-29 14:25:02.149348 eprime_data-0.2.dev1/eprime_data/constants.py
--rw-r--r--   0        0        0      811 2024-04-29 14:29:49.137905 eprime_data-0.2.dev1/eprime_data/dataframe.py
--rw-r--r--   0        0        0     1658 2024-04-29 14:21:55.678214 eprime_data-0.2.dev1/eprime_data/dict_tab_data.py
--rw-r--r--   0        0        0     3980 2024-04-29 16:05:17.960257 eprime_data-0.2.dev1/eprime_data/lib.py
--rw-r--r--   0        0        0      539 2024-04-29 16:17:46.896895 eprime_data-0.2.dev1/pyproject.toml
--rw-r--r--   0        0        0      360 1970-01-01 00:00:00.000000 eprime_data-0.2.dev1/PKG-INFO
+-rw-r--r--   0        0        0     2729 2024-04-29 14:07:21.506799 eprime_data-0.2.dev2/.gitignore
+-rw-r--r--   0        0        0     1073 2024-04-29 13:50:49.074138 eprime_data-0.2.dev2/LICENSE
+-rw-r--r--   0        0        0      125 2024-04-29 13:51:53.987008 eprime_data-0.2.dev2/README.md
+-rw-r--r--   0        0        0      459 2024-04-29 16:31:06.434319 eprime_data-0.2.dev2/eprime_data/__init__.py
+-rw-r--r--   0        0        0     3199 2024-04-29 16:19:20.498458 eprime_data-0.2.dev2/eprime_data/__main__.py
+-rw-r--r--   0        0        0      357 2024-04-29 14:25:02.149348 eprime_data-0.2.dev2/eprime_data/constants.py
+-rw-r--r--   0        0        0      810 2024-04-29 16:30:36.705819 eprime_data-0.2.dev2/eprime_data/dataframe.py
+-rw-r--r--   0        0        0     1658 2024-04-29 14:21:55.678214 eprime_data-0.2.dev2/eprime_data/dict_tab_data.py
+-rw-r--r--   0        0        0     3980 2024-04-29 16:05:17.960257 eprime_data-0.2.dev2/eprime_data/lib.py
+-rw-r--r--   0        0        0      511 2024-04-29 16:30:57.434168 eprime_data-0.2.dev2/pyproject.toml
+-rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 eprime_data-0.2.dev2/PKG-INFO
```

### Comparing `eprime_data-0.2.dev1/.gitignore` & `eprime_data-0.2.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `eprime_data-0.2.dev1/LICENSE` & `eprime_data-0.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `eprime_data-0.2.dev1/eprime_data/__main__.py` & `eprime_data-0.2.dev2/eprime_data/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 """
 
 import argparse
 import sys
 from pathlib import Path
 from typing import List
 
-from . import __version__
+from . import __version__, __author__
 from .lib import EPrimeData
 
 
 def cli():
     parser = argparse.ArgumentParser(
         description="E-Prima-data {}: Converting E-Prime txt data".format(
             __version__),
-        epilog="(c) O. Lindemann")
+        epilog=f"(c) {__author__}")
 
     parser.add_argument("PATH", nargs='+', default=None,
                         help="the path to e-prime data file")
 
     parser.add_argument("--csv", dest="csv",
                         action="store_true",
                         help="convert to csv",
```

### Comparing `eprime_data-0.2.dev1/eprime_data/dataframe.py` & `eprime_data-0.2.dev2/eprime_data/dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from .lib import EPrimeData
 
 try:
     import pandas as pd
 except ModuleNotFoundError as err:
     raise RuntimeError("To using dataframe function please install Pandas!") from err
 
-
 def dataframe(eprime_data:EPrimeData,
               level: int, add_subject_id=False):
     """returns Pandas dataframe"""
     return pd.DataFrame(eprime_data.data(level=level, add_subject_id=add_subject_id))
 
 
 def save_to_feather(eprime_data:EPrimeData,
```

### Comparing `eprime_data-0.2.dev1/eprime_data/dict_tab_data.py` & `eprime_data-0.2.dev2/eprime_data/dict_tab_data.py`

 * *Files identical despite different names*

### Comparing `eprime_data-0.2.dev1/eprime_data/lib.py` & `eprime_data-0.2.dev2/eprime_data/lib.py`

 * *Files identical despite different names*

