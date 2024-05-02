# Comparing `tmp/GReNaDIne-0.1.8.tar.gz` & `tmp/GReNaDIne-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GReNaDIne-0.1.8.tar", last modified: Wed Dec 20 14:22:46 2023, max compression
+gzip compressed data, was "GReNaDIne-0.1.9.tar", last modified: Wed Dec 20 16:52:00 2023, max compression
```

## Comparing `GReNaDIne-0.1.8.tar` & `GReNaDIne-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 14:22:46.540857 GReNaDIne-0.1.8/
-drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 14:22:46.536120 GReNaDIne-0.1.8/GReNaDIne.egg-info/
--rw-r--r--   0 speignier   (502) staff       (20)     2276 2023-12-20 14:22:46.000000 GReNaDIne-0.1.8/GReNaDIne.egg-info/PKG-INFO
--rw-r--r--   0 speignier   (502) staff       (20)      791 2023-12-20 14:22:46.000000 GReNaDIne-0.1.8/GReNaDIne.egg-info/SOURCES.txt
--rw-r--r--   0 speignier   (502) staff       (20)        1 2023-12-20 14:22:46.000000 GReNaDIne-0.1.8/GReNaDIne.egg-info/dependency_links.txt
--rw-r--r--   0 speignier   (502) staff       (20)       37 2023-12-20 14:22:46.000000 GReNaDIne-0.1.8/GReNaDIne.egg-info/requires.txt
--rw-r--r--   0 speignier   (502) staff       (20)       10 2023-12-20 14:22:46.000000 GReNaDIne-0.1.8/GReNaDIne.egg-info/top_level.txt
--rw-r--r--   0 speignier   (502) staff       (20)    35057 2023-12-16 11:04:30.000000 GReNaDIne-0.1.8/LICENSE
--rw-r--r--   0 speignier   (502) staff       (20)     2276 2023-12-20 14:22:46.540737 GReNaDIne-0.1.8/PKG-INFO
--rw-r--r--   0 speignier   (502) staff       (20)     1823 2023-12-16 11:04:30.000000 GReNaDIne-0.1.8/README.md
-drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 14:22:46.536235 GReNaDIne-0.1.8/grenadine/
-drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 14:22:46.536554 GReNaDIne-0.1.8/grenadine/Evaluation/
--rw-r--r--   0 speignier   (502) staff       (20)      391 2023-12-16 11:04:30.000000 GReNaDIne-0.1.8/grenadine/Evaluation/__init__.py
--rw-r--r--   0 speignier   (502) staff       (20)    40895 2023-12-16 11:04:30.000000 GReNaDIne-0.1.8/grenadine/Evaluation/evaluation.py
-drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 14:22:46.537673 GReNaDIne-0.1.8/grenadine/Inference/
--rw-r--r--   0 speignier   (502) staff       (20)      369 2023-12-16 11:04:30.000000 GReNaDIne-0.1.8/grenadine/Inference/__init__.py
--rw-r--r--   0 speignier   (502) staff       (20)    16153 2023-12-19 10:35:49.000000 GReNaDIne-0.1.8/grenadine/Inference/classification_predictors.py
--rw-r--r--   0 speignier   (502) staff       (20)    37359 2023-12-20 14:21:54.000000 GReNaDIne-0.1.8/grenadine/Inference/inference.py
--rw-r--r--   0 speignier   (502) staff       (20)    20780 2023-12-19 10:35:38.000000 GReNaDIne-0.1.8/grenadine/Inference/regression_predictors.py
--rw-r--r--   0 speignier   (502) staff       (20)    15219 2023-12-19 10:35:44.000000 GReNaDIne-0.1.8/grenadine/Inference/statistical_predictors.py
-drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 14:22:46.538011 GReNaDIne-0.1.8/grenadine/Model/
--rw-r--r--   0 speignier   (502) staff       (20)      349 2023-12-16 11:04:30.000000 GReNaDIne-0.1.8/grenadine/Model/__init__.py
--rw-r--r--   0 speignier   (502) staff       (20)    12348 2023-12-19 10:36:49.000000 GReNaDIne-0.1.8/grenadine/Model/model.py
-drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 14:22:46.539851 GReNaDIne-0.1.8/grenadine/Preprocessing/
--rw-r--r--   0 speignier   (502) staff       (20)      408 2023-12-16 11:04:30.000000 GReNaDIne-0.1.8/grenadine/Preprocessing/__init__.py
--rw-r--r--   0 speignier   (502) staff       (20)     7773 2023-12-19 14:44:04.000000 GReNaDIne-0.1.8/grenadine/Preprocessing/discretization.py
--rw-r--r--   0 speignier   (502) staff       (20)    11502 2023-12-19 10:36:16.000000 GReNaDIne-0.1.8/grenadine/Preprocessing/rnaseq_normalization.py
--rw-r--r--   0 speignier   (502) staff       (20)     7640 2023-12-19 10:36:23.000000 GReNaDIne-0.1.8/grenadine/Preprocessing/standard_preprocessing.py
-drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 14:22:46.540553 GReNaDIne-0.1.8/grenadine/Visualisation/
--rw-r--r--   0 speignier   (502) staff       (20)      387 2023-12-16 11:04:30.000000 GReNaDIne-0.1.8/grenadine/Visualisation/__init__.py
--rw-r--r--   0 speignier   (502) staff       (20)     5488 2023-12-19 10:44:57.000000 GReNaDIne-0.1.8/grenadine/Visualisation/visualisation.py
--rw-r--r--   0 speignier   (502) staff       (20)      466 2023-12-20 14:22:13.000000 GReNaDIne-0.1.8/grenadine/__init__.py
--rw-r--r--   0 speignier   (502) staff       (20)       38 2023-12-20 14:22:46.540898 GReNaDIne-0.1.8/setup.cfg
--rw-r--r--   0 speignier   (502) staff       (20)      820 2023-12-20 14:22:17.000000 GReNaDIne-0.1.8/setup.py
+drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 16:52:00.694071 GReNaDIne-0.1.9/
+drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 16:52:00.691511 GReNaDIne-0.1.9/GReNaDIne.egg-info/
+-rw-r--r--   0 speignier   (502) staff       (20)     2276 2023-12-20 16:52:00.000000 GReNaDIne-0.1.9/GReNaDIne.egg-info/PKG-INFO
+-rw-r--r--   0 speignier   (502) staff       (20)      791 2023-12-20 16:52:00.000000 GReNaDIne-0.1.9/GReNaDIne.egg-info/SOURCES.txt
+-rw-r--r--   0 speignier   (502) staff       (20)        1 2023-12-20 16:52:00.000000 GReNaDIne-0.1.9/GReNaDIne.egg-info/dependency_links.txt
+-rw-r--r--   0 speignier   (502) staff       (20)       37 2023-12-20 16:52:00.000000 GReNaDIne-0.1.9/GReNaDIne.egg-info/requires.txt
+-rw-r--r--   0 speignier   (502) staff       (20)       10 2023-12-20 16:52:00.000000 GReNaDIne-0.1.9/GReNaDIne.egg-info/top_level.txt
+-rw-r--r--   0 speignier   (502) staff       (20)    35057 2023-12-16 11:04:30.000000 GReNaDIne-0.1.9/LICENSE
+-rw-r--r--   0 speignier   (502) staff       (20)     2276 2023-12-20 16:52:00.693957 GReNaDIne-0.1.9/PKG-INFO
+-rw-r--r--   0 speignier   (502) staff       (20)     1823 2023-12-16 11:04:30.000000 GReNaDIne-0.1.9/README.md
+drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 16:52:00.691724 GReNaDIne-0.1.9/grenadine/
+drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 16:52:00.692003 GReNaDIne-0.1.9/grenadine/Evaluation/
+-rw-r--r--   0 speignier   (502) staff       (20)      391 2023-12-16 11:04:30.000000 GReNaDIne-0.1.9/grenadine/Evaluation/__init__.py
+-rw-r--r--   0 speignier   (502) staff       (20)    40895 2023-12-16 11:04:30.000000 GReNaDIne-0.1.9/grenadine/Evaluation/evaluation.py
+drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 16:52:00.692685 GReNaDIne-0.1.9/grenadine/Inference/
+-rw-r--r--   0 speignier   (502) staff       (20)      369 2023-12-16 11:04:30.000000 GReNaDIne-0.1.9/grenadine/Inference/__init__.py
+-rw-r--r--   0 speignier   (502) staff       (20)    16153 2023-12-19 10:35:49.000000 GReNaDIne-0.1.9/grenadine/Inference/classification_predictors.py
+-rw-r--r--   0 speignier   (502) staff       (20)    37597 2023-12-20 16:50:44.000000 GReNaDIne-0.1.9/grenadine/Inference/inference.py
+-rw-r--r--   0 speignier   (502) staff       (20)    20780 2023-12-19 10:35:38.000000 GReNaDIne-0.1.9/grenadine/Inference/regression_predictors.py
+-rw-r--r--   0 speignier   (502) staff       (20)    15219 2023-12-19 10:35:44.000000 GReNaDIne-0.1.9/grenadine/Inference/statistical_predictors.py
+drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 16:52:00.692991 GReNaDIne-0.1.9/grenadine/Model/
+-rw-r--r--   0 speignier   (502) staff       (20)      349 2023-12-16 11:04:30.000000 GReNaDIne-0.1.9/grenadine/Model/__init__.py
+-rw-r--r--   0 speignier   (502) staff       (20)    12348 2023-12-19 10:36:49.000000 GReNaDIne-0.1.9/grenadine/Model/model.py
+drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 16:52:00.693532 GReNaDIne-0.1.9/grenadine/Preprocessing/
+-rw-r--r--   0 speignier   (502) staff       (20)      408 2023-12-16 11:04:30.000000 GReNaDIne-0.1.9/grenadine/Preprocessing/__init__.py
+-rw-r--r--   0 speignier   (502) staff       (20)     7773 2023-12-19 14:44:04.000000 GReNaDIne-0.1.9/grenadine/Preprocessing/discretization.py
+-rw-r--r--   0 speignier   (502) staff       (20)    11502 2023-12-19 10:36:16.000000 GReNaDIne-0.1.9/grenadine/Preprocessing/rnaseq_normalization.py
+-rw-r--r--   0 speignier   (502) staff       (20)     7640 2023-12-19 10:36:23.000000 GReNaDIne-0.1.9/grenadine/Preprocessing/standard_preprocessing.py
+drwxr-xr-x   0 speignier   (502) staff       (20)        0 2023-12-20 16:52:00.693800 GReNaDIne-0.1.9/grenadine/Visualisation/
+-rw-r--r--   0 speignier   (502) staff       (20)      387 2023-12-16 11:04:30.000000 GReNaDIne-0.1.9/grenadine/Visualisation/__init__.py
+-rw-r--r--   0 speignier   (502) staff       (20)     5488 2023-12-19 10:44:57.000000 GReNaDIne-0.1.9/grenadine/Visualisation/visualisation.py
+-rw-r--r--   0 speignier   (502) staff       (20)      466 2023-12-20 16:50:59.000000 GReNaDIne-0.1.9/grenadine/__init__.py
+-rw-r--r--   0 speignier   (502) staff       (20)       38 2023-12-20 16:52:00.694109 GReNaDIne-0.1.9/setup.cfg
+-rw-r--r--   0 speignier   (502) staff       (20)      820 2023-12-20 16:51:06.000000 GReNaDIne-0.1.9/setup.py
```

### Comparing `GReNaDIne-0.1.8/GReNaDIne.egg-info/PKG-INFO` & `GReNaDIne-0.1.9/GReNaDIne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GReNaDIne
-Version: 0.1.8
+Version: 0.1.9
 Summary: Data-Driven Gene Regulatory Network Inference
 Home-page: 
 Author: Sergio Peignier, Pauline Schmitt, Timothée Frouté
 Author-email: sergio.peignier@insa-lyon.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `GReNaDIne-0.1.8/GReNaDIne.egg-info/SOURCES.txt` & `GReNaDIne-0.1.9/GReNaDIne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/LICENSE` & `GReNaDIne-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/PKG-INFO` & `GReNaDIne-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GReNaDIne
-Version: 0.1.8
+Version: 0.1.9
 Summary: Data-Driven Gene Regulatory Network Inference
 Home-page: 
 Author: Sergio Peignier, Pauline Schmitt, Timothée Frouté
 Author-email: sergio.peignier@insa-lyon.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `GReNaDIne-0.1.8/README.md` & `GReNaDIne-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/grenadine/Evaluation/evaluation.py` & `GReNaDIne-0.1.9/grenadine/Evaluation/evaluation.py`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/grenadine/Inference/classification_predictors.py` & `GReNaDIne-0.1.9/grenadine/Inference/classification_predictors.py`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/grenadine/Inference/inference.py` & `GReNaDIne-0.1.9/grenadine/Inference/inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,17 @@
         >>> gm = gene_model(params_gridsearch)
 
 
     """
     def __init__(self,params_gridsearch,verbose=True):
         self.params_gridsearch = params_gridsearch
         self.verbose = verbose
+        self.C_ = None
+        self.scores_ = None
+        self.gene_models_ = None
         
     def fit(self,X,Y,regulators,to_inspect=None):  
         """
         Fit the self expressive gene regulatory model
 
         Args:
             X (pandas.DataFrame): Predictor gene expression matrix where 
