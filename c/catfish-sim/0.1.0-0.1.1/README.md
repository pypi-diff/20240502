# Comparing `tmp/catfish_sim-0.1.0.tar.gz` & `tmp/catfish_sim-0.1.1.tar.gz`

## Comparing `catfish_sim-0.1.0.tar` & `catfish_sim-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/make.bat
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/requirements-dev.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/catfish_sim/__init__.py
--rw-r--r--   0        0        0     9937 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/catfish_sim/agents.py
--rw-r--r--   0        0        0    12657 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/catfish_sim/compatibility.py
--rw-r--r--   0        0        0    32357 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/catfish_sim/matchers.py
--rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/catfish_sim/strategies.py
--rw-r--r--   0        0        0    15996 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/catfish_sim/utils.py
--rw-r--r--   0        0        0  6555719 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/catfish_sim/data/LLCP2022_sex_age_height_bmi.csv
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/tests/test_dealbreaker.py
--rw-r--r--   0        0        0    10393 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/tests/test_misrepresentation.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/tests/test_recommendation_priority_order.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/.gitignore
--rw-r--r--   0        0        0    35822 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/LICENSE
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/README.md
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    45862 2020-02-02 00:00:00.000000 catfish_sim-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/readthedocs.yaml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/requirements-dev.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/catfish_sim/__init__.py
+-rw-r--r--   0        0        0     9937 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/catfish_sim/agents.py
+-rw-r--r--   0        0        0    12657 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/catfish_sim/compatibility.py
+-rw-r--r--   0        0        0    32357 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/catfish_sim/matchers.py
+-rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/catfish_sim/strategies.py
+-rw-r--r--   0        0        0    15996 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/catfish_sim/utils.py
+-rw-r--r--   0        0        0  6555719 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/catfish_sim/data/LLCP2022_sex_age_height_bmi.csv
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/docs/catfish_sim.rst
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/docs/modules.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/tests/test_dealbreaker.py
+-rw-r--r--   0        0        0    10393 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/tests/test_misrepresentation.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/tests/test_recommendation_priority_order.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35822 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/README.md
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    45872 2020-02-02 00:00:00.000000 catfish_sim-0.1.1/PKG-INFO
```

### Comparing `catfish_sim-0.1.0/CHANGELOG.md` & `catfish_sim-0.1.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/Makefile` & `catfish_sim-0.1.1/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?=
 SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = source
-BUILDDIR      = build
+SOURCEDIR     = .
+BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
```

### Comparing `catfish_sim-0.1.0/make.bat` & `catfish_sim-0.1.1/docs/make.bat`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 pushd %~dp0
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
-set SOURCEDIR=source
-set BUILDDIR=build
+set SOURCEDIR=.
+set BUILDDIR=_build
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
```

### Comparing `catfish_sim-0.1.0/catfish_sim/agents.py` & `catfish_sim-0.1.1/catfish_sim/agents.py`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/catfish_sim/compatibility.py` & `catfish_sim-0.1.1/catfish_sim/compatibility.py`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/catfish_sim/matchers.py` & `catfish_sim-0.1.1/catfish_sim/matchers.py`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/catfish_sim/strategies.py` & `catfish_sim-0.1.1/catfish_sim/strategies.py`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/catfish_sim/utils.py` & `catfish_sim-0.1.1/catfish_sim/utils.py`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/catfish_sim/data/LLCP2022_sex_age_height_bmi.csv` & `catfish_sim-0.1.1/catfish_sim/data/LLCP2022_sex_age_height_bmi.csv`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/docs/source/conf.py` & `catfish_sim-0.1.1/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,27 +2,37 @@
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
-project = 'catfish-sim'
-copyright = '2024, Oz Kilic'
-author = 'Oz Kilic'
-release = '0.1.0'
+import os
+import sys
+
+sys.path.insert(0, os.path.abspath(".."))
+
+project = "catfish-sim"
+copyright = "2024, Oz Kilic"
+author = "Oz Kilic"
+release = "0.1.1"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
-extensions = []
-
-templates_path = ['_templates']
-exclude_patterns = []
+extensions = [
+    "sphinx.ext.napoleon",
+    "sphinx_rtd_theme",
+    "sphinx.ext.todo",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.autodoc",
+]
 
+templates_path = ["_templates"]
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
-html_theme = 'alabaster'
-html_static_path = ['_static']
+html_theme = "sphinx_rtd_theme"
+html_static_path = ["_static"]
```

### Comparing `catfish_sim-0.1.0/tests/test_dealbreaker.py` & `catfish_sim-0.1.1/tests/test_dealbreaker.py`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/tests/test_misrepresentation.py` & `catfish_sim-0.1.1/tests/test_misrepresentation.py`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/tests/test_recommendation_priority_order.py` & `catfish_sim-0.1.1/tests/test_recommendation_priority_order.py`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/.gitignore` & `catfish_sim-0.1.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
-docs/build/
 
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `catfish_sim-0.1.0/LICENSE` & `catfish_sim-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/README.md` & `catfish_sim-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `catfish_sim-0.1.0/pyproject.toml` & `catfish_sim-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "catfish-sim"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Oz Kilic", email = "ozgunozankilic@gmail.com" }]
 description = "A multiagent online dating simulation framework."
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">= 3.6"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -47,8 +47,8 @@
 [project.optional-dependencies]
 dev = ["pytest >= 7.4.3"]
 
 [project.urls]
 Homepage = "https://github.com/ozgunozankilic/catfish-sim"
 Repository = "https://github.com/ozgunozankilic/catfish-sim"
 Issues = "https://github.com/ozgunozankilic/catfish-sim/issues"
-Changelog = "https://github.com/ozgunozankilic/catfish-sim/CHANGELOG.md"
+Changelog = "https://github.com/ozgunozankilic/catfish-sim/blob/main/CHANGELOG.md"
```

### Comparing `catfish_sim-0.1.0/PKG-INFO` & `catfish_sim-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: catfish-sim
-Version: 0.1.0
+Version: 0.1.1
 Summary: A multiagent online dating simulation framework.
 Project-URL: Homepage, https://github.com/ozgunozankilic/catfish-sim
 Project-URL: Repository, https://github.com/ozgunozankilic/catfish-sim
 Project-URL: Issues, https://github.com/ozgunozankilic/catfish-sim/issues
-Project-URL: Changelog, https://github.com/ozgunozankilic/catfish-sim/CHANGELOG.md
+Project-URL: Changelog, https://github.com/ozgunozankilic/catfish-sim/blob/main/CHANGELOG.md
 Author-email: Oz Kilic <ozgunozankilic@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

