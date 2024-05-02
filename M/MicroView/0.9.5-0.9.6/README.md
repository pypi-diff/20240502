# Comparing `tmp/MicroView-0.9.5.tar.gz` & `tmp/MicroView-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MicroView-0.9.5.tar", last modified: Tue Dec 13 12:12:56 2022, max compression
+gzip compressed data, was "MicroView-0.9.6.tar", last modified: Thu Oct 19 18:04:46 2023, max compression
```

## Comparing `MicroView-0.9.5.tar` & `MicroView-0.9.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2022-12-13 12:12:56.191327 MicroView-0.9.5/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1519 2022-05-23 17:42:36.000000 MicroView-0.9.5/LICENSE
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       79 2022-08-02 18:30:31.000000 MicroView-0.9.5/MANIFEST.in
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2022-12-13 12:12:56.141325 MicroView-0.9.5/MicroView.egg-info/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2294 2022-12-13 12:12:55.000000 MicroView-0.9.5/MicroView.egg-info/PKG-INFO
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      819 2022-12-13 12:12:55.000000 MicroView-0.9.5/MicroView.egg-info/SOURCES.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2022-12-13 12:12:55.000000 MicroView-0.9.5/MicroView.egg-info/dependency_links.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       50 2022-12-13 12:12:55.000000 MicroView-0.9.5/MicroView.egg-info/entry_points.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2022-12-13 12:12:55.000000 MicroView-0.9.5/MicroView.egg-info/not-zip-safe
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      162 2022-12-13 12:12:55.000000 MicroView-0.9.5/MicroView.egg-info/requires.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)       10 2022-12-13 12:12:55.000000 MicroView-0.9.5/MicroView.egg-info/top_level.txt
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2294 2022-12-13 12:12:56.191327 MicroView-0.9.5/PKG-INFO
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1395 2022-11-10 12:02:20.000000 MicroView-0.9.5/README.md
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2022-12-13 12:12:56.141325 MicroView-0.9.5/microview/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      117 2022-12-13 12:12:38.000000 MicroView-0.9.5/microview/__init__.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2801 2022-10-17 19:15:20.000000 MicroView-0.9.5/microview/cli.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     6709 2022-09-20 12:59:17.000000 MicroView-0.9.5/microview/file_finder.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     8330 2022-12-13 11:55:54.000000 MicroView-0.9.5/microview/parse_taxonomy.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     5566 2022-12-13 12:05:47.000000 MicroView-0.9.5/microview/plotting.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1359 2022-08-05 17:22:46.000000 MicroView-0.9.5/microview/rendering.py
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2022-12-13 12:12:56.167993 MicroView-0.9.5/microview/schemas/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      256 2022-08-03 14:44:55.000000 MicroView-0.9.5/microview/schemas/__init__.py
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      243 2022-09-20 16:54:14.000000 MicroView-0.9.5/microview/schemas/contrast_table.schema.json
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      613 2022-08-02 18:55:39.000000 MicroView-0.9.5/microview/schemas/kaiju_report.schema.json
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2022-12-13 12:12:56.184660 MicroView-0.9.5/microview/templates/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      236 2022-08-03 14:45:32.000000 MicroView-0.9.5/microview/templates/__init__.py
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2022-12-13 12:12:56.097991 MicroView-0.9.5/microview/templates/assets/
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2022-12-13 12:12:56.184660 MicroView-0.9.5/microview/templates/assets/css/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)   207302 2022-06-22 17:40:26.000000 MicroView-0.9.5/microview/templates/assets/css/bulma_v0.9.4.min.css
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      383 2022-08-16 18:23:02.000000 MicroView-0.9.5/microview/templates/assets/css/custom.css
-drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2022-12-13 12:12:56.184660 MicroView-0.9.5/microview/templates/assets/js/
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)    63532 2022-06-12 11:02:24.000000 MicroView-0.9.5/microview/templates/assets/js/MathJax-2.7.5.js
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)  3682474 2022-06-12 11:00:44.000000 MicroView-0.9.5/microview/templates/assets/js/plotly-2.12.1.min.js
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3635 2022-12-13 12:09:54.000000 MicroView-0.9.5/microview/templates/base.html
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      832 2022-07-16 17:45:52.000000 MicroView-0.9.5/microview/templates/head.html
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)      465 2022-12-13 12:12:56.191327 MicroView-0.9.5/setup.cfg
--rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1826 2022-12-13 12:12:38.000000 MicroView-0.9.5/setup.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-10-19 18:04:46.493329 MicroView-0.9.6/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1519 2023-10-19 16:55:22.000000 MicroView-0.9.6/LICENSE
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       79 2023-10-19 16:55:22.000000 MicroView-0.9.6/MANIFEST.in
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-10-19 18:04:46.489996 MicroView-0.9.6/MicroView.egg-info/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2313 2023-10-19 18:04:46.000000 MicroView-0.9.6/MicroView.egg-info/PKG-INFO
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      819 2023-10-19 18:04:46.000000 MicroView-0.9.6/MicroView.egg-info/SOURCES.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2023-10-19 18:04:46.000000 MicroView-0.9.6/MicroView.egg-info/dependency_links.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       49 2023-10-19 18:04:46.000000 MicroView-0.9.6/MicroView.egg-info/entry_points.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)        1 2023-10-19 18:04:46.000000 MicroView-0.9.6/MicroView.egg-info/not-zip-safe
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      165 2023-10-19 18:04:46.000000 MicroView-0.9.6/MicroView.egg-info/requires.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)       10 2023-10-19 18:04:46.000000 MicroView-0.9.6/MicroView.egg-info/top_level.txt
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2313 2023-10-19 18:04:46.493329 MicroView-0.9.6/PKG-INFO
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1434 2023-10-19 16:55:22.000000 MicroView-0.9.6/README.md
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-10-19 18:04:46.489996 MicroView-0.9.6/microview/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      117 2023-10-19 18:04:35.000000 MicroView-0.9.6/microview/__init__.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     2801 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/cli.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     6708 2023-10-19 18:04:35.000000 MicroView-0.9.6/microview/file_finder.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     8329 2023-10-19 18:04:35.000000 MicroView-0.9.6/microview/parse_taxonomy.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     5640 2023-10-19 18:04:35.000000 MicroView-0.9.6/microview/plotting.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1359 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/rendering.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-10-19 18:04:46.489996 MicroView-0.9.6/microview/schemas/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      256 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/schemas/__init__.py
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      243 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/schemas/contrast_table.schema.json
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      613 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/schemas/kaiju_report.schema.json
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-10-19 18:04:46.489996 MicroView-0.9.6/microview/templates/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      236 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/templates/__init__.py
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-10-19 18:04:46.489996 MicroView-0.9.6/microview/templates/assets/
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-10-19 18:04:46.489996 MicroView-0.9.6/microview/templates/assets/css/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)   207302 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/templates/assets/css/bulma_v0.9.4.min.css
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      383 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/templates/assets/css/custom.css
+drwxr-xr-x   0 jvfe      (1000) jvfe      (1000)        0 2023-10-19 18:04:46.489996 MicroView-0.9.6/microview/templates/assets/js/
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)    63532 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/templates/assets/js/MathJax-2.7.5.js
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)  3682474 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/templates/assets/js/plotly-2.12.1.min.js
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     3635 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/templates/base.html
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      832 2023-10-19 16:55:22.000000 MicroView-0.9.6/microview/templates/head.html
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)      465 2023-10-19 18:04:46.493329 MicroView-0.9.6/setup.cfg
+-rw-r--r--   0 jvfe      (1000) jvfe      (1000)     1829 2023-10-19 18:04:35.000000 MicroView-0.9.6/setup.py
```

### Comparing `MicroView-0.9.5/LICENSE` & `MicroView-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MicroView-0.9.5/MicroView.egg-info/PKG-INFO` & `MicroView-0.9.6/MicroView.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: MicroView
-Version: 0.9.5
+Version: 0.9.6
 Summary: Generate reports from metagenomics data
 Home-page: https://github.com/jvfe/microview
 Author: João Vitor F. Cavalcante
 Author-email: jvfe@ufrn.edu.br
 License: BSD license
 Project-URL: Bug Tracker, https://github.com/jvfe/microview/issues
 Project-URL: Documentation, https://jvfe.github.io/microview/
 Project-URL: Source Code, https://github.com/jvfe/microview
 Keywords: metagenomics workflow visualization report
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # MicroView
 
 <!-- badges: start -->
