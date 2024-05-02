# Comparing `tmp/pfc_geometry-0.2.5.tar.gz` & `tmp/pfc_geometry-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfc_geometry-0.2.5.tar", last modified: Wed May  1 08:46:13 2024, max compression
+gzip compressed data, was "pfc_geometry-0.2.6.tar", last modified: Thu May  2 13:40:48 2024, max compression
```

## Comparing `pfc_geometry-0.2.5.tar` & `pfc_geometry-0.2.6.tar`

### file list

```diff
@@ -1,31 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:46:13.280727 pfc_geometry-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-01 08:46:13.280727 pfc_geometry-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:46:13.276727 pfc_geometry-0.2.5/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/coordinate_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/geometry/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:46:13.280727 pfc_geometry-0.2.5/pfc_geometry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-01 08:46:13.000000 pfc_geometry-0.2.5/pfc_geometry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-01 08:46:13.000000 pfc_geometry-0.2.5/pfc_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:46:13.000000 pfc_geometry-0.2.5/pfc_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 08:46:13.000000 pfc_geometry-0.2.5/pfc_geometry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 08:46:13.000000 pfc_geometry-0.2.5/pfc_geometry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-01 08:46:13.280727 pfc_geometry-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:46:13.280727 pfc_geometry-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_coord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-01 08:45:58.000000 pfc_geometry-0.2.5/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:40:48.629759 pfc_geometry-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:40:48.621759 pfc_geometry-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:40:48.621759 pfc_geometry-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/.github/workflows/publish_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:40:48.625759 pfc_geometry-0.2.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-02 13:40:48.629759 pfc_geometry-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:40:48.625759 pfc_geometry-0.2.6/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/geometry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/geometry/coordinate_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/geometry/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/geometry/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/geometry/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/geometry/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/geometry/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/geometry/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/geometry/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:40:48.629759 pfc_geometry-0.2.6/pfc_geometry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-02 13:40:48.000000 pfc_geometry-0.2.6/pfc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-02 13:40:48.000000 pfc_geometry-0.2.6/pfc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:40:48.000000 pfc_geometry-0.2.6/pfc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 13:40:48.000000 pfc_geometry-0.2.6/pfc_geometry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 13:40:48.000000 pfc_geometry-0.2.6/pfc_geometry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:40:48.629759 pfc_geometry-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:40:48.625759 pfc_geometry-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79931 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/tests/quat_body_diff_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/tests/test_coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/tests/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/tests/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/tests/test_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/tests/test_remove_outliers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-02 13:40:35.000000 pfc_geometry-0.2.6/tests/test_transform.py
```

### Comparing `pfc_geometry-0.2.5/LICENSE` & `pfc_geometry-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/PKG-INFO` & `pfc_geometry-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: pfc_geometry
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for handling 3D geometry with a nice interface
-Home-page: https://github.com/PyFlightCoach/geometry
-Author: Thomas David
-Author-email: thomasdavid0@gmail.com
+Author-email: Thomas David <thomasdavid0@gmail.com>
+License: GNU GPL v3
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: numpy; extra == "dev"
+Requires-Dist: pandas; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # geometry #
 
 Tools for handling 3D geometry, mostly just adds a nice interface to various geometric enterties. Each geometric entity can also be a vector of geometric entities. Each entity wraps a numpy array with the relevant number of columns labelled according to the cols class property and rows equal to the number of elements in the vector. Attribute access to each column is available and returns a numpy array. 
 
 Where operations are supported between geometric types the size of the output is inferred based on the length of the inputs. Where the two vectors of entities are of the same length, elementwise operations are performed. Where one vector is length one and the other is greater than one then the operation will be performed on every element of the longer vector. 
 
 Magic methods are used extensively and the function of operators are logical for each type. If unsure what the logical option is then check the code where it should be pretty clear. 
 
 Many convenience methods and constructors are available. Documentation is limited but if you need something it has probably already been written so check the code first. 
 
-
 Some examples are available here: https://pfcdocumentation.readthedocs.io/pyflightcoach/geometry.html
 
 now available on pypi:
 ```bash
     pip install pfc-geometry
 ```
