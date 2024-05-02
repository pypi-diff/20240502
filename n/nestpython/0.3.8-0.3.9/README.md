# Comparing `tmp/nestpython-0.3.8.tar.gz` & `tmp/nestpython-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestpython-0.3.8.tar", last modified: Fri Apr  5 19:36:10 2024, max compression
+gzip compressed data, was "nestpython-0.3.9.tar", last modified: Sat Apr  6 16:22:59 2024, max compression
```

## Comparing `nestpython-0.3.8.tar` & `nestpython-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 19:36:10.938306 nestpython-0.3.8/
--rw-rw-rw-   0        0        0     1346 2024-04-05 19:36:10.936313 nestpython-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-05 19:36:10.000000 nestpython-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 19:36:10.928337 nestpython-0.3.8/nestpy/
--rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.8/nestpy/__init__.py
--rw-rw-rw-   0        0        0     2340 2024-04-01 14:53:49.000000 nestpython-0.3.8/nestpy/files.py
--rw-rw-rw-   0        0        0    14329 2024-04-05 19:35:29.000000 nestpython-0.3.8/nestpy/main.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:36:10.934318 nestpython-0.3.8/nestpython.egg-info/
--rw-rw-rw-   0        0        0     1346 2024-04-05 19:36:10.000000 nestpython-0.3.8/nestpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-05 19:36:10.000000 nestpython-0.3.8/nestpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 19:36:10.000000 nestpython-0.3.8/nestpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-05 19:36:10.000000 nestpython-0.3.8/nestpython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 19:36:10.938306 nestpython-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1085 2024-04-01 18:32:02.000000 nestpython-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:22:59.850209 nestpython-0.3.9/
+-rw-rw-rw-   0        0        0     1346 2024-04-06 16:22:59.846221 nestpython-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-06 16:22:58.000000 nestpython-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 16:22:59.832259 nestpython-0.3.9/nestpy/
+-rw-rw-rw-   0        0        0       39 2024-04-01 14:53:49.000000 nestpython-0.3.9/nestpy/__init__.py
+-rw-rw-rw-   0        0        0     3347 2024-04-06 16:09:19.000000 nestpython-0.3.9/nestpy/files.py
+-rw-rw-rw-   0        0        0    14329 2024-04-06 14:59:20.000000 nestpython-0.3.9/nestpy/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:22:59.843229 nestpython-0.3.9/nestpython.egg-info/
+-rw-rw-rw-   0        0        0     1346 2024-04-06 16:22:59.000000 nestpython-0.3.9/nestpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-06 16:22:59.000000 nestpython-0.3.9/nestpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 16:22:59.000000 nestpython-0.3.9/nestpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-06 16:22:59.000000 nestpython-0.3.9/nestpython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 16:22:59.851206 nestpython-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-04-01 18:32:02.000000 nestpython-0.3.9/setup.py
```

### Comparing `nestpython-0.3.8/PKG-INFO` & `nestpython-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestpython
-Version: 0.3.8
+Version: 0.3.9
 Summary: python with braces.
 Author: slycedf
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
 ## nestpy
```

### Comparing `nestpython-0.3.8/nestpy/files.py` & `nestpython-0.3.9/nestpy/files.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 from enum import Enum as _Enum
 from glob import glob as _glob
 from os import mkdir as _mkdir
 from os import path as _path
 from os import remove as _remove
 from os import walk as _walk
+from os import scandir as _scandir
+from os import chdir as _chdir
+from os import getcwd as _getcwd
 from shutil import copyfile as _copyfile
 from shutil import rmtree as _rmtree
 
 from . import main as _m
 
