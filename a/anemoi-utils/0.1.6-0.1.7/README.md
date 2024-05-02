# Comparing `tmp/anemoi_utils-0.1.6.tar.gz` & `tmp/anemoi_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi_utils-0.1.6.tar", last modified: Mon Apr 29 14:02:27 2024, max compression
+gzip compressed data, was "anemoi_utils-0.1.7.tar", last modified: Thu May  2 12:29:13 2024, max compression
```

## Comparing `anemoi_utils-0.1.6.tar` & `anemoi_utils-0.1.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.863407 anemoi_utils-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.851407 anemoi_utils-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.855407 anemoi_utils-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-04-29 14:02:27.863407 anemoi_utils-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.855407 anemoi_utils-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.855407 anemoi_utils-0.1.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.855407 anemoi_utils-0.1.6/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/installing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.855407 anemoi_utils-0.1.6/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/checkpoints.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/dates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/grib.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/humanize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/provenance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/text.rst
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:02:27.863407 anemoi_utils-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.851407 anemoi_utils-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.851407 anemoi_utils-0.1.6/src/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.859407 anemoi_utils-0.1.6/src/anemoi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi/utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/grib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.859407 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.859407 anemoi_utils-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.537678 anemoi_utils-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.525678 anemoi_utils-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.529678 anemoi_utils-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-05-02 12:29:13.537678 anemoi_utils-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.529678 anemoi_utils-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.529678 anemoi_utils-0.1.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.529678 anemoi_utils-0.1.7/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/installing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.529678 anemoi_utils-0.1.7/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/checkpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/dates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/humanize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/provenance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/modules/text.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 12:29:13.537678 anemoi_utils-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.525678 anemoi_utils-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.525678 anemoi_utils-0.1.7/src/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.533678 anemoi_utils-0.1.7/src/anemoi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi/utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/src/anemoi/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.533678 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 12:29:13.000000 anemoi_utils-0.1.7/src/anemoi_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:29:13.533678 anemoi_utils-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-02 12:28:51.000000 anemoi_utils-0.1.7/tests/test_utils.py
```

### Comparing `anemoi_utils-0.1.6/.github/workflows/python-publish.yml` & `anemoi_utils-0.1.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/.gitignore` & `anemoi_utils-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/.pre-commit-config.yaml` & `anemoi_utils-0.1.7/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -58,12 +58,12 @@
 
 # For now, we use it. But it does not support a lot of sphinx features
 - repo: https://github.com/dzhu/rstfmt
   rev: v0.0.14
   hooks:
     - id: rstfmt
 
-# - repo: ../pre-commit-docconvert
-#   rev: 07f5748
-#   hooks:
-#   - id: docconvert
-#     args: ["--in-place", "--output", "numpy"]
+- repo: https://github.com/b8raoult/pre-commit-docconvert
+  rev: "0.1.4"
+  hooks:
+  - id: docconvert
+    args: ["numpy"]
```

### Comparing `anemoi_utils-0.1.6/LICENSE` & `anemoi_utils-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/PKG-INFO` & `anemoi_utils-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `anemoi_utils-0.1.6/README.md` & `anemoi_utils-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/docs/Makefile` & `anemoi_utils-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/docs/_static/logo.png` & `anemoi_utils-0.1.7/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/docs/_static/style.css` & `anemoi_utils-0.1.7/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/docs/conf.py` & `anemoi_utils-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/docs/index.rst` & `anemoi_utils-0.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/docs/installing.rst` & `anemoi_utils-0.1.7/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/pyproject.toml` & `anemoi_utils-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/src/anemoi/utils/checkpoints.py` & `anemoi_utils-0.1.7/src/anemoi/utils/checkpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 #
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
-"""
-Read and write extra metadata in PyTorch checkpoints files. These files
+"""Read and write extra metadata in PyTorch checkpoints files. These files
 are zip archives containing the model weights.
 """
 
 import json
 import logging
 import os
 import zipfile
```

### Comparing `anemoi_utils-0.1.6/src/anemoi/utils/config.py` & `anemoi_utils-0.1.7/src/anemoi/utils/config.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/src/anemoi/utils/dates.py` & `anemoi_utils-0.1.7/src/anemoi/utils/dates.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/src/anemoi/utils/grib.py` & `anemoi_utils-0.1.7/src/anemoi/utils/grib.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,30 +7,38 @@
 
 """Utilities for working with GRIB parameters.
 
 See https://codes.ecmwf.int/grib/param-db/ for more information.
 
 """
 
