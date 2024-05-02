# Comparing `tmp/PySCIPOpt-ML-1.0.0.tar.gz` & `tmp/pyscipopt_ml-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySCIPOpt-ML-1.0.0.tar", last modified: Fri Mar 22 12:17:31 2024, max compression
+gzip compressed data, was "pyscipopt_ml-1.1.0.tar", last modified: Thu May  2 10:00:28 2024, max compression
```

## Comparing `PySCIPOpt-ML-1.0.0.tar` & `pyscipopt_ml-1.1.0.tar`

### file list

```diff
@@ -1,80 +1,82 @@
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.011365 PySCIPOpt-ML-1.0.0/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    11357 2023-12-10 20:29:52.000000 PySCIPOpt-ML-1.0.0/LICENSE
--rw-r--r--   0 bzfturne  (1000) bzfturne  (1000)     4839 2024-03-22 12:17:31.011365 PySCIPOpt-ML-1.0.0/PKG-INFO
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     4202 2024-03-11 14:50:05.000000 PySCIPOpt-ML-1.0.0/README.md
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      732 2024-03-22 12:16:58.000000 PySCIPOpt-ML-1.0.0/pyproject.toml
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      124 2024-03-22 12:17:31.011365 PySCIPOpt-ML-1.0.0/setup.cfg
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.003365 PySCIPOpt-ML-1.0.0/src/
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.011365 PySCIPOpt-ML-1.0.0/src/PySCIPOpt_ML.egg-info/
--rw-r--r--   0 bzfturne  (1000) bzfturne  (1000)     4839 2024-03-22 12:17:30.000000 PySCIPOpt-ML-1.0.0/src/PySCIPOpt_ML.egg-info/PKG-INFO
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     2508 2024-03-22 12:17:31.000000 PySCIPOpt-ML-1.0.0/src/PySCIPOpt_ML.egg-info/SOURCES.txt
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)        1 2024-03-22 12:17:30.000000 PySCIPOpt-ML-1.0.0/src/PySCIPOpt_ML.egg-info/dependency_links.txt
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       23 2024-03-22 12:17:30.000000 PySCIPOpt-ML-1.0.0/src/PySCIPOpt_ML.egg-info/requires.txt
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       13 2024-03-22 12:17:30.000000 PySCIPOpt-ML-1.0.0/src/PySCIPOpt_ML.egg-info/top_level.txt
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.003365 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      686 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/__init__.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      557 2023-12-05 11:55:26.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/_version.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     2715 2023-12-10 21:09:47.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/add_predictor.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      855 2023-10-26 07:56:52.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/exceptions.py
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.007365 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/keras/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       36 2024-03-06 15:15:13.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/keras/__init__.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    10673 2024-03-06 15:15:13.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/keras/keras.py
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.007365 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/lightgbm/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       79 2023-12-05 11:56:09.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/lightgbm/__init__.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7698 2024-03-11 14:50:05.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/lightgbm/lgbgetter.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     6352 2023-12-10 21:09:47.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/lightgbm/lightgbm_constr.py
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.007365 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      155 2023-12-05 10:28:42.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/__init__.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    11553 2024-03-22 11:59:31.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/base_predictor_constraint.py
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.007365 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/classification/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       90 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/classification/__init__.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7463 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/classification/argmax_model.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     4271 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/classification/max_model.py
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.007365 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/decision_tree/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       50 2023-10-26 07:56:52.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/decision_tree/__init__.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     8489 2023-12-10 21:09:47.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/decision_tree/decision_tree_model.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      676 2023-12-10 20:05:17.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/get_convertor.py
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.007365 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/gradient_boosting/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      209 2023-12-10 21:09:47.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/gradient_boosting/__init__.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    13867 2024-03-11 14:50:05.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/gradient_boosting/aggregate_tree_model.py
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.007365 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/neuralnet/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       37 2023-12-05 10:28:42.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/neuralnet/__init__.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    10468 2023-12-10 21:09:47.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/neuralnet/activations.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     5239 2024-03-06 15:15:13.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/neuralnet/layers.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     3109 2023-12-10 21:09:47.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/neuralnet/neural_net.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     2415 2023-12-10 21:09:47.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/var_utils.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     4913 2024-03-22 12:12:48.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/registered_predictors.py
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.007365 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      908 2024-03-22 12:12:48.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/__init__.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     2043 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/base_regression.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7727 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/centroid_cluster.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     6039 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/decision_tree.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     6551 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/gradient_boosting.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     3032 2023-12-10 20:22:27.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/linear_regression.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     9316 2024-03-11 14:50:05.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/logistic_regression.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7202 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/mlp.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     5525 2024-03-22 10:44:54.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/multi_output.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     5737 2024-03-22 12:11:56.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/pipeline.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     3491 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/pls.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    14481 2024-03-22 12:09:30.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/preprocessing.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     6074 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/random_forest.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     5226 2024-03-22 10:52:26.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/skgetter.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     8363 2024-03-22 08:40:22.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/support_vector.py
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.007365 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/torch/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       46 2023-12-05 10:28:42.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/torch/__init__.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    10269 2024-03-06 15:15:13.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/torch/sequential.py
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.011365 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/xgboost/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      156 2023-12-10 21:09:47.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/xgboost/__init__.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     6497 2024-03-11 14:50:05.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/xgboost/xgbgetter.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    10202 2023-12-10 21:09:48.000000 PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/xgboost/xgboost_constr.py
-drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-03-22 12:17:31.011365 PySCIPOpt-ML-1.0.0/tests/
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7870 2024-03-06 15:15:13.000000 PySCIPOpt-ML-1.0.0/tests/test_adversarial_example.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     2082 2023-12-10 21:09:48.000000 PySCIPOpt-ML-1.0.0/tests/test_airline_satisfcation.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    10119 2023-12-11 16:20:50.000000 PySCIPOpt-ML-1.0.0/tests/test_auto_manufacturer.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    14711 2023-12-11 16:27:42.000000 PySCIPOpt-ML-1.0.0/tests/test_city_manager.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7967 2024-03-22 12:10:12.000000 PySCIPOpt-ML-1.0.0/tests/test_formulation_error.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     5364 2024-03-11 14:50:05.000000 PySCIPOpt-ML-1.0.0/tests/test_input_types.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     9394 2024-03-06 15:15:13.000000 PySCIPOpt-ML-1.0.0/tests/test_simple_function_approximation.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    11123 2023-12-11 16:22:27.000000 PySCIPOpt-ML-1.0.0/tests/test_tree_planting.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7944 2024-03-06 15:15:13.000000 PySCIPOpt-ML-1.0.0/tests/test_water_potability.py
--rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    10540 2023-12-11 16:28:10.000000 PySCIPOpt-ML-1.0.0/tests/test_wine_manufacturer.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.612534 pyscipopt_ml-1.1.0/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    11357 2023-12-10 20:29:52.000000 pyscipopt_ml-1.1.0/LICENSE
+-rw-r--r--   0 bzfturne  (1000) bzfturne  (1000)     4839 2024-05-02 10:00:28.612534 pyscipopt_ml-1.1.0/PKG-INFO
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     4202 2024-03-11 14:50:05.000000 pyscipopt_ml-1.1.0/README.md
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      732 2024-05-02 09:35:56.000000 pyscipopt_ml-1.1.0/pyproject.toml
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      124 2024-05-02 10:00:28.612534 pyscipopt_ml-1.1.0/setup.cfg
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.600534 pyscipopt_ml-1.1.0/src/
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.612534 pyscipopt_ml-1.1.0/src/PySCIPOpt_ML.egg-info/
+-rw-r--r--   0 bzfturne  (1000) bzfturne  (1000)     4839 2024-05-02 10:00:28.000000 pyscipopt_ml-1.1.0/src/PySCIPOpt_ML.egg-info/PKG-INFO
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     2580 2024-05-02 10:00:28.000000 pyscipopt_ml-1.1.0/src/PySCIPOpt_ML.egg-info/SOURCES.txt
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)        1 2024-05-02 10:00:28.000000 pyscipopt_ml-1.1.0/src/PySCIPOpt_ML.egg-info/dependency_links.txt
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       23 2024-05-02 10:00:28.000000 pyscipopt_ml-1.1.0/src/PySCIPOpt_ML.egg-info/requires.txt
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       13 2024-05-02 10:00:28.000000 pyscipopt_ml-1.1.0/src/PySCIPOpt_ML.egg-info/top_level.txt
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.604534 pyscipopt_ml-1.1.0/src/pyscipopt_ml/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      686 2024-03-22 08:40:22.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/__init__.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      557 2023-12-05 11:55:26.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/_version.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     2715 2023-12-10 21:09:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/add_predictor.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      855 2023-10-26 07:56:52.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/exceptions.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.604534 pyscipopt_ml-1.1.0/src/pyscipopt_ml/keras/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       36 2024-03-06 15:15:13.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/keras/__init__.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    10662 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/keras/keras.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.604534 pyscipopt_ml-1.1.0/src/pyscipopt_ml/lightgbm/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       79 2023-12-05 11:56:09.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/lightgbm/__init__.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7698 2024-03-11 14:50:05.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/lightgbm/lgbgetter.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     6352 2023-12-10 21:09:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/lightgbm/lightgbm_constr.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.604534 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      155 2023-12-05 10:28:42.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/__init__.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    11689 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/base_predictor_constraint.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.604534 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/classification/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       90 2024-03-22 08:40:22.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/classification/__init__.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7463 2024-03-22 08:40:22.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/classification/argmax_model.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     4271 2024-03-22 08:40:22.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/classification/max_model.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.604534 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/decision_tree/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       50 2023-10-26 07:56:52.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/decision_tree/__init__.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     8489 2023-12-10 21:09:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/decision_tree/decision_tree_model.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      676 2023-12-10 20:05:17.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/get_convertor.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.604534 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/gradient_boosting/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      209 2023-12-10 21:09:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/gradient_boosting/__init__.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    13867 2024-03-11 14:50:05.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/gradient_boosting/aggregate_tree_model.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.608534 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/neuralnet/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       37 2023-12-05 10:28:42.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/neuralnet/__init__.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    12735 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/neuralnet/activations.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     5579 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/neuralnet/layers.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     3109 2023-12-10 21:09:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/neuralnet/neural_net.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     2415 2023-12-10 21:09:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/var_utils.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     4913 2024-03-22 12:42:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/registered_predictors.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.608534 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      908 2024-03-22 12:42:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/__init__.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     2043 2024-03-22 08:40:22.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/base_regression.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7727 2024-03-22 08:40:22.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/centroid_cluster.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     5830 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/decision_tree.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     6551 2024-03-22 08:40:22.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/gradient_boosting.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     3032 2023-12-10 20:22:27.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/linear_regression.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     9316 2024-03-11 14:50:05.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/logistic_regression.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7202 2024-03-22 08:40:22.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/mlp.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     5525 2024-03-22 12:42:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/multi_output.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     5737 2024-03-22 12:42:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/pipeline.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     3491 2024-03-22 08:40:22.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/pls.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    14481 2024-03-22 12:42:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/preprocessing.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     6074 2024-03-22 08:40:22.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/random_forest.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     5226 2024-03-22 12:42:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/skgetter.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     8363 2024-03-22 08:40:22.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/support_vector.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.608534 pyscipopt_ml-1.1.0/src/pyscipopt_ml/torch/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)       46 2023-12-05 10:28:42.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/torch/__init__.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    10269 2024-03-06 15:15:13.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/torch/sequential.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.612534 pyscipopt_ml-1.1.0/src/pyscipopt_ml/xgboost/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)      156 2023-12-10 21:09:47.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/xgboost/__init__.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     6497 2024-03-11 14:50:05.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/xgboost/xgbgetter.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    10202 2023-12-10 21:09:48.000000 pyscipopt_ml-1.1.0/src/pyscipopt_ml/xgboost/xgboost_constr.py
+drwxrwxr-x   0 bzfturne  (1000) bzfturne  (1000)        0 2024-05-02 10:00:28.612534 pyscipopt_ml-1.1.0/tests/
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     8525 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/tests/test_adversarial_example.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     2082 2023-12-10 21:09:48.000000 pyscipopt_ml-1.1.0/tests/test_airline_satisfcation.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    12709 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/tests/test_auto_manufacturer.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    16859 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/tests/test_city_manager.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     4974 2024-05-02 09:55:12.000000 pyscipopt_ml-1.1.0/tests/test_formulation_error.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     5364 2024-03-11 14:50:05.000000 pyscipopt_ml-1.1.0/tests/test_input_types.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     6654 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/tests/test_palatable_diet_problem.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    10505 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/tests/test_simple_function_approximation.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    13307 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/tests/test_tree_planting.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    10644 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/tests/test_water_potability.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)    12262 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/tests/test_wine_manufacturer.py
+-rw-rw-r--   0 bzfturne  (1000) bzfturne  (1000)     7497 2024-05-02 09:34:57.000000 pyscipopt_ml-1.1.0/tests/test_workload_dispatching.py
```

### Comparing `PySCIPOpt-ML-1.0.0/LICENSE` & `pyscipopt_ml-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/PKG-INFO` & `pyscipopt_ml-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySCIPOpt-ML
-Version: 1.0.0
+Version: 1.1.0
 Summary: automatically formulate and embed ML models into MIPs with SCIP
 Author: Mark Turner - Zuse Institute Berlin
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Opt-Mucca/PySCIPOpt-ML
 Project-URL: Documentation, https://pyscipopt-ml.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/Opt-Mucca/PySCIPOpt-ML/issues
 Keywords: mixed-integer programming,SCIP,scikit-learn,pytorch,xgboost,lightgbm,keras,ml
