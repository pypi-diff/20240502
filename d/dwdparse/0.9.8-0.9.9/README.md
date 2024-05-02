# Comparing `tmp/dwdparse-0.9.8.tar.gz` & `tmp/dwdparse-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwdparse-0.9.8.tar", last modified: Fri Sep 15 07:53:58 2023, max compression
+gzip compressed data, was "dwdparse-0.9.9.tar", last modified: Tue Dec 19 11:10:41 2023, max compression
```

## Comparing `dwdparse-0.9.8.tar` & `dwdparse-0.9.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 07:53:58.654420 dwdparse-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-09-15 07:53:52.000000 dwdparse-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2023-09-15 07:53:58.654420 dwdparse-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2023-09-15 07:53:52.000000 dwdparse-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 07:53:58.650420 dwdparse-0.9.8/dwdparse/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-09-15 07:53:52.000000 dwdparse-0.9.8/dwdparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-15 07:53:52.000000 dwdparse-0.9.8/dwdparse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2023-09-15 07:53:52.000000 dwdparse-0.9.8/dwdparse/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2023-09-15 07:53:52.000000 dwdparse-0.9.8/dwdparse/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    34599 2023-09-15 07:53:52.000000 dwdparse-0.9.8/dwdparse/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2023-09-15 07:53:52.000000 dwdparse-0.9.8/dwdparse/stations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2023-09-15 07:53:52.000000 dwdparse-0.9.8/dwdparse/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-09-15 07:53:52.000000 dwdparse-0.9.8/dwdparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 07:53:58.654420 dwdparse-0.9.8/dwdparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2023-09-15 07:53:58.000000 dwdparse-0.9.8/dwdparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      451 2023-09-15 07:53:58.000000 dwdparse-0.9.8/dwdparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-15 07:53:58.000000 dwdparse-0.9.8/dwdparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-15 07:53:58.000000 dwdparse-0.9.8/dwdparse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-15 07:53:58.000000 dwdparse-0.9.8/dwdparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-15 07:53:58.000000 dwdparse-0.9.8/dwdparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-09-15 07:53:52.000000 dwdparse-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-15 07:53:58.654420 dwdparse-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      928 2023-09-15 07:53:52.000000 dwdparse-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 07:53:58.654420 dwdparse-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17781 2023-09-15 07:53:52.000000 dwdparse-0.9.8/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-15 07:53:52.000000 dwdparse-0.9.8/tests/test_stations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-09-15 07:53:52.000000 dwdparse-0.9.8/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 11:10:41.076485 dwdparse-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-19 11:10:34.000000 dwdparse-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2023-12-19 11:10:41.076485 dwdparse-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2023-12-19 11:10:34.000000 dwdparse-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 11:10:41.072485 dwdparse-0.9.9/dwdparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-19 11:10:34.000000 dwdparse-0.9.9/dwdparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-19 11:10:34.000000 dwdparse-0.9.9/dwdparse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-12-19 11:10:34.000000 dwdparse-0.9.9/dwdparse/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2023-12-19 11:10:34.000000 dwdparse-0.9.9/dwdparse/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34599 2023-12-19 11:10:34.000000 dwdparse-0.9.9/dwdparse/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2023-12-19 11:10:34.000000 dwdparse-0.9.9/dwdparse/stations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2023-12-19 11:10:34.000000 dwdparse-0.9.9/dwdparse/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-19 11:10:34.000000 dwdparse-0.9.9/dwdparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 11:10:41.072485 dwdparse-0.9.9/dwdparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2023-12-19 11:10:41.000000 dwdparse-0.9.9/dwdparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2023-12-19 11:10:41.000000 dwdparse-0.9.9/dwdparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 11:10:41.000000 dwdparse-0.9.9/dwdparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-19 11:10:41.000000 dwdparse-0.9.9/dwdparse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-19 11:10:41.000000 dwdparse-0.9.9/dwdparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-19 11:10:41.000000 dwdparse-0.9.9/dwdparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-19 11:10:34.000000 dwdparse-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 11:10:41.076485 dwdparse-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2023-12-19 11:10:34.000000 dwdparse-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 11:10:41.072485 dwdparse-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17781 2023-12-19 11:10:34.000000 dwdparse-0.9.9/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-19 11:10:34.000000 dwdparse-0.9.9/tests/test_stations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-12-19 11:10:34.000000 dwdparse-0.9.9/tests/test_units.py
```

### Comparing `dwdparse-0.9.8/LICENSE` & `dwdparse-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.8/PKG-INFO` & `dwdparse-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdparse
-Version: 0.9.8
+Version: 0.9.9
 Summary: Parsers for DWD's open weather data.
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/
 Project-URL: Tracker, https://github.com/jdemaeyer/dwdparse/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dwdparse Version: 0.9.8 Summary: Parsers for DWD's
