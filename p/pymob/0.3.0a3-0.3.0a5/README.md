# Comparing `tmp/pymob-0.3.0a3.tar.gz` & `tmp/pymob-0.3.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymob-0.3.0a3.tar", last modified: Tue Jan 16 14:52:09 2024, max compression
+gzip compressed data, was "pymob-0.3.0a5.tar", last modified: Tue Feb  6 23:09:21 2024, max compression
```

## Comparing `pymob-0.3.0a3.tar` & `pymob-0.3.0a5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 14:52:09.239566 pymob-0.3.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-16 14:52:01.000000 pymob-0.3.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23437 2024-01-16 14:52:09.239566 pymob-0.3.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20659 2024-01-16 14:52:01.000000 pymob-0.3.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 14:52:09.231567 pymob-0.3.0a3/pymob/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 14:52:09.235566 pymob-0.3.0a3/pymob/inference/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    18620 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/numpyro_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/optimize_indy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/pyabc_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/pymoo_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 14:52:09.235566 pymob-0.3.0a3/pymob/inference/sbi/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/sbi/plot_posterior_predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/sbi/posterior_predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/sbi/process_simulations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/sbi/sbi_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/sbi/sbi_snle_sample_posterior.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/sbi/sbi_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/inference/sbi/train_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/prior_predictive_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 14:52:09.235566 pymob-0.3.0a3/pymob/sim/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/sim/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/sim/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/sim/solvetools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)    25753 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 14:52:09.239566 pymob-0.3.0a3/pymob/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/utils/bayesian.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/utils/help.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/utils/math_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/utils/plot_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pymob/utils/store_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 14:52:09.239566 pymob-0.3.0a3/pymob.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23437 2024-01-16 14:52:09.000000 pymob-0.3.0a3/pymob.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-01-16 14:52:09.000000 pymob-0.3.0a3/pymob.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 14:52:09.000000 pymob-0.3.0a3/pymob.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-16 14:52:09.000000 pymob-0.3.0a3/pymob.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-16 14:52:09.000000 pymob-0.3.0a3/pymob.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-16 14:52:09.000000 pymob-0.3.0a3/pymob.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-01-16 14:52:01.000000 pymob-0.3.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 14:52:09.239566 pymob-0.3.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 14:52:09.239566 pymob-0.3.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-01-16 14:52:01.000000 pymob-0.3.0a3/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-01-16 14:52:01.000000 pymob-0.3.0a3/tests/test_numpyro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-01-16 14:52:01.000000 pymob-0.3.0a3/tests/test_sbi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-01-16 14:52:01.000000 pymob-0.3.0a3/tests/test_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-16 14:52:01.000000 pymob-0.3.0a3/tests/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:09:21.621335 pymob-0.3.0a5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-06 23:09:12.000000 pymob-0.3.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23437 2024-02-06 23:09:21.621335 pymob-0.3.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20659 2024-02-06 23:09:12.000000 pymob-0.3.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:09:21.613335 pymob-0.3.0a5/pymob/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:09:21.617335 pymob-0.3.0a5/pymob/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33449 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/numpyro_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/optimize_indy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/pyabc_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/pymoo_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:09:21.617335 pymob-0.3.0a5/pymob/inference/sbi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/sbi/plot_posterior_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/sbi/posterior_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/sbi/process_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/sbi/sbi_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/sbi/sbi_snle_sample_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/sbi/sbi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/inference/sbi/train_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/prior_predictive_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:09:21.617335 pymob-0.3.0a5/pymob/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/sim/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/sim/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/sim/solvetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:09:21.617335 pymob-0.3.0a5/pymob/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/utils/bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/utils/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/utils/math_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/utils/plot_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pymob/utils/store_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:09:21.621335 pymob-0.3.0a5/pymob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23437 2024-02-06 23:09:21.000000 pymob-0.3.0a5/pymob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-02-06 23:09:21.000000 pymob-0.3.0a5/pymob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 23:09:21.000000 pymob-0.3.0a5/pymob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-06 23:09:21.000000 pymob-0.3.0a5/pymob.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-06 23:09:21.000000 pymob-0.3.0a5/pymob.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-06 23:09:21.000000 pymob-0.3.0a5/pymob.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-02-06 23:09:12.000000 pymob-0.3.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 23:09:21.621335 pymob-0.3.0a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 23:09:21.621335 pymob-0.3.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-02-06 23:09:12.000000 pymob-0.3.0a5/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-02-06 23:09:12.000000 pymob-0.3.0a5/tests/test_numpyro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-02-06 23:09:12.000000 pymob-0.3.0a5/tests/test_sbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-02-06 23:09:12.000000 pymob-0.3.0a5/tests/test_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-06 23:09:12.000000 pymob-0.3.0a5/tests/test_simulation.py
```

### Comparing `pymob-0.3.0a3/LICENSE` & `pymob-0.3.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/PKG-INFO` & `pymob-0.3.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymob
-Version: 0.3.0a3
+Version: 0.3.0a5
 Summary: Modelling platform for Python
 Author-email: Florian Schunck <fluncki@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Florian
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,15 @@
 Requires-Dist: matplotlib~=3.7.1
 Requires-Dist: numpy~=1.24.0
 Requires-Dist: pandas~=2.0.2
 Requires-Dist: prettytable~=3.7.0
 Requires-Dist: scipy~=1.10.1
 Requires-Dist: scikit-learn~=1.2.2
 Requires-Dist: tqdm~=4.65.0
-Requires-Dist: toopy==0.5.1
+Requires-Dist: toopy==0.6.0
 Requires-Dist: xarray~=2023.11.0
 Requires-Dist: pathos~=0.3.1
 Provides-Extra: dev
 Requires-Dist: pytest>=7.3; extra == "dev"
 Requires-Dist: pyinstrument>=4.5; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
```

### Comparing `pymob-0.3.0a3/README.md` & `pymob-0.3.0a5/README.md`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/infer.py` & `pymob-0.3.0a5/pymob/infer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import click
 import resource
 
 from pymob.utils import help
 from pymob.utils.store_file import prepare_casestudy, import_package
+from pymob.simulation import SimulationBase
 
 @click.command()
 @click.option("-c", "--case_study", type=str, default="test_case_study", 
               help=help.case_study)
 @click.option("-s", "--scenario", type=str, default="test_scenario", 
               help=help.scenario)
 @click.option("-p", "--package", type=str, default="case_studies", 
@@ -22,20 +23,23 @@
         pkg_dir=package
     )
 
     if n_cores is not None: config.set("multiprocessing", "cores", str(n_cores))
     
     # import package        
     pkg = import_package(package_path=config["case-study"]["package"])
-    Simulation = pkg.sim.Simulation
+    Simulation: SimulationBase = getattr(
+        pkg.sim, config["case-study"].get("simulation", fallback="Simulation"))
     sim = Simulation(config)
 
     sim.set_inferer(backend=inference_backend)
+    sim.prior_predictive_checks()
     sim.inferer.run()
     sim.inferer.store_results()
+    sim.posterior_predictive_checks()
     sim.inferer.plot()
 
     max_ram_mb = resource.getrusage(resource.RUSAGE_SELF).ru_maxrss / 1000
     print("RESOURCE USAGE")
     print("==============")
     print(f"Max RSS: {max_ram_mb} M")
```

