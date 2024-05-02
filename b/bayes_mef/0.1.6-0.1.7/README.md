# Comparing `tmp/bayes_mef-0.1.6.tar.gz` & `tmp/bayes_mef-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayes_mef-0.1.6.tar", max compression
+gzip compressed data, was "bayes_mef-0.1.7.tar", max compression
```

## Comparing `bayes_mef-0.1.6.tar` & `bayes_mef-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1513 2024-03-12 13:36:09.991705 bayes_mef-0.1.6/LICENSE
--rw-r--r--   0        0        0     5164 2024-03-24 07:46:37.541749 bayes_mef-0.1.6/README.md
--rw-r--r--   0        0        0       84 2024-03-22 16:24:29.359488 bayes_mef-0.1.6/bayes_mef/__init__.py
--rw-r--r--   0        0        0    13492 2024-03-19 16:50:03.612414 bayes_mef-0.1.6/bayes_mef/algos.py
--rw-r--r--   0        0        0    11571 2024-03-12 13:36:09.991705 bayes_mef-0.1.6/bayes_mef/mef_launcher.py
--rw-r--r--   0        0        0     3130 2024-03-25 15:03:38.694715 bayes_mef-0.1.6/bayes_mef/utils.py
--rw-r--r--   0        0        0      635 2024-03-25 15:03:55.102810 bayes_mef-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6125 1970-01-01 00:00:00.000000 bayes_mef-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1513 2024-03-12 13:36:09.991705 bayes_mef-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5144 2024-04-16 09:55:40.631133 bayes_mef-0.1.7/README.md
+-rw-r--r--   0        0        0       84 2024-03-22 16:24:29.359488 bayes_mef-0.1.7/bayes_mef/__init__.py
+-rw-r--r--   0        0        0    13492 2024-03-19 16:50:03.612414 bayes_mef-0.1.7/bayes_mef/algos.py
+-rw-r--r--   0        0        0    11571 2024-03-12 13:36:09.991705 bayes_mef-0.1.7/bayes_mef/mef_launcher.py
+-rw-r--r--   0        0        0     3130 2024-03-25 15:03:38.694715 bayes_mef-0.1.7/bayes_mef/utils.py
+-rw-r--r--   0        0        0      635 2024-05-02 09:46:50.187653 bayes_mef-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6105 1970-01-01 00:00:00.000000 bayes_mef-0.1.7/PKG-INFO
```

### Comparing `bayes_mef-0.1.6/LICENSE` & `bayes_mef-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bayes_mef-0.1.6/README.md` & `bayes_mef-0.1.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Bayesian MEF
 [![PyPI](https://img.shields.io/pypi/v/bayes_mef)](https://pypi.org/project/bayes_mef/)
 ![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10809893.svg)](https://doi.org/10.5281/zenodo.10809893)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-purple.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-Bayesian multi-exposure image fusion (MEF) is a general-purpose algorithm to achieve robust high dynamic range (HDR) imaging, particularly in scenarios with low signal-to-noise ratio (SNR) or variations in illumination intensity. This approach is especially crucial for high quality phase retrieval in coherent diffractive imaging (CDI). The algorithm, detailed in the [arXiv preprint](https://arxiv.org/abs/2403.11344), primarily focuses on its implementation and demonstrates the benefits in ptychography. 
+Bayesian multi-exposure image fusion (MEF) is a general-purpose algorithm to achieve robust high dynamic range (HDR) imaging, particularly in scenarios with low signal-to-noise ratio (SNR) or variations in illumination intensity. This approach is especially crucial for high quality phase retrieval in coherent diffractive imaging (CDI). The algorithm, detailed in the [arXiv preprint](https://arxiv.org/abs/2403.11344), primarily focuses on its implementation and demonstrates the benefits in ptychography. To reproduce the results in the paper, see this [section](#reproducing-results). However, to get started, please install the package and check the demo usage below.
 
 ![demo_mef](https://github.com/microscopic-image-analysis/bayes-mef/assets/64919085/d00a8c5e-5e53-4b7e-856b-381cc99523ba)
 
-To install the package and its dependencies, 
+To install this package from PyPI, 
 ```bash
 pip install bayes_mef
 ```
 
 ## Usage
 
 A minimal example demonstrating the usage of `BayesianMEF` by simulating some data.
@@ -69,33 +69,37 @@
 n_cpus = 20
 n_iter = 150
 fused_ptyem_stack, em_flux_factors = launch_mef.run_em(n_iter, n_cpus)
 ```
 
 For a detailed usage, please check [synthetic_mef.py](scripts/synthetic_mef.py) that uses synthetic ptychography data.
 
-## Publication results
+## Reproducing results
 
-Ptychography data used for the publication results can be found at [Zenodo](https://doi.org/10.5281/zenodo.10809893). It also includes the code which is in this repository. Therefore, to replicate the publication results, please follow the below steps:
-1. Download and unzip the dataset and the code from [Zenodo](https://doi.org/10.5281/zenodo.10809893).
-2. Create a virtual environment and install the dependencies as
-   
+To reproduce the ptychographic reconstruction results from the paper, please follow the below steps:
+
+1. Please clone this repository and create a conda environment.
    ```bash
+   git clone https://github.com/microscopic-image-analysis/bayes-mef.git
    cd bayes-mef
-   conda create --name bayes-mef-venv python=3.10.13 # or python version satisfying ">=3.9, <3.12" 
+   conda create --name bayes-mef-venv python=3.11.5 
+   ```
+2. Now activate the environment and install the *pinned* dependencies.
+   ```bash
    conda activate bayes-mef-venv
-   pip install -e .
+   pip install -r requirements.txt
    ```
-3. An additional dependency of `ptylab` is required for processing ptychography data
-   
+3. Download the data from [Zenodo](https://zenodo.org/doi/10.5281/zenodo.10964222) with the following command:
    ```bash
-   pip install git+https://github.com/PtyLab/PtyLab.py.git@main
+   ./download_data.sh
    ```
-4. Please run python scripts under [scripts/](scripts) directory to replicate results in the publication.
-5. Optional: For faster ptychographic reconstructions using GPU, please install `cupy` as given under its [installation guide](https://docs.cupy.dev/en/stable/install.html).
+
+4. Optional: For faster ptychographic reconstructions using GPU, please install `cupy` as given under its [installation guide](https://docs.cupy.dev/en/stable/install.html).
+
+5. Run files from the [scripts/](scripts) directory for plotting the results.
 
 ## Citation
 If you found this algorithm or the publication useful, please cite us at:
 ```tex
 @misc{Kodgirwar:24,
       title={Bayesian multi-exposure image fusion for robust high dynamic range ptychography}, 
       author={Shantanu Kodgirwar and Lars Loetgering and Chang Liu and Aleena Joseph and Leona Licht
```

### Comparing `bayes_mef-0.1.6/bayes_mef/algos.py` & `bayes_mef-0.1.7/bayes_mef/algos.py`

 * *Files identical despite different names*

### Comparing `bayes_mef-0.1.6/bayes_mef/mef_launcher.py` & `bayes_mef-0.1.7/bayes_mef/mef_launcher.py`

 * *Files identical despite different names*

### Comparing `bayes_mef-0.1.6/bayes_mef/utils.py` & `bayes_mef-0.1.7/bayes_mef/utils.py`

 * *Files identical despite different names*

### Comparing `bayes_mef-0.1.6/pyproject.toml` & `bayes_mef-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bayes_mef"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python implementation of the Bayesian MEF method"
 authors = ["Shantanu Kodgirwar <shantanu.kodgirwar@uni-jena.de>", "Michael Habeck <michael.habeck@uni-jena.de>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/microscopic-image-analysis/bayes-mef"
 
 [tool.poetry.dependencies]
```

### Comparing `bayes_mef-0.1.6/PKG-INFO` & `bayes_mef-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayes_mef
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python implementation of the Bayesian MEF method
 Home-page: https://github.com/microscopic-image-analysis/bayes-mef
 License: BSD-3-Clause
 Author: Shantanu Kodgirwar
 Author-email: shantanu.kodgirwar@uni-jena.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: BSD License
@@ -24,19 +24,19 @@
 
 # Bayesian MEF
 [![PyPI](https://img.shields.io/pypi/v/bayes_mef)](https://pypi.org/project/bayes_mef/)
 ![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10809893.svg)](https://doi.org/10.5281/zenodo.10809893)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-purple.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-Bayesian multi-exposure image fusion (MEF) is a general-purpose algorithm to achieve robust high dynamic range (HDR) imaging, particularly in scenarios with low signal-to-noise ratio (SNR) or variations in illumination intensity. This approach is especially crucial for high quality phase retrieval in coherent diffractive imaging (CDI). The algorithm, detailed in the [arXiv preprint](https://arxiv.org/abs/2403.11344), primarily focuses on its implementation and demonstrates the benefits in ptychography. 
+Bayesian multi-exposure image fusion (MEF) is a general-purpose algorithm to achieve robust high dynamic range (HDR) imaging, particularly in scenarios with low signal-to-noise ratio (SNR) or variations in illumination intensity. This approach is especially crucial for high quality phase retrieval in coherent diffractive imaging (CDI). The algorithm, detailed in the [arXiv preprint](https://arxiv.org/abs/2403.11344), primarily focuses on its implementation and demonstrates the benefits in ptychography. To reproduce the results in the paper, see this [section](#reproducing-results). However, to get started, please install the package and check the demo usage below.
 
 ![demo_mef](https://github.com/microscopic-image-analysis/bayes-mef/assets/64919085/d00a8c5e-5e53-4b7e-856b-381cc99523ba)
 
-To install the package and its dependencies, 
+To install this package from PyPI, 
 ```bash
 pip install bayes_mef
 ```
 
 ## Usage
 
 A minimal example demonstrating the usage of `BayesianMEF` by simulating some data.
@@ -93,33 +93,37 @@
 n_cpus = 20
 n_iter = 150
 fused_ptyem_stack, em_flux_factors = launch_mef.run_em(n_iter, n_cpus)
 ```
 
 For a detailed usage, please check [synthetic_mef.py](scripts/synthetic_mef.py) that uses synthetic ptychography data.
 
-## Publication results
+## Reproducing results
 
-Ptychography data used for the publication results can be found at [Zenodo](https://doi.org/10.5281/zenodo.10809893). It also includes the code which is in this repository. Therefore, to replicate the publication results, please follow the below steps:
-1. Download and unzip the dataset and the code from [Zenodo](https://doi.org/10.5281/zenodo.10809893).
-2. Create a virtual environment and install the dependencies as
-   
+To reproduce the ptychographic reconstruction results from the paper, please follow the below steps:
+
+1. Please clone this repository and create a conda environment.
    ```bash
+   git clone https://github.com/microscopic-image-analysis/bayes-mef.git
    cd bayes-mef
-   conda create --name bayes-mef-venv python=3.10.13 # or python version satisfying ">=3.9, <3.12" 
+   conda create --name bayes-mef-venv python=3.11.5 
+   ```
+2. Now activate the environment and install the *pinned* dependencies.
+   ```bash
    conda activate bayes-mef-venv
-   pip install -e .
+   pip install -r requirements.txt
    ```
-3. An additional dependency of `ptylab` is required for processing ptychography data
-   
+3. Download the data from [Zenodo](https://zenodo.org/doi/10.5281/zenodo.10964222) with the following command:
    ```bash
-   pip install git+https://github.com/PtyLab/PtyLab.py.git@main
+   ./download_data.sh
    ```
-4. Please run python scripts under [scripts/](scripts) directory to replicate results in the publication.
-5. Optional: For faster ptychographic reconstructions using GPU, please install `cupy` as given under its [installation guide](https://docs.cupy.dev/en/stable/install.html).
+
+4. Optional: For faster ptychographic reconstructions using GPU, please install `cupy` as given under its [installation guide](https://docs.cupy.dev/en/stable/install.html).
+
+5. Run files from the [scripts/](scripts) directory for plotting the results.
 
 ## Citation
 If you found this algorithm or the publication useful, please cite us at:
 ```tex
 @misc{Kodgirwar:24,
       title={Bayesian multi-exposure image fusion for robust high dynamic range ptychography}, 
       author={Shantanu Kodgirwar and Lars Loetgering and Chang Liu and Aleena Joseph and Leona Licht
```

