# Comparing `tmp/iglu_py-1.0.5.tar.gz` & `tmp/iglu_py-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iglu_py-1.0.5.tar", last modified: Mon Apr 22 21:57:03 2024, max compression
+gzip compressed data, was "iglu_py-1.0.6.tar", last modified: Thu May  2 17:32:01 2024, max compression
```

## Comparing `iglu_py-1.0.5.tar` & `iglu_py-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:57:03.173953 iglu_py-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-22 21:56:59.000000 iglu_py-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14556 2024-04-22 21:57:03.173953 iglu_py-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-04-22 21:56:59.000000 iglu_py-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:57:03.169953 iglu_py-1.0.5/iglu_py/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-22 21:56:59.000000 iglu_py-1.0.5/iglu_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-22 21:56:59.000000 iglu_py-1.0.5/iglu_py/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:57:03.173953 iglu_py-1.0.5/iglu_py/data/
--rw-r--r--   0 runner    (1001) docker     (127)   123513 2024-04-22 21:56:59.000000 iglu_py-1.0.5/iglu_py/data/example_data_1_subject.csv
--rw-r--r--   0 runner    (1001) docker     (127)   597377 2024-04-22 21:56:59.000000 iglu_py-1.0.5/iglu_py/data/example_data_5_subject.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2010192 2024-04-22 21:56:59.000000 iglu_py-1.0.5/iglu_py/data/example_data_hall.csv
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-22 21:56:59.000000 iglu_py-1.0.5/iglu_py/data/example_meals_hall.csv
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-22 21:56:59.000000 iglu_py-1.0.5/iglu_py/df.py
--rw-r--r--   0 runner    (1001) docker     (127)  4769405 2024-04-22 21:56:59.000000 iglu_py-1.0.5/iglu_py/iglu_4.0.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-22 21:56:59.000000 iglu_py-1.0.5/iglu_py/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:57:03.173953 iglu_py-1.0.5/iglu_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14556 2024-04-22 21:57:03.000000 iglu_py-1.0.5/iglu_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-22 21:57:03.000000 iglu_py-1.0.5/iglu_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:57:03.000000 iglu_py-1.0.5/iglu_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 21:57:03.000000 iglu_py-1.0.5/iglu_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 21:57:03.000000 iglu_py-1.0.5/iglu_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 21:57:03.173953 iglu_py-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-22 21:56:59.000000 iglu_py-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:32:01.276917 iglu_py-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-02 17:31:56.000000 iglu_py-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-05-02 17:32:01.276917 iglu_py-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-05-02 17:31:56.000000 iglu_py-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:32:01.272917 iglu_py-1.0.6/iglu_py/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-02 17:31:56.000000 iglu_py-1.0.6/iglu_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-02 17:31:56.000000 iglu_py-1.0.6/iglu_py/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:32:01.276917 iglu_py-1.0.6/iglu_py/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   123513 2024-05-02 17:31:56.000000 iglu_py-1.0.6/iglu_py/data/example_data_1_subject.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   597377 2024-05-02 17:31:56.000000 iglu_py-1.0.6/iglu_py/data/example_data_5_subject.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2010192 2024-05-02 17:31:56.000000 iglu_py-1.0.6/iglu_py/data/example_data_hall.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 17:31:56.000000 iglu_py-1.0.6/iglu_py/data/example_meals_hall.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 17:31:56.000000 iglu_py-1.0.6/iglu_py/df.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4769405 2024-05-02 17:31:56.000000 iglu_py-1.0.6/iglu_py/iglu_4.0.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-02 17:31:56.000000 iglu_py-1.0.6/iglu_py/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:32:01.276917 iglu_py-1.0.6/iglu_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-05-02 17:32:01.000000 iglu_py-1.0.6/iglu_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-02 17:32:01.000000 iglu_py-1.0.6/iglu_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:32:01.000000 iglu_py-1.0.6/iglu_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 17:32:01.000000 iglu_py-1.0.6/iglu_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 17:32:01.000000 iglu_py-1.0.6/iglu_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:32:01.276917 iglu_py-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-02 17:31:56.000000 iglu_py-1.0.6/setup.py
```

### Comparing `iglu_py-1.0.5/PKG-INFO` & `iglu_py-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iglu-py
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python wrapper of R package `iglu` for continuous glucose monitoring data analysis. Wraps the R functions, thus making them accessible in Python.
 Author: Nathaniel J. Fernandes, Lizzie Chun, Irina Gaynanova
 Author-email: njfernandes24@tamu.edu, lizzie_chun1@tamu.edu, irinagn@umich.edu
 Keywords: iglu,Continuous Glucose Monitoring analysis software,diabetes
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: rpy2>=3.5.13
@@ -141,15 +141,15 @@
 |-----------------|:------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|:-------:|
 | Interactive GUI |                                  iglu.iglu_shiny()                                   |                                   iglu::iglu_shiny()                                    |         |
 | All Plots       |                                          ❌                                           |                                            ✅                                            |         |
 | Example Data    | iglu.example_data_X_subject<br />iglu.example_meals_hall<br />iglu.example_data_hall | iglu::example_data_X_subject<br />iglu::example_meals_hall<br />iglu::example_data_hall |  X=1,5  |
 
 | Metrics                           |           Python           |              R               |  Comment  |
 |-----------------------------------|:--------------------------:|:----------------------------:|:---------:|