### Comparing `pymob-0.3.0a3/pymob/inference/interactive.py` & `pymob-0.3.0a5/pymob/inference/interactive.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/inference/numpyro_backend.py` & `pymob-0.3.0a5/pymob/inference/numpyro_backend.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,85 @@
 from functools import partial, lru_cache
+import re
 from typing import Tuple, Dict, Union, Optional, Callable
 import numpyro
 import jax
 import jax.numpy as jnp
 import numpy as np
 from numpyro import distributions as dist
 from numpyro.infer import Predictive
 from numpyro.distributions import Normal, transforms, TransformedDistribution
 from numpyro import infer
 import xarray as xr
 import arviz as az
 from matplotlib import pyplot as plt
-from sympy import sympify
+import sympy
 import sympy2jax
 
 from pymob.simulation import SimulationBase
 
 
+sympy2jax_extra_funcs = {
+    sympy.Array: jnp.array,
+    sympy.Tuple: tuple,
+}
+
 def LogNormalTrans(loc, scale):
     return TransformedDistribution(
-        Normal(0,1), 
-        [
+        base_distribution=Normal(0,1), 
+        transforms=[
             transforms.AffineTransform(loc=jnp.log(loc), scale=scale), 
             exp()
-        ]
-    )
+        ])
+
+def HalfNormalTrans(scale):
+    return TransformedDistribution(
+        base_distribution=Normal(0,1), 
+        transforms=[
+            transforms.AffineTransform(loc=0, scale=scale), 
+            transforms.AbsTransform()
+        ])
+
+
+def transform(transforms, x):
+    for part in transforms:
+        x = part(x)
+    return x
+
+def inv_transform(transforms, y):
+    for part in transforms[::-1]:
+        y = part.inv(y)
+    return y
+
+
+def catch_patterns(expression_str):
+    # tries to match array notation [0 1 2]
+    pattern = r"\[(\d+(\.\d+)?(\s+\d+(\.\d+)?)*|\s*)\]"
+    if re.fullmatch(pattern, expression_str) is not None:
+        expression_str = expression_str.replace(" ", ",") \
+            .removeprefix("[").removesuffix("]")
+        return f"stack({expression_str})"
 
+    return expression_str
 
 def generate_transform(expression_str):
     # check for parentheses in expression
+    
+    expression_str = catch_patterns(expression_str)
 
     # Parse the expression without knowing the symbol names in advance
-    parsed_expression = sympify(expression_str, evaluate=False)
+    parsed_expression = sympy.sympify(expression_str, evaluate=False)
     free_symbols = tuple(parsed_expression.free_symbols)
 
     # Transform expression to jax expression
-    func = sympy2jax.SymbolicModule(parsed_expression, extra_funcs=None, make_array=True)
+    func = sympy2jax.SymbolicModule(
+        parsed_expression, 
+        extra_funcs=sympy2jax_extra_funcs, 
+        make_array=True
+    )
 
     return {"transform": func, "args": [str(s) for s in free_symbols]}
 
 exp = transforms.ExpTransform
 sigmoid = transforms.SigmoidTransform
 C = transforms.ComposeTransform
 
