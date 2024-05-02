# Comparing `tmp/ml4xcube-0.0.2.tar.gz` & `tmp/ml4xcube-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml4xcube-0.0.2.tar", last modified: Thu May  2 17:35:39 2024, max compression
+gzip compressed data, was "ml4xcube-0.0.3.tar", last modified: Thu May  2 18:04:55 2024, max compression
```

## Comparing `ml4xcube-0.0.2.tar` & `ml4xcube-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 17:35:39.385018 ml4xcube-0.0.2/
--rw-rw-r--   0 julia     (1000) julia     (1000)     1113 2024-04-23 08:43:03.000000 ml4xcube-0.0.2/LICENSE
--rw-rw-r--   0 julia     (1000) julia     (1000)       33 2024-04-23 08:43:03.000000 ml4xcube-0.0.2/MANIFEST.in
--rw-r--r--   0 julia     (1000) julia     (1000)     3660 2024-05-02 17:35:39.385018 ml4xcube-0.0.2/PKG-INFO
--rw-rw-r--   0 julia     (1000) julia     (1000)     1644 2024-05-02 17:34:31.000000 ml4xcube-0.0.2/README.md
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 17:35:39.385018 ml4xcube-0.0.2/mltools/
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 17:35:39.385018 ml4xcube-0.0.2/mltools/ml4xcube/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-04-23 11:53:26.000000 ml4xcube-0.0.2/mltools/ml4xcube/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     5544 2024-05-02 16:06:56.000000 ml4xcube-0.0.2/mltools/ml4xcube/cube_utilities.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2378 2024-05-02 16:06:56.000000 ml4xcube-0.0.2/mltools/ml4xcube/data_assignment.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 17:35:39.385018 ml4xcube-0.0.2/mltools/ml4xcube/datasets/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-02 10:14:25.000000 ml4xcube-0.0.2/mltools/ml4xcube/datasets/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2765 2024-05-02 16:06:56.000000 ml4xcube-0.0.2/mltools/ml4xcube/datasets/pytorch_xr.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4292 2024-05-02 16:06:56.000000 ml4xcube-0.0.2/mltools/ml4xcube/datasets/tensorflow_xr.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4242 2024-05-02 16:06:56.000000 ml4xcube-0.0.2/mltools/ml4xcube/datasets/xr_dataset.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 17:35:39.385018 ml4xcube-0.0.2/mltools/ml4xcube/gapfilling/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:35:17.000000 ml4xcube-0.0.2/mltools/ml4xcube/gapfilling/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    14356 2024-05-02 16:06:56.000000 ml4xcube-0.0.2/mltools/ml4xcube/gapfilling/gap_dataset.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    31651 2024-05-02 16:06:56.000000 ml4xcube-0.0.2/mltools/ml4xcube/gapfilling/gap_filling.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 17:35:39.385018 ml4xcube-0.0.2/mltools/ml4xcube/gapfilling/helper/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:36:00.000000 ml4xcube-0.0.2/mltools/ml4xcube/gapfilling/helper/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4441 2024-05-01 14:21:50.000000 ml4xcube-0.0.2/mltools/ml4xcube/gapfilling/helper/lcc.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2365 2024-05-01 13:43:43.000000 ml4xcube-0.0.2/mltools/ml4xcube/geo_plots.py
--rw-rw-r--   0 julia     (1000) julia     (1000)      389 2024-05-01 13:43:43.000000 ml4xcube-0.0.2/mltools/ml4xcube/preprocessing.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     1384 2024-05-01 14:33:44.000000 ml4xcube-0.0.2/mltools/ml4xcube/statistics.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 17:35:39.385018 ml4xcube-0.0.2/mltools/ml4xcube/training/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:23:29.000000 ml4xcube-0.0.2/mltools/ml4xcube/training/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4560 2024-05-01 13:43:43.000000 ml4xcube-0.0.2/mltools/ml4xcube/training/pytorch.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     8840 2024-05-01 14:01:45.000000 ml4xcube-0.0.2/mltools/ml4xcube/training/pytorch_distributed.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     3776 2024-05-02 11:04:54.000000 ml4xcube-0.0.2/mltools/ml4xcube/training/sklearn.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2946 2024-05-01 13:43:43.000000 ml4xcube-0.0.2/mltools/ml4xcube/training/tensorflow.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 17:35:39.385018 ml4xcube-0.0.2/mltools/ml4xcube.egg-info/
--rw-r--r--   0 julia     (1000) julia     (1000)     3660 2024-05-02 17:35:39.000000 ml4xcube-0.0.2/mltools/ml4xcube.egg-info/PKG-INFO
--rw-rw-r--   0 julia     (1000) julia     (1000)     1036 2024-05-02 17:35:39.000000 ml4xcube-0.0.2/mltools/ml4xcube.egg-info/SOURCES.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)        1 2024-05-02 17:35:39.000000 ml4xcube-0.0.2/mltools/ml4xcube.egg-info/dependency_links.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)      185 2024-05-02 17:35:39.000000 ml4xcube-0.0.2/mltools/ml4xcube.egg-info/requires.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)        9 2024-05-02 17:35:39.000000 ml4xcube-0.0.2/mltools/ml4xcube.egg-info/top_level.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)      561 2024-05-02 17:35:05.000000 ml4xcube-0.0.2/pyproject.toml
--rw-rw-r--   0 julia     (1000) julia     (1000)       38 2024-05-02 17:35:39.385018 ml4xcube-0.0.2/setup.cfg
--rw-rw-r--   0 julia     (1000) julia     (1000)      543 2024-05-02 17:35:14.000000 ml4xcube-0.0.2/setup.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1113 2024-04-23 08:43:03.000000 ml4xcube-0.0.3/LICENSE
+-rw-rw-r--   0 julia     (1000) julia     (1000)       33 2024-04-23 08:43:03.000000 ml4xcube-0.0.3/MANIFEST.in
+-rw-r--r--   0 julia     (1000) julia     (1000)     3628 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/PKG-INFO
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1643 2024-05-02 18:02:31.000000 ml4xcube-0.0.3/README.md
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.995138 ml4xcube-0.0.3/mltools/
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-04-23 11:53:26.000000 ml4xcube-0.0.3/mltools/ml4xcube/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     5544 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/cube_utilities.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2378 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/data_assignment.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube/datasets/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-02 10:14:25.000000 ml4xcube-0.0.3/mltools/ml4xcube/datasets/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2765 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/datasets/pytorch_xr.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4292 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/datasets/tensorflow_xr.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4242 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/datasets/xr_dataset.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:35:17.000000 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    14356 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/gap_dataset.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    31651 2024-05-02 16:06:56.000000 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/gap_filling.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/helper/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:36:00.000000 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/helper/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4441 2024-05-01 14:21:50.000000 ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/helper/lcc.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2365 2024-05-01 13:43:43.000000 ml4xcube-0.0.3/mltools/ml4xcube/geo_plots.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)      389 2024-05-01 13:43:43.000000 ml4xcube-0.0.3/mltools/ml4xcube/preprocessing.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1384 2024-05-01 14:33:44.000000 ml4xcube-0.0.3/mltools/ml4xcube/statistics.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube/training/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:23:29.000000 ml4xcube-0.0.3/mltools/ml4xcube/training/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4560 2024-05-01 13:43:43.000000 ml4xcube-0.0.3/mltools/ml4xcube/training/pytorch.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     8840 2024-05-01 14:01:45.000000 ml4xcube-0.0.3/mltools/ml4xcube/training/pytorch_distributed.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     3776 2024-05-02 11:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube/training/sklearn.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2946 2024-05-01 13:43:43.000000 ml4xcube-0.0.3/mltools/ml4xcube/training/tensorflow.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/
+-rw-r--r--   0 julia     (1000) julia     (1000)     3628 2024-05-02 18:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/PKG-INFO
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1036 2024-05-02 18:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/SOURCES.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)        1 2024-05-02 18:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/dependency_links.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)      169 2024-05-02 18:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/requires.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)        9 2024-05-02 18:04:54.000000 ml4xcube-0.0.3/mltools/ml4xcube.egg-info/top_level.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)      561 2024-05-02 17:57:36.000000 ml4xcube-0.0.3/pyproject.toml
+-rw-rw-r--   0 julia     (1000) julia     (1000)       38 2024-05-02 18:04:54.999138 ml4xcube-0.0.3/setup.cfg
+-rw-rw-r--   0 julia     (1000) julia     (1000)      514 2024-05-02 17:57:26.000000 ml4xcube-0.0.3/setup.py
```

### Comparing `ml4xcube-0.0.2/LICENSE` & `ml4xcube-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/PKG-INFO` & `ml4xcube-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4xcube
-Version: 0.0.2
+Version: 0.0.3
 Summary: ML package for data cubes
 Author-email: Julia Peters <julia.peters@informatik.uni-leipzig.de>
 License: MIT License
         
         Copyright (c) 2022 by ScaDS.AI, the xcube development team and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,37 +26,36 @@
         SOFTWARE.
         
 Keywords: machine learning,tools,data cube utilities
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: bokeh<3,>=2.4.3
-Requires-Dist: dask>2023.1
-Requires-Dist: dask-core>2023.1
+Requires-Dist: bokeh>=2.4.3
+Requires-Dist: dask>=2023.2.0
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: mypy_extensions==1.0.0
 Requires-Dist: numpy>=1.24
 Requires-Dist: pandas>=2.2
 Requires-Dist: scikit-learn>1.3.1
