# Comparing `tmp/gfloat-0.0.5.tar.gz` & `tmp/gfloat-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfloat-0.0.5.tar", last modified: Tue Apr  2 14:34:02 2024, max compression
+gzip compressed data, was "gfloat-0.1.tar", last modified: Thu May  2 12:05:40 2024, max compression
```

## Comparing `gfloat-0.0.5.tar` & `gfloat-0.1.tar`

### file list

```diff
@@ -1,41 +1,55 @@
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.490228 gfloat-0.0.5/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/.github/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/.github/workflows/
--rw-r--r--   0 awf       (1000) awf       (1000)      667 2024-03-21 17:30:20.000000 gfloat-0.0.5/.github/workflows/ci.yaml
--rw-r--r--   0 awf       (1000) awf       (1000)     3099 2024-02-15 18:32:26.000000 gfloat-0.0.5/.gitignore
--rw-r--r--   0 awf       (1000) awf       (1000)      301 2024-01-27 13:52:18.000000 gfloat-0.0.5/.readthedocs.yaml
--rw-r--r--   0 awf       (1000) awf       (1000)     1074 2024-01-27 13:41:22.000000 gfloat-0.0.5/LICENSE
--rw-r--r--   0 awf       (1000) awf       (1000)     1586 2024-04-02 14:34:02.490228 gfloat-0.0.5/PKG-INFO
--rw-r--r--   0 awf       (1000) awf       (1000)      907 2024-04-02 14:30:00.000000 gfloat-0.0.5/README.md
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/docs/
--rw-r--r--   0 awf       (1000) awf       (1000)      638 2024-01-27 16:06:55.000000 gfloat-0.0.5/docs/Makefile
--rw-r--r--   0 awf       (1000) awf       (1000)      799 2024-01-27 13:41:22.000000 gfloat-0.0.5/docs/make.bat
--rw-r--r--   0 awf       (1000) awf       (1000)        8 2024-03-22 15:17:01.000000 gfloat-0.0.5/docs/requirements-rtd.txt
--rw-r--r--   0 awf       (1000) awf       (1000)       41 2024-01-27 13:41:22.000000 gfloat-0.0.5/docs/requirements.txt
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/docs/source/
--rw-r--r--   0 awf       (1000) awf       (1000)      876 2024-04-02 14:33:41.000000 gfloat-0.0.5/docs/source/conf.py
--rw-r--r--   0 awf       (1000) awf       (1000)     1618 2024-04-02 14:30:00.000000 gfloat-0.0.5/docs/source/index.rst
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/notebooks/
--rw-r--r--   0 awf       (1000) awf       (1000)    10166 2024-03-21 14:24:19.000000 gfloat-0.0.5/notebooks/01-decode.ipynb
--rw-r--r--   0 awf       (1000) awf       (1000)      909 2024-04-02 14:33:48.000000 gfloat-0.0.5/pyproject.toml
--rw-r--r--   0 awf       (1000) awf       (1000)       49 2024-03-21 17:23:18.000000 gfloat-0.0.5/requirements-test.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        6 2024-03-22 15:19:02.000000 gfloat-0.0.5/requirements.txt
--rw-r--r--   0 awf       (1000) awf       (1000)       38 2024-04-02 14:34:02.490228 gfloat-0.0.5/setup.cfg
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/src/
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.480228 gfloat-0.0.5/src/gfloat/
--rw-r--r--   0 awf       (1000) awf       (1000)      365 2024-04-02 14:30:00.000000 gfloat-0.0.5/src/gfloat/__init__.py
--rw-r--r--   0 awf       (1000) awf       (1000)     2471 2024-04-02 14:30:00.000000 gfloat-0.0.5/src/gfloat/decode.py
--rw-r--r--   0 awf       (1000) awf       (1000)     2228 2024-04-02 14:30:00.000000 gfloat-0.0.5/src/gfloat/formats.py
--rw-r--r--   0 awf       (1000) awf       (1000)     6093 2024-04-02 14:30:00.000000 gfloat-0.0.5/src/gfloat/round.py
--rw-r--r--   0 awf       (1000) awf       (1000)     9526 2024-04-02 14:30:00.000000 gfloat-0.0.5/src/gfloat/types.py
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.490228 gfloat-0.0.5/src/gfloat.egg-info/
--rw-r--r--   0 awf       (1000) awf       (1000)     1586 2024-04-02 14:34:02.000000 gfloat-0.0.5/src/gfloat.egg-info/PKG-INFO
--rw-r--r--   0 awf       (1000) awf       (1000)      623 2024-04-02 14:34:02.000000 gfloat-0.0.5/src/gfloat.egg-info/SOURCES.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        1 2024-04-02 14:34:02.000000 gfloat-0.0.5/src/gfloat.egg-info/dependency_links.txt
--rw-r--r--   0 awf       (1000) awf       (1000)       63 2024-04-02 14:34:02.000000 gfloat-0.0.5/src/gfloat.egg-info/requires.txt
--rw-r--r--   0 awf       (1000) awf       (1000)        7 2024-04-02 14:34:02.000000 gfloat-0.0.5/src/gfloat.egg-info/top_level.txt
-drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-04-02 14:34:02.490228 gfloat-0.0.5/test/
--rw-r--r--   0 awf       (1000) awf       (1000)     4140 2024-04-02 14:30:00.000000 gfloat-0.0.5/test/test_decode.py
--rw-r--r--   0 awf       (1000) awf       (1000)      683 2024-04-02 14:30:00.000000 gfloat-0.0.5/test/test_encode.py
--rw-r--r--   0 awf       (1000) awf       (1000)      968 2024-04-02 14:30:00.000000 gfloat-0.0.5/test/test_finfo.py
--rw-r--r--   0 awf       (1000) awf       (1000)     5572 2024-04-02 14:30:00.000000 gfloat-0.0.5/test/test_round.py
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/.github/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/.github/workflows/
+-rw-r--r--   0 awf       (1000) awf       (1000)      924 2024-05-02 11:54:43.000000 gfloat-0.1/.github/workflows/ci.yaml
+-rw-r--r--   0 awf       (1000) awf       (1000)     3178 2024-05-02 11:54:43.000000 gfloat-0.1/.gitignore
+-rw-r--r--   0 awf       (1000) awf       (1000)      645 2024-05-02 11:54:43.000000 gfloat-0.1/.pre-commit-config.yaml
+-rw-r--r--   0 awf       (1000) awf       (1000)      360 2024-05-02 11:54:43.000000 gfloat-0.1/.readthedocs.yaml
+-rw-r--r--   0 awf       (1000) awf       (1000)      103 2024-05-02 11:54:43.000000 gfloat-0.1/BUILDING.md
+-rw-r--r--   0 awf       (1000) awf       (1000)     1093 2024-05-02 11:54:43.000000 gfloat-0.1/LICENSE
+-rw-r--r--   0 awf       (1000) awf       (1000)     3297 2024-05-02 12:05:40.735762 gfloat-0.1/PKG-INFO
+-rw-r--r--   0 awf       (1000) awf       (1000)     2540 2024-05-02 11:54:43.000000 gfloat-0.1/README.md
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/docs/
+-rw-r--r--   0 awf       (1000) awf       (1000)      638 2024-01-27 16:06:55.000000 gfloat-0.1/docs/Makefile
+-rw-r--r--   0 awf       (1000) awf       (1000)      799 2024-01-27 13:41:22.000000 gfloat-0.1/docs/make.bat
+-rw-r--r--   0 awf       (1000) awf       (1000)        8 2024-03-22 15:17:01.000000 gfloat-0.1/docs/requirements-rtd.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)       74 2024-05-01 12:01:20.000000 gfloat-0.1/docs/requirements.txt
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/docs/source/
+-rw-r--r--   0 awf       (1000) awf       (1000)    12905 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/01-decode.ipynb
+-rw-r--r--   0 awf       (1000) awf       (1000)    25085 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/02-value-stats.ipynb
+-rw-r--r--   0 awf       (1000) awf       (1000)    97024 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/03-value-tables.ipynb
+-rw-r--r--   0 awf       (1000) awf       (1000)      608 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/api.rst
+-rw-r--r--   0 awf       (1000) awf       (1000)      993 2024-05-02 12:05:29.000000 gfloat-0.1/docs/source/conf.py
+-rw-r--r--   0 awf       (1000) awf       (1000)      689 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/formats.rst
+-rw-r--r--   0 awf       (1000) awf       (1000)     1923 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/index.rst
+-rw-r--r--   0 awf       (1000) awf       (1000)      228 2024-05-02 11:54:43.000000 gfloat-0.1/docs/source/notebooks.rst
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/etc/
+-rwxr-xr-x   0 awf       (1000) awf       (1000)      357 2024-05-02 11:54:43.000000 gfloat-0.1/etc/check-copyright.sh
+-rw-r--r--   0 awf       (1000) awf       (1000)      474 2024-05-02 12:05:10.000000 gfloat-0.1/etc/package.sh
+-rw-r--r--   0 awf       (1000) awf       (1000)      637 2024-05-02 11:54:43.000000 gfloat-0.1/etc/test-check-copyright.sh
+-rw-r--r--   0 awf       (1000) awf       (1000)      993 2024-05-02 12:05:29.000000 gfloat-0.1/pyproject.toml
+-rw-r--r--   0 awf       (1000) awf       (1000)       99 2024-05-02 11:54:43.000000 gfloat-0.1/requirements-test.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        6 2024-03-22 15:19:02.000000 gfloat-0.1/requirements.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)       38 2024-05-02 12:05:40.735762 gfloat-0.1/setup.cfg
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/src/
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/src/gfloat/
+-rw-r--r--   0 awf       (1000) awf       (1000)      482 2024-05-01 12:01:20.000000 gfloat-0.1/src/gfloat/__init__.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     3161 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/block.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     2815 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/decode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     4989 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/formats.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1586 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/printing.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     6556 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/round.py
+-rw-r--r--   0 awf       (1000) awf       (1000)    11911 2024-05-02 11:54:43.000000 gfloat-0.1/src/gfloat/types.py
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/src/gfloat.egg-info/
+-rw-r--r--   0 awf       (1000) awf       (1000)     3297 2024-05-02 12:05:40.000000 gfloat-0.1/src/gfloat.egg-info/PKG-INFO
+-rw-r--r--   0 awf       (1000) awf       (1000)      948 2024-05-02 12:05:40.000000 gfloat-0.1/src/gfloat.egg-info/SOURCES.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        1 2024-05-02 12:05:40.000000 gfloat-0.1/src/gfloat.egg-info/dependency_links.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)       79 2024-05-02 12:05:40.000000 gfloat-0.1/src/gfloat.egg-info/requires.txt
+-rw-r--r--   0 awf       (1000) awf       (1000)        7 2024-05-02 12:05:40.000000 gfloat-0.1/src/gfloat.egg-info/top_level.txt
+drwxr-xr-x   0 awf       (1000) awf       (1000)        0 2024-05-02 12:05:40.735762 gfloat-0.1/test/
+-rw-r--r--   0 awf       (1000) awf       (1000)      528 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_block.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     7580 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_decode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1242 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_encode.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1006 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_finfo.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     1039 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_printing.py
+-rw-r--r--   0 awf       (1000) awf       (1000)     6222 2024-05-02 11:54:43.000000 gfloat-0.1/test/test_round.py
```

### Comparing `gfloat-0.0.5/.github/workflows/ci.yaml` & `gfloat-0.1/.github/workflows/ci.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-name: unit tests
+# Copyright (c) 2024 Graphcore Ltd.  All rights reserved.
+
+name: CI
 on:
   pull_request:
   push:
     branches: [main]
 
 jobs:
   pytest-container:
@@ -21,15 +23,22 @@
           pip install .[test]
           pip install -r docs/requirements.txt
 
       - name: Log installed environment
         run: |
           python3 -m pip freeze
 
+      - name: Pre-commit all files
+        run: |
+          pre-commit run --all-files
+
       - name: Run unit tests
         run: |
           pytest .
 
+      - name: MyPy
+        run: |
+          mypy  --disallow-untyped-defs --enable-error-code redundant-expr src test
+
       - name: Ensure that docs build
         run: |
           cd docs && make html
-
```

### Comparing `gfloat-0.0.5/.gitignore` & `gfloat-0.1/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright (c) 2024 Graphcore Ltd.  All rights reserved.
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
@@ -155,7 +157,8 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 .vscode/settings.json
+.vscode/launch.json
```

### Comparing `gfloat-0.0.5/LICENSE` & `gfloat-0.1/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Andrew Fitzgibbon
+Copyright (c) 2023 Graphcore Ltd.  All rights reserved.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `gfloat-0.0.5/docs/Makefile` & `gfloat-0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gfloat-0.0.5/docs/make.bat` & `gfloat-0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gfloat-0.0.5/docs/source/conf.py` & `gfloat-0.1/docs/source/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # Copyright (c) 2024 Graphcore Ltd. All rights reserved.
 
 # Configuration file for the Sphinx documentation builder.
 
 # -- Project information
 
 project = "GFloat"
-copyright = "2023, Andrew Fitzgibbon"
+copyright = "2024, Graphcore Ltd"
 author = "Andrew Fitzgibbon"
-release = "0.0.5"
-version = "0.0.5"
+release = "0.1"  # Set version in package.sh
+version = "0.1"  # Set version in package.sh
 
 # -- General configuration
 
 extensions = [
     "sphinx.ext.duration",
     "sphinx.ext.doctest",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
+    "sphinx.ext.napoleon",
+    "sphinx_paramlinks",
+    "myst_nb",
 ]
 
 autodoc_default_options = {
     "member-order": "bysource",
 }
 
 intersphinx_mapping = {
```