@@ -56,23 +96,41 @@
             An initialized simulation.
         """
         self.EPS = 1e-8
         self.distribution_map = {
             "lognorm": (LogNormalTrans, {"scale": "loc", "s": "scale"}),
             "binom": (dist.Binomial, {"n":"total_count", "p":"probs"}),
             "normal": dist.Normal,
-            "halfnorm": dist.HalfNormal,
+            "halfnorm": HalfNormalTrans,
             "poisson": (dist.Poisson, {"mu": "rate"}),
         }
         
         self.simulation = simulation
         self.evaluator = self.parse_deterministic_model()
         self.prior = self.parse_model_priors()
         self.error_model = self.parse_error_model()
-        self.inference_model = self.parse_probabilistic_model()
+
+        # parse preprocessing
+        if self.user_defined_preprocessing is not None:
+            self.preprocessing = getattr(
+                self.simulation.prob,
+                self.user_defined_preprocessing
+            )
+
+        # parse the probability model
+        if self.user_defined_probability_model is not None:
+            self.inference_model = getattr(
+                self.simulation.prob, 
+                self.user_defined_probability_model
+            )
+        elif self.gaussian_base_distribution:
+            self.inference_model = self.parse_probabilistic_model_with_gaussian_base()
+        else:
+            self.inference_model = self.parse_probabilistic_model()
+
 
         self.idata: az.InferenceData
 
     @property
     def plot_function(self) -> Optional[str]:
         return self.simulation.config.get(
             "inference", "plot_function", 
@@ -82,14 +140,34 @@
     @property
     def extra_vars(self):
         extra = self.simulation.config.getlist( 
             "inference", "extra_vars", fallback=[]
         )
         return extra if isinstance(extra, list) else [extra]
     
+
+    @property
+    def user_defined_probability_model(self):
+        return self.simulation.config.get(
+            "inference.numpyro", "user_defined_probability_model", fallback=None
+        )
+    
+    @property
+    def user_defined_preprocessing(self):
+        return self.simulation.config.get(
+            "inference.numpyro", "user_defined_preprocessing", fallback=None
+        )
+
+    @property
+    def gaussian_base_distribution(self):
+        flag = self.simulation.config.getint(
+            "inference.numpyro", "gaussian_base_distribution", fallback=False
+        )
+        return bool(flag)
+    
     @property
     def n_predictions(self):
         return self.simulation.config.getint(
             "inference", "n_predictions", fallback=None
         )
     
 
@@ -106,14 +184,39 @@
         )
     
     @property
     def warmup(self):
         return self.simulation.config.getint(
             "inference.numpyro", "warmup", fallback=self.draws
         )
+    
+    @property
+    def thinning(self):
+        return self.simulation.config.getint(
+            "inference.numpyro", "thinning", fallback=1
+        )
+
+    @property
+    def svi_iterations(self):
+        return self.simulation.config.getint(
+            "inference.numpyro", "svi_iterations", fallback=10_000
+        )
+    
+    @property
+    def kernel(self):
+        return self.simulation.config.get(
+            "inference.numpyro", "kernel", fallback="nuts"
+        )
+    
+
+    @property
+    def adapt_state_size(self):
+        return self.simulation.config.getint(
+            "inference.numpyro", "sa_adapt_state_size", fallback=None
+        )
 
     @property
     def init_strategy(self):
         strategy = self.simulation.config.get(
             "inference.numpyro", "init_strategy", fallback="init_to_median"
         )
 
@@ -310,56 +413,213 @@
             # DONE: add biomial n --> I think this is already done
             # numpyro.sample("cext_obs", LogNormalTrans(loc=cext + EPS, scale=sigma_cext).mask(masks["cext"]), obs=obs["cext"] + EPS)
             # numpyro.sample("cint_obs", LogNormalTrans(loc=cint + EPS, scale=sigma_cint).mask(masks["cint"]), obs=obs["cint"] + EPS)
             # numpyro.sample("nrf2_obs", LogNormalTrans(loc=nrf2 + EPS, scale=sigma_nrf2).mask(masks["nrf2"]), obs=obs["nrf2"] + EPS)
             # numpyro.sample("lethality_obs", dist.Binomial(probs=leth, total_count=obs["nzfe"]).mask(masks["lethality"]), obs=obs["lethality"])
         return model
 
+    def parse_probabilistic_model_with_gaussian_base(self):
+        EPS = self.EPS
+        prior = self.prior.copy()
+        error_model = self.error_model.copy()
+        extra = {"EPS": EPS}
+
+
+        def lookup(val, deterministic, prior_samples, observations):
+            if val in deterministic:
+                return deterministic[val]
+            
+            elif val in prior_samples:
+                return prior_samples[val]
+            
+            elif val in observations:
+                return observations[val]
+            
+            elif val in extra:
+                return extra[val]
+
+            else:
+                return val
+
+        def model(solver, obs, masks):
+            theta = {}
+            theta_base = {}
+            for prior_name, prior_kwargs in prior.items():
+
+                # apply transforms to priors. This will be handy when I use nested
+                # parameters
+                prior_distribution_parameters = {}
+                for pri_par, pri_val in prior_kwargs["parameters"].items():
+                    prior_trans_func = pri_val["transform"]
+                    # TODO could be replaced by utils.config.lookup and lookup args
+                    prior_trans_func_kwargs = {k: lookup(k, {}, theta, obs) for k in pri_val["args"]}
+                    prior_distribution_parameters.update({
+                        pri_par: prior_trans_func(**prior_trans_func_kwargs)
+                    })
+
+                # parameterize the prior distribution and extract transforms
+                dist = prior_kwargs["fn"](**prior_distribution_parameters)
+                
+                try:
+                    transforms = getattr(dist, "transforms")
+                except:
+                    raise RuntimeError(
+                        "The specified distribution had no transforms. If setting "
+                        "the option 'inference.numpyro.gaussian_base_distribution = 1', "
+                        "you are only allowed to use parameter distribution, which can "
+                        "be specified as transformed normal distributions. "
+                        "Currently only 'lognorm' and 'halfnorm' are implemented. "
+                        "You can use the numypro.distributions.TransformedDistribution "
+                        "API to specify additional distributions with transforms."
+                        "And pass them to the inferer by updating the distribution map: "
+                        "sim.inferer.distribution_map.update({'newdist': your_new_distribution})"
+                    )
+
+                # sample from a random normal distribution
+                theta_base_i = numpyro.sample(
+                    name=f"{prior_name}_normal_base",
+                    fn=Normal(loc=0, scale=1),
+                    sample_shape=dist.shape()                    
+                )
+
+                # apply the transforms 
+                theta_i = numpyro.deterministic(
+                    name=prior_name,
+                    value=transform(transforms=transforms, x=theta_base_i)
+                )
+
+                theta_base.update({prior_name: theta_base_i})
+                theta.update({prior_name: theta_i})
+
+            # calculate deterministic simulation with parameter samples
+            sim_results = solver(theta=theta)
+
+            # store data_variables as deterministic model output
+            for deterministic_name, deterministic_value in sim_results.items():
+                _ = numpyro.deterministic(
+                    name=deterministic_name, 
+                    value=deterministic_value
+                )
+
+            for error_model_name, error_model_kwargs in error_model.items():
+                error_distribution = error_model_kwargs["fn"]
+                error_distribution_kwargs = {}
+                for errdist_par, errdist_val in error_model_kwargs["parameters"].items():
+                    errdist_trans_func = errdist_val["transform"]
+                    errdist_trans_func_kwargs = {
+                        k: lookup(k, sim_results, theta, obs) for k in errdist_val["args"]
+                    }
+                    error_distribution_kwargs.update({
+                        errdist_par: errdist_trans_func(**errdist_trans_func_kwargs)
+                    })
+
+                _ = numpyro.sample(
+                    name=error_model_name + "_obs",
+                    fn=error_distribution(**error_distribution_kwargs).mask(masks[error_model_name]),
+                    obs=obs[error_model_name]
+                )
+
+
+            # TODO: How to add EPS
+            # DONE: add biomial n --> I think this is already done
+            # numpyro.sample("cext_obs", LogNormalTrans(loc=cext + EPS, scale=sigma_cext).mask(masks["cext"]), obs=obs["cext"] + EPS)
+            # numpyro.sample("cint_obs", LogNormalTrans(loc=cint + EPS, scale=sigma_cint).mask(masks["cint"]), obs=obs["cint"] + EPS)
+            # numpyro.sample("nrf2_obs", LogNormalTrans(loc=nrf2 + EPS, scale=sigma_nrf2).mask(masks["nrf2"]), obs=obs["nrf2"] + EPS)
+            # numpyro.sample("lethality_obs", dist.Binomial(probs=leth, total_count=obs["nzfe"]).mask(masks["lethality"]), obs=obs["lethality"])
+        return model
+
+
+    @staticmethod
+    def preprocessing(**kwargs):
+        return kwargs
+
     def run(self):
         # set parameters of JAX and numpyro
         # jax.config.update("jax_enable_x64", True)
-        numpyro.set_host_device_count(self.chains)
 
         # generate random keys
         key = jax.random.PRNGKey(1)
         key, *subkeys = jax.random.split(key, 20)
         keys = iter(subkeys)
 
         # parse observations and masks for missing data
         obs, masks = self.observation_parser()
 
+        model_kwargs = self.preprocessing(
+            obs=obs, 
+            masks=masks,
+        )
+
         # prepare model and print information about shapes
         model = partial(
             self.inference_model, 
             solver=self.evaluator, 
-            obs=obs, 
-            masks=masks
+            **model_kwargs
         )    
 
         with numpyro.handlers.seed(rng_seed=1):
             trace = numpyro.handlers.trace(model).get_trace()
         print(numpyro.util.format_shapes(trace))
         
-        # set up kernel, MCMC        
-        kernel = infer.NUTS(
-            model, 
-            dense_mass=True, 
-            step_size=0.01,
-            adapt_mass_matrix=True,
-            adapt_step_size=True,
-            max_tree_depth=10,
-            target_accept_prob=0.8,
-            init_strategy=self.init_strategy
-        )
+        if self.kernel.lower() == "sample-adaptive-mcmc":
+            kernel = infer.SA(
+                model=model,
+                dense_mass=True,
+                adapt_state_size=self.adapt_state_size,
+                init_strategy=self.init_strategy,
+            )
+
+        elif self.kernel.lower() == "nuts":
+            kernel = infer.NUTS(
+                model, 
+                dense_mass=True, 
+                step_size=0.01,
+                adapt_mass_matrix=True,
+                adapt_step_size=True,
+                max_tree_depth=10,
+                target_accept_prob=0.8,
+                init_strategy=self.init_strategy
+            )
+
+        elif self.kernel.lower() == "svi":
+            # The current implementation of SVI only works with parameter distributions
+            # that can be derived from normal distributions.
+            # what SVI
+
+            if not self.gaussian_base_distribution:
+                raise RuntimeError(
+                    "SVI is only supported if parameter distributions can be "
+                    "re-parameterized as gaussians. Please set "
+                    "inference.numpyro.gaussian_base_distribution = 1 "
+                    "and if needed use distributions from the loc-scale family "
+                    "to specify the model parameters."
+                )
+
+            guide = infer.autoguide.AutoMultivariateNormal(model)
+            optimizer = numpyro.optim.Adam(step_size=0.0005)
+            svi = infer.SVI(model=model, guide=guide, optim=optimizer, loss=infer.Trace_ELBO())
+            svi_result = svi.run(next(keys), self.svi_iterations)
 
+            self.idata = self.svi_posterior(
+                svi_result, model, guide, next(keys), self.draws
+            )
+
+            # the full cov matrix
+            cov = svi_result.params['auto_scale_tril'].dot(
+                svi_result.params['auto_scale_tril'].T
+            )
+            median = guide.median(svi_result.params)
+            return
+        
         mcmc = infer.MCMC(
             sampler=kernel,
             num_warmup=self.warmup,
-            num_samples=self.draws,
+            num_samples=self.draws * self.thinning,
             num_chains=self.chains,
+            thinning=self.thinning,
             progress_bar=True,
         )
     
         # run inference
         mcmc.run(next(keys))
         mcmc.print_summary()
 
@@ -388,48 +648,116 @@
         posterior_coords = self.simulation.coordinates.copy()
         posterior_coords.update({
             "draw": list(range(self.draws)), 
             "chain": list(range(self.chains))
         })
         return posterior_coords
     
-    def prior_predictive_checks(self, seed=1):
+    @lru_cache
+    def prior_predictions(self, n=100, seed=1):
         key = jax.random.PRNGKey(seed)
-        model = partial(self.inference_model, solver=self.evaluator)    
-            
         obs, masks = self.observation_parser()
 
-        prior_predictive = Predictive(model, num_samples=100, batch_ndims=2)
-        prior_predictions = prior_predictive(key, obs=obs, masks=masks)
+        model_kwargs = self.preprocessing(
+            obs=obs, 
+            masks=masks,
+        )
+        
+        # prepare model
+        model = partial(
+            self.inference_model, 
+            solver=self.evaluator, 
+            **model_kwargs
+        )    
+   
+        prior_predictive = Predictive(
+            model, num_samples=n, batch_ndims=2
+        )
+        prior_predictions = prior_predictive(key)
 
         loglik = numpyro.infer.log_likelihood(
             model=model, 
             posterior_samples=prior_predictions, 
             batch_ndims=2, 
             obs=obs, 
             masks=masks
         )
 
         preds = self.simulation.data_variables
+        preds_obs = [f"{d}_obs" for d in self.simulation.data_variables]
         priors = list(self.simulation.model_parameter_dict.keys())
         posterior_coords = self.posterior_coordinates
+        posterior_coords["draw"] = list(range(n))
         data_structure = self.posterior_data_structure
         
         idata = az.from_dict(
             observed_data=obs,
             prior={k: v for k, v in prior_predictions.items() if k in priors},
-            prior_predictive={k: v for k, v in prior_predictions.items() if k in preds},
+            prior_predictive={k: v for k, v in prior_predictions.items() if k in preds+preds_obs},
             log_likelihood=loglik,
             dims=data_structure,
             coords=posterior_coords,
         )
 
-        self.idata = idata
-        self.idata.to_netcdf(f"{self.simulation.output_path}/numpyro_prior_predictions.nc")
+        return idata
+        # self.idata.to_netcdf(f"{self.simulation.output_path}/numpyro_prior_predictions.nc")
+    
+
+    def svi_posterior(self, svi_result, model, guide, key, n=1000):
+        key, *subkeys = jax.random.split(key, 4)
+        keys = iter(subkeys)
+
+        obs, masks = self.observation_parser()
+
+        params = svi_result.params
+
+        # predictive = Predictive(
+        #     model, guide=guide, params=params, 
+        #     num_samples=n, batch_ndims=2
+        # )
+        # samples = predictive(next(keys))    
+
+        predictive = Predictive(
+            guide, params=params, 
+            num_samples=n, batch_ndims=2
+        )
+        posterior_samples = predictive(next(keys))
+
+        predictive = Predictive(
+            model, posterior_samples, params=params, 
+            num_samples=1000, batch_ndims=2
+        )
+        posterior_predictions = predictive(next(keys))
+
+
+        loglik = numpyro.infer.log_likelihood(
+            model=model, 
+            posterior_samples=posterior_samples, 
+            batch_ndims=2, 
+        )
+
+        preds = self.simulation.data_variables
+        preds_obs = [f"{d}_obs" for d in self.simulation.data_variables]
+        priors = list(self.simulation.model_parameter_dict.keys())
+        posterior_coords = self.posterior_coordinates
+        posterior_coords["draw"] = list(range(n))
+        data_structure = self.posterior_data_structure
+        
+        idata = az.from_dict(
+            observed_data=obs,
+            posterior={k: v for k, v in posterior_predictions.items() if k in priors},
+            posterior_predictive={k: v for k, v in posterior_predictions.items() if k in preds},
+            log_likelihood=loglik,
+            dims=data_structure,
+            coords=posterior_coords,
+        )
+
+        return idata
     
+
     @staticmethod
     def get_dict(group: xr.Dataset):
         data_dict = group.to_dict()["data_vars"]
         return {k: np.array(val["data"]) for k, val in data_dict.items()}
 
 
     @lru_cache
@@ -471,16 +799,17 @@
         
 
         return xr.combine_by_coords(preds)
 
     def store_results(self):
         self.idata.to_netcdf(f"{self.simulation.output_path}/numpyro_posterior.nc")
 
-    def load_results(self):
-        self.idata = az.from_netcdf(f"{self.simulation.output_path}/numpyro_posterior.nc")
+    def load_results(self, file="numpyro_posterior.nc"):
+        self.idata = az.from_netcdf(f"{self.simulation.output_path}/{file}")
+
 
     def plot(self):
         # TODO: combine prior_predictions and posterior predictions
         if hasattr(self.idata, "posterior"):
             axes = az.plot_trace(
                 self.idata,
                 var_names=self.simulation.model_parameter_names
@@ -499,46 +828,137 @@
 
         if hasattr(self.idata, "prior_predictive"):
             self.plot_prior_predictive()
 
         plot_func = getattr(self.simulation, self.plot_function)
         plot_func()
 
-    def plot_prior_predictive(self):
-        self.idata
-
-    def plot_predictions(
-            self, data_variable: str, x_dim: str, ax=None, subset={}
+    def plot_prior_predictions(
+            self, data_variable: str, x_dim: str, ax=None, subset={}, 
+            n=None, seed=None
         ):
-        obs = self.simulation.observations.sel(subset)
+        if n is None:
+            n = self.n_predictions
+
+        if seed is None:
+            seed = self.simulation.seed
+        
+        idata = self.prior_predictions(
+            n=n, 
+            # seed only controls the parameters samples drawn from posterior
+            seed=seed
+        )
+        plot_func = getattr(self.simulation, self.plot_function)
         
-        post_pred = self.posterior_predictions(
+        ax = self.plot_predictions(
+            observations=self.simulation.observations,
+            predictions=idata.prior_predictive,
+            data_variable=data_variable,
+            x_dim=x_dim,
+            ax=ax,
+            subset=subset,
+            mode="draws"
+        )
+
+        return ax
+
+    def plot_posterior_predictions(
+            self, data_variable: str, x_dim: str, ax=None, subset={},
+            n=None, seed=None
+        ):
+        predictions = self.posterior_predictions(
             n=self.n_predictions, 
             # seed only controls the parameters samples drawn from posterior
             seed=self.simulation.seed
-        ).sel(subset)
+        )
+
+        ax = self.plot_predictions(
+            observations=self.simulation.observations,
+            predictions=predictions,
+            data_variable=data_variable,
+            x_dim=x_dim,
+            ax=ax,
+            subset=subset,
+        )
+
+        return ax
+
 
-        hdi = az.hdi(post_pred, .95)
+
+    def plot_predictions(
+            self, 
+            observations,
+            predictions,
+            data_variable: str, 
+            x_dim: str, 
+            ax=None, 
+            subset={},
+            mode="mean+hdi"
+        ):
+        # filter subset coordinates present in data_variable
+        subset = {k: v for k, v in subset.items() if k in observations.coords}
+        
+        # select subset
+        obs = observations.sel(subset)[data_variable]
+        preds = predictions.sel(subset)[f"{data_variable}"]
+        
+        # stack all dims that are not in the time dimension
+        if len(obs.dims) == 1:
+            # add a dummy batch dimension
+            obs = obs.expand_dims("batch")
+            obs = obs.assign_coords(batch=[0])
+
+            preds = preds.expand_dims("batch")
+            preds = preds.assign_coords(batch=[0])
+
+
+        stack_dims = [d for d in obs.dims if d != x_dim]
+        obs = obs.stack(i=stack_dims)
+        preds = preds.stack(i=stack_dims)
+        N = len(obs.coords["i"])
+            
+        hdi = az.hdi(preds, .95)[f"{data_variable}"]
 
         if ax is None:
             ax = plt.subplot(111)
         
-        y_mean = post_pred[data_variable].mean(dim=("chain", "draw"))
-        ax.plot(
-            post_pred[x_dim].values, y_mean.values, 
-            color="black", lw=.8
-        )
+        y_mean = preds.mean(dim=("chain", "draw"))
 
-        ax.fill_between(
-            post_pred[x_dim].values, *hdi[data_variable].values.T, 
-            alpha=.5, color="grey"
-        )
+        for i in obs.i:
+            if obs.sel(i=i).isnull().all():
+                # skip plotting combinations, where all values are NaN
+                continue
+            
+            if mode == "mean+hdi":
+                ax.fill_between(
+                    preds[x_dim].values, *hdi.sel(i=i).values.T, 
+                    alpha=.1, color="black"
+                )
 
-        ax.plot(
-            obs[x_dim].values, obs[data_variable].values, 
-            marker="o", ls="", ms=3
-        )
+
+                ax.plot(
+                    preds[x_dim].values, y_mean.sel(i=i).values, 
+                    alpha=max(1/N, 0.05),
+                    lw=1, color="black"
+                )
+            elif mode == "draws":
+                ys = preds.sel(i=i).stack(sample=("chain", "draw"))
+                ax.plot(
+                    preds[x_dim].values, ys.values, 
+                    alpha=max(1/N, 0.05),
+                    lw=0.5, color="black"
+                )
+            else:
+                raise NotImplementedError(
+                    f"Mode '{mode}' not implemented. "
+                    "Choose 'mean+hdi' or 'draws'."
+                )
+
+            ax.plot(
+                obs[x_dim].values, obs.sel(i=i).values, 
+                marker="o", ls="", ms=3, color="tab:blue"
+            )
         
         ax.set_ylabel(data_variable)
         ax.set_xlabel(x_dim)
 
         return ax
```

### Comparing `pymob-0.3.0a3/pymob/inference/optimization.py` & `pymob-0.3.0a5/pymob/inference/optimization.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/inference/optimize_indy.py` & `pymob-0.3.0a5/pymob/inference/optimize_indy.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/inference/pyabc_backend.py` & `pymob-0.3.0a5/pymob/inference/pyabc_backend.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 import os
+import re
 from functools import lru_cache
 import tempfile
+import inspect
 
 import numpy as np
 import pyabc
 import xarray as xr
 import arviz as az
 from matplotlib import pyplot as plt
 from pathos import multiprocessing as mp
 
 from pymob.simulation import SimulationBase
-
+from pymob.utils.store_file import is_number
 
 class PyabcBackend:
     def __init__(
         self, 
         simulation: SimulationBase
     ):
+        self.parameter_map = {}
+        
         self.simulation = simulation
         self.evaluator = self.model_parser()
         self.prior = self.prior_parser(simulation.free_model_parameters)
         self.distance_function = self.distance_function_parser()
         self.observations = simulation.observations
 
         self.abc = None
         self.history = None
         self.posterior = None
 
+
+    @property
+    def extra_vars(self):
+        extra = self.simulation.config.getlist( 
+            "inference", "extra_vars", fallback=[]
+        )
+        return extra if isinstance(extra, list) else [extra]
+    
+    
     @property
     def sampler(self):
         return self.simulation.config.get("inference.pyabc", "sampler")
     
     @property
     def population_size(self):
         return self.simulation.config.getint("inference.pyabc", "population_size")
@@ -86,55 +99,132 @@
     
     @staticmethod
     def param_to_prior(par):
         parname = par.name
         distribution, cluttered_arguments = par.prior.split("(", 1)
         param_strings = cluttered_arguments.split(")", 1)[0].split(",")
         params = {}
+        arraypattern = r"\[(\d+(\.\d+)?(\s+\d+(\.\d+)?)*|\s*)\]"
+        
         for parstr in param_strings:
-            key, val = parstr.split("=")
-            params.update({key:float(val)})
 
-        return parname, distribution, params
+            key, expression = parstr.split("=")
+            
+            # check if val is a number
+            if is_number(expression):
+                value = float(expression)
+            
+            # check if val is an array
+            elif re.fullmatch(arraypattern, expression):
+                expression = expression.removeprefix("[").removesuffix("]")
+                value = np.array([float(v) for v in expression.split(" ")])
+
+            else:
+                raise NotImplementedError(
+                    f"Prior format {expression} is not implemented. "
+                    "Use e.g."
+                    "\n- normal(loc=1.0,scale=0.5) for 1-dimensional priors, or"
+                    "\n- normal(loc=[1.0 2.4 1],scale=0.5) for n-dimensional priors." 
+                )
 
-    @classmethod
-    def prior_parser(cls, free_model_parameters: list):
+            params.update({key:value})
+
+        return parname, distribution, params
 
+    def prior_parser(self, free_model_parameters: list):
         prior_dict = {}
         for mp in free_model_parameters:
-            name, distribution, params = cls.param_to_prior(par=mp)
+            name, distribution, params = self.param_to_prior(par=mp)
+            pmap, dist_map = self.array_param_to_1d(name, distribution, params)
 
-            prior = pyabc.RV(distribution, **params)
-            prior_dict.update({name: prior})
+            self.parameter_map.update(pmap)
+            for subpar_name, subpar_dist in dist_map.items():
+                prior = pyabc.RV(subpar_dist["dist"], **subpar_dist["params"])
+                prior_dict.update({subpar_name: prior})
 
         return pyabc.Distribution(**prior_dict)
 
+    @staticmethod
+    def map_parameters(theta, parameter_map):
+        theta_mapped = {}
+        for par_name, subpar_name in parameter_map.items():
+            if isinstance(subpar_name, list):
+                subparams = np.array([theta[p] for p in subpar_name])
+            else:
+                subparams = theta[subpar_name]
+            
+            theta_mapped.update({par_name: subparams})
+        return theta_mapped
+
+    @staticmethod
+    def array_param_to_1d(name, distribution, dist_param_dict):
+        # return a distribution if all parameters of the distribution are floats
+        # and map with name
+
+        if np.all([isinstance(v, float) for _, v in dist_param_dict.items()]):
+            return {name:name}, {name: {"dist": distribution, "params": dist_param_dict}}
+        else:
+            args_as_arrays = {k:np.array(v, ndmin=1) for k, v in dist_param_dict.items()}
+            broadcasted_args = np.broadcast_arrays(*tuple(args_as_arrays.values()))
+            # args = {k: v for k, v in zip(dist_param_dict.keys(), broadcasted_args)}
+
+            param_map = {name: []}
+            dist_map = {}
+            for i, args in enumerate(zip(*broadcasted_args)):
+                p_subname = f"{name}_{i}"
+                param_map[name].append(p_subname)
+                dist_kwargs = {
+                    "dist": distribution,
+                    "params": {k:v for k, v in zip(dist_param_dict.keys(), args)}
+                }
+                dist_map.update({p_subname: dist_kwargs})
+
+            return param_map, dist_map
+
+    
     @property
     def plot_function(self):
         return self.simulation.config.get(
             "inference.pyabc", "plot_function", 
             fallback=None
         )
 
     def plot(self):
         plot_func = getattr(self.simulation, self.plot_function)
         plot_func()
         
 
     def model_parser(self):
+        extra_kwargs = {}
+        for extra in self.extra_vars:
+            extra_kwargs.update({extra: self.simulation.observations[extra].values})
+
+        obj_func_signature = inspect.signature(self.simulation.objective_function)
+        obj_func_params = list(obj_func_signature.parameters.keys())
+    
         def model(theta):
-            evaluator = self.simulation.dispatch(theta=dict(theta))
-            evaluator()
-            return {k: np.array(v) for k, v in evaluator.Y.items()}
+            theta_mapped = self.map_parameters(theta, self.parameter_map)
+            evaluator = self.simulation.dispatch(theta=theta_mapped, **extra_kwargs)
+            evaluator(seed=np.random.randint(1e6))
+            res = {k: np.array(v) for k, v in evaluator.Y.items()}
+            res.update({p: theta_mapped[p] for p in obj_func_params if p in theta_mapped})
+            return res
         return model
     
     def distance_function_parser(self):
+        obj_func_signature = inspect.signature(self.simulation.objective_function)
+        obj_func_params = list(obj_func_signature.parameters.keys())
+            
         def distance_function(x, x0):
             Y = {k: v for k, v in x.items() if k in self.simulation.data_variables}
-            obj_name, obj_value = self.simulation.objective_function(results=Y)
+            
+            theta_obj_func = {p: x[p] for p in obj_func_params if p in x}
+            obj_name, obj_value = self.simulation.objective_function(
+                results=Y, **theta_obj_func 
+            )
             return obj_value
         
         return distance_function
 
     def run(self):
         n_cores = self.simulation.n_cores
         print(f"Using {n_cores} CPU cores", flush=True)
```

### Comparing `pymob-0.3.0a3/pymob/inference/pymoo_backend.py` & `pymob-0.3.0a5/pymob/inference/pymoo_backend.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/inference/sbi/plot_posterior_predictions.py` & `pymob-0.3.0a5/pymob/inference/sbi/plot_posterior_predictions.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/inference/sbi/posterior_predictions.py` & `pymob-0.3.0a5/pymob/inference/sbi/posterior_predictions.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/inference/sbi/process_simulations.py` & `pymob-0.3.0a5/pymob/inference/sbi/process_simulations.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/inference/sbi/sbi_backend.py` & `pymob-0.3.0a5/pymob/inference/sbi/sbi_backend.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/inference/sbi/sbi_snle_sample_posterior.py` & `pymob-0.3.0a5/pymob/inference/sbi/sbi_snle_sample_posterior.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/inference/sbi/sbi_utils.py` & `pymob-0.3.0a5/pymob/inference/sbi/sbi_utils.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/inference/sbi/train_network.py` & `pymob-0.3.0a5/pymob/inference/sbi/train_network.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/prior_predictive_checks.py` & `pymob-0.3.0a5/pymob/prior_predictive_checks.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/sim/base.py` & `pymob-0.3.0a5/pymob/sim/base.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/sim/evaluator.py` & `pymob-0.3.0a5/pymob/sim/evaluator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Dict, List
+from typing import Callable, Dict, List, Optional
 import inspect
 import xarray as xr
 import numpy as np
 
 def create_dataset_from_numpy(Y, Y_names, coordinates):
     n_vars = Y.shape[-1]
     n_dims = len(Y.shape)
@@ -23,15 +23,15 @@
     dataset = xr.merge(data_arrays)
 
     return dataset
 
 def create_dataset_from_dict(Y: dict, data_structure, coordinates):
     arrays = {}
     for k, v in Y.items():
-        dims = data_structure[k]
+        dims = data_structure.get(k, tuple(coordinates.keys()))
         coords = {d: coordinates[d] for d in dims}
         da = xr.DataArray(v, coords=coords, dims=dims)
         arrays.update({k: da})
 
     return xr.Dataset(arrays)
 
 class Evaluator:
@@ -48,30 +48,40 @@
 
     def __init__(
             self,
             model: Callable,
             solver: Callable,
             parameters: Dict,
             dimensions: List,
+            n_ode_states: int,
             var_dim_mapper: List,
             data_structure: Dict,
             coordinates: Dict,
             data_variables: List,
             stochastic: bool,
+            indices: Optional[Dict] = {},
+            post_processing: Optional[Callable] = None,
             **kwargs
         ) -> None:
         
         self.model = model
         self.parameters = parameters
         self.dimensions = dimensions
+        self.n_ode_states = n_ode_states
         self.var_dim_mapper = var_dim_mapper
         self.data_structure = data_structure
         self.data_variables = data_variables
         self.coordinates = coordinates
         self.is_stochastic = stochastic
+        self.indices = indices
+        
+        if post_processing is None:
+            self.post_processing = lambda x: x
+        else: 
+            self.post_processing = post_processing
                 
         # set additional arguments of evaluator
         _ = [setattr(self, key, val) for key, val in kwargs.items()]
 
         self._signature = {}
 
         if isinstance(solver, type):
@@ -86,15 +96,15 @@
     def get_call_signature(self):
         signature = inspect.signature(self._solver)
         model_args = list(signature.parameters.keys())
 
         for a in model_args:
             if a not in self.allowed_model_signature_arguments:
                 raise ValueError(
-                    f"{a} in model signature are not attributes of the Evaluator. "
+                    f"'{a}' in model signature is not an attribute of the Evaluator. "
                     f"Use one of {self.allowed_model_signature_arguments}, "
                     f"or set as evaluator_kwargs in the call to "
                     "'SimulationBase.dispatch'" 
                 )
             
             # add argument to signature for call to model
             if a != "seed":
@@ -105,15 +115,17 @@
     def allowed_model_signature_arguments(self):
         return [a for a in self.__dict__.keys() if a[0] != "_"] + ["seed"]
 
     def __call__(self, seed=None):
         if seed is not None:
             self._signature.update({"seed": seed})
 
-        self.Y = self._solver(**self._signature)
+        Y_ = self._solver(**self._signature)
+        Y_ = self.post_processing(Y_)
+        self.Y = Y_
 
     @property
     def dimensionality(self):
         return {key: len(values) for key, values in self.coordinates.items()}
 
     @property
     def results(self):
```

### Comparing `pymob-0.3.0a3/pymob/sim/solvetools.py` & `pymob-0.3.0a5/pymob/sim/solvetools.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/simulate.py` & `pymob-0.3.0a5/pymob/simulate.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/simulation.py` & `pymob-0.3.0a5/pymob/simulation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
+import inspect
 import warnings
 import configparser
 from functools import partial
 import multiprocessing as mp
 from typing import Callable, Dict
 from multiprocessing.pool import ThreadPool, Pool
+import re
 
 import numpy as np
 import xarray as xr
 import dpath.util as dp
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
-from toopy import Param, FloatParam, IntParam
-from toopy import benchmark
+from toopy import param, benchmark
 
 from pymob.utils.errors import errormsg
 from pymob.utils.store_file import scenario_file, parse_config_section
 from pymob.sim.evaluator import Evaluator, create_dataset_from_dict, create_dataset_from_numpy
 
 def update_parameters_dict(config, x, parnames):
     for par, val, in zip(parnames, x):
@@ -23,36 +24,51 @@
         if key_exist != 1:
             raise KeyError(
                 f"prior parameter name: {par} was not found in config. " + 
                 f"make sure parameter name was spelled correctly"
             )
     return config
 
+def get_return_arguments(func):
+    ode_model_source = inspect.getsource(func)
+    
+    # extracts last return statement of source
+    return_statement = ode_model_source.split("\n")[-2]
+
+    # extract arguments returned by ode_func
+    return_args = return_statement.split("return")[1]
+
+    # strip whitespace and separate by comma
+    return_args = return_args.replace(" ", "").split(",")
 
+    return return_args
 
 class SimulationBase:
     model: Callable
     def __init__(
         self, 
         config: configparser.ConfigParser, 
     ) -> None:
         
         self.config = config
         self.model_parameters: Dict = {}
         self.observations = None
         self._objective_names = []
         self._seed_buffer_size = self.n_cores * 2
-        
+        self.indices = {}
+
         # seed gloabal RNG
         self.RNG = np.random.default_rng(self.seed)
         # draw a selection of 1e8 integers for using those throughout the
         # simulation
         self._random_integers = self.create_random_integers(n=self._seed_buffer_size)
 
+     
         self.initialize(input=self.input_file_paths)
+        self.n_ode_states = self.infer_ode_states()
         
         if self.observations is not None:
             self.create_data_scaler()
         
         coords = self.set_coordinates(input=self.input_file_paths)
         self.coordinates = self.create_coordinates(coordinate_data=coords)
         self.var_dim_mapper = self.create_dim_index()
@@ -77,29 +93,50 @@
             print(f"[{section}]", end="\n")
 
             for opt, val in self.config.items(section):
                 print(f"{opt} = {val}", end="\n")
 
         print("========================", end="\n")
 
-    def benchmark(self, n=100):
-        evaluator = self.dispatch(theta=self.model_parameter_dict)
-        evaluator() 
+    def benchmark(self, n=100, **kwargs):
+        evaluator = self.dispatch(theta=self.model_parameter_dict, **kwargs)
+        evaluator(seed=1) 
 
         @benchmark
         def run_bench():
             for i in range(n):
-                evaluator()
+                evaluator(seed=np.random.randint(1e6))
         
         print(f"\nBenchmarking with {n} evaluations")
         print(f"=================================")
         run_bench()
         print(f"=================================\n")
         
+    def infer_ode_states(self):
+        if self.n_ode_states is None:
+            try: 
+                return_args = get_return_arguments(self.model)
+                n_ode_states = len(return_args)
+                warnings.warn(
+                    "The number of ODE states was not specified in "
+                    "the config file [simulation] > 'n_ode_states = <n>'. "
+                    f"Extracted the return arguments {return_args} from the "
+                    "source code. "
+                    f"Setting 'n_ode_states={n_ode_states}."
+                )
+            except:
+                warnings.warn(
+                    "The number of ODE states was not specified in "
+                    "the config file [simulation] > 'n_ode_states = <n>' "
+                    "and could not be extracted from the return arguments."
+                )
+        else:
+            n_ode_states = self.n_ode_states
 
+        return n_ode_states
         
     def dispatch(self, theta, **evaluator_kwargs):
         """Dispatch an evaluator, which will compute the model at parameters
         (theta). Evaluators are advantageous, because they are easier serialized
         than the whole simulation object. Comparison can then happen back in 
         the simulation.
 
