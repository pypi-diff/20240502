# Comparing `tmp/refers-0.0.3.tar.gz` & `tmp/refers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refers-0.0.3.tar", max compression
+gzip compressed data, was "refers-0.0.4.tar", max compression
```

## Comparing `refers-0.0.3.tar` & `refers-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1091 2024-03-14 10:04:59.833439 refers-0.0.3/LICENSE
--rw-r--r--   0        0        0     1999 2024-05-02 10:57:05.001145 refers-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1755 2024-03-14 10:04:59.835468 refers-0.0.3/README.md
--rw-r--r--   0        0        0       23 2024-03-14 10:04:59.865198 refers-0.0.3/refers/__init__.py
--rw-r--r--   0        0        0     1167 2024-03-14 10:49:12.324159 refers-0.0.3/refers/cli.py
--rw-r--r--   0        0        0    16043 2024-03-14 10:57:10.679511 refers-0.0.3/refers/compromise_black.py
--rw-r--r--   0        0        0      539 2024-03-14 10:04:59.867227 refers-0.0.3/refers/definitions.py
--rw-r--r--   0        0        0      464 2024-03-14 10:04:59.867227 refers-0.0.3/refers/errors.py
--rw-r--r--   0        0        0    13564 2024-03-14 10:57:52.884429 refers-0.0.3/refers/refers.py
--rw-r--r--   0        0        0     5644 2024-03-14 10:56:04.473042 refers-0.0.3/refers/tags.py
--rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 refers-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-03-14 10:04:59.833439 refers-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1999 2024-05-02 12:46:34.670746 refers-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2059 2024-05-02 11:12:19.176277 refers-0.0.4/README.md
+-rw-r--r--   0        0        0       23 2024-03-14 10:04:59.865198 refers-0.0.4/refers/__init__.py
+-rw-r--r--   0        0        0     1167 2024-03-14 10:49:12.324159 refers-0.0.4/refers/cli.py
+-rw-r--r--   0        0        0    16043 2024-03-14 10:57:10.679511 refers-0.0.4/refers/compromise_black.py
+-rw-r--r--   0        0        0      539 2024-03-14 10:04:59.867227 refers-0.0.4/refers/definitions.py
+-rw-r--r--   0        0        0      464 2024-03-14 10:04:59.867227 refers-0.0.4/refers/errors.py
+-rw-r--r--   0        0        0    13837 2024-05-02 12:34:47.584351 refers-0.0.4/refers/refers.py
+-rw-r--r--   0        0        0     5644 2024-03-14 10:56:04.473042 refers-0.0.4/refers/tags.py
+-rw-r--r--   0        0        0     2541 1970-01-01 00:00:00.000000 refers-0.0.4/PKG-INFO
```

### Comparing `refers-0.0.3/LICENSE` & `refers-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `refers-0.0.3/pyproject.toml` & `refers-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "refers"
-version = "0.0.3"
+version = "0.0.4"
 description = "Reference code to improve explainability"
 authors = ["Daniel Stoops <danielstoops25@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -47,15 +47,15 @@
 warn_unused_configs = true
 no_implicit_reexport = true
 
 [tool.pytest.ini_options]
 testpaths = "tests"
 addopts = [
     "--cov=refers",
-    "--cov-fail-under=75",
+    "--cov-fail-under=81",
     "--cov-report=term-missing",
     "--cov-report=term",
     "--cov-report="
 ]
 
 [tool.tox]
 legacy_tox_ini = """
```

