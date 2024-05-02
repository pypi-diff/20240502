# Comparing `tmp/lakeapi-0.8.0.tar.gz` & `tmp/lakeapi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakeapi-0.8.0.tar", last modified: Mon Sep 25 16:38:40 2023, max compression
+gzip compressed data, was "lakeapi-0.9.1.tar", last modified: Fri Nov  3 10:50:47 2023, max compression
```

## Comparing `lakeapi-0.8.0.tar` & `lakeapi-0.9.1.tar`

### file list

```diff
@@ -1,50 +1,56 @@
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-09-25 16:38:40.046620 lakeapi-0.8.0/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      150 2022-10-08 18:58:50.000000 lakeapi-0.8.0/AUTHORS.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     3324 2023-01-24 19:55:04.000000 lakeapi-0.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     1744 2023-09-25 16:37:39.000000 lakeapi-0.8.0/HISTORY.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)    10142 2022-10-08 20:59:37.000000 lakeapi-0.8.0/LICENSE
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      262 2022-10-08 18:58:50.000000 lakeapi-0.8.0/MANIFEST.in
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       97 2022-10-08 21:00:18.000000 lakeapi-0.8.0/NOTICE.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     4583 2023-09-25 16:38:40.046620 lakeapi-0.8.0/PKG-INFO
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     2000 2023-01-24 19:57:35.000000 lakeapi-0.8.0/README.rst
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-09-25 16:38:40.042620 lakeapi-0.8.0/docs/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      608 2022-10-08 18:58:50.000000 lakeapi-0.8.0/docs/Makefile
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-09-25 16:38:40.034620 lakeapi-0.8.0/docs/_build/
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-09-25 16:38:40.034620 lakeapi-0.8.0/docs/_build/html/
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-09-25 16:38:40.042620 lakeapi-0.8.0/docs/_build/html/_static/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      286 2022-10-09 07:37:32.000000 lakeapi-0.8.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       90 2022-10-09 07:37:32.000000 lakeapi-0.8.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       90 2022-10-09 07:37:32.000000 lakeapi-0.8.0/docs/_build/html/_static/plus.png
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       28 2022-10-08 18:58:50.000000 lakeapi-0.8.0/docs/authors.rst
--rwxrwxr-x   0 lefty     (1000) lefty     (1000)     4773 2022-10-08 18:58:50.000000 lakeapi-0.8.0/docs/conf.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       33 2022-10-08 18:58:50.000000 lakeapi-0.8.0/docs/contributing.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       28 2022-10-08 18:58:50.000000 lakeapi-0.8.0/docs/history.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      305 2022-10-08 18:58:50.000000 lakeapi-0.8.0/docs/index.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     1133 2023-01-24 19:55:16.000000 lakeapi-0.8.0/docs/installation.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      292 2023-01-24 19:53:28.000000 lakeapi-0.8.0/docs/lakeapi.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      805 2022-10-08 18:58:50.000000 lakeapi-0.8.0/docs/make.bat
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       58 2022-10-09 07:37:47.000000 lakeapi-0.8.0/docs/modules.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       27 2022-10-08 18:58:50.000000 lakeapi-0.8.0/docs/readme.rst
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      658 2022-10-09 16:50:24.000000 lakeapi-0.8.0/docs/usage.rst
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-09-25 16:38:40.046620 lakeapi-0.8.0/lakeapi/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      268 2023-09-25 16:38:27.000000 lakeapi-0.8.0/lakeapi/__init__.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      429 2023-09-25 14:59:55.000000 lakeapi-0.8.0/lakeapi/_cache.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     6991 2023-08-28 13:03:07.000000 lakeapi-0.8.0/lakeapi/_read.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)    47630 2023-09-25 16:36:02.000000 lakeapi-0.8.0/lakeapi/_read_parquet.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)    15335 2022-11-19 10:30:43.000000 lakeapi-0.8.0/lakeapi/_utils.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)    10611 2023-09-25 16:30:25.000000 lakeapi-0.8.0/lakeapi/main.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     1634 2023-08-15 08:22:12.000000 lakeapi-0.8.0/lakeapi/orderbook.py
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-09-25 16:38:40.046620 lakeapi-0.8.0/lakeapi.egg-info/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     4583 2023-09-25 16:38:39.000000 lakeapi-0.8.0/lakeapi.egg-info/PKG-INFO
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      820 2023-09-25 16:38:39.000000 lakeapi-0.8.0/lakeapi.egg-info/SOURCES.txt
--rw-rw-r--   0 lefty     (1000) lefty     (1000)        1 2023-09-25 16:38:39.000000 lakeapi-0.8.0/lakeapi.egg-info/dependency_links.txt
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       45 2023-09-25 16:38:39.000000 lakeapi-0.8.0/lakeapi.egg-info/entry_points.txt
--rw-rw-r--   0 lefty     (1000) lefty     (1000)        1 2023-09-25 16:38:39.000000 lakeapi-0.8.0/lakeapi.egg-info/not-zip-safe
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      202 2023-09-25 16:38:39.000000 lakeapi-0.8.0/lakeapi.egg-info/requires.txt
--rw-rw-r--   0 lefty     (1000) lefty     (1000)        8 2023-09-25 16:38:39.000000 lakeapi-0.8.0/lakeapi.egg-info/top_level.txt
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      497 2023-09-25 16:38:40.046620 lakeapi-0.8.0/setup.cfg
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     1716 2023-09-25 16:38:27.000000 lakeapi-0.8.0/setup.py
-drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-09-25 16:38:40.046620 lakeapi-0.8.0/tests/
--rw-rw-r--   0 lefty     (1000) lefty     (1000)       37 2022-10-08 18:58:50.000000 lakeapi-0.8.0/tests/__init__.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)      858 2022-10-13 08:11:12.000000 lakeapi-0.8.0/tests/test_lakeapi.py
--rw-rw-r--   0 lefty     (1000) lefty     (1000)     1573 2023-08-15 12:57:44.000000 lakeapi-0.8.0/tests/test_orderbook.py
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-11-03 10:50:47.542780 lakeapi-0.9.1/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      150 2022-10-08 18:58:50.000000 lakeapi-0.9.1/AUTHORS.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     3324 2023-01-24 19:55:04.000000 lakeapi-0.9.1/CONTRIBUTING.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     1862 2023-11-03 10:49:20.000000 lakeapi-0.9.1/HISTORY.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    10142 2022-10-08 20:59:37.000000 lakeapi-0.9.1/LICENSE
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      262 2022-10-08 18:58:50.000000 lakeapi-0.9.1/MANIFEST.in
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       97 2022-10-08 21:00:18.000000 lakeapi-0.9.1/NOTICE.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     4752 2023-11-03 10:50:47.542780 lakeapi-0.9.1/PKG-INFO
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     2000 2023-01-24 19:57:35.000000 lakeapi-0.9.1/README.rst
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-11-03 10:50:47.530781 lakeapi-0.9.1/docs/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      608 2022-10-08 18:58:50.000000 lakeapi-0.9.1/docs/Makefile
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-11-03 10:50:47.522781 lakeapi-0.9.1/docs/_build/
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-11-03 10:50:47.522781 lakeapi-0.9.1/docs/_build/html/
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-11-03 10:50:47.534781 lakeapi-0.9.1/docs/_build/html/_static/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      286 2022-10-09 07:37:32.000000 lakeapi-0.9.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       90 2022-10-09 07:37:32.000000 lakeapi-0.9.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       90 2022-10-09 07:37:32.000000 lakeapi-0.9.1/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       28 2022-10-08 18:58:50.000000 lakeapi-0.9.1/docs/authors.rst
+-rwxrwxr-x   0 lefty     (1000) lefty     (1000)     4773 2022-10-08 18:58:50.000000 lakeapi-0.9.1/docs/conf.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       33 2022-10-08 18:58:50.000000 lakeapi-0.9.1/docs/contributing.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       28 2022-10-08 18:58:50.000000 lakeapi-0.9.1/docs/history.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      305 2022-10-08 18:58:50.000000 lakeapi-0.9.1/docs/index.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     1133 2023-01-24 19:55:16.000000 lakeapi-0.9.1/docs/installation.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      292 2023-11-03 10:32:30.000000 lakeapi-0.9.1/docs/lakeapi.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      805 2022-10-08 18:58:50.000000 lakeapi-0.9.1/docs/make.bat
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       58 2023-11-03 10:30:58.000000 lakeapi-0.9.1/docs/modules.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       27 2022-10-08 18:58:50.000000 lakeapi-0.9.1/docs/readme.rst
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      658 2022-10-09 16:50:24.000000 lakeapi-0.9.1/docs/usage.rst
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-11-03 10:50:47.538781 lakeapi-0.9.1/lakeapi/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      268 2023-11-03 10:50:27.000000 lakeapi-0.9.1/lakeapi/__init__.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      429 2023-09-25 14:59:55.000000 lakeapi-0.9.1/lakeapi/_cache.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    19328 2023-11-02 15:11:21.000000 lakeapi-0.9.1/lakeapi/_config.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    30503 2023-11-02 15:11:38.000000 lakeapi-0.9.1/lakeapi/_data_types.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    20382 2023-11-02 15:30:12.000000 lakeapi-0.9.1/lakeapi/_describe.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    23489 2023-11-03 09:32:54.000000 lakeapi-0.9.1/lakeapi/_fs.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     6615 2023-11-02 15:30:07.000000 lakeapi-0.9.1/lakeapi/_read.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    25753 2023-11-03 10:29:12.000000 lakeapi-0.9.1/lakeapi/_read_parquet.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    15308 2023-11-02 14:48:16.000000 lakeapi-0.9.1/lakeapi/_utils.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     2977 2023-11-02 14:43:52.000000 lakeapi-0.9.1/lakeapi/exceptions.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)    10824 2023-11-03 09:54:18.000000 lakeapi-0.9.1/lakeapi/main.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     1634 2023-08-15 08:22:12.000000 lakeapi-0.9.1/lakeapi/orderbook.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     2201 2023-10-09 13:44:33.000000 lakeapi-0.9.1/lakeapi/test.py
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-11-03 10:50:47.542780 lakeapi-0.9.1/lakeapi.egg-info/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     4752 2023-11-03 10:50:47.000000 lakeapi-0.9.1/lakeapi.egg-info/PKG-INFO
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      936 2023-11-03 10:50:47.000000 lakeapi-0.9.1/lakeapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)        1 2023-11-03 10:50:47.000000 lakeapi-0.9.1/lakeapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       45 2023-11-03 10:50:47.000000 lakeapi-0.9.1/lakeapi.egg-info/entry_points.txt
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)        1 2023-11-03 10:50:47.000000 lakeapi-0.9.1/lakeapi.egg-info/not-zip-safe
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      179 2023-11-03 10:50:47.000000 lakeapi-0.9.1/lakeapi.egg-info/requires.txt
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)        8 2023-11-03 10:50:47.000000 lakeapi-0.9.1/lakeapi.egg-info/top_level.txt
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      497 2023-11-03 10:50:47.542780 lakeapi-0.9.1/setup.cfg
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     1740 2023-11-03 10:50:27.000000 lakeapi-0.9.1/setup.py
+drwxrwxr-x   0 lefty     (1000) lefty     (1000)        0 2023-11-03 10:50:47.542780 lakeapi-0.9.1/tests/
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)       37 2022-10-08 18:58:50.000000 lakeapi-0.9.1/tests/__init__.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)      858 2022-10-13 08:11:12.000000 lakeapi-0.9.1/tests/test_lakeapi.py
+-rw-rw-r--   0 lefty     (1000) lefty     (1000)     1573 2023-08-15 12:57:44.000000 lakeapi-0.9.1/tests/test_orderbook.py
```

### Comparing `lakeapi-0.8.0/CONTRIBUTING.rst` & `lakeapi-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lakeapi-0.8.0/HISTORY.rst` & `lakeapi-0.9.1/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+0.9.1 (2023-11-03)
+------------------
+
+* awswrangler dependency removed, pandas 2 support added
+* python3.12 support
+
 0.8.0 (2023-09-18)
 ------------------
 
 * grow default cache size limit
 * nicer error messages when data are missing
 * pass and print warning when file is corrupted