@@ -116,28 +153,36 @@
         else:
             solver = self.solver
 
         if hasattr(self.model, "__func__"):
             model = self.model.__func__
         else:
             model = self.model
+        
+        if self.solver_post_processing is not None:
+            post_processing = getattr(self.mod, self.solver_post_processing)
+        else:
+            post_processing = None
 
         stochastic = self.config.get("simulation", "modeltype", fallback=False)
             
         evaluator = Evaluator(
             model=model,
             solver=solver,
             parameters=model_parameters,
             dimensions=self.dimensions,
+            n_ode_states=self.n_ode_states,
             var_dim_mapper=self.var_dim_mapper,
             data_structure=self.data_structure,
             data_variables=self.data_variables,
             coordinates=self.coordinates,
             # TODO: pass the whole simulation settings section
             stochastic=True if stochastic == "stochastic" else False,
+            indices=self.indices,
+            post_processing=post_processing,
             **evaluator_kwargs
         )
 
         return evaluator
 
     def evaluate(self, theta):
         """Wrapper around run to modify paramters of the model.
@@ -176,15 +221,18 @@
             s = widgets.FloatSlider(
                 par.value, description=par.name, min=par.min, max=par.max,
                 step=par.step
             )
             sliders.update({par.name: s})
 
         def func(theta):
-            evaluator = self.dispatch(theta=theta)
+            extra = self.config.getlist("inference", "extra_vars", fallback=[])
+            extra = [extra] if isinstance(extra, str) else extra
+            extra_vars = {v: self.observations[v] for v in extra}
+            evaluator = self.dispatch(theta=theta, **extra_vars)
             evaluator()
             self.plot(results=evaluator.results)
 
         out = interactive_output(func=func, controls=sliders)
 
         display(widgets.HBox([widgets.VBox([s for _, s in sliders.items()]), out]))
     
@@ -348,15 +396,15 @@
         # TODO: run checks if the simulation was set up correctly
         #       - do observation dimensions match the model output (run a mini
         #         simulation with reduced coordinates to verify)
         #       - 
         pass
 
     @staticmethod
-    def parameterize(free_parameters: list[Param], model_parameters) -> dict:
+    def parameterize(free_parameters: list[param.Param], model_parameters) -> dict:
         """
         Optional. Set parameters and initial values of the model. 
         Must return a dictionary with the keys 'y0' and 'parameters'
         
         Can be used to define parameters directly in the script or from a 
         parameter file.
 