-Requires-Dist: xarray>=2024.0
+Requires-Dist: xarray>2023.8.0
 Requires-Dist: zarr>2.11
 Requires-Dist: rechunker>=0.5.1
 Requires-Dist: sentinelhub
 Requires-Dist: xcube
 
 # ML-Toolkits
 
 The ML Toolkits provide a set of best practice Python-based Jupyter Notebooks that showcase the implementation of the three start-of-the-art Machine Learning libraries (1) scikit-learn, (2) PyTorch and (3) TensorFlow based on the Earth System Data Cube.
 
 ## Installation
 
 You can install `ml4xcube` directly via pip:
 ```bash
-pip install ml4scube
+pip install ml4xcube
 ```
 
 Make sure you have Python version 3.8 or higher.
 
 If you're planning to use `ml4xcube` with TensorFlow or PyTorch, set up these frameworks properly in your Conda environment. 
 
 ## Features
@@ -97,8 +96,8 @@
 
 # Start training
 reg_model = trainer.train()
 ```
 
 ## License
 
-ml4xcube is released under the MIT License. See the [LICENSE](https://github.com/deepesdl/ML-Toolkits/blob/develop/LICENSE) file for more details.
+ml4xcube is released under the MIT License. See the [LICENSE](https://github.com/deepesdl/ML-Toolkits/blob/master/LICENSE) file for more details.
```

