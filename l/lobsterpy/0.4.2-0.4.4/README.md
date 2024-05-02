# Comparing `tmp/lobsterpy-0.4.2.tar.gz` & `tmp/lobsterpy-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lobsterpy-0.4.2.tar", last modified: Sun Apr 21 16:54:03 2024, max compression
+gzip compressed data, was "lobsterpy-0.4.4.tar", last modified: Thu May  2 17:42:30 2024, max compression
```

## Comparing `lobsterpy-0.4.2.tar` & `lobsterpy-0.4.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:54:03.953918 lobsterpy-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-04-21 16:54:03.953918 lobsterpy-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:54:03.945918 lobsterpy-0.4.2/lobsterpy/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42439 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:54:03.949918 lobsterpy-0.4.2/lobsterpy/cohp/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/cohp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    78180 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/cohp/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)    37915 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/cohp/describe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:54:03.949918 lobsterpy-0.4.2/lobsterpy/featurize/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/featurize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32633 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/featurize/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    47979 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/featurize/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/featurize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:54:03.949918 lobsterpy-0.4.2/lobsterpy/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)    47583 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/plotting/layout_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/plotting/lobsterpy_base.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:54:03.949918 lobsterpy-0.4.2/lobsterpy/structuregraph/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/structuregraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/lobsterpy/structuregraph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:54:03.949918 lobsterpy-0.4.2/lobsterpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-04-21 16:54:03.000000 lobsterpy-0.4.2/lobsterpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-21 16:54:03.000000 lobsterpy-0.4.2/lobsterpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:54:03.000000 lobsterpy-0.4.2/lobsterpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-21 16:54:03.000000 lobsterpy-0.4.2/lobsterpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-21 16:54:03.000000 lobsterpy-0.4.2/lobsterpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 16:54:03.000000 lobsterpy-0.4.2/lobsterpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-21 16:53:10.000000 lobsterpy-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 16:54:03.953918 lobsterpy-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:42:30.462421 lobsterpy-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-05-02 17:42:30.458421 lobsterpy-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:42:30.454420 lobsterpy-0.4.4/lobsterpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42439 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:42:30.454420 lobsterpy-0.4.4/lobsterpy/cohp/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/cohp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78180 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/cohp/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37915 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/cohp/describe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:42:30.458421 lobsterpy-0.4.4/lobsterpy/featurize/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/featurize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32633 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/featurize/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47979 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/featurize/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/featurize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:42:30.458421 lobsterpy-0.4.4/lobsterpy/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)    47538 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/plotting/layout_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/plotting/lobsterpy_base.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:42:30.458421 lobsterpy-0.4.4/lobsterpy/structuregraph/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/structuregraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/lobsterpy/structuregraph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:42:30.458421 lobsterpy-0.4.4/lobsterpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-05-02 17:42:30.000000 lobsterpy-0.4.4/lobsterpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-02 17:42:30.000000 lobsterpy-0.4.4/lobsterpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:42:30.000000 lobsterpy-0.4.4/lobsterpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 17:42:30.000000 lobsterpy-0.4.4/lobsterpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-02 17:42:30.000000 lobsterpy-0.4.4/lobsterpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 17:42:30.000000 lobsterpy-0.4.4/lobsterpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-02 17:41:24.000000 lobsterpy-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:42:30.462421 lobsterpy-0.4.4/setup.cfg
```

### Comparing `lobsterpy-0.4.2/LICENSE` & `lobsterpy-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.2/PKG-INFO` & `lobsterpy-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: lobsterpy
-Version: 0.4.2
+Version: 0.4.4
 Summary: Package for automatic bonding analysis with Lobster/VASP
 Author-email: Janine George <janine.george@bam.de>
 License: BSD 3-Clause
 Project-URL: homepage, https://jageo.github.io/LobsterPy/
 Project-URL: repository, https://github.com/JaGeo/LobsterPy
 Project-URL: documentation, https://jageo.github.io/LobsterPy/
 Project-URL: changelog, https://jageo.github.io/LobsterPy/about/changelog.html
 Keywords: high-throughput,automated,lobsteroutput,bonding-analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.12,>=3.9
+Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pymatgen>=2024.4.13
+Requires-Dist: pymatgen>=2024.5.1
 Requires-Dist: numpy
 Requires-Dist: typing
 Provides-Extra: featurizer
 Requires-Dist: mendeleev==0.15.0; extra == "featurizer"
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.12.1; extra == "dev"
 Provides-Extra: tests
 Requires-Dist: flake8; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: pytest-split; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
