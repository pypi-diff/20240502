# Comparing `tmp/njab-0.0.4.tar.gz` & `tmp/njab-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "njab-0.0.4.tar", last modified: Fri Feb 23 08:56:54 2024, max compression
+gzip compressed data, was "njab-0.0.5.tar", last modified: Thu May  2 14:22:22 2024, max compression
```

## Comparing `njab-0.0.4.tar` & `njab-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:56:54.026195 njab-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-23 08:56:46.000000 njab-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-02-23 08:56:54.026195 njab-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-02-23 08:56:46.000000 njab-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-23 08:56:46.000000 njab-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-02-23 08:56:54.026195 njab-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-23 08:56:46.000000 njab-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:56:54.018195 njab-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:56:54.018195 njab-0.0.4/src/njab/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:56:54.018195 njab-0.0.4/src/njab/io/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:56:54.022194 njab-0.0.4/src/njab/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/pandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:56:54.022194 njab-0.0.4/src/njab/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/plotting/km.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/plotting/lifelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/plotting/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:56:54.022194 njab-0.0.4/src/njab/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/sklearn/pca.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/sklearn/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/sklearn/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/sklearn/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:56:54.022194 njab-0.0.4/src/njab/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/stats/ancova.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-02-23 08:56:46.000000 njab-0.0.4/src/njab/stats/groups_comparision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:56:54.022194 njab-0.0.4/src/njab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-02-23 08:56:54.000000 njab-0.0.4/src/njab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-23 08:56:54.000000 njab-0.0.4/src/njab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 08:56:54.000000 njab-0.0.4/src/njab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-23 08:56:54.000000 njab-0.0.4/src/njab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-23 08:56:54.000000 njab-0.0.4/src/njab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:56:54.022194 njab-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-23 08:56:46.000000 njab-0.0.4/test/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-23 08:56:46.000000 njab-0.0.4/test/test_pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-23 08:56:46.000000 njab-0.0.4/test/test_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 14:22:18.000000 njab-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-02 14:22:22.475694 njab-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-02 14:22:18.000000 njab-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 14:22:18.000000 njab-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-02 14:22:22.479694 njab-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 14:22:18.000000 njab-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.471693 njab-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.471693 njab-0.0.5/src/njab/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.471693 njab-0.0.5/src/njab/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.471693 njab-0.0.5/src/njab/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/pandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/src/njab/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/plotting/km.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/plotting/lifelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/plotting/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/src/njab/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/sklearn/pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/sklearn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/sklearn/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/sklearn/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/src/njab/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/stats/ancova.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-02 14:22:18.000000 njab-0.0.5/src/njab/stats/groups_comparision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/src/njab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-02 14:22:22.000000 njab-0.0.5/src/njab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-02 14:22:22.000000 njab-0.0.5/src/njab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:22:22.000000 njab-0.0.5/src/njab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 14:22:22.000000 njab-0.0.5/src/njab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 14:22:22.000000 njab-0.0.5/src/njab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:22:22.475694 njab-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-02 14:22:18.000000 njab-0.0.5/test/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-02 14:22:18.000000 njab-0.0.5/test/test_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 14:22:18.000000 njab-0.0.5/test/test_scoring.py
```

### Comparing `njab-0.0.4/LICENSE` & `njab-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/PKG-INFO` & `njab-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: njab
-Version: 0.0.4
+Version: 0.0.5
 Summary: not Just Another Biomarker
 Author: Henry Webel
 Author-email: "Henry Webel" <henry.webel@cpr.ku.dk>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
@@ -24,15 +24,15 @@
 Requires-Dist: pingouin
 Requires-Dist: seaborn
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-book-theme; extra == "docs"
 Requires-Dist: myst-nb; extra == "docs"
 Requires-Dist: ipywidgets; extra == "docs"
-Requires-Dist: sphinx-new-tab-link; extra == "docs"
+Requires-Dist: sphinx-new-tab-link!=0.2.2; extra == "docs"
 
 # (not) Just Another Biomarker (nJAB)
 
 `njab` is a collection of some python function building on top of 
 `pandas`, `scikit-learn`, `statsmodels`, `pingoin`, `numpy` and more...
 
 It aims to formalize a procedure for biomarker discovery which was first developed for