+import logging
 import re
 
 import requests
 
+LOG = logging.getLogger(__name__)
+
 
 def _search(name):
     name = re.escape(name)
     r = requests.get(f"https://codes.ecmwf.int/parameter-database/api/v1/param/?search=^{name}$&regex=true")
     r.raise_for_status()
     results = r.json()
     if len(results) == 0:
         raise KeyError(name)
 
     if len(results) > 1:
         names = [f'{r.get("id")} ({r.get("name")})' for r in results]
-        raise ValueError(f"{name} is ambiguous: {', '.join(names)}")
+        dissemination = [r for r in results if "dissemination" in r.get("access_ids", [])]
+        if len(dissemination) == 1:
+            return dissemination[0]
+
+        results = sorted(results, key=lambda x: x["id"])
+        LOG.warning(f"{name} is ambiguous: {', '.join(names)}. Using param_id={results[0]['id']}")
 
     return results[0]
 
 
 def shortname_to_paramid(shortname: str) -> int:
     """Return the GRIB parameter id given its shortname.
 
@@ -40,15 +48,14 @@
         Parameter shortname.
 
     Returns
     -------
     int
         Parameter id.
 
-
     >>> shortname_to_paramid("2t")
     167
 
     """
     return _search(shortname)["id"]
 
 
@@ -61,13 +68,12 @@
         Parameter id.
 
     Returns
     -------
     str
         Parameter shortname.
 
-
     >>> paramid_to_shortname(167)
     '2t'
 
     """
     return _search(str(paramid))["shortname"]
```

### Comparing `anemoi_utils-0.1.6/src/anemoi/utils/humanize.py` & `anemoi_utils-0.1.7/src/anemoi/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/src/anemoi/utils/provenance.py` & `anemoi_utils-0.1.7/src/anemoi/utils/provenance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # (C) Copyright 2024 European Centre for Medium-Range Weather Forecasts.
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
-"""
-Collect information about the current environment, like:
+"""Collect information about the current environment, like:
 
  - The Python version
  - The versions of the modules which are currently loaded
  - The git information for the modules which are currently loaded from a git repository
  - ...
 
 """
@@ -211,15 +210,14 @@
         - a path to a directory
 
     Returns
     -------
     dict
         An object with the git information for the given arguments.
 
-
     >>> {
             "anemoi.utils": {
                 "sha1": "c999d83ae283bcbb99f68d92c42d24315922129f",
                 "remotes": [
                     "git@github.com:ecmwf/anemoi-utils.git"
                 ],
                 "modified_files": [
```

### Comparing `anemoi_utils-0.1.6/src/anemoi/utils/text.py` & `anemoi_utils-0.1.7/src/anemoi/utils/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # (C) Copyright 2024 European Centre for Medium-Range Weather Forecasts.
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
-"""
-Text utilities
-"""
+"""Text utilities"""
 
 import sys
 from collections import defaultdict
 
 # https://en.wikipedia.org/wiki/Box-drawing_character
 
 
@@ -54,17 +52,14 @@
         The maximum width of the box, by default 80
 
     Returns
     -------
     str
         A boxed version of the input text
 
-
-
-
     """
 
     lines = text.split("\n")
     width = max(len(_) for _ in lines)
 
     if min_width is not None:
         width = max(width, min_width)
@@ -262,15 +257,14 @@
     header : A list or tuple of strings
         The header of the table
     align : A list of '<', '>', or '^'
         To align the columns to the left, right, or center
     margin : int, optional
         Extra spaces on the left side of the table, by default 0
 
-
     Returns
     -------
     str
         A table as a string
     """
 
     def _(x):
@@ -335,11 +329,10 @@
         _description_, by default 80
 
     Returns
     -------
     str
         _description_
 
-
     """
     done = min(int(done / todo * width + 0.5), width)
     return green("█" * done) + red("█" * (width - done))
```

### Comparing `anemoi_utils-0.1.6/src/anemoi_utils.egg-info/PKG-INFO` & `anemoi_utils-0.1.7/src/anemoi_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `anemoi_utils-0.1.6/src/anemoi_utils.egg-info/SOURCES.txt` & `anemoi_utils-0.1.7/src/anemoi_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.1.6/tests/test_utils.py` & `anemoi_utils-0.1.7/tests/test_utils.py`

 * *Files identical despite different names*