@@ -507,14 +555,30 @@
 
     @property
     def data_variables(self):
         data_vars = self.config.getlist("simulation", "data_variables")
         return self.option_as_list(data_vars)
 
     @property
+    def n_ode_states(self):
+        n_ode_states = self.config.getint(
+            "simulation", "n_ode_states", fallback=None
+        )
+
+        return n_ode_states
+    
+    @n_ode_states.setter
+    def n_ode_states(self, n_ode_state):
+        self.config.set("simulation", "n_ode_states", f"{n_ode_state}")
+
+    @property
+    def solver_post_processing(self):
+        return self.config["simulation"].get("solver_post_processing", fallback=None)
+
+    @property
     def input_files(self):
         input_files = self.config.getlist("simulation", "input_files", fallback=[])
         return self.option_as_list(input_files)
   
     @property
     def case_study_path(self):
         return self.config.get("case-study", "package")
@@ -675,26 +739,45 @@
         parameter_dict = {}
         for par_key, par_value in params.items():
             dp.new(parameter_dict, par_key, par_value, separator=".")
 
         # create Param instances
         parameters = []
         for param_name, param_dict in parameter_dict.items():
-            p = FloatParam(
-                value=param_dict.get("value", 1),
-                name=param_name,
-                min=param_dict.get("min", None),
-                max=param_dict.get("max", None),
-                step=param_dict.get("step", None),
-                prior=param_dict.get("prior", None)
-            )
+            value = param_dict.get("value", 1)
+            if isinstance(value, (int, float)):
+                p = param.FloatParam(
+                    value=value,
+                    name=param_name,
+                    min=param_dict.get("min", None),
+                    max=param_dict.get("max", None),
+                    step=param_dict.get("step", None),
+                    prior=param_dict.get("prior", None)
+                )
+            else:
+                # check for array notation
+                pattern = r"(\d+(\.\d+)?(\s+\d+(\.\d+)?)*|\s*)"
+                if re.fullmatch(pattern, value):
+                    value = np.array([float(v) for v in value.split(" ")])
+                    p = param.ArrayParam(
+                        value=value,
+                        name=param_name,
+                        min=param_dict.get("min", None),
+                        max=param_dict.get("max", None),
+                        step=param_dict.get("step", None),
+                        prior=param_dict.get("prior", None)
+                    )
+                else:
+                    raise NotImplementedError(
+                        f"Parameter specification '{value}' cannot be parsed."
+                    )
             parameters.append(p)
 
         return parameters
