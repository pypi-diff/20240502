# Comparing `tmp/sheval-1.1.0.tar.gz` & `tmp/sheval-1.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheval-1.1.0.tar", max compression
+gzip compressed data, was "sheval-1.1.0.post1.tar", max compression
```

## Comparing `sheval-1.1.0.tar` & `sheval-1.1.0.post1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    35065 2022-09-17 21:15:26.861224 sheval-1.1.0/LICENSE
--rw-r--r--   0        0        0      556 2022-12-03 23:55:24.252106 sheval-1.1.0/README.md
--rw-r--r--   0        0        0      455 2022-12-04 00:13:00.785595 sheval-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     7271 2022-12-04 00:12:26.616305 sheval-1.1.0/sheval/__init__.py
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 sheval-1.1.0/setup.py
--rw-r--r--   0        0        0     1168 1970-01-01 00:00:00.000000 sheval-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35084 2024-05-02 16:50:13.906154 sheval-1.1.0.post1/LICENSE
+-rw-r--r--   0        0        0      556 2024-05-02 16:50:39.569077 sheval-1.1.0.post1/README.md
+-rw-r--r--   0        0        0      461 2024-05-02 17:06:24.397835 sheval-1.1.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     7247 2024-05-02 17:03:32.040447 sheval-1.1.0.post1/sheval/__init__.py
+-rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 sheval-1.1.0.post1/PKG-INFO
```

### Comparing `sheval-1.1.0/LICENSE` & `sheval-1.1.0.post1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -627,16 +627,16 @@
 free software which everyone can redistribute and change under these terms.
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
-    deval
-    Copyright (C) 2022  deepadmax
+    sheval
+    Copyright (C) 2022  Maximillian Strand
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
@@ -648,15 +648,15 @@
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
   If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
-    <program>  Copyright (C) 2022  deepadmax
+    <program>  Copyright (C) 2022  Maximillian Strand
     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
     This is free software, and you are welcome to redistribute it
     under certain conditions; type `show c' for details.
 
 The hypothetical commands `show w' and `show c' should show the appropriate
 parts of the General Public License.  Of course, your program's commands
 might be different; for a GUI interface, you would use an "about box".
```

### Comparing `sheval-1.1.0/README.md` & `sheval-1.1.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `sheval-1.1.0/sheval/__init__.py` & `sheval-1.1.0.post1/sheval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-__version__ = '1.0.4'
-
-
 from typing import Union, Callable
 import ast
 
 
 SafeType = Union[str, int, float, complex, list, tuple, set, dict, bool, bytes, None]
```

### Comparing `sheval-1.1.0/PKG-INFO` & `sheval-1.1.0.post1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sheval
-Version: 1.1.0
+Version: 1.1.0.post1
 Summary: Safely evaluate mathematical and logical expressions.
 Home-page: https://gitlab.com/deepadmax/sheval
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maxi@millian.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://gitlab.com/deepadmax/sheval
 Description-Content-Type: text/markdown
 
 # 🐴 sheval
 
 Safely evaluate mathematical and logical expressions. Most operations are supported.
```

