# Comparing `tmp/epidemik-0.0.21.tar.gz` & `tmp/epidemik-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.21.tar", last modified: Mon Apr 15 23:56:09 2024, max compression
+gzip compressed data, was "epidemik-0.0.22.tar", last modified: Thu May  2 14:33:15 2024, max compression
```

## Comparing `epidemik-0.0.21.tar` & `epidemik-0.0.22.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:56:09.643789 epidemik-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 23:56:05.000000 epidemik-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-15 23:56:09.643789 epidemik-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-15 23:56:05.000000 epidemik-0.0.21/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-15 23:56:05.000000 epidemik-0.0.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:56:09.643789 epidemik-0.0.21/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:56:09.639789 epidemik-0.0.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:56:09.639789 epidemik-0.0.21/src/epidemik/
--rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-04-15 23:56:05.000000 epidemik-0.0.21/src/epidemik/EpiModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-04-15 23:56:05.000000 epidemik-0.0.21/src/epidemik/MetaEpiModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-15 23:56:05.000000 epidemik-0.0.21/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-15 23:56:05.000000 epidemik-0.0.21/src/epidemik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 23:56:05.000000 epidemik-0.0.21/src/epidemik/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:56:09.639789 epidemik-0.0.21/src/epidemik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-15 23:56:09.000000 epidemik-0.0.21/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-15 23:56:09.000000 epidemik-0.0.21/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:56:09.000000 epidemik-0.0.21/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 23:56:09.000000 epidemik-0.0.21/src/epidemik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 23:56:09.000000 epidemik-0.0.21/src/epidemik.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:56:09.639789 epidemik-0.0.21/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-15 23:56:05.000000 epidemik-0.0.21/tests/tests_EpiModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-15 23:56:05.000000 epidemik-0.0.21/tests/tests_MetaEpiModel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:33:15.040119 epidemik-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-02 14:33:05.000000 epidemik-0.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-02 14:33:15.040119 epidemik-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-05-02 14:33:05.000000 epidemik-0.0.22/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-02 14:33:05.000000 epidemik-0.0.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:33:15.040119 epidemik-0.0.22/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:33:15.036119 epidemik-0.0.22/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:33:15.036119 epidemik-0.0.22/src/epidemik/
+-rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-05-02 14:33:05.000000 epidemik-0.0.22/src/epidemik/EpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-05-02 14:33:05.000000 epidemik-0.0.22/src/epidemik/MetaEpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-02 14:33:05.000000 epidemik-0.0.22/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-02 14:33:05.000000 epidemik-0.0.22/src/epidemik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-02 14:33:05.000000 epidemik-0.0.22/src/epidemik/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:33:15.040119 epidemik-0.0.22/src/epidemik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-02 14:33:15.000000 epidemik-0.0.22/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-02 14:33:15.000000 epidemik-0.0.22/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:33:15.000000 epidemik-0.0.22/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 14:33:15.000000 epidemik-0.0.22/src/epidemik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 14:33:15.000000 epidemik-0.0.22/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:33:15.040119 epidemik-0.0.22/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-02 14:33:05.000000 epidemik-0.0.22/tests/tests_EpiModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-02 14:33:05.000000 epidemik-0.0.22/tests/tests_MetaEpiModel.py
```

### Comparing `epidemik-0.0.21/LICENSE` & `epidemik-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.21/PKG-INFO` & `epidemik-0.0.22/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.21
+Version: 0.0.22
 Summary: A package to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Project-URL: Documentation, https://epidemik.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,21 +22,33 @@
 <center>
 <img src="https://raw.githubusercontent.com/DataForScience/epidemik/main/images/epidemik.png" /></center>
 
 # epidemik
 
 Compartmental Epidemic Models in Python
 