-        
+
     @property
     def error_model(self):
         em = parse_config_section(self.config["error-model"], method="strfloat")
         return em
 
     @property
     def evaluator_dim_order(self):
```

### Comparing `pymob-0.3.0a3/pymob/utils/bayesian.py` & `pymob-0.3.0a5/pymob/utils/bayesian.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/utils/help.py` & `pymob-0.3.0a5/pymob/utils/help.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/utils/math_helpers.py` & `pymob-0.3.0a5/pymob/utils/math_helpers.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/utils/misc.py` & `pymob-0.3.0a5/pymob/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/utils/plot_helpers.py` & `pymob-0.3.0a5/pymob/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob/utils/store_file.py` & `pymob-0.3.0a5/pymob/utils/store_file.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pymob.egg-info/PKG-INFO` & `pymob-0.3.0a5/pymob.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymob
-Version: 0.3.0a3
+Version: 0.3.0a5
 Summary: Modelling platform for Python
 Author-email: Florian Schunck <fluncki@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Florian
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,15 @@
 Requires-Dist: matplotlib~=3.7.1
 Requires-Dist: numpy~=1.24.0
 Requires-Dist: pandas~=2.0.2
 Requires-Dist: prettytable~=3.7.0
 Requires-Dist: scipy~=1.10.1
 Requires-Dist: scikit-learn~=1.2.2
 Requires-Dist: tqdm~=4.65.0