```

### Comparing `PySCIPOpt-ML-1.0.0/README.md` & `pyscipopt_ml-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/pyproject.toml` & `pyscipopt_ml-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PySCIPOpt-ML"
-version = "1.0.0"
+version = "1.1.0"
 description = "automatically formulate and embed ML models into MIPs with SCIP"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text="Apache-2.0"}
 keywords = ["mixed-integer programming", "SCIP", "scikit-learn", "pytorch", "xgboost", "lightgbm", "keras", "ml"]
 authors = [
   {name = "Mark Turner - Zuse Institute Berlin"}
```

### Comparing `PySCIPOpt-ML-1.0.0/src/PySCIPOpt_ML.egg-info/PKG-INFO` & `pyscipopt_ml-1.1.0/src/PySCIPOpt_ML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySCIPOpt-ML
-Version: 1.0.0
+Version: 1.1.0
 Summary: automatically formulate and embed ML models into MIPs with SCIP
 Author: Mark Turner - Zuse Institute Berlin
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Opt-Mucca/PySCIPOpt-ML
 Project-URL: Documentation, https://pyscipopt-ml.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/Opt-Mucca/PySCIPOpt-ML/issues
 Keywords: mixed-integer programming,SCIP,scikit-learn,pytorch,xgboost,lightgbm,keras,ml
```

### Comparing `PySCIPOpt-ML-1.0.0/src/PySCIPOpt_ML.egg-info/SOURCES.txt` & `pyscipopt_ml-1.1.0/src/PySCIPOpt_ML.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -54,11 +54,13 @@
 src/pyscipopt_ml/xgboost/xgboost_constr.py
 tests/test_adversarial_example.py
 tests/test_airline_satisfcation.py
 tests/test_auto_manufacturer.py
 tests/test_city_manager.py
 tests/test_formulation_error.py
 tests/test_input_types.py
+tests/test_palatable_diet_problem.py
 tests/test_simple_function_approximation.py
 tests/test_tree_planting.py
 tests/test_water_potability.py
-tests/test_wine_manufacturer.py
+tests/test_wine_manufacturer.py
+tests/test_workload_dispatching.py
```

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/__init__.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/_version.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/_version.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/add_predictor.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/add_predictor.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/exceptions.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/keras/keras.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/keras/keras.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             ):
                 continue
             if isinstance(step, keras.layers.Dense):
                 config = step.get_config()
                 activation = config["activation"]
                 if activation not in ("relu", "linear", "sigmoid", "tanh"):
                     raise NoModel(predictor, f"Unsupported activation {activation}")
-                out_features = step.output_shape[-1]
+                out_features = step.units
             elif isinstance(step, keras.layers.ReLU):
                 if step.negative_slope != 0.0:
                     raise NoModel(predictor, "Only handle ReLU layers with negative slope 0.0")
                 if step.threshold != 0.0:
                     raise NoModel(predictor, "Only handle ReLU layers with threshold of 0.0")
                 if step.max_value is not None and step.max_value < float("inf"):
                     raise NoModel(predictor, "Only handle ReLU layers without maxvalue")
```

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/lightgbm/lgbgetter.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/lightgbm/lgbgetter.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/lightgbm/lightgbm_constr.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/lightgbm/lightgbm_constr.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/base_predictor_constraint.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/base_predictor_constraint.py`

 * *Files 10% similar despite different names*

```diff
@@ -100,32 +100,32 @@
 
         self._input = input_vars
         self._output = output_vars
 
     def _build_predictor_model(self, **kwargs):
         self._mip_model(**kwargs)
 
-    def _get_created_vars_and_cons(self, created_vars, created_cons):
-        created_vars += self._created_vars
-        created_cons += self._created_cons
+    def _get_created_vars_and_cons(self):
+        created_vars = [c_vars for c_vars in self._created_vars]
+        created_cons = [c_cons for c_cons in self._created_cons]
         if hasattr(self, "_estimators"):
             for estimator in self._estimators:
-                created_vars, created_cons = estimator._get_created_vars_and_cons(
-                    created_vars, created_cons
-                )
+                sub_created_vars, sub_created_cons = estimator._get_created_vars_and_cons()
+                created_vars += sub_created_vars
+                created_cons += sub_created_cons
         if hasattr(self, "_layers"):
             for layer in self._layers:
-                created_vars, created_cons = layer._get_created_vars_and_cons(
-                    created_vars, created_cons
-                )
+                sub_created_vars, sub_created_cons = layer._get_created_vars_and_cons()
+                created_vars += sub_created_vars
+                created_cons += sub_created_cons
         if hasattr(self, "_steps"):
             for step in self._steps:
-                created_vars, created_cons = step._get_created_vars_and_cons(
-                    created_vars, created_cons
-                )
+                sub_created_vars, sub_created_cons = step._get_created_vars_and_cons()
+                created_vars += sub_created_vars
+                created_cons += sub_created_cons
 
         return created_vars, created_cons
 
     def print_stats(self, file=None):
         """Print statistics on model additions stored by this class.
 
         This function prints detailed statistics on the variables
@@ -139,15 +139,15 @@
         """
 
         n_indicator_cons = 0
         n_sos_cons = 0
         n_linear_cons = 0
         n_nonlinear_cons = 0
 
-        created_vars, created_cons = self._get_created_vars_and_cons([], [])
+        created_vars, created_cons = self._get_created_vars_and_cons()
         for cons_set in created_cons:
             it = np.nditer(cons_set, flags=["multi_index", "refs_ok"])
             for _ in it:
                 if isinstance(cons_set[it.multi_index], Constraint):
                     cons_type = cons_set[it.multi_index].getConshdlrName()
                     if cons_type == "indicator":
                         n_indicator_cons += 1
```

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/classification/argmax_model.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/classification/argmax_model.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/classification/max_model.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/classification/max_model.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/decision_tree/decision_tree_model.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/decision_tree/decision_tree_model.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/get_convertor.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/get_convertor.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/gradient_boosting/aggregate_tree_model.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/gradient_boosting/aggregate_tree_model.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/neuralnet/activations.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/neuralnet/activations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Internal module to make MIP modeling of activation functions."""
-
 import numpy as np
 from pyscipopt import exp, quicksum
 
 
-def add_identity_activation_constraint_layer(layer):
+def add_identity_activation_constraint_layer(layer, max_bound):
     """
     MIP model for identity activation on a layer
 
     Parameters
     ----------
     layer : AbstractNNLayer
         Layer to which activation is applied.
 
+    max_bound : float or int
+        The maximum bound for which propagation values will be stored
+
     Returns
     -------
 
     affine_cons : np.ndarray
         A numpy array containing the linear transformation constraints
 
     """
@@ -24,111 +26,145 @@
     n_samples = layer.input.shape[0]
     n_nodes_left = layer.input.shape[-1]
     n_nodes_right = layer.output.shape[-1]
     affine_cons = np.zeros((n_samples, n_nodes_right), dtype=object)
 
     # Perform some basic activity based bound propagation
     propagation_success, lbs, ubs = propagate_identity_bounds(
-        layer, n_samples, n_nodes_left, n_nodes_right, False
+        layer, n_samples, n_nodes_left, n_nodes_right, False, max_bound
     )
 
     for i in range(n_samples):
         for j in range(n_nodes_right):
             rhs = (
                 quicksum(layer.coefs[k][j] * layer.input[i][k] for k in range(n_nodes_left))
                 + layer.intercept[j]
             )
             name = layer.unique_naming_prefix + f"affine_{i}_{j}"
             affine_cons[i][j] = layer.scip_model.addCons(layer.output[i][j] == rhs, name=name)
             # Propagate bounds
             if propagation_success:
-                if abs(lbs[i][j]) < 10**5:
+                if abs(lbs[i][j]) < max_bound:
                     output_lb = layer.output[i][j].getLbOriginal()
                     layer.scip_model.chgVarLb(layer.output[i][j], max(lbs[i][j], output_lb))
-                if abs(ubs[i][j]) < 10**5:
+                if abs(ubs[i][j]) < max_bound:
                     output_ub = layer.output[i][j].getUbOriginal()
                     layer.scip_model.chgVarUb(layer.output[i][j], min(ubs[i][j], output_ub))
 
     return affine_cons
 
 
-def add_relu_activation_constraint_layer(layer, slack, activation_only=True):
+def add_relu_activation_constraint_layer(layer, aux_vars, activation_only=True, formulation="sos"):
     """
     MIP model for ReLU activation on a layer
 
     Parameters
     ----------
     layer : AbstractNNLayer
         Layer to which activation is applied.
 
-    slack : np.ndarray
-        Slack variables that will be used in the SOS formulation
+    aux_vars : np.ndarray
+        Auxiliary variables that are used for the formulation. These are slack variables for the SOS formulation
+        and binary activation variables for the Big-M formulation
 
     activation_only : bool, optional
         Whether this layer should only feature as an activation layer, i.e., skip the affine transformation
 
+    formulation : str, optional
+        The MIP formulation used for encoding the ReLU activation. Options are ["sos", "bigm"]
+
     Returns
     -------
 
-    cons_with_slack : np.ndarray
-        A numpy array containing added constraints
-
-    sos_cons : np.ndarray
-        A numpy array containing added constraints
+    relu_cons : list
+        A list of numpy arrays containing added constraints
 
     """
 
     # Initialise values for easy access and create empty constraint arrays
     n_samples = layer.input.shape[0]
     n_nodes_left = layer.input.shape[-1]
     n_nodes_right = layer.output.shape[-1]
     sos_cons = np.zeros((n_samples, n_nodes_right), dtype=object)
     cons_with_slack = np.zeros((n_samples, n_nodes_right), dtype=object)
+    big_m_lb = np.zeros((n_samples, n_nodes_right), dtype=object)
+    big_m_ub_inactive = np.zeros((n_samples, n_nodes_right), dtype=object)
+    big_m_ub_active = np.zeros((n_samples, n_nodes_right), dtype=object)
 
     # Perform some basic activity based bound propagation
+    max_bound = 10**5 if formulation == "sos" else np.inf
     propagation_success, lbs, ubs = propagate_identity_bounds(
-        layer, n_samples, n_nodes_left, n_nodes_right, activation_only
+        layer, n_samples, n_nodes_left, n_nodes_right, activation_only, layer.scip_model.infinity()
     )
 
     # Iterate over all nodes on the right hand side and create the appropriate constraints
     for i in range(n_samples):
         for j in range(n_nodes_right):
-            if layer.output[i][j].getLbOriginal() < 0:
-                layer.scip_model.chgVarLb(layer.output[i][j], 0)
-            name = layer.unique_naming_prefix + f"slack_{i}_{j}"
-            if activation_only:
-                cons_with_slack[i][j] = layer.scip_model.addCons(
-                    layer.output[i][j] == layer.input[i][j] + slack[i][j], name=name
-                )
-            else:
-                rhs = quicksum(layer.coefs[k][j] * layer.input[i][k] for k in range(n_nodes_left))
-                rhs += layer.intercept[j] + slack[i][j]
-                cons_with_slack[i][j] = layer.scip_model.addCons(
-                    layer.output[i][j] == rhs, name=name
-                )
             # Propagate bounds
             if propagation_success:
-                if abs(lbs[i][j]) < 10**5:
+                if abs(lbs[i][j]) < max_bound:
                     output_lb = layer.output[i][j].getLbOriginal()
                     layer.scip_model.chgVarLb(
                         layer.output[i][j], max(max(lbs[i][j], 0), output_lb)
                     )
-                    layer.scip_model.chgVarUb(slack[i][j], max(-lbs[i][j], 0))
-                if abs(ubs[i][j]) < 10**5:
+                    if formulation == "sos":
+                        layer.scip_model.chgVarUb(aux_vars[i][j], max(-lbs[i][j], 0))
+                if abs(ubs[i][j]) < max_bound:
                     output_ub = layer.output[i][j].getUbOriginal()
                     layer.scip_model.chgVarUb(
                         layer.output[i][j], min(max(ubs[i][j], 0), output_ub)
                     )
-                    layer.scip_model.chgVarLb(slack[i][j], max(-ubs[i][j], 0))
-            name = layer.unique_naming_prefix + f"sos_{i}_{j}"
-            sos_cons[i][j] = layer.scip_model.addConsSOS1(
-                [layer.output[i][j], slack[i][j]], name=name
-            )
+                    if formulation == "sos":
+                        layer.scip_model.chgVarLb(aux_vars[i][j], max(-ubs[i][j], 0))
+            # Create layer constraints
+            if layer.output[i][j].getLbOriginal() < 0:
+                layer.scip_model.chgVarLb(layer.output[i][j], 0)
+            if formulation == "sos":
+                name = layer.unique_naming_prefix + f"slack_{i}_{j}"
+                if activation_only:
+                    cons_with_slack[i][j] = layer.scip_model.addCons(
+                        layer.output[i][j] == layer.input[i][j] + aux_vars[i][j], name=name
+                    )
+                else:
+                    rhs = quicksum(
+                        layer.coefs[k][j] * layer.input[i][k] for k in range(n_nodes_left)
+                    )
+                    rhs += layer.intercept[j] + aux_vars[i][j]
+                    cons_with_slack[i][j] = layer.scip_model.addCons(
+                        layer.output[i][j] == rhs, name=name
+                    )
+                name = layer.unique_naming_prefix + f"sos_{i}_{j}"
+                sos_cons[i][j] = layer.scip_model.addConsSOS1(
+                    [layer.output[i][j], aux_vars[i][j]], name=name
+                )
+            else:
+                if activation_only:
+                    rhs = layer.input[i][j]
+                else:
+                    rhs = (
+                        quicksum(
+                            layer.coefs[k][j] * layer.input[i][k] for k in range(n_nodes_left)
+                        )
+                        + layer.intercept[j]
+                    )
+                name = layer.unique_naming_prefix + f"relu_lb_{i}_{j}"
+                big_m_lb[i][j] = layer.scip_model.addCons(layer.output[i][j] >= rhs, name=name)
+                name = layer.unique_naming_prefix + f"relu_ub_inactive_{i}_{j}"
+                big_m_ub_inactive[i][j] = layer.scip_model.addCons(
+                    layer.output[i][j] <= rhs - (1 - aux_vars[i][j]) * lbs[i][j], name=name
+                )
+                name = layer.unique_naming_prefix + f"relu_ub_active_{i}_{j}"
+                big_m_ub_active[i][j] = layer.scip_model.addCons(
+                    layer.output[i][j] <= aux_vars[i][j] * ubs[i][j], name=name
+                )
 
-    return cons_with_slack, sos_cons
+    if formulation == "bigm":
+        return [big_m_lb, big_m_ub_inactive, big_m_ub_active]
+    else:
+        return [cons_with_slack, sos_cons]
 
 
 def add_sigmoid_activation_constraint_layer(layer, activation_only=True):
     """
     MIP model for Sigmoid activation on a layer
 
     Parameters
@@ -219,15 +255,17 @@
             tanh_cons[i][j] = layer.scip_model.addCons(
                 layer.output[i][j] == (1 - exp(-2 * x)) / (1 + exp(-2 * x)), name=name
             )
 
     return tanh_cons
 
 
-def propagate_identity_bounds(layer, n_samples, n_nodes_left, n_nodes_right, activation_only):
+def propagate_identity_bounds(
+    layer, n_samples, n_nodes_left, n_nodes_right, activation_only, max_bound
+):
     """
     Activity based bound propagation. Assume the worst case bound for each node individually and generate
     bounds for the next layer.
 
     Parameters
     ----------
     layer : AbstractNNLayer
@@ -236,14 +274,16 @@
         The number of samples passed by the user
     n_nodes_left : int
         The number of nodes on the left (input) layer
     n_nodes_right : int
         The number of nodes on the right (output) layer
     activation_only : bool
         Whether the bounds are going to be used for an activation only layer. In this case no weighted sum is needed.
+    max_bound : float or int
+        The maximum absolute bound value for a variable before bound propagation termination
 
     Returns
     -------
     propagation : bool
         Whether propagation worked
     lbs : np.ndarray
         An array of worst-case scenario lower bounds
@@ -265,27 +305,27 @@
             input_lbs[i][k] = layer.input[i][k].getLbOriginal()
             input_ubs[i][k] = layer.input[i][k].getUbOriginal()
 
     # In the case of activation only we can simply return the input bounds
     if activation_only:
         return True, input_lbs, input_ubs
 
-    # Skip propagation for the weighted sum if some bounds are larger than 10**5
-    if np.max(input_ubs) > 10**5 or np.min(input_lbs) < -1 * 10**5:
+    # Skip propagation for the weighted sum if some bounds are larger than max_bound
+    if np.max(np.abs(input_ubs)) + np.max(np.abs(input_lbs)) > max_bound:
         return False, ubs, lbs
 
     for i in range(n_samples):
         for j in range(n_nodes_right):
             ub = 0
             lb = 0
             for k in range(n_nodes_left):
                 coefficient = layer.coefs[k][j]
                 if coefficient > 0:
-                    ub += input_ubs[i][k] * coefficient
-                    lb += input_lbs[i][k] * coefficient
+                    ub += input_ubs[i][k] * coefficient + 10**-6
+                    lb += input_lbs[i][k] * coefficient - 10**-6
                 elif coefficient < 0:
-                    ub += input_lbs[i][k] * coefficient
-                    lb += input_ubs[i][k] * coefficient
-            ubs[i][j] = ub + layer.intercept[j]
-            lbs[i][j] = lb + layer.intercept[j]
+                    ub += input_lbs[i][k] * coefficient + 10**-6
+                    lb += input_ubs[i][k] * coefficient - 10**-6
+            ubs[i][j] = ub + layer.intercept[j] + 10**-6
+            lbs[i][j] = lb + layer.intercept[j] - 10**-6
 
     return True, lbs, ubs
```

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/neuralnet/layers.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/neuralnet/layers.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,22 +20,78 @@
         input_vars,
         output_vars,
         activation,
         unique_naming_prefix,
         **kwargs,
     ):
         self.activation = activation
