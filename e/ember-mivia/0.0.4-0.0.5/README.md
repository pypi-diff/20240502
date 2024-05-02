# Comparing `tmp/ember-mivia-0.0.4.tar.gz` & `tmp/ember-mivia-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ember-mivia-0.0.4.tar", last modified: Fri Feb  9 13:25:42 2024, max compression
+gzip compressed data, was "ember-mivia-0.0.5.tar", last modified: Thu May  2 13:43:53 2024, max compression
```

## Comparing `ember-mivia-0.0.4.tar` & `ember-mivia-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 gparrella (10199) clusterusers  (5000)        0 2024-02-09 13:26:10.060153 ember-mivia-0.0.4/
--rw-r--r--   0 gparrella (10199) clusterusers  (5000)     8846 2024-02-09 13:26:10.059153 ember-mivia-0.0.4/PKG-INFO
--rw-r--r--   0 gparrella (10199) clusterusers  (5000)     7534 2024-02-01 10:35:55.000000 ember-mivia-0.0.4/README.md
-drwxr-xr-x   0 gparrella (10199) clusterusers  (5000)        0 2024-02-09 13:26:10.039153 ember-mivia-0.0.4/ember/
--rw-r--r--   0 gparrella (10199) clusterusers  (5000)     8134 2024-02-01 10:35:55.000000 ember-mivia-0.0.4/ember/__init__.py
--rw-r--r--   0 gparrella (10199) clusterusers  (5000)    28485 2024-02-09 13:23:58.000000 ember-mivia-0.0.4/ember/features.py
-drwxr-xr-x   0 gparrella (10199) clusterusers  (5000)        0 2024-02-09 13:26:10.055153 ember-mivia-0.0.4/ember_mivia.egg-info/
--rw-r--r--   0 gparrella (10199) clusterusers  (5000)     8846 2024-02-09 13:26:09.000000 ember-mivia-0.0.4/ember_mivia.egg-info/PKG-INFO
--rw-r--r--   0 gparrella (10199) clusterusers  (5000)      194 2024-02-09 13:26:09.000000 ember-mivia-0.0.4/ember_mivia.egg-info/SOURCES.txt
--rw-r--r--   0 gparrella (10199) clusterusers  (5000)        1 2024-02-09 13:26:09.000000 ember-mivia-0.0.4/ember_mivia.egg-info/dependency_links.txt
--rw-r--r--   0 gparrella (10199) clusterusers  (5000)        6 2024-02-09 13:26:09.000000 ember-mivia-0.0.4/ember_mivia.egg-info/top_level.txt
--rw-r--r--   0 gparrella (10199) clusterusers  (5000)       38 2024-02-09 13:26:10.061153 ember-mivia-0.0.4/setup.cfg
--rw-r--r--   0 gparrella (10199) clusterusers  (5000)      612 2024-02-09 13:25:59.000000 ember-mivia-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:43:53.630121 ember-mivia-0.0.5/
+-rw-rw-rw-   0        0        0      229 2024-05-02 13:40:41.000000 ember-mivia-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     7923 2024-05-02 13:43:53.628340 ember-mivia-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7664 2024-05-02 13:40:41.000000 ember-mivia-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 13:43:53.596192 ember-mivia-0.0.5/ember/
+-rw-rw-rw-   0        0        0     8367 2024-05-02 13:40:41.000000 ember-mivia-0.0.5/ember/__init__.py
+-rw-rw-rw-   0        0        0    29350 2024-05-02 13:42:30.000000 ember-mivia-0.0.5/ember/features.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:43:53.624830 ember-mivia-0.0.5/ember_mivia.egg-info/
+-rw-rw-rw-   0        0        0     7923 2024-05-02 13:43:53.000000 ember-mivia-0.0.5/ember_mivia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2024-05-02 13:43:53.000000 ember-mivia-0.0.5/ember_mivia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 13:43:53.000000 ember-mivia-0.0.5/ember_mivia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-02 13:43:53.000000 ember-mivia-0.0.5/ember_mivia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 13:43:53.631023 ember-mivia-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      636 2024-05-02 13:43:43.000000 ember-mivia-0.0.5/setup.py
```

### Comparing `ember-mivia-0.0.4/PKG-INFO` & `ember-mivia-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,140 +1,130 @@
-Metadata-Version: 2.1
-Name: ember-mivia
-Version: 0.0.4
-Summary: Endgame Malware BEnchmark for Research
-Home-page: https://github.com/gparrella12/ember
-Author-email: proth@endgame.com
-License: UNKNOWN
-Description: <img src="resources/logo.png" align="right" width="250px" height="250px">
-        
-        # Elastic Malware Benchmark for Empowering Researchers
-        
-        The EMBER dataset is a collection of features from PE files that serve as a benchmark dataset for researchers. The EMBER2017 dataset contained features from 1.1 million PE files scanned in or before 2017 and the EMBER2018 dataset contains features from 1 million PE files scanned in or before 2018. This repository makes it easy to reproducibly train the benchmark models, extend the provided feature set, or classify new PE files with the benchmark models.
-        
-        This paper describes many more details about the dataset: [https://arxiv.org/abs/1804.04637](https://arxiv.org/abs/1804.04637)
-        
-        ## Features
-        
-        The [LIEF](https://lief.quarkslab.com/) project is used to extract features from PE files included in the EMBER dataset. Raw features are extracted to JSON format and included in the publicly available dataset. Vectorized features can be produced from these raw features and saved in binary format from which they can be converted to CSV, dataframe, or any other format. This repository makes it easy to generate raw features and/or vectorized features from any PE file. Researchers can implement their own features, or even vectorize the existing features differently from the existing implementations.
-        
-        The feature calculation is versioned. Feature version 1 is calculated with the LIEF library version 0.8.3. Feature version 2 includes the additional data directory feature, updated ordinal import processing, and is calculated with LIEF library version 0.9.0.  We have verified under Windows and Linux that LIEF provides consistent feature representation for version 2 features using LIEF version 0.10.1 and that it does not on a Mac.
-        
-        ## Years
-        
-        The first EMBER dataset consisted of version 1 features calculated over samples collected in or before 2017. The second EMBER dataset release consisted of version 2 features calculated over samples collected in or before 2018. In conjunction with the second release, we also included the version 2 features from the samples collected in 2017. Combining the data from 2017 and 2018 will allow longer longitudinal studies of the evolution of features and PE file types. But different selection criteria were applied when choosing samples from 2017 and 2018. Specifically, the samples from 2018 were chosen so that the resultant training and test sets would be harder for machine learning algorithms to classify. Please beware of this inconsistancy while constructing your multi-year studies. The original paper only describes Ember 2017 (featur version 1). For a detailed information about the Ember 2018 dataset, please refer to https://www.camlis.org/2019/talks/roth where you can find both [slides](https://docs.google.com/presentation/d/1A13tsUkgWeujTy9SD-vDFfQp9fnIqbSE_tCihNPlArQ/edit#slide=id.g476bf81b41_0_446) and a [video talk](https://youtu.be/MsZmnUO5lkY).
-        
-        ## Download
-        
-        Download the data here:
-        
-        | Year | Feature Version | Filename                     | URL                                                                                                            | sha256                                                             |
-        |------|-----------------|------------------------------|----------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
-        | 2017 | 1               | ember_dataset.tar.bz2        | [https://ember.elastic.co/ember_dataset.tar.bz2](https://ember.elastic.co/ember_dataset.tar.bz2)               | `a5603de2f34f02ab6e21df7a0f97ec4ac84ddc65caee33fb610093dd6f9e1df9` |
-        | 2017 | 2               | ember_dataset_2017_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2017_2.tar.bz2](https://ember.elastic.co/ember_dataset_2017_2.tar.bz2) | `60142493c44c11bc3fef292b216a293841283d86ff58384b5dc2d88194c87a6d` |
-        | 2018 | 2               | ember_dataset_2018_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2018_2.tar.bz2](https://ember.elastic.co/ember_dataset_2018_2.tar.bz2) | `b6052eb8d350a49a8d5a5396fbe7d16cf42848b86ff969b77464434cf2997812` |
-        
-        
-        ## Installation
-        ### Instrall directly from git
-        Use `pip` to install the `ember` and required files
-        
-        ```
-        pip install git+https://github.com/elastic/ember.git
-        ```
-        
-        This provides access to EMBER feature extaction for example.  However, to use the scripts to train the model, one would instead clone the repository.
-        
-        
-        ### Install after cloning the EMBER repository
-        Use `pip` or `conda` to install the required packages before installing `ember` itself:
-        
-        ```
-        pip install -r requirements.txt
-        python setup.py install
-        ```
-        
-        ```
-        conda config --add channels conda-forge
-        conda install --file requirements_conda.txt
-        python setup.py install
-        ```
-        
-        ### Notes on LIEF versions
-        
-        LIEF is now pinned to version 0.9.0 in the provided requirements files. This default behavior will allow new users to immediately reproduce EMBER version 2 features. LIEF 0.9.0 will not install on an M1 Mac, though. For those users, a Dockerfile is now included that installs the dependencies using conda.
-        
-        EMBER will work with more recent releases of LIEF, but keep in mind that models trained on features generated with one version of LIEF will have unpredictable results when evaluating on features generated with another.
-        
-        ## Scripts
-        
-        The `train_ember.py` script simplifies the model training process. It will vectorize the ember features if necessary and then train the LightGBM model.
-        
-        ```
-        python train_ember.py [/path/to/dataset]
-        ```
-        
-        The `classify_binaries.py` script will return model predictions on PE files.
-        
-        ```
-        python classify_binaries.py -m [/path/to/model] BINARIES
-        ```
-        
-        ## Import Usage
-        
-        The raw feature data can be expanded into vectorized form on disk for model training and into metadata form. These two functions create those extra files:
-        
-        ```
-        import ember
-        ember.create_vectorized_features("/data/ember2018/")
-        ember.create_metadata("/data/ember2018/")
-        ```
-        
-        Once created, that data can be read in using convenience functions:
-        
-        ```
-        import ember
-        X_train, y_train, X_test, y_test = ember.read_vectorized_features("/data/ember2018/")
-        metadata_dataframe = ember.read_metadata("/data/ember2018/")
-        ```
-        
-        Once the data is downloaded and the ember module is installed, this simple code should reproduce the benchmark ember model:
-        
-        ```
-        import ember
-        ember.create_vectorized_features("/data/ember2018/")
-        lgbm_model = ember.train_model("/data/ember2018/")
-        ```
-        
-        Once the model is trained, the ember module can be used to make a prediction on any input PE file:
-        
-        ```
-        import ember
-        import lightgbm as lgb
-        lgbm_model = lgb.Booster(model_file="/data/ember2018/ember_model_2018.txt")
-        putty_data = open("~/putty.exe", "rb").read()
-        print(ember.predict_sample(lgbm_model, putty_data))
-        ```
-        
-        ## Citing
-        
-        If you use this data in a publication please cite the following [paper](https://arxiv.org/abs/1804.04637):
-        
-        ```
-        H. Anderson and P. Roth, "EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models”, in ArXiv e-prints. Apr. 2018.
-        
-        @ARTICLE{2018arXiv180404637A,
-          author = {{Anderson}, H.~S. and {Roth}, P.},
-          title = "{EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models}",
-          journal = {ArXiv e-prints},
-          archivePrefix = "arXiv",
-          eprint = {1804.04637},
-          primaryClass = "cs.CR",
-          keywords = {Computer Science - Cryptography and Security},
-          year = 2018,
-          month = apr,
-          adsurl = {http://adsabs.harvard.edu/abs/2018arXiv180404637A},
-        }
-        ```
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+<img src="resources/logo.png" align="right" width="250px" height="250px">
+
+# Elastic Malware Benchmark for Empowering Researchers
+
+The EMBER dataset is a collection of features from PE files that serve as a benchmark dataset for researchers. The EMBER2017 dataset contained features from 1.1 million PE files scanned in or before 2017 and the EMBER2018 dataset contains features from 1 million PE files scanned in or before 2018. This repository makes it easy to reproducibly train the benchmark models, extend the provided feature set, or classify new PE files with the benchmark models.
+
+This paper describes many more details about the dataset: [https://arxiv.org/abs/1804.04637](https://arxiv.org/abs/1804.04637)
+
+## Features
+
+The [LIEF](https://lief.quarkslab.com/) project is used to extract features from PE files included in the EMBER dataset. Raw features are extracted to JSON format and included in the publicly available dataset. Vectorized features can be produced from these raw features and saved in binary format from which they can be converted to CSV, dataframe, or any other format. This repository makes it easy to generate raw features and/or vectorized features from any PE file. Researchers can implement their own features, or even vectorize the existing features differently from the existing implementations.
+
+The feature calculation is versioned. Feature version 1 is calculated with the LIEF library version 0.8.3. Feature version 2 includes the additional data directory feature, updated ordinal import processing, and is calculated with LIEF library version 0.9.0.  We have verified under Windows and Linux that LIEF provides consistent feature representation for version 2 features using LIEF version 0.10.1 and that it does not on a Mac.
+
+## Years
+
+The first EMBER dataset consisted of version 1 features calculated over samples collected in or before 2017. The second EMBER dataset release consisted of version 2 features calculated over samples collected in or before 2018. In conjunction with the second release, we also included the version 2 features from the samples collected in 2017. Combining the data from 2017 and 2018 will allow longer longitudinal studies of the evolution of features and PE file types. But different selection criteria were applied when choosing samples from 2017 and 2018. Specifically, the samples from 2018 were chosen so that the resultant training and test sets would be harder for machine learning algorithms to classify. Please beware of this inconsistancy while constructing your multi-year studies. The original paper only describes Ember 2017 (featur version 1). For a detailed information about the Ember 2018 dataset, please refer to https://www.camlis.org/2019/talks/roth where you can find both [slides](https://docs.google.com/presentation/d/1A13tsUkgWeujTy9SD-vDFfQp9fnIqbSE_tCihNPlArQ/edit#slide=id.g476bf81b41_0_446) and a [video talk](https://youtu.be/MsZmnUO5lkY).
+
+## Download
+
+Download the data here:
+
+| Year | Feature Version | Filename                     | URL                                                                                                            | sha256                                                             |
+|------|-----------------|------------------------------|----------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
+| 2017 | 1               | ember_dataset.tar.bz2        | [https://ember.elastic.co/ember_dataset.tar.bz2](https://ember.elastic.co/ember_dataset.tar.bz2)               | `a5603de2f34f02ab6e21df7a0f97ec4ac84ddc65caee33fb610093dd6f9e1df9` |
+| 2017 | 2               | ember_dataset_2017_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2017_2.tar.bz2](https://ember.elastic.co/ember_dataset_2017_2.tar.bz2) | `60142493c44c11bc3fef292b216a293841283d86ff58384b5dc2d88194c87a6d` |
+| 2018 | 2               | ember_dataset_2018_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2018_2.tar.bz2](https://ember.elastic.co/ember_dataset_2018_2.tar.bz2) | `b6052eb8d350a49a8d5a5396fbe7d16cf42848b86ff969b77464434cf2997812` |
+
+
+## Installation
+### Instrall directly from git
+Use `pip` to install the `ember` and required files
+
+```
+pip install git+https://github.com/elastic/ember.git
+```
+
+This provides access to EMBER feature extaction for example.  However, to use the scripts to train the model, one would instead clone the repository.
+
+
+### Install after cloning the EMBER repository
+Use `pip` or `conda` to install the required packages before installing `ember` itself:
+
+```
+pip install -r requirements.txt
+python setup.py install
+```
+
+```
+conda config --add channels conda-forge
+conda install --file requirements_conda.txt
+python setup.py install
+```
+
+### Notes on LIEF versions
+
+LIEF is now pinned to version 0.9.0 in the provided requirements files. This default behavior will allow new users to immediately reproduce EMBER version 2 features. LIEF 0.9.0 will not install on an M1 Mac, though. For those users, a Dockerfile is now included that installs the dependencies using conda.
+
+EMBER will work with more recent releases of LIEF, but keep in mind that models trained on features generated with one version of LIEF will have unpredictable results when evaluating on features generated with another.
+
+## Scripts
+
+The `train_ember.py` script simplifies the model training process. It will vectorize the ember features if necessary and then train the LightGBM model.
+
+```
+python train_ember.py [/path/to/dataset]
+```
+
+The `classify_binaries.py` script will return model predictions on PE files.
+
+```
+python classify_binaries.py -m [/path/to/model] BINARIES
+```
+
+## Import Usage
+
+The raw feature data can be expanded into vectorized form on disk for model training and into metadata form. These two functions create those extra files:
+
+```
+import ember
+ember.create_vectorized_features("/data/ember2018/")
+ember.create_metadata("/data/ember2018/")
+```
+
+Once created, that data can be read in using convenience functions:
+
+```
+import ember
+X_train, y_train, X_test, y_test = ember.read_vectorized_features("/data/ember2018/")
+metadata_dataframe = ember.read_metadata("/data/ember2018/")
+```
+
+Once the data is downloaded and the ember module is installed, this simple code should reproduce the benchmark ember model:
+
+```
+import ember
+ember.create_vectorized_features("/data/ember2018/")
+lgbm_model = ember.train_model("/data/ember2018/")
+```
+
+Once the model is trained, the ember module can be used to make a prediction on any input PE file:
+
+```
+import ember
+import lightgbm as lgb
+lgbm_model = lgb.Booster(model_file="/data/ember2018/ember_model_2018.txt")
+putty_data = open("~/putty.exe", "rb").read()
+print(ember.predict_sample(lgbm_model, putty_data))
+```
+
+## Citing
+
+If you use this data in a publication please cite the following [paper](https://arxiv.org/abs/1804.04637):
+
+```
+H. Anderson and P. Roth, "EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models”, in ArXiv e-prints. Apr. 2018.
+
+@ARTICLE{2018arXiv180404637A,
+  author = {{Anderson}, H.~S. and {Roth}, P.},
+  title = "{EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models}",
+  journal = {ArXiv e-prints},
+  archivePrefix = "arXiv",
+  eprint = {1804.04637},
+  primaryClass = "cs.CR",
+  keywords = {Computer Science - Cryptography and Security},
+  year = 2018,
+  month = apr,
+  adsurl = {http://adsabs.harvard.edu/abs/2018arXiv180404637A},
+}
+```
```

### Comparing `ember-mivia-0.0.4/README.md` & `ember-mivia-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,130 +1,139 @@
-<img src="resources/logo.png" align="right" width="250px" height="250px">
-
-# Elastic Malware Benchmark for Empowering Researchers
-
-The EMBER dataset is a collection of features from PE files that serve as a benchmark dataset for researchers. The EMBER2017 dataset contained features from 1.1 million PE files scanned in or before 2017 and the EMBER2018 dataset contains features from 1 million PE files scanned in or before 2018. This repository makes it easy to reproducibly train the benchmark models, extend the provided feature set, or classify new PE files with the benchmark models.
-
-This paper describes many more details about the dataset: [https://arxiv.org/abs/1804.04637](https://arxiv.org/abs/1804.04637)
-
-## Features
-
-The [LIEF](https://lief.quarkslab.com/) project is used to extract features from PE files included in the EMBER dataset. Raw features are extracted to JSON format and included in the publicly available dataset. Vectorized features can be produced from these raw features and saved in binary format from which they can be converted to CSV, dataframe, or any other format. This repository makes it easy to generate raw features and/or vectorized features from any PE file. Researchers can implement their own features, or even vectorize the existing features differently from the existing implementations.
-
-The feature calculation is versioned. Feature version 1 is calculated with the LIEF library version 0.8.3. Feature version 2 includes the additional data directory feature, updated ordinal import processing, and is calculated with LIEF library version 0.9.0.  We have verified under Windows and Linux that LIEF provides consistent feature representation for version 2 features using LIEF version 0.10.1 and that it does not on a Mac.
-
-## Years
-
-The first EMBER dataset consisted of version 1 features calculated over samples collected in or before 2017. The second EMBER dataset release consisted of version 2 features calculated over samples collected in or before 2018. In conjunction with the second release, we also included the version 2 features from the samples collected in 2017. Combining the data from 2017 and 2018 will allow longer longitudinal studies of the evolution of features and PE file types. But different selection criteria were applied when choosing samples from 2017 and 2018. Specifically, the samples from 2018 were chosen so that the resultant training and test sets would be harder for machine learning algorithms to classify. Please beware of this inconsistancy while constructing your multi-year studies. The original paper only describes Ember 2017 (featur version 1). For a detailed information about the Ember 2018 dataset, please refer to https://www.camlis.org/2019/talks/roth where you can find both [slides](https://docs.google.com/presentation/d/1A13tsUkgWeujTy9SD-vDFfQp9fnIqbSE_tCihNPlArQ/edit#slide=id.g476bf81b41_0_446) and a [video talk](https://youtu.be/MsZmnUO5lkY).
-
-## Download
-
-Download the data here:
-
-| Year | Feature Version | Filename                     | URL                                                                                                            | sha256                                                             |
-|------|-----------------|------------------------------|----------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
-| 2017 | 1               | ember_dataset.tar.bz2        | [https://ember.elastic.co/ember_dataset.tar.bz2](https://ember.elastic.co/ember_dataset.tar.bz2)               | `a5603de2f34f02ab6e21df7a0f97ec4ac84ddc65caee33fb610093dd6f9e1df9` |
-| 2017 | 2               | ember_dataset_2017_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2017_2.tar.bz2](https://ember.elastic.co/ember_dataset_2017_2.tar.bz2) | `60142493c44c11bc3fef292b216a293841283d86ff58384b5dc2d88194c87a6d` |
-| 2018 | 2               | ember_dataset_2018_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2018_2.tar.bz2](https://ember.elastic.co/ember_dataset_2018_2.tar.bz2) | `b6052eb8d350a49a8d5a5396fbe7d16cf42848b86ff969b77464434cf2997812` |
-
-
-## Installation
-### Instrall directly from git
-Use `pip` to install the `ember` and required files
-
-```
-pip install git+https://github.com/elastic/ember.git
-```
-
-This provides access to EMBER feature extaction for example.  However, to use the scripts to train the model, one would instead clone the repository.
-
-
-### Install after cloning the EMBER repository
-Use `pip` or `conda` to install the required packages before installing `ember` itself:
-
-```
-pip install -r requirements.txt
-python setup.py install
-```
-
-```
-conda config --add channels conda-forge
-conda install --file requirements_conda.txt
-python setup.py install
-```
-
-### Notes on LIEF versions
-
-LIEF is now pinned to version 0.9.0 in the provided requirements files. This default behavior will allow new users to immediately reproduce EMBER version 2 features. LIEF 0.9.0 will not install on an M1 Mac, though. For those users, a Dockerfile is now included that installs the dependencies using conda.
-
-EMBER will work with more recent releases of LIEF, but keep in mind that models trained on features generated with one version of LIEF will have unpredictable results when evaluating on features generated with another.
-
-## Scripts
-
-The `train_ember.py` script simplifies the model training process. It will vectorize the ember features if necessary and then train the LightGBM model.
-
-```
-python train_ember.py [/path/to/dataset]
-```
-
-The `classify_binaries.py` script will return model predictions on PE files.
-
-```
-python classify_binaries.py -m [/path/to/model] BINARIES
-```
-
-## Import Usage
-
-The raw feature data can be expanded into vectorized form on disk for model training and into metadata form. These two functions create those extra files:
-
-```
-import ember
-ember.create_vectorized_features("/data/ember2018/")
-ember.create_metadata("/data/ember2018/")
-```
-
-Once created, that data can be read in using convenience functions:
-
-```
-import ember
-X_train, y_train, X_test, y_test = ember.read_vectorized_features("/data/ember2018/")
-metadata_dataframe = ember.read_metadata("/data/ember2018/")
-```
-
-Once the data is downloaded and the ember module is installed, this simple code should reproduce the benchmark ember model:
-
-```
-import ember
-ember.create_vectorized_features("/data/ember2018/")
-lgbm_model = ember.train_model("/data/ember2018/")
-```
-
-Once the model is trained, the ember module can be used to make a prediction on any input PE file:
-
-```
-import ember
-import lightgbm as lgb
-lgbm_model = lgb.Booster(model_file="/data/ember2018/ember_model_2018.txt")
-putty_data = open("~/putty.exe", "rb").read()
-print(ember.predict_sample(lgbm_model, putty_data))
-```
-
-## Citing
-
-If you use this data in a publication please cite the following [paper](https://arxiv.org/abs/1804.04637):
-
-```
-H. Anderson and P. Roth, "EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models”, in ArXiv e-prints. Apr. 2018.
-
-@ARTICLE{2018arXiv180404637A,
-  author = {{Anderson}, H.~S. and {Roth}, P.},
-  title = "{EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models}",
-  journal = {ArXiv e-prints},
-  archivePrefix = "arXiv",
-  eprint = {1804.04637},
-  primaryClass = "cs.CR",
-  keywords = {Computer Science - Cryptography and Security},
-  year = 2018,
-  month = apr,
-  adsurl = {http://adsabs.harvard.edu/abs/2018arXiv180404637A},
-}
-```
+Metadata-Version: 2.1
+Name: ember-mivia
+Version: 0.0.5
+Summary: Endgame Malware BEnchmark for Research
+Home-page: https://github.com/gparrella12/ember
+Author-email: proth@endgame.com
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+<img src="resources/logo.png" align="right" width="250px" height="250px">
+
+# Elastic Malware Benchmark for Empowering Researchers
+
+The EMBER dataset is a collection of features from PE files that serve as a benchmark dataset for researchers. The EMBER2017 dataset contained features from 1.1 million PE files scanned in or before 2017 and the EMBER2018 dataset contains features from 1 million PE files scanned in or before 2018. This repository makes it easy to reproducibly train the benchmark models, extend the provided feature set, or classify new PE files with the benchmark models.
+
+This paper describes many more details about the dataset: [https://arxiv.org/abs/1804.04637](https://arxiv.org/abs/1804.04637)
+
+## Features
+
+The [LIEF](https://lief.quarkslab.com/) project is used to extract features from PE files included in the EMBER dataset. Raw features are extracted to JSON format and included in the publicly available dataset. Vectorized features can be produced from these raw features and saved in binary format from which they can be converted to CSV, dataframe, or any other format. This repository makes it easy to generate raw features and/or vectorized features from any PE file. Researchers can implement their own features, or even vectorize the existing features differently from the existing implementations.
+
+The feature calculation is versioned. Feature version 1 is calculated with the LIEF library version 0.8.3. Feature version 2 includes the additional data directory feature, updated ordinal import processing, and is calculated with LIEF library version 0.9.0.  We have verified under Windows and Linux that LIEF provides consistent feature representation for version 2 features using LIEF version 0.10.1 and that it does not on a Mac.
+
+## Years
+
+The first EMBER dataset consisted of version 1 features calculated over samples collected in or before 2017. The second EMBER dataset release consisted of version 2 features calculated over samples collected in or before 2018. In conjunction with the second release, we also included the version 2 features from the samples collected in 2017. Combining the data from 2017 and 2018 will allow longer longitudinal studies of the evolution of features and PE file types. But different selection criteria were applied when choosing samples from 2017 and 2018. Specifically, the samples from 2018 were chosen so that the resultant training and test sets would be harder for machine learning algorithms to classify. Please beware of this inconsistancy while constructing your multi-year studies. The original paper only describes Ember 2017 (featur version 1). For a detailed information about the Ember 2018 dataset, please refer to https://www.camlis.org/2019/talks/roth where you can find both [slides](https://docs.google.com/presentation/d/1A13tsUkgWeujTy9SD-vDFfQp9fnIqbSE_tCihNPlArQ/edit#slide=id.g476bf81b41_0_446) and a [video talk](https://youtu.be/MsZmnUO5lkY).
+
+## Download
+
+Download the data here:
+
+| Year | Feature Version | Filename                     | URL                                                                                                            | sha256                                                             |
+|------|-----------------|------------------------------|----------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
+| 2017 | 1               | ember_dataset.tar.bz2        | [https://ember.elastic.co/ember_dataset.tar.bz2](https://ember.elastic.co/ember_dataset.tar.bz2)               | `a5603de2f34f02ab6e21df7a0f97ec4ac84ddc65caee33fb610093dd6f9e1df9` |
+| 2017 | 2               | ember_dataset_2017_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2017_2.tar.bz2](https://ember.elastic.co/ember_dataset_2017_2.tar.bz2) | `60142493c44c11bc3fef292b216a293841283d86ff58384b5dc2d88194c87a6d` |
+| 2018 | 2               | ember_dataset_2018_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2018_2.tar.bz2](https://ember.elastic.co/ember_dataset_2018_2.tar.bz2) | `b6052eb8d350a49a8d5a5396fbe7d16cf42848b86ff969b77464434cf2997812` |
+
+
+## Installation
+### Instrall directly from git
+Use `pip` to install the `ember` and required files
+
+```
+pip install git+https://github.com/elastic/ember.git
+```
+
+This provides access to EMBER feature extaction for example.  However, to use the scripts to train the model, one would instead clone the repository.
+
+
+### Install after cloning the EMBER repository
+Use `pip` or `conda` to install the required packages before installing `ember` itself:
+
+```
+pip install -r requirements.txt
+python setup.py install
+```
+
+```
+conda config --add channels conda-forge
+conda install --file requirements_conda.txt
+python setup.py install
+```
+
+### Notes on LIEF versions
+
+LIEF is now pinned to version 0.9.0 in the provided requirements files. This default behavior will allow new users to immediately reproduce EMBER version 2 features. LIEF 0.9.0 will not install on an M1 Mac, though. For those users, a Dockerfile is now included that installs the dependencies using conda.
+
+EMBER will work with more recent releases of LIEF, but keep in mind that models trained on features generated with one version of LIEF will have unpredictable results when evaluating on features generated with another.
+
+## Scripts
+
+The `train_ember.py` script simplifies the model training process. It will vectorize the ember features if necessary and then train the LightGBM model.
+
+```
+python train_ember.py [/path/to/dataset]
+```
+
+The `classify_binaries.py` script will return model predictions on PE files.
+
+```
+python classify_binaries.py -m [/path/to/model] BINARIES
+```
+
+## Import Usage
+
+The raw feature data can be expanded into vectorized form on disk for model training and into metadata form. These two functions create those extra files:
+
+```
+import ember
+ember.create_vectorized_features("/data/ember2018/")
+ember.create_metadata("/data/ember2018/")
+```
+
+Once created, that data can be read in using convenience functions:
+
+```
+import ember
+X_train, y_train, X_test, y_test = ember.read_vectorized_features("/data/ember2018/")
+metadata_dataframe = ember.read_metadata("/data/ember2018/")
+```
+
+Once the data is downloaded and the ember module is installed, this simple code should reproduce the benchmark ember model:
+
+```
+import ember
+ember.create_vectorized_features("/data/ember2018/")
+lgbm_model = ember.train_model("/data/ember2018/")
+```
+
+Once the model is trained, the ember module can be used to make a prediction on any input PE file:
+
+```
+import ember
+import lightgbm as lgb
+lgbm_model = lgb.Booster(model_file="/data/ember2018/ember_model_2018.txt")
+putty_data = open("~/putty.exe", "rb").read()
+print(ember.predict_sample(lgbm_model, putty_data))
+```
+
+## Citing
+
+If you use this data in a publication please cite the following [paper](https://arxiv.org/abs/1804.04637):
+
+```
+H. Anderson and P. Roth, "EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models”, in ArXiv e-prints. Apr. 2018.
+
+@ARTICLE{2018arXiv180404637A,
+  author = {{Anderson}, H.~S. and {Roth}, P.},
+  title = "{EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models}",
+  journal = {ArXiv e-prints},
+  archivePrefix = "arXiv",
+  eprint = {1804.04637},
+  primaryClass = "cs.CR",
+  keywords = {Computer Science - Cryptography and Security},
+  year = 2018,
+  month = apr,
+  adsurl = {http://adsabs.harvard.edu/abs/2018arXiv180404637A},
+}
+```
```

### Comparing `ember-mivia-0.0.4/ember/__init__.py` & `ember-mivia-0.0.5/ember/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,233 +1,233 @@
-# -*- coding: utf-8 -*-
-
-import os
-import json
-import tqdm
-import numpy as np
-import pandas as pd
-import lightgbm as lgb
-import multiprocessing
-from .features import PEFeatureExtractor
-from sklearn.model_selection import GridSearchCV
-from sklearn.model_selection import TimeSeriesSplit
-from sklearn.metrics import (roc_auc_score, make_scorer)
-
-
-def raw_feature_iterator(file_paths):
-    """
-    Yield raw feature strings from the inputed file paths
-    """
-    for path in file_paths:
-        with open(path, "r") as fin:
-            for line in fin:
-                yield line
-
-
-def vectorize(irow, raw_features_string, X_path, y_path, extractor, nrows):
-    """
-    Vectorize a single sample of raw features and write to a large numpy file
-    """
-    raw_features = json.loads(raw_features_string)
-    feature_vector = extractor.process_raw_features(raw_features)
-
-    y = np.memmap(y_path, dtype=np.float32, mode="r+", shape=nrows)
-    y[irow] = raw_features["label"]
-
-    X = np.memmap(X_path, dtype=np.float32, mode="r+", shape=(nrows, extractor.dim))
-    X[irow] = feature_vector
-
-
-def vectorize_unpack(args):
-    """
-    Pass through function for unpacking vectorize arguments
-    """
-    return vectorize(*args)
-
-
-def vectorize_subset(X_path, y_path, raw_feature_paths, extractor, nrows):
-    """
-    Vectorize a subset of data and write it to disk
-    """
-    # Create space on disk to write features to
-    X = np.memmap(X_path, dtype=np.float32, mode="w+", shape=(nrows, extractor.dim))
-    y = np.memmap(y_path, dtype=np.float32, mode="w+", shape=nrows)
-    del X, y
-
-    # Distribute the vectorization work
-    pool = multiprocessing.Pool()
-    argument_iterator = ((irow, raw_features_string, X_path, y_path, extractor, nrows)
-                         for irow, raw_features_string in enumerate(raw_feature_iterator(raw_feature_paths)))
-    for _ in tqdm.tqdm(pool.imap_unordered(vectorize_unpack, argument_iterator), total=nrows):
-        pass
-
-
-def create_vectorized_features(data_dir, feature_version=2):
-    """
-    Create feature vectors from raw features and write them to disk
-    """
-    extractor = PEFeatureExtractor(feature_version)
-
-    print("Vectorizing training set")
-    X_path = os.path.join(data_dir, "X_train.dat")
-    y_path = os.path.join(data_dir, "y_train.dat")
-    raw_feature_paths = [os.path.join(data_dir, "train_features_{}.jsonl".format(i)) for i in range(6)]
-    nrows = sum([1 for fp in raw_feature_paths for line in open(fp)])
-    vectorize_subset(X_path, y_path, raw_feature_paths, extractor, nrows)
-
-    print("Vectorizing test set")
-    X_path = os.path.join(data_dir, "X_test.dat")
-    y_path = os.path.join(data_dir, "y_test.dat")
-    raw_feature_paths = [os.path.join(data_dir, "test_features.jsonl")]
-    nrows = sum([1 for fp in raw_feature_paths for line in open(fp)])
-    vectorize_subset(X_path, y_path, raw_feature_paths, extractor, nrows)
-
-
-def read_vectorized_features(data_dir, subset=None, feature_version=2):
-    """
-    Read vectorized features into memory mapped numpy arrays
-    """
-    if subset is not None and subset not in ["train", "test"]:
-        return None
-
-    extractor = PEFeatureExtractor(feature_version)
-    ndim = extractor.dim
-    X_train = None
-    y_train = None
-    X_test = None
-    y_test = None
-
-    if subset is None or subset == "train":
-        X_train_path = os.path.join(data_dir, "X_train.dat")
-        y_train_path = os.path.join(data_dir, "y_train.dat")
-        y_train = np.memmap(y_train_path, dtype=np.float32, mode="r")
-        N = y_train.shape[0]
-        X_train = np.memmap(X_train_path, dtype=np.float32, mode="r", shape=(N, ndim))
-        if subset == "train":
-            return X_train, y_train
-
-    if subset is None or subset == "test":
-        X_test_path = os.path.join(data_dir, "X_test.dat")
-        y_test_path = os.path.join(data_dir, "y_test.dat")
-        y_test = np.memmap(y_test_path, dtype=np.float32, mode="r")
-        N = y_test.shape[0]
-        X_test = np.memmap(X_test_path, dtype=np.float32, mode="r", shape=(N, ndim))
-        if subset == "test":
-            return X_test, y_test
-
-    return X_train, y_train, X_test, y_test
-
-
-def read_metadata_record(raw_features_string):
-    """
-    Decode a raw features string and return the metadata fields
-    """
-    all_data = json.loads(raw_features_string)
-    metadata_keys = {"sha256", "appeared", "label", "avclass"}
-    return {k: all_data[k] for k in all_data.keys() & metadata_keys}
-
-
-def create_metadata(data_dir):
-    """
-    Write metadata to a csv file and return its dataframe
-    """
-    pool = multiprocessing.Pool()
-
-    train_feature_paths = [os.path.join(data_dir, "train_features_{}.jsonl".format(i)) for i in range(6)]
-    train_records = list(pool.imap(read_metadata_record, raw_feature_iterator(train_feature_paths)))
-
-    metadata_keys = ["sha256", "appeared", "label", "avclass"]
-    ordered_metadata_keys = [k for k in metadata_keys if k in train_records[0].keys()]
-
-    train_metadf = pd.DataFrame(train_records)[ordered_metadata_keys]
-    train_metadf.to_csv(os.path.join(data_dir, "train_metadata.csv"))
-
-    train_records = [dict(record, **{"subset": "train"}) for record in train_records]
-
-    test_feature_paths = [os.path.join(data_dir, "test_features.jsonl")]
-    test_records = list(pool.imap(read_metadata_record, raw_feature_iterator(test_feature_paths)))
-
-    test_metadf = pd.DataFrame(test_records)[ordered_metadata_keys]
-    test_metadf.to_csv(os.path.join(data_dir, "test_metadata.csv"))
-
-    test_records = [dict(record, **{"subset": "test"}) for record in test_records]
-
-    all_metadata_keys = ordered_metadata_keys + ["subset"]
-    metadf = pd.DataFrame(train_records + test_records)[all_metadata_keys]
-    metadf.to_csv(os.path.join(data_dir, "metadata.csv"))
-    return metadf
-
-
-def read_metadata(data_dir):
-    """
-    Read an already created metadata file and return its dataframe
-    """
-    return pd.read_csv(os.path.join(data_dir, "metadata.csv"), index_col=0)
-
-
-def optimize_model(data_dir):
-    """
-    Run a grid search to find the best LightGBM parameters
-    """
-    # Read data
-    X_train, y_train = read_vectorized_features(data_dir, subset="train")
-
-    # Filter unlabeled data
-    train_rows = (y_train != -1)
-
-    # read training dataset
-    X_train = X_train[train_rows]
-    y_train = y_train[train_rows]
-
-    # score by roc auc
-    # we're interested in low FPR rates, so we'll consider only the AUC for FPRs in [0,5e-3]
-    score = make_scorer(roc_auc_score, max_fpr=5e-3)
-
-    # define search grid
-    param_grid = {
-        'boosting_type': ['gbdt'],
-        'objective': ['binary'],
-        'num_iterations': [500, 1000],
-        'learning_rate': [0.005, 0.05],
-        'num_leaves': [512, 1024, 2048],
-        'feature_fraction': [0.5, 0.8, 1.0],
-        'bagging_fraction': [0.5, 0.8, 1.0]
-    }
-    model = lgb.LGBMClassifier(boosting_type="gbdt", n_jobs=-1, silent=True)
-
-    # each row in X_train appears in chronological order of "appeared"
-    # so this works for progrssive time series splitting
-    progressive_cv = TimeSeriesSplit(n_splits=3).split(X_train)
-
-    grid = GridSearchCV(estimator=model, cv=progressive_cv, param_grid=param_grid, scoring=score, n_jobs=1, verbose=3)
-    grid.fit(X_train, y_train)
-
-    return grid.best_params_
-
-
-def train_model(data_dir, params={}, feature_version=2):
-    """
-    Train the LightGBM model from the EMBER dataset from the vectorized features
-    """
-    # update params
-    params.update({"application": "binary"})
-
-    # Read data
-    X_train, y_train = read_vectorized_features(data_dir, "train", feature_version)
-
-    # Filter unlabeled data
-    train_rows = (y_train != -1)
-
-    # Train
-    lgbm_dataset = lgb.Dataset(X_train[train_rows], y_train[train_rows])
-    lgbm_model = lgb.train(params, lgbm_dataset)
-
-    return lgbm_model
-
-
-def predict_sample(lgbm_model, file_data, feature_version=2):
-    """
-    Predict a PE file with an LightGBM model
-    """
-    extractor = PEFeatureExtractor(feature_version)
-    features = np.array(extractor.feature_vector(file_data), dtype=np.float32)
-    return lgbm_model.predict([features])[0]
+# -*- coding: utf-8 -*-
+
+import os
+import json
+import tqdm
+import numpy as np
+import pandas as pd
+import lightgbm as lgb
+import multiprocessing
+from .features import PEFeatureExtractor
+from sklearn.model_selection import GridSearchCV
+from sklearn.model_selection import TimeSeriesSplit
+from sklearn.metrics import (roc_auc_score, make_scorer)
+
+
+def raw_feature_iterator(file_paths):
+    """
+    Yield raw feature strings from the inputed file paths
+    """
+    for path in file_paths:
+        with open(path, "r") as fin:
+            for line in fin:
+                yield line
+
+
+def vectorize(irow, raw_features_string, X_path, y_path, extractor, nrows):
+    """
+    Vectorize a single sample of raw features and write to a large numpy file
+    """
+    raw_features = json.loads(raw_features_string)
+    feature_vector = extractor.process_raw_features(raw_features)
+
+    y = np.memmap(y_path, dtype=np.float32, mode="r+", shape=nrows)
+    y[irow] = raw_features["label"]
+
+    X = np.memmap(X_path, dtype=np.float32, mode="r+", shape=(nrows, extractor.dim))
+    X[irow] = feature_vector
+
+
+def vectorize_unpack(args):
+    """
+    Pass through function for unpacking vectorize arguments
+    """
+    return vectorize(*args)
+
+
+def vectorize_subset(X_path, y_path, raw_feature_paths, extractor, nrows):
+    """
+    Vectorize a subset of data and write it to disk
+    """
+    # Create space on disk to write features to
+    X = np.memmap(X_path, dtype=np.float32, mode="w+", shape=(nrows, extractor.dim))
+    y = np.memmap(y_path, dtype=np.float32, mode="w+", shape=nrows)
+    del X, y
+
+    # Distribute the vectorization work
+    pool = multiprocessing.Pool()
+    argument_iterator = ((irow, raw_features_string, X_path, y_path, extractor, nrows)
+                         for irow, raw_features_string in enumerate(raw_feature_iterator(raw_feature_paths)))
+    for _ in tqdm.tqdm(pool.imap_unordered(vectorize_unpack, argument_iterator), total=nrows):
+        pass
+
+
+def create_vectorized_features(data_dir, feature_version=2):
+    """
+    Create feature vectors from raw features and write them to disk
+    """
+    extractor = PEFeatureExtractor(feature_version)
+
+    print("Vectorizing training set")
+    X_path = os.path.join(data_dir, "X_train.dat")
+    y_path = os.path.join(data_dir, "y_train.dat")
+    raw_feature_paths = [os.path.join(data_dir, "train_features_{}.jsonl".format(i)) for i in range(6)]
+    nrows = sum([1 for fp in raw_feature_paths for line in open(fp)])
+    vectorize_subset(X_path, y_path, raw_feature_paths, extractor, nrows)
+
+    print("Vectorizing test set")
+    X_path = os.path.join(data_dir, "X_test.dat")
+    y_path = os.path.join(data_dir, "y_test.dat")
+    raw_feature_paths = [os.path.join(data_dir, "test_features.jsonl")]
+    nrows = sum([1 for fp in raw_feature_paths for line in open(fp)])
+    vectorize_subset(X_path, y_path, raw_feature_paths, extractor, nrows)
+
+
+def read_vectorized_features(data_dir, subset=None, feature_version=2):
+    """
+    Read vectorized features into memory mapped numpy arrays
+    """
+    if subset is not None and subset not in ["train", "test"]:
+        return None
+
+    extractor = PEFeatureExtractor(feature_version)
+    ndim = extractor.dim
+    X_train = None
+    y_train = None
+    X_test = None
+    y_test = None
+
+    if subset is None or subset == "train":
+        X_train_path = os.path.join(data_dir, "X_train.dat")
+        y_train_path = os.path.join(data_dir, "y_train.dat")
+        y_train = np.memmap(y_train_path, dtype=np.float32, mode="r")
+        N = y_train.shape[0]
+        X_train = np.memmap(X_train_path, dtype=np.float32, mode="r", shape=(N, ndim))
+        if subset == "train":
+            return X_train, y_train
+
+    if subset is None or subset == "test":
+        X_test_path = os.path.join(data_dir, "X_test.dat")
+        y_test_path = os.path.join(data_dir, "y_test.dat")
+        y_test = np.memmap(y_test_path, dtype=np.float32, mode="r")
+        N = y_test.shape[0]
+        X_test = np.memmap(X_test_path, dtype=np.float32, mode="r", shape=(N, ndim))
+        if subset == "test":
+            return X_test, y_test
+
+    return X_train, y_train, X_test, y_test
+
+
+def read_metadata_record(raw_features_string):
+    """
+    Decode a raw features string and return the metadata fields
+    """
+    all_data = json.loads(raw_features_string)
+    metadata_keys = {"sha256", "appeared", "label", "avclass"}
+    return {k: all_data[k] for k in all_data.keys() & metadata_keys}
+
+
+def create_metadata(data_dir):
+    """
+    Write metadata to a csv file and return its dataframe
+    """
+    pool = multiprocessing.Pool()
+
+    train_feature_paths = [os.path.join(data_dir, "train_features_{}.jsonl".format(i)) for i in range(6)]
+    train_records = list(pool.imap(read_metadata_record, raw_feature_iterator(train_feature_paths)))
+
+    metadata_keys = ["sha256", "appeared", "label", "avclass"]
+    ordered_metadata_keys = [k for k in metadata_keys if k in train_records[0].keys()]
+
+    train_metadf = pd.DataFrame(train_records)[ordered_metadata_keys]
+    train_metadf.to_csv(os.path.join(data_dir, "train_metadata.csv"))
+
+    train_records = [dict(record, **{"subset": "train"}) for record in train_records]
+
+    test_feature_paths = [os.path.join(data_dir, "test_features.jsonl")]
+    test_records = list(pool.imap(read_metadata_record, raw_feature_iterator(test_feature_paths)))
+
+    test_metadf = pd.DataFrame(test_records)[ordered_metadata_keys]
+    test_metadf.to_csv(os.path.join(data_dir, "test_metadata.csv"))
+
+    test_records = [dict(record, **{"subset": "test"}) for record in test_records]
+
+    all_metadata_keys = ordered_metadata_keys + ["subset"]
+    metadf = pd.DataFrame(train_records + test_records)[all_metadata_keys]
+    metadf.to_csv(os.path.join(data_dir, "metadata.csv"))
+    return metadf
+
+
+def read_metadata(data_dir):
+    """
+    Read an already created metadata file and return its dataframe
+    """
+    return pd.read_csv(os.path.join(data_dir, "metadata.csv"), index_col=0)
+
+
+def optimize_model(data_dir):
+    """
+    Run a grid search to find the best LightGBM parameters
+    """
+    # Read data
+    X_train, y_train = read_vectorized_features(data_dir, subset="train")
+
+    # Filter unlabeled data
+    train_rows = (y_train != -1)
+
+    # read training dataset
+    X_train = X_train[train_rows]
+    y_train = y_train[train_rows]
+
+    # score by roc auc
+    # we're interested in low FPR rates, so we'll consider only the AUC for FPRs in [0,5e-3]
+    score = make_scorer(roc_auc_score, max_fpr=5e-3)
+
+    # define search grid
+    param_grid = {
+        'boosting_type': ['gbdt'],
+        'objective': ['binary'],
+        'num_iterations': [500, 1000],
+        'learning_rate': [0.005, 0.05],
+        'num_leaves': [512, 1024, 2048],
+        'feature_fraction': [0.5, 0.8, 1.0],
+        'bagging_fraction': [0.5, 0.8, 1.0]
+    }
+    model = lgb.LGBMClassifier(boosting_type="gbdt", n_jobs=-1, silent=True)
+
+    # each row in X_train appears in chronological order of "appeared"
+    # so this works for progrssive time series splitting
+    progressive_cv = TimeSeriesSplit(n_splits=3).split(X_train)
+
+    grid = GridSearchCV(estimator=model, cv=progressive_cv, param_grid=param_grid, scoring=score, n_jobs=1, verbose=3)
+    grid.fit(X_train, y_train)
+
+    return grid.best_params_
+
+
+def train_model(data_dir, params={}, feature_version=2):
+    """
+    Train the LightGBM model from the EMBER dataset from the vectorized features
+    """
+    # update params
+    params.update({"application": "binary"})
+
+    # Read data
+    X_train, y_train = read_vectorized_features(data_dir, "train", feature_version)
+
+    # Filter unlabeled data
+    train_rows = (y_train != -1)
+
+    # Train
+    lgbm_dataset = lgb.Dataset(X_train[train_rows], y_train[train_rows])
+    lgbm_model = lgb.train(params, lgbm_dataset)
+
+    return lgbm_model
+
+
+def predict_sample(lgbm_model, file_data, feature_version=2):
+    """
+    Predict a PE file with an LightGBM model
+    """
+    extractor = PEFeatureExtractor(feature_version)
+    features = np.array(extractor.feature_vector(file_data), dtype=np.float32)
+    return lgbm_model.predict([features])[0]
```

### Comparing `ember-mivia-0.0.4/ember/features.py` & `ember-mivia-0.0.5/ember/features.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,656 +1,660 @@
-#!/usr/bin/python
-''' Extracts some basic features from PE files. Many of the features
-implemented have been used in previously published works. For more information,
-check out the following resources:
-* Schultz, et al., 2001: http://128.59.14.66/sites/default/files/binaryeval-ieeesp01.pdf
-* Kolter and Maloof, 2006: http://www.jmlr.org/papers/volume7/kolter06a/kolter06a.pdf
-* Shafiq et al., 2009: https://www.researchgate.net/profile/Fauzan_Mirza/publication/242084613_A_Framework_for_Efficient_Mining_of_Structural_Information_to_Detect_Zero-Day_Malicious_Portable_Executables/links/0c96052e191668c3d5000000.pdf
-* Raman, 2012: http://2012.infosecsouthwest.com/files/speaker_materials/ISSW2012_Selecting_Features_to_Classify_Malware.pdf
-* Saxe and Berlin, 2015: https://arxiv.org/pdf/1508.03096.pdf
-
-It may be useful to do feature selection to reduce this set of features to a meaningful set
-for your modeling problem.
-'''
-
-import re
-import lief
-import hashlib
-import numpy as np
-import os
-import json
-from sklearn.feature_extraction import FeatureHasher
-
-LIEF_MAJOR, LIEF_MINOR, _ = lief.__version__.split('.')
-LIEF_EXPORT_OBJECT = int(LIEF_MAJOR) > 0 or ( int(LIEF_MAJOR)==0 and int(LIEF_MINOR) >= 10 )
-LIEF_HAS_SIGNATURE = int(LIEF_MAJOR) > 0 or (int(LIEF_MAJOR) == 0 and int(LIEF_MINOR) >= 11)
-
-
-class FeatureType(object):
-    ''' Base class from which each feature type may inherit '''
-
-    name = ''
-    dim = 0
-
-    def __repr__(self):
-        return '{}({})'.format(self.name, self.dim)
-
-    def raw_features(self, bytez, lief_binary):
-        ''' Generate a JSON-able representation of the file '''
-        raise (NotImplementedError)
-
-    def process_raw_features(self, raw_obj):
-        ''' Generate a feature vector from the raw features '''
-        raise (NotImplementedError)
-
-    def feature_vector(self, bytez, lief_binary):
-        ''' Directly calculate the feature vector from the sample itself. This should only be implemented differently
-        if there are significant speedups to be gained from combining the two functions. '''
-        return self.process_raw_features(self.raw_features(bytez, lief_binary))
-
-
-class ByteHistogram(FeatureType):
-    ''' Byte histogram (count + non-normalized) over the entire binary file '''
-
-    name = 'histogram'
-    dim = 256
-
-    def __init__(self):
-        super(FeatureType, self).__init__()
-
-    def raw_features(self, bytez, lief_binary):
-        counts = np.bincount(np.frombuffer(bytez, dtype=np.uint8), minlength=256)
-        return counts.tolist()
-
-    def process_raw_features(self, raw_obj):
-        counts = np.array(raw_obj, dtype=np.float32)
-        sum = counts.sum()
-        normalized = counts / sum
-        return normalized
-
-
-class ByteEntropyHistogram(FeatureType):
-    ''' 2d byte/entropy histogram based loosely on (Saxe and Berlin, 2015).
-    This roughly approximates the joint probability of byte value and local entropy.
-    See Section 2.1.1 in https://arxiv.org/pdf/1508.03096.pdf for more info.
-    '''
-
-    name = 'byteentropy'
-    dim = 256
-
-    def __init__(self, step=1024, window=2048):
-        super(FeatureType, self).__init__()
-        self.window = window
-        self.step = step
-
-    def _entropy_bin_counts(self, block):
-        # coarse histogram, 16 bytes per bin
-        c = np.bincount(block >> 4, minlength=16)  # 16-bin histogram
-        p = c.astype(np.float32) / self.window
-        wh = np.where(c)[0]
-        H = np.sum(-p[wh] * np.log2(
-            p[wh])) * 2  # * x2 b.c. we reduced information by half: 256 bins (8 bits) to 16 bins (4 bits)
-
-        Hbin = int(H * 2)  # up to 16 bins (max entropy is 8 bits)
-        if Hbin == 16:  # handle entropy = 8.0 bits
-            Hbin = 15
-
-        return Hbin, c
-
-    def raw_features(self, bytez, lief_binary):
-        output = np.zeros((16, 16), dtype=np.int64)
-        a = np.frombuffer(bytez, dtype=np.uint8)
-        if a.shape[0] < self.window:
-            Hbin, c = self._entropy_bin_counts(a)
-            output[Hbin, :] += c
-        else:
-            # strided trick from here: http://www.rigtorp.se/2011/01/01/rolling-statistics-numpy.html
-            shape = a.shape[:-1] + (a.shape[-1] - self.window + 1, self.window)
-            strides = a.strides + (a.strides[-1],)
-            blocks = np.lib.stride_tricks.as_strided(a, shape=shape, strides=strides)[::self.step, :]
-
-            # from the blocks, compute histogram
-            for block in blocks:
-                Hbin, c = self._entropy_bin_counts(block)
-                output[Hbin, :] += c
-
-        return output.flatten().tolist()
-
-    def process_raw_features(self, raw_obj):
-        counts = np.array(raw_obj, dtype=np.float32)
-        sum = counts.sum()
-        normalized = counts / sum
-        return normalized
-
-
-class SectionInfo(FeatureType):
-    ''' Information about section names, sizes and entropy.  Uses hashing trick
-    to summarize all this section info into a feature vector.
-    '''
-
-    name = 'section'
-    dim = 5 + 50 + 50 + 50 + 50 + 50
-
-    def __init__(self):
-        super(FeatureType, self).__init__()
-
-    @staticmethod
-    def _properties(s):
-        return [str(c).split('.')[-1] for c in s.characteristics_lists]
-
-    def raw_features(self, bytez, lief_binary):
-        if lief_binary is None:
-            return {"entry": "", "sections": []}
-
-        # properties of entry point, or if invalid, the first executable section
-
-        try:
-            if int(LIEF_MAJOR) > 0 or (int(LIEF_MAJOR) == 0 and int(LIEF_MINOR) >= 12):
-                section = lief_binary.section_from_rva(lief_binary.entrypoint - lief_binary.imagebase)
-                if section is None:
-                    raise lief.not_found
-                entry_section = section.name
-            else: # lief < 0.12
-                entry_section = lief_binary.section_from_offset(lief_binary.entrypoint).name
-        except lief.not_found:
-                # bad entry point, let's find the first executable section
-                entry_section = ""
-                for s in lief_binary.sections:
-                    if lief.PE.SECTION_CHARACTERISTICS.MEM_EXECUTE in s.characteristics_lists:
-                        entry_section = s.name
-                        break
-
-        raw_obj = {"entry": entry_section}
-        raw_obj["sections"] = [{
-            'name': s.name,
-            'size': s.size,
-            'entropy': s.entropy,
-            'vsize': s.virtual_size,
-            'props': self._properties(s)
-        } for s in lief_binary.sections]
-        return raw_obj
-
-    def process_raw_features(self, raw_obj):
-        sections = raw_obj['sections']
-        general = [
-            len(sections),  # total number of sections
-            # number of sections with zero size
-            sum(1 for s in sections if s['size'] == 0),
-            # number of sections with an empty name
-            sum(1 for s in sections if s['name'] == ""),
-            # number of RX
-            sum(1 for s in sections if 'MEM_READ' in s['props'] and 'MEM_EXECUTE' in s['props']),
-            # number of W
-            sum(1 for s in sections if 'MEM_WRITE' in s['props'])
-        ]
-        # gross characteristics of each section
-        section_sizes = [(s['name'], s['size']) for s in sections]
-        section_sizes_hashed = FeatureHasher(50, input_type="pair").transform([section_sizes]).toarray()[0]
-        section_entropy = [(s['name'], s['entropy']) for s in sections]
-        section_entropy_hashed = FeatureHasher(50, input_type="pair").transform([section_entropy]).toarray()[0]
-        section_vsize = [(s['name'], s['vsize']) for s in sections]
-        section_vsize_hashed = FeatureHasher(50, input_type="pair").transform([section_vsize]).toarray()[0]
-        entry_name_hashed = FeatureHasher(50, input_type="string").transform([ [raw_obj['entry']] ]).toarray()[0]
-        characteristics = [p for s in sections for p in s['props'] if s['name'] == raw_obj['entry']]
-        characteristics_hashed = FeatureHasher(50, input_type="string").transform([characteristics]).toarray()[0]
-
-        return np.hstack([
-            general, section_sizes_hashed, section_entropy_hashed, section_vsize_hashed, entry_name_hashed,
-            characteristics_hashed
-        ]).astype(np.float32)
-
-
-class ImportsInfo(FeatureType):
-    ''' Information about imported libraries and functions from the
-    import address table.  Note that the total number of imported
-    functions is contained in GeneralFileInfo.
-    '''
-
-    name = 'imports'
-    dim = 1280
-
-    def __init__(self):
-        super(FeatureType, self).__init__()
-
-    def raw_features(self, bytez, lief_binary):
-        imports = {}
-        if lief_binary is None:
-            return imports
-
-        for lib in lief_binary.imports:
-            if lib.name not in imports:
-                imports[lib.name] = []  # libraries can be duplicated in listing, extend instead of overwrite
-
-            # Clipping assumes there are diminishing returns on the discriminatory power of imported functions
-            #  beyond the first 10000 characters, and this will help limit the dataset size
-            for entry in lib.entries:
-                if entry.is_ordinal:
-                    imports[lib.name].append("ordinal" + str(entry.ordinal))
-                else:
-                    imports[lib.name].append(entry.name[:10000])
-
-        return imports
-
-    def process_raw_features(self, raw_obj):
-        # unique libraries
-        libraries = list(set([l.lower() for l in raw_obj.keys()]))
-        libraries_hashed = FeatureHasher(256, input_type="string").transform([libraries]).toarray()[0]
-
-        # A string like "kernel32.dll:CreateFileMappingA" for each imported function
-        imports = [lib.lower() + ':' + e for lib, elist in raw_obj.items() for e in elist]
-        imports_hashed = FeatureHasher(1024, input_type="string").transform([imports]).toarray()[0]
-
-        # Two separate elements: libraries (alone) and fully-qualified names of imported functions
-        return np.hstack([libraries_hashed, imports_hashed]).astype(np.float32)
-
-
-class ExportsInfo(FeatureType):
-    ''' Information about exported functions. Note that the total number of exported
-    functions is contained in GeneralFileInfo.
-    '''
-
-    name = 'exports'
-    dim = 128
-
-    def __init__(self):
-        super(FeatureType, self).__init__()
-
-    def raw_features(self, bytez, lief_binary):
-        if lief_binary is None:
-            return []
-
-        # Clipping assumes there are diminishing returns on the discriminatory power of exports beyond
-        #  the first 10000 characters, and this will help limit the dataset size
-        if LIEF_EXPORT_OBJECT:
-            # export is an object with .name attribute (0.10.0 and later)
-            clipped_exports = [export.name[:10000] for export in lief_binary.exported_functions]
-        else:
-            # export is a string (LIEF 0.9.0 and earlier)
-            clipped_exports = [export[:10000] for export in lief_binary.exported_functions]
-
-
-        return clipped_exports
-
-    def process_raw_features(self, raw_obj):
-        exports_hashed = FeatureHasher(128, input_type="string").transform([raw_obj]).toarray()[0]
-        return exports_hashed.astype(np.float32)
-
-
-class GeneralFileInfo(FeatureType):
-    ''' General information about the file '''
-
-    name = 'general'
-    dim = 10
-
-    def __init__(self):
-        super(FeatureType, self).__init__()
-
-    def raw_features(self, bytez, lief_binary):
-        if lief_binary is None:
-            return {
-                'size': len(bytez),
-                'vsize': 0,
-                'has_debug': 0,
-                'exports': 0,
-                'imports': 0,
-                'has_relocations': 0,
-                'has_resources': 0,
-                'has_signature': 0,
-                'has_tls': 0,
-                'symbols': 0
-            }
-
-        return {
-            'size': len(bytez),
-            'vsize': lief_binary.virtual_size,
-            'has_debug': int(lief_binary.has_debug),
-            'exports': len(lief_binary.exported_functions),
-            'imports': len(lief_binary.imported_functions),
-            'has_relocations': int(lief_binary.has_relocations),
-            'has_resources': int(lief_binary.has_resources),
-            'has_signature': int(lief_binary.has_signatures) if LIEF_HAS_SIGNATURE else int(lief_binary.has_signature),
-            'has_tls': int(lief_binary.has_tls),
-            'symbols': len(lief_binary.symbols),
-        }
-
-    def process_raw_features(self, raw_obj):
-        return np.asarray([
-            raw_obj['size'], raw_obj['vsize'], raw_obj['has_debug'], raw_obj['exports'], raw_obj['imports'],
-            raw_obj['has_relocations'], raw_obj['has_resources'], raw_obj['has_signature'], raw_obj['has_tls'],
-            raw_obj['symbols']
-        ],
-                          dtype=np.float32)
-
-
-class HeaderFileInfo(FeatureType):
-    ''' Machine, architecure, OS, linker and other information extracted from header '''
-
-    name = 'header'
-    dim = 62
-
-    def __init__(self):
-        super(FeatureType, self).__init__()
-
-    def raw_features(self, bytez, lief_binary):
-        raw_obj = {}
-        raw_obj['coff'] = {'timestamp': 0, 'machine': "", 'characteristics': []}
-        raw_obj['optional'] = {
-            'subsystem': "",
-            'dll_characteristics': [],
-            'magic': "",
-            'major_image_version': 0,
-            'minor_image_version': 0,
-            'major_linker_version': 0,
-            'minor_linker_version': 0,
-            'major_operating_system_version': 0,
-            'minor_operating_system_version': 0,
-            'major_subsystem_version': 0,
-            'minor_subsystem_version': 0,
-            'sizeof_code': 0,
-            'sizeof_headers': 0,
-            'sizeof_heap_commit': 0
-        }
-        if lief_binary is None:
-            return raw_obj
-
-        raw_obj['coff']['timestamp'] = lief_binary.header.time_date_stamps
-        raw_obj['coff']['machine'] = str(lief_binary.header.machine).split('.')[-1]
-        raw_obj['coff']['characteristics'] = [str(c).split('.')[-1] for c in lief_binary.header.characteristics_list]
-        raw_obj['optional']['subsystem'] = str(lief_binary.optional_header.subsystem).split('.')[-1]
-        raw_obj['optional']['dll_characteristics'] = [
-            str(c).split('.')[-1] for c in lief_binary.optional_header.dll_characteristics_lists
-        ]
-        raw_obj['optional']['magic'] = str(lief_binary.optional_header.magic).split('.')[-1]
-        raw_obj['optional']['major_image_version'] = lief_binary.optional_header.major_image_version
-        raw_obj['optional']['minor_image_version'] = lief_binary.optional_header.minor_image_version
-        raw_obj['optional']['major_linker_version'] = lief_binary.optional_header.major_linker_version
-        raw_obj['optional']['minor_linker_version'] = lief_binary.optional_header.minor_linker_version
-        raw_obj['optional'][
-            'major_operating_system_version'] = lief_binary.optional_header.major_operating_system_version
-        raw_obj['optional'][
-            'minor_operating_system_version'] = lief_binary.optional_header.minor_operating_system_version
-        raw_obj['optional']['major_subsystem_version'] = lief_binary.optional_header.major_subsystem_version
-        raw_obj['optional']['minor_subsystem_version'] = lief_binary.optional_header.minor_subsystem_version
-        raw_obj['optional']['sizeof_code'] = lief_binary.optional_header.sizeof_code
-        raw_obj['optional']['sizeof_headers'] = lief_binary.optional_header.sizeof_headers
-        raw_obj['optional']['sizeof_heap_commit'] = lief_binary.optional_header.sizeof_heap_commit
-        return raw_obj
-
-    def process_raw_features(self, raw_obj):
-        return np.hstack([
-            raw_obj['coff']['timestamp'],
-            FeatureHasher(10, input_type="string").transform([[raw_obj['coff']['machine']]]).toarray()[0],
-            FeatureHasher(10, input_type="string").transform([raw_obj['coff']['characteristics']]).toarray()[0],
-            FeatureHasher(10, input_type="string").transform([[raw_obj['optional']['subsystem']]]).toarray()[0],
-            FeatureHasher(10, input_type="string").transform([raw_obj['optional']['dll_characteristics']]).toarray()[0],
-            FeatureHasher(10, input_type="string").transform([[raw_obj['optional']['magic']]]).toarray()[0],
-            raw_obj['optional']['major_image_version'],
-            raw_obj['optional']['minor_image_version'],
-            raw_obj['optional']['major_linker_version'],
-            raw_obj['optional']['minor_linker_version'],
-            raw_obj['optional']['major_operating_system_version'],
-            raw_obj['optional']['minor_operating_system_version'],
-            raw_obj['optional']['major_subsystem_version'],
-            raw_obj['optional']['minor_subsystem_version'],
-            raw_obj['optional']['sizeof_code'],
-            raw_obj['optional']['sizeof_headers'],
-            raw_obj['optional']['sizeof_heap_commit'],
-        ]).astype(np.float32)
-        
-        
-    def get_features_index(self, raw_obj):
-        features_list = [
-            raw_obj['coff']['timestamp'],
-            FeatureHasher(10, input_type="string").transform([[raw_obj['coff']['machine']]]).toarray()[0],
-            FeatureHasher(10, input_type="string").transform([raw_obj['coff']['characteristics']]).toarray()[0],
-            FeatureHasher(10, input_type="string").transform([[raw_obj['optional']['subsystem']]]).toarray()[0],
-            FeatureHasher(10, input_type="string").transform([raw_obj['optional']['dll_characteristics']]).toarray()[0],
-            FeatureHasher(10, input_type="string").transform([[raw_obj['optional']['magic']]]).toarray()[0],
-            raw_obj['optional']['major_image_version'],
-            raw_obj['optional']['minor_image_version'],
-            raw_obj['optional']['major_linker_version'],
-            raw_obj['optional']['minor_linker_version'],
-            raw_obj['optional']['major_operating_system_version'],
-            raw_obj['optional']['minor_operating_system_version'],
-            raw_obj['optional']['major_subsystem_version'],
-            raw_obj['optional']['minor_subsystem_version'],
-            raw_obj['optional']['sizeof_code'],
-            raw_obj['optional']['sizeof_headers'],
-            raw_obj['optional']['sizeof_heap_commit'],
-        ]
-        keys_list = [
-            'coff-timestamp',
-            'coff-machine',
-            'coff-characteristics',
-            'optional-subsystem',
-            'optional-dll_characteristics',
-            'optional-magic',
-            'optional-major_image_version',
-            'optional-minor_image_version',
-            'optional-major_linker_version',
-            'optional-minor_linker_version',
-            'optional-major_operating_system_version',
-            'optional-minor_operating_system_version',
-            'optional-major_subsystem_version',
-            'optional-minor_subsystem_version',
-            'optional-sizeof_code',
-            'optional-sizeof_headers',
-            'optional-sizeof_heap_commit',
-        ]
-
-        rv = {}
-        index = 0
-        for i in range(len(features_list)):
-            try:
-                if len(features_list[i]) > 1:
-                    rv[keys_list[i]] = (index, index+len(features_list[i]))
-                    index += len(features_list[i])
-            except TypeError:
-                    rv[keys_list[i]] = index
-                    index += 1
-        return rv
-        
-        
-class StringExtractor(FeatureType):
-    ''' Extracts strings from raw byte stream '''
-
-    name = 'strings'
-    dim = 1 + 1 + 1 + 96 + 1 + 1 + 1 + 1 + 1
-
-    def __init__(self):
-        super(FeatureType, self).__init__()
-        # all consecutive runs of 0x20 - 0x7f that are 5+ characters
-        self._allstrings = re.compile(b'[\x20-\x7f]{5,}')
-        # occurances of the string 'C:\'.  Not actually extracting the path
-        self._paths = re.compile(b'c:\\\\', re.IGNORECASE)
-        # occurances of http:// or https://.  Not actually extracting the URLs
-        self._urls = re.compile(b'https?://', re.IGNORECASE)
-        # occurances of the string prefix HKEY_.  No actually extracting registry names
-        self._registry = re.compile(b'HKEY_')
-        # crude evidence of an MZ header (dropper?) somewhere in the byte stream
-        self._mz = re.compile(b'MZ')
-
-    def raw_features(self, bytez, lief_binary):
-        allstrings = self._allstrings.findall(bytez)
-        if allstrings:
-            # statistics about strings:
-            string_lengths = [len(s) for s in allstrings]
-            avlength = sum(string_lengths) / len(string_lengths)
-            # map printable characters 0x20 - 0x7f to an int array consisting of 0-95, inclusive
-            as_shifted_string = [b - ord(b'\x20') for b in b''.join(allstrings)]
-            c = np.bincount(as_shifted_string, minlength=96)  # histogram count
-            # distribution of characters in printable strings
-            csum = c.sum()
-            p = c.astype(np.float32) / csum
-            wh = np.where(c)[0]
-            H = np.sum(-p[wh] * np.log2(p[wh]))  # entropy
-        else:
-            avlength = 0
-            c = np.zeros((96,), dtype=np.float32)
-            H = 0
-            csum = 0
-
-        return {
-            'numstrings': len(allstrings),
-            'avlength': avlength,
-            'printabledist': c.tolist(),  # store non-normalized histogram
-            'printables': int(csum),
-            'entropy': float(H),
-            'paths': len(self._paths.findall(bytez)),
-            'urls': len(self._urls.findall(bytez)),
-            'registry': len(self._registry.findall(bytez)),
-            'MZ': len(self._mz.findall(bytez))
-        }
-
-    def process_raw_features(self, raw_obj):
-        hist_divisor = float(raw_obj['printables']) if raw_obj['printables'] > 0 else 1.0
-        return np.hstack([
-            raw_obj['numstrings'], raw_obj['avlength'], raw_obj['printables'],
-            np.asarray(raw_obj['printabledist']) / hist_divisor, raw_obj['entropy'], raw_obj['paths'], raw_obj['urls'],
-            raw_obj['registry'], raw_obj['MZ']
-        ]).astype(np.float32)
-
-
-class DataDirectories(FeatureType):
-    ''' Extracts size and virtual address of the first 15 data directories '''
-
-    name = 'datadirectories'
-    dim = 15 * 2
-
-    def __init__(self):
-        super(FeatureType, self).__init__()
-        self._name_order = [
-            "EXPORT_TABLE", "IMPORT_TABLE", "RESOURCE_TABLE", "EXCEPTION_TABLE", "CERTIFICATE_TABLE",
-            "BASE_RELOCATION_TABLE", "DEBUG", "ARCHITECTURE", "GLOBAL_PTR", "TLS_TABLE", "LOAD_CONFIG_TABLE",
-            "BOUND_IMPORT", "IAT", "DELAY_IMPORT_DESCRIPTOR", "CLR_RUNTIME_HEADER"
-        ]
-
-    def raw_features(self, bytez, lief_binary):
-        output = []
-        if lief_binary is None:
-            return output
-
-        for data_directory in lief_binary.data_directories:
-            output.append({
-                "name": str(data_directory.type).replace("DATA_DIRECTORY.", ""),
-                "size": data_directory.size,
-                "virtual_address": data_directory.rva
-            })
-        return output
-
-    def process_raw_features(self, raw_obj):
-        features = np.zeros(2 * len(self._name_order), dtype=np.float32)
-        for i in range(len(self._name_order)):
-            if i < len(raw_obj):
-                features[2 * i] = raw_obj[i]["size"]
-                features[2 * i + 1] = raw_obj[i]["virtual_address"]
-        return features
-
-
-class PEFeatureExtractor(object):
-    ''' Extract useful features from a PE file, and return as a vector of fixed size. '''
-
-    def __init__(self, feature_version=2, print_feature_warning=True, features_file=''):
-        self.features = []
-        features = {
-                    'ByteHistogram': ByteHistogram(),
-                    'ByteEntropyHistogram': ByteEntropyHistogram(),
-                    'StringExtractor': StringExtractor(),
-                    'GeneralFileInfo': GeneralFileInfo(),
-                    'HeaderFileInfo': HeaderFileInfo(),
-                    'SectionInfo': SectionInfo(),
-                    'ImportsInfo': ImportsInfo(),
-                    'ExportsInfo': ExportsInfo()
-            }
-
-        if os.path.exists(features_file):
-            with open(features_file, encoding='utf8') as f:
-                x = json.load(f)
-                self.features = [features[feature] for feature in x['features'] if feature in features]
-        else:
-            self.features = list(features.values())
-
-        if feature_version == 1:
-            if not lief.__version__.startswith("0.8.3"):
-                if print_feature_warning:
-                    print(f"WARNING: EMBER feature version 1 were computed using lief version 0.8.3-18d5b75")
-                    print(f"WARNING:   lief version {lief.__version__} found instead. There may be slight inconsistencies")
-                    print(f"WARNING:   in the feature calculations.")
-        elif feature_version == 2:
-            self.features.append(DataDirectories())
-            if not lief.__version__.startswith("0.9.0"):
-                if print_feature_warning:
-                    print(f"WARNING: EMBER feature version 2 were computed using lief version 0.9.0-")
-                    print(f"WARNING:   lief version {lief.__version__} found instead. There may be slight inconsistencies")
-                    print(f"WARNING:   in the feature calculations.")
-        else:
-            raise Exception(f"EMBER feature version must be 1 or 2. Not {feature_version}")
-        self.dim = sum([fe.dim for fe in self.features])
-
-    def raw_features(self, bytez):
-        lief_errors = (lief.bad_format, lief.bad_file, lief.pe_error, lief.parser_error, lief.read_out_of_bound,
-                       RuntimeError)
-        try:
-            lief_binary = lief.PE.parse(list(bytez))
-            if lief_binary is None:
-                raise Exception("lief failed to parse bytes!")
-        except lief_errors as e:
-            print("lief error: ", str(e))
-            lief_binary = None
-            raise Exception("lief failed to parse bytes (lief errors)!")
-        except Exception:  # everything else (KeyboardInterrupt, SystemExit, ValueError):
-            raise
-
-        features = {"sha256": hashlib.sha256(bytez).hexdigest()}
-        features.update({fe.name: fe.raw_features(bytez, lief_binary) for fe in self.features})
-        return features
-
-    def process_raw_features(self, raw_obj):
-        feature_vectors = [fe.process_raw_features(raw_obj[fe.name]) for fe in self.features]
-        return np.hstack(feature_vectors).astype(np.float32)
-
-    def feature_vector(self, bytez):
-        return self.process_raw_features(self.raw_features(bytez))
-    
-    def get_json_features(self, bytez):
-        """Return the JSON of the features extracted from the bytez.
-
-        Args:
-            bytez (bytes): a byte array that represent the PE file from which extract the features.
-
-        Returns:
-            dict: a dictionary that contains the features extracted from the bytez.
-        """
-        return self.raw_features(bytez)
-    
-    def get_raw_and_processed_features(self, bytes, feature_name):
-        """
-        Return the raw and processed features of the given feature name. 
-        """
-        feature_dict = self.raw_features(bytes)
-        processed_features = self.process_raw_features(feature_dict)
-        feature_range = self.get_feature_range()[feature_name]
-        
-        raw_features = feature_dict[feature_name]
-        return raw_features, processed_features[feature_range[0]:feature_range[1]]
-        
-    def get_feature_range(self):
-        """Return a dict of the features and their range.
-
-        Returns:
-            dict: a dictionary that contains as key the type of the feature and as value a tuple that corresponds to the indexes of the EMBER's feature vector in which these features are contained.
-        """
-        return {
-            'histogram': (0, 256),
-            'byte entropy': (256, 512),
-            'strings': (512, 616),
-            'general': (616, 626),
-            'header': (626, 688),
-            'section': (688, 943),
-            'imports': (943, 2223),
-            'exports': (2223, 2351),
-            'data directories': (2351, 2381)
-        }
-    
-    def get_header_features_index(self, bytes):
-        raw_obj = self.raw_features(bytes)
+#!/usr/bin/python
+''' Extracts some basic features from PE files. Many of the features
+implemented have been used in previously published works. For more information,
+check out the following resources:
+* Schultz, et al., 2001: http://128.59.14.66/sites/default/files/binaryeval-ieeesp01.pdf
+* Kolter and Maloof, 2006: http://www.jmlr.org/papers/volume7/kolter06a/kolter06a.pdf
+* Shafiq et al., 2009: https://www.researchgate.net/profile/Fauzan_Mirza/publication/242084613_A_Framework_for_Efficient_Mining_of_Structural_Information_to_Detect_Zero-Day_Malicious_Portable_Executables/links/0c96052e191668c3d5000000.pdf
+* Raman, 2012: http://2012.infosecsouthwest.com/files/speaker_materials/ISSW2012_Selecting_Features_to_Classify_Malware.pdf
+* Saxe and Berlin, 2015: https://arxiv.org/pdf/1508.03096.pdf
+
+It may be useful to do feature selection to reduce this set of features to a meaningful set
+for your modeling problem.
+'''
+
+import re
+import lief
+import hashlib
+import numpy as np
+import os
+import json
+from sklearn.feature_extraction import FeatureHasher
+
+LIEF_MAJOR, LIEF_MINOR, _ = lief.__version__.split('.')
+LIEF_EXPORT_OBJECT = int(LIEF_MAJOR) > 0 or ( int(LIEF_MAJOR)==0 and int(LIEF_MINOR) >= 10 )
+LIEF_HAS_SIGNATURE = int(LIEF_MAJOR) > 0 or (int(LIEF_MAJOR) == 0 and int(LIEF_MINOR) >= 11)
+
+
+class FeatureType(object):
+    ''' Base class from which each feature type may inherit '''
+
+    name = ''
+    dim = 0
+
+    def __repr__(self):
+        return '{}({})'.format(self.name, self.dim)
+
+    def raw_features(self, bytez, lief_binary):
+        ''' Generate a JSON-able representation of the file '''
+        raise (NotImplementedError)
+
+    def process_raw_features(self, raw_obj):
+        ''' Generate a feature vector from the raw features '''
+        raise (NotImplementedError)
+
+    def feature_vector(self, bytez, lief_binary):
+        ''' Directly calculate the feature vector from the sample itself. This should only be implemented differently
+        if there are significant speedups to be gained from combining the two functions. '''
+        return self.process_raw_features(self.raw_features(bytez, lief_binary))
+
+
+class ByteHistogram(FeatureType):
+    ''' Byte histogram (count + non-normalized) over the entire binary file '''
+
+    name = 'histogram'
+    dim = 256
+
+    def __init__(self):
+        super(FeatureType, self).__init__()
+
+    def raw_features(self, bytez, lief_binary):
+        counts = np.bincount(np.frombuffer(bytez, dtype=np.uint8), minlength=256)
+        return counts.tolist()
+
+    def process_raw_features(self, raw_obj):
+        counts = np.array(raw_obj, dtype=np.float32)
+        sum = counts.sum()
+        normalized = counts / sum
+        return normalized
+
+
+class ByteEntropyHistogram(FeatureType):
+    ''' 2d byte/entropy histogram based loosely on (Saxe and Berlin, 2015).
+    This roughly approximates the joint probability of byte value and local entropy.
+    See Section 2.1.1 in https://arxiv.org/pdf/1508.03096.pdf for more info.
+    '''
+
+    name = 'byteentropy'
+    dim = 256
+
+    def __init__(self, step=1024, window=2048):
+        super(FeatureType, self).__init__()
+        self.window = window
+        self.step = step
+
+    def _entropy_bin_counts(self, block):
+        # coarse histogram, 16 bytes per bin
+        c = np.bincount(block >> 4, minlength=16)  # 16-bin histogram
+        p = c.astype(np.float32) / self.window
+        wh = np.where(c)[0]
+        H = np.sum(-p[wh] * np.log2(
+            p[wh])) * 2  # * x2 b.c. we reduced information by half: 256 bins (8 bits) to 16 bins (4 bits)
+
+        Hbin = int(H * 2)  # up to 16 bins (max entropy is 8 bits)
+        if Hbin == 16:  # handle entropy = 8.0 bits
+            Hbin = 15
+
+        return Hbin, c
+
+    def raw_features(self, bytez, lief_binary):
+        output = np.zeros((16, 16), dtype=np.int64)
+        a = np.frombuffer(bytez, dtype=np.uint8)
+        if a.shape[0] < self.window:
+            Hbin, c = self._entropy_bin_counts(a)
+            output[Hbin, :] += c
+        else:
+            # strided trick from here: http://www.rigtorp.se/2011/01/01/rolling-statistics-numpy.html
+            shape = a.shape[:-1] + (a.shape[-1] - self.window + 1, self.window)
+            strides = a.strides + (a.strides[-1],)
+            blocks = np.lib.stride_tricks.as_strided(a, shape=shape, strides=strides)[::self.step, :]
+
+            # from the blocks, compute histogram
+            for block in blocks:
+                Hbin, c = self._entropy_bin_counts(block)
+                output[Hbin, :] += c
+
+        return output.flatten().tolist()
+
+    def process_raw_features(self, raw_obj):
+        counts = np.array(raw_obj, dtype=np.float32)
+        sum = counts.sum()
+        normalized = counts / sum
+        return normalized
+
+
+class SectionInfo(FeatureType):
+    ''' Information about section names, sizes and entropy.  Uses hashing trick
+    to summarize all this section info into a feature vector.
+    '''
+
+    name = 'section'
+    dim = 5 + 50 + 50 + 50 + 50 + 50
+
+    def __init__(self):
+        super(FeatureType, self).__init__()
+
+    @staticmethod
+    def _properties(s):
+        return [str(c).split('.')[-1] for c in s.characteristics_lists]
+
+    def raw_features(self, bytez, lief_binary):
+        if lief_binary is None:
+            return {"entry": "", "sections": []}
+
+        # properties of entry point, or if invalid, the first executable section
+
+        try:
+            if int(LIEF_MAJOR) > 0 or (int(LIEF_MAJOR) == 0 and int(LIEF_MINOR) >= 12):
+                section = lief_binary.section_from_rva(lief_binary.entrypoint - lief_binary.imagebase)
+                if section is None:
+                    raise lief.not_found
+                entry_section = section.name
+            else: # lief < 0.12
+                entry_section = lief_binary.section_from_offset(lief_binary.entrypoint).name
+        except lief.not_found:
+                # bad entry point, let's find the first executable section
+                entry_section = ""
+                for s in lief_binary.sections:
+                    if lief.PE.SECTION_CHARACTERISTICS.MEM_EXECUTE in s.characteristics_lists:
+                        entry_section = s.name
+                        break
+
+        raw_obj = {"entry": entry_section}
+        raw_obj["sections"] = [{
+            'name': s.name,
+            'size': s.size,
+            'entropy': s.entropy,
+            'vsize': s.virtual_size,
+            'props': self._properties(s)
+        } for s in lief_binary.sections]
+        return raw_obj
+
+    def process_raw_features(self, raw_obj):
+        sections = raw_obj['sections']
+        general = [
+            len(sections),  # total number of sections
+            # number of sections with zero size
+            sum(1 for s in sections if s['size'] == 0),
+            # number of sections with an empty name
+            sum(1 for s in sections if s['name'] == ""),
+            # number of RX
+            sum(1 for s in sections if 'MEM_READ' in s['props'] and 'MEM_EXECUTE' in s['props']),
+            # number of W
+            sum(1 for s in sections if 'MEM_WRITE' in s['props'])
+        ]
+        # gross characteristics of each section
+        section_sizes = [(s['name'], s['size']) for s in sections]
+        section_sizes_hashed = FeatureHasher(50, input_type="pair").transform([section_sizes]).toarray()[0]
+        section_entropy = [(s['name'], s['entropy']) for s in sections]
+        section_entropy_hashed = FeatureHasher(50, input_type="pair").transform([section_entropy]).toarray()[0]
+        section_vsize = [(s['name'], s['vsize']) for s in sections]
+        section_vsize_hashed = FeatureHasher(50, input_type="pair").transform([section_vsize]).toarray()[0]
+        entry_name_hashed = FeatureHasher(50, input_type="string").transform([ [raw_obj['entry']] ]).toarray()[0]
+        characteristics = [p for s in sections for p in s['props'] if s['name'] == raw_obj['entry']]
+        characteristics_hashed = FeatureHasher(50, input_type="string").transform([characteristics]).toarray()[0]
+
+        return np.hstack([
+            general, section_sizes_hashed, section_entropy_hashed, section_vsize_hashed, entry_name_hashed,
+            characteristics_hashed
+        ]).astype(np.float32)
+
+
+class ImportsInfo(FeatureType):
+    ''' Information about imported libraries and functions from the
+    import address table.  Note that the total number of imported
+    functions is contained in GeneralFileInfo.
+    '''
+
+    name = 'imports'
+    dim = 1280
+
+    def __init__(self):
+        super(FeatureType, self).__init__()
+
+    def raw_features(self, bytez, lief_binary):
+        imports = {}
+        if lief_binary is None:
+            return imports
+
+        for lib in lief_binary.imports:
+            if lib.name not in imports:
+                imports[lib.name] = []  # libraries can be duplicated in listing, extend instead of overwrite
+
+            # Clipping assumes there are diminishing returns on the discriminatory power of imported functions
+            #  beyond the first 10000 characters, and this will help limit the dataset size
+            for entry in lib.entries:
+                if entry.is_ordinal:
+                    imports[lib.name].append("ordinal" + str(entry.ordinal))
+                else:
+                    imports[lib.name].append(entry.name[:10000])
+
+        return imports
+
+    def process_raw_features(self, raw_obj):
+        # unique libraries
+        libraries = list(set([l.lower() for l in raw_obj.keys()]))
+        libraries_hashed = FeatureHasher(256, input_type="string").transform([libraries]).toarray()[0]
+
+        # A string like "kernel32.dll:CreateFileMappingA" for each imported function
+        imports = [lib.lower() + ':' + e for lib, elist in raw_obj.items() for e in elist]
+        imports_hashed = FeatureHasher(1024, input_type="string").transform([imports]).toarray()[0]
+
+        # Two separate elements: libraries (alone) and fully-qualified names of imported functions
+        return np.hstack([libraries_hashed, imports_hashed]).astype(np.float32)
+
+
+class ExportsInfo(FeatureType):
+    ''' Information about exported functions. Note that the total number of exported
+    functions is contained in GeneralFileInfo.
+    '''
+
+    name = 'exports'
+    dim = 128
+
+    def __init__(self):
+        super(FeatureType, self).__init__()
+
+    def raw_features(self, bytez, lief_binary):
+        if lief_binary is None:
+            return []
+
+        # Clipping assumes there are diminishing returns on the discriminatory power of exports beyond
+        #  the first 10000 characters, and this will help limit the dataset size
+        if LIEF_EXPORT_OBJECT:
+            # export is an object with .name attribute (0.10.0 and later)
+            clipped_exports = [export.name[:10000] for export in lief_binary.exported_functions]
+        else:
+            # export is a string (LIEF 0.9.0 and earlier)
+            clipped_exports = [export[:10000] for export in lief_binary.exported_functions]
+
+
+        return clipped_exports
+
+    def process_raw_features(self, raw_obj):
+        exports_hashed = FeatureHasher(128, input_type="string").transform([raw_obj]).toarray()[0]
+        return exports_hashed.astype(np.float32)
+
+
+class GeneralFileInfo(FeatureType):
+    ''' General information about the file '''
+
+    name = 'general'
+    dim = 10
+
+    def __init__(self):
+        super(FeatureType, self).__init__()
+
+    def raw_features(self, bytez, lief_binary):
+        if lief_binary is None:
+            return {
+                'size': len(bytez),
+                'vsize': 0,
+                'has_debug': 0,
+                'exports': 0,
+                'imports': 0,
+                'has_relocations': 0,
+                'has_resources': 0,
+                'has_signature': 0,
+                'has_tls': 0,
+                'symbols': 0
+            }
+
+        return {
+            'size': len(bytez),
+            'vsize': lief_binary.virtual_size,
+            'has_debug': int(lief_binary.has_debug),
+            'exports': len(lief_binary.exported_functions),
+            'imports': len(lief_binary.imported_functions),
+            'has_relocations': int(lief_binary.has_relocations),
+            'has_resources': int(lief_binary.has_resources),
+            'has_signature': int(lief_binary.has_signatures) if LIEF_HAS_SIGNATURE else int(lief_binary.has_signature),
+            'has_tls': int(lief_binary.has_tls),
+            'symbols': len(lief_binary.symbols),
+        }
+
+    def process_raw_features(self, raw_obj):
+        return np.asarray([
+            raw_obj['size'], raw_obj['vsize'], raw_obj['has_debug'], raw_obj['exports'], raw_obj['imports'],
+            raw_obj['has_relocations'], raw_obj['has_resources'], raw_obj['has_signature'], raw_obj['has_tls'],
+            raw_obj['symbols']
+        ],
+                          dtype=np.float32)
+
+
+class HeaderFileInfo(FeatureType):
+    ''' Machine, architecure, OS, linker and other information extracted from header '''
+
+    name = 'header'
+    dim = 62
+
+    def __init__(self):
+        super(FeatureType, self).__init__()
+
+    def raw_features(self, bytez, lief_binary):
+        raw_obj = {}
+        raw_obj['coff'] = {'timestamp': 0, 'machine': "", 'characteristics': []}
+        raw_obj['optional'] = {
+            'subsystem': "",
+            'dll_characteristics': [],
+            'magic': "",
+            'major_image_version': 0,
+            'minor_image_version': 0,
+            'major_linker_version': 0,
+            'minor_linker_version': 0,
+            'major_operating_system_version': 0,
+            'minor_operating_system_version': 0,
+            'major_subsystem_version': 0,
+            'minor_subsystem_version': 0,
+            'sizeof_code': 0,
+            'sizeof_headers': 0,
+            'sizeof_heap_commit': 0
+        }
+        if lief_binary is None:
+            return raw_obj
+
+        raw_obj['coff']['timestamp'] = lief_binary.header.time_date_stamps
+        raw_obj['coff']['machine'] = str(lief_binary.header.machine).split('.')[-1]
+        raw_obj['coff']['characteristics'] = [str(c).split('.')[-1] for c in lief_binary.header.characteristics_list]
+        raw_obj['optional']['subsystem'] = str(lief_binary.optional_header.subsystem).split('.')[-1]
+        raw_obj['optional']['dll_characteristics'] = [
+            str(c).split('.')[-1] for c in lief_binary.optional_header.dll_characteristics_lists
+        ]
+        raw_obj['optional']['magic'] = str(lief_binary.optional_header.magic).split('.')[-1]
+        raw_obj['optional']['major_image_version'] = lief_binary.optional_header.major_image_version
+        raw_obj['optional']['minor_image_version'] = lief_binary.optional_header.minor_image_version
+        raw_obj['optional']['major_linker_version'] = lief_binary.optional_header.major_linker_version
+        raw_obj['optional']['minor_linker_version'] = lief_binary.optional_header.minor_linker_version
+        raw_obj['optional'][
+            'major_operating_system_version'] = lief_binary.optional_header.major_operating_system_version
+        raw_obj['optional'][
+            'minor_operating_system_version'] = lief_binary.optional_header.minor_operating_system_version
+        raw_obj['optional']['major_subsystem_version'] = lief_binary.optional_header.major_subsystem_version
+        raw_obj['optional']['minor_subsystem_version'] = lief_binary.optional_header.minor_subsystem_version
+        raw_obj['optional']['sizeof_code'] = lief_binary.optional_header.sizeof_code
+        raw_obj['optional']['sizeof_headers'] = lief_binary.optional_header.sizeof_headers
+        raw_obj['optional']['sizeof_heap_commit'] = lief_binary.optional_header.sizeof_heap_commit
+        return raw_obj
+
+    def process_raw_features(self, raw_obj):
+        return np.hstack([
+            raw_obj['coff']['timestamp'],
+            FeatureHasher(10, input_type="string").transform([[raw_obj['coff']['machine']]]).toarray()[0],
+            FeatureHasher(10, input_type="string").transform([raw_obj['coff']['characteristics']]).toarray()[0],
+            FeatureHasher(10, input_type="string").transform([[raw_obj['optional']['subsystem']]]).toarray()[0],
+            FeatureHasher(10, input_type="string").transform([raw_obj['optional']['dll_characteristics']]).toarray()[0],
+            FeatureHasher(10, input_type="string").transform([[raw_obj['optional']['magic']]]).toarray()[0],
+            raw_obj['optional']['major_image_version'],
+            raw_obj['optional']['minor_image_version'],
+            raw_obj['optional']['major_linker_version'],
+            raw_obj['optional']['minor_linker_version'],
+            raw_obj['optional']['major_operating_system_version'],
+            raw_obj['optional']['minor_operating_system_version'],
+            raw_obj['optional']['major_subsystem_version'],
+            raw_obj['optional']['minor_subsystem_version'],
+            raw_obj['optional']['sizeof_code'],
+            raw_obj['optional']['sizeof_headers'],
+            raw_obj['optional']['sizeof_heap_commit'],
+        ]).astype(np.float32)
+        
+        
+    def get_features_index(self, raw_obj):
+        features_list = [
+            raw_obj['coff']['timestamp'],
+            FeatureHasher(10, input_type="string").transform([[raw_obj['coff']['machine']]]).toarray()[0],
+            FeatureHasher(10, input_type="string").transform([raw_obj['coff']['characteristics']]).toarray()[0],
+            FeatureHasher(10, input_type="string").transform([[raw_obj['optional']['subsystem']]]).toarray()[0],
+            FeatureHasher(10, input_type="string").transform([raw_obj['optional']['dll_characteristics']]).toarray()[0],
+            FeatureHasher(10, input_type="string").transform([[raw_obj['optional']['magic']]]).toarray()[0],
+            raw_obj['optional']['major_image_version'],
+            raw_obj['optional']['minor_image_version'],
+            raw_obj['optional']['major_linker_version'],
+            raw_obj['optional']['minor_linker_version'],
+            raw_obj['optional']['major_operating_system_version'],
+            raw_obj['optional']['minor_operating_system_version'],
+            raw_obj['optional']['major_subsystem_version'],
+            raw_obj['optional']['minor_subsystem_version'],
+            raw_obj['optional']['sizeof_code'],
+            raw_obj['optional']['sizeof_headers'],
+            raw_obj['optional']['sizeof_heap_commit'],
+        ]
+        keys_list = [
+            'coff-timestamp',
+            'coff-machine',
+            'coff-characteristics',
+            'optional-subsystem',
+            'optional-dll_characteristics',
+            'optional-magic',
+            'optional-major_image_version',
+            'optional-minor_image_version',
+            'optional-major_linker_version',
+            'optional-minor_linker_version',
+            'optional-major_operating_system_version',
+            'optional-minor_operating_system_version',
+            'optional-major_subsystem_version',
+            'optional-minor_subsystem_version',
+            'optional-sizeof_code',
+            'optional-sizeof_headers',
+            'optional-sizeof_heap_commit',
+        ]
+
+        rv = {}
+        index = 0
+        for i in range(len(features_list)):
+            try:
+                if len(features_list[i]) > 1:
+                    rv[keys_list[i]] = (index, index+len(features_list[i]))
+                    index += len(features_list[i])
+            except TypeError:
+                    rv[keys_list[i]] = index
+                    index += 1
+        return rv
+        
+        
+class StringExtractor(FeatureType):
+    ''' Extracts strings from raw byte stream '''
+
+    name = 'strings'
+    dim = 1 + 1 + 1 + 96 + 1 + 1 + 1 + 1 + 1
+
+    def __init__(self):
+        super(FeatureType, self).__init__()
+        # all consecutive runs of 0x20 - 0x7f that are 5+ characters
+        self._allstrings = re.compile(b'[\x20-\x7f]{5,}')
+        # occurances of the string 'C:\'.  Not actually extracting the path
+        self._paths = re.compile(b'c:\\\\', re.IGNORECASE)
+        # occurances of http:// or https://.  Not actually extracting the URLs
+        self._urls = re.compile(b'https?://', re.IGNORECASE)
+        # occurances of the string prefix HKEY_.  No actually extracting registry names
+        self._registry = re.compile(b'HKEY_')
+        # crude evidence of an MZ header (dropper?) somewhere in the byte stream
+        self._mz = re.compile(b'MZ')
+
+    def raw_features(self, bytez, lief_binary):
+        allstrings = self._allstrings.findall(bytez)
+        if allstrings:
+            # statistics about strings:
+            string_lengths = [len(s) for s in allstrings]
+            avlength = sum(string_lengths) / len(string_lengths)
+            # map printable characters 0x20 - 0x7f to an int array consisting of 0-95, inclusive
+            as_shifted_string = [b - ord(b'\x20') for b in b''.join(allstrings)]
+            c = np.bincount(as_shifted_string, minlength=96)  # histogram count
+            # distribution of characters in printable strings
+            csum = c.sum()
+            p = c.astype(np.float32) / csum
+            wh = np.where(c)[0]
+            H = np.sum(-p[wh] * np.log2(p[wh]))  # entropy
+        else:
+            avlength = 0
+            c = np.zeros((96,), dtype=np.float32)
+            H = 0
+            csum = 0
+
+        return {
+            'numstrings': len(allstrings),
+            'avlength': avlength,
+            'printabledist': c.tolist(),  # store non-normalized histogram
+            'printables': int(csum),
+            'entropy': float(H),
+            'paths': len(self._paths.findall(bytez)),
+            'urls': len(self._urls.findall(bytez)),
+            'registry': len(self._registry.findall(bytez)),
+            'MZ': len(self._mz.findall(bytez))
+        }
+
+    def process_raw_features(self, raw_obj):
+        hist_divisor = float(raw_obj['printables']) if raw_obj['printables'] > 0 else 1.0
+        return np.hstack([
+            raw_obj['numstrings'], raw_obj['avlength'], raw_obj['printables'],
+            np.asarray(raw_obj['printabledist']) / hist_divisor, raw_obj['entropy'], raw_obj['paths'], raw_obj['urls'],
+            raw_obj['registry'], raw_obj['MZ']
+        ]).astype(np.float32)
+
+
+class DataDirectories(FeatureType):
+    ''' Extracts size and virtual address of the first 15 data directories '''
+
+    name = 'datadirectories'
+    dim = 15 * 2
+
+    def __init__(self):
+        super(FeatureType, self).__init__()
+        self._name_order = [
+            "EXPORT_TABLE", "IMPORT_TABLE", "RESOURCE_TABLE", "EXCEPTION_TABLE", "CERTIFICATE_TABLE",
+            "BASE_RELOCATION_TABLE", "DEBUG", "ARCHITECTURE", "GLOBAL_PTR", "TLS_TABLE", "LOAD_CONFIG_TABLE",
+            "BOUND_IMPORT", "IAT", "DELAY_IMPORT_DESCRIPTOR", "CLR_RUNTIME_HEADER"
+        ]
+
+    def raw_features(self, bytez, lief_binary):
+        output = []
+        if lief_binary is None:
+            return output
+
+        for data_directory in lief_binary.data_directories:
+            output.append({
+                "name": str(data_directory.type).replace("DATA_DIRECTORY.", ""),
+                "size": data_directory.size,
+                "virtual_address": data_directory.rva
+            })
+        return output
+
+    def process_raw_features(self, raw_obj):
+        features = np.zeros(2 * len(self._name_order), dtype=np.float32)
+        for i in range(len(self._name_order)):
+            if i < len(raw_obj):
+                features[2 * i] = raw_obj[i]["size"]
+                features[2 * i + 1] = raw_obj[i]["virtual_address"]
+        return features
+
+
+class PEFeatureExtractor(object):
+    ''' Extract useful features from a PE file, and return as a vector of fixed size. '''
+
+    def __init__(self, feature_version=2, print_feature_warning=True, features_file=''):
+        self.features = []
+        features = {
+                    'ByteHistogram': ByteHistogram(),
+                    'ByteEntropyHistogram': ByteEntropyHistogram(),
+                    'StringExtractor': StringExtractor(),
+                    'GeneralFileInfo': GeneralFileInfo(),
+                    'HeaderFileInfo': HeaderFileInfo(),
+                    'SectionInfo': SectionInfo(),
+                    'ImportsInfo': ImportsInfo(),
+                    'ExportsInfo': ExportsInfo()
+            }
+
+        if os.path.exists(features_file):
+            with open(features_file, encoding='utf8') as f:
+                x = json.load(f)
+                self.features = [features[feature] for feature in x['features'] if feature in features]
+        else:
+            self.features = list(features.values())
+
+        if feature_version == 1:
+            if not lief.__version__.startswith("0.8.3"):
+                if print_feature_warning:
+                    print(f"WARNING: EMBER feature version 1 were computed using lief version 0.8.3-18d5b75")
+                    print(f"WARNING:   lief version {lief.__version__} found instead. There may be slight inconsistencies")
+                    print(f"WARNING:   in the feature calculations.")
+        elif feature_version == 2:
+            self.features.append(DataDirectories())
+            if not lief.__version__.startswith("0.9.0"):
+                if print_feature_warning:
+                    print(f"WARNING: EMBER feature version 2 were computed using lief version 0.9.0-")
+                    print(f"WARNING:   lief version {lief.__version__} found instead. There may be slight inconsistencies")
+                    print(f"WARNING:   in the feature calculations.")
+        else:
+            raise Exception(f"EMBER feature version must be 1 or 2. Not {feature_version}")
+        self.dim = sum([fe.dim for fe in self.features])
+
+    def raw_features(self, bytez):
+        if LIEF_MINOR == 0 and LIEF_MAJOR >= 13:
+            lief_errors = (lief.bad_file, lief.pe_error, lief.parser_error, lief.read_out_of_bound,
+                        RuntimeError)
+        else:
+            lief_errors = (lief.bad_format, lief.bad_file, lief.pe_error, lief.parser_error, lief.read_out_of_bound,
+                        RuntimeError)
+        try:
+            lief_binary = lief.PE.parse(list(bytez))
+            if lief_binary is None:
+                raise Exception("lief failed to parse bytes!")
+        except lief_errors as e:
+            print("lief error: ", str(e))
+            lief_binary = None
+            raise Exception("lief failed to parse bytes (lief errors)!")
+        except Exception:  # everything else (KeyboardInterrupt, SystemExit, ValueError):
+            raise
+
+        features = {"sha256": hashlib.sha256(bytez).hexdigest()}
+        features.update({fe.name: fe.raw_features(bytez, lief_binary) for fe in self.features})
+        return features
+
+    def process_raw_features(self, raw_obj):
+        feature_vectors = [fe.process_raw_features(raw_obj[fe.name]) for fe in self.features]
+        return np.hstack(feature_vectors).astype(np.float32)
+
+    def feature_vector(self, bytez):
+        return self.process_raw_features(self.raw_features(bytez))
+    
+    def get_json_features(self, bytez):
+        """Return the JSON of the features extracted from the bytez.
+
+        Args:
+            bytez (bytes): a byte array that represent the PE file from which extract the features.
+
+        Returns:
+            dict: a dictionary that contains the features extracted from the bytez.
+        """
+        return self.raw_features(bytez)
+    
+    def get_raw_and_processed_features(self, bytes, feature_name):
+        """
+        Return the raw and processed features of the given feature name. 
+        """
+        feature_dict = self.raw_features(bytes)
+        processed_features = self.process_raw_features(feature_dict)
+        feature_range = self.get_feature_range()[feature_name]
+        
+        raw_features = feature_dict[feature_name]
+        return raw_features, processed_features[feature_range[0]:feature_range[1]]
+        
+    def get_feature_range(self):
+        """Return a dict of the features and their range.
+
+        Returns:
+            dict: a dictionary that contains as key the type of the feature and as value a tuple that corresponds to the indexes of the EMBER's feature vector in which these features are contained.
+        """
+        return {
+            'histogram': (0, 256),
+            'byte entropy': (256, 512),
+            'strings': (512, 616),
+            'general': (616, 626),
+            'header': (626, 688),
+            'section': (688, 943),
+            'imports': (943, 2223),
+            'exports': (2223, 2351),
+            'data directories': (2351, 2381)
+        }
+    
+    def get_header_features_index(self, bytes):
+        raw_obj = self.raw_features(bytes)
         return HeaderFileInfo().get_features_index(raw_obj['header'])
```

### Comparing `ember-mivia-0.0.4/ember_mivia.egg-info/PKG-INFO` & `ember-mivia-0.0.5/ember_mivia.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,140 +1,139 @@
-Metadata-Version: 2.1
-Name: ember-mivia
-Version: 0.0.4
-Summary: Endgame Malware BEnchmark for Research
-Home-page: https://github.com/gparrella12/ember
-Author-email: proth@endgame.com
-License: UNKNOWN
-Description: <img src="resources/logo.png" align="right" width="250px" height="250px">
-        
-        # Elastic Malware Benchmark for Empowering Researchers
-        
-        The EMBER dataset is a collection of features from PE files that serve as a benchmark dataset for researchers. The EMBER2017 dataset contained features from 1.1 million PE files scanned in or before 2017 and the EMBER2018 dataset contains features from 1 million PE files scanned in or before 2018. This repository makes it easy to reproducibly train the benchmark models, extend the provided feature set, or classify new PE files with the benchmark models.
-        
-        This paper describes many more details about the dataset: [https://arxiv.org/abs/1804.04637](https://arxiv.org/abs/1804.04637)
-        
-        ## Features
-        
-        The [LIEF](https://lief.quarkslab.com/) project is used to extract features from PE files included in the EMBER dataset. Raw features are extracted to JSON format and included in the publicly available dataset. Vectorized features can be produced from these raw features and saved in binary format from which they can be converted to CSV, dataframe, or any other format. This repository makes it easy to generate raw features and/or vectorized features from any PE file. Researchers can implement their own features, or even vectorize the existing features differently from the existing implementations.
-        
-        The feature calculation is versioned. Feature version 1 is calculated with the LIEF library version 0.8.3. Feature version 2 includes the additional data directory feature, updated ordinal import processing, and is calculated with LIEF library version 0.9.0.  We have verified under Windows and Linux that LIEF provides consistent feature representation for version 2 features using LIEF version 0.10.1 and that it does not on a Mac.
-        
-        ## Years
-        
-        The first EMBER dataset consisted of version 1 features calculated over samples collected in or before 2017. The second EMBER dataset release consisted of version 2 features calculated over samples collected in or before 2018. In conjunction with the second release, we also included the version 2 features from the samples collected in 2017. Combining the data from 2017 and 2018 will allow longer longitudinal studies of the evolution of features and PE file types. But different selection criteria were applied when choosing samples from 2017 and 2018. Specifically, the samples from 2018 were chosen so that the resultant training and test sets would be harder for machine learning algorithms to classify. Please beware of this inconsistancy while constructing your multi-year studies. The original paper only describes Ember 2017 (featur version 1). For a detailed information about the Ember 2018 dataset, please refer to https://www.camlis.org/2019/talks/roth where you can find both [slides](https://docs.google.com/presentation/d/1A13tsUkgWeujTy9SD-vDFfQp9fnIqbSE_tCihNPlArQ/edit#slide=id.g476bf81b41_0_446) and a [video talk](https://youtu.be/MsZmnUO5lkY).
-        
-        ## Download
-        
-        Download the data here:
-        
-        | Year | Feature Version | Filename                     | URL                                                                                                            | sha256                                                             |
-        |------|-----------------|------------------------------|----------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
-        | 2017 | 1               | ember_dataset.tar.bz2        | [https://ember.elastic.co/ember_dataset.tar.bz2](https://ember.elastic.co/ember_dataset.tar.bz2)               | `a5603de2f34f02ab6e21df7a0f97ec4ac84ddc65caee33fb610093dd6f9e1df9` |
-        | 2017 | 2               | ember_dataset_2017_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2017_2.tar.bz2](https://ember.elastic.co/ember_dataset_2017_2.tar.bz2) | `60142493c44c11bc3fef292b216a293841283d86ff58384b5dc2d88194c87a6d` |
-        | 2018 | 2               | ember_dataset_2018_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2018_2.tar.bz2](https://ember.elastic.co/ember_dataset_2018_2.tar.bz2) | `b6052eb8d350a49a8d5a5396fbe7d16cf42848b86ff969b77464434cf2997812` |
-        
-        
-        ## Installation
-        ### Instrall directly from git
-        Use `pip` to install the `ember` and required files
-        
-        ```
-        pip install git+https://github.com/elastic/ember.git
-        ```
-        
-        This provides access to EMBER feature extaction for example.  However, to use the scripts to train the model, one would instead clone the repository.
-        
-        
-        ### Install after cloning the EMBER repository
-        Use `pip` or `conda` to install the required packages before installing `ember` itself:
-        
-        ```
-        pip install -r requirements.txt
-        python setup.py install
-        ```
-        
-        ```
-        conda config --add channels conda-forge
-        conda install --file requirements_conda.txt
-        python setup.py install
-        ```
-        
-        ### Notes on LIEF versions
-        
-        LIEF is now pinned to version 0.9.0 in the provided requirements files. This default behavior will allow new users to immediately reproduce EMBER version 2 features. LIEF 0.9.0 will not install on an M1 Mac, though. For those users, a Dockerfile is now included that installs the dependencies using conda.
-        
-        EMBER will work with more recent releases of LIEF, but keep in mind that models trained on features generated with one version of LIEF will have unpredictable results when evaluating on features generated with another.
-        
-        ## Scripts
-        
-        The `train_ember.py` script simplifies the model training process. It will vectorize the ember features if necessary and then train the LightGBM model.
-        
-        ```
-        python train_ember.py [/path/to/dataset]
-        ```
-        
-        The `classify_binaries.py` script will return model predictions on PE files.
-        
-        ```
-        python classify_binaries.py -m [/path/to/model] BINARIES
-        ```
-        
-        ## Import Usage
-        
-        The raw feature data can be expanded into vectorized form on disk for model training and into metadata form. These two functions create those extra files:
-        
-        ```
-        import ember
-        ember.create_vectorized_features("/data/ember2018/")
-        ember.create_metadata("/data/ember2018/")
-        ```
-        
-        Once created, that data can be read in using convenience functions:
-        
-        ```
-        import ember
-        X_train, y_train, X_test, y_test = ember.read_vectorized_features("/data/ember2018/")
-        metadata_dataframe = ember.read_metadata("/data/ember2018/")
-        ```
-        
-        Once the data is downloaded and the ember module is installed, this simple code should reproduce the benchmark ember model:
-        
-        ```
-        import ember
-        ember.create_vectorized_features("/data/ember2018/")
-        lgbm_model = ember.train_model("/data/ember2018/")
-        ```
-        
-        Once the model is trained, the ember module can be used to make a prediction on any input PE file:
-        
-        ```
-        import ember
-        import lightgbm as lgb
-        lgbm_model = lgb.Booster(model_file="/data/ember2018/ember_model_2018.txt")
-        putty_data = open("~/putty.exe", "rb").read()
-        print(ember.predict_sample(lgbm_model, putty_data))
-        ```
-        
-        ## Citing
-        
-        If you use this data in a publication please cite the following [paper](https://arxiv.org/abs/1804.04637):
-        
-        ```
-        H. Anderson and P. Roth, "EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models”, in ArXiv e-prints. Apr. 2018.
-        
-        @ARTICLE{2018arXiv180404637A,
-          author = {{Anderson}, H.~S. and {Roth}, P.},
-          title = "{EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models}",
-          journal = {ArXiv e-prints},
-          archivePrefix = "arXiv",
-          eprint = {1804.04637},
-          primaryClass = "cs.CR",
-          keywords = {Computer Science - Cryptography and Security},
-          year = 2018,
-          month = apr,
-          adsurl = {http://adsabs.harvard.edu/abs/2018arXiv180404637A},
-        }
-        ```
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: ember-mivia
+Version: 0.0.5
+Summary: Endgame Malware BEnchmark for Research
+Home-page: https://github.com/gparrella12/ember
+Author-email: proth@endgame.com
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+<img src="resources/logo.png" align="right" width="250px" height="250px">
+
+# Elastic Malware Benchmark for Empowering Researchers
+
+The EMBER dataset is a collection of features from PE files that serve as a benchmark dataset for researchers. The EMBER2017 dataset contained features from 1.1 million PE files scanned in or before 2017 and the EMBER2018 dataset contains features from 1 million PE files scanned in or before 2018. This repository makes it easy to reproducibly train the benchmark models, extend the provided feature set, or classify new PE files with the benchmark models.
+
+This paper describes many more details about the dataset: [https://arxiv.org/abs/1804.04637](https://arxiv.org/abs/1804.04637)
+
+## Features
+
+The [LIEF](https://lief.quarkslab.com/) project is used to extract features from PE files included in the EMBER dataset. Raw features are extracted to JSON format and included in the publicly available dataset. Vectorized features can be produced from these raw features and saved in binary format from which they can be converted to CSV, dataframe, or any other format. This repository makes it easy to generate raw features and/or vectorized features from any PE file. Researchers can implement their own features, or even vectorize the existing features differently from the existing implementations.
+
+The feature calculation is versioned. Feature version 1 is calculated with the LIEF library version 0.8.3. Feature version 2 includes the additional data directory feature, updated ordinal import processing, and is calculated with LIEF library version 0.9.0.  We have verified under Windows and Linux that LIEF provides consistent feature representation for version 2 features using LIEF version 0.10.1 and that it does not on a Mac.
+
+## Years
+
+The first EMBER dataset consisted of version 1 features calculated over samples collected in or before 2017. The second EMBER dataset release consisted of version 2 features calculated over samples collected in or before 2018. In conjunction with the second release, we also included the version 2 features from the samples collected in 2017. Combining the data from 2017 and 2018 will allow longer longitudinal studies of the evolution of features and PE file types. But different selection criteria were applied when choosing samples from 2017 and 2018. Specifically, the samples from 2018 were chosen so that the resultant training and test sets would be harder for machine learning algorithms to classify. Please beware of this inconsistancy while constructing your multi-year studies. The original paper only describes Ember 2017 (featur version 1). For a detailed information about the Ember 2018 dataset, please refer to https://www.camlis.org/2019/talks/roth where you can find both [slides](https://docs.google.com/presentation/d/1A13tsUkgWeujTy9SD-vDFfQp9fnIqbSE_tCihNPlArQ/edit#slide=id.g476bf81b41_0_446) and a [video talk](https://youtu.be/MsZmnUO5lkY).
+
+## Download
+
+Download the data here:
+
+| Year | Feature Version | Filename                     | URL                                                                                                            | sha256                                                             |
+|------|-----------------|------------------------------|----------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
+| 2017 | 1               | ember_dataset.tar.bz2        | [https://ember.elastic.co/ember_dataset.tar.bz2](https://ember.elastic.co/ember_dataset.tar.bz2)               | `a5603de2f34f02ab6e21df7a0f97ec4ac84ddc65caee33fb610093dd6f9e1df9` |
+| 2017 | 2               | ember_dataset_2017_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2017_2.tar.bz2](https://ember.elastic.co/ember_dataset_2017_2.tar.bz2) | `60142493c44c11bc3fef292b216a293841283d86ff58384b5dc2d88194c87a6d` |
+| 2018 | 2               | ember_dataset_2018_2.tar.bz2 | [https://ember.elastic.co/ember_dataset_2018_2.tar.bz2](https://ember.elastic.co/ember_dataset_2018_2.tar.bz2) | `b6052eb8d350a49a8d5a5396fbe7d16cf42848b86ff969b77464434cf2997812` |
+
+
+## Installation
+### Instrall directly from git
+Use `pip` to install the `ember` and required files
+
+```
+pip install git+https://github.com/elastic/ember.git
+```
+
+This provides access to EMBER feature extaction for example.  However, to use the scripts to train the model, one would instead clone the repository.
+
+
+### Install after cloning the EMBER repository
+Use `pip` or `conda` to install the required packages before installing `ember` itself:
+
+```
+pip install -r requirements.txt
+python setup.py install
+```
+
+```
+conda config --add channels conda-forge
+conda install --file requirements_conda.txt
+python setup.py install
+```
+
+### Notes on LIEF versions
+
+LIEF is now pinned to version 0.9.0 in the provided requirements files. This default behavior will allow new users to immediately reproduce EMBER version 2 features. LIEF 0.9.0 will not install on an M1 Mac, though. For those users, a Dockerfile is now included that installs the dependencies using conda.
+
+EMBER will work with more recent releases of LIEF, but keep in mind that models trained on features generated with one version of LIEF will have unpredictable results when evaluating on features generated with another.
+
+## Scripts
+
+The `train_ember.py` script simplifies the model training process. It will vectorize the ember features if necessary and then train the LightGBM model.
+
+```
+python train_ember.py [/path/to/dataset]
+```
+
+The `classify_binaries.py` script will return model predictions on PE files.
+
+```
+python classify_binaries.py -m [/path/to/model] BINARIES
+```
+
+## Import Usage
+
+The raw feature data can be expanded into vectorized form on disk for model training and into metadata form. These two functions create those extra files:
+
+```
+import ember
+ember.create_vectorized_features("/data/ember2018/")
+ember.create_metadata("/data/ember2018/")
+```
+
+Once created, that data can be read in using convenience functions:
+
+```
+import ember
+X_train, y_train, X_test, y_test = ember.read_vectorized_features("/data/ember2018/")
+metadata_dataframe = ember.read_metadata("/data/ember2018/")
+```
+
+Once the data is downloaded and the ember module is installed, this simple code should reproduce the benchmark ember model:
+
+```
+import ember
+ember.create_vectorized_features("/data/ember2018/")
+lgbm_model = ember.train_model("/data/ember2018/")
+```
+
+Once the model is trained, the ember module can be used to make a prediction on any input PE file:
+
+```
+import ember
+import lightgbm as lgb
+lgbm_model = lgb.Booster(model_file="/data/ember2018/ember_model_2018.txt")
+putty_data = open("~/putty.exe", "rb").read()
+print(ember.predict_sample(lgbm_model, putty_data))
+```
+
+## Citing
+
+If you use this data in a publication please cite the following [paper](https://arxiv.org/abs/1804.04637):
+
+```
+H. Anderson and P. Roth, "EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models”, in ArXiv e-prints. Apr. 2018.
+
+@ARTICLE{2018arXiv180404637A,
+  author = {{Anderson}, H.~S. and {Roth}, P.},
+  title = "{EMBER: An Open Dataset for Training Static PE Malware Machine Learning Models}",
+  journal = {ArXiv e-prints},
+  archivePrefix = "arXiv",
+  eprint = {1804.04637},
+  primaryClass = "cs.CR",
+  keywords = {Computer Science - Cryptography and Security},
+  year = 2018,
+  month = apr,
+  adsurl = {http://adsabs.harvard.edu/abs/2018arXiv180404637A},
+}
+```
```

### Comparing `ember-mivia-0.0.4/setup.py` & `ember-mivia-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#!/usr/bin/env python
-
-import os
-
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
-
-with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="UTF-8") as f:
-    readme = f.read()
-
-version = "0.0.4"
-package_data = {}
-setup(
-    name="ember-mivia",
-    version=version,
-    url = "https://github.com/gparrella12/ember",
-    long_description_content_type = "text/markdown",
-    description="Endgame Malware BEnchmark for Research",
-    long_description=readme,
-    packages=["ember"],
-    package_data=package_data,
-    author_email="proth@endgame.com")
+#!/usr/bin/env python
+
+import os
+
+try:
+    from setuptools import setup
+except ImportError:
+    from distutils.core import setup
+
+with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="UTF-8") as f:
+    readme = f.read()
+
+version = "0.0.5"
+package_data = {}
+setup(
+    name="ember-mivia",
+    version=version,
+    url = "https://github.com/gparrella12/ember",
+    long_description_content_type = "text/markdown",
+    description="Endgame Malware BEnchmark for Research",
+    long_description=readme,
+    packages=["ember"],
+    package_data=package_data,
+    author_email="proth@endgame.com")
```

