# Comparing `tmp/scCellFie-0.1.7.tar.gz` & `tmp/sccellfie-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scCellFie-0.1.7.tar", last modified: Fri Apr  5 09:05:17 2024, max compression
+gzip compressed data, was "sccellfie-0.1.8.tar", last modified: Thu Apr 25 11:04:44 2024, max compression
```

## Comparing `scCellFie-0.1.7.tar` & `sccellfie-0.1.8.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.843825 scCellFie-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-05 09:05:08.000000 scCellFie-0.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-05 09:05:17.843825 scCellFie-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-05 09:05:08.000000 scCellFie-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.843825 scCellFie-0.1.7/scCellFie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-05 09:05:17.000000 scCellFie-0.1.7/scCellFie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-05 09:05:17.000000 scCellFie-0.1.7/scCellFie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:05:17.000000 scCellFie-0.1.7/scCellFie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 09:05:17.000000 scCellFie-0.1.7/scCellFie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 09:05:17.000000 scCellFie-0.1.7/scCellFie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.835825 scCellFie-0.1.7/sccellfie/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.835825 scCellFie-0.1.7/sccellfie/expression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.835825 scCellFie-0.1.7/sccellfie/expression/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/tests/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/tests/test_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/expression/thresholds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.835825 scCellFie-0.1.7/sccellfie/external/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.835825 scCellFie-0.1.7/sccellfie/external/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/external/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/external/tests/test_tf_idf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/external/tf_idf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/gene_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/io/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/save_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/io/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/tests/test_load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/io/tests/test_save_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/metabolic_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/preprocessing/prepare_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/preprocessing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/preprocessing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/preprocessing/tests/test_prepare_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/reaction_activity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/spatial/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/assortativity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/hotspots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/knn_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.839825 scCellFie-0.1.7/sccellfie/spatial/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/tests/test_assortativity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/tests/test_hotspots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/spatial/tests/test_knn_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.843825 scCellFie-0.1.7/sccellfie/stats/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/stats/markers_from_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.843825 scCellFie-0.1.7/sccellfie/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/stats/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/stats/tests/test_markers_from_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:17.843825 scCellFie-0.1.7/sccellfie/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/tests/test_gene_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/tests/test_metabolic_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/tests/test_reaction_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-05 09:05:08.000000 scCellFie-0.1.7/sccellfie/tests/toy_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 09:05:17.843825 scCellFie-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 09:05:08.000000 scCellFie-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.363158 sccellfie-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-25 11:04:37.000000 sccellfie-0.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-25 11:04:44.363158 sccellfie-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-25 11:04:37.000000 sccellfie-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.363158 sccellfie-0.1.8/scCellFie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-25 11:04:44.000000 sccellfie-0.1.8/scCellFie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-25 11:04:44.000000 sccellfie-0.1.8/scCellFie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:04:44.000000 sccellfie-0.1.8/scCellFie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-25 11:04:44.000000 sccellfie-0.1.8/scCellFie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 11:04:44.000000 sccellfie-0.1.8/scCellFie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.355157 sccellfie-0.1.8/sccellfie/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.355157 sccellfie-0.1.8/sccellfie/expression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/expression/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/expression/smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.355157 sccellfie-0.1.8/sccellfie/expression/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/expression/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/expression/tests/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/expression/tests/test_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18717 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/expression/tests/test_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/expression/thresholds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.355157 sccellfie-0.1.8/sccellfie/external/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.355157 sccellfie-0.1.8/sccellfie/external/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/external/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/external/tests/test_tf_idf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/external/tf_idf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/gene_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.359158 sccellfie-0.1.8/sccellfie/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/io/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/io/save_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.359158 sccellfie-0.1.8/sccellfie/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/io/tests/test_load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/io/tests/test_save_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/metabolic_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.359158 sccellfie-0.1.8/sccellfie/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/preprocessing/prepare_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.359158 sccellfie-0.1.8/sccellfie/preprocessing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/preprocessing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/preprocessing/tests/test_prepare_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/reaction_activity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.359158 sccellfie-0.1.8/sccellfie/spatial/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/spatial/assortativity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/spatial/hotspots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/spatial/knn_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.359158 sccellfie-0.1.8/sccellfie/spatial/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/spatial/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/spatial/tests/test_assortativity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/spatial/tests/test_hotspots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/spatial/tests/test_knn_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.359158 sccellfie-0.1.8/sccellfie/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/stats/markers_from_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.359158 sccellfie-0.1.8/sccellfie/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/stats/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/stats/tests/test_markers_from_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:44.363158 sccellfie-0.1.8/sccellfie/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/tests/test_gene_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/tests/test_metabolic_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/tests/test_reaction_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-25 11:04:37.000000 sccellfie-0.1.8/sccellfie/tests/toy_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 11:04:44.363158 sccellfie-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-25 11:04:37.000000 sccellfie-0.1.8/setup.py
```

### Comparing `scCellFie-0.1.7/LICENSE.txt` & `sccellfie-0.1.8/LICENSE.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023, scCellFie development team.
+Copyright (c) 2024, Wellcome Sanger Institute.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `scCellFie-0.1.7/PKG-INFO` & `sccellfie-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCellFie
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool for studying metabolic tasks from single-cell and spatial transcriptomics
 Home-page: https://github.com/earmingol/scCellFie
 Author: Erick Armingol
 Author-email: erickarmingol@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,14 +35,15 @@
 ## About scCellFie
 Single-cell CellFie is a Python implementation of [CellFie](https://github.com/LewisLabUCSD/CellFie), a tool for studying metabolic tasks 
 originally developed in MATLAB by the [Lewis Lab](https://lewislab.ucsd.edu/). This version is designed to be 
 compatible with single-cell and spatial data analysis using Scanpy.
 
 
 <img src="https://github.com/earmingol/scCellFie/blob/main/scCellFie-Logo.png?raw=true" width="350" height="350" alt="Logo" style="margin-right: 10px;">
+<p style="font-size:10px;">This image was created with the assistance of DALL·E</p>
 
 ## Installation
 To install scCellFie, use pip:
 
 `pip install sccellfie`
 
 ## Features
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scCellFie-0.1.7/README.md` & `sccellfie-0.1.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ## About scCellFie
 Single-cell CellFie is a Python implementation of [CellFie](https://github.com/LewisLabUCSD/CellFie), a tool for studying metabolic tasks 
 originally developed in MATLAB by the [Lewis Lab](https://lewislab.ucsd.edu/). This version is designed to be 
 compatible with single-cell and spatial data analysis using Scanpy.
 
 
 <img src="https://github.com/earmingol/scCellFie/blob/main/scCellFie-Logo.png?raw=true" width="350" height="350" alt="Logo" style="margin-right: 10px;">
+<p style="font-size:10px;">This image was created with the assistance of DALL·E</p>
 
 ## Installation
 To install scCellFie, use pip:
 
 `pip install sccellfie`
 
 ## Features
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scCellFie-0.1.7/scCellFie.egg-info/PKG-INFO` & `sccellfie-0.1.8/scCellFie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCellFie
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool for studying metabolic tasks from single-cell and spatial transcriptomics
 Home-page: https://github.com/earmingol/scCellFie
 Author: Erick Armingol
 Author-email: erickarmingol@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,14 +35,15 @@
 ## About scCellFie
 Single-cell CellFie is a Python implementation of [CellFie](https://github.com/LewisLabUCSD/CellFie), a tool for studying metabolic tasks 
 originally developed in MATLAB by the [Lewis Lab](https://lewislab.ucsd.edu/). This version is designed to be 
 compatible with single-cell and spatial data analysis using Scanpy.
 
 
 <img src="https://github.com/earmingol/scCellFie/blob/main/scCellFie-Logo.png?raw=true" width="350" height="350" alt="Logo" style="margin-right: 10px;">
+<p style="font-size:10px;">This image was created with the assistance of DALL·E</p>
 
 ## Installation
 To install scCellFie, use pip:
 
 `pip install sccellfie`
 
 ## Features
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scCellFie-0.1.7/scCellFie.egg-info/SOURCES.txt` & `sccellfie-0.1.8/scCellFie.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 scCellFie.egg-info/top_level.txt
 sccellfie/__init__.py
 sccellfie/gene_score.py
 sccellfie/metabolic_task.py
 sccellfie/reaction_activity.py
 sccellfie/expression/__init__.py
 sccellfie/expression/aggregation.py
+sccellfie/expression/smoothing.py
 sccellfie/expression/thresholds.py
 sccellfie/expression/tests/__init__.py
 sccellfie/expression/tests/test_aggregation.py
+sccellfie/expression/tests/test_smoothing.py
 sccellfie/expression/tests/test_threshold.py
 sccellfie/external/__init__.py
 sccellfie/external/tf_idf.py
 sccellfie/external/tests/__init__.py
 sccellfie/external/tests/test_tf_idf.py
 sccellfie/io/__init__.py
 sccellfie/io/load_data.py
```

