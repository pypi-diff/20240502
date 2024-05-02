# Comparing `tmp/pycatfile-0.9.2.tar.gz` & `tmp/pycatfile-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatfile-0.9.2.tar", last modified: Tue Apr 30 21:57:33 2024, max compression
+gzip compressed data, was "pycatfile-0.9.4.tar", last modified: Thu May  2 01:11:38 2024, max compression
```

## Comparing `pycatfile-0.9.2.tar` & `pycatfile-0.9.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:57:33.053427 pycatfile-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-30 21:57:25.000000 pycatfile-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-30 21:57:33.053427 pycatfile-0.9.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:57:33.053427 pycatfile-0.9.2/PyCatFile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-30 21:57:33.000000 pycatfile-0.9.2/PyCatFile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-30 21:57:33.000000 pycatfile-0.9.2/PyCatFile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:57:33.000000 pycatfile-0.9.2/PyCatFile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 21:57:33.000000 pycatfile-0.9.2/PyCatFile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:57:33.000000 pycatfile-0.9.2/PyCatFile.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 21:57:25.000000 pycatfile-0.9.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     9957 2024-04-30 21:57:25.000000 pycatfile-0.9.2/catfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4969 2024-04-30 21:57:25.000000 pycatfile-0.9.2/neocatfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   360786 2024-04-30 21:57:25.000000 pycatfile-0.9.2/pycatfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-30 21:57:33.053427 pycatfile-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5451 2024-04-30 21:57:25.000000 pycatfile-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:11:38.355999 pycatfile-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-02 01:11:29.000000 pycatfile-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 01:11:38.355999 pycatfile-0.9.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:11:38.355999 pycatfile-0.9.4/PyCatFile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 01:11:38.000000 pycatfile-0.9.4/PyCatFile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 01:11:38.000000 pycatfile-0.9.4/PyCatFile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:11:38.000000 pycatfile-0.9.4/PyCatFile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 01:11:38.000000 pycatfile-0.9.4/PyCatFile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:11:38.000000 pycatfile-0.9.4/PyCatFile.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 01:11:29.000000 pycatfile-0.9.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9956 2024-05-02 01:11:29.000000 pycatfile-0.9.4/catfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4968 2024-05-02 01:11:29.000000 pycatfile-0.9.4/neocatfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   305547 2024-05-02 01:11:29.000000 pycatfile-0.9.4/pycatfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 01:11:38.355999 pycatfile-0.9.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5450 2024-05-02 01:11:29.000000 pycatfile-0.9.4/setup.py
```

### Comparing `pycatfile-0.9.2/LICENSE` & `pycatfile-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycatfile-0.9.2/PKG-INFO` & `pycatfile-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.9.2
+Version: 0.9.4
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `pycatfile-0.9.2/PyCatFile.egg-info/PKG-INFO` & `pycatfile-0.9.4/PyCatFile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.9.2
+Version: 0.9.4
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `pycatfile-0.9.2/catfile.py` & `pycatfile-0.9.4/catfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: catfile.py - Last Update: 4/30/2024 Ver. 0.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: catfile.py - Last Update: 5/1/2024 Ver. 0.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import sys, argparse, pycatfile, binascii;
 
 rarfile_support = pycatfile.rarfile_support;
 py7zr_support = pycatfile.py7zr_support;
```

### Comparing `pycatfile-0.9.2/neocatfile.py` & `pycatfile-0.9.4/neocatfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: neocatfile.py - Last Update: 4/30/2024 Ver. 0.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: neocatfile.py - Last Update: 5/1/2024 Ver. 0.9.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 import argparse
 import pycatfile
 
 # Compatibility layer for Python 2 and 3 input
```

### Comparing `pycatfile-0.9.2/setup.py` & `pycatfile-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2016-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2016-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2016-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: setup.py - Last Update: 4/30/2024 Ver. 0.9.2 RC 1 - Author: cooldude2k $
+    $FileInfo: setup.py - Last Update: 5/1/2024 Ver. 0.9.4 RC 1 - Author: cooldude2k $
 '''
 
 import os, re, sys, pkg_resources;
 from setuptools import setup;
 
 verinfofilename = os.path.realpath("."+os.path.sep+os.path.sep+"pycatfile.py");
 verinfofile = open(verinfofilename, "r");
```