### Comparing `ml4xcube-0.0.2/README.md` & `ml4xcube-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 The ML Toolkits provide a set of best practice Python-based Jupyter Notebooks that showcase the implementation of the three start-of-the-art Machine Learning libraries (1) scikit-learn, (2) PyTorch and (3) TensorFlow based on the Earth System Data Cube.
 
 ## Installation
 
 You can install `ml4xcube` directly via pip:
 ```bash
-pip install ml4scube
+pip install ml4xcube
 ```
 
 Make sure you have Python version 3.8 or higher.
 
 If you're planning to use `ml4xcube` with TensorFlow or PyTorch, set up these frameworks properly in your Conda environment. 
 
 ## Features
@@ -51,8 +51,8 @@
 
 # Start training
 reg_model = trainer.train()
 ```
 
 ## License
 
-ml4xcube is released under the MIT License. See the [LICENSE](https://github.com/deepesdl/ML-Toolkits/blob/develop/LICENSE) file for more details.
+ml4xcube is released under the MIT License. See the [LICENSE](https://github.com/deepesdl/ML-Toolkits/blob/master/LICENSE) file for more details.
```

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/cube_utilities.py` & `ml4xcube-0.0.3/mltools/ml4xcube/cube_utilities.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/data_assignment.py` & `ml4xcube-0.0.3/mltools/ml4xcube/data_assignment.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/datasets/pytorch_xr.py` & `ml4xcube-0.0.3/mltools/ml4xcube/datasets/pytorch_xr.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/datasets/tensorflow_xr.py` & `ml4xcube-0.0.3/mltools/ml4xcube/datasets/tensorflow_xr.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/datasets/xr_dataset.py` & `ml4xcube-0.0.3/mltools/ml4xcube/datasets/xr_dataset.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/gapfilling/gap_dataset.py` & `ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/gap_dataset.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/gapfilling/gap_filling.py` & `ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/gap_filling.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/gapfilling/helper/lcc.py` & `ml4xcube-0.0.3/mltools/ml4xcube/gapfilling/helper/lcc.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/geo_plots.py` & `ml4xcube-0.0.3/mltools/ml4xcube/geo_plots.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/statistics.py` & `ml4xcube-0.0.3/mltools/ml4xcube/statistics.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/training/pytorch.py` & `ml4xcube-0.0.3/mltools/ml4xcube/training/pytorch.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/training/pytorch_distributed.py` & `ml4xcube-0.0.3/mltools/ml4xcube/training/pytorch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/training/sklearn.py` & `ml4xcube-0.0.3/mltools/ml4xcube/training/sklearn.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube/training/tensorflow.py` & `ml4xcube-0.0.3/mltools/ml4xcube/training/tensorflow.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube.egg-info/PKG-INFO` & `ml4xcube-0.0.3/mltools/ml4xcube.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4xcube
-Version: 0.0.2
+Version: 0.0.3
 Summary: ML package for data cubes
 Author-email: Julia Peters <julia.peters@informatik.uni-leipzig.de>
 License: MIT License
         
         Copyright (c) 2022 by ScaDS.AI, the xcube development team and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,37 +26,36 @@
         SOFTWARE.
         
 Keywords: machine learning,tools,data cube utilities
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: bokeh<3,>=2.4.3
-Requires-Dist: dask>2023.1
-Requires-Dist: dask-core>2023.1
+Requires-Dist: bokeh>=2.4.3
+Requires-Dist: dask>=2023.2.0
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: mypy_extensions==1.0.0
 Requires-Dist: numpy>=1.24
 Requires-Dist: pandas>=2.2
 Requires-Dist: scikit-learn>1.3.1
