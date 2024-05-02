# Comparing `tmp/pytabtex-0.1.2.tar.gz` & `tmp/pytabtex-0.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytabtex-0.1.2.tar", last modified: Thu May  2 08:28:50 2024, max compression
+gzip compressed data, was "pytabtex-0.1.2.1.tar", last modified: Thu May  2 08:36:00 2024, max compression
```

## Comparing `pytabtex-0.1.2.tar` & `pytabtex-0.1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 08:28:50.927805 pytabtex-0.1.2/
--rw-rw-rw-   0        0        0     1095 2024-04-29 17:50:55.000000 pytabtex-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5186 2024-05-02 08:28:50.925812 pytabtex-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      653 2024-05-02 08:28:44.000000 pytabtex-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     4617 2024-05-02 08:27:41.000000 pytabtex-0.1.2/readme.md
--rw-rw-rw-   0        0        0       42 2024-05-02 08:28:50.927805 pytabtex-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-02 08:28:50.878703 pytabtex-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 08:28:50.894171 pytabtex-0.1.2/src/pytabtex/
--rw-rw-rw-   0        0        0     6197 2024-05-01 16:11:45.000000 pytabtex-0.1.2/src/pytabtex/Table.py
--rw-rw-rw-   0        0        0        0 2024-05-01 01:00:35.000000 pytabtex-0.1.2/src/pytabtex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 08:28:50.923809 pytabtex-0.1.2/src/pytabtex.egg-info/
--rw-rw-rw-   0        0        0     5186 2024-05-02 08:28:50.000000 pytabtex-0.1.2/src/pytabtex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-02 08:28:50.000000 pytabtex-0.1.2/src/pytabtex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 08:28:50.000000 pytabtex-0.1.2/src/pytabtex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-02 08:28:50.000000 pytabtex-0.1.2/src/pytabtex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 08:28:50.000000 pytabtex-0.1.2/src/pytabtex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 08:28:50.920810 pytabtex-0.1.2/tests/
--rw-rw-rw-   0        0        0      899 2024-05-01 14:37:28.000000 pytabtex-0.1.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-02 08:36:00.399638 pytabtex-0.1.2.1/
+-rw-rw-rw-   0        0        0     1095 2024-04-29 17:50:55.000000 pytabtex-0.1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     5212 2024-05-02 08:36:00.399638 pytabtex-0.1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2024-05-02 08:35:51.000000 pytabtex-0.1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     4641 2024-05-02 08:35:45.000000 pytabtex-0.1.2.1/readme.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 08:36:00.399638 pytabtex-0.1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 08:36:00.311136 pytabtex-0.1.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 08:36:00.335488 pytabtex-0.1.2.1/src/pytabtex/
+-rw-rw-rw-   0        0        0     6197 2024-05-01 16:11:45.000000 pytabtex-0.1.2.1/src/pytabtex/Table.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 01:00:35.000000 pytabtex-0.1.2.1/src/pytabtex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 08:36:00.394169 pytabtex-0.1.2.1/src/pytabtex.egg-info/
+-rw-rw-rw-   0        0        0     5212 2024-05-02 08:36:00.000000 pytabtex-0.1.2.1/src/pytabtex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-02 08:36:00.000000 pytabtex-0.1.2.1/src/pytabtex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 08:36:00.000000 pytabtex-0.1.2.1/src/pytabtex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-02 08:36:00.000000 pytabtex-0.1.2.1/src/pytabtex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 08:36:00.000000 pytabtex-0.1.2.1/src/pytabtex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 08:36:00.391343 pytabtex-0.1.2.1/tests/
+-rw-rw-rw-   0        0        0      899 2024-05-01 14:37:28.000000 pytabtex-0.1.2.1/tests/test.py
```

### Comparing `pytabtex-0.1.2/LICENSE` & `pytabtex-0.1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytabtex-0.1.2/PKG-INFO` & `pytabtex-0.1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytabtex
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: Use simple python to create custom latex tables
 Author-email: Nour Oulad Moussa <nourom.professional@gmail.com>
 Project-URL: Homepage, https://github.com/NourOM02/pytabtex
 Project-URL: Issues, https://github.com/NourOM02/pytabtex/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 
 The columns parameter is a dictionary where each key is the name of the columns, the value is 0 if there are no subcolulmns, or a list of subcolumns names if there are subcolumns.
 
 **Example (simple columns) :**
 
 Desired output :
 
-![Simple columns](media/simple.png)
+![Simple columns](https://i.postimg.cc/rsTqGMK0/simple.png)
 
 Python code :
 ```python
 columns = {"column 1" : 0, "column 2" : 0, "column 3" : 0, "column 4" : 0}
 ```
 
 **Example (multilevel columns) :**
```

### Comparing `pytabtex-0.1.2/pyproject.toml` & `pytabtex-0.1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytabtex"
-version = "0.1.2"
+version = "0.1.2.1"
 authors = [
   { name="Nour Oulad Moussa", email="nourom.professional@gmail.com" },
 ]
 description = "Use simple python to create custom latex tables"
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pytabtex-0.1.2/readme.md` & `pytabtex-0.1.2.1/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 The columns parameter is a dictionary where each key is the name of the columns, the value is 0 if there are no subcolulmns, or a list of subcolumns names if there are subcolumns.
 
 **Example (simple columns) :**
 
 Desired output :
 
-![Simple columns](media/simple.png)
+![Simple columns](https://i.postimg.cc/rsTqGMK0/simple.png)
 
 Python code :
 ```python
 columns = {"column 1" : 0, "column 2" : 0, "column 3" : 0, "column 4" : 0}
 ```
 
 **Example (multilevel columns) :**
```

### Comparing `pytabtex-0.1.2/src/pytabtex/Table.py` & `pytabtex-0.1.2.1/src/pytabtex/Table.py`

 * *Files identical despite different names*

### Comparing `pytabtex-0.1.2/src/pytabtex.egg-info/PKG-INFO` & `pytabtex-0.1.2.1/src/pytabtex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytabtex
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: Use simple python to create custom latex tables
 Author-email: Nour Oulad Moussa <nourom.professional@gmail.com>
 Project-URL: Homepage, https://github.com/NourOM02/pytabtex
 Project-URL: Issues, https://github.com/NourOM02/pytabtex/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 
 The columns parameter is a dictionary where each key is the name of the columns, the value is 0 if there are no subcolulmns, or a list of subcolumns names if there are subcolumns.
 
 **Example (simple columns) :**
 
 Desired output :
 
-![Simple columns](media/simple.png)
+![Simple columns](https://i.postimg.cc/rsTqGMK0/simple.png)
 
 Python code :
 ```python
 columns = {"column 1" : 0, "column 2" : 0, "column 3" : 0, "column 4" : 0}
 ```
 
 **Example (multilevel columns) :**
```

### Comparing `pytabtex-0.1.2/tests/test.py` & `pytabtex-0.1.2.1/tests/test.py`

 * *Files identical despite different names*

