# Comparing `tmp/lca_algebraic_dev-1.1.1750653.dev0.tar.gz` & `tmp/lca_algebraic_dev-1.1.1753145.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lca_algebraic_dev-1.1.1750653.dev0.tar", last modified: Tue Apr 30 15:33:02 2024, max compression
+gzip compressed data, was "lca_algebraic_dev-1.1.1753145.dev0.tar", last modified: Thu May  2 09:05:42 2024, max compression
```

## Comparing `lca_algebraic_dev-1.1.1750653.dev0.tar` & `lca_algebraic_dev-1.1.1753145.dev0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      199 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/.gitignore
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1331 2020-03-30 15:19:57.000000 lca_algebraic_dev-1.1.1750653.dev0/LICENSE
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      693 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/Makefile
--rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     2916 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/PKG-INFO
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2118 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/README.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5451 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/RELEASE_NOTES.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        3 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/VERSION
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-30 15:33:02.527867 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1147 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    26296 2024-04-30 11:37:51.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/activity.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2224 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/axis_dict.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4736 2024-04-29 09:36:57.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/base_utils.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3015 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/cache.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     6009 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/database.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3600 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/interpolation.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2043 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/io.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    28054 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/lca.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      547 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/log.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1760 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/methods.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    41317 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/params.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      103 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/settings.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    39547 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/stats.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     7874 2024-04-29 10:45:25.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/units.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/
--rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     2916 2024-04-30 15:33:02.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/PKG-INFO
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      757 2024-04-30 15:33:02.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        1 2024-04-30 15:33:02.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      122 2024-04-30 15:33:02.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/requires.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       14 2024-04-30 15:33:02.000000 lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/top_level.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      167 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/requirements.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      338 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/setup.cfg
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2062 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/setup.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/test/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2021-06-23 08:53:38.000000 lca_algebraic_dev-1.1.1750653.dev0/test/__init__.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-04-30 15:33:02.531867 lca_algebraic_dev-1.1.1750653.dev0/test/fixtures/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1016 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/test/fixtures/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      777 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1750653.dev0/test/test_axis_dict.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3877 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1750653.dev0/test/test_units.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      199 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/.gitignore
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1331 2020-03-30 15:19:57.000000 lca_algebraic_dev-1.1.1753145.dev0/LICENSE
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      693 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/Makefile
+-rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     2916 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/PKG-INFO
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2118 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/README.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5509 2024-05-02 09:02:10.000000 lca_algebraic_dev-1.1.1753145.dev0/RELEASE_NOTES.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        3 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/VERSION
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1147 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    26296 2024-04-30 11:37:51.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/activity.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2224 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/axis_dict.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4736 2024-04-29 09:36:57.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/base_utils.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3015 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/cache.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     6009 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/database.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3600 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/interpolation.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2043 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/io.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    28054 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/lca.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      547 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/log.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1760 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/methods.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    41317 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/params.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      103 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/settings.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    39547 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/stats.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     8202 2024-05-02 08:57:26.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/units.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/
+-rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     2916 2024-05-02 09:05:42.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      757 2024-05-02 09:05:42.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        1 2024-05-02 09:05:42.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      122 2024-05-02 09:05:42.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/requires.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       14 2024-05-02 09:05:42.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/top_level.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      167 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/requirements.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      338 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/setup.cfg
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2132 2024-05-02 09:05:24.000000 lca_algebraic_dev-1.1.1753145.dev0/setup.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/test/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2021-06-23 08:53:38.000000 lca_algebraic_dev-1.1.1753145.dev0/test/__init__.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/test/fixtures/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1016 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/test/fixtures/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      777 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/test/test_axis_dict.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3877 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/test/test_units.py
```

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/LICENSE` & `lca_algebraic_dev-1.1.1753145.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/Makefile` & `lca_algebraic_dev-1.1.1753145.dev0/Makefile`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/PKG-INFO` & `lca_algebraic_dev-1.1.1753145.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lca_algebraic_dev
-Version: 1.1.1750653.dev0
+Version: 1.1.1753145.dev0
 Summary: This library provides a layer above brightway2 for defining parametric models and running super fast LCA for monte carlo analysis.
 Home-page: https://github.com/oie-mines-paristech/lca_algebraic/
 Author: OIE - Mines ParisTech
 Author-email: raphael.jolivet@mines-paristech.fr
 License: BSD
 Keywords: LCA brightway2 monte-carlo parametric
 Description-Content-Type: text/markdown
@@ -14,18 +14,18 @@
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: seaborn
 Requires-Dist: sympy
 Requires-Dist: matplotlib
 Requires-Dist: deprecation
 Requires-Dist: brightway2
-Requires-Dist: pypardiso
 Requires-Dist: SALib
 Requires-Dist: pint
 Requires-Dist: typing-extensions
