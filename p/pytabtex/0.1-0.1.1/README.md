# Comparing `tmp/pytabtex-0.1.tar.gz` & `tmp/pytabtex-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytabtex-0.1.tar", last modified: Thu May  2 08:23:04 2024, max compression
+gzip compressed data, was "pytabtex-0.1.1.tar", last modified: Thu May  2 08:25:55 2024, max compression
```

## Comparing `pytabtex-0.1.tar` & `pytabtex-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 08:23:04.620204 pytabtex-0.1/
--rw-rw-rw-   0        0        0     1095 2024-04-29 17:50:55.000000 pytabtex-0.1/LICENSE
--rw-rw-rw-   0        0        0     5137 2024-05-02 08:23:04.618711 pytabtex-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      651 2024-05-02 08:22:20.000000 pytabtex-0.1/pyproject.toml
--rw-rw-rw-   0        0        0     4570 2024-05-01 16:08:00.000000 pytabtex-0.1/readme.md
--rw-rw-rw-   0        0        0       42 2024-05-02 08:23:04.620204 pytabtex-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-02 08:23:04.572977 pytabtex-0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 08:23:04.582870 pytabtex-0.1/src/pytabtex/
--rw-rw-rw-   0        0        0     6197 2024-05-01 16:11:45.000000 pytabtex-0.1/src/pytabtex/Table.py
--rw-rw-rw-   0        0        0        0 2024-05-01 01:00:35.000000 pytabtex-0.1/src/pytabtex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 08:23:04.616701 pytabtex-0.1/src/pytabtex.egg-info/
--rw-rw-rw-   0        0        0     5137 2024-05-02 08:23:04.000000 pytabtex-0.1/src/pytabtex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-02 08:23:04.000000 pytabtex-0.1/src/pytabtex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 08:23:04.000000 pytabtex-0.1/src/pytabtex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-02 08:23:04.000000 pytabtex-0.1/src/pytabtex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 08:23:04.000000 pytabtex-0.1/src/pytabtex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 08:23:04.614690 pytabtex-0.1/tests/
--rw-rw-rw-   0        0        0      899 2024-05-01 14:37:28.000000 pytabtex-0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-02 08:25:55.856970 pytabtex-0.1.1/
+-rw-rw-rw-   0        0        0     1095 2024-04-29 17:50:55.000000 pytabtex-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5192 2024-05-02 08:25:55.854917 pytabtex-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-05-02 08:25:48.000000 pytabtex-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0     4623 2024-05-02 08:25:32.000000 pytabtex-0.1.1/readme.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 08:25:55.856970 pytabtex-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 08:25:55.800111 pytabtex-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 08:25:55.816887 pytabtex-0.1.1/src/pytabtex/
+-rw-rw-rw-   0        0        0     6197 2024-05-01 16:11:45.000000 pytabtex-0.1.1/src/pytabtex/Table.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 01:00:35.000000 pytabtex-0.1.1/src/pytabtex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 08:25:55.852924 pytabtex-0.1.1/src/pytabtex.egg-info/
+-rw-rw-rw-   0        0        0     5192 2024-05-02 08:25:55.000000 pytabtex-0.1.1/src/pytabtex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-02 08:25:55.000000 pytabtex-0.1.1/src/pytabtex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 08:25:55.000000 pytabtex-0.1.1/src/pytabtex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-02 08:25:55.000000 pytabtex-0.1.1/src/pytabtex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 08:25:55.000000 pytabtex-0.1.1/src/pytabtex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 08:25:55.849589 pytabtex-0.1.1/tests/
+-rw-rw-rw-   0        0        0      899 2024-05-01 14:37:28.000000 pytabtex-0.1.1/tests/test.py
```

### Comparing `pytabtex-0.1/LICENSE` & `pytabtex-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytabtex-0.1/PKG-INFO` & `pytabtex-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytabtex
-Version: 0.1
+Version: 0.1.1
 Summary: Use simple python to create custom latex tables
 Author-email: Nour Oulad Moussa <nourom.professional@gmail.com>
 Project-URL: Homepage, https://github.com/NourOM02/pytabtex
 Project-URL: Issues, https://github.com/NourOM02/pytabtex/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,15 +65,15 @@
 
 ### Define body of the table
 
 The body of the table can be a dictionary, a pandas Dataframe or a csv file path.
 
 **Example**
 
-![Body](media/body.png)
+![Body](media/https://github.com/NourOM02/pytabtex/blob/main/media/body.png)
 
 **Dictionary**
 
 ```python
 {
     "id 1" : [29, 31, 90],
     "id 2" : [97, 78, 67]
```

### Comparing `pytabtex-0.1/pyproject.toml` & `pytabtex-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytabtex"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="Nour Oulad Moussa", email="nourom.professional@gmail.com" },
 ]
 description = "Use simple python to create custom latex tables"
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pytabtex-0.1/readme.md` & `pytabtex-0.1.1/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 ### Define body of the table
 
 The body of the table can be a dictionary, a pandas Dataframe or a csv file path.
 
 **Example**
 
-![Body](media/body.png)
+![Body](media/https://github.com/NourOM02/pytabtex/blob/main/media/body.png)
 
 **Dictionary**
 
 ```python
 {
     "id 1" : [29, 31, 90],
     "id 2" : [97, 78, 67]
```

### Comparing `pytabtex-0.1/src/pytabtex/Table.py` & `pytabtex-0.1.1/src/pytabtex/Table.py`

 * *Files identical despite different names*

### Comparing `pytabtex-0.1/src/pytabtex.egg-info/PKG-INFO` & `pytabtex-0.1.1/src/pytabtex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytabtex
-Version: 0.1
+Version: 0.1.1
 Summary: Use simple python to create custom latex tables
 Author-email: Nour Oulad Moussa <nourom.professional@gmail.com>
 Project-URL: Homepage, https://github.com/NourOM02/pytabtex
 Project-URL: Issues, https://github.com/NourOM02/pytabtex/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,15 +65,15 @@
 
 ### Define body of the table
 
 The body of the table can be a dictionary, a pandas Dataframe or a csv file path.
 
 **Example**
 
-![Body](media/body.png)
+![Body](media/https://github.com/NourOM02/pytabtex/blob/main/media/body.png)
 
 **Dictionary**
 
 ```python
 {
     "id 1" : [29, 31, 90],
     "id 2" : [97, 78, 67]
```

### Comparing `pytabtex-0.1/tests/test.py` & `pytabtex-0.1.1/tests/test.py`

 * *Files identical despite different names*