-| CGMS2DayByDay                     |             ❌              |    iglu::CGMS2DayByDay()     |           |
+| CGMS2DayByDay                     |    iglu.CGMS2DayByDay()    |    iglu::CGMS2DayByDay()     |           |
 | Above %                           |    iglu.above_percent()    |    iglu::above_percent()     |           |
 | Active %                          |   iglu.active_percent()    |    iglu::active_percent()    |           |
 | ADRR                              |        iglu.adrr()         |         iglu::adrr()         |           |
 | AGP                               |             ❌              |         iglu::agp()          | Is a plot |
 | AGP Metrics                       |     iglu.agp_metrics()     |     iglu::agp_metrics()      |           |
 | All Metrics                       |     iglu.all_metrics()     |      iglu::all_metrics       |           |
 | AUC                               |         iglu.auc()         |         iglu::auc()          |           |
@@ -166,15 +166,15 @@
 | GRADE                             |        iglu.grade()        |        iglu::grade()         |           |
 | Grade Eugly                       |     iglu.grade_eugly()     |     iglu::grade_eugly()      |           |
 | Grade Hyper                       |     iglu.grade_hyper()     |     iglu::grade_hyper()      |           |
 | Grade Hypo                        |     iglu.grade_hypo()      |      iglu::grade_hypo()      |           |
 | GRI                               |         iglu.gri()         |         iglu::gri()          |           |
 | GVP                               |         iglu.gvp()         |         iglu::gvp()          |           |
 | HBGI                              |        iglu.hbgi()         |         iglu::hbgi()         |           |
-| Hist_roc                              |        ❌         |         iglu::hist_roc()         |     Is a plot      |
+| Hist_roc                          |             ❌              |       iglu::hist_roc()       | Is a plot |
 | Hyperglucemia Index               |     iglu.hyper_index()     |     iglu::hyper_index()      |           |
 | Hypoglycemia Index                |     iglu.hypo_index()      |      iglu::hypo_index()      |           |
 | Index of Glycemic Control         |         iglu.igc()         |         iglu::igc()          |           |
 | % in target range                 |  iglu.in_range_percent()   |   iglu::in_range_percent()   |           |
 | IQR                               |       iglu.iqr_glu()       |       iglu::iqr_glu()        |           |
 | J-Index                           |       iglu.j_index()       |       iglu::j_index()        |           |
 | LBGI                              |        iglu.lbgi()         |         iglu::lbgi()         |           |
```

### Comparing `iglu_py-1.0.5/README.md` & `iglu_py-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 |-----------------|:------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|:-------:|
 | Interactive GUI |                                  iglu.iglu_shiny()                                   |                                   iglu::iglu_shiny()                                    |         |
 | All Plots       |                                          ❌                                           |                                            ✅                                            |         |
 | Example Data    | iglu.example_data_X_subject<br />iglu.example_meals_hall<br />iglu.example_data_hall | iglu::example_data_X_subject<br />iglu::example_meals_hall<br />iglu::example_data_hall |  X=1,5  |
 
 | Metrics                           |           Python           |              R               |  Comment  |
 |-----------------------------------|:--------------------------:|:----------------------------:|:---------:|