+Requires-Dist: pypardiso
 
 # Introduction
 
 This library is a layer above [**brightway2**](https://brightway.dev/) designed for the definition of **parametric inventories** 
 with fast computation of LCA impacts, suitable for **monte-carlo** / global sensitivity analysis 
 
 It integrates the magic of [Sympy](https://www.sympy.org/en/index.html) in order to write parametric formulas as regular Python expressions.
```

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/README.md` & `lca_algebraic_dev-1.1.1753145.dev0/README.md`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/RELEASE_NOTES.md` & `lca_algebraic_dev-1.1.1753145.dev0/RELEASE_NOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 1.2-UPCOMMING
+
+* Removed pypardisio from iOS/ARM build
+
 # 1.1
 
 * Fixed bug in ActivityExtended#getExchanges introduced by merge #14
 * Added linear interpolation between activities with function `interpolate_activities`
 * Rename multiLCaAlgebraic => compute_impacts
 * Added breakdown of impacts by arbitrary attribute with the parameter `axis` of `compute_impacts`
 * Added `functional_unit` in compute_impacts : You are not obliged to define a custom activity anymore
```

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/__init__.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/__init__.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/activity.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/activity.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/axis_dict.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/axis_dict.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/base_utils.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/base_utils.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/cache.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/cache.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/database.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/database.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/interpolation.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/interpolation.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/io.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/io.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/lca.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/lca.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/log.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/log.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/methods.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/methods.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/params.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/params.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/stats.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/stats.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic/units.py` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,7 +212,24 @@
         raise OffsetUnitCalculusError(self._units, other._units)
 
     return self.__class__(magnitude, units)
 
 
 # Override the _add_sub method
 PlainQuantity._add_sub = _add_sub_modified
+
+
+def __quantity__or__(self: PlainQuantity, unit: Unit):
+    return self.to(unit)
+
+
+PlainQuantity.__or__ = __quantity__or__
+
+
+def __unit__ror__(self: Unit, value):
+    if isinstance(value, PlainQuantity):
+        return value.to(self)
+    else:
+        return self._REGISTRY.Quantity(value, self)
+
+
+Unit.__ror__ = __unit__ror__
```

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/PKG-INFO` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lca_algebraic_dev
-Version: 1.1.1750653.dev0
+Version: 1.1.1753145.dev0
 Summary: This library provides a layer above brightway2 for defining parametric models and running super fast LCA for monte carlo analysis.
 Home-page: https://github.com/oie-mines-paristech/lca_algebraic/
 Author: OIE - Mines ParisTech
 Author-email: raphael.jolivet@mines-paristech.fr
 License: BSD
 Keywords: LCA brightway2 monte-carlo parametric
 Description-Content-Type: text/markdown
@@ -14,18 +14,18 @@
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: seaborn
 Requires-Dist: sympy
 Requires-Dist: matplotlib
 Requires-Dist: deprecation
 Requires-Dist: brightway2
-Requires-Dist: pypardiso
 Requires-Dist: SALib
 Requires-Dist: pint
 Requires-Dist: typing-extensions
+Requires-Dist: pypardiso
 
 # Introduction
 
 This library is a layer above [**brightway2**](https://brightway.dev/) designed for the definition of **parametric inventories** 
 with fast computation of LCA impacts, suitable for **monte-carlo** / global sensitivity analysis 
 
 It integrates the magic of [Sympy](https://www.sympy.org/en/index.html) in order to write parametric formulas as regular Python expressions.
```

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/lca_algebraic_dev.egg-info/SOURCES.txt` & `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/setup.py` & `lca_algebraic_dev-1.1.1753145.dev0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 import os
+import platform
 import subprocess
 from datetime import datetime
 
 from setuptools import setup
 
+REQUIREMENTS = [
+    "tabulate",
+    "ipywidgets",
+    "pandas",
+    "pyarrow",
+    "seaborn",
+    "sympy",
+    "matplotlib",
+    "deprecation",
+    "brightway2",
+    "SALib",
+    "pint",
+    "typing-extensions",
+]
+
+PYPARDISO = "pypardiso"
+
 
 # Utility function to read the README file.
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read().strip()
@@ -16,14 +34,17 @@
 def run(args):
     return subprocess.run(args, stdout=subprocess.PIPE).stdout.decode("utf-8").splitlines()
 
 
 version = read("VERSION")
 name = "lca_algebraic"
 
+if platform.processor() == "x86_64":
+    REQUIREMENTS.append(PYPARDISO)
+
 # Try to get branch from git
 try:
     branches = run(["git", "branch"])
     curr_branch = next(line for line in branches if "*" in line)
     curr_branch = curr_branch.replace(" ", "").replace("*", "")
 
     if curr_branch != "master":
@@ -53,23 +74,9 @@
     license="BSD",
     keywords="LCA brightway2 monte-carlo parametric",
     url="https://github.com/oie-mines-paristech/lca_algebraic/",
     packages=["lca_algebraic"],
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     classifiers=[],
-    install_requires=[
-        "tabulate",
-        "ipywidgets",
-        "pandas",
-        "pyarrow",
-        "seaborn",
-        "sympy",
-        "matplotlib",
-        "deprecation",
-        "brightway2",
-        "pypardiso",
-        "SALib",
-        "pint",
-        "typing-extensions",
-    ],
+    install_requires=REQUIREMENTS,
 )
```

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/test/fixtures/__init__.py` & `lca_algebraic_dev-1.1.1753145.dev0/test/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/test/test_axis_dict.py` & `lca_algebraic_dev-1.1.1753145.dev0/test/test_axis_dict.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1750653.dev0/test/test_units.py` & `lca_algebraic_dev-1.1.1753145.dev0/test/test_units.py`

 * *Files identical despite different names*

