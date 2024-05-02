# Comparing `tmp/pppfy-1.0.1.tar.gz` & `tmp/pppfy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pppfy-1.0.1.tar", last modified: Mon Apr 29 09:47:08 2024, max compression
+gzip compressed data, was "pppfy-1.1.0.tar", last modified: Thu May  2 09:45:03 2024, max compression
```

## Comparing `pppfy-1.0.1.tar` & `pppfy-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-04-29 09:47:08.096092 pppfy-1.0.1/
--rw-r--r--   0 gkoduri    (502) staff       (20)      716 2024-04-29 08:54:50.000000 pppfy-1.0.1/LICENSE
--rw-r--r--   0 gkoduri    (502) staff       (20)       66 2024-04-29 08:55:56.000000 pppfy-1.0.1/MANIFEST.in
--rw-r--r--   0 gkoduri    (502) staff       (20)     2925 2024-04-29 09:47:08.095762 pppfy-1.0.1/PKG-INFO
--rw-r--r--   0 gkoduri    (502) staff       (20)     1867 2024-04-29 09:31:47.000000 pppfy-1.0.1/README.md
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-04-29 09:47:08.093464 pppfy-1.0.1/ppp/
--rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-04-29 09:28:12.000000 pppfy-1.0.1/ppp/__init__.py
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-04-29 09:47:08.093562 pppfy-1.0.1/ppp/data/
--rw-r--r--   0 gkoduri    (502) staff       (20)   221712 2024-04-25 07:31:35.000000 pppfy-1.0.1/ppp/data/ppp-gdp.csv
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-04-29 09:47:08.094701 pppfy-1.0.1/pppfy/
--rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-04-25 07:31:26.000000 pppfy-1.0.1/pppfy/__init__.py
--rw-r--r--   0 gkoduri    (502) staff       (20)     4584 2024-04-29 08:26:27.000000 pppfy-1.0.1/pppfy/converter.py
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-04-29 09:47:08.095560 pppfy-1.0.1/pppfy.egg-info/
--rw-r--r--   0 gkoduri    (502) staff       (20)     2925 2024-04-29 09:47:08.000000 pppfy-1.0.1/pppfy.egg-info/PKG-INFO
--rw-r--r--   0 gkoduri    (502) staff       (20)      228 2024-04-29 09:47:08.000000 pppfy-1.0.1/pppfy.egg-info/SOURCES.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)        1 2024-04-29 09:47:08.000000 pppfy-1.0.1/pppfy.egg-info/dependency_links.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)       10 2024-04-29 09:47:08.000000 pppfy-1.0.1/pppfy.egg-info/top_level.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)       38 2024-04-29 09:47:08.096135 pppfy-1.0.1/setup.cfg
--rw-r--r--   0 gkoduri    (502) staff       (20)     1578 2024-04-29 09:45:53.000000 pppfy-1.0.1/setup.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-02 09:45:03.135744 pppfy-1.1.0/
+-rw-r--r--   0 gkoduri    (502) staff       (20)      716 2024-04-29 08:54:50.000000 pppfy-1.1.0/LICENSE
+-rw-r--r--   0 gkoduri    (502) staff       (20)       66 2024-04-29 08:55:56.000000 pppfy-1.1.0/MANIFEST.in
+-rw-r--r--   0 gkoduri    (502) staff       (20)     2925 2024-05-02 09:45:03.135539 pppfy-1.1.0/PKG-INFO
+-rw-r--r--   0 gkoduri    (502) staff       (20)     1867 2024-04-29 09:31:47.000000 pppfy-1.1.0/README.md
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-02 09:45:03.133254 pppfy-1.1.0/ppp/
+-rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-04-29 09:28:12.000000 pppfy-1.1.0/ppp/__init__.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-02 09:45:03.133350 pppfy-1.1.0/ppp/data/
+-rw-r--r--   0 gkoduri    (502) staff       (20)   221712 2024-04-25 07:31:35.000000 pppfy-1.1.0/ppp/data/ppp-gdp.csv
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-02 09:45:03.134411 pppfy-1.1.0/pppfy/
+-rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-04-25 07:31:26.000000 pppfy-1.1.0/pppfy/__init__.py
+-rw-r--r--   0 gkoduri    (502) staff       (20)     4713 2024-05-02 03:50:41.000000 pppfy-1.1.0/pppfy/converter.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-02 09:45:03.135329 pppfy-1.1.0/pppfy.egg-info/
+-rw-r--r--   0 gkoduri    (502) staff       (20)     2925 2024-05-02 09:45:03.000000 pppfy-1.1.0/pppfy.egg-info/PKG-INFO
+-rw-r--r--   0 gkoduri    (502) staff       (20)      228 2024-05-02 09:45:03.000000 pppfy-1.1.0/pppfy.egg-info/SOURCES.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)        1 2024-05-02 09:45:03.000000 pppfy-1.1.0/pppfy.egg-info/dependency_links.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)       10 2024-05-02 09:45:03.000000 pppfy-1.1.0/pppfy.egg-info/top_level.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)       38 2024-05-02 09:45:03.135784 pppfy-1.1.0/setup.cfg
+-rw-r--r--   0 gkoduri    (502) staff       (20)     1578 2024-05-02 09:44:56.000000 pppfy-1.1.0/setup.py
```

### Comparing `pppfy-1.0.1/LICENSE` & `pppfy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pppfy-1.0.1/PKG-INFO` & `pppfy-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pppfy
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python package to get prices based on Purchasing Power Parity (PPP)
 Home-page: https://github.com/gopalkoduri/pppfy
 Author: Gopala Krishna Koduri
 Author-email: gopal@riyazapp.com
 Project-URL: Source Code, https://github.com/gopalkoduri/pppfy
 Project-URL: Issue Tracker, https://github.com/gopalkoduri/pppfy/issues
 Project-URL: Connect w/ Author, https://linkedin.com/in/gopalkoduri