-| CGMS2DayByDay                     |             ❌              |    iglu::CGMS2DayByDay()     |           |
+| CGMS2DayByDay                     |    iglu.CGMS2DayByDay()    |    iglu::CGMS2DayByDay()     |           |
 | Above %                           |    iglu.above_percent()    |    iglu::above_percent()     |           |
 | Active %                          |   iglu.active_percent()    |    iglu::active_percent()    |           |
 | ADRR                              |        iglu.adrr()         |         iglu::adrr()         |           |
 | AGP                               |             ❌              |         iglu::agp()          | Is a plot |
 | AGP Metrics                       |     iglu.agp_metrics()     |     iglu::agp_metrics()      |           |
 | All Metrics                       |     iglu.all_metrics()     |      iglu::all_metrics       |           |
 | AUC                               |         iglu.auc()         |         iglu::auc()          |           |
@@ -154,15 +154,15 @@
 | GRADE                             |        iglu.grade()        |        iglu::grade()         |           |
 | Grade Eugly                       |     iglu.grade_eugly()     |     iglu::grade_eugly()      |           |
 | Grade Hyper                       |     iglu.grade_hyper()     |     iglu::grade_hyper()      |           |
 | Grade Hypo                        |     iglu.grade_hypo()      |      iglu::grade_hypo()      |           |
 | GRI                               |         iglu.gri()         |         iglu::gri()          |           |
 | GVP                               |         iglu.gvp()         |         iglu::gvp()          |           |
 | HBGI                              |        iglu.hbgi()         |         iglu::hbgi()         |           |
-| Hist_roc                              |        ❌         |         iglu::hist_roc()         |     Is a plot      |
+| Hist_roc                          |             ❌              |       iglu::hist_roc()       | Is a plot |
 | Hyperglucemia Index               |     iglu.hyper_index()     |     iglu::hyper_index()      |           |
 | Hypoglycemia Index                |     iglu.hypo_index()      |      iglu::hypo_index()      |           |
 | Index of Glycemic Control         |         iglu.igc()         |         iglu::igc()          |           |
 | % in target range                 |  iglu.in_range_percent()   |   iglu::in_range_percent()   |           |
 | IQR                               |       iglu.iqr_glu()       |       iglu::iqr_glu()        |           |
 | J-Index                           |       iglu.j_index()       |       iglu::j_index()        |           |
 | LBGI                              |        iglu.lbgi()         |         iglu::lbgi()         |           |
```

### Comparing `iglu_py-1.0.5/iglu_py/__init__.py` & `iglu_py-1.0.6/iglu_py/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     above_percent,
     active_percent,
     adrr,
     agp_metrics,
     all_metrics,
     auc,
     below_percent,
+    CGMS2DayByDay,
     cogi,
     conga,
     cv_glu,
     cv_measures,
     ea1c,
     epicalc_profile,
     episode_calculation,
```

### Comparing `iglu_py-1.0.5/iglu_py/bridge.py` & `iglu_py-1.0.6/iglu_py/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,18 +66,22 @@
         "plotly",
     ]
 
     try:
         utils = importr("utils")
 
         for dependency in dependencies:
-            utils.install_packages(dependency, repos="https://cloud.r-project.org/")
+            utils.install_packages(
+                dependency, method="wget", repos="https://cloud.r-project.org/"
+            )
 
         if name_type == "CRAN":
-            utils.install_packages(name, repos="https://cloud.r-project.org/")
+            utils.install_packages(
+                name, method="wget", repos="https://cloud.r-project.org/"
+            )
 
         if name_type == "relative":
             # get file path
             parent_directory = Path(__file__).parent.absolute()
             filepath = os.path.join(parent_directory, name)
 
             print(parent_directory, Path(__file__), filepath)