```

### Comparing `pfc_geometry-0.2.5/README.md` & `pfc_geometry-0.2.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 
 Where operations are supported between geometric types the size of the output is inferred based on the length of the inputs. Where the two vectors of entities are of the same length, elementwise operations are performed. Where one vector is length one and the other is greater than one then the operation will be performed on every element of the longer vector. 
 
 Magic methods are used extensively and the function of operators are logical for each type. If unsure what the logical option is then check the code where it should be pretty clear. 
 
 Many convenience methods and constructors are available. Documentation is limited but if you need something it has probably already been written so check the code first. 
 
-
 Some examples are available here: https://pfcdocumentation.readthedocs.io/pyflightcoach/geometry.html
 
 now available on pypi:
 ```bash
     pip install pfc-geometry
 ```
```

### Comparing `pfc_geometry-0.2.5/geometry/__init__.py` & `pfc_geometry-0.2.6/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/geometry/base.py` & `pfc_geometry-0.2.6/geometry/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
             a = self.tile(len(bdat))
         else:
             a = self
         return func(a, bdat)
     
     return wrapper
 
-
 class Base:
     __array_priority__ = 15.0   # this is a quirk of numpy so the __r*__ methods here take priority
     cols=[]
     from_np_base = []
     from_np = []
     def __init__(self, *args, **kwargs):
         if len(kwargs) > 0:
```

### Comparing `pfc_geometry-0.2.5/geometry/coordinate_frame.py` & `pfc_geometry-0.2.6/geometry/coordinate_frame.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/geometry/gps.py` & `pfc_geometry-0.2.6/geometry/gps.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/geometry/mass.py` & `pfc_geometry-0.2.6/geometry/mass.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/geometry/point.py` & `pfc_geometry-0.2.6/geometry/point.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/geometry/quaternion.py` & `pfc_geometry-0.2.6/geometry/quaternion.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/geometry/time.py` & `pfc_geometry-0.2.6/geometry/time.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/geometry/transformation.py` & `pfc_geometry-0.2.6/geometry/transformation.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/pfc_geometry.egg-info/PKG-INFO` & `pfc_geometry-0.2.6/pfc_geometry.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: pfc_geometry
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for handling 3D geometry with a nice interface
-Home-page: https://github.com/PyFlightCoach/geometry
-Author: Thomas David
-Author-email: thomasdavid0@gmail.com
+Author-email: Thomas David <thomasdavid0@gmail.com>
+License: GNU GPL v3
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: numpy; extra == "dev"
+Requires-Dist: pandas; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # geometry #
 
 Tools for handling 3D geometry, mostly just adds a nice interface to various geometric enterties. Each geometric entity can also be a vector of geometric entities. Each entity wraps a numpy array with the relevant number of columns labelled according to the cols class property and rows equal to the number of elements in the vector. Attribute access to each column is available and returns a numpy array. 
 
 Where operations are supported between geometric types the size of the output is inferred based on the length of the inputs. Where the two vectors of entities are of the same length, elementwise operations are performed. Where one vector is length one and the other is greater than one then the operation will be performed on every element of the longer vector. 
 
 Magic methods are used extensively and the function of operators are logical for each type. If unsure what the logical option is then check the code where it should be pretty clear. 
 
 Many convenience methods and constructors are available. Documentation is limited but if you need something it has probably already been written so check the code first. 
 
-
 Some examples are available here: https://pfcdocumentation.readthedocs.io/pyflightcoach/geometry.html
 
 now available on pypi:
 ```bash
     pip install pfc-geometry
 ```
```

### Comparing `pfc_geometry-0.2.5/tests/test_base.py` & `pfc_geometry-0.2.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/tests/test_coord.py` & `pfc_geometry-0.2.6/tests/test_coord.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/tests/test_gps.py` & `pfc_geometry-0.2.6/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/tests/test_mass.py` & `pfc_geometry-0.2.6/tests/test_mass.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/tests/test_point.py` & `pfc_geometry-0.2.6/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/tests/test_quaternion.py` & `pfc_geometry-0.2.6/tests/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.2.5/tests/test_transform.py` & `pfc_geometry-0.2.6/tests/test_transform.py`

 * *Files identical despite different names*