```

### Comparing `pppfy-1.0.1/README.md` & `pppfy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pppfy-1.0.1/ppp/data/ppp-gdp.csv` & `pppfy-1.1.0/ppp/data/ppp-gdp.csv`

 * *Files identical despite different names*

### Comparing `pppfy-1.0.1/pppfy/converter.py` & `pppfy-1.1.0/pppfy/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import csv
+from pkg_resources import resource_filename
 
 
 class Converter:
-    def __init__(self, ppp_data_file="ppp/data/ppp-gdp.csv"):
+    def __init__(self, ppp_data_file=None):
         # map of country_iso2_code: {year: ppp} data
         self._ppp_data = {}
+        if not ppp_data_file:
+            ppp_data_file = resource_filename("ppp", "data/ppp-gdp.csv")
         self._load_ppp_data(ppp_data_file)
 
     def _load_ppp_data(self, ppp_data_file):
         with open(ppp_data_file, mode="r", encoding="utf-8") as file:
             csv_reader = csv.DictReader(file)
             for row in csv_reader:
                 country_iso2_code = row["Country ID"]
```

### Comparing `pppfy-1.0.1/pppfy.egg-info/PKG-INFO` & `pppfy-1.1.0/pppfy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pppfy
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python package to get prices based on Purchasing Power Parity (PPP)
 Home-page: https://github.com/gopalkoduri/pppfy
 Author: Gopala Krishna Koduri
 Author-email: gopal@riyazapp.com
 Project-URL: Source Code, https://github.com/gopalkoduri/pppfy
 Project-URL: Issue Tracker, https://github.com/gopalkoduri/pppfy/issues
 Project-URL: Connect w/ Author, https://linkedin.com/in/gopalkoduri
```

### Comparing `pppfy-1.0.1/setup.py` & `pppfy-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pppfy",
-    version="1.0.1",
+    version="1.1.0",
     description="A Python package to get prices based on Purchasing Power Parity (PPP)",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",  # Ensure you include a README.md in your package
     author="Gopala Krishna Koduri",
     author_email="gopal@riyazapp.com",
     url="https://github.com/gopalkoduri/pppfy",  # Company URL
     project_urls={  # Additional URLs
```