+Metadata-Version: 2.1 Name: dwdparse Version: 0.9.9 Summary: Parsers for DWD's
 open weather data. Author: Jakob de Maeyer Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/ Project-URL:
 Tracker, https://github.com/jdemaeyer/dwdparse/issues/ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Provides-Extra:
 lean Requires-Dist: ijson; extra == "lean" # dwdparse [![Build Status](https://
```

### Comparing `dwdparse-0.9.8/README.md` & `dwdparse-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.8/dwdparse/api.py` & `dwdparse-0.9.9/dwdparse/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from dwdparse.parsers import get_parser
 from dwdparse.utils import fetch
 
 
 logger = logging.getLogger(__name__)
 
 
-def parse(path, **extra):
-    return get_parser(pathlib.Path(path).name)().parse(path, **extra)
+def parse(path, parser=None, **extra):
+    parser = parser or get_parser(pathlib.Path(path).name)()
+    return parser.parse(path, **extra)
 
 
-def parse_url(url):
+def parse_url(url, parser=None):
     with tempfile.TemporaryDirectory() as tmpdir:
         file_path = _download(url, tmpdir)
-        parser = get_parser(file_path.name)()
+        parser = parser or get_parser(file_path.name)()
         extra = {
             kwarg: _download(extra_url, tmpdir)
             for kwarg, extra_url in parser.get_extra_urls(file_path).items()
         }
         yield from parser.parse(file_path, **extra)
```

### Comparing `dwdparse-0.9.8/dwdparse/cli.py` & `dwdparse-0.9.9/dwdparse/cli.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.8/dwdparse/parsers.py` & `dwdparse-0.9.9/dwdparse/parsers.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.8/dwdparse/stations.py` & `dwdparse-0.9.9/dwdparse/stations.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.8/dwdparse/units.py` & `dwdparse-0.9.9/dwdparse/units.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.8/dwdparse.egg-info/PKG-INFO` & `dwdparse-0.9.9/dwdparse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdparse
-Version: 0.9.8
+Version: 0.9.9
 Summary: Parsers for DWD's open weather data.
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/
 Project-URL: Tracker, https://github.com/jdemaeyer/dwdparse/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dwdparse Version: 0.9.8 Summary: Parsers for DWD's
+Metadata-Version: 2.1 Name: dwdparse Version: 0.9.9 Summary: Parsers for DWD's
 open weather data. Author: Jakob de Maeyer Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/ Project-URL:
 Tracker, https://github.com/jdemaeyer/dwdparse/issues/ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Provides-Extra:
 lean Requires-Dist: ijson; extra == "lean" # dwdparse [![Build Status](https://
```

### Comparing `dwdparse-0.9.8/setup.py` & `dwdparse-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.8/tests/test_parsers.py` & `dwdparse-0.9.9/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.8/tests/test_stations.py` & `dwdparse-0.9.9/tests/test_stations.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.8/tests/test_units.py` & `dwdparse-0.9.9/tests/test_units.py`

 * *Files identical despite different names*

