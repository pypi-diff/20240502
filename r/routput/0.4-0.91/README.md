# Comparing `tmp/routput-0.4.tar.gz` & `tmp/routput-0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.4.tar", last modified: Wed May  1 23:49:43 2024, max compression
+gzip compressed data, was "routput-0.91.tar", last modified: Thu May  2 00:59:07 2024, max compression
```

## Comparing `routput-0.4.tar` & `routput-0.91.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-01 23:49:43.156872 routput-0.4/
--rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-04-14 05:51:33.000000 routput-0.4/LICENCE
--rw-r--r--   0 joel-watson   (501) staff       (20)     2505 2024-05-01 23:49:43.155975 routput-0.4/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)     2000 2024-05-01 23:41:41.000000 routput-0.4/README.md
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-01 23:49:43.152798 routput-0.4/routput/
--rw-r--r--   0 joel-watson   (501) staff       (20)        0 2024-05-01 23:41:41.000000 routput-0.4/routput/__init__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)       31 2024-05-01 23:41:41.000000 routput-0.4/routput/__main__.py
--rw-r--r--   0 joel-watson   (501) staff       (20)     7856 2024-05-01 23:41:41.000000 routput-0.4/routput/routput.py
-drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-01 23:49:43.155277 routput-0.4/routput.egg-info/
--rw-r--r--   0 joel-watson   (501) staff       (20)     2505 2024-05-01 23:49:42.000000 routput-0.4/routput.egg-info/PKG-INFO
--rw-r--r--   0 joel-watson   (501) staff       (20)      209 2024-05-01 23:49:42.000000 routput-0.4/routput.egg-info/SOURCES.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-01 23:49:42.000000 routput-0.4/routput.egg-info/dependency_links.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)        8 2024-05-01 23:49:42.000000 routput-0.4/routput.egg-info/top_level.txt
--rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-01 23:49:43.157069 routput-0.4/setup.cfg
--rw-r--r--   0 joel-watson   (501) staff       (20)      451 2024-05-01 23:47:35.000000 routput-0.4/setup.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 00:59:07.846929 routput-0.91/
+-rw-r--r--   0 joel-watson   (501) staff       (20)    25171 2024-04-14 05:51:33.000000 routput-0.91/LICENCE
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2533 2024-05-02 00:59:07.845560 routput-0.91/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2000 2024-05-01 23:41:41.000000 routput-0.91/README.md
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 00:59:07.841287 routput-0.91/routput/
+-rw-r--r--   0 joel-watson   (501) staff       (20)        0 2024-05-01 23:41:41.000000 routput-0.91/routput/__init__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)       31 2024-05-01 23:41:41.000000 routput-0.91/routput/__main__.py
+-rw-r--r--   0 joel-watson   (501) staff       (20)     7856 2024-05-01 23:41:41.000000 routput-0.91/routput/routput.py
+drwxr-xr-x   0 joel-watson   (501) staff       (20)        0 2024-05-02 00:59:07.844416 routput-0.91/routput.egg-info/
+-rw-r--r--   0 joel-watson   (501) staff       (20)     2533 2024-05-02 00:59:07.000000 routput-0.91/routput.egg-info/PKG-INFO
+-rw-r--r--   0 joel-watson   (501) staff       (20)      209 2024-05-02 00:59:07.000000 routput-0.91/routput.egg-info/SOURCES.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        1 2024-05-02 00:59:07.000000 routput-0.91/routput.egg-info/dependency_links.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)        8 2024-05-02 00:59:07.000000 routput-0.91/routput.egg-info/top_level.txt
+-rw-r--r--   0 joel-watson   (501) staff       (20)       38 2024-05-02 00:59:07.847081 routput-0.91/setup.cfg
+-rw-r--r--   0 joel-watson   (501) staff       (20)      541 2024-05-02 00:57:44.000000 routput-0.91/setup.py
```

### Comparing `routput-0.4/LICENCE` & `routput-0.91/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.4/PKG-INFO` & `routput-0.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.4
+Version: 0.91
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
+Requires: templated_setup
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Recursive Output Utility
 
 ## Overview
 
@@ -86,9 +87,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.4 released on 2nd/5/2024
+## V0.91 released on 2nd/5/2024
 hopefully we will be able to install from pip. :p
```

### Comparing `routput-0.4/README.md` & `routput-0.91/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.4/routput/routput.py` & `routput-0.91/routput/routput.py`

 * *Files identical despite different names*

### Comparing `routput-0.4/routput.egg-info/PKG-INFO` & `routput-0.91/routput.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.4
+Version: 0.91
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
+Requires: templated_setup
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Recursive Output Utility
 
 ## Overview
 
@@ -86,9 +87,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.4 released on 2nd/5/2024
+## V0.91 released on 2nd/5/2024
 hopefully we will be able to install from pip. :p
```