### Comparing `refers-0.0.3/README.md` & `refers-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # refers
 *<p style="text-align: center;">reference code simply</p>*
 ![Tests](https://github.com/Stoops-ML/refers/actions/workflows/test.yml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/refers.svg)](https://badge.fury.io/py/refers)
 
 The refers library allows referencing plain text files from plain text files.
 
 Usage:
-1. Add a `@tag` to the line that you want to reference: `@tag:TAG_NAME`
-2. To reference the tag use `@ref` followed by an *optional* option: `@ref:TAG_NAME:OPTION`
+1. Add a `@tag` to the line that you want to reference: `@tag:NAME`
+2. To reference the tag use `@ref` followed by an *optional* option: `@ref:NAME:OPTION`
 3. run the refers library in the command line
 
 
 The refers library will create new files with the outputted references in place of the tags.
 Changes of line placement, file name, relative path etc. are reflected in the updated references when the refers library is executed.
 
-## Reference options
+## Installation
 
-| `ref` option  | result                               |
+`pip install refers`
+
+## Reference Options
+
+A reference has the following structure: `@ref:NAME:OPTION`. This will reference the named tag with the specified option. The available options are outlined in the table below.
+
+| Option        | Output                               |
 |---------------|--------------------------------------|
 | *blank*       | file name and line number            |
 | :file         | file name                            |
 | :line         | line number                          |
 | :link         | relative link to file                |
 | :linkline     | relative link to line in file        |
 | :fulllink     | full path link to file               |
```

### Comparing `refers-0.0.3/refers/cli.py` & `refers-0.0.4/refers/cli.py`

 * *Files identical despite different names*

### Comparing `refers-0.0.3/refers/compromise_black.py` & `refers-0.0.4/refers/compromise_black.py`

 * *Files identical despite different names*

### Comparing `refers-0.0.3/refers/definitions.py` & `refers-0.0.4/refers/definitions.py`

 * *Files identical despite different names*

### Comparing `refers-0.0.3/refers/refers.py` & `refers-0.0.4/refers/refers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import re
 from pathlib import Path
 from typing import List
 from typing import Optional
-from typing import (
-    TypeVar,
-)
+from typing import TypeVar
 from typing import Union
 
 import black
 import toml
 from black import nodes
 from black.parsing import lib2to3_parse
 from blib2to3.pytree import Leaf
@@ -236,58 +234,51 @@
         if not rootdir.is_absolute():
             rootdir = Path().cwd() / rootdir
 
     # pyproject. Inputs to function takes precedence
     pyproject_path = rootdir / "pyproject.toml"
     if pyproject_path.is_file():
         pyproject = toml.load(str(pyproject_path))
-        if LIBRARY_NAME not in pyproject["tool"].keys():
-            if "refers_path" in pyproject["tool"][LIBRARY_NAME].keys():
-                rootdir = Path(pyproject["tool"][LIBRARY_NAME]["refers_path"])
-            if "allow_not_found_tags" in pyproject["tool"][LIBRARY_NAME].keys():
+        if LIBRARY_NAME in pyproject["tool"].keys():
+            inputs_to_change = pyproject["tool"][LIBRARY_NAME].keys()
+            if "refers_path" in inputs_to_change:
+                rootdir_tmp = Path(pyproject["tool"][LIBRARY_NAME]["refers_path"])
+                if rootdir_tmp.exists():
+                    rootdir = rootdir_tmp
+                else:  # refers_path is defined in relation to pyproject_path
+                    rootdir = rootdir / rootdir_tmp
+            if "allow_not_found_tags" in inputs_to_change:
                 allow_not_found_tags = pyproject["tool"][LIBRARY_NAME][
                     "allow_not_found_tags"
                 ]
-            if (
-                "dirs2ignore" in pyproject["tool"][LIBRARY_NAME].keys()
-                and dirs2ignore is None
-            ):
+            if "dirs2ignore" in inputs_to_change and dirs2ignore is None:
                 dirs2ignore = [
                     Path(f) for f in pyproject["tool"][LIBRARY_NAME]["dirs2ignore"]
                 ]
-            if (
-                "dirs2search" in pyproject["tool"][LIBRARY_NAME].keys()
-                and dirs2search is None
-            ):
+            if "dirs2search" in inputs_to_change and dirs2search is None:
                 dirs2search = [
                     Path(f) for f in pyproject["tool"][LIBRARY_NAME]["dirs2search"]
                 ]
-            if (
-                "ref_files" in pyproject["tool"][LIBRARY_NAME].keys()
-                and ref_files is None
-            ):
+            if "ref_files" in inputs_to_change and ref_files is None:
                 ref_files = [
                     Path(f) for f in pyproject["tool"][LIBRARY_NAME]["ref_files"]
                 ]
-            if (
-                "tag_files" in pyproject["tool"][LIBRARY_NAME].keys()
-                and tag_files is None
-            ):
+            if "tag_files" in inputs_to_change and tag_files is None:
                 tag_files = [
                     Path(f) for f in pyproject["tool"][LIBRARY_NAME]["tag_files"]
                 ]
             if (
-                "accepted_tag_extensions" in pyproject["tool"][LIBRARY_NAME].keys()
+                "accepted_tag_extensions" in inputs_to_change
                 and accepted_tag_extensions is None
             ):
                 accepted_tag_extensions = pyproject["tool"][LIBRARY_NAME][
-                    "accepted_mime_tag_types"
+                    "accepted_tag_extensions"
                 ]
             if (
-                "accepted_ref_extensions" in pyproject["tool"][LIBRARY_NAME].keys()
+                "accepted_ref_extensions" in inputs_to_change
                 and accepted_ref_extensions is None
             ):
                 accepted_ref_extensions = pyproject["tool"][LIBRARY_NAME][
                     "accepted_ref_extensions"
                 ]
 
     # inputs (overrides pyproject)
@@ -350,14 +341,24 @@
     if isinstance(tag_files, str):
         tag_files = [Path(tag_files)]
     elif isinstance(tag_files, list) and isinstance(tag_files[0], str):
         tag_files = [Path(f) for f in tag_files]
     else:
         tag_files = None
 
+    # checks
+    if not rootdir.exists():
+        raise ValueError(f"The root directory does not exist: {rootdir}.")
+    if dirs2search is not None:
+        for d in dirs2search:
+            if not d.exists():
+                raise ValueError(
+                    f"The following directory which was requested to be searched does not exist: {d}."
+                )
+
     # get tags
     tags = get_tags(
         rootdir, accepted_tag_extensions, dirs2search, dirs2ignore, tag_files
     )
 
     # output document
     replace_tags(
```

### Comparing `refers-0.0.3/refers/tags.py` & `refers-0.0.4/refers/tags.py`

 * *Files identical despite different names*

### Comparing `refers-0.0.3/PKG-INFO` & `refers-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refers
-Version: 0.0.3
+Version: 0.0.4
 Summary: Reference code to improve explainability
 License: MIT
 Author: Daniel Stoops
 Author-email: danielstoops25@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,29 +13,36 @@
 Requires-Dist: black (>=24.2.0,<25.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # refers
 *<p style="text-align: center;">reference code simply</p>*
 ![Tests](https://github.com/Stoops-ML/refers/actions/workflows/test.yml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/refers.svg)](https://badge.fury.io/py/refers)
 
 The refers library allows referencing plain text files from plain text files.
 
 Usage:
-1. Add a `@tag` to the line that you want to reference: `@tag:TAG_NAME`
-2. To reference the tag use `@ref` followed by an *optional* option: `@ref:TAG_NAME:OPTION`
+1. Add a `@tag` to the line that you want to reference: `@tag:NAME`
+2. To reference the tag use `@ref` followed by an *optional* option: `@ref:NAME:OPTION`
 3. run the refers library in the command line
 
 
 The refers library will create new files with the outputted references in place of the tags.
 Changes of line placement, file name, relative path etc. are reflected in the updated references when the refers library is executed.
 
-## Reference options
+## Installation
 
-| `ref` option  | result                               |
+`pip install refers`
+
+## Reference Options
+
+A reference has the following structure: `@ref:NAME:OPTION`. This will reference the named tag with the specified option. The available options are outlined in the table below.
+
+| Option        | Output                               |
 |---------------|--------------------------------------|
 | *blank*       | file name and line number            |
 | :file         | file name                            |
 | :line         | line number                          |
 | :link         | relative link to file                |
 | :linkline     | relative link to line in file        |
 | :fulllink     | full path link to file               |
```