### Comparing `gfloat-0.0.5/pyproject.toml` & `gfloat-0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+# Copyright (c) 2024 Graphcore Ltd. All rights reserved.
+
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ['gfloat']
 package-dir = {"" = "src"}
 
 [project]
 name =  "gfloat"
-version = "0.0.5"
+version = "0.1" # Set version in package.sh
 authors = [
     {name = "Andrew Fitzgibbon", email = "awf@fitzgibbon.ie"},
 ]
 description = "Generic floating point handling in Python"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `gfloat-0.0.5/src/gfloat/decode.py` & `gfloat-0.1/src/gfloat/decode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 # Copyright (c) 2024 Graphcore Ltd. All rights reserved.
 
-from .types import FormatInfo, FloatValue, FloatClass
-
 import numpy as np
 
+from .types import FloatClass, FloatValue, FormatInfo
+
 
 def decode_float(fi: FormatInfo, i: int) -> FloatValue:
-    """
+    r"""
     Given :py:class:`FormatInfo` and integer code point, decode to a :py:class:`FloatValue`
 
-    :param fi: Foating point format descriptor.
-    :type fi: FormatInfo
-
-    :param i: Integer code point, in the range :math:`0 \le i < 2^{k}`,
-              where :math:`k` = ``fi.k``
-    :type i: int
-
-    :return: Decoded float value
-    :rtype: FloatValue
-
-    :raise ValueError: If i is outside the range of valid code points in fi.
+    Args:
+      fi (FormatInfo): Floating point format descriptor.
+      i (int):  Integer code point, in the range :math:`0 \le i < 2^{k}`,
+                where :math:`k` = ``fi.k``
+
+    Returns:
+      Decoded float value
+
+    Raises:
+      ValueError:
+        If :paramref:`i` is outside the range of valid code points in :paramref:`fi`.
     """
     k = fi.k
     p = fi.precision
-    t = p - 1  # trailing significand field width
-    w = k - p
+    t = p - 1  # Trailing significand field width
+    num_signbits = 1 if fi.is_signed else 0
+    w = k - t - num_signbits  # Exponent field width
 
     if i < 0 or i >= 2**k:
         raise ValueError(f"Code point {i} not in range [0, 2**{k})")
 
-    signmask = 1 << (k - 1)
-    signbit = 1 if i & signmask else 0
-    sign = -1 if signbit else 1
+    if fi.is_signed:
+        signmask = 1 << (k - 1)
+        signbit = 1 if i & signmask else 0
+        sign = -1 if signbit else 1
+    else:
+        signmask = None
+        signbit = 0
+        sign = 1
 
-    exp = (i & (signmask - 1)) >> t
+    exp = (i >> t) & ((1 << w) - 1)
     significand = i & ((1 << t) - 1)
+    if fi.is_twos_complement and signbit:
+        significand = (1 << t) - significand
 
     expBias = fi.expBias
 
-    iszero = exp == 0 and significand == 0
+    iszero = exp == 0 and significand == 0 and fi.has_zero
     issubnormal = fi.has_subnormals and (exp == 0) and (significand != 0)
     isnormal = not iszero and not issubnormal
     if iszero or issubnormal:
         expval = 1 - expBias
         fsignificand = significand * 2**-t
     else:
         expval = exp - expBias
@@ -52,23 +60,23 @@
     val = sign * fsignificand * 2.0**expval
 
     # Now overwrite the raw value with specials: Infs, NaN, -0, NaN_0
     signed_infinity = -np.inf if signbit else np.inf
 
     fval = val
     # All-bits-special exponent (ABSE)
-    if exp == 2**w - 1:
+    if w > 0 and exp == 2**w - 1:
         min_i_with_nan = 2 ** (p - 1) - fi.num_high_nans
         if significand >= min_i_with_nan:
             fval = np.nan
         if fi.has_infs and significand == min_i_with_nan - 1:
             fval = signed_infinity
 
     # Negative zero or NaN
-    if i == signmask:
+    if iszero and i == signmask and not fi.is_twos_complement:
         if fi.has_nz:
             fval = -0.0
         else:
             fval = np.nan
 
     # Compute FloatClass
     fclass = None
```