-Requires-Dist: toopy==0.5.1
+Requires-Dist: toopy==0.6.0
 Requires-Dist: xarray~=2023.11.0
 Requires-Dist: pathos~=0.3.1
 Provides-Extra: dev
 Requires-Dist: pytest>=7.3; extra == "dev"
 Requires-Dist: pyinstrument>=4.5; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
```

### Comparing `pymob-0.3.0a3/pymob.egg-info/SOURCES.txt` & `pymob-0.3.0a5/pymob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/pyproject.toml` & `pymob-0.3.0a5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymob"
-version = "0.3.0a3"
+version = "0.3.0a5"
 authors = [
   { name="Florian Schunck", email="fluncki@protonmail.com" },
 ]
 description = "Modelling platform for Python"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies=[
@@ -18,15 +18,15 @@
   "matplotlib ~= 3.7.1",
   "numpy ~= 1.24.0",
   "pandas ~= 2.0.2",
   "prettytable ~= 3.7.0",
   "scipy ~= 1.10.1",
   "scikit-learn ~= 1.2.2",
   "tqdm ~= 4.65.0",
-  "toopy == 0.5.1",
+  "toopy == 0.6.0",
   "xarray ~= 2023.11.0",
   "pathos ~= 0.3.1",
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
@@ -51,15 +51,15 @@
 dev = ["pytest >= 7.3", "pyinstrument >= 4.5", "bumpver", "sphinx", "myst-parser", "sphinx-book-theme"]
 inference = ["pyabc ~= 0.12.3"]
 numpyro = ["jax ~= 0.4.21", "jaxlib ~= 0.4.21", "sympy ~= 1.12", "sympy2jax ~= 0.0.5", "numpyro ~= 0.13.2", "diffrax ~= 0.4.1"]
 optimize = ["pymoo ~= 0.6.0"]
 interactive = ["ipywidgets ~= 8.1.1", "IPython ~= 8.17.2"]
 
 [tool.bumpver]
-current_version = "0.3.0a3"
+current_version = "0.3.0a5"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
@@ -67,7 +67,10 @@
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"'
 ]
