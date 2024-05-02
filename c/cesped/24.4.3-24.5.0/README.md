# Comparing `tmp/cesped-24.4.3.tar.gz` & `tmp/cesped-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesped-24.4.3.tar", last modified: Sat Apr 20 13:57:14 2024, max compression
+gzip compressed data, was "cesped-24.5.0.tar", last modified: Thu May  2 00:12:20 2024, max compression
```

## Comparing `cesped-24.4.3.tar` & `cesped-24.5.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.107537 cesped-24.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-20 13:46:10.000000 cesped-24.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-20 13:46:10.000000 cesped-24.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-04-20 13:57:14.107537 cesped-24.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-20 13:46:10.000000 cesped-24.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.099537 cesped-24.4.3/cesped/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.103537 cesped-24.4.3/cesped/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultDataAugmentation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultDataConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultInferenceConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultModelConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultOptimizerConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultRelionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/configs/defaultTrainerConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.103537 cesped-24.4.3/cesped/datamanager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/datamanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/datamanager/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/datamanager/ctf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/datamanager/plDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    22286 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/evaluateEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/inferEntry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.103537 cesped-24.4.3/cesped/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/network/featureExtractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/network/image2sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/network/plModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    28525 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/particlesDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/trainEntry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.107537 cesped-24.4.3/cesped/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/angles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/anglesStats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/cliBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/fsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/gaussianFilters.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/tensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/utils/volumeStats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.107537 cesped-24.4.3/cesped/zenodo/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/zenodo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/zenodo/bechmarkUrls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/zenodo/downloadFromZenodo.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/zenodo/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-20 13:46:10.000000 cesped-24.4.3/cesped/zenodo/uploadToZenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.107537 cesped-24.4.3/cesped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-04-20 13:57:14.000000 cesped-24.4.3/cesped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-20 13:57:14.000000 cesped-24.4.3/cesped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:57:14.000000 cesped-24.4.3/cesped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-20 13:57:14.000000 cesped-24.4.3/cesped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 13:57:14.000000 cesped-24.4.3/cesped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-20 13:46:10.000000 cesped-24.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:57:14.107537 cesped-24.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-20 13:46:10.000000 cesped-24.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:57:14.107537 cesped-24.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 13:46:10.000000 cesped-24.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-20 13:46:10.000000 cesped-24.4.3/tests/test_anglesStats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-20 13:46:10.000000 cesped-24.4.3/tests/test_particlesDataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.241055 cesped-24.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-02 00:05:43.000000 cesped-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 00:05:43.000000 cesped-24.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-02 00:12:20.241055 cesped-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-05-02 00:05:43.000000 cesped-24.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.233055 cesped-24.5.0/cesped/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.233055 cesped-24.5.0/cesped/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultDataAugmentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultDataConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultInferenceConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultModelConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultOptimizerConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultRelionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultTrainerConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/cesped/datamanager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/datamanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/datamanager/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/datamanager/ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/datamanager/plDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22438 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/evaluateEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/inferEntry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/cesped/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/network/featureExtractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/network/image2sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/network/plModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28525 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/particlesDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/trainEntry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/cesped/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/angles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/anglesStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/cliBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/fsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/gaussianFilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/tensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/volumeStats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/cesped/zenodo/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/zenodo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/zenodo/bechmarkUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/zenodo/downloadFromZenodo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/zenodo/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/zenodo/uploadToZenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/cesped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-02 00:12:20.000000 cesped-24.5.0/cesped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-02 00:12:20.000000 cesped-24.5.0/cesped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:12:20.000000 cesped-24.5.0/cesped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-02 00:12:20.000000 cesped-24.5.0/cesped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 00:12:20.000000 cesped-24.5.0/cesped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-02 00:05:43.000000 cesped-24.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:12:20.241055 cesped-24.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-02 00:05:43.000000 cesped-24.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:05:43.000000 cesped-24.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-02 00:05:43.000000 cesped-24.5.0/tests/test_anglesStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-02 00:05:43.000000 cesped-24.5.0/tests/test_particlesDataset.py
```

### Comparing `cesped-24.4.3/LICENSE` & `cesped-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/PKG-INFO` & `cesped-24.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesped
-Version: 24.4.3
+Version: 24.5.0
 Summary: Code utilities for the CESPED (Cryo-EM Supervised Pose Estimation Dataset) benchmark
 Home-page: https://github.com/rsanchezgarc/cesped
 Author: Ruben Sanchez-Garcia
 Author-email: ruben.sanchez-garcia@stats.ox.ac.uk
 Keywords: deep learning cryoem pose estimation
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,15 +25,15 @@
 Requires-Dist: starstack>=0.2.0
 Requires-Dist: tensorboard>=2.12.1
 Requires-Dist: torch<3.0.0,>=2.0.0
 Requires-Dist: torchvision>=0.15.2
 
 # CESPED: Utilities for the Cryo-EM Supervised Pose Estimation Dataset
 