### Comparing `gfloat-0.0.5/src/gfloat/round.py` & `gfloat-0.1/src/gfloat/round.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,92 +1,90 @@
 # Copyright (c) 2024 Graphcore Ltd. All rights reserved.
 
-from enum import Enum
-import numpy as np
 import math
 
-from .types import FormatInfo, RoundMode, FloatValue
-from .decode import decode_float
+import numpy as np
+
+from .types import FormatInfo, RoundMode
 
 
-def _isodd(v: int):
+def _isodd(v: int) -> bool:
     return v & 0x1 == 1
 
 
-def round_float(fi: FormatInfo, v: float, rnd=RoundMode.TiesToEven, sat=False) -> float:
+def round_float(
+    fi: FormatInfo, v: float, rnd: RoundMode = RoundMode.TiesToEven, sat: bool = False
+) -> float:
     """
     Round input to the given :py:class:`FormatInfo`, given rounding mode and saturation flag
 
     An input NaN will convert to a NaN in the target.
-    An input Infinity will convert to the largest float if |sat|,
+    An input Infinity will convert to the largest float if :paramref:`sat`,
     otherwise to an Inf, if present, otherwise to a NaN.
-    Negative zero will be returned if the format has negative zero.
-
-    :param fi: FormatInfo describing the target format
-    :type fi: FormatInfo
-
-    :param v: Input float
-    :type v: float
-
-    :param rnd: Rounding mode to use
-    :type rnd: RoundMode
-
-    :param sat: Saturation flag: if True, round overflowed values to `fi.max`
-    :type sat: bool
-
-    :raises ValueError: The target format cannot represent the input
-       (e.g. converting a NaN, or an Inf when the target has no Inf or NaN, and `¬sat`)
+    Negative zero will be returned if the format has negative zero, otherwise zero.
 
-    :return: A float which equals (inc. nan) one of the values in the format
-    :rtype: float
+    Args:
+      fi (FormatInfo): Describes the target format
+      v (float): Input value to be rounded
+      rnd (RoundMode): Rounding mode to use
+      sat (bool): Saturation flag: if True, round overflowed values to `fi.max`
+
+    Returns:
+      A float which is one of the values in the format.
+
+    Raises:
+       ValueError: The target format cannot represent the input
+             (e.g. converting a `NaN`, or an `Inf` when the target has no
+             `NaN` or `Inf`, and :paramref:`sat` is false)
     """
 
     # Constants
-    k = fi.k
     p = fi.precision
-    w = fi.expBits
     bias = fi.expBias
     t = p - 1
 
     if np.isnan(v):
         if fi.num_nans == 0:
             raise ValueError(f"No NaN in format {fi}")
 
         # Note that this does not preserve the NaN payload
         return np.nan
 
     # Extract sign