+        if "formulation" in kwargs:
+            if kwargs["formulation"] not in ["sos", "bigm"]:
+                formulation = kwargs["formulation"]
+                raise ParameterError(f"Formulation type {formulation} is neither sos nor bigm")
+            self.formulation = kwargs["formulation"]
+        else:
+            self.formulation = "sos"
         AbstractPredictorConstr.__init__(
             self, scip_model, input_vars, output_vars, unique_naming_prefix, **kwargs
         )
 
     def get_error(self, eps=None):
         # We can't compute externally the error of a layer
         raise AssertionError("Cannot compute the error of an individual layer")
 
+    def _layer_mip_model(self, activation_only=True, **kwargs):
+        """Add the layer to model."""
+        if self.activation == "relu":
+            if self.formulation == "sos":
+                slack = create_vars(
+                    self.scip_model,
+                    (self.input.shape[0], self.output.shape[-1]),
+                    vtype="C",
+                    lb=0.0,
+                    ub=None,
+                    name_prefix=self.unique_naming_prefix + "slack",
+                )
+                relu_cons = add_relu_activation_constraint_layer(
+                    self, slack, activation_only=activation_only
+                )
+                self._created_vars.append(slack)
+            else:
+                activation_vars = create_vars(
+                    self.scip_model,
+                    (self.input.shape[0], self.output.shape[-1]),
+                    vtype="B",
+                    lb=0,
+                    ub=1,
+                    name_prefix=self.unique_naming_prefix + "relu_act",
+                )
+                relu_cons = add_relu_activation_constraint_layer(
+                    self, activation_vars, activation_only=activation_only, formulation="bigm"
+                )
+                self._created_vars.append(activation_vars)
+            for cons in relu_cons:
+                self._created_cons.append(cons)
+        elif self.activation == "logistic" or self.activation == "sigmoid":
+            sigmoid_cons = add_sigmoid_activation_constraint_layer(
+                self, activation_only=activation_only
+            )
+            self._created_cons.append(sigmoid_cons)
+        elif self.activation == "tanh":
+            tanh_cons = add_tanh_activation_constraint_layer(self, activation_only=activation_only)
+            self._created_cons.append(tanh_cons)
+        elif self.activation == "identity" and not activation_only:
+            max_bound = self.scip_model.infinity() if self.formulation == "bigm" else 10**5
+            affine_cons = add_identity_activation_constraint_layer(self, max_bound)
+            self._created_vars.append(affine_cons)
+        else:
+            if activation_only:
+                raise ParameterError(f"Activation layer of type {self.activation} shouldn't exist")
+            else:
+                raise ParameterError(f"Dense layer of type {self.activation} shouldn't exist")
+
 
 class ActivationLayer(AbstractNNLayer):
     """Class to build one activation layer of a neural network."""
 
     def __init__(
         self,
         scip_model,
@@ -61,38 +117,15 @@
             lb=None,
             ub=None,
             name_prefix=self.unique_naming_prefix + "output",
         )
         return output_vars
 
     def _mip_model(self, **kwargs):
-        """Add the layer to model."""
-        if self.activation == "relu":
-            slack = create_vars(
-                self.scip_model,
-                (self.input.shape[0], self.output.shape[-1]),
-                vtype="C",
-                lb=0.0,
-                ub=None,
-                name_prefix=self.unique_naming_prefix + "slack",
-            )
-            affine_slack_cons, sos_cons = add_relu_activation_constraint_layer(
-                self, slack, activation_only=True
-            )
-            self._created_vars.append(slack)
-            self._created_cons.append(affine_slack_cons)
-            self._created_cons.append(sos_cons)
-        elif self.activation == "logistic" or self.activation == "sigmoid":
-            sigmoid_cons = add_sigmoid_activation_constraint_layer(self, activation_only=True)
-            self._created_cons.append(sigmoid_cons)
-        elif self.activation == "tanh":
-            tanh_cons = add_tanh_activation_constraint_layer(self, activation_only=True)
-            self._created_cons.append(tanh_cons)
-        else:
-            raise ParameterError(f"Activation layer of type {self.activation} shouldn't exist")
+        self._layer_mip_model(activation_only=True, **kwargs)
 
 
 class DenseLayer(AbstractNNLayer):
     """Class to build one layer of a neural network."""
 
     def __init__(
         self,
@@ -123,34 +156,8 @@
             lb=None,
             ub=None,
             name_prefix=self.unique_naming_prefix + "output",
         )
         return output_vars
 
     def _mip_model(self, **kwargs):
