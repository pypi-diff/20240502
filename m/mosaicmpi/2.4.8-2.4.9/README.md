# Comparing `tmp/mosaicmpi-2.4.8.tar.gz` & `tmp/mosaicmpi-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicmpi-2.4.8.tar", last modified: Tue Mar  5 18:33:14 2024, max compression
+gzip compressed data, was "mosaicmpi-2.4.9.tar", last modified: Wed Apr 24 04:01:02 2024, max compression
```

## Comparing `mosaicmpi-2.4.8.tar` & `mosaicmpi-2.4.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 18:33:14.325664 mosaicmpi-2.4.8/
--rw-rw-rw-   0        0        0     1090 2023-08-21 20:09:52.000000 mosaicmpi-2.4.8/LICENSE
--rw-rw-rw-   0        0        0     4503 2024-03-05 18:33:14.325664 mosaicmpi-2.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     3475 2024-03-05 18:30:37.000000 mosaicmpi-2.4.8/README.md
--rw-rw-rw-   0        0        0       86 2023-08-21 03:26:20.000000 mosaicmpi-2.4.8/pyproject.toml
--rw-rw-rw-   0        0        0     1002 2024-03-05 18:33:14.326676 mosaicmpi-2.4.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-05 18:33:14.289339 mosaicmpi-2.4.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-05 18:33:14.310447 mosaicmpi-2.4.8/src/mosaicmpi/
--rw-rw-rw-   0        0        0      550 2024-01-30 22:56:25.000000 mosaicmpi-2.4.8/src/mosaicmpi/__init__.py
--rw-rw-rw-   0        0        0    17785 2023-11-29 18:30:29.000000 mosaicmpi-2.4.8/src/mosaicmpi/biomart.py
--rw-rw-rw-   0        0        0    69264 2024-02-08 04:04:02.000000 mosaicmpi-2.4.8/src/mosaicmpi/cli.py
--rw-rw-rw-   0        0        0    36586 2024-03-05 18:20:37.000000 mosaicmpi-2.4.8/src/mosaicmpi/cnmf.py
--rw-rw-rw-   0        0        0    16074 2024-01-13 03:13:37.000000 mosaicmpi-2.4.8/src/mosaicmpi/colors.py
--rw-rw-rw-   0        0        0     3126 2023-09-14 15:15:14.000000 mosaicmpi-2.4.8/src/mosaicmpi/config.py
--rw-rw-rw-   0        0        0    58017 2024-03-05 18:23:55.000000 mosaicmpi-2.4.8/src/mosaicmpi/dataset.py
--rw-rw-rw-   0        0        0     3751 2024-02-23 18:15:35.000000 mosaicmpi-2.4.8/src/mosaicmpi/gprofiler.py
--rw-rw-rw-   0        0        0    23345 2024-02-20 17:12:09.000000 mosaicmpi-2.4.8/src/mosaicmpi/integration.py
--rw-rw-rw-   0        0        0     6613 2023-08-21 03:26:20.000000 mosaicmpi-2.4.8/src/mosaicmpi/nancorrmp.py
--rw-rw-rw-   0        0        0    53535 2024-02-02 18:58:00.000000 mosaicmpi-2.4.8/src/mosaicmpi/network.py
--rw-rw-rw-   0        0        0     9186 2023-09-13 17:49:00.000000 mosaicmpi-2.4.8/src/mosaicmpi/orphan.py
--rw-rw-rw-   0        0        0    79357 2024-02-07 22:09:34.000000 mosaicmpi-2.4.8/src/mosaicmpi/plots.py
--rw-rw-rw-   0        0        0     5798 2024-01-19 19:04:03.000000 mosaicmpi-2.4.8/src/mosaicmpi/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-05 18:33:14.324354 mosaicmpi-2.4.8/src/mosaicmpi.egg-info/
--rw-rw-rw-   0        0        0     4503 2024-03-05 18:33:14.000000 mosaicmpi-2.4.8/src/mosaicmpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2024-03-05 18:33:14.000000 mosaicmpi-2.4.8/src/mosaicmpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 18:33:14.000000 mosaicmpi-2.4.8/src/mosaicmpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-03-05 18:33:14.000000 mosaicmpi-2.4.8/src/mosaicmpi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      178 2024-03-05 18:33:14.000000 mosaicmpi-2.4.8/src/mosaicmpi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-05 18:33:14.000000 mosaicmpi-2.4.8/src/mosaicmpi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 04:01:02.925857 mosaicmpi-2.4.9/
+-rw-rw-rw-   0        0        0     1090 2023-08-21 20:09:52.000000 mosaicmpi-2.4.9/LICENSE
+-rw-rw-rw-   0        0        0     4517 2024-04-24 04:01:02.924855 mosaicmpi-2.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3489 2024-04-24 03:56:06.000000 mosaicmpi-2.4.9/README.md
+-rw-rw-rw-   0        0        0       86 2023-08-21 03:26:20.000000 mosaicmpi-2.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1002 2024-04-24 04:01:02.926869 mosaicmpi-2.4.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 04:01:02.872254 mosaicmpi-2.4.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 04:01:02.896913 mosaicmpi-2.4.9/src/mosaicmpi/
+-rw-rw-rw-   0        0        0      550 2024-01-30 22:56:25.000000 mosaicmpi-2.4.9/src/mosaicmpi/__init__.py
+-rw-rw-rw-   0        0        0    17785 2023-11-29 18:30:29.000000 mosaicmpi-2.4.9/src/mosaicmpi/biomart.py
+-rw-rw-rw-   0        0        0    69264 2024-02-08 04:04:02.000000 mosaicmpi-2.4.9/src/mosaicmpi/cli.py
+-rw-rw-rw-   0        0        0    36516 2024-04-24 03:51:35.000000 mosaicmpi-2.4.9/src/mosaicmpi/cnmf.py
+-rw-rw-rw-   0        0        0    16074 2024-01-13 03:13:37.000000 mosaicmpi-2.4.9/src/mosaicmpi/colors.py
+-rw-rw-rw-   0        0        0     3126 2023-09-14 15:15:14.000000 mosaicmpi-2.4.9/src/mosaicmpi/config.py
+-rw-rw-rw-   0        0        0    58396 2024-03-25 17:20:06.000000 mosaicmpi-2.4.9/src/mosaicmpi/dataset.py
+-rw-rw-rw-   0        0        0     3751 2024-02-23 18:15:35.000000 mosaicmpi-2.4.9/src/mosaicmpi/gprofiler.py
+-rw-rw-rw-   0        0        0    23345 2024-02-20 17:12:09.000000 mosaicmpi-2.4.9/src/mosaicmpi/integration.py
+-rw-rw-rw-   0        0        0     6613 2023-08-21 03:26:20.000000 mosaicmpi-2.4.9/src/mosaicmpi/nancorrmp.py
+-rw-rw-rw-   0        0        0    53535 2024-02-02 18:58:00.000000 mosaicmpi-2.4.9/src/mosaicmpi/network.py
+-rw-rw-rw-   0        0        0     9186 2023-09-13 17:49:00.000000 mosaicmpi-2.4.9/src/mosaicmpi/orphan.py
+-rw-rw-rw-   0        0        0    79357 2024-02-07 22:09:34.000000 mosaicmpi-2.4.9/src/mosaicmpi/plots.py
+-rw-rw-rw-   0        0        0     5798 2024-01-19 19:04:03.000000 mosaicmpi-2.4.9/src/mosaicmpi/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 04:01:02.923856 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/
+-rw-rw-rw-   0        0        0     4517 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      178 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/top_level.txt
```

### Comparing `mosaicmpi-2.4.8/LICENSE` & `mosaicmpi-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/PKG-INFO` & `mosaicmpi-2.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicmpi
-Version: 2.4.8
+Version: 2.4.9
 Summary: mosaicMPI: Mosaic Multi-resolution Program Integration
 Home-page: https://github.com/MorrissyLab/mosaicMPI
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/mosaicMPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,26 +32,26 @@
 Requires-Dist: fastcluster
 Requires-Dist: tqdm
 
 ![mosaicMPI logo](https://github.com/MorrissyLab/mosaicMPI/blob/main/docs/source/_static/img/logo.png?raw=True)
 
 # mosaicMPI: mosaic multi-resolution program integration
 
-![version badge](https://img.shields.io/badge/version-2.4.8-blue)
+![version badge](https://img.shields.io/badge/version-2.4.9-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mosaicmpi.svg)](https://pypi.org/project/mosaicmpi/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/mosaicmpi)](https://anaconda.org/conda-forge/mosaicmpi/)
 [![Documentation status](https://readthedocs.org/projects/mosaicmpi/badge/?version=latest&style=flat)](https://mosaicmpi.readthedocs.io)
 [![Downloads](https://static.pepy.tech/badge/mosaicmpi)](https://pepy.tech/project/mosaicmpi)
 [![Stars](https://img.shields.io/github/stars/MorrissyLab/mosaicMPI?logo=GitHub&color=yellow)](https://github.com/MorrissyLab/mosaicMPI/stargazers)
 [![License](https://img.shields.io/pypi/l/mosaicmpi.svg)](https://github.com/MorrissyLab/mosaicMPI/blob/main/LICENSE)
 [![DOI:10.1101/2023.08.18.553919](http://img.shields.io/badge/DOI-10.1101/2023.08.18.553919-B31B1B.svg)](https://doi.org/10.1101/2023.08.18.553919)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Sorana Morrissy](https://github.com/ancasorana)
 
-Contributors: Hyojin Song, Aaron Gillmor, Courtney Hall
+Contributors: Hyojin Song, Aaron Gillmor, Gurveer Gill, Courtney Hall
 
 **mosaicMPI** is a Python package enabling mosaic integration of bulk, single-cell, and spatial expression data through program-level integration.
 Programs are first discovered using consensus non-negative matrix factorization and then integrated using a flexible network-based approach to
 group similar programs together across resolutions and datasets. Program communities are then interpreted using sample/cell metadata and gene set analyses. Integrative program communities enable metadata transfer across datasets.
 
 ## ⚡Main Features
```

### Comparing `mosaicmpi-2.4.8/README.md` & `mosaicmpi-2.4.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ![mosaicMPI logo](https://github.com/MorrissyLab/mosaicMPI/blob/main/docs/source/_static/img/logo.png?raw=True)
 
 # mosaicMPI: mosaic multi-resolution program integration
 
-![version badge](https://img.shields.io/badge/version-2.4.8-blue)
+![version badge](https://img.shields.io/badge/version-2.4.9-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mosaicmpi.svg)](https://pypi.org/project/mosaicmpi/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/mosaicmpi)](https://anaconda.org/conda-forge/mosaicmpi/)
 [![Documentation status](https://readthedocs.org/projects/mosaicmpi/badge/?version=latest&style=flat)](https://mosaicmpi.readthedocs.io)
 [![Downloads](https://static.pepy.tech/badge/mosaicmpi)](https://pepy.tech/project/mosaicmpi)
 [![Stars](https://img.shields.io/github/stars/MorrissyLab/mosaicMPI?logo=GitHub&color=yellow)](https://github.com/MorrissyLab/mosaicMPI/stargazers)
 [![License](https://img.shields.io/pypi/l/mosaicmpi.svg)](https://github.com/MorrissyLab/mosaicMPI/blob/main/LICENSE)
 [![DOI:10.1101/2023.08.18.553919](http://img.shields.io/badge/DOI-10.1101/2023.08.18.553919-B31B1B.svg)](https://doi.org/10.1101/2023.08.18.553919)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Sorana Morrissy](https://github.com/ancasorana)
 
-Contributors: Hyojin Song, Aaron Gillmor, Courtney Hall
+Contributors: Hyojin Song, Aaron Gillmor, Gurveer Gill, Courtney Hall
 
 **mosaicMPI** is a Python package enabling mosaic integration of bulk, single-cell, and spatial expression data through program-level integration.
 Programs are first discovered using consensus non-negative matrix factorization and then integrated using a flexible network-based approach to
 group similar programs together across resolutions and datasets. Program communities are then interpreted using sample/cell metadata and gene set analyses. Integrative program communities enable metadata transfer across datasets.
 
 ## ⚡Main Features
```

### Comparing `mosaicmpi-2.4.8/setup.cfg` & `mosaicmpi-2.4.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f73 6169 636d 7069 0d0a 7665   = mosaicmpi..ve
-00000020: 7273 696f 6e20 3d20 322e 342e 380d 0a61  rsion = 2.4.8..a
+00000020: 7273 696f 6e20 3d20 322e 342e 390d 0a61  rsion = 2.4.9..a
 00000030: 7574 686f 7220 3d20 5465 6420 5665 7268  uthor = Ted Verh
 00000040: 6579 0d0a 6175 7468 6f72 5f65 6d61 696c  ey..author_email
 00000050: 203d 2074 6276 6572 6865 7940 7563 616c   = tbverhey@ucal
 00000060: 6761 7279 2e63 610d 0a64 6573 6372 6970  gary.ca..descrip
 00000070: 7469 6f6e 203d 206d 6f73 6169 634d 5049  tion = mosaicMPI
 00000080: 3a20 4d6f 7361 6963 204d 756c 7469 2d72  : Mosaic Multi-r
 00000090: 6573 6f6c 7574 696f 6e20 5072 6f67 7261  esolution Progra
```

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/__init__.py` & `mosaicmpi-2.4.9/src/mosaicmpi/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/biomart.py` & `mosaicmpi-2.4.9/src/mosaicmpi/biomart.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/cli.py` & `mosaicmpi-2.4.9/src/mosaicmpi/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/cnmf.py` & `mosaicmpi-2.4.9/src/mosaicmpi/cnmf.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,22 +701,19 @@
         if missing_combined:
             failed = []
             # Check if all output files and iterations exist
             for _, row in run_params.iterrows():
                 iter_result = self.paths['iter_spectra'] % (row['n_components'], row['iter'])
                 if not os.path.exists(iter_result) or os.path.getsize(iter_result) == 0:
                     failed.append(iter_result)
-            if failed:
-                raise ValueError(
-                    f"{(len(failed))} files from the factorization step are missing or empty:\n  - " + 
-                    "\n  - ".join(failed)
-                )
             if failed and not skip_missing_iterations:
                 raise ValueError(
-                    f"Postprocessing could not proceed. To skip missing iterations, use --skip_missing_iterations."
+                    f"Postprocessing could not proceed. To skip missing iterations, use --skip_missing_iterations." + 
+                    f"\n {(len(failed))} files from the factorization step are missing or empty:\n  - " + 
+                    "\n  - ".join(failed)
                 )
             elif failed and skip_missing_iterations:
                 logging.warning("Missing files will be skipped")
             else:
                 logging.info(f"Factorization outputs (individual iterations) were found for all values of k. No missing files were detected.")
 
             # combine individual iterations
@@ -738,8 +735,8 @@
             for k in sorted(set(run_params.n_components)):
                 call_consensus(k)
         else:
             logging.error(f"{cpus} is an invalid number of cpus. Please specify a positive integer.")
 
         # create k-selection plot
         self.k_selection_plot(close_fig=True)
-    
+
```

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/colors.py` & `mosaicmpi-2.4.9/src/mosaicmpi/colors.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/config.py` & `mosaicmpi-2.4.9/src/mosaicmpi/config.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/dataset.py` & `mosaicmpi-2.4.9/src/mosaicmpi/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -3383,245 +3383,268 @@
 0000d360: 612e 6f62 732e 7365 6c65 6374 5f64 7479  a.obs.select_dty
 0000d370: 7065 7328 696e 636c 7564 653d 6474 7970  pes(include=dtyp
 0000d380: 6573 290d 0a20 2020 2020 2020 2064 6620  es)..        df 
 0000d390: 3d20 6466 2e64 726f 706e 6128 6178 6973  = df.dropna(axis
 0000d3a0: 3d31 2c20 686f 773d 2261 6c6c 2229 0d0a  =1, how="all")..
 0000d3b0: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
 0000d3c0: 7265 706c 6163 6528 226e 616e 222c 206e  replace("nan", n
-0000d3d0: 702e 4e61 4e29 0d0a 2020 2020 2020 2020  p.NaN)..        
-0000d3e0: 7265 7475 726e 2064 660d 0a20 2020 200d  return df..    .
-0000d3f0: 0a20 2020 2064 6566 2067 6574 5f63 6174  .    def get_cat
-0000d400: 6567 6f72 795f 6f76 6572 7265 7072 6573  egory_overrepres
-0000d410: 656e 7461 7469 6f6e 2873 656c 662c 0d0a  entation(self,..
-0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d440: 2020 2020 2020 2020 6c61 7965 723a 2073          layer: s
-0000d450: 7472 2c0d 0a20 2020 2020 2020 2020 2020  tr,..           
-0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d470: 2020 2020 2020 2020 2020 2020 2074 7275               tru
-0000d480: 6e63 6174 655f 6e65 6761 7469 7665 3a20  ncate_negative: 
-0000d490: 626f 6f6c 203d 2054 7275 652c 0d0a 2020  bool = True,..  
-0000d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4c0: 2020 2020 2020 7375 6273 6574 5f63 6174        subset_cat
-0000d4d0: 6567 6f72 6965 733a 2043 6f6c 6c65 6374  egories: Collect
-0000d4e0: 696f 6e5b 7374 725d 203d 204e 6f6e 650d  ion[str] = None.
-0000d4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d510: 2020 2020 2020 2020 2029 202d 3e20 7064           ) -> pd
-0000d520: 2e44 6174 6146 7261 6d65 3a0d 0a20 2020  .DataFrame:..   
-0000d530: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
-0000d540: 6520 5065 6172 736f 6e20 7265 7369 6475  e Pearson residu
-0000d550: 616c 206f 6620 6368 692d 7371 7561 7265  al of chi-square
-0000d560: 6420 7465 7374 2c20 6173 736f 6369 6174  d test, associat
-0000d570: 696e 6720 7072 6f67 7261 6d73 2066 6f72  ing programs for
-0000d580: 2065 6163 6820 7261 6e6b 2028 6b29 2074   each rank (k) t
-0000d590: 6f20 6361 7465 676f 7269 6573 206f 6620  o categories of 
-0000d5a0: 7361 6d70 6c65 732f 6f62 7365 7276 6174  samples/observat
-0000d5b0: 696f 6e73 2e20 4279 2064 6566 6175 6c74  ions. By default
-0000d5c0: 2c20 7472 756e 6361 7465 7320 6e65 6761  , truncates nega
-0000d5d0: 7469 7665 2076 616c 7565 732e 0d0a 0d0a  tive values.....
-0000d5e0: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
-0000d5f0: 6179 6572 3a20 6e61 6d65 206f 6620 6361  ayer: name of ca
-0000d600: 7465 676f 7269 6361 6c20 6461 7461 206c  tegorical data l
-0000d610: 6179 6572 0d0a 2020 2020 2020 2020 3a74  ayer..        :t
-0000d620: 7970 6520 6c61 7965 723a 2073 7472 0d0a  ype layer: str..
-0000d630: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
-0000d640: 7275 6e63 6174 655f 6e65 6761 7469 7665  runcate_negative
-0000d650: 3a20 5472 756e 6361 7465 206e 6567 6174  : Truncate negat
-0000d660: 6976 6520 7265 7369 6475 616c 7320 746f  ive residuals to
-0000d670: 2030 2c20 6465 6661 756c 7473 2074 6f20   0, defaults to 
-0000d680: 5472 7565 0d0a 2020 2020 2020 2020 3a74  True..        :t
-0000d690: 7970 6520 7472 756e 6361 7465 5f6e 6567  ype truncate_neg
-0000d6a0: 6174 6976 653a 2062 6f6f 6c2c 206f 7074  ative: bool, opt
-0000d6b0: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
-0000d6c0: 7061 7261 6d20 7375 6273 6574 5f63 6174  param subset_cat
-0000d6d0: 6567 6f72 6965 733a 2050 726f 7669 6465  egories: Provide
-0000d6e0: 2061 2073 7562 7365 7420 6f66 2063 6174   a subset of cat
-0000d6f0: 6567 6f72 6965 7320 666f 7220 6361 6c63  egories for calc
-0000d700: 756c 6174 696e 6720 6f76 6572 7265 7072  ulating overrepr
-0000d710: 6573 656e 7461 7469 6f6e 0d0a 2020 2020  esentation..    
-0000d720: 2020 2020 3a74 7970 6520 7375 6273 6574      :type subset
-0000d730: 5f63 6174 6567 6f72 6965 733a 2043 6f6c  _categories: Col
-0000d740: 6c65 6374 696f 6e5b 7374 725d 0d0a 2020  lection[str]..  
-0000d750: 2020 2020 2020 3a72 6574 7572 6e3a 2063        :return: c
-0000d760: 6174 6567 6f72 7920 c397 2070 726f 6772  ategory .. progr
-0000d770: 616d 206d 6174 7269 7820 6f66 206f 7665  am matrix of ove
-0000d780: 7272 6570 7265 7365 6e74 6174 696f 6e20  rrepresentation 
-0000d790: 7661 6c75 6573 0d0a 2020 2020 2020 2020  values..        
-0000d7a0: 3a72 7479 7065 3a20 7064 2e44 6174 6146  :rtype: pd.DataF
-0000d7b0: 7261 6d65 0d0a 2020 2020 2020 2020 2222  rame..        ""
-0000d7c0: 220d 0a20 2020 2020 2020 2075 7361 6765  "..        usage
-0000d7d0: 203d 2073 656c 662e 6765 745f 7573 6167   = self.get_usag
-0000d7e0: 6573 286e 6f72 6d61 6c69 7a65 3d54 7275  es(normalize=Tru
-0000d7f0: 6529 2e63 6f70 7928 290d 0a20 2020 2020  e).copy()..     
-0000d800: 2020 2073 616d 706c 655f 746f 5f63 6c61     sample_to_cla
-0000d810: 7373 203d 2073 656c 662e 6765 745f 6d65  ss = self.get_me
-0000d820: 7461 6461 7461 5f64 6628 295b 6c61 7965  tadata_df()[laye
-0000d830: 725d 0d0a 2020 2020 2020 2020 6966 2073  r]..        if s
-0000d840: 7562 7365 745f 6361 7465 676f 7269 6573  ubset_categories
-0000d850: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-0000d860: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
-0000d870: 655f 746f 5f63 6c61 7373 5b7e 7361 6d70  e_to_class[~samp
-0000d880: 6c65 5f74 6f5f 636c 6173 732e 6973 696e  le_to_class.isin
-0000d890: 2873 7562 7365 745f 6361 7465 676f 7269  (subset_categori
-0000d8a0: 6573 295d 203d 206e 702e 4e61 4e0d 0a20  es)] = np.NaN.. 
-0000d8b0: 2020 2020 2020 2075 7361 6765 2e69 6e64         usage.ind
-0000d8c0: 6578 203d 2075 7361 6765 2e69 6e64 6578  ex = usage.index
-0000d8d0: 2e6d 6170 2873 616d 706c 655f 746f 5f63  .map(sample_to_c
-0000d8e0: 6c61 7373 290d 0a20 2020 2020 2020 206f  lass)..        o
-0000d8f0: 6273 6572 7665 6420 3d20 7573 6167 652e  bserved = usage.
-0000d900: 6772 6f75 7062 7928 6c65 7665 6c3d 302c  groupby(level=0,
-0000d910: 206f 6273 6572 7665 643d 5472 7565 292e   observed=True).
-0000d920: 7375 6d28 290d 0a20 2020 2020 2020 206f  sum()..        o
-0000d930: 6273 6572 7665 6420 3d20 6f62 7365 7276  bserved = observ
-0000d940: 6564 5b6f 6273 6572 7665 642e 7375 6d28  ed[observed.sum(
-0000d950: 6178 6973 3d31 2920 3e20 305d 0d0a 2020  axis=1) > 0]..  
-0000d960: 2020 2020 2020 6e5f 6361 7465 676f 7269        n_categori
-0000d970: 6573 203d 206f 6273 6572 7665 642e 7368  es = observed.sh
-0000d980: 6170 655b 305d 0d0a 2020 2020 2020 2020  ape[0]..        
-0000d990: 6966 206e 5f63 6174 6567 6f72 6965 7320  if n_categories 
-0000d9a0: 3c20 323a 0d0a 2020 2020 2020 2020 2020  < 2:..          
-0000d9b0: 2020 6966 206c 6179 6572 2021 3d20 2268    if layer != "h
-0000d9c0: 7667 5f61 6c6c 5f30 223a 0d0a 2020 2020  vg_all_0":..    
-0000d9d0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000d9e0: 696e 672e 7761 726e 696e 6728 6622 4f76  ing.warning(f"Ov
-0000d9f0: 6572 7265 7072 6573 656e 7461 7469 6f6e  errepresentation
-0000da00: 2063 6f75 6c64 206e 6f74 2062 6520 6361   could not be ca
-0000da10: 6c63 756c 6174 6564 2066 6f72 206c 6179  lculated for lay
-0000da20: 6572 2027 7b6c 6179 6572 7d27 2c20 6173  er '{layer}', as
-0000da30: 206f 6e6c 7920 7b6e 5f63 6174 6567 6f72   only {n_categor
-0000da40: 6965 737d 2063 6174 6567 6f72 6965 7320  ies} categories 
-0000da50: 7765 7265 2066 6f75 6e64 2069 6e20 7468  were found in th
-0000da60: 6520 6461 7461 2e20 220d 0a20 2020 2020  e data. "..     
-0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da80: 2020 2020 2020 2020 2020 2066 224e 6f74             f"Not
-0000da90: 6520 7468 6174 2065 6d70 7479 2076 616c  e that empty val
-0000daa0: 7565 7320 696e 2074 6865 206d 6574 6164  ues in the metad
-0000dab0: 6174 6120 6172 6520 6e6f 7420 636f 6e73  ata are not cons
-0000dac0: 6964 6572 6564 2061 2063 6174 6567 6f72  idered a categor
-0000dad0: 792e 2022 0d0a 2020 2020 2020 2020 2020  y. "..          
-0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daf0: 2020 2020 2020 6622 4f76 6572 7265 7072        f"Overrepr
-0000db00: 6573 656e 7461 7469 6f6e 2063 616e 6e6f  esentation canno
-0000db10: 7420 6265 2063 616c 6375 6c61 7465 6420  t be calculated 
-0000db20: 7769 7468 2066 6577 6572 2074 6861 6e20  with fewer than 
-0000db30: 3220 6361 7465 676f 7269 6573 2066 6f72  2 categories for
-0000db40: 2065 6163 6820 6c61 7965 722e 2022 290d   each layer. ").
-0000db50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000db60: 7572 6e20 7064 2e44 6174 6146 7261 6d65  urn pd.DataFrame
-0000db70: 286e 702e 4e61 4e2c 2069 6e64 6578 203d  (np.NaN, index =
-0000db80: 206f 6273 6572 7665 642e 696e 6465 782c   observed.index,
-0000db90: 2063 6f6c 756d 6e73 3d6f 6273 6572 7665   columns=observe
-0000dba0: 642e 636f 6c75 6d6e 7329 0d0a 2020 2020  d.columns)..    
-0000dbb0: 2020 2020 6578 7065 6374 6564 203d 205b      expected = [
-0000dbc0: 5d0d 0a20 2020 2020 2020 2066 6f72 206b  ]..        for k
-0000dbd0: 2c20 6f62 735f 6b20 696e 206f 6273 6572  , obs_k in obser
-0000dbe0: 7665 642e 542e 6772 6f75 7062 7928 6c65  ved.T.groupby(le
-0000dbf0: 7665 6c3d 3129 3a0d 0a20 2020 2020 2020  vel=1):..       
-0000dc00: 2020 2020 2065 7870 5f6b 203d 2070 642e       exp_k = pd.
-0000dc10: 4461 7461 4672 616d 6528 6f62 735f 6b2e  DataFrame(obs_k.
-0000dc20: 7375 6d28 6178 6973 3d31 2929 2040 2070  sum(axis=1)) @ p
-0000dc30: 642e 4461 7461 4672 616d 6528 6f62 735f  d.DataFrame(obs_
-0000dc40: 6b2e 7375 6d28 6178 6973 3d30 2929 2e54  k.sum(axis=0)).T
-0000dc50: 202f 206f 6273 5f6b 2e73 756d 2829 2e73   / obs_k.sum().s
-0000dc60: 756d 2829 0d0a 2020 2020 2020 2020 2020  um()..          
-0000dc70: 2020 6578 7065 6374 6564 2e61 7070 656e    expected.appen
-0000dc80: 6428 6578 705f 6b29 0d0a 2020 2020 2020  d(exp_k)..      
-0000dc90: 2020 6578 7065 6374 6564 203d 2070 642e    expected = pd.
-0000dca0: 636f 6e63 6174 2865 7870 6563 7465 6429  concat(expected)
-0000dcb0: 2e54 0d0a 2020 2020 2020 2020 6368 6973  .T..        chis
-0000dcc0: 715f 7265 7369 6420 3d20 286f 6273 6572  q_resid = (obser
-0000dcd0: 7665 6420 2d20 6578 7065 6374 6564 2920  ved - expected) 
-0000dce0: 2f20 6e70 2e73 7172 7428 6578 7065 6374  / np.sqrt(expect
-0000dcf0: 6564 2920 2023 2070 6561 7273 6f6e 2072  ed)  # pearson r
-0000dd00: 6573 6964 7561 6c20 6f66 2063 6869 2d73  esidual of chi-s
-0000dd10: 7175 6172 6564 2074 6573 7420 6f66 2063  quared test of c
-0000dd20: 6f6e 7469 6e67 656e 6379 2074 6162 6c65  ontingency table
-0000dd30: 0d0a 2020 2020 2020 2020 6966 2074 7275  ..        if tru
-0000dd40: 6e63 6174 655f 6e65 6761 7469 7665 3a0d  ncate_negative:.
-0000dd50: 0a20 2020 2020 2020 2020 2020 2063 6869  .            chi
-0000dd60: 7371 5f72 6573 6964 203d 2063 6869 7371  sq_resid = chisq
-0000dd70: 5f72 6573 6964 2e63 6c69 7028 6c6f 7765  _resid.clip(lowe
-0000dd80: 723d 3029 0d0a 2020 2020 2020 2020 7265  r=0)..        re
-0000dd90: 7475 726e 2063 6869 7371 5f72 6573 6964  turn chisq_resid
-0000dda0: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
-0000ddb0: 0d0a 2020 2020 6465 6620 6765 745f 6d65  ..    def get_me
-0000ddc0: 7461 6461 7461 5f63 6f72 7265 6c61 7469  tadata_correlati
-0000ddd0: 6f6e 2873 656c 662c 200d 0a20 2020 2020  on(self, ..     
-0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddf0: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
-0000de00: 723a 2073 7472 2c0d 0a20 2020 2020 2020  r: str,..       
-0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de20: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
-0000de30: 3a20 7374 7220 3d20 2270 6561 7273 6f6e  : str = "pearson
-0000de40: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de60: 2020 2020 2920 2d3e 2070 642e 5365 7269      ) -> pd.Seri
-0000de70: 6573 3a0d 0a20 2020 2020 2020 2022 2222  es:..        """
-0000de80: 4361 6c63 756c 6174 6520 5065 6172 736f  Calculate Pearso
-0000de90: 6e20 636f 7272 656c 6174 696f 6e20 6f66  n correlation of
-0000dea0: 2047 4550 2075 7361 6765 2074 6f20 6e75   GEP usage to nu
-0000deb0: 6d65 7269 6361 6c20 6d65 7461 6461 7461  merical metadata
-0000dec0: 2061 6372 6f73 7320 7361 6d70 6c65 732f   across samples/
-0000ded0: 6f62 7365 7276 6174 696f 6e73 2e0d 0a0d  observations....
-0000dee0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000def0: 6c61 7965 723a 206e 616d 6520 6f66 206e  layer: name of n
-0000df00: 756d 6572 6963 616c 2064 6174 6120 6c61  umerical data la
-0000df10: 7965 720d 0a20 2020 2020 2020 203a 7479  yer..        :ty
-0000df20: 7065 206c 6179 6572 3a20 7374 720d 0a20  pe layer: str.. 
-0000df30: 2020 2020 2020 203a 7061 7261 6d20 6d65         :param me
-0000df40: 7468 6f64 3a20 436f 7272 656c 6174 696f  thod: Correlatio
-0000df50: 6e20 6d65 7468 6f64 3a20 2270 6561 7273  n method: "pears
-0000df60: 6f6e 222c 2022 7370 6561 726d 616e 222c  on", "spearman",
-0000df70: 206f 7220 226b 656e 6461 6c6c 222e 2044   or "kendall". D
-0000df80: 6566 6175 6c74 7320 746f 2022 7065 6172  efaults to "pear
-0000df90: 736f 6e22 0d0a 2020 2020 2020 2020 3a74  son"..        :t
-0000dfa0: 7970 6520 6d65 7468 6f64 3a20 7374 722c  ype method: str,
-0000dfb0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-0000dfc0: 2020 203a 7265 7475 726e 3a20 636f 7272     :return: corr
-0000dfd0: 656c 6174 696f 6e20 6f66 2047 4550 2074  elation of GEP t
-0000dfe0: 6f20 6d65 7461 6461 7461 0d0a 2020 2020  o metadata..    
-0000dff0: 2020 2020 3a72 7479 7065 3a20 7064 2e53      :rtype: pd.S
-0000e000: 6572 6965 730d 0a20 2020 2020 2020 2022  eries..        "
-0000e010: 2222 0d0a 2020 2020 2020 2020 7573 6167  ""..        usag
-0000e020: 6520 3d20 7365 6c66 2e67 6574 5f75 7361  e = self.get_usa
-0000e030: 6765 7328 292e 636f 7079 2829 0d0a 2020  ges().copy()..  
-0000e040: 2020 2020 2020 6d65 7461 6461 7461 203d        metadata =
-0000e050: 2073 656c 662e 6765 745f 6d65 7461 6461   self.get_metada
-0000e060: 7461 5f64 6628 295b 6c61 7965 725d 0d0a  ta_df()[layer]..
-0000e070: 2020 2020 2020 2020 6d64 5f63 6f72 7220          md_corr 
-0000e080: 3d20 7573 6167 652e 636f 7272 7769 7468  = usage.corrwith
-0000e090: 286d 6574 6164 6174 612c 206d 6574 686f  (metadata, metho
-0000e0a0: 643d 6d65 7468 6f64 290d 0a20 2020 2020  d=method)..     
-0000e0b0: 2020 2072 6574 7572 6e20 6d64 5f63 6f72     return md_cor
-0000e0c0: 720d 0a20 2020 2020 2020 200d 0a20 2020  r..        ..   
-0000e0d0: 2064 6566 2061 7070 656e 645f 746f 5f68   def append_to_h
-0000e0e0: 6973 746f 7279 2873 656c 662c 2065 6e74  istory(self, ent
-0000e0f0: 7279 293a 0d0a 2020 2020 2020 2020 2222  ry):..        ""
-0000e100: 2241 6464 2065 6e74 7279 2074 6f20 4461  "Add entry to Da
-0000e110: 7461 7365 7420 6869 7374 6f72 792e 0d0a  taset history...
-0000e120: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000e130: 2065 6e74 7279 3a20 4465 7363 7269 7074   entry: Descript
-0000e140: 696f 6e20 6f66 2065 7665 6e74 2074 6f20  ion of event to 
-0000e150: 7265 636f 7264 2069 6e20 7468 6520 6869  record in the hi
-0000e160: 7374 6f72 792e 0d0a 2020 2020 2020 2020  story...        
-0000e170: 3a74 7970 6520 656e 7472 793a 2073 7472  :type entry: str
+0000d3d0: 702e 4e61 4e29 2020 2354 4f44 4f3a 2041  p.NaN)  #TODO: A
+0000d3e0: 6464 7265 7373 2065 7272 6f72 3a20 2f68  ddress error: /h
+0000d3f0: 6f6d 652f 7462 7665 7268 6579 2f6d 696e  ome/tbverhey/min
+0000d400: 6963 6f6e 6461 332f 656e 7673 2f6d 6f73  iconda3/envs/mos
+0000d410: 6169 636d 7069 2f6c 6962 2f70 7974 686f  aicmpi/lib/pytho
+0000d420: 6e33 2e31 312f 7369 7465 2d70 6163 6b61  n3.11/site-packa
+0000d430: 6765 732f 6d6f 7361 6963 6d70 692f 6461  ges/mosaicmpi/da
+0000d440: 7461 7365 742e 7079 3a31 3032 313a 2046  taset.py:1021: F
+0000d450: 7574 7572 6557 6172 6e69 6e67 3a20 5468  utureWarning: Th
+0000d460: 6520 6265 6861 7669 6f72 206f 6620 5365  e behavior of Se
+0000d470: 7269 6573 2e72 6570 6c61 6365 2028 616e  ries.replace (an
+0000d480: 6420 4461 7461 4672 616d 652e 7265 706c  d DataFrame.repl
+0000d490: 6163 6529 2077 6974 6820 4361 7465 676f  ace) with Catego
+0000d4a0: 7269 6361 6c44 7479 7065 2069 7320 6465  ricalDtype is de
+0000d4b0: 7072 6563 6174 6564 2e20 496e 2061 2066  precated. In a f
+0000d4c0: 7574 7572 6520 7665 7273 696f 6e2c 2072  uture version, r
+0000d4d0: 6570 6c61 6365 2077 696c 6c20 6f6e 6c79  eplace will only
+0000d4e0: 2062 6520 7573 6564 2066 6f72 2063 6173   be used for cas
+0000d4f0: 6573 2074 6861 7420 7072 6573 6572 7665  es that preserve
+0000d500: 2074 6865 2063 6174 6567 6f72 6965 732e   the categories.
+0000d510: 2054 6f20 6368 616e 6765 2074 6865 2063   To change the c
+0000d520: 6174 6567 6f72 6965 732c 2075 7365 2073  ategories, use s
+0000d530: 6572 2e63 6174 2e72 656e 616d 655f 6361  er.cat.rename_ca
+0000d540: 7465 676f 7269 6573 2069 6e73 7465 6164  tegories instead
+0000d550: 2e0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+0000d560: 6e20 6466 0d0a 2020 2020 0d0a 2020 2020  n df..    ..    
+0000d570: 6465 6620 6765 745f 6361 7465 676f 7279  def get_category
+0000d580: 5f6f 7665 7272 6570 7265 7365 6e74 6174  _overrepresentat
+0000d590: 696f 6e28 7365 6c66 2c0d 0a20 2020 2020  ion(self,..     
+0000d5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5c0: 2020 206c 6179 6572 3a20 7374 722c 0d0a     layer: str,..
+0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5f0: 2020 2020 2020 2020 7472 756e 6361 7465          truncate
+0000d600: 5f6e 6567 6174 6976 653a 2062 6f6f 6c20  _negative: bool 
+0000d610: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
+0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d640: 2073 7562 7365 745f 6361 7465 676f 7269   subset_categori
+0000d650: 6573 3a20 436f 6c6c 6563 7469 6f6e 5b73  es: Collection[s
+0000d660: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
+0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d690: 2020 2020 2920 2d3e 2070 642e 4461 7461      ) -> pd.Data
+0000d6a0: 4672 616d 653a 0d0a 2020 2020 2020 2020  Frame:..        
+0000d6b0: 2222 2243 616c 6375 6c61 7465 2050 6561  """Calculate Pea
+0000d6c0: 7273 6f6e 2072 6573 6964 7561 6c20 6f66  rson residual of
+0000d6d0: 2063 6869 2d73 7175 6172 6564 2074 6573   chi-squared tes
+0000d6e0: 742c 2061 7373 6f63 6961 7469 6e67 2070  t, associating p
+0000d6f0: 726f 6772 616d 7320 666f 7220 6561 6368  rograms for each
+0000d700: 2072 616e 6b20 286b 2920 746f 2063 6174   rank (k) to cat
+0000d710: 6567 6f72 6965 7320 6f66 2073 616d 706c  egories of sampl
+0000d720: 6573 2f6f 6273 6572 7661 7469 6f6e 732e  es/observations.
+0000d730: 2042 7920 6465 6661 756c 742c 2074 7275   By default, tru
+0000d740: 6e63 6174 6573 206e 6567 6174 6976 6520  ncates negative 
+0000d750: 7661 6c75 6573 2e0d 0a0d 0a20 2020 2020  values.....     
+0000d760: 2020 203a 7061 7261 6d20 6c61 7965 723a     :param layer:
+0000d770: 206e 616d 6520 6f66 2063 6174 6567 6f72   name of categor
+0000d780: 6963 616c 2064 6174 6120 6c61 7965 720d  ical data layer.
+0000d790: 0a20 2020 2020 2020 203a 7479 7065 206c  .        :type l
+0000d7a0: 6179 6572 3a20 7374 720d 0a20 2020 2020  ayer: str..     
+0000d7b0: 2020 203a 7061 7261 6d20 7472 756e 6361     :param trunca
+0000d7c0: 7465 5f6e 6567 6174 6976 653a 2054 7275  te_negative: Tru
+0000d7d0: 6e63 6174 6520 6e65 6761 7469 7665 2072  ncate negative r
+0000d7e0: 6573 6964 7561 6c73 2074 6f20 302c 2064  esiduals to 0, d
+0000d7f0: 6566 6175 6c74 7320 746f 2054 7275 650d  efaults to True.
+0000d800: 0a20 2020 2020 2020 203a 7479 7065 2074  .        :type t
+0000d810: 7275 6e63 6174 655f 6e65 6761 7469 7665  runcate_negative
+0000d820: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+0000d830: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000d840: 2073 7562 7365 745f 6361 7465 676f 7269   subset_categori
+0000d850: 6573 3a20 5072 6f76 6964 6520 6120 7375  es: Provide a su
+0000d860: 6273 6574 206f 6620 6361 7465 676f 7269  bset of categori
+0000d870: 6573 2066 6f72 2063 616c 6375 6c61 7469  es for calculati
+0000d880: 6e67 206f 7665 7272 6570 7265 7365 6e74  ng overrepresent
+0000d890: 6174 696f 6e0d 0a20 2020 2020 2020 203a  ation..        :
+0000d8a0: 7479 7065 2073 7562 7365 745f 6361 7465  type subset_cate
+0000d8b0: 676f 7269 6573 3a20 436f 6c6c 6563 7469  gories: Collecti
+0000d8c0: 6f6e 5b73 7472 5d0d 0a20 2020 2020 2020  on[str]..       
+0000d8d0: 203a 7265 7475 726e 3a20 6361 7465 676f   :return: catego
+0000d8e0: 7279 20c3 9720 7072 6f67 7261 6d20 6d61  ry .. program ma
+0000d8f0: 7472 6978 206f 6620 6f76 6572 7265 7072  trix of overrepr
+0000d900: 6573 656e 7461 7469 6f6e 2076 616c 7565  esentation value
+0000d910: 730d 0a20 2020 2020 2020 203a 7274 7970  s..        :rtyp
+0000d920: 653a 2070 642e 4461 7461 4672 616d 650d  e: pd.DataFrame.
+0000d930: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0000d940: 2020 2020 2020 7573 6167 6520 3d20 7365        usage = se
+0000d950: 6c66 2e67 6574 5f75 7361 6765 7328 6e6f  lf.get_usages(no
+0000d960: 726d 616c 697a 653d 5472 7565 292e 636f  rmalize=True).co
+0000d970: 7079 2829 0d0a 2020 2020 2020 2020 7361  py()..        sa
+0000d980: 6d70 6c65 5f74 6f5f 636c 6173 7320 3d20  mple_to_class = 
+0000d990: 7365 6c66 2e67 6574 5f6d 6574 6164 6174  self.get_metadat
+0000d9a0: 615f 6466 2829 5b6c 6179 6572 5d0d 0a20  a_df()[layer].. 
+0000d9b0: 2020 2020 2020 2069 6620 7375 6273 6574         if subset
+0000d9c0: 5f63 6174 6567 6f72 6965 7320 6973 206e  _categories is n
+0000d9d0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000d9e0: 2020 2020 2020 7361 6d70 6c65 5f74 6f5f        sample_to_
+0000d9f0: 636c 6173 735b 7e73 616d 706c 655f 746f  class[~sample_to
+0000da00: 5f63 6c61 7373 2e69 7369 6e28 7375 6273  _class.isin(subs
+0000da10: 6574 5f63 6174 6567 6f72 6965 7329 5d20  et_categories)] 
+0000da20: 3d20 6e70 2e4e 614e 0d0a 2020 2020 2020  = np.NaN..      
+0000da30: 2020 7573 6167 652e 696e 6465 7820 3d20    usage.index = 
+0000da40: 7573 6167 652e 696e 6465 782e 6d61 7028  usage.index.map(
+0000da50: 7361 6d70 6c65 5f74 6f5f 636c 6173 7329  sample_to_class)
+0000da60: 0d0a 2020 2020 2020 2020 6f62 7365 7276  ..        observ
+0000da70: 6564 203d 2075 7361 6765 2e67 726f 7570  ed = usage.group
+0000da80: 6279 286c 6576 656c 3d30 2c20 6f62 7365  by(level=0, obse
+0000da90: 7276 6564 3d54 7275 6529 2e73 756d 2829  rved=True).sum()
+0000daa0: 0d0a 2020 2020 2020 2020 6f62 7365 7276  ..        observ
+0000dab0: 6564 203d 206f 6273 6572 7665 645b 6f62  ed = observed[ob
+0000dac0: 7365 7276 6564 2e73 756d 2861 7869 733d  served.sum(axis=
+0000dad0: 3129 203e 2030 5d0d 0a20 2020 2020 2020  1) > 0]..       
+0000dae0: 206e 5f63 6174 6567 6f72 6965 7320 3d20   n_categories = 
+0000daf0: 6f62 7365 7276 6564 2e73 6861 7065 5b30  observed.shape[0
+0000db00: 5d0d 0a20 2020 2020 2020 2069 6620 6e5f  ]..        if n_
+0000db10: 6361 7465 676f 7269 6573 203c 2032 3a0d  categories < 2:.
+0000db20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000db30: 6c61 7965 7220 213d 2022 6876 675f 616c  layer != "hvg_al
+0000db40: 6c5f 3022 3a0d 0a20 2020 2020 2020 2020  l_0":..         
+0000db50: 2020 2020 2020 206c 6f67 6769 6e67 2e77         logging.w
+0000db60: 6172 6e69 6e67 2866 224f 7665 7272 6570  arning(f"Overrep
+0000db70: 7265 7365 6e74 6174 696f 6e20 636f 756c  resentation coul
+0000db80: 6420 6e6f 7420 6265 2063 616c 6375 6c61  d not be calcula
+0000db90: 7465 6420 666f 7220 6c61 7965 7220 277b  ted for layer '{
+0000dba0: 6c61 7965 727d 272c 2061 7320 6f6e 6c79  layer}', as only
+0000dbb0: 207b 6e5f 6361 7465 676f 7269 6573 7d20   {n_categories} 
+0000dbc0: 6361 7465 676f 7269 6573 2077 6572 6520  categories were 
+0000dbd0: 666f 756e 6420 696e 2074 6865 2064 6174  found in the dat
+0000dbe0: 612e 2022 0d0a 2020 2020 2020 2020 2020  a. "..          
+0000dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc00: 2020 2020 2020 6622 4e6f 7465 2074 6861        f"Note tha
+0000dc10: 7420 656d 7074 7920 7661 6c75 6573 2069  t empty values i
+0000dc20: 6e20 7468 6520 6d65 7461 6461 7461 2061  n the metadata a
+0000dc30: 7265 206e 6f74 2063 6f6e 7369 6465 7265  re not considere
+0000dc40: 6420 6120 6361 7465 676f 7279 2e20 220d  d a category. ".
+0000dc50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc70: 2066 224f 7665 7272 6570 7265 7365 6e74   f"Overrepresent
+0000dc80: 6174 696f 6e20 6361 6e6e 6f74 2062 6520  ation cannot be 
+0000dc90: 6361 6c63 756c 6174 6564 2077 6974 6820  calculated with 
+0000dca0: 6665 7765 7220 7468 616e 2032 2063 6174  fewer than 2 cat
+0000dcb0: 6567 6f72 6965 7320 666f 7220 6561 6368  egories for each
+0000dcc0: 206c 6179 6572 2e20 2229 0d0a 2020 2020   layer. ")..    
+0000dcd0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+0000dce0: 642e 4461 7461 4672 616d 6528 6e70 2e4e  d.DataFrame(np.N
+0000dcf0: 614e 2c20 696e 6465 7820 3d20 6f62 7365  aN, index = obse
+0000dd00: 7276 6564 2e69 6e64 6578 2c20 636f 6c75  rved.index, colu
+0000dd10: 6d6e 733d 6f62 7365 7276 6564 2e63 6f6c  mns=observed.col
+0000dd20: 756d 6e73 290d 0a20 2020 2020 2020 2065  umns)..        e
+0000dd30: 7870 6563 7465 6420 3d20 5b5d 0d0a 2020  xpected = []..  
+0000dd40: 2020 2020 2020 666f 7220 6b2c 206f 6273        for k, obs
+0000dd50: 5f6b 2069 6e20 6f62 7365 7276 6564 2e54  _k in observed.T
+0000dd60: 2e67 726f 7570 6279 286c 6576 656c 3d31  .groupby(level=1
+0000dd70: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000dd80: 6578 705f 6b20 3d20 7064 2e44 6174 6146  exp_k = pd.DataF
+0000dd90: 7261 6d65 286f 6273 5f6b 2e73 756d 2861  rame(obs_k.sum(a
+0000dda0: 7869 733d 3129 2920 4020 7064 2e44 6174  xis=1)) @ pd.Dat
+0000ddb0: 6146 7261 6d65 286f 6273 5f6b 2e73 756d  aFrame(obs_k.sum
+0000ddc0: 2861 7869 733d 3029 292e 5420 2f20 6f62  (axis=0)).T / ob
+0000ddd0: 735f 6b2e 7375 6d28 292e 7375 6d28 290d  s_k.sum().sum().
+0000dde0: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
+0000ddf0: 6563 7465 642e 6170 7065 6e64 2865 7870  ected.append(exp
+0000de00: 5f6b 290d 0a20 2020 2020 2020 2065 7870  _k)..        exp
+0000de10: 6563 7465 6420 3d20 7064 2e63 6f6e 6361  ected = pd.conca
+0000de20: 7428 6578 7065 6374 6564 292e 540d 0a20  t(expected).T.. 
+0000de30: 2020 2020 2020 2063 6869 7371 5f72 6573         chisq_res
+0000de40: 6964 203d 2028 6f62 7365 7276 6564 202d  id = (observed -
+0000de50: 2065 7870 6563 7465 6429 202f 206e 702e   expected) / np.
+0000de60: 7371 7274 2865 7870 6563 7465 6429 2020  sqrt(expected)  
+0000de70: 2320 7065 6172 736f 6e20 7265 7369 6475  # pearson residu
+0000de80: 616c 206f 6620 6368 692d 7371 7561 7265  al of chi-square
+0000de90: 6420 7465 7374 206f 6620 636f 6e74 696e  d test of contin
+0000dea0: 6765 6e63 7920 7461 626c 650d 0a20 2020  gency table..   
+0000deb0: 2020 2020 2069 6620 7472 756e 6361 7465       if truncate
+0000dec0: 5f6e 6567 6174 6976 653a 0d0a 2020 2020  _negative:..    
+0000ded0: 2020 2020 2020 2020 6368 6973 715f 7265          chisq_re
+0000dee0: 7369 6420 3d20 6368 6973 715f 7265 7369  sid = chisq_resi
+0000def0: 642e 636c 6970 286c 6f77 6572 3d30 290d  d.clip(lower=0).
+0000df00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000df10: 6368 6973 715f 7265 7369 640d 0a20 2020  chisq_resid..   
+0000df20: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
+0000df30: 2064 6566 2067 6574 5f6d 6574 6164 6174   def get_metadat
+0000df40: 615f 636f 7272 656c 6174 696f 6e28 7365  a_correlation(se
+0000df50: 6c66 2c20 0d0a 2020 2020 2020 2020 2020  lf, ..          
+0000df60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df70: 2020 2020 2020 206c 6179 6572 3a20 7374         layer: st
+0000df80: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+0000df90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfa0: 2020 2020 206d 6574 686f 643a 2073 7472       method: str
+0000dfb0: 203d 2022 7065 6172 736f 6e22 0d0a 2020   = "pearson"..  
+0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfd0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000dfe0: 202d 3e20 7064 2e53 6572 6965 733a 0d0a   -> pd.Series:..
+0000dff0: 2020 2020 2020 2020 2222 2243 616c 6375          """Calcu
+0000e000: 6c61 7465 2050 6561 7273 6f6e 2063 6f72  late Pearson cor
+0000e010: 7265 6c61 7469 6f6e 206f 6620 4745 5020  relation of GEP 
+0000e020: 7573 6167 6520 746f 206e 756d 6572 6963  usage to numeric
+0000e030: 616c 206d 6574 6164 6174 6120 6163 726f  al metadata acro
+0000e040: 7373 2073 616d 706c 6573 2f6f 6273 6572  ss samples/obser
+0000e050: 7661 7469 6f6e 732e 0d0a 0d0a 2020 2020  vations.....    
+0000e060: 2020 2020 3a70 6172 616d 206c 6179 6572      :param layer
+0000e070: 3a20 6e61 6d65 206f 6620 6e75 6d65 7269  : name of numeri
+0000e080: 6361 6c20 6461 7461 206c 6179 6572 0d0a  cal data layer..
+0000e090: 2020 2020 2020 2020 3a74 7970 6520 6c61          :type la
+0000e0a0: 7965 723a 2073 7472 0d0a 2020 2020 2020  yer: str..      
+0000e0b0: 2020 3a70 6172 616d 206d 6574 686f 643a    :param method:
+0000e0c0: 2043 6f72 7265 6c61 7469 6f6e 206d 6574   Correlation met
+0000e0d0: 686f 643a 2022 7065 6172 736f 6e22 2c20  hod: "pearson", 
+0000e0e0: 2273 7065 6172 6d61 6e22 2c20 6f72 2022  "spearman", or "
+0000e0f0: 6b65 6e64 616c 6c22 2e20 4465 6661 756c  kendall". Defaul
+0000e100: 7473 2074 6f20 2270 6561 7273 6f6e 220d  ts to "pearson".
+0000e110: 0a20 2020 2020 2020 203a 7479 7065 206d  .        :type m
+0000e120: 6574 686f 643a 2073 7472 2c20 6f70 7469  ethod: str, opti
+0000e130: 6f6e 616c 0d0a 2020 2020 2020 2020 3a72  onal..        :r
+0000e140: 6574 7572 6e3a 2063 6f72 7265 6c61 7469  eturn: correlati
+0000e150: 6f6e 206f 6620 4745 5020 746f 206d 6574  on of GEP to met
+0000e160: 6164 6174 610d 0a20 2020 2020 2020 203a  adata..        :
+0000e170: 7274 7970 653a 2070 642e 5365 7269 6573  rtype: pd.Series
 0000e180: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000e190: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-0000e1a0: 612e 756e 735b 2268 6973 746f 7279 225d  a.uns["history"]
-0000e1b0: 5b64 6174 6574 696d 652e 7574 636e 6f77  [datetime.utcnow
-0000e1c0: 2829 2e69 736f 666f 726d 6174 2829 5d20  ().isoformat()] 
-0000e1d0: 3d20 656e 7472 790d 0a20 2020 2020 2020  = entry..       
-0000e1e0: 200d 0a20 2020 2064 6566 2067 6574 5f68   ..    def get_h
-0000e1f0: 6973 746f 7279 2873 656c 6629 3a0d 0a20  istory(self):.. 
-0000e200: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-0000e210: 7320 7469 6d65 7374 616d 7065 6420 6869  s timestamped hi
-0000e220: 7374 6f72 7920 6f66 2044 6174 6173 6574  story of Dataset
-0000e230: 206f 626a 6563 742e 0d0a 0d0a 2020 2020   object.....    
-0000e240: 2020 2020 3a72 6574 7572 6e3a 2068 6973      :return: his
-0000e250: 746f 7279 0d0a 2020 2020 2020 2020 3a72  tory..        :r
-0000e260: 7479 7065 3a20 6469 6374 0d0a 2020 2020  type: dict..    
-0000e270: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-0000e280: 2072 6574 7572 6e20 7365 6c66 2e61 6461   return self.ada
-0000e290: 7461 2e75 6e73 5b22 6869 7374 6f72 7922  ta.uns["history"
-0000e2a0: 5d                                       ]
+0000e190: 2020 2020 2020 2075 7361 6765 203d 2073         usage = s
+0000e1a0: 656c 662e 6765 745f 7573 6167 6573 2829  elf.get_usages()
+0000e1b0: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
+0000e1c0: 206d 6574 6164 6174 6120 3d20 7365 6c66   metadata = self
+0000e1d0: 2e67 6574 5f6d 6574 6164 6174 615f 6466  .get_metadata_df
+0000e1e0: 2829 5b6c 6179 6572 5d0d 0a20 2020 2020  ()[layer]..     
+0000e1f0: 2020 206d 645f 636f 7272 203d 2075 7361     md_corr = usa
+0000e200: 6765 2e63 6f72 7277 6974 6828 6d65 7461  ge.corrwith(meta
+0000e210: 6461 7461 2c20 6d65 7468 6f64 3d6d 6574  data, method=met
+0000e220: 686f 6429 0d0a 2020 2020 2020 2020 7265  hod)..        re
+0000e230: 7475 726e 206d 645f 636f 7272 0d0a 2020  turn md_corr..  
+0000e240: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
+0000e250: 6170 7065 6e64 5f74 6f5f 6869 7374 6f72  append_to_histor
+0000e260: 7928 7365 6c66 2c20 656e 7472 7929 3a0d  y(self, entry):.
+0000e270: 0a20 2020 2020 2020 2022 2222 4164 6420  .        """Add 
+0000e280: 656e 7472 7920 746f 2044 6174 6173 6574  entry to Dataset
+0000e290: 2068 6973 746f 7279 2e0d 0a0d 0a20 2020   history.....   
+0000e2a0: 2020 2020 203a 7061 7261 6d20 656e 7472       :param entr
+0000e2b0: 793a 2044 6573 6372 6970 7469 6f6e 206f  y: Description o
+0000e2c0: 6620 6576 656e 7420 746f 2072 6563 6f72  f event to recor
+0000e2d0: 6420 696e 2074 6865 2068 6973 746f 7279  d in the history
+0000e2e0: 2e0d 0a20 2020 2020 2020 203a 7479 7065  ...        :type
+0000e2f0: 2065 6e74 7279 3a20 7374 720d 0a20 2020   entry: str..   
+0000e300: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+0000e310: 2020 7365 6c66 2e61 6461 7461 2e75 6e73    self.adata.uns
+0000e320: 5b22 6869 7374 6f72 7922 5d5b 6461 7465  ["history"][date
+0000e330: 7469 6d65 2e75 7463 6e6f 7728 292e 6973  time.utcnow().is
+0000e340: 6f66 6f72 6d61 7428 295d 203d 2065 6e74  oformat()] = ent
+0000e350: 7279 0d0a 2020 2020 2020 2020 0d0a 2020  ry..        ..  
+0000e360: 2020 6465 6620 6765 745f 6869 7374 6f72    def get_histor
+0000e370: 7928 7365 6c66 293a 0d0a 2020 2020 2020  y(self):..      
+0000e380: 2020 2222 2252 6574 7572 6e73 2074 696d    """Returns tim
+0000e390: 6573 7461 6d70 6564 2068 6973 746f 7279  estamped history
+0000e3a0: 206f 6620 4461 7461 7365 7420 6f62 6a65   of Dataset obje
+0000e3b0: 6374 2e0d 0a0d 0a20 2020 2020 2020 203a  ct.....        :
+0000e3c0: 7265 7475 726e 3a20 6869 7374 6f72 790d  return: history.
+0000e3d0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+0000e3e0: 2064 6963 740d 0a20 2020 2020 2020 2022   dict..        "
+0000e3f0: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
+0000e400: 726e 2073 656c 662e 6164 6174 612e 756e  rn self.adata.un
+0000e410: 735b 2268 6973 746f 7279 225d            s["history"]
```

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/gprofiler.py` & `mosaicmpi-2.4.9/src/mosaicmpi/gprofiler.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/integration.py` & `mosaicmpi-2.4.9/src/mosaicmpi/integration.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/nancorrmp.py` & `mosaicmpi-2.4.9/src/mosaicmpi/nancorrmp.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/network.py` & `mosaicmpi-2.4.9/src/mosaicmpi/network.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/orphan.py` & `mosaicmpi-2.4.9/src/mosaicmpi/orphan.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/plots.py` & `mosaicmpi-2.4.9/src/mosaicmpi/plots.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi/utils.py` & `mosaicmpi-2.4.9/src/mosaicmpi/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi.egg-info/PKG-INFO` & `mosaicmpi-2.4.9/src/mosaicmpi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicmpi
-Version: 2.4.8
+Version: 2.4.9
 Summary: mosaicMPI: Mosaic Multi-resolution Program Integration
 Home-page: https://github.com/MorrissyLab/mosaicMPI
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/mosaicMPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,26 +32,26 @@
 Requires-Dist: fastcluster
 Requires-Dist: tqdm
 
 ![mosaicMPI logo](https://github.com/MorrissyLab/mosaicMPI/blob/main/docs/source/_static/img/logo.png?raw=True)
 
 # mosaicMPI: mosaic multi-resolution program integration
 
-![version badge](https://img.shields.io/badge/version-2.4.8-blue)
+![version badge](https://img.shields.io/badge/version-2.4.9-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mosaicmpi.svg)](https://pypi.org/project/mosaicmpi/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/mosaicmpi)](https://anaconda.org/conda-forge/mosaicmpi/)
 [![Documentation status](https://readthedocs.org/projects/mosaicmpi/badge/?version=latest&style=flat)](https://mosaicmpi.readthedocs.io)
 [![Downloads](https://static.pepy.tech/badge/mosaicmpi)](https://pepy.tech/project/mosaicmpi)
 [![Stars](https://img.shields.io/github/stars/MorrissyLab/mosaicMPI?logo=GitHub&color=yellow)](https://github.com/MorrissyLab/mosaicMPI/stargazers)
 [![License](https://img.shields.io/pypi/l/mosaicmpi.svg)](https://github.com/MorrissyLab/mosaicMPI/blob/main/LICENSE)
 [![DOI:10.1101/2023.08.18.553919](http://img.shields.io/badge/DOI-10.1101/2023.08.18.553919-B31B1B.svg)](https://doi.org/10.1101/2023.08.18.553919)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Sorana Morrissy](https://github.com/ancasorana)
 
-Contributors: Hyojin Song, Aaron Gillmor, Courtney Hall
+Contributors: Hyojin Song, Aaron Gillmor, Gurveer Gill, Courtney Hall
 
 **mosaicMPI** is a Python package enabling mosaic integration of bulk, single-cell, and spatial expression data through program-level integration.
 Programs are first discovered using consensus non-negative matrix factorization and then integrated using a flexible network-based approach to
 group similar programs together across resolutions and datasets. Program communities are then interpreted using sample/cell metadata and gene set analyses. Integrative program communities enable metadata transfer across datasets.
 
 ## ⚡Main Features
```

### Comparing `mosaicmpi-2.4.8/src/mosaicmpi.egg-info/SOURCES.txt` & `mosaicmpi-2.4.9/src/mosaicmpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