-Requires-Dist: sphinx<6,>=5; extra == "docs"
+Requires-Dist: sphinx<8,>=5; extra == "docs"
 Requires-Dist: sphinx_design==0.5.0; extra == "docs"
 Requires-Dist: myst-nb==1.1.0; extra == "docs"
 Requires-Dist: sphinx-book-theme==1.1.2; extra == "docs"
 Requires-Dist: sphinx-argparse==0.4.0; extra == "docs"
 Requires-Dist: sphinx-toolbox==3.5.0; extra == "docs"
 
 ![CI Status](https://github.com/JaGeo/LobsterPy/actions/workflows/python-package.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JaGeo/LobsterPy/main.svg)](https://results.pre-commit.ci/latest/github/JaGeo/LobsterPy/main) [![codecov](https://codecov.io/gh/JaGeo/LobsterPy/graph/badge.svg?token=MC5BRXVEGW)](https://codecov.io/gh/JaGeo/LobsterPy) [![build-docs](https://github.com/JaGeo/LobsterPy/actions/workflows/docs.yml/badge.svg)](https://jageo.github.io/LobsterPy/) [![PyPI version](https://badge.fury.io/py/lobsterpy.svg)](https://badge.fury.io/py/lobsterpy) [![PyPI downloads](https://img.shields.io/pypi/dm/lobsterpy?style=flat&color=blue&label=pypi%20downloads)](https://pypi.org/project/lobsterpy) [![Downloads](https://pepy.tech/badge/lobsterpy)](https://pepy.tech/project/lobsterpy) ![supported python versions](https://img.shields.io/pypi/pyversions/lobsterpy) [![DOI](https://zenodo.org/badge/343384088.svg)](https://zenodo.org/badge/latestdoi/343384088) [![status](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2/status.svg)](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2)
```

### Comparing `lobsterpy-0.4.2/README.md` & `lobsterpy-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.2/lobsterpy/cli.py` & `lobsterpy-0.4.4/lobsterpy/cli.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.2/lobsterpy/cohp/analyze.py` & `lobsterpy-0.4.4/lobsterpy/cohp/analyze.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.2/lobsterpy/cohp/describe.py` & `lobsterpy-0.4.4/lobsterpy/cohp/describe.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.2/lobsterpy/featurize/batch.py` & `lobsterpy-0.4.4/lobsterpy/featurize/batch.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.2/lobsterpy/featurize/core.py` & `lobsterpy-0.4.4/lobsterpy/featurize/core.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.2/lobsterpy/featurize/utils.py` & `lobsterpy-0.4.4/lobsterpy/featurize/utils.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.2/lobsterpy/plotting/__init__.py` & `lobsterpy-0.4.4/lobsterpy/plotting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,33 +3,31 @@
 
 """Here classes and functions to plot Lobster outputs are provided."""
 
 from __future__ import annotations
 
 import typing
 from itertools import cycle
+from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import matplotlib as mpl
 import numpy as np
 import plotly.graph_objs as go
 from matplotlib import pyplot as plt
-from pkg_resources import resource_filename
 from pymatgen.core import Structure
 from pymatgen.electronic_structure.cohp import Cohp, CompleteCohp, IcohpCollection
 from pymatgen.electronic_structure.core import Spin
 from pymatgen.electronic_structure.dos import LobsterCompleteDos
 from pymatgen.electronic_structure.plotter import CohpPlotter, DosPlotter
 
 if TYPE_CHECKING:
     from lobsterpy.cohp.analyze import Analysis
 from lobsterpy.plotting import layout_dicts as ld
 
-base_style = resource_filename("lobsterpy.plotting", "lobsterpy_base.mplstyle")
-
 
 def get_style_list(
     no_base_style: bool = False,
     styles: list[str | dict[str, Any]] | None = None,
     **kwargs,
 ) -> list[str | dict[str, Any]]:
     """
@@ -39,15 +37,15 @@
 
     :param no_base_style: If true, do not include lobsterpy_base.mplstyle
     :param styles: User-requested styles. These can be paths to mplstyle files,
         the names of known (matplotlib-supplied) styles, or dicts of rcParam options.
     :param kwargs: matplotlib-style sheet keyword arguments
 
     """
-    base = [] if no_base_style else [base_style]
+    base = [] if no_base_style else [str(Path(__file__).absolute().parent / "lobsterpy_base.mplstyle")]
     if styles is None:
         styles = []
 
     return base + styles + [kwargs]
 
 
 class PlainCohpPlotter(CohpPlotter):
```

### Comparing `lobsterpy-0.4.2/lobsterpy/plotting/layout_dicts.py` & `lobsterpy-0.4.4/lobsterpy/plotting/layout_dicts.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.2/lobsterpy/structuregraph/graph.py` & `lobsterpy-0.4.4/lobsterpy/structuregraph/graph.py`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.2/lobsterpy.egg-info/PKG-INFO` & `lobsterpy-0.4.4/lobsterpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: lobsterpy
-Version: 0.4.2
+Version: 0.4.4
 Summary: Package for automatic bonding analysis with Lobster/VASP
 Author-email: Janine George <janine.george@bam.de>
 License: BSD 3-Clause
 Project-URL: homepage, https://jageo.github.io/LobsterPy/
 Project-URL: repository, https://github.com/JaGeo/LobsterPy
 Project-URL: documentation, https://jageo.github.io/LobsterPy/
 Project-URL: changelog, https://jageo.github.io/LobsterPy/about/changelog.html
 Keywords: high-throughput,automated,lobsteroutput,bonding-analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.12,>=3.9
+Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pymatgen>=2024.4.13
+Requires-Dist: pymatgen>=2024.5.1
 Requires-Dist: numpy
 Requires-Dist: typing
 Provides-Extra: featurizer
 Requires-Dist: mendeleev==0.15.0; extra == "featurizer"
 Provides-Extra: dev
 Requires-Dist: pre-commit>=2.12.1; extra == "dev"
 Provides-Extra: tests
 Requires-Dist: flake8; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: pytest-split; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
-Requires-Dist: sphinx<6,>=5; extra == "docs"
+Requires-Dist: sphinx<8,>=5; extra == "docs"
 Requires-Dist: sphinx_design==0.5.0; extra == "docs"
 Requires-Dist: myst-nb==1.1.0; extra == "docs"
 Requires-Dist: sphinx-book-theme==1.1.2; extra == "docs"
 Requires-Dist: sphinx-argparse==0.4.0; extra == "docs"
 Requires-Dist: sphinx-toolbox==3.5.0; extra == "docs"
 
 ![CI Status](https://github.com/JaGeo/LobsterPy/actions/workflows/python-package.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JaGeo/LobsterPy/main.svg)](https://results.pre-commit.ci/latest/github/JaGeo/LobsterPy/main) [![codecov](https://codecov.io/gh/JaGeo/LobsterPy/graph/badge.svg?token=MC5BRXVEGW)](https://codecov.io/gh/JaGeo/LobsterPy) [![build-docs](https://github.com/JaGeo/LobsterPy/actions/workflows/docs.yml/badge.svg)](https://jageo.github.io/LobsterPy/) [![PyPI version](https://badge.fury.io/py/lobsterpy.svg)](https://badge.fury.io/py/lobsterpy) [![PyPI downloads](https://img.shields.io/pypi/dm/lobsterpy?style=flat&color=blue&label=pypi%20downloads)](https://pypi.org/project/lobsterpy) [![Downloads](https://pepy.tech/badge/lobsterpy)](https://pepy.tech/project/lobsterpy) ![supported python versions](https://img.shields.io/pypi/pyversions/lobsterpy) [![DOI](https://zenodo.org/badge/343384088.svg)](https://zenodo.org/badge/latestdoi/343384088) [![status](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2/status.svg)](https://joss.theoj.org/papers/4e8524125e36486c65a4b435bbfe2df2)
```

### Comparing `lobsterpy-0.4.2/lobsterpy.egg-info/SOURCES.txt` & `lobsterpy-0.4.4/lobsterpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lobsterpy-0.4.2/pyproject.toml` & `lobsterpy-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 [project]
 name = "lobsterpy"
 description = "Package for automatic bonding analysis with Lobster/VASP"
 readme = "README.md"
 keywords = ["high-throughput", "automated", "lobsteroutput", "bonding-analysis"]
 license = { text = "BSD 3-Clause" }
 authors = [{ name = "Janine George", email = "janine.george@bam.de" }]
-version = "0.4.2"
+version = "0.4.4"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
 ]
-requires-python = ">=3.9,<3.12"
+requires-python = ">=3.9,<3.13"
 dependencies = [
-     "pymatgen>=2024.4.13",
+     "pymatgen>=2024.5.1",
      "numpy",
      "typing",
 ]
 
 [tool.setuptools.package-data]
 "lobsterpy.plotting" = ["lobsterpy_base.mplstyle"]
 
@@ -44,15 +45,15 @@
 
 [project.optional-dependencies]
 featurizer = ["mendeleev==0.15.0"]
 dev = ["pre-commit>=2.12.1"]
 tests = ["flake8", "pytest", "pytest-mock", "pytest-split", "pytest-cov"]
 docs = [
     "sphinx-copybutton==0.5.2",
-    "sphinx>=5,<6",
+    "sphinx>=5,<8",
     "sphinx_design==0.5.0",
     "myst-nb==1.1.0",
     "sphinx-book-theme==1.1.2",
     "sphinx-argparse==0.4.0",
     "sphinx-toolbox==3.5.0",
 ]
```

