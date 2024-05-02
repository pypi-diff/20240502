# Comparing `tmp/pi_folder_organizer-2.2.0.tar.gz` & `tmp/pi_folder_organizer-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi_folder_organizer-2.2.0.tar", last modified: Tue Apr 16 15:58:00 2024, max compression
+gzip compressed data, was "pi_folder_organizer-2.2.1.tar", last modified: Thu May  2 16:19:50 2024, max compression
```

## Comparing `pi_folder_organizer-2.2.0.tar` & `pi_folder_organizer-2.2.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:58:00.793553 pi_folder_organizer-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-16 15:58:00.793553 pi_folder_organizer-2.2.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:58:00.793553 pi_folder_organizer-2.2.0/pi_folder_organizer/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/pi_folder_organizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/pi_folder_organizer/_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13754 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/pi_folder_organizer/pi_folder_organizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:58:00.793553 pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-16 15:58:00.000000 pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-16 15:58:00.000000 pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:58:00.000000 pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 15:58:00.000000 pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:58:00.793553 pi_folder_organizer-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-16 15:57:57.000000 pi_folder_organizer-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:19:50.647819 pi_folder_organizer-2.2.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-02 16:19:47.000000 pi_folder_organizer-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-02 16:19:50.647819 pi_folder_organizer-2.2.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-05-02 16:19:47.000000 pi_folder_organizer-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:19:50.647819 pi_folder_organizer-2.2.1/pi_folder_organizer/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      206 2024-05-02 16:19:47.000000 pi_folder_organizer-2.2.1/pi_folder_organizer/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      435 2024-05-02 16:19:47.000000 pi_folder_organizer-2.2.1/pi_folder_organizer/_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-02 16:19:47.000000 pi_folder_organizer-2.2.1/pi_folder_organizer/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13754 2024-05-02 16:19:47.000000 pi_folder_organizer-2.2.1/pi_folder_organizer/pi_folder_organizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      342 2024-05-02 16:19:47.000000 pi_folder_organizer-2.2.1/pi_folder_organizer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:19:50.647819 pi_folder_organizer-2.2.1/pi_folder_organizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-02 16:19:50.000000 pi_folder_organizer-2.2.1/pi_folder_organizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-02 16:19:50.000000 pi_folder_organizer-2.2.1/pi_folder_organizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:19:50.000000 pi_folder_organizer-2.2.1/pi_folder_organizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 16:19:50.000000 pi_folder_organizer-2.2.1/pi_folder_organizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:19:50.647819 pi_folder_organizer-2.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1429 2024-05-02 16:19:47.000000 pi_folder_organizer-2.2.1/setup.py
```

### Comparing `pi_folder_organizer-2.2.0/LICENSE` & `pi_folder_organizer-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pi_folder_organizer-2.2.0/PKG-INFO` & `pi_folder_organizer-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-folder-organizer
-Version: 2.2.0
+Version: 2.2.1
 Summary: A Python package for cleaning up cluttered files and organizing them into respective folders.
 Author: Qadeer Ahmad
 Author-email: mrqdeer1231122@gmail.com
 Keywords: python,file organization,file cleanup,cluttered files,folder management,data organization,file management,data cleanup,Python package,developer tools,data processing,file sorting,data structuring,automated file organization,Python library,data management,data handling,file optimization,data optimization
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pi_folder_organizer-2.2.0/README.md` & `pi_folder_organizer-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pi_folder_organizer-2.2.0/pi_folder_organizer/pi_folder_organizer.py` & `pi_folder_organizer-2.2.1/pi_folder_organizer/pi_folder_organizer.py`

 * *Files identical despite different names*

### Comparing `pi_folder_organizer-2.2.0/pi_folder_organizer.egg-info/PKG-INFO` & `pi_folder_organizer-2.2.1/pi_folder_organizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-folder-organizer
-Version: 2.2.0
+Version: 2.2.1
 Summary: A Python package for cleaning up cluttered files and organizing them into respective folders.
 Author: Qadeer Ahmad
 Author-email: mrqdeer1231122@gmail.com
 Keywords: python,file organization,file cleanup,cluttered files,folder management,data organization,file management,data cleanup,Python package,developer tools,data processing,file sorting,data structuring,automated file organization,Python library,data management,data handling,file optimization,data optimization
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pi_folder_organizer-2.2.0/setup.py` & `pi_folder_organizer-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.2.0'
+VERSION = '2.2.1' 
 DESCRIPTION = "A Python package for cleaning up cluttered files and organizing them into respective folders."
 # Setting up
 setup(
     name="pi-folder-organizer",
     version=VERSION,
     author="Qadeer Ahmad",
     author_email="mrqdeer1231122@gmail.com",
```