### Comparing `scCellFie-0.1.7/sccellfie/expression/aggregation.py` & `sccellfie-0.1.8/sccellfie/expression/aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,11 +89,11 @@
         agg_expression[group] = AGG_FUNC[agg_func](group_data, axis=0)
 
     return agg_expression.transpose()
 
 
 AGG_FUNC = {'mean' : np.nanmean,
             'median' : np.nanmedian,
-            '25p' : lambda x, axis: np.percentile(x, q=25, axis=axis),
-            '75p' : lambda x, axis: np.percentile(x, q=75, axis=axis),
-            'trimean' : lambda x, axis: 0.5*np.percentile(x, q=50, axis=axis) + 0.25*(np.percentile(x, q=25, axis=axis) + np.percentile(x, q=75, axis=axis))
+            '25p' : lambda x, axis: np.nanpercentile(x, q=25, axis=axis),
+            '75p' : lambda x, axis: np.nanpercentile(x, q=75, axis=axis),
+            'trimean' : lambda x, axis: 0.5*np.nanpercentile(x, q=50, axis=axis) + 0.25*(np.nanpercentile(x, q=25, axis=axis) + np.nanpercentile(x, q=75, axis=axis))
             }
```

### Comparing `scCellFie-0.1.7/sccellfie/expression/tests/test_aggregation.py` & `sccellfie-0.1.8/sccellfie/expression/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/expression/tests/test_threshold.py` & `sccellfie-0.1.8/sccellfie/expression/tests/test_threshold.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 import pandas as pd
 
 from pandas.testing import assert_frame_equal