-        """Add the layer to model."""
-        if self.activation == "relu":
-            slack = create_vars(
-                self.scip_model,
-                (self.input.shape[0], self.output.shape[-1]),
-                vtype="C",
-                lb=0.0,
-                ub=None,
-                name_prefix=self.unique_naming_prefix + "slack",
-            )
-            affine_slack_cons, sos_cons = add_relu_activation_constraint_layer(
-                self, slack, activation_only=False
-            )
-            self._created_vars.append(slack)
-            self._created_cons.append(affine_slack_cons)
-            self._created_cons.append(sos_cons)
-        elif self.activation == "logistic" or self.activation == "sigmoid":
-            sigmoid_cons = add_sigmoid_activation_constraint_layer(self, activation_only=False)
-            self._created_cons.append(sigmoid_cons)
-        elif self.activation == "tanh":
-            tanh_cons = add_tanh_activation_constraint_layer(self, activation_only=False)
-            self._created_cons.append(tanh_cons)
-        elif self.activation == "identity":
-            affine_cons = add_identity_activation_constraint_layer(self)
-            self._created_vars.append(affine_cons)
-        else:
-            raise ParameterError(f"Activation layer of type {self.activation} shouldn't exist")
+        self._layer_mip_model(activation_only=False, **kwargs)
```

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/neuralnet/neural_net.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/neuralnet/neural_net.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/modelling/var_utils.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/modelling/var_utils.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/registered_predictors.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/registered_predictors.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/__init__.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/base_regression.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/base_regression.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/centroid_cluster.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/centroid_cluster.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/decision_tree.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/decision_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,18 +147,14 @@
                 self.output_size = 1
             else:
                 self.output_size = predictor.n_classes_
         else:
             self.output_size = predictor.n_outputs_
         SKgetter.__init__(self, predictor, **kwargs)
 
-        formulations = "leafs"
-        if formulation not in formulations:
-            raise ValueError(f"Wrong value for formulation should be one of {formulations}.")
-        self._formulation = formulation
         AbstractPredictorConstr.__init__(
             self, scip_model, input_vars, output_vars, unique_naming_prefix, **kwargs
         )
 
     def _mip_model(self, **kwargs):
         tree = self.predictor.tree_
```

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/gradient_boosting.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/linear_regression.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/linear_regression.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/logistic_regression.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/mlp.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/mlp.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/multi_output.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/multi_output.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/pipeline.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/pls.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/pls.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/preprocessing.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/random_forest.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/random_forest.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/skgetter.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/skgetter.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/sklearn/support_vector.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/sklearn/support_vector.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/torch/sequential.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/torch/sequential.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/xgboost/xgbgetter.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/xgboost/xgbgetter.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/src/pyscipopt_ml/xgboost/xgboost_constr.py` & `pyscipopt_ml-1.1.0/src/pyscipopt_ml/xgboost/xgboost_constr.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/tests/test_adversarial_example.py` & `pyscipopt_ml-1.1.0/tests/test_adversarial_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 
 import numpy as np
-import pytest
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from pyscipopt import Model, quicksum
 from torch.utils.data import DataLoader
 from torchvision import datasets, transforms
 
@@ -34,36 +33,39 @@
 the predictor now misclassifies it. There is a budget on how much the image can be perturbed.
 
 Let I be the x coordinate and J be the y coordinate of the image.
 Let f be the ML predictor that outputs the probability of each label for the input image
 Let image[i][j] be the input image in grey scale with pixel values between 0-1.
 Let x[i][j] the perturbed image in grey scale with pixel values between 0-1.
 Let y be the probability of each label given the ML predictor
-W.l.o.g assume that y[0] is the true label and y[1]is the fake label.
+W.l.o.g assume that y[0] is the true label and y[1] is the fake label.
 
 x[i][j] - image[i][j] <= abs_diff[i][j] for all i, j
 image[i][j] - x[i][j] <= abs_diff[i][j] for all i, j
 \sum_i,j abs_diff[i][j] <= 5
 y = f(x)
 
 max(y[1] - y[0])
 """
 
 
 def build_and_optimise_adversarial_mnist_torch(
-    seed=42,
+    data_seed=42,
+    training_seed=42,
     n_pixel_1d=16,
-    layer_sizes=(40, 20),
-    image_number=10000,
+    layer_size=16,
+    n_layers=2,
     test=True,
+    formulation="sos",
     build_only=False,
 ):
-    assert 0 <= image_number < 30000, f"Image number {image_number} out of range"
-    # Set random seed for reproducibility
-    torch.manual_seed(seed)
+    # Set random seed for reproducibility and select the image that is going to be perturbed
+    data_random_state = np.random.RandomState(data_seed)
+    image_number = data_random_state.randint(low=0, high=30000)
+    torch.manual_seed(training_seed)
 
     # Define transformations for the MNIST dataset
     transform = transforms.Compose(
         [
             transforms.Resize(n_pixel_1d),  # Resize the image
             transforms.ToTensor(),  # Convert images to tensors. This automatically normalises to [0,1]
         ]
@@ -79,22 +81,20 @@
 
     # Create DataLoader for handling batches
     batch_size = 64
     train_dataloader = DataLoader(train_dataset, batch_size=batch_size, shuffle=True)
     test_dataloader = DataLoader(test_dataset, batch_size=batch_size, shuffle=False)
 
     # Create the neural network
-    reg = nn.Sequential(
-        nn.Flatten(),
-        nn.Linear(n_pixel_1d**2, layer_sizes[0]),
-        nn.ReLU(),
-        nn.Linear(layer_sizes[0], layer_sizes[1]),
-        nn.ReLU(),
-        nn.Linear(layer_sizes[1], 10),
-    )
+    layers = [nn.Flatten(), nn.Linear(n_pixel_1d**2, layer_size), nn.ReLU()]
+    for i in range(n_layers - 1):
+        layers.append(nn.Linear(layer_size, layer_size))
+        layers.append(nn.ReLU())
+    layers.append(nn.Linear(layer_size, 10))
+    reg = nn.Sequential(*layers)
 
     # If the model is already saved then skip the training step
     saved_neural_network_path = "./tests/data/adversarial.pt"
     if test and os.path.isfile(saved_neural_network_path):
         reg.load_state_dict(torch.load(saved_neural_network_path))
         reg.eval()
 
@@ -163,14 +163,15 @@
 
     # Create the output variables. (Note that these variables will be automatically constructed if not specified)
     output_vars = np.zeros((10,), dtype=object)
     for i in range(10):
         output_vars[i] = scip.addVar(name=f"y_{i}", vtype="C", lb=None, ub=None)
 
     # Create the difference variables
+    sum_max_diff = data_random_state.uniform(low=4.5, high=5.5)
     abs_diff = np.zeros((n_pixel_1d, n_pixel_1d), dtype=object)
     for i in range(n_pixel_1d):
         for j in range(n_pixel_1d):
             abs_diff[i][j] = scip.addVar(name=f"abs_diff_{i}", vtype="C", lb=0, ub=1)
 
     # Create constraints ensuring only a total certain amount of the picture can change
     for i in range(n_pixel_1d):
@@ -180,23 +181,28 @@
             )
             scip.addCons(
                 abs_diff[i][j] >= -input_vars[0][i][j] + train_dataset[image_number][0][0][i][j]
             )
 
     scip.addCons(
         quicksum(quicksum(abs_diff[i][j] for j in range(n_pixel_1d)) for i in range(n_pixel_1d))
-        <= 5
+        <= sum_max_diff
     )
 
     # Set an objective to maximise the difference between the correct and the wrong label
     scip.setObjective(-output_vars[wrong_label] + output_vars[right_label] + 1)
 
     # Add the ML constraint
     pred_cons = add_predictor_constr(
-        scip, reg, input_vars, output_vars, unique_naming_prefix="adversarial_"
+        scip,
+        reg,
+        input_vars,
+        output_vars,
+        unique_naming_prefix="adversarial_",
+        formulation=formulation,
     )
 
     if not build_only:
         scip.optimize()
 
         # We can check the "error" of the MIP embedding by determining the difference between the Torch and SCIP output
         if np.max(pred_cons.get_error()) > 10**-3:
@@ -204,9 +210,27 @@
             raise AssertionError(f"Max error {error} exceeds threshold of {10**-3}")
 
     return scip
 
 
 def test_mnist_torch():
     scip = build_and_optimise_adversarial_mnist_torch(
-        42, 12, layer_sizes=(10, 10), image_number=10000, test=True
+        data_seed=42,
+        training_seed=42,
+        n_pixel_1d=12,
+        layer_size=10,
+        n_layers=2,
+        test=True,
+        formulation="sos",
+    )
+
+
+def test_mnist_torch_bigm():
+    scip = build_and_optimise_adversarial_mnist_torch(
+        data_seed=42,
+        training_seed=42,
+        n_pixel_1d=12,
+        layer_size=10,
+        n_layers=2,
+        test=True,
+        formulation="bigm",
     )
```

### Comparing `PySCIPOpt-ML-1.0.0/tests/test_airline_satisfcation.py` & `pyscipopt_ml-1.1.0/tests/test_airline_satisfcation.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/tests/test_auto_manufacturer.py` & `pyscipopt_ml-1.1.0/tests/test_auto_manufacturer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from pyscipopt import Model
 from sklearn.ensemble import GradientBoostingRegressor, RandomForestRegressor
+from sklearn.neural_network import MLPRegressor
 from utils import read_csv_to_dict
 
 from src.pyscipopt_ml.add_predictor import add_predictor_constr
 
 """
 In this scenario we take the point of view of an auto manufacturer.
 