-    sign = np.signbit(v)
+    sign = np.signbit(v) and fi.is_signed
     vpos = -v if sign else v
 
-    if vpos < fi.smallest_subnormal / 2:
+    if np.isinf(vpos):
+        result = np.inf
+
+    elif fi.has_subnormals and vpos < fi.smallest_subnormal / 2:
         # Test against smallest_subnormal to avoid subnormals in frexp below
         # Note that this restricts us to types narrower than float64
-        result = 0
-
-    elif np.isinf(vpos):
-        result = np.inf
+        result = 0.0
 
     else:
         # Extract significand (mantissa) and exponent
         fsignificand, expval = np.frexp(vpos)
         assert fsignificand >= 0.5 and fsignificand < 1.0
         # Bring significand into range [1.0, 2.0)
         fsignificand *= 2
         expval -= 1
 
         # Effective precision, accounting for right shift for subnormal values
         biased_exp = expval + bias
-        effective_precision = t + min(biased_exp - 1, 0)
+        if fi.has_subnormals:
+            effective_precision = t + min(biased_exp - 1, 0)
+        else:
+            effective_precision = t
 
         # Lift to "integer * 2^e"
         fsignificand *= 2.0**effective_precision
         expval -= effective_precision
 
-        # round
+        # Round
         isignificand = math.floor(fsignificand)
         if isignificand != fsignificand:
             # Need to round
             if rnd == RoundMode.TowardZero:
                 pass
             elif rnd == RoundMode.TowardPositive:
                 isignificand += 1 if not sign else 0
@@ -117,15 +115,15 @@
     if result == 0:
         if sign and fi.has_nz:
             return -0.0
         else:
             return 0.0
 
     # Overflow
-    if result > fi.max:
+    if result > (-fi.min if sign else fi.max):
         if sat:
             result = fi.max
         else:
             if fi.has_infs:
                 result = np.inf
             elif fi.num_nans > 0:
                 result = np.nan
@@ -139,80 +137,91 @@
     return result
 
 
 def encode_float(fi: FormatInfo, v: float) -> int:
     """
     Encode input to the given :py:class:`FormatInfo`.
 
-    Will round toward zero if v is not in the value set.
-    Will saturate to inf, nan, fi.max in order of precedence.
-    Encode -0 to 0 if not fi.has_nz
-    For other roundings, and saturations, call round_float first.
+    Will round toward zero if :paramref:`v` is not in the value set.
+    Will saturate to `Inf`, `NaN`, `fi.max` in order of precedence.
+    Encode -0 to 0 if not `fi.has_nz`
+
+    For other roundings and saturations, call :func:`round_float` first.
+
+    Args:
+      fi (FormatInfo): Describes the target format
+      v (float): The value to be encoded.
 
-    :return: The integer code point
-    :rtype: int
+    Returns:
+      The integer code point
     """
 
     # Format Constants
     k = fi.bits
     p = fi.precision
     t = p - 1
 
     # Encode
     if np.isnan(v):
         return fi.code_of_nan
 
     # Overflow/underflow
     if v > fi.max:
-        return (
-            fi.code_of_posinf
-            if fi.has_infs
-            else fi.code_of_nan if fi.num_nans > 0 else fi.max
-        )
+        if fi.has_infs:
+            return fi.code_of_posinf
+        if fi.num_nans > 0:
+            return fi.code_of_nan
+        return fi.code_of_max
+
     if v < fi.min:
-        return (
-            fi.code_of_neginf
-            if fi.has_infs
-            else fi.code_of_nan if fi.num_nans > 0 else fi.min
-        )
+        if fi.has_infs:
+            return fi.code_of_neginf
+        if fi.num_nans > 0:
+            return fi.code_of_nan
+        return fi.code_of_min
 
     # Finite values
-    sign = np.signbit(v)
+    sign = fi.is_signed and np.signbit(v)
     vpos = -v if sign else v
 
-    if vpos <= fi.smallest_subnormal / 2:
+    if fi.has_subnormals and vpos <= fi.smallest_subnormal / 2:
         isig = 0
         biased_exp = 0
     else:
         assert fi.bits < 64  # TODO: check implementation if fi is binary64
         sig, exp = np.frexp(vpos)
         # sig in range [0.5, 1)
         sig *= 2
         exp -= 1
         # now sig in range [1, 2)
 
         biased_exp = exp + fi.expBias
-        if biased_exp < 1:
+        if biased_exp < 1 and fi.has_subnormals:
             # subnormal
             sig *= 2.0 ** (biased_exp - 1)
             biased_exp = 0
             assert vpos == sig * 2 ** (1 - fi.expBias)
         else:
             if sig > 0:
                 sig -= 1.0
 
         isig = math.floor(sig * 2**t)
 
     # Zero
-    if isig == 0 and biased_exp == 0:
+    if isig == 0 and biased_exp == 0 and fi.has_zero:
         if sign and fi.has_nz:
             return fi.code_of_negzero
         else:
             return fi.code_of_zero
 
     # Nonzero
     assert isig < 2**t
-    assert biased_exp < 2**fi.expBits
+    assert biased_exp < 2**fi.expBits or fi.is_twos_complement
+
+    # Handle two's complement encoding
+    if fi.is_twos_complement and sign:
+        isig = (1 << t) - isig
 
