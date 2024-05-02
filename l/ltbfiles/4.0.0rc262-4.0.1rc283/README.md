# Comparing `tmp/ltbfiles-4.0.0rc262.tar.gz` & `tmp/ltbfiles-4.0.1rc283.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltbfiles-4.0.0rc262.tar", last modified: Mon Apr 22 12:55:24 2024, max compression
+gzip compressed data, was "ltbfiles-4.0.1rc283.tar", last modified: Thu May  2 12:51:04 2024, max compression
```

## Comparing `ltbfiles-4.0.0rc262.tar` & `ltbfiles-4.0.1rc283.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:55:24.706880 ltbfiles-4.0.0rc262/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2024-04-22 12:55:16.000000 ltbfiles-4.0.0rc262/LICENSE_GPL_v3.txt
--rw-r--r--   0 root         (0) root         (0)     2992 2024-04-22 12:55:24.706880 ltbfiles-4.0.0rc262/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2057 2024-04-22 12:55:16.000000 ltbfiles-4.0.0rc262/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-04-22 12:55:16.000000 ltbfiles-4.0.0rc262/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:55:24.702880 ltbfiles-4.0.0rc262/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:55:24.704880 ltbfiles-4.0.0rc262/python/ltbfiles/
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-04-22 12:55:16.000000 ltbfiles-4.0.0rc262/python/ltbfiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2024-04-22 12:55:16.000000 ltbfiles-4.0.0rc262/python/ltbfiles/autoimagelog.py
--rw-rw-rw-   0 root         (0) root         (0)    24062 2024-04-22 12:55:16.000000 ltbfiles-4.0.0rc262/python/ltbfiles/ltbfiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 12:55:24.705880 ltbfiles-4.0.0rc262/python/ltbfiles.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2992 2024-04-22 12:55:24.000000 ltbfiles-4.0.0rc262/python/ltbfiles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      325 2024-04-22 12:55:24.000000 ltbfiles-4.0.0rc262/python/ltbfiles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 12:55:24.000000 ltbfiles-4.0.0rc262/python/ltbfiles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-22 12:55:24.000000 ltbfiles-4.0.0rc262/python/ltbfiles.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-22 12:55:24.000000 ltbfiles-4.0.0rc262/python/ltbfiles.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-04-22 12:55:24.706880 ltbfiles-4.0.0rc262/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 12:51:04.562434 ltbfiles-4.0.1rc283/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2024-05-02 12:50:56.000000 ltbfiles-4.0.1rc283/LICENSE_GPL_v3.txt
+-rw-r--r--   0 root         (0) root         (0)     3030 2024-05-02 12:51:04.562434 ltbfiles-4.0.1rc283/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-05-02 12:50:56.000000 ltbfiles-4.0.1rc283/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-05-02 12:50:56.000000 ltbfiles-4.0.1rc283/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 12:51:04.559434 ltbfiles-4.0.1rc283/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 12:51:04.560433 ltbfiles-4.0.1rc283/python/ltbfiles/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-02 12:50:56.000000 ltbfiles-4.0.1rc283/python/ltbfiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2024-05-02 12:50:56.000000 ltbfiles-4.0.1rc283/python/ltbfiles/autoimagelog.py
+-rw-rw-rw-   0 root         (0) root         (0)    24053 2024-05-02 12:50:56.000000 ltbfiles-4.0.1rc283/python/ltbfiles/ltbfiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 12:51:04.561433 ltbfiles-4.0.1rc283/python/ltbfiles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3030 2024-05-02 12:51:04.000000 ltbfiles-4.0.1rc283/python/ltbfiles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-02 12:51:04.000000 ltbfiles-4.0.1rc283/python/ltbfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 12:51:04.000000 ltbfiles-4.0.1rc283/python/ltbfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-02 12:51:04.000000 ltbfiles-4.0.1rc283/python/ltbfiles.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-02 12:51:04.000000 ltbfiles-4.0.1rc283/python/ltbfiles.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-02 12:51:04.562434 ltbfiles-4.0.1rc283/setup.cfg
```

### Comparing `ltbfiles-4.0.0rc262/LICENSE_GPL_v3.txt` & `ltbfiles-4.0.1rc283/LICENSE_GPL_v3.txt`

 * *Files identical despite different names*

### Comparing `ltbfiles-4.0.0rc262/PKG-INFO` & `ltbfiles-4.0.1rc283/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 4.0.0rc262
+Version: 4.0.1rc283
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
-Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
+Project-URL: Docs, https://ltb_berlin.gitlab.io/ltb_files/ltbfiles.html
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -32,15 +32,15 @@
 
 ## Installation
 
 ### Python
 
 [![Pyversions](https://img.shields.io/pypi/pyversions/ltbfiles.svg?style=flat-square)](https://pypi.python.org/pypi/ltbfiles)
 
-Users of Python can install directly from pypi using:
+Users of Python can install directly from [pypi](https://pypi.org/project/ltbfiles/) using:
 
 ```bash
 pip install ltbfiles
 ```
 
 ### Matlab
```

### Comparing `ltbfiles-4.0.0rc262/README.md` & `ltbfiles-4.0.1rc283/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## Installation
 
 ### Python
 
 [![Pyversions](https://img.shields.io/pypi/pyversions/ltbfiles.svg?style=flat-square)](https://pypi.python.org/pypi/ltbfiles)
 
-Users of Python can install directly from pypi using:
+Users of Python can install directly from [pypi](https://pypi.org/project/ltbfiles/) using:
 
 ```bash
 pip install ltbfiles
 ```
 
 ### Matlab
```

### Comparing `ltbfiles-4.0.0rc262/pyproject.toml` & `ltbfiles-4.0.1rc283/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "pytest",
     "pytest-cov"
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/ltb_berlin/ltb_files"
 "Bug Tracker" = "https://gitlab.com/ltb_berlin/ltb_files/-/issues"
-"Wiki" = "https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home"
+"Docs" = "https://ltb_berlin.gitlab.io/ltb_files/ltbfiles.html"
 
 [tool.setuptools.packages.find]
 where = ["python"]
 include = ["ltbfiles"]
 exclude = ["tests"]
 
 [tool.setuptools.dynamic]
```

### Comparing `ltbfiles-4.0.0rc262/python/ltbfiles/autoimagelog.py` & `ltbfiles-4.0.1rc283/python/ltbfiles/autoimagelog.py`

 * *Files identical despite different names*

### Comparing `ltbfiles-4.0.0rc262/python/ltbfiles/ltbfiles.py` & `ltbfiles-4.0.1rc283/python/ltbfiles/ltbfiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 __pdoc__['Spectra.head'] = 'A list[dict] containing the spectra metadata. Its len is "n"'
 
 
 SPEC_EXTENSIONS = ['.ary', '.aryx']
 """Default set of supported extensions for Aryelle spectra files."""
 
 
-TIMESTAMP_MISSING = "1970-01-01T00:00:00.000Z"
+TIMESTAMP_MISSING = ""
 """Timestamp used in case it is missing"""
 
 
 METADATA_HEADERS_V1 = (
     "version", "systemSerial", "spectrometerSerial", "setupName", "softwareVersion", \
     "timeStampKernelStart", "timeStampMeasurement", "ramanExcitationWavelength", "movementMode", "posX", \
     "posY", "posZ", "posA", "posB", "posC", \
@@ -64,15 +64,15 @@
 
 METADATA_DEFAULT_V1 = (
     1, "", "", "", "", \
     TIMESTAMP_MISSING, TIMESTAMP_MISSING, np.NaN, "AtRest", np.NaN, \
     np.NaN, np.NaN, np.NaN, np.NaN, np.NaN, \
     "", "", "", 1, np.NaN, \
     "Open", False, np.NaN, np.NaN, np.NaN, \
-    0, "", np.NaN, np.NaN, np.NaN, \
+    0, TIMESTAMP_MISSING, np.NaN, np.NaN, np.NaN, \
     np.NaN, np.NaN, np.NaN, np.NaN, np.NaN, \
     np.NaN, np.NaN, np.NaN, np.NaN, np.NaN, \
     np.NaN, np.NaN, np.NaN, np.NaN, True, \
     np.NaN, np.NaN, np.NaN, np.NaN, np.NaN
 )
 """Default values for unified metadata, if missing."""
```

### Comparing `ltbfiles-4.0.0rc262/python/ltbfiles.egg-info/PKG-INFO` & `ltbfiles-4.0.1rc283/python/ltbfiles.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 4.0.0rc262
+Version: 4.0.1rc283
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
-Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
+Project-URL: Docs, https://ltb_berlin.gitlab.io/ltb_files/ltbfiles.html
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -32,15 +32,15 @@
 
 ## Installation
 
 ### Python
 
 [![Pyversions](https://img.shields.io/pypi/pyversions/ltbfiles.svg?style=flat-square)](https://pypi.python.org/pypi/ltbfiles)
 
-Users of Python can install directly from pypi using:
+Users of Python can install directly from [pypi](https://pypi.org/project/ltbfiles/) using:
 
 ```bash
 pip install ltbfiles
 ```
 
 ### Matlab
```