@@ -51,24 +52,28 @@
 resale >= c * price
 
 max(amount_sold)
 """
 
 
 def build_and_optimise_auto_manufacturer(
-    seed=0,
-    gbdt_or_rf="gbdt",
-    max_depth=6,
-    n_estimators=6,
-    min_fuel_efficiency=40,
-    min_resale_ratio=0.8,
+    training_seed=42,
+    data_seed=42,
+    gbdt_rf_or_mlp="gbdt",
+    formulation="sos",
+    max_depth_or_layer_size=6,
+    n_estimators_or_layers=6,
     build_only=False,
 ):
+    # Initialise a numpy random state
+    data_random_state = np.random.RandomState(data_seed)
+    training_random_state = np.random.RandomState(training_seed)
+
     # Path to car data
-    data_dict = read_csv_to_dict("./tests/data/Car_sales.csv")
+    data_dict = read_csv_to_dict("./tests/data/car_sales.csv")
 
     # Get an array of the features
     features = [
         "Vehicle_type",
         "Engine_size",
         "Horsepower",
         "Wheelbase",
@@ -95,34 +100,61 @@
         if feature == "Vehicle_type":
             X.append((np.array(data_dict[feature]) == "Passenger").astype(int))
         else:
             X.append(np.array([float(x) for x in data_dict[feature]]))
     X = np.swapaxes(np.array(X), 0, 1)
 
     # Create the prediction models
-    if gbdt_or_rf == "gbdt":
+    if gbdt_rf_or_mlp == "gbdt":
         reg_sales = GradientBoostingRegressor(
-            n_estimators=n_estimators, max_depth=max_depth, random_state=seed
+            n_estimators=n_estimators_or_layers,
+            max_depth=max_depth_or_layer_size,
+            random_state=training_random_state,
         ).fit(np.concatenate((X, price), axis=1), amount_sales.reshape(-1))
         reg_price = GradientBoostingRegressor(
-            n_estimators=n_estimators, max_depth=max_depth, random_state=seed
+            n_estimators=n_estimators_or_layers,
+            max_depth=max_depth_or_layer_size,
+            random_state=training_random_state,
         ).fit(X, price.reshape(-1))
         reg_resale = GradientBoostingRegressor(
-            n_estimators=n_estimators, max_depth=max_depth, random_state=seed
+            n_estimators=n_estimators_or_layers,
+            max_depth=max_depth_or_layer_size,
+            random_state=training_random_state,
         ).fit(np.concatenate((X, price), axis=1), resale_price.reshape(-1))
-    else:
+    elif gbdt_rf_or_mlp == "rf":
         reg_sales = RandomForestRegressor(
-            n_estimators=n_estimators, max_depth=max_depth, random_state=seed
+            n_estimators=n_estimators_or_layers,
+            max_depth=max_depth_or_layer_size,
+            random_state=training_random_state,
         ).fit(np.concatenate((X, price), axis=1), amount_sales.reshape(-1))
         reg_price = RandomForestRegressor(
-            n_estimators=n_estimators, max_depth=max_depth, random_state=seed
+            n_estimators=n_estimators_or_layers,
+            max_depth=max_depth_or_layer_size,
+            random_state=training_random_state,
         ).fit(X, price.reshape(-1))
         reg_resale = RandomForestRegressor(
-            n_estimators=n_estimators, max_depth=max_depth, random_state=seed
+            n_estimators=n_estimators_or_layers,
+            max_depth=max_depth_or_layer_size,
+            random_state=training_random_state,
+        ).fit(np.concatenate((X, price), axis=1), resale_price.reshape(-1))
+    elif gbdt_rf_or_mlp == "mlp":
+        hidden_layer_sizes = tuple(
+            [max_depth_or_layer_size for i in range(n_estimators_or_layers)]
+        )
+        reg_sales = MLPRegressor(
+            random_state=training_random_state, hidden_layer_sizes=hidden_layer_sizes
+        ).fit(np.concatenate((X, price), axis=1), amount_sales.reshape(-1))
+        reg_price = MLPRegressor(
+            random_state=training_random_state, hidden_layer_sizes=hidden_layer_sizes
+        ).fit(X, price.reshape(-1))
+        reg_resale = MLPRegressor(
+            random_state=training_random_state, hidden_layer_sizes=hidden_layer_sizes
         ).fit(np.concatenate((X, price), axis=1), resale_price.reshape(-1))
+    else:
+        raise ValueError(f"Unknown value: {gbdt_rf_or_mlp}")
 
     # Create the SCIP Model
     scip = Model()
 
     # Create variables deciding the features of the manufactured car and the predicted sales information
     feature_vars = np.zeros((1, n_features), dtype=object)
     amount_sold_vars = np.zeros((1, 1), dtype=object)
@@ -165,14 +197,15 @@
             pos_slack[i][j] = scip.addVar(vtype="C", lb=0, ub=big_m, name=f"pos_slack_{i}_{j}")
             neg_slack[i][j] = scip.addVar(vtype="C", lb=0, ub=big_m, name=f"neg_slack_{i}_{j}")
             binary_slack[i][j] = scip.addVar(vtype="B", name=f"bin_slack_{i}_{j}")
 
     # Now add constraints to the model. Our constraints are that the new car is sufficiently different from those
     # already on the market, and that the resale value remains relatively high.
     top_selling_ids = np.argsort(price.reshape(-1))[-n_car_comparisons:]
+    min_diff = data_random_state.uniform(low=2.8, high=3.3)
     for j, car_idx in enumerate(top_selling_ids):
         sum_slack = 0
         for i in range(1, n_features):
             big_m = feature_vars[0][i].getUbOriginal() - feature_vars[0][i].getLbOriginal()
             scip.addCons(
                 pos_slack[i][j] <= big_m * binary_slack[i][j], name=f"bound_pos_slack_{i}_{j}"
             )
@@ -182,65 +215,103 @@
             )
             feature_val = X[car_idx][i]
             scip.addCons(
                 feature_vars[0][i] - feature_val == pos_slack[i][j] - neg_slack[i][j],
                 name=f"l1_diff_{i}_{j}",
             )
             sum_slack += (pos_slack[i][j] + neg_slack[i][j]) / big_m
-        scip.addCons(sum_slack >= 3, name=f"min_diff_{j}")
+        scip.addCons(sum_slack >= min_diff, name=f"min_diff_{j}")
 
     # Now add the ML predictor constraints
     pred_cons = [
         add_predictor_constr(
             scip,
             reg_sales,
             np.concatenate((feature_vars, price_vars), axis=1),
             amount_sold_vars,
             epsilon=0.0001,
+            formulation=formulation,
             unique_naming_prefix="num_sales_",
         ),
         add_predictor_constr(
             scip,
             reg_price,
             feature_vars,
             price_vars,
             epsilon=0.0001,
+            formulation=formulation,
             unique_naming_prefix="price_",
         ),
         add_predictor_constr(
             scip,
             reg_resale,
             np.concatenate((feature_vars, price_vars), axis=1),
             resale_vars,
             epsilon=0.0001,
+            formulation=formulation,
             unique_naming_prefix="resale_",
         ),
     ]
 
     # Add constraints that the resale value of the car must be sufficiently large and that the car is fuel efficient
+    min_resale_ratio = data_random_state.uniform(low=0.70, high=0.75)
+    min_fuel_efficiency = data_random_state.uniform(low=38, high=43)
     scip.addCons(resale_vars[0][0] >= min_resale_ratio * price_vars[0][0], name="min_resale")
     scip.addCons(feature_vars[0][8] >= min_fuel_efficiency, name="fuel_efficient")
 
     scip.setObjective(-amount_sold_vars[0][0] + 10000)
 
     if not build_only:
         # Optimise the SCIP model
         scip.optimize()
-
-        # We can check the "error" of the MIP embedding by determining the difference between the SKLearn and SCIP output
+        # We can check the "error" of the MIP embedding by determining the difference SKLearn and SCIP output
         for predictor_constraint in pred_cons:
             if np.max(predictor_constraint.get_error()) > 10**-4:
                 error = np.max(predictor_constraint.get_error())
                 raise AssertionError(f"Max error {error} exceeds threshold of {10 ** -4}")
 
     return scip
 
 
-def test_auto_manufacturer():
+def test_gbdt_auto_manufacturer():
+    scip = build_and_optimise_auto_manufacturer(
+        training_seed=42,
+        data_seed=42,
+        gbdt_rf_or_mlp="gbdt",
+        max_depth_or_layer_size=5,
+        n_estimators_or_layers=5,
+        build_only=False,
+    )
+
+
+def test_rf_auto_manufacturer():
+    scip = build_and_optimise_auto_manufacturer(
+        training_seed=42,
+        data_seed=42,
+        gbdt_rf_or_mlp="rf",
+        max_depth_or_layer_size=5,
+        n_estimators_or_layers=5,
+        build_only=False,
+    )
+
+
+def test_mlp_auto_manufacturer():
+    scip = build_and_optimise_auto_manufacturer(
+        training_seed=42,
+        data_seed=42,
+        gbdt_rf_or_mlp="mlp",
+        max_depth_or_layer_size=6,
+        n_estimators_or_layers=2,
+        build_only=False,
+    )
+
+
+def test_mlp_auto_manufacturer_bigm():
     scip = build_and_optimise_auto_manufacturer(
-        seed=0,
-        gbdt_or_rf="gbdt",
-        max_depth=6,
-        n_estimators=6,
-        min_fuel_efficiency=40,
-        min_resale_ratio=0.8,
+        training_seed=42,
+        data_seed=42,
+        gbdt_rf_or_mlp="mlp",
+        formulation="bigm",
+        max_depth_or_layer_size=6,
+        n_estimators_or_layers=2,
+        build_only=False,
     )
```

### Comparing `PySCIPOpt-ML-1.0.0/tests/test_city_manager.py` & `pyscipopt_ml-1.1.0/tests/test_city_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 from pyscipopt import Model
+from sklearn.ensemble import GradientBoostingRegressor
+from sklearn.neural_network import MLPRegressor
 from sklearn.tree import DecisionTreeRegressor
 from utils import read_csv_to_dict
 
 from src.pyscipopt_ml.add_predictor import add_predictor_constr
 
 """
 In this scenario we take the point of view of a city manager in Poland.