+    # Pack values into a single integer
     ival = (sign << (k - 1)) | (biased_exp << t) | (isig << 0)
 
     return ival
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gfloat-0.0.5/src/gfloat/types.py` & `gfloat-0.1/src/gfloat/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (c) 2024 Graphcore Ltd. All rights reserved.
 
 from dataclasses import dataclass
 from enum import Enum
-import numpy as np
 
 
 class RoundMode(Enum):
     """
     Enum for IEEE-754 rounding modes.
 
     Result r is obtained from input v depending on rounding mode as follows
@@ -82,28 +81,39 @@
 
     #: Number of NaNs that are encoded in the highest encodings for each sign
     num_high_nans: int
 
     #: Set if format encodes subnormals
     has_subnormals: bool
 
+    #: Set if the format has a sign bit
+    is_signed: bool
+
+    #: Set if the format uses two's complement encoding for the significand
+    is_twos_complement: bool
+
     #: ## Derived values
 
     @property
-    def tSignificandBits(self):
+    def tSignificandBits(self) -> int:
         """The number of trailing significand bits, t"""
         return self.precision - 1
 
     @property
-    def expBits(self):
+    def expBits(self) -> int:
         """The number of exponent bits, w"""
-        return self.k - self.precision
+        return self.k - self.precision + (0 if self.is_signed else 1)
+
+    @property
+    def signBits(self) -> int:
+        """The number of sign bits, s"""
+        return 1 if self.is_signed else 0
 
     @property
-    def expBias(self):
+    def expBias(self) -> int:
         """The exponent bias derived from (p,emax)
 
         This is the bias that should be applied so that
            :math:`floor(log_2(maxFinite)) = emax`
         """
         # Calculate whether all of the all-bits-one-exponent values contain specials.
         # If so, emax will be obtained for exponent value 2^w-2, otherwise it is 2^w-1
@@ -179,35 +189,55 @@
             # binade below, so significand is 0xFFF..F
             isig = 2**self.tSignificandBits - 1
         else:
             # All-bits-one exponent field is not full, value is in the
             # final binade, so significand is 0xFFF..F - num_non_finites
             isig = 2**self.tSignificandBits - 1 - num_non_finites
 
-        return 2**self.emax * (1.0 + isig * 2**-self.tSignificandBits)
+        if self.is_all_subnormal:
+            return 2**self.emax * (isig * 2 ** (1 - self.tSignificandBits))
+        else:
+            return 2**self.emax * (1.0 + isig * 2**-self.tSignificandBits)
 
     @property
     def maxexp(self) -> int:
         """
         The smallest positive power of the base (2) that causes overflow.
         """
         return self.emax + 1
 
     @property
     def min(self) -> float:
         """
         The smallest representable number, typically ``-max``.
         """
-        return -self.max
+        if self.is_signed:
+            if not self.is_twos_complement:
+                return -self.max
+            else:
+                assert not self.has_infs and self.num_high_nans == 0 and not self.has_nz
+                return -(2 ** (self.emax + 1))
+        elif self.has_zero:
+            return 0.0
+        else:
+            return 2**-self.expBias
 
     @property
-    def num_nans(self):
+    def num_nans(self) -> int:
         """
         The number of code points which decode to NaN
         """
+        if not self.is_signed:
+            return self.num_high_nans
+
+        # Signed
+        if self.is_twos_complement:
+            assert not self.has_infs and self.num_high_nans == 0 and not self.has_nz
+            return 0
+
         return (0 if self.has_nz else 1) + 2 * self.num_high_nans
 
     @property
     def code_of_nan(self) -> int:
         """
         Return a codepoint for a NaN
         """
@@ -238,39 +268,57 @@
         return 2**self.k - 1 - self.num_high_nans
 
     @property
     def code_of_zero(self) -> int:
         """
         Return a codepoint for (non-negative) zero
         """
+        assert self.has_zero
         return 0
 
     @property
+    def has_zero(self) -> bool:
+        """
+        Does the format have zero?
+
+        This is false if the mantissa is 0 width and we don't have subnormals -
+        essentially the mantissa is always decoded as 1.
+        If we have subnormals, the only subnormal is zero, and the mantissa is
+        always decoded as 0.
+        """
+        return self.precision > 1 or self.has_subnormals
+
+    @property
     def code_of_negzero(self) -> int:
         """
         Return a codepoint for negative zero
         """
         if not self.has_nz:
             raise ValueError(f"No negative zero in {self}")
 
         return 2 ** (self.k - 1)
 
     @property
     def code_of_max(self) -> int:
         """
         Return a codepoint for fi.max
         """
-        return 2 ** (self.k - 1) - self.num_high_nans - self.has_infs - 1
+        return 2 ** (self.k - self.signBits) - self.num_high_nans - self.has_infs - 1
 
     @property
     def code_of_min(self) -> int:
         """
