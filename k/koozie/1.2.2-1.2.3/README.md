# Comparing `tmp/koozie-1.2.2.tar.gz` & `tmp/koozie-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koozie-1.2.2.tar", max compression
+gzip compressed data, was "koozie-1.2.3.tar", max compression
```

## Comparing `koozie-1.2.2.tar` & `koozie-1.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1473 2024-02-23 05:54:03.577579 koozie-1.2.2/LICENSE.txt
--rw-r--r--   0        0        0     2644 2024-02-23 05:54:03.577579 koozie-1.2.2/README.md
--rw-r--r--   0        0        0       90 2024-02-23 05:54:03.577579 koozie-1.2.2/koozie/__init__.py
--rw-r--r--   0        0        0      176 2024-02-23 05:54:03.577579 koozie-1.2.2/koozie/__main__.py
--rw-r--r--   0        0        0     2281 2024-02-23 05:54:03.577579 koozie-1.2.2/koozie/cli.py
--rw-r--r--   0        0        0     5639 2024-02-23 05:54:03.577579 koozie-1.2.2/koozie/koozie.py
--rw-r--r--   0        0        0      826 2024-02-23 05:54:15.345682 koozie-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 koozie-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1473 2024-05-02 18:13:02.856766 koozie-1.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     2644 2024-05-02 18:13:02.856766 koozie-1.2.3/README.md
+-rw-r--r--   0        0        0       90 2024-05-02 18:13:02.856766 koozie-1.2.3/koozie/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-02 18:13:02.856766 koozie-1.2.3/koozie/__main__.py
+-rw-r--r--   0        0        0     2281 2024-05-02 18:13:02.856766 koozie-1.2.3/koozie/cli.py
+-rw-r--r--   0        0        0     4723 2024-05-02 18:13:02.856766 koozie-1.2.3/koozie/koozie.py
+-rw-r--r--   0        0        0      812 2024-05-02 18:13:17.304783 koozie-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 koozie-1.2.3/PKG-INFO
```

### Comparing `koozie-1.2.2/LICENSE.txt` & `koozie-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `koozie-1.2.2/README.md` & `koozie-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `koozie-1.2.2/koozie/cli.py` & `koozie-1.2.3/koozie/cli.py`

 * *Files identical despite different names*

### Comparing `koozie-1.2.2/koozie/koozie.py` & `koozie-1.2.3/koozie/koozie.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,19 @@
 """koozie functions"""
 
-import importlib.resources as pkg_resources
 from collections import OrderedDict
 from collections.abc import Iterable
 from typing import SupportsFloat
 from typing import List, Union  # Needed for python < 3.10
 
 import pint
 
-# Edit constants template to stop using h to represent planck_constant
-# See https://github.com/hgrecco/pint/issues/719#issuecomment-998872301
-# ---------------------------------------------------------------------
-constants_template = (
-    pkg_resources.read_text(pint, "constants_en.txt")
-    .replace("= h  ", "     ")
-    .replace(" h ", " planck_constant ")
-)
-
-# Edit units template to use h to represent hour instead of planck_constant
-units_template = (
-    pkg_resources.read_text(pint, "default_en.txt")
-    .replace("@import constants_en.txt", "")
-    .replace(" h ", " planck_constant ")
-    .replace("hour = 60 * minute = hr", "hour = 60 * minute = h = hr")
-)
-
-# Join templates as iterable object
-full_template = constants_template.split("\n") + units_template.split("\n")
-
 # Set up UnitRegistry with abbreviated scientific format
-unit_registry = pint.UnitRegistry(full_template)
+unit_registry = pint.UnitRegistry()
 unit_registry.default_format = "~P"  # short pretty
-# ---------------------------------------------------------------------
 
 # Add new aliases
 unit_registry.define("@alias inch_H2O_39F = in_H2O")
 unit_registry.define("@alias ton_of_refrigeration = ton_ref")
 unit_registry.define("@alias pound = lb_m")
 unit_registry.define("@alias force_pound = lb_f")
```

### Comparing `koozie-1.2.2/pyproject.toml` & `koozie-1.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [tool.poetry]
 name = "koozie"
-version = "v1.2.2" # Generated from git on CI
+version = "v1.2.3" # Generated from git on CI
 description = "A light-weight wrapper around pint for unit conversions."
 authors = ["Big Ladder Software"]
 license = "BSD-3"
 readme = "README.md"
 keywords = ["units"]
 repository = "https://github.com/bigladder/koozie"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pint = "^0.18"
+pint = "^0.21"
 click = "^8.1.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pylint = "*"
 black = "*"
 mypy = "*"
-# numpy = "*"
 
 [tool.poetry.scripts]
 koozie = "koozie.cli:koozie_cli"
 
 [tool.black]
-line-length = 100
+line-length = 120
 
 [tool.mypy]
 disallow_incomplete_defs = true
 no_implicit_optional = true
 check_untyped_defs = true
 
 [[tool.mypy.overrides]]
```

### Comparing `koozie-1.2.2/PKG-INFO` & `koozie-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: koozie
-Version: 1.2.2
+Version: 1.2.3
 Summary: A light-weight wrapper around pint for unit conversions.
 Home-page: https://github.com/bigladder/koozie
 License: BSD-3
 Keywords: units
 Author: Big Ladder Software
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: pint (>=0.18,<0.19)
+Requires-Dist: pint (>=0.21,<0.22)
 Project-URL: Repository, https://github.com/bigladder/koozie
 Description-Content-Type: text/markdown
 
 [![Release](https://img.shields.io/pypi/v/koozie.svg)](https://pypi.python.org/pypi/koozie)
 
 [![Test](https://github.com/bigladder/koozie/actions/workflows/test.yaml/badge.svg)](https://github.com/bigladder/koozie/actions/workflows/test.yaml)
```