-Requires-Dist: xarray>=2024.0
+Requires-Dist: xarray>2023.8.0
 Requires-Dist: zarr>2.11
 Requires-Dist: rechunker>=0.5.1
 Requires-Dist: sentinelhub
 Requires-Dist: xcube
 
 # ML-Toolkits
 
 The ML Toolkits provide a set of best practice Python-based Jupyter Notebooks that showcase the implementation of the three start-of-the-art Machine Learning libraries (1) scikit-learn, (2) PyTorch and (3) TensorFlow based on the Earth System Data Cube.
 
 ## Installation
 
 You can install `ml4xcube` directly via pip:
 ```bash
-pip install ml4scube
+pip install ml4xcube
 ```
 
 Make sure you have Python version 3.8 or higher.
 
 If you're planning to use `ml4xcube` with TensorFlow or PyTorch, set up these frameworks properly in your Conda environment. 
 
 ## Features
@@ -97,8 +96,8 @@
 
 # Start training
 reg_model = trainer.train()
 ```
 
 ## License
 
-ml4xcube is released under the MIT License. See the [LICENSE](https://github.com/deepesdl/ML-Toolkits/blob/develop/LICENSE) file for more details.
+ml4xcube is released under the MIT License. See the [LICENSE](https://github.com/deepesdl/ML-Toolkits/blob/master/LICENSE) file for more details.
```

### Comparing `ml4xcube-0.0.2/mltools/ml4xcube.egg-info/SOURCES.txt` & `ml4xcube-0.0.3/mltools/ml4xcube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.2/pyproject.toml` & `ml4xcube-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ml4xcube"
-version = "0.0.2"
+version = "0.0.3"
 dynamic = ["dependencies"]
 description = "ML package for data cubes"
 authors = [{ name = "Julia Peters", email = "julia.peters@informatik.uni-leipzig.de" }]
 readme = "./README.md"
 license = { file = "LICENSE" }
 keywords = ["machine learning", "tools", "data cube utilities"]
 classifiers = [
```

### Comparing `ml4xcube-0.0.2/setup.py` & `ml4xcube-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ml4xcube',
-    version='0.0.2',
+    version='0.0.3',
     package_dir={'': 'mltools'},
     packages=find_packages(where='mltools'),
     install_requires=[
-        'bokeh >=2.4.3, <3',
-        'dask >2023.1',
-        'dask-core >2023.1',
+        'bokeh >=2.4.3',
+        'dask >=2023.2.0',
         'jinja2 ==3.1.3',
         'mypy_extensions ==1.0.0',
         'numpy >=1.24',
         'pandas >=2.2',
         'scikit-learn >1.3.1',
-        'xarray >=2024.0',
+        'xarray >2023.8.0',
         'zarr >2.11',
         'rechunker >=0.5.1',
         'sentinelhub',
         'xcube'
     ],
 )
```