```

### Comparing `lakeapi-0.8.0/LICENSE` & `lakeapi-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeapi-0.8.0/PKG-INFO` & `lakeapi-0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeapi
-Version: 0.8.0
+Version: 0.9.1
 Summary: API for accessing Lake crypto market data
 Home-page: https://github.com/crypto-lake/lake-api
 Author: Jan Skoda
 Author-email: skoda@jskoda.cz
 License: Apache 2 license
 Keywords: lakeapi
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 License-File: LICENSE
 License-File: NOTICE.rst
 License-File: AUTHORS.rst
 
 ========
 Lake API
@@ -89,14 +90,20 @@
 working directory.
 
 
 =======
 History
 =======
 
+0.9.1 (2023-11-03)
+------------------
+
+* awswrangler dependency removed, pandas 2 support added
+* python3.12 support
+
 0.8.0 (2023-09-18)
 ------------------
 
 * grow default cache size limit
 * nicer error messages when data are missing
 * pass and print warning when file is corrupted
```

### Comparing `lakeapi-0.8.0/README.rst` & `lakeapi-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `lakeapi-0.8.0/docs/Makefile` & `lakeapi-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lakeapi-0.8.0/docs/conf.py` & `lakeapi-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lakeapi-0.8.0/docs/installation.rst` & `lakeapi-0.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lakeapi-0.8.0/docs/make.bat` & `lakeapi-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lakeapi-0.8.0/docs/usage.rst` & `lakeapi-0.9.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `lakeapi-0.8.0/lakeapi/_read.py` & `lakeapi-0.9.1/lakeapi/_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,20 @@
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union, cast
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import union_categoricals
 from tqdm.contrib.concurrent import thread_map
 