```

### Comparing `njab-0.0.4/README.md` & `njab-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/setup.cfg` & `njab-0.0.5/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = njab
-version = 0.0.4
+version = 0.0.5
 description = not Just Another Biomarker
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Henry Webel
 author_email = "Henry Webel" <henry.webel@cpr.ku.dk>
 license = MIT
 license_files = LICENSE
@@ -36,15 +36,15 @@
 
 [options.extras_require]
 docs = 
 	sphinx
 	sphinx-book-theme
 	myst-nb
 	ipywidgets
-	sphinx-new-tab-link
+	sphinx-new-tab-link!=0.2.2
 
 [options.packages.find]
 where = src
 exclude = 
 	test*
 
 [yapf]
```

### Comparing `njab-0.0.4/src/njab/pandas/__init__.py` & `njab-0.0.5/src/njab/pandas/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import logging
 import typing
 
+import omegaconf
 import pandas as pd
 import pandas.io.formats.format as pf
 
-import omegaconf
-
 logger = logging.getLogger(__name__)
 
 
-def set_pandas_options() -> None:
+def set_pandas_options(max_columns: int = 100,
+                       max_row: int = 30,
+                       min_row: int = 20,
+                       float_format='{:,.3f}') -> None:
     """Update default pandas options for better display."""
-    pd.options.display.max_columns = 100
-    pd.options.display.max_rows = 30
-    pd.options.display.min_rows = 20
-    pd.options.display.float_format = '{:,.3f}'.format
+    pd.options.display.max_columns = max_columns
+    pd.options.display.max_rows = max_row
+    pd.options.display.min_rows = min_row
+    set_pandas_number_formatting(float_format=float_format)
+
+
+def set_pandas_number_formatting(float_format='{:,.3f}') -> None:
+    pd.options.display.float_format = float_format.format
     # https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.describe_option.html#pandas.describe_option
     pd.options.styler.format.thousands = ','
     # # https://github.com/pandas-dev/pandas/blob/main/pandas/io/formats/format.py#L1475
     # Originally found: https://stackoverflow.com/a/29663750/9684872
 
     try:
         base_class = pf.GenericArrayFormatter
```

### Comparing `njab-0.0.4/src/njab/plotting/__init__.py` & `njab-0.0.5/src/njab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/src/njab/plotting/km.py` & `njab-0.0.5/src/njab/plotting/km.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/src/njab/plotting/lifelines.py` & `njab-0.0.5/src/njab/plotting/lifelines.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/src/njab/plotting/metrics.py` & `njab-0.0.5/src/njab/plotting/metrics.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/src/njab/sklearn/__init__.py` & `njab-0.0.5/src/njab/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/src/njab/sklearn/pca.py` & `njab-0.0.5/src/njab/sklearn/pca.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/src/njab/sklearn/preprocessing.py` & `njab-0.0.5/src/njab/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/src/njab/sklearn/scoring.py` & `njab-0.0.5/src/njab/sklearn/scoring.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/src/njab/sklearn/types.py` & `njab-0.0.5/src/njab/sklearn/types.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/src/njab/stats/ancova.py` & `njab-0.0.5/src/njab/stats/ancova.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/src/njab/stats/groups_comparision.py` & `njab-0.0.5/src/njab/stats/groups_comparision.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.4/src/njab.egg-info/PKG-INFO` & `njab-0.0.5/src/njab.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: njab
-Version: 0.0.4
+Version: 0.0.5
 Summary: not Just Another Biomarker
 Author: Henry Webel
 Author-email: "Henry Webel" <henry.webel@cpr.ku.dk>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
@@ -24,15 +24,15 @@
 Requires-Dist: pingouin
 Requires-Dist: seaborn
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-book-theme; extra == "docs"
 Requires-Dist: myst-nb; extra == "docs"
 Requires-Dist: ipywidgets; extra == "docs"
-Requires-Dist: sphinx-new-tab-link; extra == "docs"
+Requires-Dist: sphinx-new-tab-link!=0.2.2; extra == "docs"
 
 # (not) Just Another Biomarker (nJAB)
 
 `njab` is a collection of some python function building on top of 
 `pandas`, `scikit-learn`, `statsmodels`, `pingoin`, `numpy` and more...
 
 It aims to formalize a procedure for biomarker discovery which was first developed for
```

### Comparing `njab-0.0.4/src/njab.egg-info/SOURCES.txt` & `njab-0.0.5/src/njab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

