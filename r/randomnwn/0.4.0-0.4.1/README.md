# Comparing `tmp/randomnwn-0.4.0.tar.gz` & `tmp/randomnwn-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randomnwn-0.4.0.tar", last modified: Wed May  1 21:34:02 2024, max compression
+gzip compressed data, was "randomnwn-0.4.1.tar", last modified: Thu May  2 19:55:21 2024, max compression
```

## Comparing `randomnwn-0.4.0.tar` & `randomnwn-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:34:02.647827 randomnwn-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 21:33:57.000000 randomnwn-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-01 21:34:02.647827 randomnwn-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-01 21:33:57.000000 randomnwn-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:34:02.643827 randomnwn-0.4.0/randomnwn/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/fromtext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/line_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/nanowires.py
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/units.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 21:33:57.000000 randomnwn-0.4.0/randomnwn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:34:02.647827 randomnwn-0.4.0/randomnwn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-01 21:34:02.000000 randomnwn-0.4.0/randomnwn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-01 21:34:02.000000 randomnwn-0.4.0/randomnwn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:34:02.000000 randomnwn-0.4.0/randomnwn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 21:34:02.000000 randomnwn-0.4.0/randomnwn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:34:02.647827 randomnwn-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-01 21:33:57.000000 randomnwn-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:34:02.647827 randomnwn-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-01 21:33:57.000000 randomnwn-0.4.0/tests/test_nanowires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:55:21.032698 randomnwn-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-02 19:55:14.000000 randomnwn-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-02 19:55:21.032698 randomnwn-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-02 19:55:14.000000 randomnwn-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:55:21.032698 randomnwn-0.4.1/randomnwn/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/fromtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/line_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/nanowires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:55:21.032698 randomnwn-0.4.1/randomnwn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-02 19:55:21.000000 randomnwn-0.4.1/randomnwn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-02 19:55:21.000000 randomnwn-0.4.1/randomnwn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:55:21.000000 randomnwn-0.4.1/randomnwn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 19:55:21.000000 randomnwn-0.4.1/randomnwn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:55:21.032698 randomnwn-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-02 19:55:14.000000 randomnwn-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:55:21.032698 randomnwn-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-02 19:55:14.000000 randomnwn-0.4.1/tests/test_nanowires.py
```

### Comparing `randomnwn-0.4.0/LICENSE` & `randomnwn-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/PKG-INFO` & `randomnwn-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: randomnwn
-Version: 0.4.0
+Version: 0.4.1
 Summary: Modelling and analyzing random nanowire networks in Python.
 Home-page: https://github.com/marcus-k/Random-NWNs
 Author: Marcus Kasdorf
 Author-email: marcus.kasdorf@ucalgary.ca
 License: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `randomnwn-0.4.0/README.md` & `randomnwn-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/randomnwn/__init__.py` & `randomnwn-0.4.1/randomnwn/__init__.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/randomnwn/_models.py` & `randomnwn-0.4.1/randomnwn/_models.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/randomnwn/calculations.py` & `randomnwn-0.4.1/randomnwn/calculations.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/randomnwn/dynamics.py` & `randomnwn-0.4.1/randomnwn/dynamics.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/randomnwn/fromtext.py` & `randomnwn-0.4.1/randomnwn/fromtext.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/randomnwn/line_functions.py` & `randomnwn-0.4.1/randomnwn/line_functions.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/randomnwn/nanowires.py` & `randomnwn-0.4.1/randomnwn/nanowires.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/randomnwn/plotting.py` & `randomnwn-0.4.1/randomnwn/plotting.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/randomnwn/units.py` & `randomnwn-0.4.1/randomnwn/units.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/randomnwn.egg-info/PKG-INFO` & `randomnwn-0.4.1/randomnwn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: randomnwn
-Version: 0.4.0
+Version: 0.4.1
 Summary: Modelling and analyzing random nanowire networks in Python.
 Home-page: https://github.com/marcus-k/Random-NWNs
 Author: Marcus Kasdorf
 Author-email: marcus.kasdorf@ucalgary.ca
 License: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `randomnwn-0.4.0/setup.py` & `randomnwn-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.0/tests/test_nanowires.py` & `randomnwn-0.4.1/tests/test_nanowires.py`

 * *Files identical despite different names*