@@ -60,26 +62,31 @@
 y[i] = f(x[i][:]) for all I
 
 max(sum_i y[i])
 """
 
 
 def build_and_optimise_city_manager(
-    seed=0,
-    max_depth=6,
+    data_seed=42,
+    training_seed=42,
+    dt_gbdt_or_mlp="dt",
+    formulation="sos",
+    max_depth_or_layer_size=6,
+    n_estimators_layers=3,
     n_apartments=50,
     grid_length=5,
     epsilon=0.001,
     build_only=False,
 ):
     # Path to apartment price data
     data_dict = read_csv_to_dict("./tests/data/apartments.csv")
 
     # Set the random seed
-    np.random.seed(seed)
+    data_random_state = np.random.RandomState(data_seed)
+    training_random_state = np.random.RandomState(training_seed)
 
     # The features of our predictor. All distance based features are variables.
     features = [
         "squareMeters",
         "rooms",
         "floorCount",
         "centreDistance",
@@ -104,24 +111,40 @@
         if "has" in feature:
             X.append(np.array([x == "yes" for x in data_dict[feature]]))
         else:
             X.append(np.array([float(x) for x in data_dict[feature]]))
     X = np.swapaxes(np.array(X), 0, 1)
 
     # Train the ML predictor
-    reg = DecisionTreeRegressor(random_state=seed, max_depth=max_depth).fit(X, y)
+    if dt_gbdt_or_mlp == "dt":
+        reg = DecisionTreeRegressor(
+            random_state=training_random_state, max_depth=max_depth_or_layer_size
+        ).fit(X, y)
+    elif dt_gbdt_or_mlp == "gbdt":
+        reg = GradientBoostingRegressor(
+            random_state=training_random_state,
+            max_depth=max_depth_or_layer_size,
+            n_estimators=n_estimators_layers,
+        ).fit(X, y.reshape(-1))
+    elif dt_gbdt_or_mlp == "mlp":
+        hidden_layers = tuple([max_depth_or_layer_size for i in range(n_estimators_layers)])
+        reg = MLPRegressor(
+            random_state=training_random_state, hidden_layer_sizes=hidden_layers
+        ).fit(X, y.reshape(-1))
+    else:
+        raise ValueError(f"Unknown value: {dt_gbdt_or_mlp}")
 
     # Create the SCIP Model
     scip = Model()
 
     # Create variables for the n_apartments many imaginary apartments.The apartments lie on an imaginary square that is
     # defined by the four corners [(0, 0), (0, grid_length), (grid_length, grid_length), (grid_length, 0)]
     feature_vars = np.zeros((n_apartments, n_features), dtype=object)
     price_vars = np.zeros((n_apartments, 1), dtype=object)
-    apartment_locations = np.random.uniform(0, grid_length, size=(n_apartments, 2))
+    apartment_locations = data_random_state.uniform(0, grid_length, size=(n_apartments, 2))
     rooms = np.random.randint(
         np.min(X[feature_to_idx["rooms"]]),
         np.max(X[feature_to_idx["rooms"]]) + 1,
         size=n_apartments,
     )
     floors = np.random.randint(
         np.min(X[feature_to_idx["floorCount"]]),
@@ -150,35 +173,40 @@
         ("restaurant", "restaurantDistance", restaurant_vars),
         ("college", "collegeDistance", college_vars),
         ("pharmacy", "pharmacyDistance", pharmacy_vars),
     ]
 
     # Now fill in the actual variables
     for i in range(n_apartments):
-        price_vars[i][0] = scip.addVar(vtype="C", lb=0, name=f"price_{i}")
+        price_vars[i][0] = scip.addVar(vtype="C", lb=0, ub=50, name=f"price_{i}")
         for j, feature in enumerate(features):
             feature_vars[i][j] = scip.addVar(vtype="C", lb=0, name=f"feature_{i}_{j}")
             # Randomly generate characteristics
             if "has" in feature:
                 scip.fixVar(feature_vars[i][j], int(np.random.randint(0, 2)))
             elif feature == "rooms":
                 scip.fixVar(feature_vars[i][j], int(rooms[i]))
-            elif feature == "floors":
+            elif feature == "floorCount":
                 scip.fixVar(feature_vars[i][j], int(floors[i]))
             elif feature == "squareMeters":
                 scip.fixVar(feature_vars[i][j], int(square_meters[i]))
             elif feature == "centreDistance":
                 scip.fixVar(
                     feature_vars[i][j],
                     np.sum(
                         np.abs(
                             apartment_locations[i] - np.array([grid_length / 2, grid_length / 2])
                         )
                     ),
                 )
+            elif feature == "squareMeters":
+                scip.chgVarUb(feature_vars[i][j], 200)
+            else:
+                scip.chgVarUb(feature_vars[i][j], 2 * grid_length)
+
     for building_type, _, building_var in building_vars:
         for i in range(building_var.shape[0]):
             building_var[i][0] = scip.addVar(
                 vtype="C", lb=0, ub=grid_length, name=f"{building_type}_{i}_0"
             )
             building_var[i][1] = scip.addVar(
                 vtype="C", lb=0, ub=grid_length, name=f"{building_type}_{i}_1"
@@ -315,40 +343,87 @@
                 )
                 scip.addCons(
                     feature_vars[i][feature_idx] >= dist_builds[1] - big_m * aux_max_var_bin,
                     name=f"dist_{i}_{building_type}_3",
                 )
 
     # Embed the ML predictors for each apartment. A small epsilon ensures we match sklearn
-    predictor_constraints = []
-    for i in range(n_apartments):
-        predictor_constraints.append(
-            add_predictor_constr(
-                scip,
-                reg,
-                feature_vars[i],
-                price_vars[i],
-                epsilon=epsilon,
-                unique_naming_prefix=f"predictor_{i}_",
-            )
-        )
+    pred_cons = add_predictor_constr(
+        scip,
+        reg,
+        feature_vars,
+        price_vars,
+        epsilon=epsilon,
+        formulation=formulation,
+        unique_naming_prefix=f"predictor_",
+    )
 
     # Add the objective to the MIP
     scip.setObjective(-np.sum(price_vars) + (20 * n_apartments))
 
     if not build_only:
         # Optimise the SCIP model
         scip.optimize()
-
-        # We can check the "error" of the MIP embedding by determining the difference between the SKLearn and SCIP output
-        for pred_cons in predictor_constraints:
-            if np.max(pred_cons.get_error()) > 10**-4:
-                error = np.max(pred_cons.get_error())
-                raise AssertionError(f"Max error {error} exceeds threshold of {10 ** -4}")
+        # We can check the "error" of the MIP embedding by determining the difference SKLearn and SCIP output
+        if np.max(pred_cons.get_error()) > 10**-4:
+            error = np.max(pred_cons.get_error())
+            raise AssertionError(f"Max error {error} exceeds threshold of {10 ** -4}")
 
     return scip
 
 
-def test_city_manager():
-    scip = build_and_optimise_city_manager(
-        seed=0, max_depth=6, n_apartments=50, grid_length=5, epsilon=0.001
+def test_dt_city_manager():
+    build_and_optimise_city_manager(
+        data_seed=42,
+        training_seed=42,
+        dt_gbdt_or_mlp="dt",
+        max_depth_or_layer_size=6,
+        n_estimators_layers=3,
+        n_apartments=50,
+        grid_length=5,
+        epsilon=0.001,
+        build_only=False,
+    )
+
+
+def test_gbdt_city_manager():
+    build_and_optimise_city_manager(
+        data_seed=50,
+        training_seed=80,
+        dt_gbdt_or_mlp="gbdt",
+        max_depth_or_layer_size=4,
+        n_estimators_layers=3,
+        n_apartments=50,
+        grid_length=5,
+        epsilon=0.001,
+        build_only=False,
+    )
+
+
+def test_mlp_city_manager():
+    build_and_optimise_city_manager(
+        data_seed=50,
+        training_seed=80,
+        dt_gbdt_or_mlp="mlp",
+        formulation="sos",
+        max_depth_or_layer_size=3,
+        n_estimators_layers=2,
+        n_apartments=3,
+        grid_length=5,
+        epsilon=0.001,
+        build_only=False,
+    )
+
+
+def test_mlp_bigm_city_manager():
+    build_and_optimise_city_manager(
+        data_seed=50,
+        training_seed=80,
+        dt_gbdt_or_mlp="mlp",
+        formulation="bigm",
+        max_depth_or_layer_size=3,
+        n_estimators_layers=2,
+        n_apartments=3,
+        grid_length=5,
+        epsilon=0.001,
+        build_only=False,
     )
```

### Comparing `PySCIPOpt-ML-1.0.0/tests/test_input_types.py` & `pyscipopt_ml-1.1.0/tests/test_input_types.py`

 * *Files identical despite different names*

### Comparing `PySCIPOpt-ML-1.0.0/tests/test_simple_function_approximation.py` & `pyscipopt_ml-1.1.0/tests/test_simple_function_approximation.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,90 +23,91 @@
   volume={131},
   pages={106580},
   year={2019},
   publisher={Elsevier}
 }
 
 Let there be two random quadratic functions:
-xQ_1x + A_1x + c_1
-xQ_2x + A_2x + c_2
+xQ_1x + a_1x + c_1
+xQ_2x + a_2x + c_2
 
 Let f be a NN that approximates the first quadratic function, and g be a NN
 that approximates the second quadratic function.
 Let const be some constant value in the range of the randomly generated quadratic function
 
 The MIP model is:
 
 g(x) = const
 min(f(x))
 """
 
 
 def build_and_optimise_function_approximation_model(
-    seed=42,
     n_inputs=5,
     n_samples=1000,
     framework="sklearn",
-    layers_sizes=(20, 20, 10),
+    formulation="sos",
+    layer_size=8,
+    training_seed=42,
+    data_seed=42,
     build_only=False,
 ):
-    assert len(layers_sizes) == 3
-
     X, y_1, y_2 = build_random_quadratic_functions(
-        seed=seed, n_inputs=n_inputs, n_samples=n_samples
+        seed=data_seed, n_inputs=n_inputs, n_samples=n_samples
     )
 
     if framework == "sklearn":
+        hidden_layer_sizes = tuple([layer_size for i in range(3)])
         reg_1 = MLPRegressor(
-            random_state=seed,
-            hidden_layer_sizes=(layers_sizes[0], layers_sizes[1], layers_sizes[2]),
+            random_state=training_seed,
+            hidden_layer_sizes=hidden_layer_sizes,
         ).fit(X, y_1.reshape(-1))
         reg_2 = MLPRegressor(
-            random_state=seed,
-            hidden_layer_sizes=(layers_sizes[0], layers_sizes[1], layers_sizes[2]),
+            random_state=training_seed,
+            hidden_layer_sizes=hidden_layer_sizes,
         ).fit(X, y_2.reshape(-1))
     elif framework == "keras":
-        keras.utils.set_random_seed(seed)
+        keras.utils.set_random_seed(training_seed)
         reg_1 = keras.Sequential()
         reg_1.add(keras.Input(shape=(n_inputs,)))
-        reg_1.add(keras.layers.Dense(layers_sizes[0], activation="linear"))
+        reg_1.add(keras.layers.Dense(layer_size, activation="linear"))
         reg_1.add(keras.layers.Activation(keras.activations.relu))
-        reg_1.add(keras.layers.Dense(layers_sizes[1], activation="sigmoid"))
-        reg_1.add(keras.layers.Dense(layers_sizes[2], activation="relu"))
+        reg_1.add(keras.layers.Dense(layer_size, activation="sigmoid"))
+        reg_1.add(keras.layers.Dense(layer_size, activation="relu"))
         reg_1.add(keras.layers.Dense(1, activation="linear"))
         reg_1.compile(optimizer="adam", loss="mse")
-        reg_1.fit(X, y_1, batch_size=32, epochs=50)
+        reg_1.fit(X, y_1, batch_size=32, epochs=200)
         reg_2 = keras.Sequential()
         reg_2.add(keras.Input(shape=(n_inputs,)))
-        reg_2.add(keras.layers.Dense(layers_sizes[0], activation="linear"))
+        reg_2.add(keras.layers.Dense(layer_size, activation="linear"))
         reg_2.add(keras.layers.Activation(keras.activations.sigmoid))
-        reg_2.add(keras.layers.Dense(layers_sizes[1], activation="tanh"))
-        reg_2.add(keras.layers.Dense(layers_sizes[2], activation="relu"))
+        reg_2.add(keras.layers.Dense(layer_size, activation="tanh"))
+        reg_2.add(keras.layers.Dense(layer_size, activation="relu"))
         reg_2.add(keras.layers.Dense(1, activation="linear"))
         reg_2.compile(optimizer="adam", loss="mse")
         reg_2.fit(X, y_2, batch_size=32, epochs=200)
     elif framework == "torch":
-        torch.random.manual_seed(seed)
+        torch.random.manual_seed(training_seed)
         reg_1 = nn.Sequential(
-            nn.Linear(n_inputs, layers_sizes[0]),
+            nn.Linear(n_inputs, layer_size),
             nn.ReLU(),
-            nn.Linear(layers_sizes[0], layers_sizes[1]),
+            nn.Linear(layer_size, layer_size),
             nn.ReLU(),
-            nn.Linear(layers_sizes[1], layers_sizes[2]),
+            nn.Linear(layer_size, layer_size),
             nn.ReLU(),
-            nn.Linear(layers_sizes[2], 1),
+            nn.Linear(layer_size, 1),
         )
         reg_2 = nn.Sequential(
-            nn.Linear(n_inputs, layers_sizes[0]),
+            nn.Linear(n_inputs, layer_size),
             nn.ReLU(),
-            nn.Linear(layers_sizes[0], layers_sizes[1]),
+            nn.Linear(layer_size, layer_size),
             nn.ReLU(),
-            nn.Linear(layers_sizes[1], layers_sizes[2]),
+            nn.Linear(layer_size, layer_size),
             nn.ReLU(),
-            nn.Linear(layers_sizes[2], 1),
+            nn.Linear(layer_size, 1),
         )
 
         # Convert data into PyTorch tensors
         X_tensor = torch.tensor(X, dtype=torch.float32)
         y_1_tensor = torch.tensor(y_1, dtype=torch.float32)
         y_2_tensor = torch.tensor(y_2, dtype=torch.float32)
 
@@ -148,18 +149,28 @@
                 optimizer_2.step()
     else:
         raise ValueError(f"Framework {framework} is unknown")
 
     # Now build the SCIP Model and embed the neural networks
     scip, input_vars, output_vars = build_basic_scip_model(n_inputs)
     mlp_cons_1 = add_predictor_constr(
-        scip, reg_1, input_vars[0], output_vars[0], unique_naming_prefix="reg_1_"
+        scip,
+        reg_1,
+        input_vars,
+        output_vars[0],
+        unique_naming_prefix="reg_1_",
+        formulation=formulation,
     )
     mlp_cons_2 = add_predictor_constr(
-        scip, reg_2, input_vars[1], output_vars[1], unique_naming_prefix="reg_2_"
+        scip,
+        reg_2,
+        input_vars,
+        output_vars[1],
+        unique_naming_prefix="reg_2_",
+        formulation=formulation,
     )
 
     if not build_only:
         # Optimize the model
         scip.optimize()
 
         # We can check the "error" of the MIP embedding via the difference between SKLearn / Torch and SCIP output
@@ -204,21 +215,20 @@
 
 
 def build_basic_scip_model(n_inputs):
     # Initialise a SCIP Model
     scip = Model()
 
     # Create the input variables
-    input_vars = np.zeros((2, n_inputs), dtype=object)
-    for i in range(2):
-        for j in range(n_inputs):
-            # Tight bounds are important for MIP formulations of neural networks. They often drastically improve
-            # performance. As our training data is in the range [-10, 10], we pass that as bounds [-10, 10].
-            # These bounds will then propagate to other variables.
-            input_vars[i][j] = scip.addVar(name=f"x_{i}_{j}", vtype="C", lb=-10, ub=10)
+    input_vars = np.zeros((1, n_inputs), dtype=object)
+    for i in range(n_inputs):
+        # Tight bounds are important for MIP formulations of neural networks. They often drastically improve
+        # performance. As our training data is in the range [-10, 10], we pass that as bounds [-10, 10].
+        # These bounds will then propagate to other variables.
+        input_vars[0][i] = scip.addVar(name=f"x_{i}", vtype="C", lb=-10, ub=10)
 
     # Create the output variables. (Note that these variables will be automatically constructed if not specified)
     output_vars = np.zeros((2, 1), dtype=object)
     for i in range(2):
         output_vars[i] = scip.addVar(name=f"y_{i}", vtype="C", lb=None, ub=None)
 
     # Now set additional constraints and set the objective