-        Return a codepoint for fi.max
+        Return a codepoint for fi.min
         """
-        return 2**self.k - self.num_high_nans - self.has_infs - 1
+        if self.is_signed and not self.is_twos_complement:
+            return 2**self.k - self.num_high_nans - self.has_infs - 1
+        elif self.is_signed and self.is_twos_complement:
+            return 2 ** (self.k - 1)
+        else:
+            return 0  # codepoint of smallest value, whether 0 or 2^-expBias
 
     # @property
     # def minexp(self) -> int:
     #     """
     #     The most negative power of the base (2) consistent with there
     #     being no leading 0's in the mantissa.
     #     """
@@ -309,25 +357,48 @@
 
     # @property
     # def tiny(self) -> float:
     #     """
     #     An alias for `smallest_normal`, kept for backwards compatibility.
     #     """
 
-    # @property
-    # def smallest_normal(self) -> float:
-    #     """
-    #     The smallest positive floating point number with 1 as leading bit in
-    #     the mantissa following IEEE-754 (see Notes).
-    #     """
+    @property
+    def smallest_normal(self) -> float:
+        """
+        The smallest positive floating point number with 1 as leading bit in
+        the significand following IEEE-754.
+        """
+        if self.has_subnormals:
+            return 2 ** (1 - self.expBias)
+        elif self.has_zero:
+            return 2**-self.expBias + 2 ** (-self.expBias - self.tSignificandBits)
+        else:
+            return 2**-self.expBias
 
     @property
     def smallest_subnormal(self) -> float:
         """
         The smallest positive floating point number with 0 as leading bit in
-        the mantissa following IEEE-754.
+        the significand following IEEE-754.
         """
         assert self.has_subnormals, "not implemented"
         return 2 ** -(self.expBias + self.tSignificandBits - 1)
 
-    def __str__(self):
+    @property
+    def smallest(self) -> float:
+        """
+        The smallest positive floating point number.
+        """
+        if self.has_subnormals:
+            return self.smallest_subnormal
+        else:
+            return self.smallest_normal
+
+    @property
+    def is_all_subnormal(self) -> bool:
+        """
+        Are all encoded values subnormal?
+        """
+        return (self.expBits == 0) and self.has_subnormals
+
+    def __str__(self) -> str:
         return f"{self.name}"
```

### Comparing `gfloat-0.0.5/test/test_encode.py` & `gfloat-0.1/test/test_encode.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 # Copyright (c) 2024 Graphcore Ltd. All rights reserved.
 
-import pytest
 import ml_dtypes
 import numpy as np
+import pytest
 
 from gfloat import decode_float, encode_float
 from gfloat.formats import *
 
 
 @pytest.mark.parametrize("fi", all_formats, ids=str)
-def test_encode(fi):
+def test_encode(fi: FormatInfo) -> None:
     dec = lambda v: decode_float(fi, v).fval
 
     if fi.bits <= 8:
         step = 1
     elif fi.bits <= 16:
         step = 13
     elif fi.bits <= 32:
         step = 73013
 
     for i in range(0, 2**fi.bits, step):
         fv = decode_float(fi, i)
         ival = encode_float(fi, fv.fval)
-        fv2 = decode_float(fi, ival)
         assert (i == ival) or np.isnan(fv.fval)
+        fv2 = decode_float(fi, ival)
         np.testing.assert_equal(fv2.fval, fv.fval)
+
+
+@pytest.mark.parametrize("fi", all_formats, ids=str)
+def test_encode_edges(fi: FormatInfo) -> None:
+    assert encode_float(fi, fi.max) == fi.code_of_max
+
+    assert encode_float(fi, fi.max * 1.25) == (
+        fi.code_of_posinf
+        if fi.has_infs
+        else fi.code_of_nan if fi.num_nans > 0 else fi.code_of_max
+    )
+
+    if fi.is_signed:
+        assert encode_float(fi, fi.min * 1.25) == (
+            fi.code_of_neginf
+            if fi.has_infs
+            else fi.code_of_nan if fi.num_nans > 0 else fi.code_of_min
+        )
```

### Comparing `gfloat-0.0.5/test/test_finfo.py` & `gfloat-0.1/test/test_finfo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Copyright (c) 2024 Graphcore Ltd. All rights reserved.
 
 # Test that finfo methods on FloatFormat agree with numpy/ml_dtypes
 
-import pytest
 import ml_dtypes
 import numpy as np
+import pytest
 
 from gfloat import decode_float, round_float
 from gfloat.formats import *
 
 
 @pytest.mark.parametrize(
     "fmt,npfmt",
     [
         (format_info_ocp_e5m2, ml_dtypes.float8_e5m2),
         (format_info_ocp_e4m3, ml_dtypes.float8_e4m3fn),
         (format_info_binary16, np.float16),
         (format_info_bfloat16, ml_dtypes.bfloat16),
     ],
 )
-def test_finfo(fmt, npfmt):
+def test_finfo(fmt: FormatInfo, npfmt: np.dtype) -> None:
     assert fmt.eps == ml_dtypes.finfo(npfmt).eps
     assert fmt.epsneg == ml_dtypes.finfo(npfmt).epsneg
     assert fmt.max == ml_dtypes.finfo(npfmt).max
     assert fmt.maxexp == ml_dtypes.finfo(npfmt).maxexp
 
 
-def test_constants():
+def test_constants() -> None:
     assert format_info_p3109(1).smallest_subnormal == 2.0**-62
     assert format_info_p3109(4).smallest_subnormal == 2.0**-10
     assert format_info_p3109(7).smallest_subnormal == 2.0**-6