-CESPED, is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check our manuscript at https://arxiv.org/abs/2311.06194.
+CESPED is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check our manuscript at https://arxiv.org/abs/2311.06194.
 
 ## Installation
 cesped has been tested on python 3.11. Installation should be automatic using pip
 ```
 pip install cesped
 #Or directy from the master branch
 pip install git+https://github.com/rsanchezgarc/cesped
@@ -133,17 +133,21 @@
 python -m cesped.particlesDataset download_entry -t 10166 --halfset 0
 ```
 This will download the associated starfile and mrcs file to the default benchmark directory (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml).
 Use `--benchmarkDir` to specify another directory<br/>
 
 In order to list the entries available for download and the ones already downloaded, you can use
 ```
-python -m cesped.particlesDataset preprocess_entry --t 10166 --halfset 0--o /tmp/dumpedData/ --ctf_correction "phase_flip"
+python -m cesped.particlesDataset list_entries
 ```
-use `-h` to display the list of available preprocessing operations.
+Preprocessing of the dataset entries can be executed using
+```
+python -m cesped.particlesDataset preprocess_entry --t 10166 --halfset 0 --o /tmp/dumpedData/ --ctf_correction "phase_flip"
+```
+where `--t` is the target name. Use `-h` to display the list of available preprocessing operations.
 
 The raw data can be easily accessed using the Python package [starstack](https://pypi.org/project/starstack/), which relies on the [mrcfile](https://pypi.org/project/mrcfile/) and [starfile](https://pypi.org/project/starfile/) packages. Predictions should be written as a star file with the newly
 predicted Euler angles.
 
 Evaluation can be computed once the predictions for the half-set 0 and half-set 1 are saved
 
 ```
@@ -175,15 +179,15 @@
 
 | EMPIAR ID | Composition | Symmetry | Image Pixels | FSCR<sub>0.143</sub> (Å) | Masked FSCR<sub>0.143</sub> (Å) | # Particles |
 |-----------|-------------|----------|--------------|-------------------------|---------------------------------|-------------|
 | 10166     | Human 26S proteasome bound to the chemotherapeutic Oprozomib | C1 | 284 | 5.0 | 3.9 | 238631 |
 | 10786     | Substance P-Neurokinin Receptor G protein complexes (SP-NK1R-miniGs399) | C1 | 184 | 3.3 | 3.0* | 288659 |
 | 10280     | Calcium-bound TMEM16F in nanodisc with supplement of PIP2 | C2 | 182 | 3.6 | 3.0* | 459504 |
 | 11120     | M22 bound TSHR Gs 7TM G protein | C1 | 232 | 3.4 | 3.0* | 244973 |
-| 10647     | PKM2 in complex with L-threonine | D2 | 222 | 3.7 | 3.3 | 234956 |
+| 10648     | PKM2 in complex with Compound 5 | D2 | 222 | 3.7 | 3.3 | 234956 |
 | 10409     | Replicating SARS-CoV-2 polymerase (Map 1) | C1 | 240 | 3.3 | 3.0* | 406001 |
 | 10374     | Human ABCG2 transporter with inhibitor MZ29 and 5D3-Fab | C2 | 216 | 3.7 | 3.0* | 323681 |
 
 `*` Nyquist Frequency at 1.5 Å/pixel; Resolution is estimated at the usual threshold 0.143.  
 Reported FSCR<sub>0.143</sub> values were obtained directly from the relion_refine logs while Masked FSCR<sub>0.143</sub> values were collected from the relion_postprocess logs.
 
 In addition, the entry TEST is a small subset of EMPIAR-11120
```

### Comparing `cesped-24.4.3/README.md` & `cesped-24.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # CESPED: Utilities for the Cryo-EM Supervised Pose Estimation Dataset
 
-CESPED, is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check our manuscript at https://arxiv.org/abs/2311.06194.
+CESPED is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check our manuscript at https://arxiv.org/abs/2311.06194.
 
 ## Installation
 cesped has been tested on python 3.11. Installation should be automatic using pip
 ```
 pip install cesped
 #Or directy from the master branch
 pip install git+https://github.com/rsanchezgarc/cesped
@@ -104,17 +104,21 @@
 python -m cesped.particlesDataset download_entry -t 10166 --halfset 0
 ```
 This will download the associated starfile and mrcs file to the default benchmark directory (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml).
 Use `--benchmarkDir` to specify another directory<br/>
 
 In order to list the entries available for download and the ones already downloaded, you can use
 ```
-python -m cesped.particlesDataset preprocess_entry --t 10166 --halfset 0--o /tmp/dumpedData/ --ctf_correction "phase_flip"
+python -m cesped.particlesDataset list_entries
 ```
-use `-h` to display the list of available preprocessing operations.
+Preprocessing of the dataset entries can be executed using
+```
+python -m cesped.particlesDataset preprocess_entry --t 10166 --halfset 0 --o /tmp/dumpedData/ --ctf_correction "phase_flip"
+```
+where `--t` is the target name. Use `-h` to display the list of available preprocessing operations.
 
 The raw data can be easily accessed using the Python package [starstack](https://pypi.org/project/starstack/), which relies on the [mrcfile](https://pypi.org/project/mrcfile/) and [starfile](https://pypi.org/project/starfile/) packages. Predictions should be written as a star file with the newly
 predicted Euler angles.
 
 Evaluation can be computed once the predictions for the half-set 0 and half-set 1 are saved
 
 ```
@@ -146,15 +150,15 @@
 
 | EMPIAR ID | Composition | Symmetry | Image Pixels | FSCR<sub>0.143</sub> (Å) | Masked FSCR<sub>0.143</sub> (Å) | # Particles |
 |-----------|-------------|----------|--------------|-------------------------|---------------------------------|-------------|
 | 10166     | Human 26S proteasome bound to the chemotherapeutic Oprozomib | C1 | 284 | 5.0 | 3.9 | 238631 |
 | 10786     | Substance P-Neurokinin Receptor G protein complexes (SP-NK1R-miniGs399) | C1 | 184 | 3.3 | 3.0* | 288659 |
 | 10280     | Calcium-bound TMEM16F in nanodisc with supplement of PIP2 | C2 | 182 | 3.6 | 3.0* | 459504 |
 | 11120     | M22 bound TSHR Gs 7TM G protein | C1 | 232 | 3.4 | 3.0* | 244973 |
-| 10647     | PKM2 in complex with L-threonine | D2 | 222 | 3.7 | 3.3 | 234956 |
+| 10648     | PKM2 in complex with Compound 5 | D2 | 222 | 3.7 | 3.3 | 234956 |
 | 10409     | Replicating SARS-CoV-2 polymerase (Map 1) | C1 | 240 | 3.3 | 3.0* | 406001 |
 | 10374     | Human ABCG2 transporter with inhibitor MZ29 and 5D3-Fab | C2 | 216 | 3.7 | 3.0* | 323681 |
 
 `*` Nyquist Frequency at 1.5 Å/pixel; Resolution is estimated at the usual threshold 0.143.  
 Reported FSCR<sub>0.143</sub> values were obtained directly from the relion_refine logs while Masked FSCR<sub>0.143</sub> values were collected from the relion_postprocess logs.
 
 In addition, the entry TEST is a small subset of EMPIAR-11120
```

### Comparing `cesped-24.4.3/cesped/configs/defaultDataAugmentation.yaml` & `cesped-24.5.0/cesped/configs/defaultDataAugmentation.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/configs/defaultDataConfig.yaml` & `cesped-24.5.0/cesped/configs/defaultDataConfig.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/configs/defaultTrainerConfig.yaml` & `cesped-24.5.0/cesped/configs/defaultTrainerConfig.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/constants.py` & `cesped-24.5.0/cesped/constants.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/datamanager/augmentations.py` & `cesped-24.5.0/cesped/datamanager/augmentations.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/datamanager/ctf.py` & `cesped-24.5.0/cesped/datamanager/ctf.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/datamanager/plDataset.py` & `cesped-24.5.0/cesped/datamanager/plDataset.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/evaluateEntry.py` & `cesped-24.5.0/cesped/evaluateEntry.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,36 +284,38 @@
             pred_map, pred_sampling, pred_corr, pred_resolut, pred_resolt05 = self.computeAvgMap(
                 prepStarFname0, prepStarFname1,
                 particlesDir=ps0.datadir, outbasename="pred",
                 symmetry=symmetry, cleanExisting=rm_prev_reconstructions, mask=mask_fname)
 
             if self.verbose:
                 print("Computing statistics...")
-            mapVsGT_cor, (mapVsGT_resolt, m_mapVsGT_resolt, *_) = compute_stats(gt_map, pred_map,
+            (mapVsGT_cor, mapVsGT_masked_cor), (mapVsGT_resolt, m_mapVsGT_resolt, *_) = compute_stats(gt_map, pred_map,
                                                                                 samplingRate=gt_sampling,
                                                                                 resolution_threshold=0.143,
                                                                                 maskOrFname=mask_fname)
             _, (mapVsGT_resolt05, m_mapVsGT_resolt05, *_) = compute_stats(gt_map, pred_map,
                                                                           samplingRate=gt_sampling,
                                                                           resolution_threshold=0.5,
                                                                           maskOrFname=mask_fname)
-            cor_diff = (gt_cor - mapVsGT_cor) #/ gt_cor
-
+            cor_diff = (gt_cor - mapVsGT_cor)
+            cor_diff_masked = (gt_cor - mapVsGT_masked_cor) 
+            
             res_diff05 = mapVsGT_resolt05 - gt_resolt05
             res_diff = mapVsGT_resolt - gt_resolt0143
 
 
             metrics = dict(meanAngularError=meanAngularError, wMeanAngularError=wMeanAngularError,
                            shiftsRMSE=shiftsRMSE,
                            GT_correlation=gt_cor,
                            GT_resolution0143=gt_resolt0143, GT_resolution05=gt_resolt05,
                            half2half_resolution=pred_resolut, half2half_resolution05=pred_resolt05,
                            half2half_correlation=pred_corr,
-                           mapVsGT_correlaton_masked=mapVsGT_cor[1], mapVsGT_correlaton_unmasked=mapVsGT_cor[0],
+                           mapVsGT_correlaton_masked=mapVsGT_masked_cor, mapVsGT_correlaton_unmasked=mapVsGT_cor,
                            mapVsGT_resolution=mapVsGT_resolt, mapVsGT_resolution05=mapVsGT_resolt05,
+                           mapVsGT_correlaton_diff_masked=cor_diff_masked, mapVsGT_correlaton_diff=cor_diff,
                            )
 
             with open(osp.join(self.wdir, "metrics.json"), "w") as f:
                 json.dump(metrics, f)
 
             report_str = f"""
 > EVALUATION for target:                  {targetName}
@@ -323,18 +325,18 @@
 #Predictions
 mean_angular_error (°):                   {meanAngularError} 
 w_mean_angular_error (°):                 {wMeanAngularError} 
 shifts_RMSE (Å):                          {shiftsRMSE}
 #Reconstruction
 half2half_correlation:                    {pred_corr}
 half2half_resolution (Å) (th=0.143, 0.5): {pred_resolut}  {pred_resolt05}
-mapVsGT_correlaton (masked, unmasked):    {"  ".join(reversed([str(x) for x in mapVsGT_cor]))}
+mapVsGT_correlaton (masked, unmasked):    {mapVsGT_masked_cor}  {mapVsGT_cor}
 mapVsGT_resolution (Å) (th=0.143, 0.5)    {mapVsGT_resolt}  {mapVsGT_resolt05}
 #Reconstruction differences
-cor_diff (%) (masked, unmasked):          {"  ".join(reversed([str(x * 100) for x in cor_diff]))}
+cor_diff   (masked, unmasked):            {cor_diff}  {cor_diff_masked}
 res_diff (Å) th=0.143, 0.5):              {res_diff}  {res_diff05}
             """
 
             if self.verbose:
                 print(report_str)
             return metrics
```

### Comparing `cesped-24.4.3/cesped/inferEntry.py` & `cesped-24.5.0/cesped/inferEntry.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,29 +88,27 @@
         super().parse_arguments(parser, args)
 
     def _instantiate_trainer(self, config: Dict[str, Any], callbacks: List[Callback]) -> Trainer:
 
         outFname = self.config[_outname_argname]
         outDir = osp.join(osp.dirname(outFname), "_tmp_" + osp.basename(osp.splitext(outFname)[0]))
         os.makedirs(outDir, exist_ok=True)
-
+        resultsWriter = CustomPredWriter(outDir)
+        self.resultsWriter = resultsWriter
+        callbacks += [resultsWriter]
+        trainer = super()._instantiate_trainer(config, callbacks)
         def remove_temp_dir(dir_path):
-            if os.path.exists(dir_path):
+            if os.path.exists(dir_path) and trainer.is_global_zero:
                 try:
                     shutil.rmtree(dir_path)
-                    print(f"Removed temporary directory: {dir_path}")
+                    print(f"Removed temporary directory: {dir_path} PID {os.getgid()}")
                 except OSError:
                     pass
         atexit.register(remove_temp_dir, outDir)
-
-        resultsWriter = CustomPredWriter(outDir)
-        self.resultsWriter = resultsWriter
-        callbacks += [resultsWriter]
-        return super()._instantiate_trainer(config, callbacks)
-
+        return trainer
 
 if __name__ == "__main__":
 
     config_fnames = [
         osp.join(default_configs_dir, "defaultDataConfig.yaml"),
         osp.join(default_configs_dir, "defaultInferenceConfig.yaml"),
     ]
```

### Comparing `cesped-24.4.3/cesped/network/featureExtractors.py` & `cesped-24.5.0/cesped/network/featureExtractors.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/network/image2sphere.py` & `cesped-24.5.0/cesped/network/image2sphere.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/network/plModule.py` & `cesped-24.5.0/cesped/network/plModule.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/particlesDataset.py` & `cesped-24.5.0/cesped/particlesDataset.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/trainEntry.py` & `cesped-24.5.0/cesped/trainEntry.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/utils/angles.py` & `cesped-24.5.0/cesped/utils/angles.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/utils/anglesStats.py` & `cesped-24.5.0/cesped/utils/anglesStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/utils/cliBuilder.py` & `cesped-24.5.0/cesped/utils/cliBuilder.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/utils/fsc.py` & `cesped-24.5.0/cesped/utils/fsc.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/utils/gaussianFilters.py` & `cesped-24.5.0/cesped/utils/gaussianFilters.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/utils/tensors.py` & `cesped-24.5.0/cesped/utils/tensors.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/utils/volumeStats.py` & `cesped-24.5.0/cesped/utils/volumeStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/cesped/zenodo/downloadFromZenodo.py` & `cesped-24.5.0/cesped/zenodo/downloadFromZenodo.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,42 @@
 import shutil
 import tempfile
 from hashlib import md5
 
 import requests
 from tqdm import tqdm
 
-from cesped.zenodo.bechmarkUrls import ROOT_URL_PATTERN, NAME_TO_MASK_URL
+from cesped.zenodo.bechmarkUrls import ROOT_URL_PATTERN, NAME_TO_MASK_URL, RECORD_DEPENDENCIES, \
+    NAME_PARTITION_TO_RECORID
 
 
 def getDoneFname(destination_dir, record_id):
     return os.path.join(destination_dir, f"SUCCESSFUL_DOWNLOAD_{record_id}.txt")
-def download_record(record_id:str, destination_dir:str, root_url:str=ROOT_URL_PATTERN):
+def download_record(record_id:str, destination_dir:str, root_url:str=ROOT_URL_PATTERN, check_mrcs=True):
     """
 
     @param record_id:
     @param destination_dir:
     @param root_url:
 
     """
 
+    if record_id in RECORD_DEPENDENCIES:
+        data_root_dir, targetName = os.path.split(destination_dir)
+        os.makedirs(destination_dir, exist_ok=True)
+        RECORD_TO_NAME = {record:name for (name,_), record in NAME_PARTITION_TO_RECORID.items()}
+        for dep_rec_id in RECORD_DEPENDENCIES[record_id]:
+            _destination_dir = os.path.join(data_root_dir, RECORD_TO_NAME[dep_rec_id])
+            os.makedirs(_destination_dir, exist_ok=True)
+            print(f"Downloading dependency {dep_rec_id}")
+            download_record(dep_rec_id, _destination_dir, root_url, check_mrcs=True)
+            for fname in os.listdir(_destination_dir):
+                if fname not in os.listdir(destination_dir) and not fname.endswith(".star"):
+                    os.symlink(os.path.join(_destination_dir, fname), os.path.join(destination_dir, fname))
+        check_mrcs = False
     donefname = getDoneFname(destination_dir, record_id)
     if os.path.isfile(donefname):
         return
     root_url = f"{root_url}/{record_id}"
     r = requests.get(root_url)
     assert r.status_code == 200, f"Error, bad request response {r} for {root_url}"
     # print(r.json())
@@ -112,31 +126,34 @@
 
     assert jsonFname, "Error, json file not found in the record"
     url, size, checksum = files_info_dict[jsonFname]
     output_file_path = os.path.join(destination_dir, jsonFname)
     download_and_concatenate_files([url], [size], [checksum], output_file_path)
     print(f"Particle json downloaded at {output_file_path}")
 
-    assert mrcsFnames, "Error, mrcs files not found in the record"
-    urls = []
-    sizes = []
-    checksums = []
-    for fname in sorted(mrcsFnames, key=lambda x: int(x.split("mrcs.chunk_")[-1])):
-        url, size, checksum = files_info_dict[fname]
-        urls += [url]
-        sizes += [size]
-        checksums += [checksum]
-
-    output_file_path = os.path.join(destination_dir, starFname.replace(".star", ".mrcs"))
-    current_size = download_and_concatenate_files(urls, sizes, checksums, output_file_path)
-    print(f"Particle stack downloaded at {output_file_path}")
+    current_size = 0
+    if check_mrcs:
+        assert mrcsFnames, "Error, mrcs files not found in the record"
+    if mrcsFnames:
+        urls = []
+        sizes = []
+        checksums = []
+        for fname in sorted(mrcsFnames, key=lambda x: int(x.split("mrcs.chunk_")[-1])):
+            url, size, checksum = files_info_dict[fname]
+            urls += [url]
+            sizes += [size]
+            checksums += [checksum]
+
+        output_file_path = os.path.join(destination_dir, starFname.replace(".star", ".mrcs"))
+        current_size = download_and_concatenate_files(urls, sizes, checksums, output_file_path)
+        print(f"Particle stack downloaded at {output_file_path}")
+        print()
     with open(donefname, "w") as f:
         f.write("%s\n"%record_id)
         f.write("%s\n"%current_size)
-    print()
 
 def download_mask(targetName, mask_fname):
 
     if os.path.exists(mask_fname):
         return
     mask_url = NAME_TO_MASK_URL[targetName]
     response = requests.get(mask_url, stream=True)
@@ -148,7 +165,8 @@
         for chunk in response.iter_content(chunk_size=100 * 1024 * 2):  # 100MB chunks
             tmpf.write(chunk)
         shutil.copyfile(tmpf.name, mask_fname)
 
 if __name__ == "__main__":
     from argParseFromDoc import parse_function_and_call
     parse_function_and_call(download_record)
+
```

### Comparing `cesped-24.4.3/cesped/zenodo/uploadToZenodo.py` & `cesped-24.5.0/cesped/zenodo/uploadToZenodo.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,59 +5,64 @@
 import json
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 import argparse
 
 from cesped.zenodo import tokens
 
-#TODO: Ask for symmetry and store it.
 
 SANDBOX = False
-CHUNK_SIZE = 1024 ** 2 * 300  # 300MB
+CHUNK_SIZE = 1000 ** 2 * 500  # 500MB
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("-d", "--dirname" , type=str, required=True)
-    parser.add_argument("-e", "--empiarID" , type=int, required=True)
+    parser.add_argument("-e", "--empiarID" , type=str, required=True)
     parser.add_argument("-s", "--split" , type=int, required=True)
     parser.add_argument("-y", "--symmetry" , type=str, required=True)
-
+    parser.add_argument("--update_id", type=str, help="update existing entry with id", default=None)
+    parser.add_argument("--token", type=str, help="The access token", default=None)
+    
     args = parser.parse_args()
-    # dir_to_upload = "/homes/sanchezg/ScipionUserData/projects/EMPIAR-10166/Runs/000463_ProtRelionAutorefSplitData/extra/subset_1/"  # "/home/sanchezg/tmp/ConorData/bound/postprocess/"
+    # dir_to_upload = "/homes/sanchezg/ScipionUserData/projects/EMPIAR-10166/Runs/000463_ProtRelionAutorefSplitData/extra/subset_1/"
     # dataset_name = "CESPED-10166_split1"
     dir_to_upload = args.dirname
     assert args.split in [0,1]
     dataset_name = f"CESPED-{args.empiarID}_split{args.split}"
     print(dir_to_upload)
     print(dataset_name)
 
 
 
     assert os.path.exists(dir_to_upload), f"Error, file {dir_to_upload} does not exists"
 
     if not SANDBOX:
         # zenodo
-        ACCESS_TOKEN = tokens.ACCESS_TOKEN_ZENODO
+        ACCESS_TOKEN = tokens.ACCESS_TOKEN_ZENODO if args.token is None else args.token
         baseurl = 'https://zenodo.org/api/'
     else:
         # zenodo sandbox
-        ACCESS_TOKEN = tokens.ACCESS_TOKEN_ZENODO_SANDBOX
+        ACCESS_TOKEN = tokens.ACCESS_TOKEN_ZENODO_SANDBOX if args.token is None else args.token
         baseurl = 'https://sandbox.zenodo.org/api/'
 
     r = requests.get(baseurl + 'deposit/depositions', params={'access_token': ACCESS_TOKEN})
     assert r.status_code == 200, "Error, cannot connect"
     r.json()
 
 
     # Creates empty deposition
     headers = {"Content-Type": "application/json"}
     params = {'access_token': ACCESS_TOKEN}
-    r = requests.post(baseurl + 'deposit/depositions', params=params, json={}, headers=headers)
+    
+    if args.update_id is not None:
+        r = requests.post(baseurl + f'deposit/depositions/{args.update_id}/actions/newversion', params=params, json={}, headers=headers)
+    else:
+        r = requests.post(baseurl + 'deposit/depositions', params=params, json={}, headers=headers)
 
     print("Empty deposition creation status", r.status_code)
-    assert r.status_code == 201
+    assert r.status_code == 201, r.json()
     # 201
     print(r.json())
 
     print("URL TO CHECK IN THE BROWSER", r.json()["links"]["latest_draft_html"])
 
     bucket_url = r.json()["links"]["bucket"]
     deposition_id = r.json()["id"]
@@ -99,29 +104,29 @@
                     chunk = f.read(chunk_size)
                     if not chunk:
                         break
                     chunk_filename = f"{web_filename}.chunk_{chunk_number}"
                     target_url = f"{upload_url}/{chunk_filename}"
                     #                print(chunk_filename)
                     r = requests.put(target_url, data=chunk, params=params)
-                    assert r.status_code == 200
+                    assert r.status_code in [200, 201], f"{r.status_code}"
                     chunk_number += 1
 
 
     def upload(path, upload_url, web_filename):
         file_size = os.stat(path).st_size
         with open(path, "rb") as fp:
             with tqdm(total=file_size, unit="B", unit_scale=True, unit_divisor=1024) as t:
                 wrapped_file = CallbackIOWrapper(t.update, fp, "read")
                 r = requests.put(
                     "%s/%s" % (upload_url, web_filename),
                     data=wrapped_file,
                     params=params,
                 )
-                assert r.status_code == 200, f"Error, {web_filename} was not uploaded"
+                assert r.status_code in [200, 201], f"Error, {web_filename} was not uploaded"
 
 
     with tempfile.TemporaryDirectory() as temp_dir:
         temp_file_path = os.path.join(temp_dir, f"info_{args.split}.json")
         with open(temp_file_path, "w") as f:
             json.dump({"symmetry": args.symmetry.upper()}, f)
             f.seek(0)
@@ -134,8 +139,8 @@
 
 
 
 
     print("URL TO CHECK IN THE BROWSER", r.json()["links"]["latest_draft_html"])
     ## WARNING, THE FOLLOWING LINE WILL PUBLISH THE RESULTS. ARE YOU SURE?
     # input(" THE FOLLOWING LINE WILL PUBLISH THE RESULTS. ARE YOU SURE?")
-    # r = requests.post(baseurl+'deposit/depositions/%s/actions/publish' % deposition_id, params={'access_token': ACCESS_TOKEN} )
+    # r = requests.post(baseurl+'deposit/depositions/%s/actions/publish' % deposition_id, params={'access_token': ACCESS_TOKEN} )
```

### Comparing `cesped-24.4.3/cesped.egg-info/PKG-INFO` & `cesped-24.5.0/cesped.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesped
-Version: 24.4.3
+Version: 24.5.0
 Summary: Code utilities for the CESPED (Cryo-EM Supervised Pose Estimation Dataset) benchmark
 Home-page: https://github.com/rsanchezgarc/cesped
 Author: Ruben Sanchez-Garcia
 Author-email: ruben.sanchez-garcia@stats.ox.ac.uk
 Keywords: deep learning cryoem pose estimation
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,15 +25,15 @@
 Requires-Dist: starstack>=0.2.0
 Requires-Dist: tensorboard>=2.12.1
 Requires-Dist: torch<3.0.0,>=2.0.0
 Requires-Dist: torchvision>=0.15.2
 
 # CESPED: Utilities for the Cryo-EM Supervised Pose Estimation Dataset
 
-CESPED, is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check our manuscript at https://arxiv.org/abs/2311.06194.
+CESPED is a new dataset specifically designed for Supervised Pose Estimation in Cryo-EM. You can check our manuscript at https://arxiv.org/abs/2311.06194.
 
 ## Installation
 cesped has been tested on python 3.11. Installation should be automatic using pip
 ```
 pip install cesped
 #Or directy from the master branch
 pip install git+https://github.com/rsanchezgarc/cesped
@@ -133,17 +133,21 @@
 python -m cesped.particlesDataset download_entry -t 10166 --halfset 0
 ```
 This will download the associated starfile and mrcs file to the default benchmark directory (defined in [defaultDataConfig.yaml](cesped%2Fconfigs%2FdefaultDataConfig.yaml).
 Use `--benchmarkDir` to specify another directory<br/>
 
 In order to list the entries available for download and the ones already downloaded, you can use
 ```
-python -m cesped.particlesDataset preprocess_entry --t 10166 --halfset 0--o /tmp/dumpedData/ --ctf_correction "phase_flip"
+python -m cesped.particlesDataset list_entries
 ```
-use `-h` to display the list of available preprocessing operations.
+Preprocessing of the dataset entries can be executed using
+```
+python -m cesped.particlesDataset preprocess_entry --t 10166 --halfset 0 --o /tmp/dumpedData/ --ctf_correction "phase_flip"
+```
+where `--t` is the target name. Use `-h` to display the list of available preprocessing operations.
 
 The raw data can be easily accessed using the Python package [starstack](https://pypi.org/project/starstack/), which relies on the [mrcfile](https://pypi.org/project/mrcfile/) and [starfile](https://pypi.org/project/starfile/) packages. Predictions should be written as a star file with the newly
 predicted Euler angles.
 
 Evaluation can be computed once the predictions for the half-set 0 and half-set 1 are saved
 
 ```
@@ -175,15 +179,15 @@
 
 | EMPIAR ID | Composition | Symmetry | Image Pixels | FSCR<sub>0.143</sub> (Å) | Masked FSCR<sub>0.143</sub> (Å) | # Particles |
 |-----------|-------------|----------|--------------|-------------------------|---------------------------------|-------------|
 | 10166     | Human 26S proteasome bound to the chemotherapeutic Oprozomib | C1 | 284 | 5.0 | 3.9 | 238631 |
 | 10786     | Substance P-Neurokinin Receptor G protein complexes (SP-NK1R-miniGs399) | C1 | 184 | 3.3 | 3.0* | 288659 |
 | 10280     | Calcium-bound TMEM16F in nanodisc with supplement of PIP2 | C2 | 182 | 3.6 | 3.0* | 459504 |
 | 11120     | M22 bound TSHR Gs 7TM G protein | C1 | 232 | 3.4 | 3.0* | 244973 |
-| 10647     | PKM2 in complex with L-threonine | D2 | 222 | 3.7 | 3.3 | 234956 |
+| 10648     | PKM2 in complex with Compound 5 | D2 | 222 | 3.7 | 3.3 | 234956 |
 | 10409     | Replicating SARS-CoV-2 polymerase (Map 1) | C1 | 240 | 3.3 | 3.0* | 406001 |
 | 10374     | Human ABCG2 transporter with inhibitor MZ29 and 5D3-Fab | C2 | 216 | 3.7 | 3.0* | 323681 |
 
 `*` Nyquist Frequency at 1.5 Å/pixel; Resolution is estimated at the usual threshold 0.143.  
 Reported FSCR<sub>0.143</sub> values were obtained directly from the relion_refine logs while Masked FSCR<sub>0.143</sub> values were collected from the relion_postprocess logs.
 
 In addition, the entry TEST is a small subset of EMPIAR-11120
```

### Comparing `cesped-24.4.3/cesped.egg-info/SOURCES.txt` & `cesped-24.5.0/cesped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/setup.py` & `cesped-24.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/tests/test_anglesStats.py` & `cesped-24.5.0/tests/test_anglesStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.4.3/tests/test_particlesDataset.py` & `cesped-24.5.0/tests/test_particlesDataset.py`

 * *Files identical despite different names*