@@ -226,21 +236,75 @@
     scip.setObjective(output_vars[0][0] + 10000)
 
     return scip, input_vars, output_vars
 
 
 def test_sklearn_mlp_regression():
     scip = build_and_optimise_function_approximation_model(
-        seed=42, n_inputs=5, n_samples=1000, framework="sklearn", layers_sizes=(20, 20, 10)
+        data_seed=42,
+        training_seed=42,
+        n_inputs=5,
+        n_samples=1000,
+        framework="sklearn",
+        formulation="sos",
+        layer_size=8,
+    )
+
+
+def test_sklearn_mlp_regression_bigm():
+    scip = build_and_optimise_function_approximation_model(
+        data_seed=42,
+        training_seed=42,
+        n_inputs=5,
+        n_samples=1000,
+        framework="sklearn",
+        formulation="bigm",
+        layer_size=8,
     )
 
 
 def test_torch_sequential_regression():
     scip = build_and_optimise_function_approximation_model(
-        seed=42, n_inputs=5, n_samples=1000, framework="torch", layers_sizes=(20, 20, 10)
+        data_seed=42,
+        training_seed=42,
+        n_inputs=5,
+        n_samples=1000,
+        framework="torch",
+        formulation="sos",
+        layer_size=8,
+    )
+
+
+def test_torch_sequential_regression_bigm():
+    scip = build_and_optimise_function_approximation_model(
+        data_seed=42,
+        training_seed=42,
+        n_inputs=5,
+        n_samples=1000,
+        framework="torch",
+        formulation="bigm",
+        layer_size=8,
     )
 
 
 def test_keras_sequential_regression():
     scip = build_and_optimise_function_approximation_model(
-        seed=42, n_inputs=5, n_samples=1000, framework="keras", layers_sizes=(10, 10, 10)
+        data_seed=42,
+        training_seed=42,
+        n_inputs=5,
+        n_samples=1000,
+        framework="keras",
+        formulation="sos",
+        layer_size=3,
+    )
+
+
+def test_keras_sequential_regression_bigm():
+    scip = build_and_optimise_function_approximation_model(
+        data_seed=42,
+        training_seed=42,
+        n_inputs=5,
+        n_samples=1000,
+        framework="keras",
+        formulation="bigm",
+        layer_size=3,
     )
```

### Comparing `PySCIPOpt-ML-1.0.0/tests/test_tree_planting.py` & `pyscipopt_ml-1.1.0/tests/test_tree_planting.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 from pyscipopt import Model, quicksum
+from sklearn.ensemble import GradientBoostingRegressor
 from sklearn.linear_model import LinearRegression
+from sklearn.neural_network import MLPRegressor
 from sklearn.tree import DecisionTreeRegressor
 from utils import read_csv_to_dict
 
 from src.pyscipopt_ml.add_predictor import add_predictor_constr
 
 """
 In this scenario we take the point of view of an agency tasked with replanting a stretch of land.
@@ -42,39 +44,45 @@
 Let costs[t] be the cost of planting tree t, and budget be the total budget
 Let sterilisation_budget be the amount of grid points that be sterilised
 Let f be the ML predictor for the survival of tree t at grid point i,j with soil feature x[i][j]
 
 The MIP model is:
 
 sum_t p[i][j][t] = 1 for all i,j
-sum_{i,j} s[i][j][t] >= min_survive[t] forall t
+sum_{i,j} s'[i][j][t] >= min_survive[t] forall t
 sum_t (sum_{i,j} p[i][j][t] * cost[t]) <= budget
 sum_{i,j} x[i][j][sterilisation_idx] <= sterilisation_budget
 s[i][j][t] = f(x[i][j][:])
 p[i][j][t] = 1 => s'[i][j][t] <= s[i][j][t] forall i,j,t
-p[i][j][t] = 0 => x'[i][j][t] <= 0
+p[i][j][t] = 0 => s'[i][j][t] <= 0
 
 max(sum_{i,j,t} s'[i][j][t])
 """
 
 
 def build_and_optimise_tree_planting(
-    seed=42,
+    data_seed=42,
+    training_seed=42,
     predictor_type="linear",
+    formulation="sos",
     max_depth=5,
+    n_estimators_layers=2,
+    layer_size=8,
     n_grid_size=10,
-    min_trees=(2, 2, 2, 2),
-    max_sterilise=10,
-    costs=(25, 30, 40, 50),
-    max_budget=3350,
+    min_trees=(1.7, 1.7, 1.7, 1.7),
     build_only=False,
 ):
-    assert predictor_type in ("linear", "decision_tree")
+    assert predictor_type in ("linear", "decision_tree", "gbdt", "mlp")
+    training_random_state = np.random.RandomState(training_seed)
+    data_random_state = np.random.RandomState(data_seed)
+    max_sterilise = data_random_state.randint(low=8, high=13)
+    costs = data_random_state.uniform(low=25, high=45, size=4)
+    max_budget = (n_grid_size**2) * np.median(costs) * 1.1
     # Read the csv data
-    data_dict = read_csv_to_dict("./tests/data/Tree_Data.csv")
+    data_dict = read_csv_to_dict("./tests/data/tree_survivability.csv")
 
     # Extract the min and max light values
     light_values = np.array(
         [float(data_dict["Light_ISF"][i]) for i in range(len(data_dict["Light_ISF"]))]
     )
     min_light = np.min(light_values)
     max_light = np.max(light_values)
@@ -106,16 +114,31 @@
     # Create and train the regression model
     regression_models = []
     for i in range(len(species)):
         X_i = np.array(X[i])
         y_i = np.array(y[i])
         if predictor_type == "linear":
             reg = LinearRegression().fit(X_i, y_i)
+        elif predictor_type == "decision_tree":
+            reg = DecisionTreeRegressor(
+                random_state=training_random_state, max_depth=max_depth
+            ).fit(X_i, y_i)
+        elif predictor_type == "gbdt":
+            reg = GradientBoostingRegressor(
+                random_state=training_random_state,
+                n_estimators=n_estimators_layers,
+                max_depth=max_depth,
+            ).fit(X_i, y_i.reshape(-1))
+        elif predictor_type == "mlp":
+            hidden_layers = tuple([layer_size for i in range(n_estimators_layers)])
+            reg = MLPRegressor(
+                random_state=training_random_state, hidden_layer_sizes=hidden_layers
+            ).fit(X_i, y_i.reshape(-1))
         else:
-            reg = DecisionTreeRegressor(random_state=seed, max_depth=max_depth).fit(X_i, y_i)
+            raise ValueError(f"Unknown predictor type: {predictor_type}")
         regression_models.append(reg)
 
     # Initialise the SCIP Model
     scip = Model()
 
     # Create variables deciding which tree is planted in which grid point and the survival rate of each planted tree
     tree_planting_vars = np.zeros((n_grid_size, n_grid_size, 4), dtype=object)
@@ -124,33 +147,33 @@
     for i in range(n_grid_size):
         for j in range(n_grid_size):
             for k in range(4):
                 tree_planting_vars[i][j][k] = scip.addVar(
                     vtype="B", name=f"plant_tree_{i}_{j}_{k}"
                 )
                 tree_survive_vars[i][j][k] = scip.addVar(
-                    vtype="C", ub=1, name=f"survive_tree_{i}_{j}_{k}"
+                    vtype="C", lb=-10, ub=10, name=f"survive_tree_{i}_{j}_{k}"
                 )
                 tree_adjusted_survive_vars[i][j][k] = scip.addVar(
-                    vtype="C", ub=1, name=f"adjusted_survive_tree_{i}_{j}_{k}"
+                    vtype="C", lb=-1, ub=1, name=f"adjusted_survive_tree_{i}_{j}_{k}"
                 )
 
     # Ensure that only a single tree is planted in a single grid point
     for i in range(n_grid_size):
         for j in range(n_grid_size):
             scip.addCons(
                 quicksum(tree_planting_vars[i][j][k] for k in range(4)) == 1,
                 name=f"square_{i}_{j}",
             )
 
     # Ensure an expected minimum amount of each tree type survives
     for k in range(4):
         scip.addCons(
             quicksum(
-                quicksum(tree_survive_vars[i][j][k] for j in range(n_grid_size))
+                quicksum(tree_adjusted_survive_vars[i][j][k] for j in range(n_grid_size))
                 for i in range(n_grid_size)
             )
             >= min_trees[k],
             name=f"min_trees_{k}",
         )
 
     # Ensure that the budget is respected, and not more trees are planted than can be afforded
@@ -175,32 +198,29 @@
                     tree_planting_vars[i][j][k],
                     name=f"tree_survive_ind_{i}_{j}_{k}_0",
                 )
                 scip.addConsIndicator(
                     tree_adjusted_survive_vars[i][j][k] <= 0,
                     tree_planting_vars[i][j][k],
                     activeone=False,
-                    name=f"tree_survive_ind_{i}_{j}_{k}_1",
+                    name=f"tree_survive_ind_{i}_{j}_{k}_2",
                 )
 
-    # Randomly generate the grid characteristics
-    np.random.seed(seed)
-
     # Create feature variables
     feature_variables = np.zeros((n_grid_size, n_grid_size, 7), dtype=object)
     for i in range(n_grid_size):
         light_isf = max_light - ((i / n_grid_size) * (max_light - min_light))
         for j in range(n_grid_size):