+![GitHub Release](https://img.shields.io/github/v/release/DataForScience/epidemik)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/epidemik)
+![GitHub followers](https://img.shields.io/github/followers/DataForScience)
+![GitHub forks](https://img.shields.io/github/forks/DataForScience/epidemik)
+![GitHub Repo stars](https://img.shields.io/github/stars/DataForScience/epidemik)
+![GitHub License](https://img.shields.io/github/license/DataForScience/epidemik)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/m/DataForScience/epidemik)
+![GitHub last commit](https://img.shields.io/github/last-commit/DataForScience/epidemik)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/DataForScience/epidemik)
+
+
 
 ---
 
 ## Table of contents[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#toc)
 - [Installation](#installation)
 - [Tech Stack](#tech)
-- [Usage](#usage)
+- [Basic Usage](#usage)
+- [Documentation](#documentation)
 - [Contributing](#contributing)
 - [License](#license)
 
 ---
 
 ## Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#installation)
 
@@ -63,15 +75,15 @@
 
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
 
 ---
 
 
-## Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#usage)
+## Basic Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#usage)
 
 `epidemik` provides three main modules, `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly from the `epidemik` package using the module name
 
 ```python
 from epidemik import EpiModel
 ```
 
@@ -140,14 +152,23 @@
 
 <img src="https://raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png" />
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
 
 ---
 
+
+## Documentation[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#documentation)
+
+The full documentation for this project is available at ReadTheDocs in [html](https://epidemik.readthedocs.io/), [PDF](https://epidemik.readthedocs.io/_/downloads/en/latest/pdf/) and [ePub](https://epidemik.readthedocs.io/_/downloads/en/latest/epub/) formats.
+
+<div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
+
+---
+
 ## Contributing[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#contributing)
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

#### html2text {}

```diff
@@ -1,38 +1,49 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.21 Summary: A package to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.22 Summary: A package to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues Project-
 URL: Documentation, https://epidemik.readthedocs.io/ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 matplotlib>=3.3 Requires-Dist: networkx>=3 Requires-Dist: numpy>=1.20 Requires-
 Dist: pandas>=2.0 Requires-Dist: scipy>=1.10 Requires-Dist: tqdm>=4
     [https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
                                  epidemik.png]
-# epidemik Compartmental Epidemic Models in Python --- ## Table of contents[![]
-(https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
-pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Usage]
-(#usage) - [Contributing](#contributing) - [License](#license) --- ##
-Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/
-main/images/pin.svg)](#installation) Use the package manager [pip](https://
-pip.pypa.io/en/stable/) to install epidemik. ```bash pip install epidemik ```
+# epidemik Compartmental Epidemic Models in Python ![GitHub Release](https://
+img.shields.io/github/v/release/DataForScience/epidemik) ![PyPI - Downloads]
+(https://img.shields.io/pypi/dm/epidemik) ![GitHub followers](https://
+img.shields.io/github/followers/DataForScience) ![GitHub forks](https://
+img.shields.io/github/forks/DataForScience/epidemik) ![GitHub Repo stars]
+(https://img.shields.io/github/stars/DataForScience/epidemik) ![GitHub License]
+(https://img.shields.io/github/license/DataForScience/epidemik) ![GitHub commit
+activity](https://img.shields.io/github/commit-activity/m/DataForScience/
+epidemik) ![GitHub last commit](https://img.shields.io/github/last-commit/
+DataForScience/epidemik) ![GitHub code size in bytes](https://img.shields.io/
+github/languages/code-size/DataForScience/epidemik) --- ## Table of contents[!
+[](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
+pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Basic
+Usage](#usage) - [Documentation](#documentation) - [Contributing]
+(#contributing) - [License](#license) --- ## Installation[![](https://
+raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)]
+(#installation) Use the package manager [pip](https://pip.pypa.io/en/stable/
+) to install epidemik. ```bash pip install epidemik ```
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Tech Stack[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#tech) Here's a brief high-level overview of the
 tech stack the `epidemik` package uses: - The model is implemented as a
 directed multigraph using [networkx](https://networkx.org/) - Ordinary
 Differential Equations are numerically integrated using [scipy](https://
 scipy.org/) - Random numbers are generated by [numpy](https://numpy.org/) -
 Model structure visualizations rely on [matplotlib](https://matplotlib.org/) -
 Progress bars generated by [tqdm](https://tqdm.github.io/)
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
---- ## Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/
-main/images/pin.svg)](#usage) `epidemik` provides three main modules,
+--- ## Basic Usage[![](https://raw.githubusercontent.com/DataForScience/
+epidemik/main/images/pin.svg)](#usage) `epidemik` provides three main modules,
 `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly
 from the `epidemik` package using the module name ```python from epidemik
 import EpiModel ``` - __EpiModel__ -e Simple compartmental model in a
 homogeneously mixed population. - __NetworkEpiModel__ - Compartmental model on
 a network where nodes interact only along edges connecting them. -
 __MetaEpiModel__ - Meta population model where populations interact with one
 another along the edges of a network. Each sub-population has it's own internal
@@ -53,14 +64,20 @@
 number of time steps to integrate over and the remaining arguments are the
 initial populations of each compartment. ```python N = 10_000 I0 = 10
 SIR.integrate(365, S=N-I0, I=I0, R=0) ``` The results of the integration are
 stored in the `values_` field. A quick visualization of the results can be
 obtained using: ```python SIR.plot() ``` which produces:[https://
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png]
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
+--- ## Documentation[![](https://raw.githubusercontent.com/DataForScience/
+epidemik/main/images/pin.svg)](#documentation) The full documentation for this
+project is available at ReadTheDocs in [html](https://epidemik.readthedocs.io/
+), [PDF](https://epidemik.readthedocs.io/_/downloads/en/latest/pdf/) and [ePub]
+(https://epidemik.readthedocs.io/_/downloads/en/latest/epub/) formats.
+                                                        [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Contributing[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#contributing) Pull requests are welcome. For
 major changes, please open an issue first to discuss what you would like to
 change. Please make sure to update tests as appropriate. Join our project and
 provide assistance by: * Checking out the list of [open issues](https://
 github.com/DataForScience/epidemik/
 issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help. *
```

### Comparing `epidemik-0.0.21/README.md` & `epidemik-0.0.22/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 <center>
 <img src="https://raw.githubusercontent.com/DataForScience/epidemik/main/images/epidemik.png" /></center>
 
 # epidemik
 
 Compartmental Epidemic Models in Python
 
+![GitHub Release](https://img.shields.io/github/v/release/DataForScience/epidemik)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/epidemik)
+![GitHub followers](https://img.shields.io/github/followers/DataForScience)
+![GitHub forks](https://img.shields.io/github/forks/DataForScience/epidemik)
+![GitHub Repo stars](https://img.shields.io/github/stars/DataForScience/epidemik)
+![GitHub License](https://img.shields.io/github/license/DataForScience/epidemik)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/m/DataForScience/epidemik)
+![GitHub last commit](https://img.shields.io/github/last-commit/DataForScience/epidemik)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/DataForScience/epidemik)
+
+
 
 ---
 
 ## Table of contents[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#toc)
 - [Installation](#installation)
 - [Tech Stack](#tech)
-- [Usage](#usage)
+- [Basic Usage](#usage)
+- [Documentation](#documentation)
 - [Contributing](#contributing)
 - [License](#license)
 
 ---
 
 ## Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#installation)
 
@@ -42,15 +54,15 @@
 
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
 
 ---
 
 
-## Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#usage)
+## Basic Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#usage)
 
 `epidemik` provides three main modules, `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly from the `epidemik` package using the module name
 
 ```python
 from epidemik import EpiModel
 ```
 
@@ -119,14 +131,23 @@
 
 <img src="https://raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png" />
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
 
 ---
 
+
+## Documentation[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#documentation)
+
+The full documentation for this project is available at ReadTheDocs in [html](https://epidemik.readthedocs.io/), [PDF](https://epidemik.readthedocs.io/_/downloads/en/latest/pdf/) and [ePub](https://epidemik.readthedocs.io/_/downloads/en/latest/epub/) formats.
+
+<div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
+
+---
+
 ## Contributing[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#contributing)
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

#### html2text {}

```diff
@@ -1,28 +1,39 @@
     [https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
                                  epidemik.png]
-# epidemik Compartmental Epidemic Models in Python --- ## Table of contents[![]
-(https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
-pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Usage]
-(#usage) - [Contributing](#contributing) - [License](#license) --- ##
-Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/
-main/images/pin.svg)](#installation) Use the package manager [pip](https://
-pip.pypa.io/en/stable/) to install epidemik. ```bash pip install epidemik ```
+# epidemik Compartmental Epidemic Models in Python ![GitHub Release](https://
+img.shields.io/github/v/release/DataForScience/epidemik) ![PyPI - Downloads]
+(https://img.shields.io/pypi/dm/epidemik) ![GitHub followers](https://
+img.shields.io/github/followers/DataForScience) ![GitHub forks](https://
+img.shields.io/github/forks/DataForScience/epidemik) ![GitHub Repo stars]
+(https://img.shields.io/github/stars/DataForScience/epidemik) ![GitHub License]
+(https://img.shields.io/github/license/DataForScience/epidemik) ![GitHub commit
+activity](https://img.shields.io/github/commit-activity/m/DataForScience/
+epidemik) ![GitHub last commit](https://img.shields.io/github/last-commit/
+DataForScience/epidemik) ![GitHub code size in bytes](https://img.shields.io/
+github/languages/code-size/DataForScience/epidemik) --- ## Table of contents[!
+[](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
+pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Basic
+Usage](#usage) - [Documentation](#documentation) - [Contributing]
+(#contributing) - [License](#license) --- ## Installation[![](https://
+raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)]
+(#installation) Use the package manager [pip](https://pip.pypa.io/en/stable/
+) to install epidemik. ```bash pip install epidemik ```
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Tech Stack[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#tech) Here's a brief high-level overview of the
 tech stack the `epidemik` package uses: - The model is implemented as a
 directed multigraph using [networkx](https://networkx.org/) - Ordinary
 Differential Equations are numerically integrated using [scipy](https://
 scipy.org/) - Random numbers are generated by [numpy](https://numpy.org/) -
 Model structure visualizations rely on [matplotlib](https://matplotlib.org/) -
 Progress bars generated by [tqdm](https://tqdm.github.io/)
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
---- ## Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/
-main/images/pin.svg)](#usage) `epidemik` provides three main modules,
+--- ## Basic Usage[![](https://raw.githubusercontent.com/DataForScience/
+epidemik/main/images/pin.svg)](#usage) `epidemik` provides three main modules,
 `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly
 from the `epidemik` package using the module name ```python from epidemik
 import EpiModel ``` - __EpiModel__ -e Simple compartmental model in a
 homogeneously mixed population. - __NetworkEpiModel__ - Compartmental model on
 a network where nodes interact only along edges connecting them. -
 __MetaEpiModel__ - Meta population model where populations interact with one
 another along the edges of a network. Each sub-population has it's own internal
@@ -43,14 +54,20 @@
 number of time steps to integrate over and the remaining arguments are the
 initial populations of each compartment. ```python N = 10_000 I0 = 10
 SIR.integrate(365, S=N-I0, I=I0, R=0) ``` The results of the integration are
 stored in the `values_` field. A quick visualization of the results can be
 obtained using: ```python SIR.plot() ``` which produces:[https://
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png]
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
+--- ## Documentation[![](https://raw.githubusercontent.com/DataForScience/
+epidemik/main/images/pin.svg)](#documentation) The full documentation for this
+project is available at ReadTheDocs in [html](https://epidemik.readthedocs.io/
+), [PDF](https://epidemik.readthedocs.io/_/downloads/en/latest/pdf/) and [ePub]
+(https://epidemik.readthedocs.io/_/downloads/en/latest/epub/) formats.
+                                                        [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Contributing[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#contributing) Pull requests are welcome. For
 major changes, please open an issue first to discuss what you would like to
 change. Please make sure to update tests as appropriate. Join our project and
 provide assistance by: * Checking out the list of [open issues](https://
 github.com/DataForScience/epidemik/
 issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help. *
```

### Comparing `epidemik-0.0.21/pyproject.toml` & `epidemik-0.0.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.21/src/epidemik/EpiModel.py` & `epidemik-0.0.22/src/epidemik/EpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.21/src/epidemik/MetaEpiModel.py` & `epidemik-0.0.22/src/epidemik/MetaEpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.21/src/epidemik/NetworkEpiModel.py` & `epidemik-0.0.22/src/epidemik/NetworkEpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.21/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.22/src/epidemik.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.21
+Version: 0.0.22
 Summary: A package to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Project-URL: Documentation, https://epidemik.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,21 +22,33 @@
 <center>
 <img src="https://raw.githubusercontent.com/DataForScience/epidemik/main/images/epidemik.png" /></center>
 
 # epidemik
 
 Compartmental Epidemic Models in Python
 
+![GitHub Release](https://img.shields.io/github/v/release/DataForScience/epidemik)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/epidemik)
+![GitHub followers](https://img.shields.io/github/followers/DataForScience)
+![GitHub forks](https://img.shields.io/github/forks/DataForScience/epidemik)
+![GitHub Repo stars](https://img.shields.io/github/stars/DataForScience/epidemik)
+![GitHub License](https://img.shields.io/github/license/DataForScience/epidemik)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/m/DataForScience/epidemik)
+![GitHub last commit](https://img.shields.io/github/last-commit/DataForScience/epidemik)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/DataForScience/epidemik)
+
+
 
 ---
 
 ## Table of contents[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#toc)
 - [Installation](#installation)
 - [Tech Stack](#tech)
-- [Usage](#usage)
+- [Basic Usage](#usage)
+- [Documentation](#documentation)
 - [Contributing](#contributing)
 - [License](#license)
 
 ---
 
 ## Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#installation)
 
@@ -63,15 +75,15 @@
 
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
 
 ---
 
 
-## Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#usage)
+## Basic Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#usage)
 
 `epidemik` provides three main modules, `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly from the `epidemik` package using the module name
 
 ```python
 from epidemik import EpiModel
 ```
 
@@ -140,14 +152,23 @@
 
 <img src="https://raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png" />
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
 
 ---
 
+
+## Documentation[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#documentation)
+
+The full documentation for this project is available at ReadTheDocs in [html](https://epidemik.readthedocs.io/), [PDF](https://epidemik.readthedocs.io/_/downloads/en/latest/pdf/) and [ePub](https://epidemik.readthedocs.io/_/downloads/en/latest/epub/) formats.
+
+<div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
+
+---
+
 ## Contributing[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#contributing)
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

#### html2text {}

```diff
@@ -1,38 +1,49 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.21 Summary: A package to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.22 Summary: A package to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues Project-
 URL: Documentation, https://epidemik.readthedocs.io/ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 matplotlib>=3.3 Requires-Dist: networkx>=3 Requires-Dist: numpy>=1.20 Requires-
 Dist: pandas>=2.0 Requires-Dist: scipy>=1.10 Requires-Dist: tqdm>=4
     [https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
                                  epidemik.png]
-# epidemik Compartmental Epidemic Models in Python --- ## Table of contents[![]
-(https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
-pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Usage]
-(#usage) - [Contributing](#contributing) - [License](#license) --- ##
-Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/
-main/images/pin.svg)](#installation) Use the package manager [pip](https://
-pip.pypa.io/en/stable/) to install epidemik. ```bash pip install epidemik ```
+# epidemik Compartmental Epidemic Models in Python ![GitHub Release](https://
+img.shields.io/github/v/release/DataForScience/epidemik) ![PyPI - Downloads]
+(https://img.shields.io/pypi/dm/epidemik) ![GitHub followers](https://
+img.shields.io/github/followers/DataForScience) ![GitHub forks](https://
+img.shields.io/github/forks/DataForScience/epidemik) ![GitHub Repo stars]
+(https://img.shields.io/github/stars/DataForScience/epidemik) ![GitHub License]
+(https://img.shields.io/github/license/DataForScience/epidemik) ![GitHub commit
+activity](https://img.shields.io/github/commit-activity/m/DataForScience/
+epidemik) ![GitHub last commit](https://img.shields.io/github/last-commit/
+DataForScience/epidemik) ![GitHub code size in bytes](https://img.shields.io/
+github/languages/code-size/DataForScience/epidemik) --- ## Table of contents[!
+[](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
+pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Basic
+Usage](#usage) - [Documentation](#documentation) - [Contributing]
+(#contributing) - [License](#license) --- ## Installation[![](https://
+raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)]
+(#installation) Use the package manager [pip](https://pip.pypa.io/en/stable/
+) to install epidemik. ```bash pip install epidemik ```
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Tech Stack[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#tech) Here's a brief high-level overview of the
 tech stack the `epidemik` package uses: - The model is implemented as a
 directed multigraph using [networkx](https://networkx.org/) - Ordinary
 Differential Equations are numerically integrated using [scipy](https://
 scipy.org/) - Random numbers are generated by [numpy](https://numpy.org/) -
 Model structure visualizations rely on [matplotlib](https://matplotlib.org/) -
 Progress bars generated by [tqdm](https://tqdm.github.io/)
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
---- ## Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/
-main/images/pin.svg)](#usage) `epidemik` provides three main modules,
+--- ## Basic Usage[![](https://raw.githubusercontent.com/DataForScience/
+epidemik/main/images/pin.svg)](#usage) `epidemik` provides three main modules,
 `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly
 from the `epidemik` package using the module name ```python from epidemik
 import EpiModel ``` - __EpiModel__ -e Simple compartmental model in a
 homogeneously mixed population. - __NetworkEpiModel__ - Compartmental model on
 a network where nodes interact only along edges connecting them. -
 __MetaEpiModel__ - Meta population model where populations interact with one
 another along the edges of a network. Each sub-population has it's own internal
@@ -53,14 +64,20 @@
 number of time steps to integrate over and the remaining arguments are the
 initial populations of each compartment. ```python N = 10_000 I0 = 10
 SIR.integrate(365, S=N-I0, I=I0, R=0) ``` The results of the integration are
 stored in the `values_` field. A quick visualization of the results can be
 obtained using: ```python SIR.plot() ``` which produces:[https://
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png]
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
+--- ## Documentation[![](https://raw.githubusercontent.com/DataForScience/
+epidemik/main/images/pin.svg)](#documentation) The full documentation for this
+project is available at ReadTheDocs in [html](https://epidemik.readthedocs.io/
+), [PDF](https://epidemik.readthedocs.io/_/downloads/en/latest/pdf/) and [ePub]
+(https://epidemik.readthedocs.io/_/downloads/en/latest/epub/) formats.
+                                                        [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Contributing[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#contributing) Pull requests are welcome. For
 major changes, please open an issue first to discuss what you would like to
 change. Please make sure to update tests as appropriate. Join our project and
 provide assistance by: * Checking out the list of [open issues](https://
 github.com/DataForScience/epidemik/
 issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help. *
```

### Comparing `epidemik-0.0.21/tests/tests_EpiModel.py` & `epidemik-0.0.22/tests/tests_EpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.21/tests/tests_MetaEpiModel.py` & `epidemik-0.0.22/tests/tests_MetaEpiModel.py`

 * *Files identical despite different names*