-from sccellfie.expression.thresholds import get_local_mean_threshold, get_global_mean_threshold, get_global_percentile_threshold, get_local_percentile_threshold, set_manual_threshold
+from sccellfie.expression.thresholds import get_local_mean_threshold, get_global_mean_threshold, get_local_percentile_threshold, get_global_percentile_threshold, get_local_trimean_threshold, get_global_trimean_threshold, set_manual_threshold
 from sccellfie.tests.toy_inputs import create_controlled_adata
 
 
 @pytest.mark.parametrize("use_raw, lower_bound, upper_bound, exclude_zeros",
                          [(False, 1e-5, None, False),
                           (True, 1e-5, None, False),
                           (False, 10, None, False),
@@ -241,14 +241,126 @@
     columns = ['threshold-{}'.format(p) for p in percentile]
 
     # Test output structure
     assert all(col in local_thresholds.columns for col in columns), "Missing columns"
     assert all(col in global_thresholds.columns for col in columns), "Missing columns"
 
 
+@pytest.mark.parametrize("use_raw, lower_bound, upper_bound, exclude_zeros",
+                         [(False, 1e-5, None, False),
+                          (True, 1e-5, None, False),
+                          (False, 10, None, False),
+                          (False, 1e-5, 4, False),
+                          (False, 1e-5, None, True),
+                          (False, pd.DataFrame({f'threshold-trimean': [10, 8, 12]}, index=['gene1', 'gene2', 'gene3'], dtype=float), None, False),
+                          (False, 1e-5, pd.DataFrame({f'threshold-trimean': [1, 2, 3]}, index=['gene1', 'gene2', 'gene3'], dtype=float), False),
+                         ])
+def test_get_local_trimean_threshold(use_raw, lower_bound, upper_bound, exclude_zeros):
+    # Create a small, controlled AnnData object
+    adata = create_controlled_adata()
+
+    # Run the function
+    thresholds = get_local_trimean_threshold(adata,
+                                             use_raw=use_raw,
+                                             lower_bound=lower_bound,
+                                             upper_bound=upper_bound,
+                                             exclude_zeros=exclude_zeros)
+
+    # Expected values
+    expected_values = pd.DataFrame({'threshold-trimean': [4., 5., 4.25]},
+                                   index=['gene1', 'gene2', 'gene3'],
+                                   dtype=float)
+
+    if exclude_zeros:
+        expected_values.loc['gene3', 'threshold-trimean'] = 6.0
+
+    if lower_bound is not None:
+        if isinstance(lower_bound, (int, float, complex)):
+            expected_values[expected_values < lower_bound] = lower_bound
+        else:
+            lb = lower_bound.copy()
+            expected_values[expected_values < lb] = lb[expected_values < lb]
+
+    if upper_bound is not None:
+        if isinstance(upper_bound, (int, float, complex)):
+            expected_values[expected_values > upper_bound] = upper_bound
+        else:
+            ub = upper_bound.copy()
+            expected_values[expected_values > ub] = ub[expected_values > ub]
+
+    # Test output structure
+    assert isinstance(thresholds, pd.DataFrame)
+    assert 'threshold-trimean' in thresholds.columns
+    assert thresholds.shape == expected_values.shape
+
+    # Test correctness of values
+    assert_frame_equal(thresholds, expected_values, check_exact=False), "Threshold values do not match expected results"
+    if lower_bound is not None:
+        assert (thresholds >= lower_bound).all().all(), "Lower bound not respected"
+    if upper_bound is not None:
+        assert (thresholds <= upper_bound).all().all(), "Upper bound not respected"
+
+
+@pytest.mark.parametrize("use_raw, lower_bound, upper_bound, exclude_zeros",
+                         [(False, 1e-5, None, False),
+                          (True, 1e-5, None, False),
+                          (False, 10, None, False),
+                          (False, 1e-5, 4, False),
+                          (False, 1e-5, None, True),
+                          (False, pd.DataFrame({f'threshold-trimean': [10, 8, 12]}, index=['gene1', 'gene2', 'gene3'], dtype=float), None, False),
+                          (False, 1e-5, pd.DataFrame({f'threshold-trimean': [1, 2, 3]}, index=['gene1', 'gene2', 'gene3'], dtype=float), False),
+                         ])
+def test_get_global_trimean_threshold(use_raw, lower_bound, upper_bound, exclude_zeros):
+    # Create a small, controlled AnnData object
+    adata = create_controlled_adata()
+
+    # Run the function
+    thresholds = get_global_trimean_threshold(adata,
+                                              use_raw=use_raw,
+                                              lower_bound=lower_bound,
+                                              upper_bound=upper_bound,
+                                              exclude_zeros=exclude_zeros)
+
+    # Expected values
+    expected_values = pd.DataFrame({'threshold-trimean': [4.375, 4.375, 4.375]},
+                                   index=['gene1', 'gene2', 'gene3'],
+                                   dtype=float)
+
+    if exclude_zeros:
+        expected_values = pd.DataFrame({'threshold-trimean': [4.75, 4.75, 4.75]},
+                                       index=['gene1', 'gene2', 'gene3'],
+                                       dtype=float)
+
+    if lower_bound is not None:
+        if isinstance(lower_bound, (int, float, complex)):
+            expected_values[expected_values < lower_bound] = lower_bound
+        else:
+            lb = lower_bound.copy()
+            expected_values[expected_values < lb] = lb[expected_values < lb]
+
+    if upper_bound is not None:
+        if isinstance(upper_bound, (int, float, complex)):
+            expected_values[expected_values > upper_bound] = upper_bound
+        else:
+            ub = upper_bound.copy()
+            expected_values[expected_values > ub] = ub[expected_values > ub]
+
+    # Test output structure
+    assert isinstance(thresholds, pd.DataFrame)
+    assert 'threshold-trimean' in thresholds.columns
+    assert thresholds.shape == expected_values.shape
+
+    # Test correctness of values
+    assert_frame_equal(thresholds, expected_values, check_exact=False), "Threshold values do not match expected results"
+    if lower_bound is not None:
+        assert (thresholds >= lower_bound).all().all(), "Lower bound not respected"
+    if upper_bound is not None:
+        assert (thresholds <= upper_bound).all().all(), "Upper bound not respected"
+
+
 def test_set_manual_threshold():
     # Create a small, controlled AnnData object
     adata = create_controlled_adata()
 
     # Run the function
     thresholds = set_manual_threshold(adata, threshold=5)
```

### Comparing `scCellFie-0.1.7/sccellfie/expression/thresholds.py` & `sccellfie-0.1.8/sccellfie/expression/thresholds.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,18 +34,16 @@
         A pandas.DataFrame object with the local percentile threshold for each gene.
     '''
     if use_raw:
         X = adata.raw.X.toarray()
     else:
         X = adata.X.toarray()
     if exclude_zeros:
-        X = np.ma.masked_equal(X, 0)
-        thresholds = np.quantile(X, q=percentile, axis=0, method='midpoint').data
-    else:
-        thresholds = np.quantile(X, q=percentile, axis=0, method='midpoint')
+        X = np.where(X==0, np.nan, X)
+    thresholds = np.nanquantile(X, q=percentile, axis=0, method='midpoint')
     if isinstance(percentile, list):
         columns = ['threshold-{}'.format(p) for p in percentile]
     else:
         columns = ['threshold-{}'.format(percentile)]
     thresholds = pd.DataFrame(thresholds.T, index=adata.var_names, columns=columns, dtype=float)
 
     if lower_bound is not None:
@@ -98,18 +96,16 @@
         A pandas.DataFrame object with the global percentile threshold for each gene.
     '''
     if use_raw:
         X = adata.raw.X.toarray()
     else:
         X = adata.X.toarray()
     if exclude_zeros:
-        X = np.ma.masked_equal(X, 0)
-        thresholds = np.quantile(X, q=percentile, method='midpoint')
-    else:
-        thresholds = np.quantile(X, q=percentile, method='midpoint')
+        X = np.where(X == 0, np.nan, X)
+    thresholds = np.nanquantile(X, q=percentile, method='midpoint')
     if isinstance(percentile, list):
         columns = ['threshold-{}'.format(p) for p in percentile]
         thresholds = pd.DataFrame({col: [thresholds[i]]*adata.shape[1] for i, col in enumerate(columns)})
     else:
         columns = ['threshold-{}'.format(percentile)]
         thresholds = pd.DataFrame(thresholds.T, index=adata.var_names, columns=columns, dtype=float)
 
@@ -160,18 +156,16 @@
         A pandas.DataFrame object with the local mean threshold for each gene.
     '''
     if use_raw:
         X = adata.raw.X.toarray()
     else:
         X = adata.X.toarray()
     if exclude_zeros:
-        X = np.ma.masked_equal(X, 0)
-        thresholds = np.ma.mean(X, axis=0).data
-    else:
-        thresholds = np.nanmean(X, axis=0)
+        X = np.where(X==0, np.nan, X)
+    thresholds = np.nanmean(X, axis=0)
     columns = ['threshold-mean']
     thresholds = pd.DataFrame(thresholds, index=adata.var_names, columns=columns, dtype=float)
 
     if lower_bound is not None:
         if type(lower_bound) not in (int, float, complex):
             lb = lower_bound.copy()
             lb.columns = columns
@@ -216,26 +210,146 @@
         A pandas.DataFrame object with the global mean threshold for each gene.
     '''
     if use_raw:
         X = adata.raw.X.toarray()
     else:
         X = adata.X.toarray()
     if exclude_zeros:
-        X = np.ma.masked_equal(X, 0)
-        thresholds = np.ma.mean(X)
-    else:
-        thresholds = np.nanmean(X)
+        X = np.where(X == 0, np.nan, X)
+    thresholds = np.nanmean(X)
     columns = ['threshold-mean']
     thresholds = pd.DataFrame(thresholds, index=adata.var_names, columns=columns, dtype=float)
 
     if lower_bound is not None:
         if type(lower_bound) not in (int, float, complex):
             lb = lower_bound.copy()
             lb.columns = columns
             thresholds[thresholds < lb] = lb[thresholds < lb]
+        else:
+            thresholds[thresholds < lower_bound] = lower_bound
+
+    if upper_bound is not None:
+        if type(upper_bound) not in (int, float, complex):
+            ub = upper_bound.copy()
+            ub.columns = columns
+            thresholds[thresholds > ub] = ub[thresholds > ub]
+        else:
+            thresholds[thresholds > upper_bound] = upper_bound
+    return thresholds
+
+
+def get_local_trimean_threshold(adata, lower_bound=1e-5, upper_bound=None, exclude_zeros=False, use_raw=False):
+    '''
+    Obtains the local Tukey's trimean threshold for each gene in a AnnData object.
+
+    Parameters
+    ----------
+    adata: AnnData object
+        Annotated data matrix.
+
+    lower_bound: float or pandas.DataFrame, optional (default: 1e-5)
+        Lower bound for the threshold. If a pandas.DataFrame is provided, it must have the same number of genes
+        as the adata object.
+
+    upper_bound: float or pandas.DataFrame, optional (default: None)
+        Upper bound for the threshold. If a pandas.DataFrame is provided, it must have the same number of genes
+        as the adata object.
+
+    exclude_zeros: bool, optional (default: False)
+        Whether to exclude zeros when computing the threshold.
+
+    use_raw: bool, optional (default: False)
+        Whether to use the raw data stored in adata.raw.X.
+
+    Returns
+    -------
+    thresholds: pandas.DataFrame
+        A pandas.DataFrame object with the local Tukey's trimean threshold for each gene.
+    '''
+    if use_raw:
+        X = adata.raw.X.toarray()
+    else:
+        X = adata.X.toarray()
+
+    if exclude_zeros:
+        X = np.where(X == 0, np.nan, X)
+    q1 = np.nanquantile(X, q=0.25, axis=0, method='midpoint')
+    median = np.nanquantile(X, q=0.5, axis=0, method='midpoint')
+    q3 = np.nanquantile(X, q=0.75, axis=0, method='midpoint')
+    thresholds = (q1 + 2 * median + q3) / 4
+
+    columns = ['threshold-trimean']
+    thresholds = pd.DataFrame(thresholds.T, index=adata.var_names, columns=columns, dtype=float)
+
+    if lower_bound is not None:
+        if type(lower_bound) not in (int, float, complex):
+            lb = lower_bound.copy()
+            lb.columns = columns
+            thresholds[thresholds < lb] = lb[thresholds < lb]
+        else:
+            thresholds[thresholds < lower_bound] = lower_bound
+
+    if upper_bound is not None:
+        if type(upper_bound) not in (int, float, complex):
+            ub = upper_bound.copy()
+            ub.columns = columns
+            thresholds[thresholds > ub] = ub[thresholds > ub]
+        else:
+            thresholds[thresholds > upper_bound] = upper_bound
+    return thresholds
+
+
+def get_global_trimean_threshold(adata, lower_bound=1e-5, upper_bound=None, exclude_zeros=False, use_raw=False):
+    '''
+    Obtains the global Tukey's trimean threshold for each gene in a AnnData object.
+
+    Parameters
+    ----------
+    adata: AnnData object
+        Annotated data matrix.
+
+    lower_bound: float or pandas.DataFrame, optional (default: 1e-5)
+        Lower bound for the threshold. If a pandas.DataFrame is provided, it must have the same number of genes
+        as the adata object.
+
+    upper_bound: float or pandas.DataFrame, optional (default: None)
+        Upper bound for the threshold. If a pandas.DataFrame is provided, it must have the same number of genes
+        as the adata object.
+
+    exclude_zeros: bool, optional (default: False)
+        Whether to exclude zeros when computing the threshold.
+
+    use_raw: bool, optional (default: False)
+        Whether to use the raw data stored in adata.raw.X.
+
+    Returns
+    -------
+    thresholds: pandas.DataFrame
+        A pandas.DataFrame object with the global Tukey's trimean threshold for each gene.
+    '''
+    if use_raw:
+        X = adata.raw.X.toarray()
+    else:
+        X = adata.X.toarray()
+
+    if exclude_zeros:
+        X = np.where(X == 0, np.nan, X)
+    q1 = np.nanquantile(X, q=0.25, method='midpoint')
+    median = np.nanquantile(X, q=0.5, method='midpoint')
+    q3 = np.nanquantile(X, q=0.75, method='midpoint')
+    thresholds = (q1 + 2 * median + q3) / 4
+
+    columns = ['threshold-trimean']
+    thresholds = pd.DataFrame(thresholds, index=adata.var_names, columns=columns, dtype=float)
+
+    if lower_bound is not None:
+        if type(lower_bound) not in (int, float, complex):
+            lb = lower_bound.copy()
+            lb.columns = columns
+            thresholds[thresholds < lb] = lb[thresholds < lb]
         else:
             thresholds[thresholds < lower_bound] = lower_bound
 
     if upper_bound is not None:
         if type(upper_bound) not in (int, float, complex):
             ub = upper_bound.copy()
             ub.columns = columns
```

### Comparing `scCellFie-0.1.7/sccellfie/external/tests/test_tf_idf.py` & `sccellfie-0.1.8/sccellfie/external/tests/test_tf_idf.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/external/tf_idf.py` & `sccellfie-0.1.8/sccellfie/external/tf_idf.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/gene_score.py` & `sccellfie-0.1.8/sccellfie/gene_score.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/io/load_data.py` & `sccellfie-0.1.8/sccellfie/io/load_data.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/io/save_data.py` & `sccellfie-0.1.8/sccellfie/io/save_data.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/io/tests/test_load_data.py` & `sccellfie-0.1.8/sccellfie/io/tests/test_load_data.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/io/tests/test_save_data.py` & `sccellfie-0.1.8/sccellfie/io/tests/test_save_data.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/metabolic_task.py` & `sccellfie-0.1.8/sccellfie/metabolic_task.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/preprocessing/prepare_inputs.py` & `sccellfie-0.1.8/sccellfie/preprocessing/prepare_inputs.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/preprocessing/tests/test_prepare_inputs.py` & `sccellfie-0.1.8/sccellfie/preprocessing/tests/test_prepare_inputs.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/reaction_activity.py` & `sccellfie-0.1.8/sccellfie/reaction_activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     gene_scores = adata.layers[layer]
     rxns = gpr_dict.keys()
     ral = np.zeros((gene_scores.shape[0], len(rxns)))
 
     # This could be optimized by paralellization, returning multiple vectors (one per cell)
     # And concatenating them later.
     rxn_max_genes = []
-    for i in tqdm(range(gene_scores.shape[0]), disable=disable_pbar, desc='Cell Rxn Activities', leave=False): # Iterate through single cells
+    for i in tqdm(range(gene_scores.shape[0]), disable=disable_pbar, desc='Cell Rxn Activities', leave=True): # Iterate through single cells
         max_gene_vector = []
         scores = defaultdict(float)
         scores.update({name: value for name, value in zip(genes, gene_scores[i, :])})
 
         # For accounting for specificity
         selected_gene = defaultdict(float)
         rxn_ids_gene = defaultdict(list)
```

### Comparing `scCellFie-0.1.7/sccellfie/spatial/assortativity.py` & `sccellfie-0.1.8/sccellfie/spatial/assortativity.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/spatial/hotspots.py` & `sccellfie-0.1.8/sccellfie/spatial/hotspots.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/spatial/knn_network.py` & `sccellfie-0.1.8/sccellfie/spatial/knn_network.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/spatial/tests/test_assortativity.py` & `sccellfie-0.1.8/sccellfie/spatial/tests/test_assortativity.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/spatial/tests/test_hotspots.py` & `sccellfie-0.1.8/sccellfie/spatial/tests/test_hotspots.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/spatial/tests/test_knn_network.py` & `sccellfie-0.1.8/sccellfie/spatial/tests/test_knn_network.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/stats/markers_from_task.py` & `sccellfie-0.1.8/sccellfie/stats/markers_from_task.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/stats/tests/test_markers_from_task.py` & `sccellfie-0.1.8/sccellfie/stats/tests/test_markers_from_task.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/tests/test_gene_score.py` & `sccellfie-0.1.8/sccellfie/tests/test_gene_score.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/tests/test_metabolic_task.py` & `sccellfie-0.1.8/sccellfie/tests/test_metabolic_task.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/tests/test_reaction_activity.py` & `sccellfie-0.1.8/sccellfie/tests/test_reaction_activity.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/sccellfie/tests/toy_inputs.py` & `sccellfie-0.1.8/sccellfie/tests/toy_inputs.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.7/setup.py` & `sccellfie-0.1.8/setup.py`

 * *Files identical despite different names*

