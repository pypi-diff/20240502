# Comparing `tmp/pytket_pecos-0.1.8.tar.gz` & `tmp/pytket_pecos-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket_pecos-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytket_pecos-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytket_pecos-0.1.8.tar` & `pytket_pecos-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      270 2023-12-12 11:14:16.004456 pytket_pecos-0.1.8/.github/dependabot.yml
--rw-r--r--   0        0        0      612 2023-12-12 14:38:33.015343 pytket_pecos-0.1.8/.github/workflows/test.yml
--rw-r--r--   0        0        0       13 2023-12-12 11:14:16.004456 pytket_pecos-0.1.8/.gitignore
--rw-r--r--   0        0        0     9161 2023-12-12 11:14:16.004456 pytket_pecos-0.1.8/LICENSE
--rw-r--r--   0        0        0      699 2024-01-15 15:39:46.184190 pytket_pecos-0.1.8/README.md
--rw-r--r--   0        0        0      837 2024-01-16 10:59:35.630027 pytket_pecos-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      159 2023-12-12 11:14:16.004456 pytket_pecos-0.1.8/src/pytket_pecos/__init__.py
--rw-r--r--   0        0        0     1549 2024-01-16 10:57:57.811255 pytket_pecos-0.1.8/src/pytket_pecos/emulator.py
--rw-r--r--   0        0        0       20 2023-12-12 11:14:16.004456 pytket_pecos-0.1.8/test/__init__.py
--rw-r--r--   0        0        0     2967 2024-01-16 10:58:18.131831 pytket_pecos-0.1.8/test/test_emulator.py
--rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 pytket_pecos-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      270 2024-01-16 14:24:53.834721 pytket_pecos-0.1.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      620 2024-01-18 08:33:33.256621 pytket_pecos-0.1.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0       13 2023-11-29 15:38:04.003304 pytket_pecos-0.1.9/.gitignore
+-rw-r--r--   0        0        0     9161 2023-11-29 15:38:04.003304 pytket_pecos-0.1.9/LICENSE
+-rw-r--r--   0        0        0      705 2024-01-18 08:33:33.256621 pytket_pecos-0.1.9/README.md
+-rw-r--r--   0        0        0      883 2024-01-18 08:34:45.548961 pytket_pecos-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      159 2023-12-06 13:14:25.598431 pytket_pecos-0.1.9/src/pytket_pecos/__init__.py
+-rw-r--r--   0        0        0     1549 2023-12-07 12:18:23.257797 pytket_pecos-0.1.9/src/pytket_pecos/emulator.py
+-rw-r--r--   0        0        0       20 2023-11-29 15:38:04.003304 pytket_pecos-0.1.9/test/__init__.py
+-rw-r--r--   0        0        0     2967 2024-01-16 14:24:53.834721 pytket_pecos-0.1.9/test/test_emulator.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 pytket_pecos-0.1.9/PKG-INFO
```

### Comparing `pytket_pecos-0.1.8/.github/workflows/test.yml` & `pytket_pecos-0.1.9/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     branches:
       - 'main'
 jobs:
   run_tests:
     strategy:
       matrix:
         os: ['ubuntu-22.04', 'macos-12', 'macos-13-xlarge', 'windows-2022']
-        pyver: ['3.10', '3.11']
+        pyver: ['3.10', '3.11', '3.12']
     runs-on:
       ${{ matrix.os }}
     steps:
     - uses: actions/checkout@v4
     - name: Set up python
       uses: actions/setup-python@v5
       with:
```

### Comparing `pytket_pecos-0.1.8/LICENSE` & `pytket_pecos-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytket_pecos-0.1.8/README.md` & `pytket_pecos-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 This package enables emulation of [pytket](https://github.com/CQCL/tket)
 circuits using the
 [PECOS](https://github.com/PECOS-packages/PECOS/tree/development) emulator.
 
 ## Installation
 
-Installation requires Python 3.10 or 3.11. Linux, MacOS and Windows are all
-supported.
+Installation requires Python 3.10, 3.11 or 3.12. Linux, MacOS and Windows are
+all supported.
 
 ### From pypi
 
 ```shell
 pip install pytket_pecos
 ```
```

### Comparing `pytket_pecos-0.1.8/pyproject.toml` & `pytket_pecos-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "pytket_pecos"
-version = "0.1.8"
+version = "0.1.9"
 description = "This package enables emulation of pytket circuits using the PECOS emulator."
 authors = [{name = "Alec Edgington", email = "alec.edgington@quantinuum.com"}]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows"
     ]
 dependencies = [
-    "pytket >= 1.23.0",
-    "pytket-phir >= 0.2.0",
+    "pytket >= 1.24.0",
+    "pytket-phir >= 0.2.1",
     "projectq >= 0.8.0",
     "quantum-pecos >= 0.5.0dev6"
     ]
 
 [project.urls]
 Home = "https://github.com/CQCL/pytket-pecos"
```

### Comparing `pytket_pecos-0.1.8/src/pytket_pecos/emulator.py` & `pytket_pecos-0.1.9/src/pytket_pecos/emulator.py`

 * *Files identical despite different names*

### Comparing `pytket_pecos-0.1.8/test/test_emulator.py` & `pytket_pecos-0.1.9/test/test_emulator.py`

 * *Files identical despite different names*

### Comparing `pytket_pecos-0.1.8/PKG-INFO` & `pytket_pecos-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pytket_pecos
-Version: 0.1.8
+Version: 0.1.9
 Summary: This package enables emulation of pytket circuits using the PECOS emulator.
 Author-email: Alec Edgington <alec.edgington@quantinuum.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Dist: pytket >= 1.23.0
-Requires-Dist: pytket-phir >= 0.2.0
+Requires-Dist: pytket >= 1.24.0
+Requires-Dist: pytket-phir >= 0.2.1
 Requires-Dist: projectq >= 0.8.0
 Requires-Dist: quantum-pecos >= 0.5.0dev6
 Project-URL: Home, https://github.com/CQCL/pytket-pecos
```