+
 [![license](https://img.shields.io/badge/license-BSD%203--Clause-green)](https://github.com/dalmolingroup/microview/blob/master/LICENSE)
 [![pytest status](https://github.com/dalmolingroup/microview/workflows/test-and-lint/badge.svg)](https://github.com/dalmolingroup/microview/actions)
-[![documentation status](https://github.com/dalmolingroup/microview/workflows/docs/badge.svg)](https://dalmolingroup.github.io/MicroView/)
+[![Documentation Status](https://readthedocs.org/projects/microview-bio/badge/?version=latest)](https://microview-bio.readthedocs.io/en/latest/?badge=latest)
+
 <!-- badges: end -->
 
 MicroView, a reporting tool for taxonomic classification
 
 MicroView agreggates results from taxonomic classification tools,
 such as Kaiju and Kraken, building an interactive HTML report with
 insightful visualizations.
 
-Checkout the [full documentation](https://dalmolingroup.github.io/MicroView/).
+Checkout the [full documentation](https://microview-bio.readthedocs.io/en/latest/?badge=latest).
 
 ## Quickstart
 
 Install the package:
 
 ```sh
 pip install microview
@@ -67,9 +68,7 @@
 microview -df contrast_table.csv -o report_with_table.html
 ```
 
 Then, an HTML file named `microview_report.html` -
 or the name you defined with the `-o` param -
 should be available in your working directory,
 try opening it with your browser!
-
-
```

### Comparing `MicroView-0.9.5/MicroView.egg-info/SOURCES.txt` & `MicroView-0.9.6/MicroView.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MicroView-0.9.5/PKG-INFO` & `MicroView-0.9.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: MicroView
-Version: 0.9.5
+Version: 0.9.6
 Summary: Generate reports from metagenomics data
 Home-page: https://github.com/jvfe/microview
 Author: João Vitor F. Cavalcante
 Author-email: jvfe@ufrn.edu.br
 License: BSD license
 Project-URL: Bug Tracker, https://github.com/jvfe/microview/issues
 Project-URL: Documentation, https://jvfe.github.io/microview/
 Project-URL: Source Code, https://github.com/jvfe/microview
 Keywords: metagenomics workflow visualization report
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # MicroView
 
 <!-- badges: start -->
+
 [![license](https://img.shields.io/badge/license-BSD%203--Clause-green)](https://github.com/dalmolingroup/microview/blob/master/LICENSE)
 [![pytest status](https://github.com/dalmolingroup/microview/workflows/test-and-lint/badge.svg)](https://github.com/dalmolingroup/microview/actions)
-[![documentation status](https://github.com/dalmolingroup/microview/workflows/docs/badge.svg)](https://dalmolingroup.github.io/MicroView/)
+[![Documentation Status](https://readthedocs.org/projects/microview-bio/badge/?version=latest)](https://microview-bio.readthedocs.io/en/latest/?badge=latest)
+
 <!-- badges: end -->
 
 MicroView, a reporting tool for taxonomic classification
 
 MicroView agreggates results from taxonomic classification tools,
 such as Kaiju and Kraken, building an interactive HTML report with
 insightful visualizations.
 
-Checkout the [full documentation](https://dalmolingroup.github.io/MicroView/).
+Checkout the [full documentation](https://microview-bio.readthedocs.io/en/latest/?badge=latest).
 
 ## Quickstart
 
 Install the package:
 
 ```sh
 pip install microview
@@ -67,9 +68,7 @@
 microview -df contrast_table.csv -o report_with_table.html
 ```
 
 Then, an HTML file named `microview_report.html` -
 or the name you defined with the `-o` param -
 should be available in your working directory,
 try opening it with your browser!
-
-
```

### Comparing `MicroView-0.9.5/README.md` & `MicroView-0.9.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # MicroView
 
 <!-- badges: start -->
+
 [![license](https://img.shields.io/badge/license-BSD%203--Clause-green)](https://github.com/dalmolingroup/microview/blob/master/LICENSE)
 [![pytest status](https://github.com/dalmolingroup/microview/workflows/test-and-lint/badge.svg)](https://github.com/dalmolingroup/microview/actions)
-[![documentation status](https://github.com/dalmolingroup/microview/workflows/docs/badge.svg)](https://dalmolingroup.github.io/MicroView/)
+[![Documentation Status](https://readthedocs.org/projects/microview-bio/badge/?version=latest)](https://microview-bio.readthedocs.io/en/latest/?badge=latest)
+
 <!-- badges: end -->
 
 MicroView, a reporting tool for taxonomic classification
 
 MicroView agreggates results from taxonomic classification tools,
 such as Kaiju and Kraken, building an interactive HTML report with
 insightful visualizations.
 
-Checkout the [full documentation](https://dalmolingroup.github.io/MicroView/).
+Checkout the [full documentation](https://microview-bio.readthedocs.io/en/latest/?badge=latest).
 
 ## Quickstart
 
 Install the package:
 
 ```sh
 pip install microview
```

### Comparing `MicroView-0.9.5/microview/cli.py` & `MicroView-0.9.6/microview/cli.py`

 * *Files identical despite different names*

### Comparing `MicroView-0.9.5/microview/file_finder.py` & `MicroView-0.9.6/microview/file_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         if is_kraken_report(kraken_report)
     ]
 
     if len(kraken_reports) == 0 and len(kaiju_reports) == 0:
         console.print("\n Could not find any valid reports", style="red")
         raise Exception("Could not find any valid files.")
     else:
-
         kraken_not_in_kaiju = list(
             filter(lambda report: report not in kaiju_reports, kraken_reports)
         )
 
         # TODO: Improve how this looks
         all_reports = list(
             chain(
```

### Comparing `MicroView-0.9.5/microview/parse_taxonomy.py` & `MicroView-0.9.6/microview/parse_taxonomy.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
 
 def parse_kaiju2table(sample_name: str, df, parsed_stats: Dict) -> None:
     """
     Parses kaiju report
     """
     for row in df.itertuples():
-
         row_dict = {"n_reads": row.reads, "percent": row.percent}
         if row.taxon_name == "unclassified":
             parsed_stats[sample_name].update({"unclassified": row_dict})
         elif row.taxon_name.startswith("cannot"):
             parsed_stats[sample_name].update({"cannot be assigned": row_dict})
         else:
             taxon_name: str = list(filter(None, row.taxon_name.split(";")))[-1]
```

### Comparing `MicroView-0.9.5/microview/plotting.py` & `MicroView-0.9.6/microview/plotting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import Dict, Optional
 
 from plotly import io
 from plotly.express import bar, colors, line, scatter
 from plotly.graph_objects import Figure
 
 
@@ -48,15 +49,14 @@
         x="index",
         y="value",
         color="variable",
         labels={
             "index": "Sample name",
             "value": "% of reads",
             "variable": "Taxon name",
-            "group": "Group",
         },
         template="plotly_white",
         color_discrete_sequence=colors.qualitative.Alphabet,
         **kwargs,
     )
 
 
@@ -66,15 +66,15 @@
     """
     return scatter(
         abund_div_df,
         x="Pielou Evenness",
         y="Shannon Diversity",
         size="N Taxas",
         hover_data=["index"],
-        labels={"group": "Group", "N Taxas": "# taxas"},
+        labels={"N Taxas": "# taxas"},
         template="plotly_white",
         color_discrete_sequence=colors.qualitative.Safe[3:],
         **kwargs,
     )
 
 
 def plot_beta_pcoa(beta_pcoa, **kwargs):
@@ -82,15 +82,15 @@
     Generate scatter plot of two first coordinates of Beta Diversity PCoA
     """
     fig = scatter(
         beta_pcoa,
         x="PC1",
         y="PC2",
         hover_data=["sample"],
-        labels={"sample": "Sample name", "group": "Group"},
+        labels={"sample": "Sample name"},
         template="plotly_white",
         **kwargs,
     )
     fig.update_traces(marker_size=10)
     return fig
 
 
@@ -153,14 +153,17 @@
             text="PC",
             template="plotly_white",
         )
         pcoa_var.update_traces(textposition="bottom right")
 
     # TODO: Improve this check
     if contrast_df is not None and "group" in contrast_df.columns:
+        contrast_df["sample"] = [
+            str(Path(s).name) for s in contrast_df["sample"].to_list()
+        ]
         merged_taxas_df = merge_with_contrasts(tax_data["common taxas"], contrast_df)
 
         common_taxas = plot_common_taxas(merged_taxas_df, facet_col="group")
         common_taxas.update_xaxes(matches=None)
 
         abund_div = plot_abund_div(
             merge_with_contrasts(tax_data["abund and div"], contrast_df),
```

### Comparing `MicroView-0.9.5/microview/rendering.py` & `MicroView-0.9.6/microview/rendering.py`

 * *Files identical despite different names*

### Comparing `MicroView-0.9.5/microview/schemas/kaiju_report.schema.json` & `MicroView-0.9.6/microview/schemas/kaiju_report.schema.json`

 * *Files identical despite different names*

### Comparing `MicroView-0.9.5/microview/templates/assets/css/bulma_v0.9.4.min.css` & `MicroView-0.9.6/microview/templates/assets/css/bulma_v0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `MicroView-0.9.5/microview/templates/assets/js/MathJax-2.7.5.js` & `MicroView-0.9.6/microview/templates/assets/js/MathJax-2.7.5.js`

 * *Files identical despite different names*

### Comparing `MicroView-0.9.5/microview/templates/assets/js/plotly-2.12.1.min.js` & `MicroView-0.9.6/microview/templates/assets/js/plotly-2.12.1.min.js`

 * *Files identical despite different names*

### Comparing `MicroView-0.9.5/microview/templates/base.html` & `MicroView-0.9.6/microview/templates/base.html`

 * *Files identical despite different names*

### Comparing `MicroView-0.9.5/microview/templates/head.html` & `MicroView-0.9.6/microview/templates/head.html`

 * *Files identical despite different names*

### Comparing `MicroView-0.9.5/setup.py` & `MicroView-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 install_requirements = [
-    "scipy<=1.8",
+    "scipy",
     "scikit-bio",
     "pandas",
     "numpy",
     "plotly",
     "jinja2",
     "rich",
     "rich-click",
     "click-option-group",
-    "frictionless",
+    "frictionless==4.32.0",
 ]
 
 test_requirements = [
     "pytest>=3",
 ]
 
 # Docs reqs
@@ -32,21 +32,21 @@
     "wheel",
     "twine",
 ]
 
 setup(
     author="João Vitor F. Cavalcante",
     author_email="jvfe@ufrn.edu.br",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Natural Language :: English",
     ],
     description="Generate reports from metagenomics data",
     install_requires=install_requirements,
     license="BSD license",
     long_description=readme,
     long_description_content_type="text/markdown",
@@ -60,10 +60,10 @@
     extras_require={"dev": extra_requirements},
     url="https://github.com/jvfe/microview",
     project_urls={
         "Bug Tracker": "https://github.com/jvfe/microview/issues",
         "Documentation": "https://jvfe.github.io/microview/",
         "Source Code": "https://github.com/jvfe/microview",
     },
-    version="0.9.5",
+    version="0.9.6",
     zip_safe=False,
 )
```