```

### Comparing `gfloat-0.0.5/test/test_round.py` & `gfloat-0.1/test/test_round.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # Copyright (c) 2024 Graphcore Ltd. All rights reserved.
 
-import pytest
+from typing import Type
+
 import ml_dtypes
 import numpy as np
+import pytest
 
-from gfloat import decode_float, round_float, RoundMode
+from gfloat import RoundMode, decode_float, round_float
 from gfloat.formats import *
 
 
-def _mlround(v, dty):
+def _mlround(v: float, dty: Type) -> float:
     """
     Round `v` using ml_dtypes library
     """
     return np.array([v]).astype(dty).astype(float).item()
 
 
-def test_round_p3109():
+def test_round_p3109() -> None:
     fi = format_info_p3109(4)
     assert round_float(fi, 0.0068359375) == 0.0068359375
     assert round_float(fi, 0.0029296875) == 0.0029296875
     assert round_float(fi, 0.0078125) == 0.0078125
     assert round_float(fi, 0.017578125) == 0.017578125
     assert round_float(fi, 224.0) == 224.0
     assert round_float(fi, 240.0) == np.inf
@@ -37,15 +39,15 @@
     assert round_float(fi, -232.0, RoundMode.TowardZero) == -224.0
     assert round_float(fi, -232.0, RoundMode.TowardNegative) == -np.inf
     assert round_float(fi, -232.0, RoundMode.TowardPositive) == -224.0
 
     assert round_float(fi, 232.1) == np.inf
 
 
-def test_round_e5m2():
+def test_round_e5m2() -> None:
     fi = format_info_ocp_e5m2
 
     assert fi.max == 57344
 
     assert round_float(fi, 1.5258789e-05) == 2**-16
 
     # Default NONSAT rounding
@@ -63,15 +65,15 @@
     assert round_float(fi, 61439.9, sat=True) == 57344
     assert round_float(fi, 61440.0, sat=True) == 57344
     assert round_float(fi, np.inf, sat=True) == 57344
     assert round_float(fi, -np.inf, sat=True) == -57344
     assert np.isnan(round_float(fi, np.nan, sat=True))
 
 
-def test_round_e4m3():
+def test_round_e4m3() -> None:
     fi = format_info_ocp_e4m3
 
     assert fi.max == 448
 
     # Default NONSAT rounding
     assert round_float(fi, 448.0) == 448
     assert round_float(fi, 448.1) == 448
@@ -113,15 +115,15 @@
     [
         format_info_ocp_e5m2,
         format_info_ocp_e4m3,
         *p3109_formats,
     ],
     ids=str,
 )
-def test_round(fi):
+def test_round(fi: FormatInfo) -> None:
     """
     Test rounding from values between exact binary8 values
     For integer code point i, let
       v0 = the float value at i
       v1 = the float value at i+1, i.e. nextUp(v0)
       dv = v1 - v0
     Then check that:
@@ -145,37 +147,53 @@
 
 test_formats = [
     (format_info_ocp_e5m2, ml_dtypes.float8_e5m2),
     (format_info_ocp_e4m3, ml_dtypes.float8_e4m3fn),
 ]
 
 
-def _linterp(a, b, t):
+def _linterp(a: float, b: float, t: float) -> float:
     return a * (1 - t) + b * t
 
 
 @pytest.mark.parametrize("fi,mldtype", test_formats)
-def test_ml_dtype_compatible(fi, mldtype):
+def test_ml_dtype_compatible(fi: FormatInfo, mldtype: Type) -> None:
     """
     Test that rounding is compatible with ml_dtypes, assuming IEEE-like rounding
     """
     for i in range(255):
+        # For each float v, check values at various interpolations
+        # between v and nextUp(v)
         v0 = decode_float(fi, i + 0).fval
         v1 = decode_float(fi, i + 1).fval
 
-        for alpha in np.arange(0, 1.3, 0.3):
+        for alpha in (0, 0.3, 0.5, 0.6, 0.9, 1.25):
             v = _linterp(v0, v1, alpha)
             if np.isfinite(v):
-                print(i)
                 val = round_float(fi, v, RoundMode.TiesToEven)
 
                 mlval = _mlround(v, mldtype)
                 np.testing.assert_equal(val, mlval)
 
 
 @pytest.mark.parametrize("fi,mldtype", test_formats)
-def test_round_ints(fi, mldtype):
+def test_round_ints(fi: FormatInfo, mldtype: Type) -> None:
     for v in np.arange(289).astype(float):
         val = round_float(fi, v)
 
         mlval = _mlround(v, mldtype)
         np.testing.assert_equal(val, mlval)
+
+
+@pytest.mark.parametrize("fi", all_formats, ids=str)
+def test_round_roundtrip(fi: FormatInfo) -> None:
+    if fi.bits <= 8:
+        step = 1
+    elif fi.bits <= 16:
+        step = 13
+    elif fi.bits <= 32:
+        step = 73013
+
+    for i in range(0, 2**fi.bits, step):
+        fv = decode_float(fi, i)
+        fval2 = round_float(fi, fv.fval)
+        np.testing.assert_equal(fval2, fv.fval)
```

