# Comparing `tmp/DreamCreator-0.0.2.tar.gz` & `tmp/DreamCreator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DreamCreator-0.0.2.tar", last modified: Wed Apr  3 23:25:05 2024, max compression
+gzip compressed data, was "DreamCreator-0.0.3.tar", last modified: Wed Apr  3 23:41:02 2024, max compression
```

## Comparing `DreamCreator-0.0.2.tar` & `DreamCreator-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 23:25:05.365542 DreamCreator-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-03-18 02:28:05.000000 DreamCreator-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1957 2024-04-03 23:25:05.364532 DreamCreator-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 23:25:05.151097 DreamCreator-0.0.2/app/
-drwxrwxrwx   0        0        0        0 2024-04-03 23:25:05.171086 DreamCreator-0.0.2/app/DreamCreator.egg-info/
--rw-rw-rw-   0        0        0     1957 2024-04-03 23:25:04.000000 DreamCreator-0.0.2/app/DreamCreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1511 2024-04-03 23:25:04.000000 DreamCreator-0.0.2/app/DreamCreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 23:25:04.000000 DreamCreator-0.0.2/app/DreamCreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2024-04-03 23:25:04.000000 DreamCreator-0.0.2/app/DreamCreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-03 23:25:04.000000 DreamCreator-0.0.2/app/DreamCreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 23:25:05.211083 DreamCreator-0.0.2/app/dreamcreator/
-drwxrwxrwx   0        0        0        0 2024-04-03 23:25:05.214080 DreamCreator-0.0.2/app/dreamcreator/File_edits/
--rw-rw-rw-   0        0        0        0 2024-03-28 21:58:12.000000 DreamCreator-0.0.2/app/dreamcreator/File_edits/__init__.py
--rw-rw-rw-   0        0        0       31 2024-01-24 23:45:27.000000 DreamCreator-0.0.2/app/dreamcreator/__init__.py
--rw-rw-rw-   0        0        0    62177 2024-03-28 22:14:35.000000 DreamCreator-0.0.2/app/dreamcreator/sequencecreator.py
--rw-rw-rw-   0        0        0       68 2024-01-23 01:45:18.000000 DreamCreator-0.0.2/app/dreamcreator/sequencecreatorvariables.py
-drwxrwxrwx   0        0        0        0 2024-04-03 23:25:05.310666 DreamCreator-0.0.2/app/dreamcreator/sequences/
--rw-rw-rw-   0        0        0      112 2024-01-23 01:45:18.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 23:25:05.352530 DreamCreator-0.0.2/app/dreamcreator/sequences/core/
--rw-rw-rw-   0        0        0      106 2024-01-23 01:45:18.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/core/__init__.py
--rw-rw-rw-   0        0        0    10207 2024-03-28 22:17:23.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/core/laser_sweep.py
--rw-rw-rw-   0        0        0    15635 2024-01-23 01:45:19.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/core/results.py
--rw-rw-rw-   0        0        0     3086 2024-03-28 22:17:29.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/core/sequence.py
--rw-rw-rw-   0        0        0     7492 2024-03-28 22:17:32.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/core/smu_sweep.py
--rw-rw-rw-   0        0        0     2409 2024-03-28 22:15:55.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/current_sweep.py
--rw-rw-rw-   0        0        0     2044 2024-03-28 22:15:49.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/current_sweep_ida.py
--rw-rw-rw-   0        0        0     2476 2024-03-28 22:16:02.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/set_current_wavelength_sweep.py
--rw-rw-rw-   0        0        0     2884 2024-03-28 22:15:58.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/set_current_wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0     2793 2024-03-28 22:16:08.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/set_voltage_wavelength_sweep.py
--rw-rw-rw-   0        0        0     2974 2024-03-28 22:16:05.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/set_voltage_wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0     2549 2024-03-28 22:16:14.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/set_wavelength_current_sweep.py
--rw-rw-rw-   0        0        0     2508 2024-03-28 22:16:11.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/set_wavelength_current_sweep_ida.py
--rw-rw-rw-   0        0        0     2918 2024-03-28 22:16:19.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/set_wavelength_voltage_sweep.py
--rw-rw-rw-   0        0        0     2603 2024-03-28 22:16:17.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/set_wavelength_voltage_sweep_ida.py
-drwxrwxrwx   0        0        0        0 2024-04-03 23:25:05.354529 DreamCreator-0.0.2/app/dreamcreator/sequences/template/
--rw-rw-rw-   0        0        0      971 2024-01-23 01:45:19.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/template/__init__.py
--rw-rw-rw-   0        0        0     2273 2024-03-28 22:16:25.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/voltage_sweep.py
--rw-rw-rw-   0        0        0     1952 2024-03-28 22:16:22.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/voltage_sweep_ida.py
--rw-rw-rw-   0        0        0     2260 2024-03-28 22:16:36.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/wavelength_sweep.py
--rw-rw-rw-   0        0        0     2033 2024-03-28 22:16:28.000000 DreamCreator-0.0.2/app/dreamcreator/sequences/wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0     3071 2024-01-23 01:45:19.000000 DreamCreator-0.0.2/app/dreamcreator/sequencetracker.py
--rw-rw-rw-   0        0        0     4334 2024-01-23 01:45:51.000000 DreamCreator-0.0.2/app/dreamcreator/yamlcheck.py
--rw-rw-rw-   0        0        0       42 2024-04-03 23:25:05.365542 DreamCreator-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1225 2024-04-03 23:24:56.000000 DreamCreator-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.274162 DreamCreator-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-03-18 02:28:05.000000 DreamCreator-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1957 2024-04-03 23:41:02.273161 DreamCreator-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.168157 DreamCreator-0.0.3/app/
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.184141 DreamCreator-0.0.3/app/DreamCreator.egg-info/
+-rw-rw-rw-   0        0        0     1957 2024-04-03 23:41:01.000000 DreamCreator-0.0.3/app/DreamCreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1511 2024-04-03 23:41:01.000000 DreamCreator-0.0.3/app/DreamCreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 23:41:01.000000 DreamCreator-0.0.3/app/DreamCreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2024-04-03 23:41:01.000000 DreamCreator-0.0.3/app/DreamCreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-03 23:41:01.000000 DreamCreator-0.0.3/app/DreamCreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.196788 DreamCreator-0.0.3/app/dreamcreator/
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.199784 DreamCreator-0.0.3/app/dreamcreator/File_edits/
+-rw-rw-rw-   0        0        0        0 2024-03-28 21:58:12.000000 DreamCreator-0.0.3/app/dreamcreator/File_edits/__init__.py
+-rw-rw-rw-   0        0        0       31 2024-01-24 23:45:27.000000 DreamCreator-0.0.3/app/dreamcreator/__init__.py
+-rw-rw-rw-   0        0        0    62177 2024-03-28 22:14:35.000000 DreamCreator-0.0.3/app/dreamcreator/sequencecreator.py
+-rw-rw-rw-   0        0        0       68 2024-01-23 01:45:18.000000 DreamCreator-0.0.3/app/dreamcreator/sequencecreatorvariables.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.235163 DreamCreator-0.0.3/app/dreamcreator/sequences/
+-rw-rw-rw-   0        0        0      112 2024-01-23 01:45:18.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.246166 DreamCreator-0.0.3/app/dreamcreator/sequences/core/
+-rw-rw-rw-   0        0        0      106 2024-01-23 01:45:18.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/core/__init__.py
+-rw-rw-rw-   0        0        0    10207 2024-03-28 22:17:23.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/core/laser_sweep.py
+-rw-rw-rw-   0        0        0    15635 2024-01-23 01:45:19.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/core/results.py
+-rw-rw-rw-   0        0        0     3086 2024-03-28 22:17:29.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/core/sequence.py
+-rw-rw-rw-   0        0        0     7492 2024-03-28 22:17:32.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/core/smu_sweep.py
+-rw-rw-rw-   0        0        0     2409 2024-03-28 22:15:55.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/current_sweep.py
+-rw-rw-rw-   0        0        0     2044 2024-03-28 22:15:49.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/current_sweep_ida.py
+-rw-rw-rw-   0        0        0     2476 2024-03-28 22:16:02.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_current_wavelength_sweep.py
+-rw-rw-rw-   0        0        0     2884 2024-03-28 22:15:58.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_current_wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     2793 2024-03-28 22:16:08.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_voltage_wavelength_sweep.py
+-rw-rw-rw-   0        0        0     2974 2024-03-28 22:16:05.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_voltage_wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     2549 2024-03-28 22:16:14.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_current_sweep.py
+-rw-rw-rw-   0        0        0     2508 2024-03-28 22:16:11.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_current_sweep_ida.py
+-rw-rw-rw-   0        0        0     2918 2024-03-28 22:16:19.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_voltage_sweep.py
+-rw-rw-rw-   0        0        0     2603 2024-03-28 22:16:17.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_voltage_sweep_ida.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:41:02.249163 DreamCreator-0.0.3/app/dreamcreator/sequences/template/
+-rw-rw-rw-   0        0        0      971 2024-01-23 01:45:19.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/template/__init__.py
+-rw-rw-rw-   0        0        0     2273 2024-03-28 22:16:25.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/voltage_sweep.py
+-rw-rw-rw-   0        0        0     1952 2024-03-28 22:16:22.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/voltage_sweep_ida.py
+-rw-rw-rw-   0        0        0     2260 2024-03-28 22:16:36.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/wavelength_sweep.py
+-rw-rw-rw-   0        0        0     2033 2024-03-28 22:16:28.000000 DreamCreator-0.0.3/app/dreamcreator/sequences/wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     3071 2024-01-23 01:45:19.000000 DreamCreator-0.0.3/app/dreamcreator/sequencetracker.py
+-rw-rw-rw-   0        0        0     4334 2024-01-23 01:45:51.000000 DreamCreator-0.0.3/app/dreamcreator/yamlcheck.py
+-rw-rw-rw-   0        0        0       42 2024-04-03 23:41:02.274162 DreamCreator-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2024-04-03 23:40:55.000000 DreamCreator-0.0.3/setup.py
```

### Comparing `DreamCreator-0.0.2/LICENSE` & `DreamCreator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/PKG-INFO` & `DreamCreator-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DreamCreator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for creating YAML files for use in Dream Photonics and edx course
 Home-page: https://github.com/dreamphotonics/DreamCreator.git
 Author: Jonathan Barnes
 Author-email: jonathanyorkbarnes@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DreamCreator-0.0.2/app/DreamCreator.egg-info/PKG-INFO` & `DreamCreator-0.0.3/app/DreamCreator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DreamCreator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for creating YAML files for use in Dream Photonics and edx course
 Home-page: https://github.com/dreamphotonics/DreamCreator.git
 Author: Jonathan Barnes
 Author-email: jonathanyorkbarnes@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DreamCreator-0.0.2/app/DreamCreator.egg-info/SOURCES.txt` & `DreamCreator-0.0.3/app/DreamCreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequencecreator.py` & `DreamCreator-0.0.3/app/dreamcreator/sequencecreator.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/core/laser_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/core/laser_sweep.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/core/results.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/core/results.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/core/sequence.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/core/sequence.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/core/smu_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/core/smu_sweep.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/current_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/current_sweep.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/current_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/current_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/set_current_wavelength_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_current_wavelength_sweep.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/set_current_wavelength_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_current_wavelength_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/set_voltage_wavelength_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_voltage_wavelength_sweep.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/set_voltage_wavelength_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_voltage_wavelength_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/set_wavelength_current_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_current_sweep.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/set_wavelength_current_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_current_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/set_wavelength_voltage_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_voltage_sweep.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/set_wavelength_voltage_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/set_wavelength_voltage_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/template/__init__.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/template/__init__.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/voltage_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/voltage_sweep.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/voltage_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/voltage_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/wavelength_sweep.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/wavelength_sweep.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequences/wavelength_sweep_ida.py` & `DreamCreator-0.0.3/app/dreamcreator/sequences/wavelength_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/sequencetracker.py` & `DreamCreator-0.0.3/app/dreamcreator/sequencetracker.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/app/dreamcreator/yamlcheck.py` & `DreamCreator-0.0.3/app/dreamcreator/yamlcheck.py`

 * *Files identical despite different names*

### Comparing `DreamCreator-0.0.2/setup.py` & `DreamCreator-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = "DreamCreator",
-    version = "0.0.2",
+    version = "0.0.3",
     description = "A tool for creating YAML files for use in Dream Photonics and edx course",
     package_dir = {"": "app"},
     packages = find_packages(where="app"),
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/dreamphotonics/DreamCreator.git",
     author = "Jonathan Barnes",
@@ -21,16 +21,16 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[    
         'numpy==1.26.3',
         'pandas==2.2.0',
         'pillow==10.2.0',
         'pkginfo==1.10.0',
-        'PyQt5==5.15.10',
-        'PyQt5-Qt5==5.15.2',
+        'PyQt5>=5.15.10',
+        'PyQt5-Qt5>=5.15.2',
         'PyQt5-sip==12.13.0',
         'pywin32-ctypes==0.2.2',
         'PyYAML==6.0.1',
         'scipy==1.12.0',
         'twine==5.0.0',
         'watchdog==3.0.0',
         'matplotlib==3.8.2'
```