@@ -439,16 +442,22 @@
             >>> def score_criteria(score):
                     score["mean_train_roc_auc_ovr_weighted"]>0.6 and score["mean_test_average_precision"]>0.6
             >>> gxn.purify_model(score_criteria)
 
         """
         mask = [i for i in self.scores_.index if score_condition(self.scores_.loc[i])]
         gene_models_ = {i:self.gene_models_[i] for i in mask}
-        C_ = self.C_.loc[mask]
-        scores_ = self.scores_.loc[mask]
+        if self.C_ is not None:
+            C_ = self.C_.loc[mask]
+        else:
+            C_ = None
+        if self.scores_ is not None:
+            scores_ = self.scores_.loc[mask]
+        else:
+            scores_ = None
         if inplace:
             self.gene_models_ = gene_models_
             self.C_ = C_
             self.scores_ = scores_
             return self
         else:
             purified_model = gxn_model(self.params_gridsearch)
```

### Comparing `GReNaDIne-0.1.8/grenadine/Inference/regression_predictors.py` & `GReNaDIne-0.1.9/grenadine/Inference/regression_predictors.py`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/grenadine/Inference/statistical_predictors.py` & `GReNaDIne-0.1.9/grenadine/Inference/statistical_predictors.py`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/grenadine/Model/model.py` & `GReNaDIne-0.1.9/grenadine/Model/model.py`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/grenadine/Preprocessing/discretization.py` & `GReNaDIne-0.1.9/grenadine/Preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/grenadine/Preprocessing/rnaseq_normalization.py` & `GReNaDIne-0.1.9/grenadine/Preprocessing/rnaseq_normalization.py`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/grenadine/Preprocessing/standard_preprocessing.py` & `GReNaDIne-0.1.9/grenadine/Preprocessing/standard_preprocessing.py`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/grenadine/Visualisation/visualisation.py` & `GReNaDIne-0.1.9/grenadine/Visualisation/visualisation.py`

 * *Files identical despite different names*

### Comparing `GReNaDIne-0.1.8/setup.py` & `GReNaDIne-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="GReNaDIne",
-    version="0.1.8",
+    version="0.1.9",
     author="Sergio Peignier, Pauline Schmitt, Timothée Frouté",
     author_email="sergio.peignier@insa-lyon.fr",
     description="Data-Driven Gene Regulatory Network Inference",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