-            light_cat = np.random.randint(0, 3)
-            myco = np.random.randint(0, 2)
-            soil_myco = np.random.randint(0, 2)
+            light_cat = data_random_state.randint(0, 3)
+            myco = data_random_state.randint(0, 2)
+            soil_myco = data_random_state.randint(0, 2)
             for k in range(7):
                 if k == 0:
                     feature_variables[i][j][k] = scip.addVar(
-                        vtype="C", lb=0, ub=1, name=f"feature_{i}_{j}_{k}"
+                        vtype="C", lb=min_light, ub=max_light, name=f"feature_{i}_{j}_{k}"
                     )
                     scip.fixVar(feature_variables[i][j][k], light_isf)
                 else:
                     feature_variables[i][j][k] = scip.addVar(
                         vtype="B", name=f"feature_{i}_{j}_{k}"
                     )
                     if (
@@ -232,14 +252,16 @@
         pred_cons_list.append(
             add_predictor_constr(
                 scip,
                 regression_models[i],
                 feature_variables.reshape(-1, 7),
                 tree_survive_vars[:, :, i].reshape(-1, 1),
                 unique_naming_prefix=f"predictor_{i}_",
+                epsilon=0.0001,
+                formulation=formulation,
             )
         )
 
     # Set the objective to maximise amount of trees that survive
     scip.setObjective(
         -quicksum(
             quicksum(
@@ -262,28 +284,69 @@
                 raise AssertionError(f"Max error {error} exceeds threshold of {10 ** -5}")
 
     return scip
 
 
 def test_tree_planting_linear():
     scip = build_and_optimise_tree_planting(
-        seed=42,
+        data_seed=42,
+        training_seed=42,
         predictor_type="linear",
+        max_depth=5,
+        n_estimators_layers=2,
+        layer_size=8,
         n_grid_size=10,
         min_trees=(2, 2, 2, 2),
-        max_sterilise=10,
-        costs=(25, 30, 40, 50),
-        max_budget=3350,
     )
 
 
 def test_tree_planting_decision_tree():
     scip = build_and_optimise_tree_planting(
-        seed=42,
+        data_seed=42,
+        training_seed=42,
         predictor_type="decision_tree",
         max_depth=5,
+        n_estimators_layers=2,
+        layer_size=8,
+        n_grid_size=10,
+        min_trees=(2, 2, 2, 2),
+    )
+
+
+def test_tree_planing_gbdt():
+    scip = build_and_optimise_tree_planting(
+        data_seed=18,
+        training_seed=35,
+        predictor_type="gbdt",
+        max_depth=5,
+        n_estimators_layers=8,
+        layer_size=8,
         n_grid_size=10,
         min_trees=(2, 2, 2, 2),
-        max_sterilise=10,
-        costs=(25, 30, 40, 50),
-        max_budget=3350,
+    )
+
+
+def test_tree_planting_mlp():
+    scip = build_and_optimise_tree_planting(
+        data_seed=18,
+        training_seed=35,
+        predictor_type="mlp",
+        max_depth=5,
+        n_estimators_layers=2,
+        layer_size=6,
+        n_grid_size=3,
+        min_trees=(0.5, 0.5, 0.5, 0.5),
+    )
+
+
+def test_tree_planting_mlp_bigm():
+    scip = build_and_optimise_tree_planting(
+        data_seed=18,
+        training_seed=35,
+        predictor_type="mlp",
+        formulation="bigm",
+        max_depth=5,
+        n_estimators_layers=2,
+        layer_size=6,
+        n_grid_size=3,
+        min_trees=(0.5, 0.5, 0.5, 0.5),
     )
```

### Comparing `PySCIPOpt-ML-1.0.0/tests/test_wine_manufacturer.py` & `pyscipopt_ml-1.1.0/tests/test_wine_manufacturer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import pdb
-
 import numpy as np
 from lightgbm import LGBMRegressor
 from pyscipopt import Model, quicksum
 from sklearn.ensemble import GradientBoostingRegressor, RandomForestRegressor
+from sklearn.neural_network import MLPRegressor
 from utils import read_csv_to_dict
 from xgboost import XGBRegressor, XGBRFRegressor
 
 from src.pyscipopt_ml.add_predictor import add_predictor_constr
 
 """
 In this scenario we take the point of view of a wine manufacturer.
@@ -58,30 +57,34 @@
 sum_{i,k} m[i][k] * costs[k] <= budget
 
 max(sum_i y[i])
 """
 
 
 def build_and_optimise_wine_manufacturer(
-    seed=42,
+    data_seed=42,
+    training_seed=42,
     n_vineyards=35,
     n_wines_to_produce=5,
-    min_wine_quality=4.25,
     sklearn_xgboost_lightgbm="sklearn",
-    gbdt_or_rf="rf",
-    n_estimators=3,
+    gbdt_rf_or_mlp="rf",
+    formulation="sos",
+    n_estimators_layers=3,
     max_depth=3,
+    layer_size=16,
     epsilon=0.0001,
     build_only=False,
 ):
     assert sklearn_xgboost_lightgbm in ("sklearn", "xgboost", "lightgbm")
-    assert gbdt_or_rf in ("gbdt", "rf")
+    assert gbdt_rf_or_mlp in ("gbdt", "rf", "mlp")
+    data_random_state = np.random.RandomState(data_seed)
+    training_random_state = np.random.RandomState(training_seed)
 
     # Path to red wine data
-    data_dict = read_csv_to_dict("./tests/data/wineQualityReds.csv")
+    data_dict = read_csv_to_dict("./tests/data/red_wine_quality.csv")
 
     features = [
         "fixed.acidity",
         "volatile.acidity",
         "citric.acid",
         "residual.sugar",
         "chlorides",
@@ -101,53 +104,67 @@
         -1,
     )
     for feature in features:
         X.append(np.array([float(x) for x in data_dict[feature]]))
     X = np.swapaxes(np.array(X), 0, 1)
 
     # Train the ML predictor
-    if sklearn_xgboost_lightgbm == "sklearn":
-        if gbdt_or_rf == "rf":
+    if gbdt_rf_or_mlp == "mlp":
+        hidden_layers = tuple([layer_size for i in range(n_estimators_layers)])
+        reg = MLPRegressor(
+            random_state=training_random_state, hidden_layer_sizes=hidden_layers
+        ).fit(X, quality)
+    elif sklearn_xgboost_lightgbm == "sklearn":
+        if gbdt_rf_or_mlp == "rf":
             reg = RandomForestRegressor(
-                random_state=seed, n_estimators=n_estimators, max_depth=max_depth
+                random_state=training_random_state,
+                n_estimators=n_estimators_layers,
+                max_depth=max_depth,
             ).fit(X, quality)
         else:
             reg = GradientBoostingRegressor(
-                random_state=seed, n_estimators=n_estimators, max_depth=max_depth
+                random_state=training_random_state,
+                n_estimators=n_estimators_layers,
+                max_depth=max_depth,
             ).fit(X, quality)
     elif sklearn_xgboost_lightgbm == "xgboost":
-        if gbdt_or_rf == "gbdt":
+        if gbdt_rf_or_mlp == "gbdt":
             reg = XGBRegressor(
-                random_state=seed, n_estimators=n_estimators, max_depth=max_depth
+                random_state=training_random_state,
+                n_estimators=n_estimators_layers,
+                max_depth=max_depth,
             ).fit(X, quality)
         else:
             reg = XGBRFRegressor(
-                random_state=seed, n_estimators=n_estimators, max_depth=max_depth
+                random_state=training_random_state,
+                n_estimators=n_estimators_layers,
+                max_depth=max_depth,
             ).fit(X, quality)
     else:
-        if gbdt_or_rf == "gbdt":
+        if gbdt_rf_or_mlp == "gbdt":
             reg = LGBMRegressor(
-                random_state=seed, n_estimators=n_estimators, max_depth=max_depth
+                random_state=training_random_state,
+                n_estimators=n_estimators_layers,
+                max_depth=max_depth,
             ).fit(X, quality)
         else:
             reg = LGBMRegressor(
-                random_state=seed,
-                n_estimators=n_estimators,
+                random_state=training_random_state,
+                n_estimators=n_estimators_layers,
                 max_depth=max_depth,
                 boosting_type="rf",
                 bagging_freq=1,
                 bagging_fraction=0.5,
             ).fit(X, quality)
 
     # Create artificial data from some vineyards
-    np.random.seed(seed)
     vineyard_order = np.arange(X.shape[0])
-    np.random.shuffle(vineyard_order)
-    vineyard_litre_limits = np.random.uniform(0.25, 0.35, n_vineyards)
-    vineyard_costs = np.random.uniform(1, 2, n_vineyards)
+    data_random_state.shuffle(vineyard_order)
+    vineyard_litre_limits = data_random_state.uniform(0.25, 0.35, n_vineyards)
+    vineyard_costs = data_random_state.uniform(1, 2, n_vineyards)
     vineyard_features = []
     low_quality_vineyards_i = 0
     for i in vineyard_order:
         if low_quality_vineyards_i >= n_vineyards:
             break
         if quality[i] <= 5:
             low_quality_vineyards_i += 1
@@ -205,18 +222,25 @@
         )
         <= budget,
         name=f"budget_cons",
     )
 
     # Add the ML constraint. Add in a single batch!
     pred_cons = add_predictor_constr(
-        scip, reg, feature_vars, quality_vars, unique_naming_prefix="predictor_", epsilon=epsilon
+        scip,
+        reg,
+        feature_vars,
+        quality_vars,
+        unique_naming_prefix="predictor_",
+        epsilon=epsilon,
+        formulation=formulation,
     )
 
     # Add a constraint ensuring minimum wine quality on those produced
+    min_wine_quality = data_random_state.uniform(4.2, 4.5)
     for i in range(n_wines_to_produce):
         scip.addCons(quality_vars[i][0] >= min_wine_quality, name=f"min_quality_{i}")
 
     # Set the SCIP objective
     scip.setObjective(
         quicksum(-quality_vars[i][0] for i in range(n_wines_to_produce)) / n_wines_to_produce + 10
     )
@@ -231,81 +255,110 @@
             raise AssertionError(f"Max error {error} exceeds threshold of {10 ** -3}")
 
     return scip
 
 
 def test_wine_manufacturer_sk_rf():
     scip = build_and_optimise_wine_manufacturer(
-        seed=42,
+        data_seed=42,
+        training_seed=42,
         n_vineyards=35,
         n_wines_to_produce=5,
-        min_wine_quality=4.25,
         sklearn_xgboost_lightgbm="sklearn",
-        gbdt_or_rf="rf",
-        n_estimators=3,
+        gbdt_rf_or_mlp="rf",
         max_depth=3,
+        n_estimators_layers=3,
     )
 
 
 def test_wine_manufacturer_sk_gbdt():
     scip = build_and_optimise_wine_manufacturer(
-        seed=42,
+        data_seed=42,
+        training_seed=42,
         n_vineyards=35,
         n_wines_to_produce=5,
-        min_wine_quality=4.25,
         sklearn_xgboost_lightgbm="sklearn",
-        gbdt_or_rf="gbdt",
-        n_estimators=3,
+        gbdt_rf_or_mlp="gbdt",
         max_depth=3,
+        n_estimators_layers=3,
     )
 
 
 def test_wine_manufacturer_xgb_rf():
     scip = build_and_optimise_wine_manufacturer(
-        seed=42,
+        data_seed=21,
+        training_seed=21,
         n_vineyards=35,
         n_wines_to_produce=5,
-        min_wine_quality=4.25,
         sklearn_xgboost_lightgbm="xgboost",
-        gbdt_or_rf="rf",
-        n_estimators=3,
+        gbdt_rf_or_mlp="rf",
         max_depth=3,
+        n_estimators_layers=3,
     )
 
 
 def test_wine_manufacturer_xgb_gbdt():
     scip = build_and_optimise_wine_manufacturer(
-        seed=42,
+        data_seed=21,
+        training_seed=21,
         n_vineyards=35,
         n_wines_to_produce=5,
-        min_wine_quality=4.25,
         sklearn_xgboost_lightgbm="xgboost",
-        gbdt_or_rf="gbdt",
-        n_estimators=3,
+        gbdt_rf_or_mlp="gbdt",
         max_depth=3,
+        n_estimators_layers=3,
     )
 
 
 def test_wine_manufacturer_lgb_rf():
     scip = build_and_optimise_wine_manufacturer(
-        seed=42,
+        data_seed=18,
+        training_seed=18,
         n_vineyards=35,
         n_wines_to_produce=5,
-        min_wine_quality=4.25,
         sklearn_xgboost_lightgbm="lightgbm",
-        gbdt_or_rf="rf",
-        n_estimators=3,
+        gbdt_rf_or_mlp="rf",
         max_depth=3,
+        n_estimators_layers=3,
     )
 
 
 def test_wine_manufacturer_lgb_gbdt():
     scip = build_and_optimise_wine_manufacturer(
-        seed=42,
+        data_seed=18,
+        training_seed=18,
         n_vineyards=35,
         n_wines_to_produce=5,
-        min_wine_quality=4.25,
         sklearn_xgboost_lightgbm="lightgbm",
-        gbdt_or_rf="gbdt",
-        n_estimators=3,
+        gbdt_rf_or_mlp="gbdt",
+        max_depth=3,
+        n_estimators_layers=3,
+    )
+
+
+def test_wine_manufacturer_sklearn_mlp():
+    scip = build_and_optimise_wine_manufacturer(
+        data_seed=18,
+        training_seed=18,
+        n_vineyards=35,
+        n_wines_to_produce=5,
+        sklearn_xgboost_lightgbm="sklearn",
+        gbdt_rf_or_mlp="mlp",
+        max_depth=3,
+        n_estimators_layers=3,
+        layer_size=7,
+    )
+
+
+def test_wine_manufacturer_sklearn_mlp_bigm():
+    scip = build_and_optimise_wine_manufacturer(
+        data_seed=18,
+        training_seed=18,
+        n_vineyards=35,
+        n_wines_to_produce=5,
+        sklearn_xgboost_lightgbm="sklearn",
+        gbdt_rf_or_mlp="mlp",
+        formulation="bigm",
         max_depth=3,
+        n_estimators_layers=3,
+        layer_size=7,
     )
```