-slashConverter = str.maketrans('\\','/')
+_slashConverter = str.maketrans('\\','/')
 def _getAllFilePaths(dirPath):
     return [
-        _path.join(dirpath,f).translate(slashConverter) for (
+        _path.join(dirpath,f).translate(_slashConverter) for (
             dirpath, dirnames, filenames
         ) in _walk(dirPath) for f in filenames
     ]
 
+def _getFilesDirs(dirPath):
+    oldDir=_getcwd()
+    _chdir(dirPath)
+    a = []
+    b = []
+    for f in _scandir():
+        g = f.path.translate(_slashConverter).removeprefix('./')
+        if f.is_dir():
+            b.append(g)
+        else:
+            a.append(g)
+    _chdir(oldDir)
+    return a, b
+
 def _filterByFileExt(files, fileExt):
     passed = []
     failed = []
     for file in files:
         if _path.splitext(file)[-1] == fileExt:
             passed.append(file)
             continue
@@ -40,37 +57,56 @@
     compile(file)
   else:
     i = input(
       f'File \'{file}\' already exists. Would you like to overwrite it? [y/(n)]: ')
     if i.lower() == 'y':
       compile(file)
 
-def nbuild(dir, new_dir, indent_amount=1, erase_dir=False, 
+
+def nbuild(dir, new_dir, indent_amount=1, erase_dir=None,
            replace_previous=False, transfer_other_files=True):
-    if _path.isdir(new_dir):
+ subpath = ''
+ def subbuild():
+    nonlocal dir
+    nonlocal subpath
+    nonlocal new_dir
+    nonlocal indent_amount
+    nonlocal erase_dir
+    nonlocal replace_previous
+    nonlocal transfer_other_files
+    print(subpath)
+    if _path.isdir(f'{new_dir}/{subpath}'):
       def remove():
-        _rmtree(new_dir)
-        _mkdir(new_dir)
-      if erase_dir:
-        remove()
-      else:
-        i = input(
-          f'Directory \'{new_dir}\' already exists. Would you like to erase it? [y/(n)]: ')
-        if i.lower() == 'y':
+        _rmtree(f'{new_dir}/{subpath}')
+        _mkdir(f'{new_dir}/{subpath}')
+      match erase_dir:
+        case True:
           remove()
+        case None:
+          i = input(
+            f'Directory \'{new_dir}/{subpath}\' already exists. Would you like to erase it? [y/(n)]: ')
+          if i.lower() == 'y':
+            remove()
+
     else:
-      _mkdir(new_dir)
-    compilable, leaveBe = _filterByFileExt(_getAllFilePaths(dir), '.npy')
+      _mkdir(f'{new_dir}/{subpath}')
+    compilable, leaveBe = _filterByFileExt(_getFilesDirs(f'{dir}/{subpath}')[0], '.npy')
+    print(_getFilesDirs(f'{dir}/{subpath}'))
     for file in compilable:
-      ncompile_to(file, f'{new_dir}/{file.split("/")[-1].rsplit(".", 1)[0]}.py', 
+      ncompile_to(f'{dir}/{subpath}/{file}', f'{new_dir}/{subpath}/{file.rsplit("/", 1)[-1].rsplit(".", 1)[0]}.py',
                indent_amount, replace_previous)
     if transfer_other_files:
       for file in leaveBe:
-        print(f'> transferring {file}')
-        _copyfile(file, f'{new_dir}/{file.split("/")[-1]}')
+        print(f'> transferring {dir}/{subpath}/{file}')
+        _copyfile(f'{dir}/{subpath}/{file}', f'{new_dir}/{subpath}/{file.rsplit("/", 1)[-1].lstrip("/")}')
+    for subdir in _getFilesDirs(f'{dir}/{subpath}')[~0]:
+        subpath += subdir
+        subbuild()
+
+ subbuild()
 
 def ncompile(file, indent_amount=1):
   with open(file, 'r') as f:
     return _m.ncompile(f.read(), indent_amount)
 
 def nexec(file):
   exec(ncompile(file))
```

### Comparing `nestpython-0.3.8/nestpy/main.py` & `nestpython-0.3.9/nestpy/main.py`

 * *Files identical despite different names*

### Comparing `nestpython-0.3.8/nestpython.egg-info/PKG-INFO` & `nestpython-0.3.9/nestpython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestpython
-Version: 0.3.8
+Version: 0.3.9
 Summary: python with braces.
 Author: slycedf
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
 ## nestpy
```

### Comparing `nestpython-0.3.8/setup.py` & `nestpython-0.3.9/setup.py`

 * *Files identical despite different names*

