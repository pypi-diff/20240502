# Comparing `tmp/hazard_map-0.2.0.tar.gz` & `tmp/hazard_map-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazard_map-0.2.0.tar", max compression
+gzip compressed data, was "hazard_map-0.2.1.tar", max compression
```

## Comparing `hazard_map-0.2.0.tar` & `hazard_map-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2523 2024-04-19 15:58:27.141956 hazard_map-0.2.0/hazard_map/__init__.py
--rw-r--r--   0        0        0    16039 2024-04-19 15:58:27.141956 hazard_map-0.2.0/hazard_map/hazard_map.py
--rw-r--r--   0        0        0      835 2024-04-19 15:58:27.141956 hazard_map-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2798 2024-04-19 15:58:27.141956 hazard_map-0.2.0/readme.md
--rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 hazard_map-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2523 2024-05-02 10:55:17.115293 hazard_map-0.2.1/hazard_map/__init__.py
+-rw-r--r--   0        0        0    16039 2024-05-02 10:55:17.115293 hazard_map-0.2.1/hazard_map/hazard_map.py
+-rw-r--r--   0        0        0      835 2024-05-02 10:55:17.115293 hazard_map-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2798 2024-05-02 10:55:17.116293 hazard_map-0.2.1/readme.md
+-rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 hazard_map-0.2.1/PKG-INFO
```

### Comparing `hazard_map-0.2.0/hazard_map/__init__.py` & `hazard_map-0.2.1/hazard_map/__init__.py`

 * *Files identical despite different names*

### Comparing `hazard_map-0.2.0/hazard_map/hazard_map.py` & `hazard_map-0.2.1/hazard_map/hazard_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         """Allows nodes to be sorted according to their kind and number."""
         if list(Kind).index(self.kind) > list(Kind).index(other.kind):
             return True
         else:
             return self.number > other.number
 
 
-ZERO_PADDING_DIGITS = 2
+ZERO_PADDING_DIGITS = 3
 DEFAULT_RENDERING_DPI = 480
 
 NODE_MATCHER = re.compile(r'^(?P<kind>H|CA|CO)-?(?P<number>\d+)$')
 MAPPING_MATCHER = re.compile(r'^\s*[Y]\s*$', re.I)
 
 KIND_STR_DICT = {
     'H': Kind.HAZARD,
```

### Comparing `hazard_map-0.2.0/pyproject.toml` & `hazard_map-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hazard-map"
-version = "0.2.0"
+version = "0.2.1"
 description = "Build and analyze a network model of hazards, causes, and controls"
 authors = ["Thom Cameron <thomcm@proton.me>"]
 readme = "readme.md"
 license = "license.txt"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `hazard_map-0.2.0/readme.md` & `hazard_map-0.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `hazard_map-0.2.0/PKG-INFO` & `hazard_map-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hazard-map
-Version: 0.2.0
+Version: 0.2.1
 Summary: Build and analyze a network model of hazards, causes, and controls
 License: license.txt
 Author: Thom Cameron
 Author-email: thomcm@proton.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