-from awswrangler import exceptions
+from lakeapi import exceptions
 from lakeapi._utils import boto3_to_primitives, ensure_cpu_count
-from awswrangler.s3._list import _prefix_cleanup
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-def _get_path_root(path: Union[str, List[str]], dataset: bool) -> Optional[str]:
-    if (dataset is True) and (not isinstance(path, str)):
-        raise exceptions.InvalidArgument("The path argument must be a string if dataset=True (Amazon S3 prefix).")
-    return _prefix_cleanup(str(path)) if dataset is True else None
-
-
 def _get_path_ignore_suffix(path_ignore_suffix: Union[str, List[str], None]) -> Union[List[str], None]:
     if isinstance(path_ignore_suffix, str):
         path_ignore_suffix = [path_ignore_suffix, "/_SUCCESS"]
     elif path_ignore_suffix is None:
         path_ignore_suffix = ["/_SUCCESS"]
     else:
         path_ignore_suffix = path_ignore_suffix + ["/_SUCCESS"]
```

### Comparing `lakeapi-0.8.0/lakeapi/_read_parquet.py` & `lakeapi-0.9.1/lakeapi/_read_parquet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 """Amazon S3 Read PARQUET Module (PRIVATE)."""
 
-import concurrent.futures
+# import concurrent.futures
 import datetime
-import functools
-import itertools
+# import functools
+# import itertools
+# from contextlib import contextmanager
 import json
 import logging
 import pprint
 import warnings
-from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional, Tuple, Union, cast
+from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional, Tuple, Union, cast, Sequence
 
 import boto3
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet
 
-from awswrangler import _data_types, exceptions
+from lakeapi import _data_types
 from lakeapi import _utils
