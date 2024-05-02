# Comparing `tmp/tga_data_analysis-2.0.9.tar.gz` & `tmp/tga_data_analysis-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tga_data_analysis-2.0.9.tar", last modified: Sat Apr 27 13:16:55 2024, max compression
+gzip compressed data, was "tga_data_analysis-2.1.0.tar", last modified: Thu May  2 21:34:02 2024, max compression
```

## Comparing `tga_data_analysis-2.0.9.tar` & `tga_data_analysis-2.1.0.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:55.417639 tga_data_analysis-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-27 13:16:55.417639 tga_data_analysis-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 13:16:55.417639 tga_data_analysis-2.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:55.413639 tga_data_analysis-2.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:55.413639 tga_data_analysis-2.0.9/src/tga_data_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/src/tga_data_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/src/tga_data_analysis/kas_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/src/tga_data_analysis/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)    27504 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/src/tga_data_analysis/myfigure.py
--rw-r--r--   0 runner    (1001) docker     (127)    64570 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/src/tga_data_analysis/tga.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:55.417639 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-27 13:16:55.000000 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-27 13:16:55.000000 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 13:16:55.000000 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-27 13:16:55.000000 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 13:16:55.000000 tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:16:55.417639 tga_data_analysis-2.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_deconvolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_kas_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_my_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_oxidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_proximate.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-27 13:16:46.000000 tga_data_analysis-2.0.9/tests/test_soliddist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:34:02.709221 tga_data_analysis-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/src/tga_data_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/src/tga_data_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/src/tga_data_analysis/kas_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/src/tga_data_analysis/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68222 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/src/tga_data_analysis/tga.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-02 21:34:02.000000 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-02 21:34:02.000000 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:34:02.000000 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 21:34:02.000000 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 21:34:02.000000 tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:34:02.713221 tga_data_analysis-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_deconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_kas_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_oxidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_proximate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-02 21:33:56.000000 tga_data_analysis-2.1.0/tests/test_soliddist.py
```

### Comparing `tga_data_analysis-2.0.9/PKG-INFO` & `tga_data_analysis-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tga_data_analysis
-Version: 2.0.9
+Version: 2.1.0
 Summary: Tool for automatic analysis of multiple TGA results
 Author: Matteo Pecchi
 License: MIT
 Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
 Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: matplotlib>=3.4.3
 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: openpyxl
 Requires-Dist: pyarrow
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: lmfit>=1.0.2
+Requires-Dist: myfigure>=1.0.0
 
 # Thermogravimetric Analysis in Python
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ![Python 3.10](https://img.shields.io/badge/python-3.10%2B-blue)
 
@@ -156,7 +157,13 @@
 ## Nomenclature
 
 * ar: as received
 * db: dry basis
 * daf: dry, ash-free
 * vm: volatile matter
 * fc: fixed carbon
+
+## Plotting with myfigure
+
+Plots rely on the package ``myfigure``, a package to simplify 
+Check out the [documentation](https://myfigure.readthedocs.io/) and 
+[GitHub](https://github.com/mpecchi/myfigure/).
```

### Comparing `tga_data_analysis-2.0.9/README.md` & `tga_data_analysis-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -133,8 +133,14 @@
 
 ## Nomenclature
 
 * ar: as received
 * db: dry basis
 * daf: dry, ash-free
 * vm: volatile matter
-* fc: fixed carbon
+* fc: fixed carbon
+
+## Plotting with myfigure
+
+Plots rely on the package ``myfigure``, a package to simplify 
+Check out the [documentation](https://myfigure.readthedocs.io/) and 
+[GitHub](https://github.com/mpecchi/myfigure/).
```

### Comparing `tga_data_analysis-2.0.9/pyproject.toml` & `tga_data_analysis-2.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tga_data_analysis"
-version = "2.0.9"
+version = "2.1.0"
 authors = [
     { name = "Matteo Pecchi"}
 ]
 description = "Tool for automatic analysis of multiple TGA results"
 readme = "README.md"
 license = { text = "MIT" }
 classifiers = [
@@ -19,15 +19,16 @@
     "numpy>=1.21.2",
     "pandas>=1.3.3",
     "matplotlib>=3.4.3",
     "seaborn>=0.11.2",
     "openpyxl",
     "pyarrow",
     "scipy>=1.7.1",
-    "lmfit>=1.0.2"
+    "lmfit>=1.0.2",
+    "myfigure>=1.0.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/mpecchi/tga_data_analysis"
 Documentation = "https://tga-data-analysis.readthedocs.io/en/latest/"
 
 [tool.black]
```

### Comparing `tga_data_analysis-2.0.9/src/tga_data_analysis/kas_kinetics.py` & `tga_data_analysis-2.1.0/src/tga_data_analysis/kas_kinetics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # %%
-import numpy as np
 import pathlib as plib
+import numpy as np
 from tga_data_analysis.tga import Project, Sample
-from tga_data_analysis.myfigure import MyFigure, colors, letters, linestyles, markers
+from myfigure.myfigure import MyFigure, colors, linestyles, markers
 
 
 class KasSample:
     """
     A class to handle and analyze kinetic data using the Kissinger-Akahira-Sunose (KAS) method.
     It provides functionalities to perform KAS analysis on a set of samples, plot analysis results,
     and compare different samples' kinetic parameters.
```

### Comparing `tga_data_analysis-2.0.9/src/tga_data_analysis/measure.py` & `tga_data_analysis-2.1.0/src/tga_data_analysis/measure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.9/src/tga_data_analysis/tga.py` & `tga_data_analysis-2.1.0/src/tga_data_analysis/tga.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Literal, Any
 import pathlib as plib
 import numpy as np
 import pandas as pd
 from scipy.signal import savgol_filter
 from lmfit.models import GaussianModel, LinearModel
 from tga_data_analysis.measure import Measure
-from tga_data_analysis.myfigure import MyFigure, colors, linestyles
+from myfigure.myfigure import MyFigure, colors, linestyles
 
 
 class Project:
     """
     Represents a project (identified by the folder where the data is stored)
     for TGA data analysis.
 
@@ -921,15 +921,21 @@
                     np.round(np.min(file["m_mg"]), 3),
                 )
                 file["m_mg"] = file["m_mg"] - np.min(file["m_mg"])
         except KeyError:
             file["m_mg"] = file["m_p"]
         file["m_p"] = file["m_mg"] / np.max(file["m_mg"]) * 100
         if correct_ash_fr is not None:
-            file["m_p"] = file["m_p"] - np.min(file["m_p"]) + correct_ash_fr
+            # set the ash value to zero
+            file["m_p"] = file["m_p"] - np.min(file["m_p"])
+            # shift the non-ash fraction up by enough to have ash_ar=correct_ash_fr
+            file["m_p"] = file["m_p"] + np.max(file["m_p"]) * (
+                correct_ash_fr / (1 - correct_ash_fr)
+            )
+            # scale everything to 100 %
             file["m_p"] = file["m_p"] / np.max(file["m_p"]) * 100
         file = file[file["T_C"] >= self.temp_initial_celsius].copy()
         file["T_K"] = file["T_C"] + 273.15
         return file
 
     def load_files(self):
         """
@@ -1329,45 +1335,88 @@
             mf.axs[4].plot(
                 self.time.stk(f),
                 self.mp_db.stk(f),
                 color=colors[f],
                 linestyle=linestyles[f],
                 label=self.filenames[f],
             )
-            mf.axs[0].vlines(
-                self.time.stk(f)[self.idx_moist.stk(f)],
-                self.temp.stk(f)[self.idx_moist.stk(f)] - 50,
-                self.temp.stk(f)[self.idx_moist.stk(f)] + 50,
-                linestyle=linestyles[f],
-                color=colors[f],
-            )
-            mf.axs[2].vlines(
-                self.time.stk(f)[self.idx_moist.stk(f)],
-                self.mp_ar.stk(f)[self.idx_moist.stk(f)] - 5,
-                self.mp_ar.stk(f)[self.idx_moist.stk(f)] + 5,
-                linestyle=linestyles[f],
-                color=colors[f],
-            )
+            if self.time_moist:
+                mf.axs[0].plot(
+                    self.time.stk(f)[self.idx_moist.stk(f)],
+                    self.temp.stk(f)[self.idx_moist.stk(f)],
+                    marker="x",
+                    linestyle="None",
+                    color=colors[f],
+                )
+                mf.axs[2].plot(
+                    self.time.stk(f)[self.idx_moist.stk(f)],
+                    self.mp_ar.stk(f)[self.idx_moist.stk(f)],
+                    marker="x",
+                    linestyle="None",
+                    color=colors[f],
+                )
+                if f == self.n_repl - 1:  # only add at the end
+                    mf.axs[0].plot(
+                        [], [], marker="x", linestyle="None", color="grey", label="moist_loc"
+                    )
+                    mf.axs[2].plot(
+                        [], [], marker="x", linestyle="None", color="grey", label="moist_loc"
+                    )
+                # mf.axs[0].vlines(
+                #     self.time.stk(f)[self.idx_moist.stk(f)],
+                #     self.temp.stk(f)[self.idx_moist.stk(f)] - 50,
+                #     self.temp.stk(f)[self.idx_moist.stk(f)] + 50,
+                #     linestyle=linestyles[f],
+                #     color=colors[f],
+                # )
+                # mf.axs[2].vlines(
+                #     self.time.stk(f)[self.idx_moist.stk(f)],
+                #     self.mp_ar.stk(f)[self.idx_moist.stk(f)] - 5,
+                #     self.mp_ar.stk(f)[self.idx_moist.stk(f)] + 5,
+                #     linestyle=linestyles[f],
+                #     color=colors[f],
+                # )
 
             # only try to plot VM is the analysis includes it
-            if self.time_vm is not None:
-                mf.axs[0].vlines(
+            if self.time_vm:
+                # mf.axs[0].vlines(
+                #     self.time.stk(f)[self.idx_vm.stk(f)],
+                #     self.temp.stk(f)[self.idx_vm.stk(f)] - 50,
+                #     self.temp.stk(f)[self.idx_vm.stk(f)] + 50,
+                #     linestyle=linestyles[f],
+                #     color=colors[f],
+                # )
+                # mf.axs[4].vlines(
+                #     self.time.stk(f)[self.idx_vm.stk(f)],
+                #     self.mp_db.stk(f)[self.idx_vm.stk(f)] - 5,
+                #     self.mp_db.stk(f)[self.idx_vm.stk(f)] + 5,
+                #     linestyle=linestyles[f],
+                #     color=colors[f],
+                # )
+                mf.axs[0].plot(
                     self.time.stk(f)[self.idx_vm.stk(f)],
-                    self.temp.stk(f)[self.idx_vm.stk(f)] - 50,
-                    self.temp.stk(f)[self.idx_vm.stk(f)] + 50,
-                    linestyle=linestyles[f],
+                    self.temp.stk(f)[self.idx_vm.stk(f)],
+                    marker="+",
+                    linestyle="None",
                     color=colors[f],
                 )
-                mf.axs[4].vlines(
+                mf.axs[4].plot(
                     self.time.stk(f)[self.idx_vm.stk(f)],
-                    self.mp_db.stk(f)[self.idx_vm.stk(f)] - 5,
-                    self.mp_db.stk(f)[self.idx_vm.stk(f)] + 5,
-                    linestyle=linestyles[f],
+                    self.mp_db.stk(f)[self.idx_vm.stk(f)],
+                    marker="+",
+                    linestyle="None",
                     color=colors[f],
                 )
+                if f == self.n_repl - 1:  # only add at the end
+                    mf.axs[0].plot(
+                        [], [], marker="+", linestyle="None", color="grey", label="vm_loc"
+                    )
+                    mf.axs[4].plot(
+                        [], [], marker="+", linestyle="None", color="grey", label="vm_loc"
+                    )
             # tg plot 1, 3, 5 on the right
             mf.axs[1].plot(
                 self.time_dtg.stk(f),
                 self.temp_dtg,
                 color=colors[f],
                 linestyle=linestyles[f],
                 label=self.filenames[f],
@@ -1384,35 +1433,66 @@
                 self.dtg_db.stk(f),
                 color=colors[f],
                 linestyle=linestyles[f],
                 label=self.filenames[f],
             )
             #
             if self.oxidation_computed:
-                mf.axs[5].vlines(
+                # mf.axs[5].vlines(
+                #     self.time_dtg.stk(f)[self.temp_i_idx.stk(f)],
+                #     ymin=-1.5,
+                #     ymax=0,
+                #     linestyle=linestyles[f],
+                #     color=colors[f],
+                # )
+                # mf.axs[5].vlines(
+                #     self.time_dtg.stk(f)[self.temp_p_idx.stk(f)],
+                #     ymin=np.min(self.dtg_db.stk(f)),
+                #     ymax=np.min(self.dtg_db.stk(f)) / 5,
+                #     linestyle=linestyles[f],
+                #     color=colors[f],
+                # )
+                # mf.axs[5].vlines(
+                #     self.time_dtg.stk(f)[self.temp_b_idx.stk(f)],
+                #     ymin=-1.5,
+                #     ymax=0,
+                #     linestyle=linestyles[f],
+                #     color=colors[f],
+                # )
+                mf.axs[5].plot(
                     self.time_dtg.stk(f)[self.temp_i_idx.stk(f)],
-                    ymin=-1.5,
-                    ymax=0,
-                    linestyle=linestyles[f],
+                    self.dtg_db.stk(f)[self.temp_i_idx.stk(f)],
+                    marker="x",
+                    linestyle="None",
                     color=colors[f],
                 )
-                mf.axs[5].vlines(
+                mf.axs[5].plot(
                     self.time_dtg.stk(f)[self.temp_p_idx.stk(f)],
-                    ymin=np.min(self.dtg_db.stk(f)),
-                    ymax=np.min(self.dtg_db.stk(f)) / 5,
-                    linestyle=linestyles[f],
+                    self.dtg_db.stk(f)[self.temp_p_idx.stk(f)],
+                    marker="+",
+                    linestyle="None",
                     color=colors[f],
                 )
-                mf.axs[5].vlines(
+                mf.axs[5].plot(
                     self.time_dtg.stk(f)[self.temp_b_idx.stk(f)],
-                    ymin=-1.5,
-                    ymax=0,
-                    linestyle=linestyles[f],
+                    self.dtg_db.stk(f)[self.temp_b_idx.stk(f)],
+                    marker="1",
+                    linestyle="None",
                     color=colors[f],
                 )
+                if f == self.n_repl - 1:  # only add at the end
+                    mf.axs[5].plot(
+                        [], [], marker="x", linestyle="None", color="grey", label="Ti_loc"
+                    )
+                    mf.axs[5].plot(
+                        [], [], marker="+", linestyle="None", color="grey", label="Tp_loc"
+                    )
+                    mf.axs[5].plot(
+                        [], [], marker="1", linestyle="None", color="grey", label="Tb_loc"
+                    )
         mf.save_figure()
         return mf
 
     def plot_soliddist(self, **kwargs: dict[str, Any]) -> MyFigure:
         """
         Generate a plot illustrating the solid distribution analysis results.
```

### Comparing `tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/PKG-INFO` & `tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tga_data_analysis
-Version: 2.0.9
+Version: 2.1.0
 Summary: Tool for automatic analysis of multiple TGA results
 Author: Matteo Pecchi
 License: MIT
 Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
 Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: matplotlib>=3.4.3
 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: openpyxl
 Requires-Dist: pyarrow
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: lmfit>=1.0.2
+Requires-Dist: myfigure>=1.0.0
 
 # Thermogravimetric Analysis in Python
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ![Python 3.10](https://img.shields.io/badge/python-3.10%2B-blue)
 
@@ -156,7 +157,13 @@
 ## Nomenclature
 
 * ar: as received
 * db: dry basis
 * daf: dry, ash-free
 * vm: volatile matter
 * fc: fixed carbon
+
+## Plotting with myfigure
+
+Plots rely on the package ``myfigure``, a package to simplify 
+Check out the [documentation](https://myfigure.readthedocs.io/) and 
+[GitHub](https://github.com/mpecchi/myfigure/).
```

### Comparing `tga_data_analysis-2.0.9/src/tga_data_analysis.egg-info/SOURCES.txt` & `tga_data_analysis-2.1.0/src/tga_data_analysis.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 README.md
 pyproject.toml
 src/tga_data_analysis/__init__.py
 src/tga_data_analysis/kas_kinetics.py
 src/tga_data_analysis/measure.py
-src/tga_data_analysis/myfigure.py
 src/tga_data_analysis/tga.py
 src/tga_data_analysis.egg-info/PKG-INFO
 src/tga_data_analysis.egg-info/SOURCES.txt
 src/tga_data_analysis.egg-info/dependency_links.txt
 src/tga_data_analysis.egg-info/requires.txt
 src/tga_data_analysis.egg-info/top_level.txt
 tests/test_deconvolution.py
 tests/test_kas_kinetics.py
 tests/test_measure.py
-tests/test_my_figure.py
 tests/test_oxidation.py
 tests/test_proximate.py
 tests/test_soliddist.py
```

### Comparing `tga_data_analysis-2.0.9/tests/test_deconvolution.py` & `tga_data_analysis-2.1.0/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.9/tests/test_kas_kinetics.py` & `tga_data_analysis-2.1.0/tests/test_kas_kinetics.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.9/tests/test_measure.py` & `tga_data_analysis-2.1.0/tests/test_measure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.9/tests/test_oxidation.py` & `tga_data_analysis-2.1.0/tests/test_oxidation.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.9/tests/test_proximate.py` & `tga_data_analysis-2.1.0/tests/test_proximate.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.9/tests/test_soliddist.py` & `tga_data_analysis-2.1.0/tests/test_soliddist.py`

 * *Files identical despite different names*