+"pymob/__init__.py" = [
+    '__version__ = "{version}"'
+]
```

### Comparing `pymob-0.3.0a3/tests/test_inference.py` & `pymob-0.3.0a5/tests/test_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,11 +65,8 @@
     
     args = "--case_study=test_case_study --scenario=test_scenario"
     result = runner.invoke(main, args.split(" "))
 
 if __name__ == "__main__":
     import sys
     import os
-    sys.path.append(os.getcwd())
-    test_scripting_api_pyabc()
-    test_inference_evaluation()
-    # test_commandline_API_infer()
+    sys.path.append(os.getcwd())
```

### Comparing `pymob-0.3.0a3/tests/test_sbi.py` & `pymob-0.3.0a5/tests/test_sbi.py`

 * *Files identical despite different names*

### Comparing `pymob-0.3.0a3/tests/test_simulate.py` & `pymob-0.3.0a5/tests/test_simulate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess
+import pytest
 import xarray as xr
 import numpy as np
 from click.testing import CliRunner
 
 from pymob.utils.store_file import prepare_casestudy
 
 def load_test_case_study():
@@ -22,14 +22,17 @@
     ds_ref = xr.load_dataset(f"{sim.data_path}/simulated_data.nc")
 
     np.testing.assert_allclose(
         (ds - ds_ref).to_array().values,
         0
     )
 
+def test_indexing_simulation():
+    pytest.skip()
+
 def test_interactive_mode():
     sim = load_test_case_study()
     sim.interactive()
 
 def test_commandline_API():
     from pymob.simulate import main
     runner = CliRunner()
```