-from awswrangler._config import apply_configs
-from awswrangler.catalog._get import _get_partitions
-from awswrangler.s3._fs import open_s3_object
-from awswrangler.s3._list import _path2list
+from lakeapi import exceptions
+from lakeapi._describe import _prefix_cleanup
+from lakeapi import _fs
+# from lakeapi._config import apply_configs
+# from awswrangler.catalog._get import _get_partitions
+from lakeapi._fs import open_s3_object
+from lakeapi._describe import _path2list, _get_path_root
+
 
 from lakeapi._read import (
     _apply_partition_filter,
     _apply_partitions,
-    _extract_partitions_dtypes_from_table_details,
-    _extract_partitions_metadata_from_paths,
+    # _extract_partitions_dtypes_from_table_details,
+    # _extract_partitions_metadata_from_paths,
     _get_path_ignore_suffix,
-    _get_path_root,
+    # _get_path_root,
     _read_dfs_from_multiple_paths,
     _union,
 )
 from lakeapi._cache import cached
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
+
 def _pyarrow_parquet_file_wrapper(
     source: Any, path: str,
     read_dictionary: Optional[List[str]] = None, coerce_int96_timestamp_unit: Optional[str] = None,
 ) -> pyarrow.parquet.ParquetFile:
     try:
         try:
             return pyarrow.parquet.ParquetFile(
@@ -57,196 +63,26 @@
             return None
         if str(ex) == "Parquet magic bytes not found in footer. Either the file is corrupted or this is not a parquet file.":
             _logger.warning("Ignoring corrupted file = %s", path)
             return None
         raise
 
 
-def _read_parquet_metadata_file(
-    path: str,
-    boto3_session: boto3.Session,
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    use_threads: Union[bool, int],
-    version_id: Optional[str] = None,
-    ignore_null: bool = False,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
-) -> Optional[Dict[str, str]]:
-    pyarrow_args = _set_default_pyarrow_additional_kwargs(pyarrow_additional_kwargs)
-    with open_s3_object(
-        path=path,
-        mode="rb",
-        version_id=version_id,
-        use_threads=use_threads,
-        s3_block_size=131_072,  # 128 KB (128 * 2**10)
-        s3_additional_kwargs=s3_additional_kwargs,
-        boto3_session=boto3_session,
-    ) as f:
-        pq_file: Optional[pyarrow.parquet.ParquetFile] = _pyarrow_parquet_file_wrapper(
-            source=f, coerce_int96_timestamp_unit=pyarrow_args["coerce_int96_timestamp_unit"], path = path,
-        )
-        if pq_file is None:
-            return None
-        return _data_types.athena_types_from_pyarrow_schema(
-            schema=pq_file.schema.to_arrow_schema(), partitions=None, ignore_null=ignore_null
-        )[0]
-
-
-def _read_schemas_from_files(
-    paths: List[str],
-    sampling: float,
-    use_threads: Union[bool, int],
-    boto3_session: boto3.Session,
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    version_ids: Optional[Dict[str, str]] = None,
-    ignore_null: bool = False,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
-) -> Tuple[Dict[str, str], ...]:
-
-    paths = _utils.list_sampling(lst=paths, sampling=sampling)
-    schemas: Tuple[Optional[Dict[str, str]], ...] = tuple()
-    n_paths: int = len(paths)
-    cpus: int = _utils.ensure_cpu_count(use_threads)
-    if cpus == 1 or n_paths == 1:
-        schemas = tuple(
-            _read_parquet_metadata_file(
-                path=p,
-                boto3_session=boto3_session,
-                s3_additional_kwargs=s3_additional_kwargs,
-                use_threads=use_threads,
-                version_id=version_ids.get(p) if isinstance(version_ids, dict) else None,
-                ignore_null=ignore_null,
-                pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-            )
-            for p in paths
-        )
-    elif n_paths > 1:
-        versions = [version_ids.get(p) if isinstance(version_ids, dict) else None for p in paths]
-        with concurrent.futures.ThreadPoolExecutor(max_workers=cpus) as executor:
-            schemas = tuple(
-                executor.map(
-                    _read_parquet_metadata_file,
-                    paths,
-                    itertools.repeat(_utils.boto3_to_primitives(boto3_session=boto3_session)),  # Boto3.Session
-                    itertools.repeat(s3_additional_kwargs),
-                    itertools.repeat(use_threads),
-                    versions,
-                    itertools.repeat(ignore_null),
-                    itertools.repeat(pyarrow_additional_kwargs),
-                )
-            )
-    schemas = cast(Tuple[Dict[str, str], ...], tuple(x for x in schemas if x is not None))
-    _logger.debug("schemas: %s", schemas)
-    return schemas
-
-
-def _validate_schemas(schemas: Tuple[Dict[str, str], ...]) -> None:
-    if len(schemas) < 2:
-        return None
-    first: Dict[str, str] = schemas[0]
-    for schema in schemas[1:]:
-        if first != schema:
-            raise exceptions.InvalidSchemaConvergence(
-                f"Was detect at least 2 different schemas:\n    1 - {first}\n    2 - {schema}."
-            )
-    return None
-
-
-def _validate_schemas_from_files(
-    paths: List[str],
-    sampling: float,
-    use_threads: Union[bool, int],
-    boto3_session: boto3.Session,
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    version_ids: Optional[Dict[str, str]] = None,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
-) -> None:
-    schemas: Tuple[Dict[str, str], ...] = _read_schemas_from_files(
-        paths=paths,
-        sampling=sampling,
-        use_threads=use_threads,
-        boto3_session=boto3_session,
-        s3_additional_kwargs=s3_additional_kwargs,
-        version_ids=version_ids,
-        pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-    )
-    _validate_schemas(schemas=schemas)
-
-
 def _merge_schemas(schemas: Tuple[Dict[str, str], ...]) -> Dict[str, str]:
     columns_types: Dict[str, str] = {}
     for schema in schemas:
         for column, dtype in schema.items():
             if (column in columns_types) and (columns_types[column] != dtype):
                 raise exceptions.InvalidSchemaConvergence(
                     f"Was detect at least 2 different types in column {column} ({columns_types[column]} and {dtype})."
                 )
             columns_types[column] = dtype
     return columns_types
 
 
-def _read_parquet_metadata(
-    path: Union[str, List[str]],
-    path_suffix: Optional[str],
-    path_ignore_suffix: Optional[str],
-    ignore_empty: bool,
-    ignore_null: bool,
-    dtype: Optional[Dict[str, str]],
-    sampling: float,
-    dataset: bool,
-    use_threads: Union[bool, int],
-    boto3_session: boto3.Session,
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    version_id: Optional[Union[str, Dict[str, str]]] = None,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
-) -> Tuple[Dict[str, str], Optional[Dict[str, str]], Optional[Dict[str, List[str]]]]:
-    """Handle wr.s3.read_parquet_metadata internally."""
-    path_root: Optional[str] = _get_path_root(path=path, dataset=dataset)
-    paths: List[str] = _path2list(
-        path=path,
-        boto3_session=boto3_session,
-        suffix=path_suffix,
-        ignore_suffix=_get_path_ignore_suffix(path_ignore_suffix=path_ignore_suffix),
-        ignore_empty=ignore_empty,
-        s3_additional_kwargs=s3_additional_kwargs,
-    )
-
-    # Files
-    schemas: Tuple[Dict[str, str], ...] = _read_schemas_from_files(
-        paths=paths,
-        sampling=sampling,
-        use_threads=use_threads,
-        boto3_session=boto3_session,
-        s3_additional_kwargs=s3_additional_kwargs,
-        version_ids=version_id
-        if isinstance(version_id, dict)
-        else {paths[0]: version_id}
-        if isinstance(version_id, str)
-        else None,
-        ignore_null=ignore_null,
-        pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-    )
-    columns_types: Dict[str, str] = _merge_schemas(schemas=schemas)
-
-    # Partitions
-    partitions_types: Optional[Dict[str, str]] = None
-    partitions_values: Optional[Dict[str, List[str]]] = None
-    if (dataset is True) and (path_root is not None):
-        partitions_types, partitions_values = _extract_partitions_metadata_from_paths(path=path_root, paths=paths)
-
-    # Casting
-    if dtype:
-        for k, v in dtype.items():
-            if columns_types and k in columns_types:
-                columns_types[k] = v
-            if partitions_types and k in partitions_types:
-                partitions_types[k] = v
-
-    return columns_types, partitions_types, partitions_values
-
-
 def _apply_index(df: pd.DataFrame, metadata: Dict[str, Any]) -> pd.DataFrame:
     index_columns: List[Any] = metadata["index_columns"]
     ignore_index: bool = True
     _logger.debug("df.columns: %s", df.columns)
 
     if index_columns:
         if isinstance(index_columns[0], str):
@@ -366,15 +202,14 @@
         _logger.debug("Reading Row Group %s...", i)
         yield pq_file.read_row_group(i=i, columns=columns, use_threads=use_threads_flag, use_pandas_metadata=False)
 
 
 def _read_parquet_chunked(  # pylint: disable=too-many-branches
     paths: List[str],
     chunked: Union[bool, int],
-    validate_schema: bool,
     ignore_index: Optional[bool],
     columns: Optional[List[str]],
     categories: Optional[List[str]],
     safe: bool,
     map_types: bool,
     boto3_session: boto3.Session,
     dataset: bool,
@@ -403,27 +238,14 @@
                 source=f,
                 read_dictionary=categories,
                 coerce_int96_timestamp_unit=pyarrow_args["coerce_int96_timestamp_unit"],
                 path = path,
             )
             if pq_file is None:
                 continue
-            if validate_schema is True:
-                schema: Dict[str, str] = _data_types.athena_types_from_pyarrow_schema(
-                    schema=pq_file.schema.to_arrow_schema(), partitions=None
-                )[0]
-                if last_schema is not None:
-                    if schema != last_schema:
-                        raise exceptions.InvalidSchemaConvergence(
-                            f"Was detect at least 2 different schemas:\n"
-                            f"    - {last_path} -> {last_schema}\n"
-                            f"    - {path} -> {schema}"
-                        )
-                last_schema = schema
-                last_path = path
             num_row_groups: int = pq_file.num_row_groups
             _logger.debug("num_row_groups: %s", num_row_groups)
             use_threads_flag: bool = use_threads if isinstance(use_threads, bool) else bool(use_threads > 1)
             # iter_batches is only available for pyarrow >= 3.0.0
             if callable(getattr(pq_file, "iter_batches", None)):
                 chunk_generator = _pyarrow_chunk_generator(
                     pq_file=pq_file, chunked=chunked, columns=columns, use_threads_flag=use_threads_flag
@@ -529,15 +351,14 @@
     version_id: Optional[str],
     columns: Optional[List[str]],
     categories: Optional[List[str]],
     safe: bool,
     map_types: bool,
     boto3_session: Union[boto3.Session, _utils.Boto3PrimitivesType],
     dataset: bool,
-    validate_schema: Optional[bool],
     path_root: Optional[str],
     s3_additional_kwargs: Optional[Dict[str, str]],
     use_threads: Union[bool, int],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> pd.DataFrame:
     pyarrow_args = _set_default_pyarrow_additional_kwargs(pyarrow_additional_kwargs)
     boto3_session = _utils.ensure_session(boto3_session)
@@ -557,33 +378,28 @@
         map_types=map_types,
         use_threads=use_threads,
         dataset=dataset,
         path=path,
         path_root=path_root,
         timestamp_as_object=pyarrow_args["timestamp_as_object"],
     )
-    if validate_schema and columns:
-        for column in columns:
-            if column not in df.columns:
-                raise exceptions.InvalidArgument(f"column: {column} does not exist")
     return df
 _read_parquet = cached(_read_parquet_nocache, ignore = ['boto3_session'])
 
 
 def read_parquet(
     path: Union[str, List[str]],
     path_root: Optional[str] = None,
     path_suffix: Union[str, List[str], None] = None,
     path_ignore_suffix: Union[str, List[str], None] = None,
     version_id: Optional[Union[str, Dict[str, str]]] = None,
     ignore_empty: bool = True,
     ignore_index: Optional[bool] = None,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = None,
     columns: Optional[List[str]] = None,
-    validate_schema: bool = False,
     chunked: Union[bool, int] = False,
     dataset: bool = False,
     categories: Optional[List[str]] = None,
     safe: bool = True,
     map_types: bool = True,
     use_threads: Union[bool, int] = True,
     last_modified_begin: Optional[datetime.datetime] = None,
@@ -652,18 +468,14 @@
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
     columns : List[str], optional
         Names of columns to read from the file(s).
-    validate_schema:
-        Check that individual file schemas are all the same / compatible. Schemas within a
-        folder prefix should all be the same. Disable if you have schemas that are different
-        and want to disable this check.
     chunked : Union[int, bool]
         If passed will split the data in a Iterable of DataFrames (Memory friendly).
         If `True` awswrangler iterates on the data by files in the most efficient way without guarantee of chunksize.
         If an `INTEGER` is passed awswrangler will iterate on the data by number of rows igual the received INTEGER.
     dataset: bool
         If `True` read a parquet dataset instead of simple file(s) loading all the related partitions as columns.
     categories: Optional[List[str]], optional
@@ -767,15 +579,14 @@
         "columns": columns,
         "categories": categories,
         "safe": safe,
         "map_types": map_types,
         "boto3_session": session,
         "dataset": dataset,
         "path_root": path_root,
-        "validate_schema": validate_schema,
         "s3_additional_kwargs": s3_additional_kwargs,
         "use_threads": use_threads,
         "pyarrow_additional_kwargs": pyarrow_additional_kwargs,
     }
     _logger.debug("args:\n%s", pprint.pformat(args))
     if chunked is not False:
         return _read_parquet_chunked(
@@ -787,355 +598,26 @@
         )
     if len(paths) == 1:
         return _read_parquet(
             path=paths[0],
             version_id=versions[paths[0]] if isinstance(versions, dict) else None,
             **args,
         )
-    if validate_schema is True:
-        _validate_schemas_from_files(
-            paths=paths,
-            version_ids=versions,
-            sampling=1.0,
-            use_threads=True,
-            boto3_session=boto3_session,
-            s3_additional_kwargs=s3_additional_kwargs,
-        )
     return _union(
         dfs=_read_dfs_from_multiple_paths(
             read_func=_read_parquet,
             paths=paths,
             version_ids=versions,
             use_threads=use_threads,
             kwargs=args,
         ),
         ignore_index=ignore_index,
     )
 
 
-@apply_configs
-def read_parquet_table(
-    table: str,
-    database: str,
-    filename_suffix: Union[str, List[str], None] = None,
-    filename_ignore_suffix: Union[str, List[str], None] = None,
-    catalog_id: Optional[str] = None,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = None,
-    columns: Optional[List[str]] = None,
-    validate_schema: bool = True,
-    categories: Optional[List[str]] = None,
-    safe: bool = True,
-    map_types: bool = True,
-    chunked: Union[bool, int] = False,
-    use_threads: Union[bool, int] = True,
-    boto3_session: Optional[boto3.Session] = None,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    """Read Apache Parquet table registered on AWS Glue Catalog.
-
-    Note
-    ----
-    ``Batching`` (`chunked` argument) (Memory Friendly):
-
-    Will enable the function to return an Iterable of DataFrames instead of a regular DataFrame.
-
-    There are two batching strategies on awswrangler:
-
-    - If **chunked=True**, a new DataFrame will be returned for each file in your path/dataset.
-
-    - If **chunked=INTEGER**, awswrangler will paginate through files slicing and concatenating
-      to return DataFrames with the number of row igual the received INTEGER.
-
-    `P.S.` `chunked=True` if faster and uses less memory while `chunked=INTEGER` is more precise
-    in number of rows for each Dataframe.
-
-
-    Note
-    ----
-    In case of `use_threads=True` the number of threads
-    that will be spawned will be gotten from os.cpu_count().
-
-    Parameters
-    ----------
-    table : str
-        AWS Glue Catalog table name.
-    database : str
-        AWS Glue Catalog database name.
-    filename_suffix: Union[str, List[str], None]
-        Suffix or List of suffixes to be read (e.g. [".gz.parquet", ".snappy.parquet"]).
-        If None, will try to read all files. (default)
-    filename_ignore_suffix: Union[str, List[str], None]
-        Suffix or List of suffixes for S3 keys to be ignored.(e.g. [".csv", "_SUCCESS"]).
-        If None, will try to read all files. (default)
-    catalog_id : str, optional
-        The ID of the Data Catalog from which to retrieve Databases.
-        If none is provided, the AWS account ID is used by default.
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]]
-        Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
-        This function MUST receive a single argument (Dict[str, str]) where keys are partition
-        names and values are partition values. Partition values will be always strings extracted from S3.
-        This function MUST return a bool, True to read the partition or False to ignore it.
-        Ignored if `dataset=False`.
-        E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/2.16.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
-    columns : List[str], optional
-        Names of columns to read from the file(s).
-    validate_schema:
-        Check that individual file schemas are all the same / compatible. Schemas within a
-        folder prefix should all be the same. Disable if you have schemas that are different
-        and want to disable this check.
-    categories: Optional[List[str]], optional
-        List of columns names that should be returned as pandas.Categorical.
-        Recommended for memory restricted environments.
-    safe : bool, default True
-        For certain data types, a cast is needed in order to store the
-        data in a pandas DataFrame or Series (e.g. timestamps are always
-        stored as nanoseconds in pandas). This option controls whether it
-        is a safe cast or not.
-    map_types : bool, default True
-        True to convert pyarrow DataTypes to pandas ExtensionDtypes. It is
-        used to override the default pandas type for conversion of built-in
-        pyarrow types or in absence of pandas_metadata in the Table schema.
-    chunked : bool
-        If True will break the data in smaller DataFrames (Non-deterministic number of lines).
-        Otherwise return a single DataFrame with the whole data.
-    use_threads : Union[bool, int]
-        True to enable concurrent requests, False to disable multiple threads.
-        If enabled os.cpu_count() will be used as the max number of threads.
-        If integer is provided, specified number is used.
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-    s3_additional_kwargs : Optional[Dict[str, Any]]
-        Forward to botocore requests, only "SSECustomerAlgorithm" and "SSECustomerKey" arguments will be considered.
-
-    Returns
-    -------
-    Union[pandas.DataFrame, Generator[pandas.DataFrame, None, None]]
-        Pandas DataFrame or a Generator in case of `chunked=True`.
-
-    Examples
-    --------
-    Reading Parquet Table
-
-    >>> import awswrangler as wr
-    >>> df = wr.s3.read_parquet_table(database='...', table='...')
-
-    Reading Parquet Table encrypted
-
-    >>> import awswrangler as wr
-    >>> df = wr.s3.read_parquet_table(
-    ...     database='...',
-    ...     table='...'
-    ...     s3_additional_kwargs={
-    ...         'ServerSideEncryption': 'aws:kms',
-    ...         'SSEKMSKeyId': 'YOUR_KMS_KEY_ARN'
-    ...     }
-    ... )
-
-    Reading Parquet Table in chunks (Chunk by file)
-
-    >>> import awswrangler as wr
-    >>> dfs = wr.s3.read_parquet_table(database='...', table='...', chunked=True)
-    >>> for df in dfs:
-    >>>     print(df)  # Smaller Pandas DataFrame
-
-    Reading Parquet Dataset with PUSH-DOWN filter over partitions
-
-    >>> import awswrangler as wr
-    >>> my_filter = lambda x: True if x["city"].startswith("new") else False
-    >>> df = wr.s3.read_parquet_table(path, dataset=True, partition_filter=my_filter)
-
-    """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
-    args: Dict[str, Any] = {"DatabaseName": database, "Name": table}
-    if catalog_id is not None:
-        args["CatalogId"] = catalog_id
-    res: Dict[str, Any] = client_glue.get_table(**args)
-    try:
-        location: str = res["Table"]["StorageDescriptor"]["Location"]
-        path: str = location if location.endswith("/") else f"{location}/"
-    except KeyError as ex:
-        raise exceptions.InvalidTable(f"Missing s3 location for {database}.{table}.") from ex
-    path_root: Optional[str] = None
-    paths: Union[str, List[str]] = path
-    # If filter is available, fetch & filter out partitions
-    # Then list objects & process individual object keys under path_root
-    if partition_filter is not None:
-        available_partitions_dict = _get_partitions(
-            database=database,
-            table=table,
-            catalog_id=catalog_id,
-            boto3_session=boto3_session,
-        )
-        available_partitions = list(_ensure_locations_are_valid(available_partitions_dict.keys()))
-        if available_partitions:
-            paths = []
-            path_root = path
-            partitions: Union[str, List[str]] = _apply_partition_filter(
-                path_root=path_root, paths=available_partitions, filter_func=partition_filter
-            )
-            for partition in partitions:
-                paths += _path2list(
-                    path=partition,
-                    boto3_session=boto3_session,
-                    suffix=filename_suffix,
-                    ignore_suffix=_get_path_ignore_suffix(path_ignore_suffix=filename_ignore_suffix),
-                    s3_additional_kwargs=s3_additional_kwargs,
-                )
-    df = read_parquet(
-        path=paths,
-        path_root=path_root,
-        path_suffix=filename_suffix if path_root is None else None,
-        path_ignore_suffix=filename_ignore_suffix if path_root is None else None,
-        columns=columns,
-        validate_schema=validate_schema,
-        categories=categories,
-        safe=safe,
-        map_types=map_types,
-        chunked=chunked,
-        dataset=True,
-        use_threads=use_threads,
-        boto3_session=boto3_session,
-        s3_additional_kwargs=s3_additional_kwargs,
-    )
-    partial_cast_function = functools.partial(
-        _data_types.cast_pandas_with_athena_types, dtype=_extract_partitions_dtypes_from_table_details(response=res)
-    )
-
-    if isinstance(df, pd.DataFrame):
-        return partial_cast_function(df)
-
-    # df is a generator, so map is needed for casting dtypes
-    return map(partial_cast_function, df)
-
-
-def _ensure_locations_are_valid(paths: Iterable[str]) -> Iterator[str]:
-    for path in paths:
-        suffix: str = path.rpartition("/")[2]
-        # If the suffix looks like a partition,
-        if (suffix != "") and (suffix.count("=") == 1):
-            # the path should end in a '/' character.
-            path = f"{path}/"
-        yield path
-
-
-@apply_configs
-def read_parquet_metadata(
-    path: Union[str, List[str]],
-    version_id: Optional[Union[str, Dict[str, str]]] = None,
-    path_suffix: Optional[str] = None,
-    path_ignore_suffix: Optional[str] = None,
-    ignore_empty: bool = True,
-    ignore_null: bool = False,
-    dtype: Optional[Dict[str, str]] = None,
-    sampling: float = 1.0,
-    dataset: bool = False,
-    use_threads: Union[bool, int] = True,
-    boto3_session: Optional[boto3.Session] = None,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
-) -> Tuple[Dict[str, str], Optional[Dict[str, str]]]:
-    """Read Apache Parquet file(s) metadata from a received S3 prefix or list of S3 objects paths.
-
-    The concept of Dataset goes beyond the simple idea of files and enable more
-    complex features like partitioning and catalog integration (AWS Glue Catalog).
-
-    This function accepts Unix shell-style wildcards in the path argument.
-    * (matches everything), ? (matches any single character),
-    [seq] (matches any character in seq), [!seq] (matches any character not in seq).
-    If you want to use a path which includes Unix shell-style wildcard characters (`*, ?, []`),
-    you can use `glob.escape(path)` before passing the path to this function.
-
-    Note
-    ----
-    In case of `use_threads=True` the number of threads
-    that will be spawned will be gotten from os.cpu_count().
-
-    Parameters
-    ----------
-    path : Union[str, List[str]]
-        S3 prefix (accepts Unix shell-style wildcards)
-        (e.g. s3://bucket/prefix) or list of S3 objects paths (e.g. [s3://bucket/key0, s3://bucket/key1]).
-    version_id: Optional[Union[str, Dict[str, str]]]
-        Version id of the object or mapping of object path to version id.
-        (e.g. {'s3://bucket/key0': '121212', 's3://bucket/key1': '343434'})
-    path_suffix: Union[str, List[str], None]
-        Suffix or List of suffixes to be read (e.g. [".gz.parquet", ".snappy.parquet"]).
-        If None, will try to read all files. (default)
-    path_ignore_suffix: Union[str, List[str], None]
-        Suffix or List of suffixes for S3 keys to be ignored.(e.g. [".csv", "_SUCCESS"]).
-        If None, will try to read all files. (default)
-    ignore_empty: bool
-        Ignore files with 0 bytes.
-    ignore_null: bool
-        Ignore columns with null type.
-    dtype : Dict[str, str], optional
-        Dictionary of columns names and Athena/Glue types to be casted.
-        Useful when you have columns with undetermined data types as partitions columns.
-        (e.g. {'col name': 'bigint', 'col2 name': 'int'})
-    sampling : float
-        Random sample ratio of files that will have the metadata inspected.
-        Must be `0.0 < sampling <= 1.0`.
-        The higher, the more accurate.
-        The lower, the faster.
-    dataset: bool
-        If True read a parquet dataset instead of simple file(s) loading all the related partitions as columns.
-    use_threads : bool, int
-        True to enable concurrent requests, False to disable multiple threads.
-        If enabled os.cpu_count() will be used as the max number of threads.
-        If integer is provided, specified number is used.
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-    s3_additional_kwargs : Optional[Dict[str, Any]]
-        Forward to botocore requests, only "SSECustomerAlgorithm" and "SSECustomerKey" arguments will be considered.
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]]
-        Forward kwargs to parquet reader currently only excepts "coerce_int96_timestamp_unit". Which can be used to cast
-        deprecated Parquet INT96 into a specified timestamp unit (e.g. "ms").
-
-    Returns
-    -------
-    Tuple[Dict[str, str], Optional[Dict[str, str]]]
-        columns_types: Dictionary with keys as column names and values as
-        data types (e.g. {'col0': 'bigint', 'col1': 'double'}). /
-        partitions_types: Dictionary with keys as partition names
-        and values as data types (e.g. {'col2': 'date'}).
-
-    Examples
-    --------
-    Reading all Parquet files (with partitions) metadata under a prefix
-
-    >>> import awswrangler as wr
-    >>> columns_types, partitions_types = wr.s3.read_parquet_metadata(path='s3://bucket/prefix/', dataset=True)
-
-    Reading all Parquet files metadata from a list
-
-    >>> import awswrangler as wr
-    >>> columns_types, partitions_types = wr.s3.read_parquet_metadata(path=[
-    ...     's3://bucket/filename0.parquet',
-    ...     's3://bucket/filename1.parquet'
-    ... ])
-
-    """
-    return _read_parquet_metadata(
-        path=path,
-        version_id=version_id,
-        path_suffix=path_suffix,
-        path_ignore_suffix=path_ignore_suffix,
-        ignore_empty=ignore_empty,
-        ignore_null=ignore_null,
-        dtype=dtype,
-        sampling=sampling,
-        dataset=dataset,
-        use_threads=use_threads,
-        s3_additional_kwargs=s3_additional_kwargs,
-        boto3_session=_utils.ensure_session(session=boto3_session),
-        pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-    )[:2]
-
-
 def _set_default_pyarrow_additional_kwargs(pyarrow_additional_kwargs: Optional[Dict[str, Any]]) -> Dict[str, Any]:
     if pyarrow_additional_kwargs is None:
         pyarrow_additional_kwargs = {}
     defaults = {
         "coerce_int96_timestamp_unit": None,
         "timestamp_as_object": False,
     }
```

### Comparing `lakeapi-0.8.0/lakeapi/_utils.py` & `lakeapi-0.9.1/lakeapi/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 from typing import Any, Callable, Dict, Generator, List, Optional, Sequence, Tuple, Union, cast
 
 import boto3
 import botocore.config
 import numpy as np
 import pandas as pd
 
-from awswrangler import _config, exceptions
-from lakeapi import __version__
-from awswrangler._config import apply_configs
+from lakeapi import __version__, exceptions, _config
+from lakeapi._config import apply_configs
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 Boto3PrimitivesType = Dict[str, Optional[str]]
 
 
 def ensure_session(session: Union[None, boto3.Session, Boto3PrimitivesType] = None) -> boto3.Session:
```

### Comparing `lakeapi-0.8.0/lakeapi/main.py` & `lakeapi-0.9.1/lakeapi/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 except ImportError:
     from typing_extensions import Literal
 import datetime
 
 import boto3
 import botocore
 import botocore.exceptions
-import awswrangler._utils
-import awswrangler as wr
 import pandas as pd
 from cachetools_ext.fs import FSLRUCache
 from botocache.botocache import botocache_context
 
 import lakeapi._read_parquet
 import lakeapi._cache
+import lakeapi._utils
+import lakeapi.exceptions
 
-DataType = Literal["book", "book_delta", "trades", "trades_mpid", "candles", "level_1", "funding", "open_interest", "liquiditions"]
+DataType = Literal[
+    "book", "book_delta", "trades", "trades_mpid", "candles", "level_1", "funding", "open_interest", "liquiditions",
+    "book_1m"
+]
 
 cache = FSLRUCache(ttl=8 * 60 * 60, path=".lake_cache/boto", maxsize=10_000)
 default_bucket = 'qnt.data/market-data/cryptofeed'
 is_anonymous_access = False
+_old_default_config = None
 
 
 def set_default_bucket(bucket: str) -> None:
     global default_bucket
     default_bucket = bucket
 
 def set_cache_size_limit(limit_bytes: int) -> None:
@@ -38,26 +42,31 @@
 
 def use_sample_data(anonymous_access: bool) -> None:
     '''
     Use sample data lake configuration, which is free for testing Lake.
 
     :param anonymous_access: Whether to enable anonymous AWS access, that can be used without AWS credentials.
     '''
-    global is_anonymous_access
+    global is_anonymous_access, _old_default_config
     set_default_bucket('sample.crypto.lake')
 
-    old_default_config = awswrangler._utils.default_botocore_config
+    if _old_default_config is None:
+        _old_default_config = lakeapi._utils.default_botocore_config
     def _anonymous_access_config() -> None:
-        config = old_default_config()
+        config = _old_default_config()
         config.signature_version = botocore.UNSIGNED
         return config
 
     if anonymous_access:
         is_anonymous_access = True
-        awswrangler._utils.default_botocore_config = _anonymous_access_config
+        lakeapi._utils.default_botocore_config = _anonymous_access_config
+    else:
+        is_anonymous_access = False
+        lakeapi._utils.default_botocore_config = _old_default_config
+
 
 def load_data(
     table: DataType,
     start: Optional[datetime.datetime] = None,
     end: Optional[datetime.datetime] = None,
     symbols: Optional[List[str]] = None,
     exchanges: Optional[List[str]] = None,
@@ -130,17 +139,17 @@
                 if int(ex.response['Error']['Code']) == 404:
                     # An error occurred (404) when calling the HeadObject operation: Not Found
                     cache.clear()
                     last_ex = ex
                     continue
                 else:
                     raise
-            except awswrangler.exceptions.NoFilesFound:
+            except lakeapi.exceptions.NoFilesFound:
                 if is_anonymous_access:
-                    raise awswrangler.exceptions.NoFilesFound("No data found for your query in the free sample dataset. Please subscribe to access more data.")
+                    raise lakeapi.exceptions.NoFilesFound("No data found for your query in the free sample dataset. Please subscribe to access more data.")
                 else:
                     raise
         else:
             # got error 404 both before and after the cache.clear()
             raise last_ex
     if drop_partition_cols:
         # useful when loading just one symbol and exchange
@@ -223,15 +232,15 @@
             last_modified_end=last_modified_end,
             # ignore_empty=ignore_empty,
             s3_additional_kwargs={},
         )
         path_root = lakeapi._read_parquet._get_path_root(path=path, dataset=True)
     paths = lakeapi._read_parquet._apply_partition_filter(path_root=path_root, paths=paths, filter_func=partition_filter)
     if len(paths) < 1:
-        raise wr.exceptions.NoFilesFound(f"No files Found on: {path}.")
+        raise lakeapi.exceptions.NoFilesFound(f"No files Found on: {path}.")
     return [_path_to_dict(path) for path in paths]
 
 def _path_to_dict(path: str) -> Dict[str, Any]:
     *_, table, exchange, symbol, dt, filename = path.split('/')
     return {
         'table': table,
         'exchange': exchange.lstrip('exchange='),
```

### Comparing `lakeapi-0.8.0/lakeapi/orderbook.py` & `lakeapi-0.9.1/lakeapi/orderbook.py`

 * *Files identical despite different names*

### Comparing `lakeapi-0.8.0/lakeapi.egg-info/PKG-INFO` & `lakeapi-0.9.1/lakeapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeapi
-Version: 0.8.0
+Version: 0.9.1
 Summary: API for accessing Lake crypto market data
 Home-page: https://github.com/crypto-lake/lake-api
 Author: Jan Skoda
 Author-email: skoda@jskoda.cz
 License: Apache 2 license
 Keywords: lakeapi
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 License-File: LICENSE
 License-File: NOTICE.rst
 License-File: AUTHORS.rst
 
 ========
 Lake API
@@ -89,14 +90,20 @@
 working directory.
 
 
 =======
 History
 =======
 
+0.9.1 (2023-11-03)
+------------------
+
+* awswrangler dependency removed, pandas 2 support added
+* python3.12 support
+
 0.8.0 (2023-09-18)
 ------------------
 
 * grow default cache size limit
 * nicer error messages when data are missing
 * pass and print warning when file is corrupted
```

### Comparing `lakeapi-0.8.0/lakeapi.egg-info/SOURCES.txt` & `lakeapi-0.9.1/lakeapi.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -20,19 +20,25 @@
 docs/readme.rst
 docs/usage.rst
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 lakeapi/__init__.py
 lakeapi/_cache.py
+lakeapi/_config.py
+lakeapi/_data_types.py
+lakeapi/_describe.py
+lakeapi/_fs.py
 lakeapi/_read.py
 lakeapi/_read_parquet.py
 lakeapi/_utils.py
+lakeapi/exceptions.py
 lakeapi/main.py
 lakeapi/orderbook.py
+lakeapi/test.py
 lakeapi.egg-info/PKG-INFO
 lakeapi.egg-info/SOURCES.txt
 lakeapi.egg-info/dependency_links.txt
 lakeapi.egg-info/entry_points.txt
 lakeapi.egg-info/not-zip-safe
 lakeapi.egg-info/requires.txt
 lakeapi.egg-info/top_level.txt
```

### Comparing `lakeapi-0.8.0/setup.py` & `lakeapi-0.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
-   'Click>=7.0', 'pandas>=1.0.5,<2', 'boto3>=1.24,<2', 'cachetools_ext>=0.0.8,<0.1.0', 'botocache>=0.0.4,<0.1.0',
-   'awswrangler>=2.16.1,<2.20.0', 'joblib>=1.0.0', 'tqdm>=4,<5',
+   'pandas>=1.0.5', 'boto3>=1.24,<2', 'cachetools_ext>=0.0.8,<0.1.0', 'botocache>=0.0.4,<0.1.0',
+   'joblib>=1.0.0', 'tqdm>=4,<5', 'pyarrow>=2.0.0,<15',
    'typing-extensions>=4.0,<5; python_version < \'3.8\''
 ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Jan Skoda",
@@ -29,14 +29,15 @@
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     description="API for accessing Lake crypto market data",
     entry_points={
         'console_scripts': [
             'lakeapi=lakeapi.cli:main',
         ],
     },
@@ -46,10 +47,10 @@
     include_package_data=True,
     keywords='lakeapi',
     name='lakeapi',
     packages=find_packages(include=['lakeapi', 'lakeapi.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/crypto-lake/lake-api',
-    version='0.8.0',
+    version='0.9.1',
     zip_safe=False,
 )
```

### Comparing `lakeapi-0.8.0/tests/test_lakeapi.py` & `lakeapi-0.9.1/tests/test_lakeapi.py`

 * *Files identical despite different names*

### Comparing `lakeapi-0.8.0/tests/test_orderbook.py` & `lakeapi-0.9.1/tests/test_orderbook.py`

 * *Files identical despite different names*

