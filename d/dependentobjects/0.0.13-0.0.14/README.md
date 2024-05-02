# Comparing `tmp/dependentobjects-0.0.13.tar.gz` & `tmp/dependentobjects-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dependentobjects-0.0.13.tar", last modified: Thu May  2 06:19:29 2024, max compression
+gzip compressed data, was "dependentobjects-0.0.14.tar", last modified: Thu May  2 06:21:26 2024, max compression
```

## Comparing `dependentobjects-0.0.13.tar` & `dependentobjects-0.0.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 06:19:28.989844 dependentobjects-0.0.13/
--rw-rw-rw-   0        0        0     1091 2024-05-01 00:20:48.000000 dependentobjects-0.0.13/LICENSE.txt
--rw-rw-rw-   0        0        0     1720 2024-05-02 06:19:28.989844 dependentobjects-0.0.13/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2024-05-02 06:19:00.000000 dependentobjects-0.0.13/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 06:19:28.989844 dependentobjects-0.0.13/dependentobjects/
--rw-rw-rw-   0        0        0     7622 2024-05-02 06:08:59.000000 dependentobjects-0.0.13/dependentobjects/DependentObjects.py
--rw-rw-rw-   0        0        0        0 2024-05-01 00:26:47.000000 dependentobjects-0.0.13/dependentobjects/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:19:28.989844 dependentobjects-0.0.13/dependentobjects.egg-info/
--rw-rw-rw-   0        0        0     1720 2024-05-02 06:19:28.000000 dependentobjects-0.0.13/dependentobjects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2024-05-02 06:19:28.000000 dependentobjects-0.0.13/dependentobjects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 06:19:28.000000 dependentobjects-0.0.13/dependentobjects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-02 06:19:28.000000 dependentobjects-0.0.13/dependentobjects.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-02 06:19:28.000000 dependentobjects-0.0.13/dependentobjects.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 06:19:28.989844 dependentobjects-0.0.13/setup.cfg
--rw-rw-rw-   0        0        0     1220 2024-05-02 06:19:18.000000 dependentobjects-0.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:21:26.853169 dependentobjects-0.0.14/
+-rw-rw-rw-   0        0        0     1091 2024-05-01 00:20:48.000000 dependentobjects-0.0.14/LICENSE.txt
+-rw-rw-rw-   0        0        0     1720 2024-05-02 06:21:26.853169 dependentobjects-0.0.14/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2024-05-02 06:20:54.000000 dependentobjects-0.0.14/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 06:21:26.833562 dependentobjects-0.0.14/dependentobjects/
+-rw-rw-rw-   0        0        0     7622 2024-05-02 06:08:59.000000 dependentobjects-0.0.14/dependentobjects/DependentObjects.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 00:26:47.000000 dependentobjects-0.0.14/dependentobjects/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:21:26.853169 dependentobjects-0.0.14/dependentobjects.egg-info/
+-rw-rw-rw-   0        0        0     1720 2024-05-02 06:21:26.000000 dependentobjects-0.0.14/dependentobjects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2024-05-02 06:21:26.000000 dependentobjects-0.0.14/dependentobjects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 06:21:26.000000 dependentobjects-0.0.14/dependentobjects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-02 06:21:26.000000 dependentobjects-0.0.14/dependentobjects.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-02 06:21:26.000000 dependentobjects-0.0.14/dependentobjects.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 06:21:26.853169 dependentobjects-0.0.14/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2024-05-02 06:21:16.000000 dependentobjects-0.0.14/setup.py
```

### Comparing `dependentobjects-0.0.13/LICENSE.txt` & `dependentobjects-0.0.14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dependentobjects-0.0.13/PKG-INFO` & `dependentobjects-0.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dependentobjects
-Version: 0.0.13
+Version: 0.0.14
 Summary: creates an excel with all the dependent objects in a powerbi datasets or analysis services
 Author: vamshi krishna
 Author-email: vamshikrishna.r@sonata-software.com
 Keywords: nested measures,dependent objects,dependent
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dependentobjects-0.0.13/README.md` & `dependentobjects-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `dependentobjects-0.0.13/dependentobjects/DependentObjects.py` & `dependentobjects-0.0.14/dependentobjects/DependentObjects.py`

 * *Files identical despite different names*

### Comparing `dependentobjects-0.0.13/dependentobjects.egg-info/PKG-INFO` & `dependentobjects-0.0.14/dependentobjects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dependentobjects
-Version: 0.0.13
+Version: 0.0.14
 Summary: creates an excel with all the dependent objects in a powerbi datasets or analysis services
 Author: vamshi krishna
 Author-email: vamshikrishna.r@sonata-software.com
 Keywords: nested measures,dependent objects,dependent
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dependentobjects-0.0.13/setup.py` & `dependentobjects-0.0.14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.13'
+VERSION = '0.0.14'
 DESCRIPTION = 'creates an excel with all the dependent objects in a powerbi datasets or analysis services'
 LONG_DESCRIPTION = 'creates an excel with all the dependent objects in a powerbi datasets or analysis services'
 
 # Setting up
 setup(
     name="dependentobjects",
     version=VERSION,
```