```

### Comparing `iglu_py-1.0.5/iglu_py/data/example_data_1_subject.csv` & `iglu_py-1.0.6/iglu_py/data/example_data_1_subject.csv`

 * *Files identical despite different names*

### Comparing `iglu_py-1.0.5/iglu_py/data/example_data_5_subject.csv` & `iglu_py-1.0.6/iglu_py/data/example_data_5_subject.csv`

 * *Files identical despite different names*

### Comparing `iglu_py-1.0.5/iglu_py/data/example_data_hall.csv` & `iglu_py-1.0.6/iglu_py/data/example_data_hall.csv`

 * *Files identical despite different names*

### Comparing `iglu_py-1.0.5/iglu_py/df.py` & `iglu_py-1.0.6/iglu_py/df.py`

 * *Files identical despite different names*

### Comparing `iglu_py-1.0.5/iglu_py/iglu_4.0.0.tar.gz` & `iglu_py-1.0.6/iglu_py/iglu_4.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `iglu_py-1.0.5/iglu_py.egg-info/PKG-INFO` & `iglu_py-1.0.6/iglu_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iglu-py
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python wrapper of R package `iglu` for continuous glucose monitoring data analysis. Wraps the R functions, thus making them accessible in Python.
 Author: Nathaniel J. Fernandes, Lizzie Chun, Irina Gaynanova
 Author-email: njfernandes24@tamu.edu, lizzie_chun1@tamu.edu, irinagn@umich.edu
 Keywords: iglu,Continuous Glucose Monitoring analysis software,diabetes
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: rpy2>=3.5.13
@@ -141,15 +141,15 @@
 |-----------------|:------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|:-------:|
 | Interactive GUI |                                  iglu.iglu_shiny()                                   |                                   iglu::iglu_shiny()                                    |         |
 | All Plots       |                                          ❌                                           |                                            ✅                                            |         |
 | Example Data    | iglu.example_data_X_subject<br />iglu.example_meals_hall<br />iglu.example_data_hall | iglu::example_data_X_subject<br />iglu::example_meals_hall<br />iglu::example_data_hall |  X=1,5  |
 
 | Metrics                           |           Python           |              R               |  Comment  |
 |-----------------------------------|:--------------------------:|:----------------------------:|:---------:|
-| CGMS2DayByDay                     |             ❌              |    iglu::CGMS2DayByDay()     |           |
+| CGMS2DayByDay                     |    iglu.CGMS2DayByDay()    |    iglu::CGMS2DayByDay()     |           |
 | Above %                           |    iglu.above_percent()    |    iglu::above_percent()     |           |
 | Active %                          |   iglu.active_percent()    |    iglu::active_percent()    |           |
 | ADRR                              |        iglu.adrr()         |         iglu::adrr()         |           |
 | AGP                               |             ❌              |         iglu::agp()          | Is a plot |
 | AGP Metrics                       |     iglu.agp_metrics()     |     iglu::agp_metrics()      |           |
 | All Metrics                       |     iglu.all_metrics()     |      iglu::all_metrics       |           |
 | AUC                               |         iglu.auc()         |         iglu::auc()          |           |
@@ -166,15 +166,15 @@
 | GRADE                             |        iglu.grade()        |        iglu::grade()         |           |
 | Grade Eugly                       |     iglu.grade_eugly()     |     iglu::grade_eugly()      |           |
 | Grade Hyper                       |     iglu.grade_hyper()     |     iglu::grade_hyper()      |           |
 | Grade Hypo                        |     iglu.grade_hypo()      |      iglu::grade_hypo()      |           |
 | GRI                               |         iglu.gri()         |         iglu::gri()          |           |
 | GVP                               |         iglu.gvp()         |         iglu::gvp()          |           |
 | HBGI                              |        iglu.hbgi()         |         iglu::hbgi()         |           |
-| Hist_roc                              |        ❌         |         iglu::hist_roc()         |     Is a plot      |
+| Hist_roc                          |             ❌              |       iglu::hist_roc()       | Is a plot |
 | Hyperglucemia Index               |     iglu.hyper_index()     |     iglu::hyper_index()      |           |
 | Hypoglycemia Index                |     iglu.hypo_index()      |      iglu::hypo_index()      |           |
 | Index of Glycemic Control         |         iglu.igc()         |         iglu::igc()          |           |
 | % in target range                 |  iglu.in_range_percent()   |   iglu::in_range_percent()   |           |
 | IQR                               |       iglu.iqr_glu()       |       iglu::iqr_glu()        |           |
 | J-Index                           |       iglu.j_index()       |       iglu::j_index()        |           |
 | LBGI                              |        iglu.lbgi()         |         iglu::lbgi()         |           |
```

### Comparing `iglu_py-1.0.5/setup.py` & `iglu_py-1.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.0.5"
+VERSION = "1.0.6"
 DESCRIPTION = "Python wrapper of R package `iglu` for continuous glucose monitoring data analysis. Wraps the R functions, thus making them accessible in Python."
 
 # read the contents of your README file
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
```

