# Comparing `tmp/fedot_ind-0.4.1.2.tar.gz` & `tmp/fedot_ind-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedot_ind-0.4.1.2.tar", last modified: Thu Mar  7 12:51:47 2024, max compression
+gzip compressed data, was "fedot_ind-0.4.2.tar", max compression
```

## Comparing `fedot_ind-0.4.1.2.tar` & `fedot_ind-0.4.2.tar`

### file list

```diff
@@ -1,210 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.321554 fedot_ind-0.4.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-07 12:51:36.000000 fedot_ind-0.4.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-07 12:51:36.000000 fedot_ind-0.4.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-03-07 12:51:47.321554 fedot_ind-0.4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-03-07 12:51:36.000000 fedot_ind-0.4.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.293554 fedot_ind-0.4.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:36.000000 fedot_ind-0.4.1.2/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.293554 fedot_ind-0.4.1.2/fedot_ind/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.293554 fedot_ind-0.4.1.2/fedot_ind/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22849 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.293554 fedot_ind-0.4.1.2/fedot_ind/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/api/utils/checkers_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/api/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/api/utils/metafeatures.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/api/utils/path_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/api/utils/recurrent_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/api/utils/saver_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.293554 fedot_ind-0.4.1.2/fedot_ind/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.293554 fedot_ind-0.4.1.2/fedot_ind/core/architecture/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.297554 fedot_ind-0.4.1.2/fedot_ind/core/architecture/abstraction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/abstraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/abstraction/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/abstraction/сheckers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.297554 fedot_ind-0.4.1.2/fedot_ind/core/architecture/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/pipelines/abstract_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/pipelines/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/pipelines/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.297554 fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/optimisation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/results_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    32241 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/ucr_datasets.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.297554 fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/visualisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/visualisation/gradcam_vis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.297554 fedot_ind-0.4.1.2/fedot_ind/core/architecture/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22580 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/preprocessing/data_convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.297554 fedot_ind-0.4.1.2/fedot_ind/core/architecture/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/settings/computational.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/architecture/settings/pipeline_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.297554 fedot_ind-0.4.1.2/fedot_ind/core/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/ensemble/base_ensembler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/ensemble/kernel_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/ensemble/random_automl_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/ensemble/rank_ensembler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.301554 fedot_ind-0.4.1.2/fedot_ind/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/metrics/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.301554 fedot_ind-0.4.1.2/fedot_ind/core/metrics/loss/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/metrics/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/metrics/loss/basis_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/metrics/loss/soft_dtw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/metrics/loss/svd_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/metrics/metrics_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.301554 fedot_ind-0.4.1.2/fedot_ind/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.301554 fedot_ind-0.4.1.2/fedot_ind/core/models/automl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/automl/fedot_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/base_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.301554 fedot_ind-0.4.1.2/fedot_ind/core/models/detection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.301554 fedot_ind-0.4.1.2/fedot_ind/core/models/detection/probalistic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/detection/probalistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19099 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/detection/probalistic/kalman.py
--rw-r--r--   0 runner    (1001) docker     (127)    17521 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/detection/probalistic/sigma.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.301554 fedot_ind-0.4.1.2/fedot_ind/core/models/detection/subspaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/detection/subspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/detection/subspaces/func_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/detection/subspaces/sst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.301554 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.305554 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/base_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11125 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/explainable_convolution_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/inception.py
--rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/mini_rocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/omni_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)    18479 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/patch_tst.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/tst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.305554 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/activation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.305554 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/attention_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/conv_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12460 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/head_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/linear_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/padding_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/pooling_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16816 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/special.py
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/other.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.305554 fedot_ind-0.4.1.2/fedot_ind/core/models/quantile/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/quantile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/quantile/quantile_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/quantile/stat_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.309554 fedot_ind-0.4.1.2/fedot_ind/core/models/recurrence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/recurrence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/recurrence/reccurence_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/recurrence/sequences.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.309554 fedot_ind-0.4.1.2/fedot_ind/core/models/topological/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/topological/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/topological/topofeatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/topological/topological_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.309554 fedot_ind-0.4.1.2/fedot_ind/core/models/ts_forecasting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/ts_forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/models/ts_forecasting/ssa_forecaster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.309554 fedot_ind-0.4.1.2/fedot_ind/core/operation/
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/IndustrialCachableOperation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.309554 fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/decomposed_conv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.309554 fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/matrix_decomposition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/matrix_decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/matrix_decomposition/column_sampling_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/matrix_decomposition/dmd_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/matrix_decomposition/power_iteration_decomposition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.309554 fedot_ind-0.4.1.2/fedot_ind/core/operation/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/dummy/dummy_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.309554 fedot_ind-0.4.1.2/fedot_ind/core/operation/filtration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/filtration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/filtration/feature_filtration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.309554 fedot_ind-0.4.1.2/fedot_ind/core/operation/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/interfaces/fedot_automl_evaluation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/interfaces/industrial_model_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19717 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.313554 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.313554 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/basis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/basis/abstract_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/basis/eigen_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/basis/fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/basis/wavelet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.313554 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/data/eigen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/data/hankel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/data/kernel_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/data/point_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.313554 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/regularization/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/window_cutter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/window_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.313554 fedot_ind-0.4.1.2/fedot_ind/core/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/optimizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.317554 fedot_ind-0.4.1.2/fedot_ind/core/repository/
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/IndustrialDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/IndustrialOperationParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30794 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/constanst_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.317554 fedot_ind-0.4.1.2/fedot_ind/core/repository/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/data/default_operation_params.json
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/data/industrial_data_operation_repository.json
--rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/data/industrial_model_repository.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.317554 fedot_ind-0.4.1.2/fedot_ind/core/repository/industrial_implementations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/industrial_implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/industrial_implementations/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/industrial_implementations/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    23088 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/industrial_implementations/optimisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/initializer_industrial_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/repository/model_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.317554 fedot_ind-0.4.1.2/fedot_ind/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31995 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/core/tuning/search_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.317554 fedot_ind-0.4.1.2/fedot_ind/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/tools/example_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.317554 fedot_ind-0.4.1.2/fedot_ind/tools/explain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/tools/explain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/tools/explain/distances.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/tools/explain/explain.py
--rw-r--r--   0 runner    (1001) docker     (127)    44594 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/tools/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.317554 fedot_ind-0.4.1.2/fedot_ind/tools/synthetic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/tools/synthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/tools/synthetic/anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/tools/synthetic/anomaly_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/tools/synthetic/ts_datasets_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/fedot_ind/tools/synthetic/ts_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:51:47.317554 fedot_ind-0.4.1.2/fedot_ind.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-03-07 12:51:47.000000 fedot_ind-0.4.1.2/fedot_ind.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-03-07 12:51:47.000000 fedot_ind-0.4.1.2/fedot_ind.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 12:51:47.000000 fedot_ind-0.4.1.2/fedot_ind.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-07 12:51:47.000000 fedot_ind-0.4.1.2/fedot_ind.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-07 12:51:47.000000 fedot_ind-0.4.1.2/fedot_ind.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 12:51:47.321554 fedot_ind-0.4.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-07 12:51:38.000000 fedot_ind-0.4.1.2/setup.py
+-rw-r--r--   0        0        0     1538 2024-05-02 12:21:48.038684 fedot_ind-0.4.2/LICENSE.md
+-rw-r--r--   0        0        0    13897 2024-05-02 12:21:48.038684 fedot_ind-0.4.2/README_en.rst
+-rw-r--r--   0        0        0       26 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/api/__init__.py
+-rw-r--r--   0        0        0    27013 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/api/main.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/api/utils/__init__.py
+-rw-r--r--   0        0        0     7228 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/api/utils/checkers_collections.py
+-rw-r--r--   0        0        0     2658 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/api/utils/data.py
+-rw-r--r--   0        0        0    12016 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/api/utils/industrial_strategy.py
+-rw-r--r--   0        0        0     2122 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/api/utils/metafeatures.py
+-rw-r--r--   0        0        0      513 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/api/utils/path_lib.py
+-rw-r--r--   0        0        0     2739 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/api/utils/recurrent_image.py
+-rw-r--r--   0        0        0     2137 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/api/utils/saver_collections.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/core/architecture/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/core/architecture/abstraction/__init__.py
+-rw-r--r--   0        0        0     3802 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/core/architecture/abstraction/decorators.py
+-rw-r--r--   0        0        0      696 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/core/architecture/abstraction/сheckers.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/core/architecture/pipelines/__init__.py
+-rw-r--r--   0        0        0     5142 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/core/architecture/pipelines/abstract_pipeline.py
+-rw-r--r--   0        0        0     7566 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/core/architecture/pipelines/anomaly_detection.py
+-rw-r--r--   0        0        0     9045 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/core/architecture/pipelines/classification.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/core/architecture/postprocessing/__init__.py
+-rw-r--r--   0        0        0     2743 2024-05-02 12:21:49.654705 fedot_ind-0.4.2/fedot_ind/core/architecture/postprocessing/optimisation_history.py
+-rw-r--r--   0        0        0     7017 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/architecture/postprocessing/results_picker.py
+-rw-r--r--   0        0        0    32241 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/architecture/postprocessing/ucr_datasets.json
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/architecture/postprocessing/visualisation/__init__.py
+-rw-r--r--   0        0        0     1151 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/architecture/postprocessing/visualisation/gradcam_vis.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/architecture/preprocessing/__init__.py
+-rw-r--r--   0        0        0    25086 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/architecture/preprocessing/data_convertor.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/architecture/settings/__init__.py
+-rw-r--r--   0        0        0     2887 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/architecture/settings/computational.py
+-rw-r--r--   0        0        0     3336 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/architecture/settings/pipeline_factory.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/ensemble/__init__.py
+-rw-r--r--   0        0        0     2226 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/ensemble/base_ensembler.py
+-rw-r--r--   0        0        0     8300 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/ensemble/kernel_ensemble.py
+-rw-r--r--   0        0        0     4444 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/ensemble/random_automl_forest.py
+-rw-r--r--   0        0        0    12696 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/ensemble/rank_ensembler.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/metrics/__init__.py
+-rw-r--r--   0        0        0     2553 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/metrics/evaluation.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/metrics/loss/__init__.py
+-rw-r--r--   0        0        0     1285 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/metrics/loss/basis_loss.py
+-rw-r--r--   0        0        0     4365 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/metrics/loss/soft_dtw.py
+-rw-r--r--   0        0        0     2512 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/metrics/loss/svd_loss.py
+-rw-r--r--   0        0        0    10951 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/metrics/metrics_implementation.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/automl/__init__.py
+-rw-r--r--   0        0        0     2219 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/automl/fedot_implementation.py
+-rw-r--r--   0        0        0     6845 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/base_extractor.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/detection/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/detection/probalistic/__init__.py
+-rw-r--r--   0        0        0    19099 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/detection/probalistic/kalman.py
+-rw-r--r--   0        0        0    17521 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/detection/probalistic/sigma.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/detection/subspaces/__init__.py
+-rw-r--r--   0        0        0     7965 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/detection/subspaces/func_pca.py
+-rw-r--r--   0        0        0    11482 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/detection/subspaces/sst.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/manifold/__init__.py
+-rw-r--r--   0        0        0     5276 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/manifold/riemann_embeding.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/__init__.py
+-rw-r--r--   0        0        0     9392 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/base_nn_model.py
+-rw-r--r--   0        0        0     4766 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/chronos_tst.py
+-rw-r--r--   0        0        0    11124 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/explainable_convolution_model.py
+-rw-r--r--   0        0        0     4219 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/inception.py
+-rw-r--r--   0        0        0    14641 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/mini_rocket.py
+-rw-r--r--   0        0        0     7497 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/omni_scale.py
+-rw-r--r--   0        0        0    18452 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/patch_tst.py
+-rw-r--r--   0        0        0     5588 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/resnet.py
+-rw-r--r--   0        0        0     4285 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/transformer.py
+-rw-r--r--   0        0        0    12905 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/tst.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/__init__.py
+-rw-r--r--   0        0        0     2262 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/activation.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/__init__.py
+-rw-r--r--   0        0        0     6796 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/attention_layers.py
+-rw-r--r--   0        0        0     2684 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/backbone.py
+-rw-r--r--   0        0        0     8797 2024-05-02 12:21:49.658705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/conv_layers.py
+-rw-r--r--   0        0        0    12460 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/head_layers.py
+-rw-r--r--   0        0        0     8484 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/linear_layers.py
+-rw-r--r--   0        0        0     1902 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/padding_layers.py
+-rw-r--r--   0        0        0     7244 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/pooling_layers.py
+-rw-r--r--   0        0        0    16816 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/special.py
+-rw-r--r--   0        0        0     8812 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/losses.py
+-rw-r--r--   0        0        0    22475 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/other.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/quantile/__init__.py
+-rw-r--r--   0        0        0     4174 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/quantile/quantile_extractor.py
+-rw-r--r--   0        0        0     8376 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/quantile/stat_features.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/recurrence/__init__.py
+-rw-r--r--   0        0        0     4380 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/recurrence/reccurence_extractor.py
+-rw-r--r--   0        0        0     6915 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/recurrence/sequences.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/topological/__init__.py
+-rw-r--r--   0        0        0    10205 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/topological/topofeatures.py
+-rw-r--r--   0        0        0     6619 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/topological/topological_extractor.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/ts_forecasting/__init__.py
+-rw-r--r--   0        0        0     5436 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/ts_forecasting/glm.py
+-rw-r--r--   0        0        0    10200 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/models/ts_forecasting/ssa_forecaster.py
+-rw-r--r--   0        0        0     4326 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/IndustrialCachableOperation.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/__init__.py
+-rw-r--r--   0        0        0     3628 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/caching.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/decomposition/__init__.py
+-rw-r--r--   0        0        0     7148 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/decomposition/decomposed_conv.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/decomposition/matrix_decomposition/__init__.py
+-rw-r--r--   0        0        0     5852 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/decomposition/matrix_decomposition/column_sampling_decomposition.py
+-rw-r--r--   0        0        0     4040 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/decomposition/matrix_decomposition/dmd_decomposition.py
+-rw-r--r--   0        0        0     5796 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/decomposition/matrix_decomposition/power_iteration_decomposition.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/dummy/__init__.py
+-rw-r--r--   0        0        0     1217 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/dummy/dummy_operation.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/filtration/__init__.py
+-rw-r--r--   0        0        0     8657 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/filtration/channel_filtration.py
+-rw-r--r--   0        0        0    10795 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/filtration/feature_filtration.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/interfaces/__init__.py
+-rw-r--r--   0        0        0     3360 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/interfaces/fedot_automl_evaluation_strategy.py
+-rw-r--r--   0        0        0     8319 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/interfaces/industrial_model_strategy.py
+-rw-r--r--   0        0        0    21017 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/basis/__init__.py
+-rw-r--r--   0        0        0     3169 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/basis/abstract_basis.py
+-rw-r--r--   0        0        0     8836 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/basis/eigen_basis.py
+-rw-r--r--   0        0        0     1949 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/basis/fourier.py
+-rw-r--r--   0        0        0     3406 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/basis/wavelet.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/data/__init__.py
+-rw-r--r--   0        0        0     3220 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/data/eigen.py
+-rw-r--r--   0        0        0     4457 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/data/hankel.py
+-rw-r--r--   0        0        0     3603 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/data/kernel_matrix.py
+-rw-r--r--   0        0        0     7444 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/data/point_cloud.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/regularization/__init__.py
+-rw-r--r--   0        0        0     3114 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/regularization/spectrum.py
+-rw-r--r--   0        0        0    11937 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/splitter.py
+-rw-r--r--   0        0        0     1383 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/window_cutter.py
+-rw-r--r--   0        0        0    10183 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/operation/transformation/window_selector.py
+-rw-r--r--   0        0        0     1767 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/optimizer/__init__.py
+-rw-r--r--   0        0        0     5044 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/repository/IndustrialDispatcher.py
+-rw-r--r--   0        0        0     1861 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/repository/IndustrialOperationParameters.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.662705 fedot_ind-0.4.2/fedot_ind/core/repository/__init__.py
+-rw-r--r--   0        0        0    33408 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/repository/constanst_repository.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/repository/data/__init__.py
+-rw-r--r--   0        0        0     4669 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/repository/data/default_operation_params.json
+-rw-r--r--   0        0        0    14954 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/repository/data/industrial_data_operation_repository.json
+-rw-r--r--   0        0        0    15411 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/repository/data/industrial_model_repository.json
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/repository/industrial_implementations/__init__.py
+-rw-r--r--   0        0        0    19018 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/repository/industrial_implementations/abstract.py
+-rw-r--r--   0        0        0     1987 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/repository/industrial_implementations/metric.py
+-rw-r--r--   0        0        0    23419 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/repository/industrial_implementations/optimisation.py
+-rw-r--r--   0        0        0     6956 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/repository/initializer_industrial_models.py
+-rw-r--r--   0        0        0    11023 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/repository/model_repository.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/tuning/__init__.py
+-rw-r--r--   0        0        0    30039 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/core/tuning/search_space.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/tools/__init__.py
+-rw-r--r--   0        0        0     5576 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/tools/example_utils.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/tools/explain/__init__.py
+-rw-r--r--   0        0        0     3521 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/tools/explain/distances.py
+-rw-r--r--   0        0        0     7917 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/tools/explain/explain.py
+-rw-r--r--   0        0        0    45352 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/tools/loader.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/tools/synthetic/__init__.py
+-rw-r--r--   0        0        0     3900 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/tools/synthetic/anomalies.py
+-rw-r--r--   0        0        0    11227 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/tools/synthetic/anomaly_generator.py
+-rw-r--r--   0        0        0     3977 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/tools/synthetic/ts_datasets_generator.py
+-rw-r--r--   0        0        0     7461 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/fedot_ind/tools/synthetic/ts_generator.py
+-rw-r--r--   0        0        0     1075 2024-05-02 12:21:49.666705 fedot_ind-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    15384 1970-01-01 00:00:00.000000 fedot_ind-0.4.2/PKG-INFO
```

### Comparing `fedot_ind-0.4.1.2/LICENSE.md` & `fedot_ind-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/PKG-INFO` & `fedot_ind-0.4.2/README_en.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: fedot_ind
-Version: 0.4.1.2
-Summary: Automated machine learning framework for time series analysis
-Home-page: https://github.com/aimclub/Fedot.Industrial
-Author: NSS Lab
-Author-email: itmo.nss.team@gmail.com
-License: BSD 3-Clause
-Keywords: automated machine learning,time series analysis,anomaly detection,classification
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE.md
-Requires-Dist: fedot
-Requires-Dist: catboost==1.1.1; sys_platform == "darwin"
-Requires-Dist: MKLpy==0.6
-Requires-Dist: PyMonad==2.4.0
-Requires-Dist: PyWavelets==1.4.1
-Requires-Dist: giotto_tda==0.6.0
-Requires-Dist: ripser==0.6.4
-Requires-Dist: fastcore
-Requires-Dist: fastai
-Requires-Dist: distributed
-Requires-Dist: datasetsforecast
-Requires-Dist: tensorly==0.8.1
-Requires-Dist: torch==2.0.0
-Requires-Dist: torchvision==0.15.1
-Requires-Dist: statsforecast==1.5.0
-Requires-Dist: chardet
-
 .. image:: /docs/img/fedot-industrial.png
     :width: 600px
     :align: center
     :alt: Fedot Industrial logo
 
 
 ================================================================================
@@ -90,15 +57,15 @@
     :target: https://mybinder.org/v2/gh/aimclub/Fedot.Industrial/HEAD
 
 .. |downloads| image:: https://static.pepy.tech/personalized-badge/fedot-ind?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
     :target: https://pepy.tech/project/fedot-ind
     :alt: Downloads
 
 .. |support| image:: https://img.shields.io/badge/Telegram-Group-blue.svg
-    :target: https://t.me/fedotindustrial_support
+    :target: https://t.me/FEDOT_helpdesk
     :alt: Support
 
 .. |rus| image:: https://img.shields.io/badge/lang-ru-yellow.svg
     :target: /README.rst
 
 .. |eng| image:: https://img.shields.io/badge/lang-eng-green.svg
     :target: /README_en.rst
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/api/main.py` & `fedot_ind-0.4.2/fedot_ind/api/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import logging
 import os
 import warnings
 from copy import deepcopy
 from pathlib import Path
 from typing import Union
 
+import matplotlib
 import numpy as np
 import pandas as pd
 from fedot.api.main import Fedot
 from fedot.core.pipelines.pipeline import Pipeline
-from fedot.core.pipelines.tuning.tuner_builder import TunerBuilder
+from fedot.core.repository.tasks import TsForecastingParams
+from fedot.core.visualisation.pipeline_specific_visuals import PipelineHistoryVisualizer
+from golem.core.optimisers.opt_history_objects.opt_history import OptHistory
 
 from fedot_ind.api.utils.checkers_collections import DataCheck
+from fedot_ind.api.utils.industrial_strategy import IndustrialStrategy
 from fedot_ind.api.utils.path_lib import DEFAULT_PATH_RESULTS as default_path_to_save_results
 from fedot_ind.core.architecture.abstraction.decorators import DaskServer
+from fedot_ind.core.architecture.preprocessing.data_convertor import ApiConverter
 from fedot_ind.core.architecture.settings.computational import BackendMethods
-from fedot_ind.core.ensemble.random_automl_forest import RAFensembler
 from fedot_ind.core.operation.transformation.splitter import TSTransformer
 from fedot_ind.core.optimizer.IndustrialEvoOptimizer import IndustrialEvoOptimizer
-from fedot_ind.core.repository.constanst_repository import BATCH_SIZE_FOR_FEDOT_WORKER, FEDOT_WORKER_NUM, \
-    FEDOT_WORKER_TIMEOUT_PARTITION, FEDOT_GET_METRICS, FEDOT_TUNING_METRICS, FEDOT_HEAD_ENSEMBLE, \
+from fedot_ind.core.repository.constanst_repository import \
+    FEDOT_GET_METRICS, FEDOT_TUNING_METRICS, \
     FEDOT_API_PARAMS, FEDOT_ASSUMPTIONS, FEDOT_TUNER_STRATEGY
 from fedot_ind.core.repository.industrial_implementations.abstract import build_tuner
 from fedot_ind.core.repository.initializer_industrial_models import IndustrialModels
 from fedot_ind.core.repository.model_repository import default_industrial_availiable_operation
 from fedot_ind.tools.explain.explain import PointExplainer
 from fedot_ind.tools.synthetic.anomaly_generator import AnomalyGenerator
 from fedot_ind.tools.synthetic.ts_generator import TimeSeriesGenerator
@@ -64,241 +68,296 @@
 
     """
 
     def __init__(self, **kwargs):
 
         # init Fedot and Industrial hyperparams and path to results
         self.output_folder = kwargs.get('output_folder', None)
-        self.preprocessing = kwargs.get('industrial_preprocessing', False)
+        self.industrial_strategy_params = kwargs.get('industrial_strategy_params', None)
+        self.industrial_strategy = kwargs.get('industrial_strategy', None)
+        self.path_to_composition_results = kwargs.get('history_dir', None)
         self.backend_method = kwargs.get('backend', 'cpu')
-        self.RAF_workers = kwargs.get('RAF_workers', None)
         self.task_params = kwargs.get('task_params', None)
-        self.model_params = kwargs.get('model_params', None)
-        self.path_to_composition_results = kwargs.get('history_dir', None)
+
+        # TODO: unused params
+        # self.model_params = kwargs.get('model_params', None)
+        # self.RAF_workers = kwargs.get('RAF_workers', None)
 
         # create dirs with results
-        prefix = './composition_results' if self.path_to_composition_results is None else \
-            self.path_to_composition_results
+        if self.path_to_composition_results is None:
+            prefix = './composition_results'
+        else:
+            prefix = self.path_to_composition_results
+
         Path(prefix).mkdir(parents=True, exist_ok=True)
+
         # create dirs with results
         if self.output_folder is None:
             self.output_folder = default_path_to_save_results
             Path(self.output_folder).mkdir(parents=True, exist_ok=True)
         else:
             Path(self.output_folder).mkdir(parents=True, exist_ok=True)
             del kwargs['output_folder']
         # init logger
-        logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)s: %(name)s - %(message)s',
+        logging.basicConfig(level=logging.INFO,
+                            format='%(asctime)s %(levelname)s: %(name)s - %(message)s',
                             handlers=[logging.FileHandler(Path(self.output_folder) / 'log.log'),
-                                      logging.StreamHandler()])
+                                      logging.StreamHandler()]
+                            )
         super(Fedot, self).__init__()
+
         # init hidden state variables
         self.logger = logging.getLogger('FedotIndustrialAPI')
         self.solver = None
         self.predicted_labels = None
         self.predicted_probs = None
         self.predict_data = None
         self.target_encoder = None
+        self.is_finetuned = False
+
         # map Fedot params to Industrial params
         self.config_dict = kwargs
         self.config_dict['history_dir'] = prefix
-        self.config_dict['available_operations'] = kwargs.get('available_operations',
-                                                              default_industrial_availiable_operation(
-                                                                  self.config_dict['problem']))
+        self.config_dict['available_operations'] = kwargs.get(
+            'available_operations',
+            default_industrial_availiable_operation(
+                self.config_dict['problem'])
+        )
 
         self.config_dict['optimizer'] = kwargs.get(
             'optimizer', IndustrialEvoOptimizer)
         self.config_dict['initial_assumption'] = kwargs.get('initial_assumption',
                                                             FEDOT_ASSUMPTIONS[self.config_dict['problem']])
+        self.config_dict['use_input_preprocessing'] = kwargs.get(
+            'use_input_preprocessing', False)
+
+        if self.task_params is not None and self.config_dict['problem'] == 'ts_forecasting':
+            self.config_dict['task_params'] = TsForecastingParams(
+                forecast_length=self.task_params['forecast_length'])
+
+        # create API subclasses for side task
         self.__init_experiment_setup()
+        self.condition_check = ApiConverter()
+        self.industrial_strategy_class = IndustrialStrategy(api_config=self.config_dict,
+                                                            industrial_strategy=self.industrial_strategy,
+                                                            industrial_strategy_params=self.industrial_strategy_params,
+                                                            logger=self.logger)
 
     def __init_experiment_setup(self):
         self.logger.info('Initialising experiment setup')
-        industrial_params = [param for param in self.config_dict.keys(
-        ) if param not in list(FEDOT_API_PARAMS.keys())]
-        [self.config_dict.pop(x, None) for x in industrial_params]
+        # industrial_params = [p for p in self.config_dict.keys() if p not in list(FEDOT_API_PARAMS.keys())]
+        # [self.config_dict.pop(x, None) for x in industrial_params]
+
+        industrial_params = set(self.config_dict.keys()) - \
+            set(FEDOT_API_PARAMS.keys())
+        for param in industrial_params:
+            self.config_dict.pop(param, None)
+
         backend_method_current, backend_scipy_current = BackendMethods(
             self.backend_method).backend
         globals()['backend_methods'] = backend_method_current
         globals()['backend_scipy'] = backend_scipy_current
 
     def __init_solver(self):
         self.logger.info('Initialising Industrial Repository')
         self.repo = IndustrialModels().setup_repository()
-        if self.config_dict['problem'] == 'ts_forecasting':
-            solver = self.config_dict['initial_assumption'].build()
-            solver.root_node.parameters = self.model_params
-        else:
-            self.logger.info('Initialising Dask Server')
-            self.config_dict['initial_assumption'] = self.config_dict['initial_assumption'].build(
-            )
-            self.dask_client = DaskServer().client
-            self.logger.info(
-                f'LinK Dask Server - {self.dask_client.dashboard_link}')
-            self.logger.info('Initialising solver')
-            solver = Fedot(**self.config_dict)
-        return solver
+        self.logger.info('Initialising Dask Server')
+        self.config_dict['initial_assumption'] = self.config_dict['initial_assumption'].build()
+        self.dask_client = DaskServer().client
+        self.logger.info(
+            f'LinK Dask Server - {self.dask_client.dashboard_link}')
+        self.logger.info('Initialising solver')
+        self.solver = Fedot(**self.config_dict)
 
     def shutdown(self):
         self.dask_client.close()
         del self.dask_client
 
-    def _predict_raf_ensemble(self, mode: str = 'labels'):
-        self.predicted_branch_probs = [x.predict(self.predict_data).predict
-                                       for x in self.solver.root_node.nodes_from]
-        self.predicted_branch_labels = [np.argmax(x, axis=1) for x in self.predicted_branch_probs]
-        n_samples, n_channels, n_classes = self.predicted_branch_probs[0].shape[0], \
-                                           len(self.predicted_branch_probs), \
-                                           self.predicted_branch_probs[0].shape[1]
-        head_model = deepcopy(self.solver.root_node)
-        head_model.nodes_from = []
-        self.predict_data.features = np.hstack(self.predicted_branch_labels).reshape(n_samples,
-                                                                                     n_channels, 1)
-        head_predict = head_model.predict(self.predict_data).predict
-        if mode == 'labels':
-            return head_predict
-        else:
-            return np.argmax(head_predict, axis=1)
-
-    def _preprocessing_strategy(self, input_data):
-        if input_data.features.shape[0] > BATCH_SIZE_FOR_FEDOT_WORKER:
-            self._batch_strategy(input_data)
-
-    def _batch_strategy(self, input_data):
-        self.logger.info('RAF algorithm was applied')
-        batch_size = round(input_data.features.shape[0] / self.RAF_workers if self.RAF_workers
-                                                                              is not None else FEDOT_WORKER_NUM)
-        batch_timeout = round(
-            self.config_dict['timeout'] / FEDOT_WORKER_TIMEOUT_PARTITION)
-        self.config_dict['timeout'] = batch_timeout
-        self.logger.info(
-            f'Batch_size - {batch_size}. Number of batches - {self.RAF_workers}')
-        self.solver = RAFensembler(composing_params=self.config_dict, n_splits=self.RAF_workers,
-                                   batch_size=batch_size)
-        self.logger.info(
-            f'Number of AutoMl models in ensemble - {self.solver.n_splits}')
-
     def fit(self,
             input_data: tuple,
             **kwargs):
         """
         Method for training Industrial model.
 
         Args:
             input_data: tuple with train_features and train_target
             **kwargs: additional parameters
 
         """
         self.train_data = deepcopy(
             input_data)  # we do not want to make inplace changes
         input_preproc = DataCheck(input_data=self.train_data, task=self.config_dict['problem'],
-                                  task_params=self.task_params)
+                                  task_params=self.task_params, industrial_task_params=self.industrial_strategy_params)
         self.train_data = input_preproc.check_input_data()
         self.target_encoder = input_preproc.get_target_encoder()
-        self.solver = self.__init_solver()
-        if self.preprocessing:
-            self._preprocessing_strategy(self.train_data)
-        self.solver.fit(self.train_data)
+        self.__init_solver()
+        if self.industrial_strategy is not None:
+            self.solver = self.industrial_strategy_class.fit(self.train_data)
+        else:
+            self.solver.fit(self.train_data)
+        self.is_finetuned = False
 
     def predict(self,
                 predict_data: tuple,
                 predict_mode: str = 'default',
                 **kwargs):
         """
         Method to obtain prediction labels from trained Industrial model.
 
         Args:
+            predict_mode: ``default='default'``. Defines the mode of prediction. Could be 'default' or 'probs'.
             predict_data: tuple with test_features and test_target
 
         Returns:
             the array with prediction values
 
         """
-        self.predict_data = deepcopy(predict_data)  # we do not want to make inplace changes
+        self.predict_data = deepcopy(
+            predict_data)  # we do not want to make inplace changes
         self.predict_data = DataCheck(input_data=self.predict_data,
                                       task=self.config_dict['problem'],
-                                      task_params=self.task_params).check_input_data()
-        if predict_mode == 'RAF_ensemble':
-            self.predicted_labels = self._predict_raf_ensemble()
+                                      task_params=self.task_params,
+                                      industrial_task_params=self.industrial_strategy_params).check_input_data()
+        if self.industrial_strategy is not None and not self.is_finetuned:
+            if predict_mode == 'ensemble':
+                predict = self.industrial_strategy_class.predict(
+                    self.predict_data, 'probs')
+                ensemble_strat = self.industrial_strategy_class.ensemble_strategy
+                predict = {
+                    strategy: np.argmax(self.industrial_strategy_class.ensemble_predictions(
+                        predict, strategy), axis=1)
+                    for
+                    strategy in ensemble_strat}
+            else:
+                predict = self.industrial_strategy_class.predict(
+                    self.predict_data, 'labels')
+            self.predicted_labels = predict
         else:
-            if isinstance(self.solver, Fedot):
+            if self.condition_check.solver_is_fedot_class(self.solver):
                 predict = self.solver.predict(self.predict_data)
             else:
-                predict = self.solver.predict(self.predict_data, 'labels').predict
-                if self.config_dict['problem'] == 'classification' \
-                        and self.predict_data.target.min() - predict.min() != 0 \
-                        and len(np.unique(predict).shape) != 1:
-                    predict = predict + (self.predict_data.target.min() - predict.min())
-            if self.target_encoder is not None:
-                self.predicted_labels = self.target_encoder.inverse_transform(predict)
-                self.predict_data.target = self.target_encoder.inverse_transform(self.predict_data.target)
+                predict = self.solver.predict(
+                    self.predict_data, 'labels').predict
+                if self.condition_check.is_multiclf_with_labeling_problem(self.config_dict['problem'],
+                                                                          self.predict_data.target,
+                                                                          predict):
+                    predict = predict + \
+                        (self.predict_data.target.min() - predict.min())
+
+            if self.condition_check.solver_have_target_encoder(self.target_encoder):
+                self.predicted_labels = self.target_encoder.inverse_transform(
+                    predict)
+                self.predict_data.target = self.target_encoder.inverse_transform(
+                    self.predict_data.target)
             else:
                 self.predicted_labels = predict
         return self.predicted_labels
 
     def predict_proba(self,
                       predict_data: tuple,
                       predict_mode: str = 'default',
                       **kwargs):
         """
         Method to obtain prediction probabilities from trained Industrial model.
 
         Args:
+            predict_mode: ``default='default'``. Defines the mode of prediction. Could be 'default' or 'probs'.
             predict_data: tuple with test_features and test_target
 
         Returns:
             the array with prediction probabilities
 
         """
         self.predict_data = deepcopy(
             predict_data)  # we do not want to make inplace changes
         self.predict_data = DataCheck(input_data=self.predict_data,
                                       task=self.config_dict['problem'],
-                                      task_params=self.task_params).check_input_data()
-        if predict_mode == 'RAF_ensemble':
-            predict = self.predicted_labels = self._predict_raf_ensemble()
+                                      task_params=self.task_params,
+                                      industrial_task_params=self.industrial_strategy_params).check_input_data()
+        if self.industrial_strategy is not None and not self.is_finetuned:
+            predict = self.industrial_strategy_class.predict(
+                self.predict_data, 'probs')
+            if predict_mode == 'ensemble':
+                ensemble_strat = self.industrial_strategy_class.ensemble_strategy
+                predict = {strategy: self.industrial_strategy_class.ensemble_predictions(predict, strategy)
+                           for strategy in ensemble_strat}
         else:
-            if isinstance(self.solver, Fedot):
+            if self.condition_check.solver_is_fedot_class(self.solver):
                 predict = self.solver.predict_proba(self.predict_data)
             else:
-                predict = self.solver.predict(self.predict_data, 'probs').predict
-                if self.config_dict['problem'] == 'classification' and \
-                        self.predict_data.target.min() - predict.min() != 0:
-                    predict = predict + (self.predict_data.target.min() - predict.min())
+                predict = self.solver.predict(
+                    self.predict_data, 'probs').predict
+                if self.condition_check.is_multiclf_with_labeling_problem(self.config_dict['problem'],
+                                                                          self.predict_data.target,
+                                                                          predict):
+                    predict = predict + \
+                        (self.predict_data.target.min() - predict.min())
         self.predicted_probs = predict
         return self.predicted_probs
 
     def finetune(self,
                  train_data,
                  tuning_params=None,
+                 model_to_tune=None,
                  mode: str = 'head'):
-        """
-            Method to obtain prediction probabilities from trained Industrial model.
+        """Method to obtain prediction probabilities from trained Industrial model.
 
             Args:
+                model_to_tune: model to fine-tune
                 train_data: raw train data
                 tuning_params: dictionary with tuning parameters
-                mode: str, ``default='full'``. Defines the mode of fine-tuning. Could be 'full' or 'head'.
+                mode: str, ``default='head'``. Defines the mode of fine-tuning. Could be 'full' or 'head'.
 
             """
-
-        train_data = DataCheck(
-            input_data=train_data, task=self.config_dict['problem']).check_input_data()
-        tuning_params = {} if tuning_params is None else tuning_params
+        if not self.condition_check.input_data_is_fedot_type(train_data):
+            input_preproc = DataCheck(input_data=train_data,
+                                      task=self.config_dict['problem'],
+                                      task_params=self.task_params)
+            train_data = input_preproc.check_input_data()
+            self.target_encoder = input_preproc.get_target_encoder()
+        tuning_params = ApiConverter.tuning_params_is_none(tuning_params)
         tuned_metric = 0
         tuning_params['metric'] = FEDOT_TUNING_METRICS[self.config_dict['problem']]
         for tuner_name, tuner_type in FEDOT_TUNER_STRATEGY.items():
-            model_to_tune = deepcopy(self.solver.current_pipeline) if isinstance(self.solver, Fedot) \
-                else deepcopy(self.solver)
+            if self.condition_check.solver_is_fedot_class(self.solver):
+                model_to_tune = deepcopy(self.solver.current_pipeline)
+            elif not self.condition_check.solver_is_none(model_to_tune):
+                model_to_tune = model_to_tune
+            else:
+                model_to_tune = deepcopy(
+                    self.config_dict['initial_assumption']).build()
             tuning_params['tuner'] = tuner_type
             pipeline_tuner, model_to_tune = build_tuner(
                 self, model_to_tune, tuning_params, train_data, mode)
             if abs(pipeline_tuner.obtained_metric) > tuned_metric:
                 tuned_metric = abs(pipeline_tuner.obtained_metric)
                 self.solver = model_to_tune
+        self.is_finetuned = True
+
+    def _metric_evaluation_loop(self,
+                                target,
+                                predicted_labels,
+                                predicted_probs,
+                                problem,
+                                metric_names,
+                                rounding_order):
+        valid_shape = target.shape
+        if self.condition_check.solver_have_target_encoder(self.target_encoder):
+            new_target = self.target_encoder.transform(target.flatten())
+            labels = self.target_encoder.transform(
+                predicted_labels).reshape(valid_shape)
+        else:
+            new_target = target.flatten()
+            labels = predicted_labels.reshape(valid_shape)
+
+        return FEDOT_GET_METRICS[problem](target=new_target,
+                                          metric_names=metric_names,
+                                          rounding_order=rounding_order,
+                                          labels=labels,
+                                          probs=predicted_probs)
 
     def get_metrics(self,
                     target: Union[list, np.array] = None,
                     metric_names: tuple = ('f1', 'roc_auc', 'accuracy'),
                     rounding_order: int = 3,
                     **kwargs) -> pd.DataFrame:
         """
@@ -318,22 +377,31 @@
             pandas DataFrame with calculated metrics
 
         """
         problem = self.config_dict['problem']
         if problem == 'classification' and self.predicted_probs is None and 'roc_auc' in metric_names:
             self.logger.info(
                 'Predicted probabilities are not available. Use `predict_proba()` method first')
+        if isinstance(self.predicted_probs, dict):
+            metric_dict = {strategy: self._metric_evaluation_loop(target=target,
+                                                                  problem=problem,
+                                                                  predicted_labels=self.predicted_labels[strategy],
+                                                                  predicted_probs=probs,
+                                                                  rounding_order=rounding_order,
+                                                                  metric_names=metric_names) for strategy, probs in
+                           self.predicted_probs.items()}
 
-        valid_shape = target.shape
-        return FEDOT_GET_METRICS[problem](target=target.flatten(),
-                                          metric_names=metric_names,
-                                          rounding_order=rounding_order,
-                                          labels=self.predicted_labels.reshape(
-                                              valid_shape),
-                                          probs=self.predicted_probs)
+        else:
+            metric_dict = self._metric_evaluation_loop(target=target,
+                                                       problem=problem,
+                                                       predicted_labels=self.predicted_labels,
+                                                       predicted_probs=self.predicted_probs,
+                                                       rounding_order=rounding_order,
+                                                       metric_names=metric_names)
+        return metric_dict
 
     def save_predict(self, predicted_data, **kwargs) -> None:
         """
         Method to save prediction locally in csv format
 
         Args:
             predicted_data: predicted data. For TSC task it could be either labels or probabilities
@@ -376,58 +444,47 @@
             self.solver = Pipeline().load(path)
         else:
             self.solver = []
             for p in dir_list:
                 self.solver.append(Pipeline().load(
                     f'{path}/{p}/0_pipeline_saved'))
 
-    def save_optimization_history(self, **kwargs):
+    def save_optimization_history(self, return_history: bool = False):
         """Plot prediction of the model"""
         self.solver.history.save(
             f"{self.output_folder}/optimization_history.json")
+        if return_history:
+            return self.solver.history
 
     def save_best_model(self):
-        if isinstance(self.solver, Fedot):
+        if self.condition_check.solver_is_fedot_class(self.solver):
             return self.solver.current_pipeline.save(path=self.output_folder, create_subdir=True,
                                                      is_datetime_in_path=True)
-        elif isinstance(self.solver, Pipeline):
+        elif self.condition_check.solver_is_pipeline_class(self.solver):
             return self.solver.save(path=self.output_folder, create_subdir=True,
                                     is_datetime_in_path=True)
         else:
             for idx, p in enumerate(self.solver.ensemble_branches):
-                Pipeline(p).save(f'./raf_ensemble/{idx}_ensemble_branch', create_subdir=True)
-            Pipeline(self.solver.ensemble_head).save(f'./raf_ensemble/ensemble_head', create_subdir=True)
-            self.solver.current_pipeline.save(f'./raf_ensemble/ensemble_composed', create_subdir=True)
-
-    def plot_fitness_by_generation(self, **kwargs):
-        """Plot prediction of the model"""
-        self.solver.history.show.fitness_box(save_path=f'{self.output_folder}/fitness_by_gen.png',
-                                             best_fraction=0.5,
-                                             dpi=100)
-
-    def plot_operation_distribution(self, mode: str = 'total'):
-        """Plot prediction of the model"""
-        if mode == 'total':
-            self.solver.history.show.operations_kde(
-                save_path=f'{self.output_folder}/operation_kde.png', dpi=100)
-        else:
-            self.solver.history.show.operations_animated_bar(
-                save_path=f'{self.output_folder}/history_animated_bars.gif', show_fitness=True, dpi=100)
+                Pipeline(p).save(
+                    f'./raf_ensemble/{idx}_ensemble_branch', create_subdir=True)
+            Pipeline(self.solver.ensemble_head).save(
+                f'./raf_ensemble/ensemble_head', create_subdir=True)
+            self.solver.current_pipeline.save(
+                f'./raf_ensemble/ensemble_composed', create_subdir=True)
 
     def explain(self, **kwargs):
-        """ Explain model's prediction via time series points perturbation
-
-        Args:
-            samples: int, ``default=1``. Number of samples to explain.
-            window: int, ``default=5``. Window size for perturbation.
-            metric: str ``default='rmse'``. Distance metric for perturbation impact assessment.
-            threshold: int, ``default=90``. Threshold for perturbation impact assessment.
-            name: str, ``default='test'``. Name of the dataset to be placed on plot.
+        """Explain model's prediction via time series points perturbation
 
+            Args:
+                **kwargs: Additional arguments for explanation. These arguments control the
+                         number of samples, window size, metric, threshold, and dataset name.
+                         See the function implementation for detailed information on
+                         supported arguments.
         """
+
         methods = {'point': PointExplainer,
                    'shap': NotImplementedError,
                    'lime': NotImplementedError}
 
         explainer = methods[kwargs.get('method', 'point')](model=self,
                                                            features=self.predict_data.features.squeeze(),
                                                            target=self.predict_data.target)
@@ -440,14 +497,41 @@
         explainer.explain(n_samples=samples, window=window, method=metric)
         explainer.visual(threshold=threshold, name=name)
 
     def return_report(self) -> pd.DataFrame:
         if isinstance(self.solver, Fedot):
             return self.solver.return_report()
 
+    def vis_optimisation_history(self, opt_history_path: str = None,
+                                 mode: str = 'all',
+                                 return_history: bool = False):
+        """ The function runs visualization of the composing history and the best pipeline. """
+        # Gather pipeline and history.
+        matplotlib.use('TkAgg')
+        if isinstance(opt_history_path, str):
+            history = OptHistory.load(
+                opt_history_path + 'optimization_history.json')
+        else:
+            history = opt_history_path
+        history_visualizer = PipelineHistoryVisualizer(history)
+        vis_func = {
+            'fitness': (history_visualizer.fitness_box, dict(save_path='fitness_by_generation.png',
+                                                             best_fraction=1)),
+            'models': (history_visualizer.operations_animated_bar,
+                       dict(save_path='operations_animated_bar.gif', show_fitness=True)),
+            'diversity': (history_visualizer.diversity_population, dict(save_path='diversity_population.gif', fps=1))}
+        if mode == 'all':
+            for func, params in vis_func.values():
+                func(**params)
+        else:
+            func, params = vis_func[mode]
+            func(**params)
+        if return_history:
+            return history_visualizer.history
+
     @staticmethod
     def generate_ts(ts_config: dict):
         """
         Method to generate synthetic time series
 
         Args:
             ts_config: dict with config for synthetic ts_data.
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/api/utils/checkers_collections.py` & `fedot_ind-0.4.2/fedot_ind/api/utils/checkers_collections.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 from typing import Union
 
 import pandas as pd
 from fedot.core.data.data import InputData
 from fedot.core.repository.dataset_types import DataTypesEnum
+from fedot.core.repository.tasks import Task, TsForecastingParams, TaskTypesEnum
 from sklearn.preprocessing import LabelEncoder
 
 from fedot_ind.api.utils.data import check_multivariate_data
-from fedot_ind.core.architecture.preprocessing.data_convertor import NumpyConverter
+from fedot_ind.core.architecture.preprocessing.data_convertor import NumpyConverter, DataConverter
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
 from fedot_ind.core.repository.constanst_repository import FEDOT_TASK
 
 
 class DataCheck:
     """Class for checking and preprocessing input data for Fedot AutoML.
 
@@ -26,32 +27,35 @@
         task_dict (dict): Mapping of string task names to Fedot Task objects.
 
     """
 
     def __init__(self,
                  input_data: Union[tuple, InputData] = None,
                  task: str = None,
-                 task_params=None):
+                 task_params=None,
+                 industrial_task_params=None):
         self.logger = logging.getLogger(self.__class__.__name__)
+        self.industrial_task_params = industrial_task_params
         self.input_data = input_data
+        self.data_convertor = DataConverter(data=self.input_data)
         self.task = task
         self.task_params = task_params
         self.task_dict = FEDOT_TASK
         self.label_encoder = None
 
     def __check_features_and_target(self, X, y):
         multi_features, X = check_multivariate_data(X)
         multi_target = len(y.shape) > 1 and y.shape[1] > 2
 
         if multi_features:
             features = np.array(X.tolist()).astype(float)
         else:
             features = X
 
-        if type(y) is pd.DataFrame or type(y) is pd.Series:
+        if isinstance(y, (pd.DataFrame, pd.Series)):
             y = y.values
         if multi_target:
             target = y
         elif multi_features and not multi_target:
             target = y.reshape(-1, 1)
         else:
             target = np.ravel(y).reshape(-1, 1)
@@ -65,42 +69,52 @@
         with appropriate data types and task information. If an existing InputData
         object is provided, it checks if it requires further initialization.
 
         Raises:
             ValueError: If the input data format is invalid.
 
         """
-        is_multivariate_data = False
-        if isinstance(self.input_data, tuple):
-            X, y = self.input_data[0], self.input_data[1]
-            features, is_multivariate_data, target = self.__check_features_and_target(X, y)
+        # is_multivariate_data = False
+
+        if self.data_convertor.is_tuple:
+            features, is_multivariate_data, target = self.__check_features_and_target(self.input_data[0],
+                                                                                      self.input_data[1])
+        else:
+            features, is_multivariate_data, target = self.__check_features_and_target(self.input_data.features,
+                                                                                      self.input_data.target)
 
         if self.label_encoder is None and self.task == 'classification':
-            if type(y[0]) is np.str_:
+            # x, y = self.input_data.features, self.input_data.target
+            if type(target[0]) is np.str_:
                 self.label_encoder = LabelEncoder()
                 target = self.label_encoder.fit_transform(target)
-            else:
-                self.label_encoder = self.label_encoder
+            # else:
+            #     self.label_encoder = self.label_encoder
+
         if is_multivariate_data:
-            self.input_data = InputData(idx=np.arange(len(X)),
+            self.input_data = InputData(idx=np.arange(len(features)),
                                         features=features,
                                         target=target,
                                         task=self.task_dict[self.task],
                                         data_type=DataTypesEnum.image)
         elif self.task == 'ts_forecasting':
-            if type(self.input_data) is pd.DataFrame:
-                features_array = np.array(self.input_data.values)
-            ts_task = self.task_dict[self.task]
-            ts_task.task_params = self.task_params
+            features_array = self.data_convertor.convert_to_1d_array()
+            task = Task(TaskTypesEnum.ts_forecasting,
+                        TsForecastingParams(forecast_length=self.task_params['forecast_length']))
+            if self.industrial_task_params is None:
+                features_array = features_array[:-self.task_params['forecast_length']]
+                target = features_array
             self.input_data = InputData.from_numpy_time_series(
                 features_array=features_array,
-                task=ts_task)
+                target_array=target,
+                task=task
+            )
         else:
-            self.input_data = InputData(idx=np.arange(len(X)),
-                                        features=X,
+            self.input_data = InputData(idx=np.arange(len(features)),
+                                        features=features,
                                         target=target,
                                         task=self.task_dict[self.task],
                                         data_type=DataTypesEnum.image)
 
     def _check_input_data_features(self):
         """Checks and preprocesses the features in the input data.
 
@@ -108,16 +122,17 @@
         - Converts features to torch format using NumpyConverter.
 
         """
         self.input_data.features = np.where(
             np.isnan(self.input_data.features), 0, self.input_data.features)
         self.input_data.features = np.where(
             np.isinf(self.input_data.features), 0, self.input_data.features)
-        self.input_data.features = NumpyConverter(
-            data=self.input_data.features).convert_to_torch_format()
+        if self.task != 'ts_forecasting':
+            self.input_data.features = NumpyConverter(
+                data=self.input_data.features).convert_to_torch_format()
 
     def _check_input_data_target(self):
         """Checks and preprocesses the features in the input data.
 
         - Replaces NaN and infinite values with 0.
         - Converts features to torch format using NumpyConverter.
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/api/utils/data.py` & `fedot_ind-0.4.2/fedot_ind/api/utils/data.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/api/utils/metafeatures.py` & `fedot_ind-0.4.2/fedot_ind/api/utils/metafeatures.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/api/utils/path_lib.py` & `fedot_ind-0.4.2/fedot_ind/api/utils/path_lib.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/api/utils/recurrent_image.py` & `fedot_ind-0.4.2/fedot_ind/api/utils/recurrent_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
                   'stride': 1,
                   'image_mode': True}
         recur = RecurrenceExtractor(params)
         output = recur.transform(input_data)
 
         for idx, image in enumerate(output.predict):
             image_mode = 'L' if len(image.shape) == 2 else 'RGB'
-            Image.fromarray(image, mode=image_mode).save(f'{path_to_save}/{output.target[idx][0]}/image_{idx}.png')
+            Image.fromarray(image, mode=image_mode).save(
+                f'{path_to_save}/{output.target[idx][0]}/image_{idx}.png')
 
     # for cls in np.unique(input_data.target):
     #     fig, axs = plt.subplots(len(windows), len(strides), figsize=(20, 20))
     #     fig.suptitle(f'{dataset_name}, class {cls}', fontsize=40)
     #     for window_idx, window in enumerate(windows):
     #         for stride_idx, stride in enumerate(strides):
     #             params = {'window_size': window,
@@ -58,14 +59,16 @@
     #
     # plt.tight_layout()
     # if save:
     #     plt.savefig(f'{dataset_name}_recurrence_matrix.png')
     # if show:
     #     plt.show()
 
+
 def show_class_balance(target):
     plt.hist(target, bins=len(np.unique(target)))
     plt.show()
 
+
 if __name__ == '__main__':
     ds = 'Epilepsy'
     plot_recurrence_matrix(dataset_name=ds)
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/api/utils/saver_collections.py` & `fedot_ind-0.4.2/fedot_ind/api/utils/saver_collections.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/abstraction/decorators.py` & `fedot_ind-0.4.2/fedot_ind/core/architecture/abstraction/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+from weakref import WeakValueDictionary
+
 from distributed import Client, LocalCluster
 from fedot.core.data.data import InputData
 from fedot.core.repository.dataset_types import DataTypesEnum
 
 from fedot_ind.core.architecture.preprocessing.data_convertor import CustomDatasetCLF, CustomDatasetTS, DataConverter, \
     TensorConverter
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
 
-from weakref import WeakValueDictionary
-
 
 def fedot_data_type(func):
     def decorated_func(self, *args):
         if type(args[0]) is not InputData:
             args[0] = DataConverter(data=args[0])
         features = args[0].features
 
@@ -102,16 +102,14 @@
 
 
 class Singleton(type):
     _instances = WeakValueDictionary()
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
-            # This variable declaration is required to force a
-            # strong reference on the instance.
             instance = super(Singleton, cls).__call__(*args, **kwargs)
             cls._instances[cls] = instance
         return cls._instances[cls]
 
 
 class DaskServer(metaclass=Singleton):
     def __init__(self):
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/abstraction/сheckers.py` & `fedot_ind-0.4.2/fedot_ind/core/architecture/abstraction/сheckers.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/pipelines/abstract_pipeline.py` & `fedot_ind-0.4.2/fedot_ind/core/architecture/pipelines/abstract_pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/pipelines/anomaly_detection.py` & `fedot_ind-0.4.2/fedot_ind/core/architecture/pipelines/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/pipelines/classification.py` & `fedot_ind-0.4.2/fedot_ind/core/architecture/pipelines/classification.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/optimisation_history.py` & `fedot_ind-0.4.2/fedot_ind/core/architecture/postprocessing/optimisation_history.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/results_picker.py` & `fedot_ind-0.4.2/fedot_ind/core/architecture/postprocessing/results_picker.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/ucr_datasets.json` & `fedot_ind-0.4.2/fedot_ind/core/architecture/postprocessing/ucr_datasets.json`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/postprocessing/visualisation/gradcam_vis.py` & `fedot_ind-0.4.2/fedot_ind/core/architecture/postprocessing/visualisation/gradcam_vis.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/preprocessing/data_convertor.py` & `fedot_ind-0.4.2/fedot_ind/core/architecture/preprocessing/data_convertor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from functools import partial
 from inspect import signature
 
 import pandas as pd
 import torch
 import torch.nn as nn
+from fedot import Fedot
 from fedot.core.data.data import InputData, OutputData
+from fedot.core.data.multi_modal import MultiModalData
+from fedot.core.pipelines.pipeline import Pipeline
 from fedot.core.repository.dataset_types import DataTypesEnum
 from fedot.core.repository.tasks import Task, TaskTypesEnum
 from pymonad.list import ListMonad
 from sklearn.preprocessing import LabelEncoder
 
 from fedot_ind.api.utils.data import check_multivariate_data
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
@@ -116,17 +119,17 @@
                                    data_type=MATRIX)
         return input_data
 
     def convert_to_output_data(self,
                                prediction,
                                predict_data,
                                output_data_type):
-        if type(prediction) is OutputData:
+        if isinstance(prediction, OutputData):
             output_data = prediction
-        elif type(prediction) is list:
+        elif isinstance(prediction, list):
             output_data = prediction[0]
             target = NumpyConverter(
                 data=np.concatenate([p.target for p in prediction], axis=0)).convert_to_torch_format()
             predict = NumpyConverter(
                 data=np.concatenate([p.predict for p in prediction], axis=0)).convert_to_torch_format()
             output_data = OutputData(idx=predict_data.idx,
                                      features=predict_data.features,
@@ -160,25 +163,33 @@
 
     def convert_to_industrial_composing_format(self, mode):
         if mode == 'one_dimensional':
             new_features, new_target = [
                 array.reshape(array.shape[0], array.shape[1] * array.shape[2])
                 if array is not None and len(array.shape) > 2 else array
                 for array in [self.input_data.features, self.input_data.target]]
+            # if new_features.shape[0] != new_target.shape[0]:
+            #     min_samples = min(new_features.shape[0], new_target.shape[0])
+            #     new_features, new_target = new_features[:min_samples], new_target[:min_samples]
             input_data = InputData(idx=self.input_data.idx,
                                    features=new_features,
                                    target=new_target,
                                    task=self.input_data.task,
                                    data_type=self.input_data.data_type,
                                    supplementary_data=self.input_data.supplementary_data)
         elif mode == 'channel_independent':
-            if len(self.input_data.features.shape) == 1:
-                self.input_data.features = self.input_data.features.reshape(1, -1)
+            feats = self.input_data.features
             flat_input = self.input_data.features.shape[0] == 1
-            feats = self.input_data.features if flat_input else self.input_data.features.swapaxes(1, 0)
+            if len(self.input_data.features.shape) == 1:
+                feats = self.input_data.features.reshape(1, -1)
+            elif len(self.input_data.features.shape) == 3 and self.input_data.features.shape[0] == 1:
+                feats = self.input_data.features.reshape(self.input_data.features.shape[1],
+                                                         1 * self.input_data.features.shape[2])
+            elif not flat_input:
+                feats = self.input_data.features.swapaxes(1, 0)
             input_data = [InputData(idx=self.input_data.idx,
                                     features=features,
                                     target=self.input_data.target,
                                     task=self.input_data.task,
                                     data_type=self.input_data.data_type,
                                     supplementary_data=self.input_data.supplementary_data) for features in
                           feats]
@@ -196,20 +207,26 @@
 
 
 class TensorConverter:
     def __init__(self, data):
         self.tensor_data = self.convert_to_tensor(data)
 
     def convert_to_tensor(self, data):
+        if isinstance(data, tuple):
+            data = data[0]
+
         if isinstance(data, torch.Tensor):
             return data
         elif isinstance(data, np.ndarray):
             return torch.from_numpy(data)
         elif isinstance(data, pd.DataFrame):
-            return torch.from_numpy(data.values)
+            if data.values.dtype == object:
+                return torch.from_numpy(np.array(data.values.tolist()).astype(float))
+            else:
+                return torch.from_numpy(data.values)
         elif isinstance(data, InputData):
             return torch.from_numpy(data.features)
         else:
             print(f"Can't convert {type(data)} to torch.Tensor", Warning)
 
     def convert_to_1d_tensor(self):
         if self.tensor_data.ndim == 1:
@@ -244,14 +261,17 @@
         self.numpy_data = self.convert_to_array(data)
         self.numpy_data = np.where(
             np.isnan(self.numpy_data), 0, self.numpy_data)
         self.numpy_data = np.where(
             np.isinf(self.numpy_data), 0, self.numpy_data)
 
     def convert_to_array(self, data):
+        if isinstance(data, tuple):
+            data = data[0]
+
         if isinstance(data, np.ndarray):
             return data
         elif isinstance(data, torch.Tensor):
             return data.detach().numpy()
         elif isinstance(data, pd.DataFrame):
             return data.values
         elif isinstance(data, InputData):
@@ -317,18 +337,18 @@
                                            1)
         elif self.numpy_data.ndim == 2 and self.numpy_data.shape[0] != 1:
             # add 1 channel
             return self.numpy_data.reshape(self.numpy_data.shape[0],
                                            1,
                                            self.numpy_data.shape[1])
         elif self.numpy_data.ndim == 2 and self.numpy_data.shape[0] == 1:
-            # add transpose data to (features, channel = 1 , sample = 1)
-            return self.numpy_data.reshape(self.numpy_data.shape[1],
+            # add 1 channel
+            return self.numpy_data.reshape(1,
                                            1,
-                                           self.numpy_data.shape[0])
+                                           self.numpy_data.shape[1])
 
         elif self.numpy_data.ndim > 3:
             return self.numpy_data.squeeze()
         assert False, print(
             f'Please, review input dimensions {self.numpy_data.ndim}')
 
     def convert_to_ts_format(self):
@@ -338,31 +358,33 @@
             return self.numpy_data
 
 
 class ConditionConverter:
     def __init__(self, train_data, operation_implementation, mode):
         self.train_data = train_data
         self.operation_implementation = operation_implementation
+        self.operation_example = operation_implementation[0] if isinstance(operation_implementation, list) \
+            else operation_implementation
         self.mode = mode
 
     @property
     def have_transform_method(self):
-        return 'transform' in dir(self.operation_implementation)
+        return 'transform' in dir(self.operation_example)
 
     @property
     def have_fit_method(self):
-        return 'fit' in dir(self.operation_implementation)
+        return 'fit' in dir(self.operation_example)
 
     @property
     def have_predict_method(self):
-        return 'predict' in dir(self.operation_implementation)
+        return 'predict' in dir(self.operation_example)
 
     @property
     def have_predict_for_fit_method(self):
-        return 'predict_for_fit' in dir(self.operation_implementation)
+        return 'predict_for_fit' in dir(self.operation_example)
 
     @property
     def is_one_dim_operation(self):
         return self.mode == 'one_dimensional'
 
     @property
     def is_channel_independent_operation(self):
@@ -378,59 +400,110 @@
 
     @property
     def is_operation_is_list_container(self):
         return type(self.operation_implementation) is list
 
     @property
     def have_predict_atr(self):
-        return 'predict' in vars(self.operation_implementation[0]) if self.is_operation_is_list_container else False
+        return 'predict' in vars(self.operation_example) if self.is_operation_is_list_container else False
 
     @property
     def is_fit_input_fedot(self):
-        return str(list(signature(self.operation_implementation.fit).parameters.keys())[0]) == 'input_data'
+        return str(list(signature(self.operation_example.fit).parameters.keys())[0]) == 'input_data'
 
     @property
     def is_transform_input_fedot(self):
-        return str(list(signature(self.operation_implementation.transform).parameters.keys())[0]) == 'input_data'
+        return str(list(signature(self.operation_example.transform).parameters.keys())[0]) == 'input_data'
 
     @property
     def is_predict_input_fedot(self):
-        return str(list(signature(self.operation_implementation.predict).parameters.keys())[0]) == 'input_data'
+        return str(list(signature(self.operation_example.predict).parameters.keys())[0]) == 'input_data'
 
     @property
     def is_regression_of_forecasting_task(self):
         return self.train_data.task.task_type.value in ['regression', 'ts_forecasting']
 
     @property
     def is_multi_output_target(self):
-        return isinstance(self.operation_implementation.classes_, list)
+        return isinstance(self.operation_example.classes_, list)
+
+    @property
+    def solver_is_fedot_class(self):
+        return isinstance(self.operation_example, Fedot)
+
+    @property
+    def solver_is_none(self):
+        return self.operation_example is None
 
     def output_mode_converter(self, output_mode, n_classes):
         if output_mode == 'labels':
-            return self.operation_implementation.predict(self.train_data.features).reshape(-1, 1)
+            return self.operation_example.predict(self.train_data.features).reshape(-1, 1)
         else:
             return self.probs_prediction_converter(output_mode, n_classes)
 
     def probs_prediction_converter(self, output_mode, n_classes):
         try:
-            prediction = self.operation_implementation.predict_proba(self.train_data.features)
+            prediction = self.operation_example.predict_proba(
+                self.train_data.features)
         except Exception:
-            prediction = self.operation_implementation.predict_proba(self.train_data.features.T)
+            prediction = self.operation_example.predict_proba(
+                self.train_data.features.T)
         if n_classes < 2:
             raise ValueError(
                 'Data set contain only 1 target class. Please reformat your data.')
         elif n_classes == 2 and output_mode != 'full_probs':
             if self.is_multi_output_target:
                 prediction = np.stack([pred[:, 1]
                                        for pred in prediction]).T
             else:
                 prediction = prediction[:, 1]
         return prediction
 
 
+class ApiConverter:
+
+    @staticmethod
+    def solver_is_fedot_class(operation_implementation):
+        return isinstance(operation_implementation, Fedot)
+
+    @staticmethod
+    def solver_is_none(operation_implementation):
+        return operation_implementation is None
+
+    @staticmethod
+    def solver_is_pipeline_class(operation_implementation):
+        return isinstance(operation_implementation, Pipeline)
+
+    @staticmethod
+    def solver_is_dict(operation_implementation):
+        return isinstance(operation_implementation, dict)
+
+    @staticmethod
+    def tuning_params_is_none(tuning_params):
+        return {} if tuning_params is None else tuning_params
+
+    @staticmethod
+    def ensemble_mode(predict_mode):
+        return predict_mode == 'RAF_ensemble'
+
+    @staticmethod
+    def solver_have_target_encoder(encoder):
+        return encoder is not None
+
+    @staticmethod
+    def input_data_is_fedot_type(input_data):
+        return isinstance(input_data, (InputData, MultiModalData))
+
+    def is_multiclf_with_labeling_problem(self, problem, target, predict):
+        clf_problem = problem == 'classification'
+        uncorrect_labels = target.min() - predict.min() != 0
+        multiclass = len(np.unique(predict).shape) != 1
+        return clf_problem and uncorrect_labels and multiclass
+
+
 class DataConverter(TensorConverter, NumpyConverter):
     def __init__(self, data):
         super().__init__(data)
         self.data = data
         self.numpy_data = self.convert_to_array(data)
 
     @property
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/settings/computational.py` & `fedot_ind-0.4.2/fedot_ind/core/architecture/settings/computational.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/architecture/settings/pipeline_factory.py` & `fedot_ind-0.4.2/fedot_ind/core/architecture/settings/pipeline_factory.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/ensemble/base_ensembler.py` & `fedot_ind-0.4.2/fedot_ind/core/ensemble/base_ensembler.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/ensemble/random_automl_forest.py` & `fedot_ind-0.4.2/fedot_ind/core/ensemble/random_automl_forest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from copy import deepcopy
 
 from fedot.core.data.data import InputData
 from fedot.core.data.multi_modal import MultiModalData
 from fedot.core.pipelines.pipeline import Pipeline
 from fedot.core.pipelines.pipeline_builder import PipelineBuilder
 from fedot.core.repository.dataset_types import DataTypesEnum
-from sklearn.model_selection import StratifiedKFold, StratifiedGroupKFold, train_test_split
+
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
-from fedot_ind.core.repository.constanst_repository import FEDOT_ATOMIZE_OPERATION, FEDOT_HEAD_ENSEMBLE, FEDOT_TASK, \
-    FEDOT_ENSEMBLE_ASSUMPTIONS
+from fedot_ind.core.repository.constanst_repository import FEDOT_ATOMIZE_OPERATION, FEDOT_HEAD_ENSEMBLE, FEDOT_TASK
 from fedot_ind.core.repository.model_repository import SKLEARN_CLF_MODELS, SKLEARN_REG_MODELS
 
 
 class RAFensembler:
     """Class for ensemble of random automl forest
 
     Args:
@@ -56,15 +55,16 @@
 
     def fit(self, train_data):
         if self.n_splits is None:
             self.n_splits = round(
                 train_data.features.shape[0] / self.batch_size)
         new_features = np.array_split(train_data.features, self.n_splits)
         new_target = np.array_split(train_data.target, self.n_splits)
-        self.current_pipeline = self.ensemble_method(new_features, new_target, n_splits=self.n_splits)
+        self.current_pipeline = self.ensemble_method(
+            new_features, new_target, n_splits=self.n_splits)
         self._decompose_pipeline()
 
     def predict(self, test_data, output_mode: str = 'labels'):
         return self.current_pipeline.predict(test_data, output_mode).predict
 
     def _raf_ensemble(self, features, target, n_splits):
         raf_ensemble = PipelineBuilder()
@@ -83,11 +83,12 @@
             data_dict.update({f'data_source_img/{i}': train_fold})
         train_multimodal = MultiModalData(data_dict)
         head_automl_params = deepcopy(self.atomized_automl_params)
         head_automl_params['available_operations'] = [operation for operation
                                                       in head_automl_params['available_operations']
                                                       if operation in list(SKLEARN_CLF_MODELS.keys())
                                                       or operation in list(SKLEARN_REG_MODELS.keys())]
-        #head_automl_params['initial_assumption'] = FEDOT_ENSEMBLE_ASSUMPTIONS[self.atomized_automl_params['problem']].build()
+        # head_automl_params['initial_assumption'] = FEDOT_ENSEMBLE_ASSUMPTIONS[self.atomized_automl_params[
+        # 'problem']].build()
         raf_ensemble = raf_ensemble.join_branches(self.head).build()
         raf_ensemble.fit(input_data=train_multimodal)
         return raf_ensemble
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/ensemble/rank_ensembler.py` & `fedot_ind-0.4.2/fedot_ind/core/ensemble/rank_ensembler.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/metrics/evaluation.py` & `fedot_ind-0.4.2/fedot_ind/core/metrics/evaluation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/metrics/loss/basis_loss.py` & `fedot_ind-0.4.2/fedot_ind/core/metrics/loss/basis_loss.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/metrics/loss/soft_dtw.py` & `fedot_ind-0.4.2/fedot_ind/core/metrics/loss/soft_dtw.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/metrics/loss/svd_loss.py` & `fedot_ind-0.4.2/fedot_ind/core/metrics/loss/svd_loss.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/metrics/metrics_implementation.py` & `fedot_ind-0.4.2/fedot_ind/core/metrics/metrics_implementation.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,17 @@
                              log_loss, mean_absolute_error,
                              mean_absolute_percentage_error,
                              mean_squared_error, mean_squared_log_error,
                              precision_score, r2_score, roc_auc_score)
 from sklearn.metrics import d2_absolute_error_score, explained_variance_score, max_error, median_absolute_error
 
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
+from sktime.performance_metrics.forecasting import mean_absolute_scaled_error
+
+import numpy as np
 
 
 class ParetoMetrics:
     def pareto_metric_list(self, costs: Union[list, np.ndarray], maximise: bool = True) -> np.ndarray:
         """ Calculates the pareto front for a list of costs.
 
         Args:
@@ -35,15 +38,16 @@
         return is_efficient
 
 
 class QualityMetric:
     def __init__(self, target,
                  predicted_labels,
                  predicted_probs=None,
-                 metric_list: list = ('f1', 'roc_auc', 'accuracy', 'logloss', 'precision'),
+                 metric_list: list = (
+                     'f1', 'roc_auc', 'accuracy', 'logloss', 'precision'),
                  default_value: float = 0.0):
         self.predicted_probs = predicted_probs
         if len(predicted_labels.shape) >= 2:
             self.predicted_labels = np.argmax(predicted_labels, axis=1)
         else:
             self.predicted_labels = np.array(predicted_labels).flatten()
         self.target = np.array(target).flatten()
@@ -163,14 +167,22 @@
 class Accuracy(QualityMetric):
     output_mode = 'labels'
 
     def metric(self) -> float:
         return accuracy_score(y_true=self.target, y_pred=self.predicted_labels)
 
 
+def mase(A, F, y_train):
+    return mean_absolute_scaled_error(A, F, y_train=y_train)
+
+
+def smape(a, f, _=None):
+    return 1 / len(a) * np.sum(2 * np.abs(f - a) / (np.abs(a) + np.abs(f)) * 100)
+
+
 def calculate_regression_metric(target,
                                 labels,
                                 rounding_order=3,
                                 metric_names=('r2', 'rmse', 'mae'),
                                 **kwargs):
     target = target.astype(float)
 
@@ -190,14 +202,39 @@
 
     df = pd.DataFrame({name: func(target, labels) for name, func in metric_dict.items()
                        if name in metric_names},
                       index=[0])
     return df.round(rounding_order)
 
 
+def calculate_forecasting_metric(target,
+                                 labels,
+                                 rounding_order=3,
+                                 metric_names=('smape', 'rmse',
+                                               'median_absolute_error'),
+                                 **kwargs):
+    target = target.astype(float)
+
+    def rmse(y_true, y_pred):
+        return np.sqrt(mean_squared_error(y_true, y_pred))
+
+    metric_dict = {
+        'rmse': rmse,
+        'mae': mean_absolute_error,
+        'median_absolute_error': median_absolute_error,
+        'smape': smape,
+        'mase': mase
+    }
+
+    df = pd.DataFrame({name: func(target, labels) for name, func in metric_dict.items()
+                       if name in metric_names},
+                      index=[0])
+    return df.round(rounding_order)
+
+
 def calculate_classification_metric(target,
                                     labels,
                                     probs,
                                     rounding_order=3,
                                     metric_names=('f1', 'roc_auc', 'accuracy')):
     metric_dict = {'accuracy': Accuracy,
                    'f1': F1,
@@ -212,30 +249,44 @@
 
 
 def kl_divergence(solution: pd.DataFrame,
                   submission: pd.DataFrame,
                   epsilon: float = 0.001,
                   micro_average: bool = False,
                   sample_weights: pd.Series = None):
-    # Overwrite solution for convenience
+    """
+    Calculates the Kullback-Leibler (KL) divergence between the solution and submission dataframes.
+
+    The KL divergence is a measure of how one probability distribution diverges from a second, expected
+    probability distribution.
+
+    Args:
+        solution (pd.DataFrame): The expected probability distribution.
+        submission (pd.DataFrame): The probability distribution to compare.
+        epsilon (float, optional): A small value to avoid division by zero or log of zero. Defaults to 0.001.
+        micro_average (bool, optional): If True, compute the micro-average (i.e., the total sum for all classes) of
+                                        the KL divergence. If False, compute the macro-average (i.e., the unweighted
+                                        mean for all classes). Defaults to False.
+        sample_weights (pd.Series, optional): An array of weights that are assigned to individual samples.
+                                              If None, then samples are equally weighted. Defaults to None.
+
+    Returns:
+        float: The average KL divergence between the solution and submission dataframes.
+
+    """
+
     for col in solution.columns:
-        # Prevent issue with populating int columns with floats
         if not pd.api.types.is_float_dtype(solution[col]):
             solution[col] = solution[col].astype(float)
 
-        # Clip both the min and max following Kaggle conventions for related metrics like log loss
-        # Clipping the max avoids cases where the loss would be infinite or undefined, clipping the min
-        # prevents users from playing games with the 20th decimal place of predictions.
         submission[col] = np.clip(submission[col], epsilon, 1 - epsilon)
 
         y_nonzero_indices = solution[col] != 0
         solution[col] = solution[col].astype(float)
         solution.loc[y_nonzero_indices, col] = solution.loc[y_nonzero_indices, col] * np.log(
             solution.loc[y_nonzero_indices, col] / submission.loc[y_nonzero_indices, col])
-        # Set the loss equal to zero where y_true equals zero following the scipy convention:
-        # https://docs.scipy.org/doc/scipy/reference/generated/scipy.special.rel_entr.html#scipy.special.rel_entr
         solution.loc[~y_nonzero_indices, col] = 0
 
     if micro_average:
         return np.average(solution.sum(axis=1), weights=sample_weights)
     else:
         return np.average(solution.mean())
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/automl/fedot_implementation.py` & `fedot_ind-0.4.2/fedot_ind/core/models/automl/fedot_implementation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/base_extractor.py` & `fedot_ind-0.4.2/fedot_ind/core/models/base_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import logging
 import math
 from itertools import chain
 from multiprocessing import cpu_count
-from typing import Optional
-import pandas as pd
-import numpy as np
 
 from fedot.core.data.data import InputData
 from fedot.core.operations.operation_parameters import OperationParameters
 from fedot.core.repository.dataset_types import DataTypesEnum
 from joblib import delayed, Parallel
+from typing import Optional
 
 from fedot_ind.api.utils.data import init_input_data
 from fedot_ind.core.architecture.abstraction.decorators import convert_to_input_data
 from fedot_ind.core.metrics.metrics_implementation import *
 from fedot_ind.core.operation.IndustrialCachableOperation import IndustrialCachableOperationImplementation
 from fedot_ind.core.operation.transformation.data.hankel import HankelMatrix
 from fedot_ind.core.repository.constanst_repository import STAT_METHODS, STAT_METHODS_GLOBAL
@@ -157,12 +155,13 @@
             1, -1) for component in multi_ts_stat_features], axis=0)
 
         for index, component in enumerate(multi_ts_stat_features):
             # try:
             #     component.supplementary_data['feature_name'] = [f'{x} for component {index}'
             #                                                     for x in component.supplementary_data['feature_name']]
             # except Exception as ex:
-            component.supplementary_data['feature_name'] = [f'component {index}']
+            component.supplementary_data['feature_name'] = [
+                f'component {index}']
         names = list(chain(*[x.supplementary_data['feature_name']
-                     for x in multi_ts_stat_features]))
+                             for x in multi_ts_stat_features]))
 
         return features, names
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/detection/probalistic/kalman.py` & `fedot_ind-0.4.2/fedot_ind/core/models/detection/probalistic/kalman.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/detection/probalistic/sigma.py` & `fedot_ind-0.4.2/fedot_ind/core/models/detection/probalistic/sigma.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/detection/subspaces/func_pca.py` & `fedot_ind-0.4.2/fedot_ind/core/models/detection/subspaces/func_pca.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/detection/subspaces/sst.py` & `fedot_ind-0.4.2/fedot_ind/core/models/detection/subspaces/sst.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/base_nn_model.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/base_nn_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import copy
 import os
-from typing import Optional
 
 import torch
 import torch.nn.functional as F
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.data.data_split import train_test_data_setup
 from fedot.core.operations.operation_parameters import OperationParameters
 from fedot.core.repository.dataset_types import DataTypesEnum
 from torch import Tensor
 from torch.optim import lr_scheduler
+from typing import Optional
 
 from fedot_ind.core.architecture.abstraction.decorators import convert_inputdata_to_torch_dataset, \
     convert_to_4d_torch_array, fedot_data_type
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
 from fedot_ind.core.models.nn.network_modules.layers.special import adjust_learning_rate, EarlyStopping
 
 
@@ -106,54 +106,54 @@
                                             epochs=self.epochs,
                                             max_lr=self.learning_rate)
         if val_loader is None:
             print('Not enough class samples for validation')
 
         best_model = None
         best_val_loss = float('inf')
-        val_interval = self.get_validation_frequency(self.epochs, self.learning_rate)
+        val_interval = self.get_validation_frequency(
+            self.epochs, self.learning_rate)
 
         for epoch in range(1, self.epochs + 1):
             training_loss = 0.0
             valid_loss = 0.0
             self.model.train()
             total = 0
             correct = 0
             for batch in train_loader:
                 optimizer.zero_grad()
                 inputs, targets = batch
                 output = self.model(inputs)
-                try:
-                    loss = loss_fn()(output, targets.float())
-                except Exception:
-                    loss = loss_fn(output, targets.float())
+                loss = loss_fn(output, targets.float())
                 loss.backward()
                 optimizer.step()
                 training_loss += loss.data.item() * inputs.size(0)
                 total += targets.size(0)
-                correct += (torch.argmax(output, 1) == torch.argmax(targets, 1)).sum().item()
+                correct += (torch.argmax(output, 1) ==
+                            torch.argmax(targets, 1)).sum().item()
 
             accuracy = correct / total
             training_loss /= len(train_loader.dataset)
-            print('Epoch: {}, Accuracy = {}, Training Loss: {:.2f}'.format(epoch, accuracy, training_loss))
+            print('Epoch: {}, Accuracy = {}, Training Loss: {:.2f}'.format(
+                epoch, accuracy, training_loss))
 
             if val_loader is not None and epoch % val_interval == 0:
                 self.model.eval()
                 total = 0
                 correct = 0
                 for batch in val_loader:
                     inputs, targets = batch
                     output = self.model(inputs)
-                    try:
-                        loss = loss_fn()(output, targets.float())
-                    except Exception:
-                        loss = loss_fn(output, targets.float())
+
+                    loss = loss_fn(output, targets.float())
+
                     valid_loss += loss.data.item() * inputs.size(0)
                     total += targets.size(0)
-                    correct += (torch.argmax(output, 1) == torch.argmax(targets, 1)).sum().item()
+                    correct += (torch.argmax(output, 1) ==
+                                torch.argmax(targets, 1)).sum().item()
                 if valid_loss < best_val_loss:
                     best_val_loss = valid_loss
                     best_model = copy.deepcopy(self.model)
 
             early_stopping(training_loss, self.model, './')
             adjust_learning_rate(optimizer, scheduler,
                                  epoch + 1, self.learning_rate, printout=False)
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/explainable_convolution_model.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/explainable_convolution_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Optional
-
 import torch
 from fastai.callback.hook import *
 from fastai.layers import BatchNorm, LinBnDrop, SigmoidRange
 from fastai.torch_core import Module
 from fedot.core.operations.operation_parameters import OperationParameters
 from torch import nn, optim
+from typing import Optional
 
 from fedot_ind.core.architecture.abstraction.decorators import convert_inputdata_to_torch_dataset
 from fedot_ind.core.architecture.postprocessing.visualisation.gradcam_vis import visualise_gradcam
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
 from fedot_ind.core.architecture.settings.computational import default_device
 from fedot_ind.core.models.nn.network_impl.base_nn_model import BaseNeuralModel
 from fedot_ind.core.models.nn.network_modules.layers.conv_layers import Conv1d, Conv2d
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/inception.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/inception.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,21 +12,16 @@
 from fedot_ind.core.models.nn.network_modules.layers.pooling_layers import GAP1d
 from fedot_ind.core.models.nn.network_modules.layers.special import InceptionBlock, InceptionModule
 from fedot_ind.core.repository.constanst_repository import CROSS_ENTROPY, MULTI_CLASS_CROSS_ENTROPY, RMSE
 
 
 @delegates(InceptionModule.__init__)
 class InceptionTime(Module):
-    def __init__(self,
-                 input_dim,
-                 output_dim,
-                 seq_len=None,
-                 number_of_filters=32,
-                 nb_filters=None,
-                 **kwargs):
+    def __init__(self, input_dim, output_dim, seq_len=None, number_of_filters=32, nb_filters=None, **kwargs):
+        super().__init__()
         if number_of_filters is None:
             number_of_filters = nb_filters
         self.inception_block = InceptionBlock(
             input_dim, number_of_filters, **kwargs)
         self.gap = GAP1d(1)
         self.fc = nn.Linear(number_of_filters * 4, output_dim)
 
@@ -73,19 +68,19 @@
                                    output_dim=self.num_classes).to(default_device())
         self.model_for_inference = InceptionTime(input_dim=ts.features.shape[1],
                                                  output_dim=self.num_classes)
         self._evaluate_num_of_epochs(ts)
         optimizer = optim.Adam(self.model.parameters(), lr=self.learning_rate)
         if ts.task.task_type.value == 'classification':
             if ts.num_classes == 2:
-                loss_fn = CROSS_ENTROPY
+                loss_fn = CROSS_ENTROPY()
             else:
-                loss_fn = MULTI_CLASS_CROSS_ENTROPY
+                loss_fn = MULTI_CLASS_CROSS_ENTROPY()
         else:
-            loss_fn = RMSE
+            loss_fn = RMSE()
         return loss_fn, optimizer
 
     def _fit_model(self, ts: InputData, split_data: bool = False):
         loss_fn, optimizer = self._init_model(ts)
         train_loader, val_loader = self._prepare_data(ts, split_data)
 
         self._train_loop(
@@ -97,8 +92,7 @@
 
     @convert_to_3d_torch_array
     def _predict_model(self, x_test, output_mode: str = 'default'):
         self.model.eval()
         x_test = Tensor(x_test).to(default_device('cpu'))
         pred = self.model(x_test)
         return self._convert_predict(pred, output_mode)
-
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/mini_rocket.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/mini_rocket.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import OrderedDict
-from typing import Optional
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.operations.operation_parameters import OperationParameters
 from fedot.core.repository.dataset_types import DataTypesEnum
+from typing import Optional
 
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
 from fedot_ind.core.architecture.settings.computational import default_device
 from fedot_ind.core.models.base_extractor import BaseExtractor
 
 
 class MiniRocketFeatures(nn.Module):
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/omni_scale.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/omni_scale.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/patch_tst.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/patch_tst.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,14 @@
                          patch_len=self.patch_len,
                          preprocess_to_lagged=self.preprocess_to_lagged,
                          activation=self.activation).to(default_device())
         optimizer = optim.Adam(model.parameters(), lr=self.learning_rate)
         patch_pred_len = round(self.horizon / 4)
         loss_fn = EXPONENTIAL_WEIGHTED_LOSS(
             time_steps=patch_pred_len, tolerance=0.3)
-        # loss_fn = RMSE()
         return model, loss_fn, optimizer
 
     def _fit_model(self, input_data: InputData, split_data: bool = True):
         if self.preprocess_to_lagged:
             self.patch_len = input_data.features.shape[1]
             train_loader = self.__create_torch_loader(input_data)
         else:
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/resnet.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/resnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,19 +130,19 @@
         self.model_for_inference = ResNet(input_dim=ts.features.shape[1],
                                           output_dim=self.num_classes,
                                           model_name=self.model_name).model
         self.model = self.model.model
         optimizer = optim.Adam(self.model.parameters(), lr=0.001)
         if ts.task.task_type.value == 'classification':
             if ts.num_classes == 2:
-                loss_fn = CROSS_ENTROPY
+                loss_fn = CROSS_ENTROPY()
             else:
-                loss_fn = MULTI_CLASS_CROSS_ENTROPY
+                loss_fn = MULTI_CLASS_CROSS_ENTROPY()
         else:
-            loss_fn = RMSE
+            loss_fn = RMSE()
         return loss_fn, optimizer
 
     @convert_to_4d_torch_array
     def _predict_model(self, x_test):
         self.model.eval()
         x_test = Tensor(x_test).to(default_device())
         pred = self.model(x_test)
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/transformer.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/transformer.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_impl/tst.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_impl/tst.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/activation.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/activation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/attention_layers.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/attention_layers.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/backbone.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/backbone.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/conv_layers.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/conv_layers.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/head_layers.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/head_layers.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/linear_layers.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/linear_layers.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/padding_layers.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/padding_layers.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/pooling_layers.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/layers/special.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/layers/special.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/losses.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             loss (torch.Tensor): loss.
             loss_normalized (torch.Tensor): loss, where regularization parameters are 1.
         """
         # res = torch.sum(input ** 2, dim=0).reshape(self.n_t, -1)
         res = torch.mean(input_, axis=0).reshape(self.n_t, -1)
         target = torch.mean(target, axis=0).reshape(self.n_t, -1)
         m = torch.triu(torch.ones((self.n_t, self.n_t),
-                       dtype=res.dtype), diagonal=1).T.to(default_device())
+                                  dtype=res.dtype), diagonal=1).T.to(default_device())
         with torch.no_grad():
             w = torch.exp(- self.tol * (m @ res))
         loss = torch.mean(w * res)
         loss = torch.mean(torch.sqrt((loss - target) ** 2).flatten())
         return loss
 
 
@@ -89,15 +89,15 @@
         super().__init__()
 
     def forward(self, input: Tensor, target: Tensor) -> Tensor:
         diff = input - target
         abs_diff = torch.abs(diff)
         mask = abs_diff < self.delta
         loss = torch.cat([(.5 * diff[mask] ** 2), self.delta *
-                         (abs_diff[~mask] - (.5 * self.delta))])
+                          (abs_diff[~mask] - (.5 * self.delta))])
         if self.reduction == 'mean':
             return loss.mean()
         elif self.reduction == 'sum':
             return loss.sum()
         else:
             return loss
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/nn/network_modules/other.py` & `fedot_ind-0.4.2/fedot_ind/core/models/nn/network_modules/other.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/quantile/quantile_extractor.py` & `fedot_ind-0.4.2/fedot_ind/core/models/quantile/quantile_extractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/quantile/stat_features.py` & `fedot_ind-0.4.2/fedot_ind/core/models/quantile/stat_features.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/recurrence/reccurence_extractor.py` & `fedot_ind-0.4.2/fedot_ind/core/models/recurrence/reccurence_extractor.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/recurrence/sequences.py` & `fedot_ind-0.4.2/fedot_ind/core/models/recurrence/sequences.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,25 +111,25 @@
                     np.log(distribution[i] / sum_frequency_distribution)
         return -entropy_lines
 
     def laminarity_or_determinism(self, factor, number_of_vectors, distribution, lam: bool):
         if lam:
             number_of_vectors = number_of_vectors + 1
         numerator = np.sum([i * distribution[i]
-                           for i in range(factor, number_of_vectors)])
+                            for i in range(factor, number_of_vectors)])
         denominator = np.sum([i * distribution[i]
-                             for i in range(1, number_of_vectors)])
+                              for i in range(1, number_of_vectors)])
         return numerator / denominator
 
     def longest_line_length(self, frequency_distribution, number_of_vectors, diag: bool):
         longest_line_length = 1
         for i in range(number_of_vectors, 0, -1):
             if frequency_distribution[i] != 0:
                 return i
         return longest_line_length
 
     def average_line_length(self, factor, number_of_vectors, distribution):
         numerator = np.sum([i * distribution[i]
-                           for i in range(factor, number_of_vectors + 1)])
+                            for i in range(factor, number_of_vectors + 1)])
         denominator = np.sum([distribution[i]
-                             for i in range(factor, number_of_vectors + 1)])
+                              for i in range(factor, number_of_vectors + 1)])
         return numerator / denominator
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/topological/topofeatures.py` & `fedot_ind-0.4.2/fedot_ind/core/models/topological/topofeatures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# -*- coding: utf-8 -*-
-
 from abc import ABC
 from multiprocessing.dummy import Pool as ThreadPool
 
-from fedot_ind.core.architecture.settings.computational import backend_methods as np
 import pandas as pd
 from gtda.diagrams import BettiCurve, Filtering, PersistenceEntropy, PersistenceLandscape, Scaler
 from gtda.homology import VietorisRipsPersistence
 
+from fedot_ind.core.architecture.settings.computational import backend_methods as np
+
 
 class PersistenceDiagramFeatureExtractor(ABC):
     """Abstract class persistence diagrams features extractor.
 
     """
 
     def extract_feature_(self, persistence_diagram):
@@ -264,10 +263,10 @@
         super(RadiusAtMaxBNFeature).__init__()
 
     def extract_feature_(self, persistence_diagram, n_bins=100):
         betti_curve = BettiCurve(
             n_jobs=-1, n_bins=n_bins).fit_transform([persistence_diagram])[0]
         max_dim = int(np.max(persistence_diagram[:, 2])) + 1
         max_bettis = np.array([np.max(betti_curve[i, :])
-                              for i in range(max_dim)])
+                               for i in range(max_dim)])
         return np.array(
             [np.where(betti_curve[i, :] == max_bettis[i])[0][0] / (n_bins * max_dim) for i in range(max_dim)])
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/topological/topological_extractor.py` & `fedot_ind-0.4.2/fedot_ind/core/models/topological/topological_extractor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 from functools import partial
-from typing import Optional
 
 import pandas as pd
 from fedot.core.data.data import InputData
 from fedot.core.operations.operation_parameters import OperationParameters
 from fedot.core.repository.dataset_types import DataTypesEnum
 from gtda.time_series import takens_embedding_optimal_parameters
 from scipy import stats
 from tqdm import tqdm
+from typing import Optional
 
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
 from fedot_ind.core.models.base_extractor import BaseExtractor
 from fedot_ind.core.models.topological.topofeatures import PersistenceDiagramsExtractor, TopologicalFeaturesExtractor
 from fedot_ind.core.operation.transformation.data.point_cloud import TopologicalTransformation
 from fedot_ind.core.repository.constanst_repository import PERSISTENCE_DIAGRAM_EXTRACTOR, \
     PERSISTENCE_DIAGRAM_FEATURES
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/models/ts_forecasting/ssa_forecaster.py` & `fedot_ind-0.4.2/fedot_ind/core/models/ts_forecasting/ssa_forecaster.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,16 @@
                          'tuner': SimultaneousTuner}
         component_mode_dict = {
             'topological': PipelineBuilder().add_node('lagged').add_node('topological_features').add_node('treg'),
             'ar': PipelineBuilder().add_node('ar')}
 
         self.window_size_method = params.get('window_size_method')
         self.history_lookback = max(params.get('history_lookback', 0), 100)
-        self.low_rank_approximation = params.get('low_rank_approximation', False)
+        self.low_rank_approximation = params.get(
+            'low_rank_approximation', False)
         self.tuning_params = params.get('tuning_params', tuning_params)
         self.component_model = params.get('component_model', 'topological')
         self.mode = params.get('mode', 'channel_independent')
         self.component_model = component_mode_dict[self.component_model]
         self.trend_model = PipelineBuilder().add_node('lagged').add_node('ridge')
         self.trend_model = self.component_model
         self._decomposer = None
@@ -75,29 +76,31 @@
         self.tuning_params['metric'] = FEDOT_TUNING_METRICS['regression']
         pipeline_tuner, component_model = build_tuner(self,
                                                       model_to_tune,
                                                       self.tuning_params,
                                                       component,
                                                       'head')
         component_model.fit(component)
-        reconstructed_forecast = component_model.predict(component).predict[-self.horizon:]
+        reconstructed_forecast = component_model.predict(
+            component).predict[-self.horizon:]
         return reconstructed_forecast, component_model
 
     def _combine_trajectory(self, U, VT, n_components):
         if len(self._rank_thr) > 2:
             self.PCT = np.concatenate([U[:, 0].reshape(1, -1),
                                        np.array([np.sum([U[:, i], U[:, i + 1]], axis=0) for i in self._rank_thr if
                                                  i != 0 and i % 2 != 0])]).T
 
             current_dynamics = np.concatenate([VT[0, :].reshape(1, -1),
                                                np.array(
                                                    [np.sum([VT[i, :], VT[i + 1, :]], axis=0) for i in self._rank_thr
                                                     if i != 0 and i % 2 != 0])])
         else:
-            self.PCT, current_dynamics = U[:, :n_components], VT[:n_components, :]
+            self.PCT, current_dynamics = U[:,
+                                           :n_components], VT[:n_components, :]
 
         return current_dynamics
 
     def predict(self, input_data: InputData) -> OutputData:
         hankel_matrix = HankelMatrix(time_series=input_data.features,
                                      window_size=self._decomposer.window_size).trajectory_matrix
         U, s, VT = np.linalg.svd(hankel_matrix)
@@ -106,17 +109,19 @@
 
         if self.mode == 'one_dimensional':
             comp = deepcopy(input_data)
             basis = reconstruct_basis(U=self.PCT,
                                       Sigma=s[:self.PCT.shape[1]],
                                       VT=current_dynamics,
                                       ts_length=input_data.features.shape[0])
-            comp.features, comp.idx = np.array(basis).sum(axis=1), np.arange(np.array(basis).sum(axis=1).shape[0])
+            comp.features, comp.idx = np.array(basis).sum(
+                axis=1), np.arange(np.array(basis).sum(axis=1).shape[0])
 
-            reconstructed_forecast, self.model_by_channel = self._tune_component_model(self.trend_model.build(), comp)
+            reconstructed_forecast, self.model_by_channel = self._tune_component_model(
+                self.trend_model.build(), comp)
         elif self.mode == 'channel_independent':
             forecast_by_channel, self.model_by_channel = self._predict_channel(input_data,
                                                                                current_dynamics,
                                                                                self.horizon)
 
             self.forecasted_dynamics = np.concatenate([current_dynamics,
                                                        np.vstack(list(forecast_by_channel.values()))], axis=1)
@@ -152,15 +157,16 @@
 
     def predict_for_fit(self, input_data: InputData) -> OutputData:
         if self.horizon is None:
             self.horizon = input_data.task.task_params.forecast_length
         if input_data.features.shape[0] > self.history_lookback:
             self.history_lookback = round(input_data.features.shape[0] * 0.2) \
                 if self.history_lookback == 0 else self.history_lookback
-            input_data.features = input_data.features[-self.history_lookback:].squeeze()
+            input_data.features = input_data.features[-self.history_lookback:].squeeze(
+            )
         else:
             self.history_lookback = None
         self._decomposer = EigenBasisImplementation({'low_rank_approximation': self.low_rank_approximation,
                                                      'rank_regularization': 'explained_dispersion'})
         predict = self.__predict_for_fit(input_data)
         return predict
 
@@ -168,16 +174,19 @@
         comp = deepcopy(input_data)
         comp.features, comp.target, comp.idx = component_dynamics, component_dynamics, \
             np.arange(component_dynamics.shape[1])
         forecast_by_channel, model_by_channel = {}, {}
         for index, ts_comp in enumerate(comp.features):
             comp.features = ts_comp
             comp.target = ts_comp
-            model_to_tune = self.component_model.build() if index != 0 else self.trend_model.build()
-            reconstructed_forecast, component_model = self._tune_component_model(model_to_tune, comp)
-            forecast_by_channel.update({f'{index}_channel': reconstructed_forecast})
+            model_to_tune = self.component_model.build(
+            ) if index != 0 else self.trend_model.build()
+            reconstructed_forecast, component_model = self._tune_component_model(
+                model_to_tune, comp)
+            forecast_by_channel.update(
+                {f'{index}_channel': reconstructed_forecast})
             model_by_channel.update({f'{index}_channel': component_model})
 
         return forecast_by_channel, model_by_channel
 
     def reconstruct_basis(self, U, s, VT):
         return Either.insert([U, s, VT]).then(self._decomposer.data_driven_basis).value[0]
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/IndustrialCachableOperation.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/IndustrialCachableOperation.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     def _convert_to_fedot_datatype(self, input_data=None, transformed_features=None):
         if not isinstance(input_data, InputData):
             input_data = InputData(idx=np.arange(len(transformed_features)),
                                    features=transformed_features,
                                    target='no_target',
                                    task='no_task',
                                    data_type=DataTypesEnum.table)
+
         if type(transformed_features) is OutputData:
             transformed_features = transformed_features.predict
 
         predict = OutputData(idx=input_data.idx,
                              features=input_data.features,
                              features_names=input_data.features_names,
                              predict=transformed_features,
@@ -52,14 +53,22 @@
 
     def try_load_from_cache(self, hashed_info: str) -> np.array:
         predict = self.cacher.load_data_from_cache(hashed_info=hashed_info)
         return predict
 
     def transform(self, input_data: InputData, use_cache: bool = False) -> OutputData:
         """Method firstly tries to load result from cache. If unsuccessful, it starts to generate features
+
+        Args:
+            input_data: InputData - data to transform
+            use_cache: bool - whether to use cache or not
+
+        Returns:
+            OutputData - transformed data
+
         """
         if use_cache:
             class_params = {k: v for k, v in self.__dict__.items() if k not in ['cacher',
                                                                                 'data_type',
                                                                                 'params',
                                                                                 'n_processes',
                                                                                 'logging_params',
@@ -75,12 +84,13 @@
                 self.cacher.cache_data(hashed_info, predict)
 
             predict = self._convert_to_output(
                 input_data, predict, data_type=self.data_type)
             return predict
         else:
             transformed_features = self._transform(input_data)
-            predict = self._convert_to_fedot_datatype(input_data, transformed_features)
+            predict = self._convert_to_fedot_datatype(
+                input_data, transformed_features)
             return predict
 
     def _transform(self, input_data):
         pass
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/caching.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/caching.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             Hashed string.
         """
         # key = ''.join([repr(arg) for arg in kwargs.values()]).encode('utf8')
         # key += data.__str__().encode('utf8')
         # hsh = hashlib.md5(key).hexdigest()[:10]
 
         key_info = ''.join([repr(arg)
-                           for arg in kwargs.values()]).encode('utf8')
+                            for arg in kwargs.values()]).encode('utf8')
         key_data = data.__str__()
 
         key = key_info + key_data.encode('utf8')
         hsh = hashlib.md5(key).hexdigest()[:20]
 
         return hsh
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/decomposed_conv.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/decomposition/decomposed_conv.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/matrix_decomposition/column_sampling_decomposition.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/decomposition/matrix_decomposition/column_sampling_decomposition.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/matrix_decomposition/dmd_decomposition.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/decomposition/matrix_decomposition/dmd_decomposition.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/decomposition/matrix_decomposition/power_iteration_decomposition.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/decomposition/matrix_decomposition/power_iteration_decomposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import math
+
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
-from fedot_ind.core.architecture.settings.computational import backend_scipy
+from fedot_ind.core.operation.filtration.channel_filtration import _detect_knee_point
 from fedot_ind.core.operation.transformation.regularization.spectrum import singular_value_hard_threshold, \
     sv_to_explained_variance_ratio
-import math
 
 
 class RSVDDecomposition:
     def __init__(self,
                  rank: int = None
                  ):
         self.rank = rank
@@ -29,53 +30,51 @@
     def _spectrum_regularization(self,
                                  spectrum: np.array,
                                  reg_type: str = 'hard_thresholding'):
         if reg_type == 'explained_dispersion':
             low_rank = sv_to_explained_variance_ratio(spectrum, 3)[1]
         elif reg_type == 'hard_thresholding':
             low_rank = len(singular_value_hard_threshold(spectrum))
-        return low_rank
+        return max(low_rank, 2)
 
     def _matrix_approx_regularization(self, low_rank, Ut, block, tensor):
         if low_rank == 1:
             return low_rank
         else:
             list_of_rank = list(range(1, low_rank + 1, 1))
             reconstr_matrix = [self._compute_matrix_approximation(
                 Ut, block, tensor, rank) for rank in list_of_rank]
-            fro_norms = [abs(np.linalg.norm(tensor - reconstr_m, 'fro')/np.linalg.norm(tensor)*100)
+            fro_norms = [abs(np.linalg.norm(tensor - reconstr_m, 'fro') / np.linalg.norm(tensor) * 100)
                          for reconstr_m in reconstr_matrix]
-            deriviate_of_error = abs(np.diff(fro_norms))
-            regularized_rank = len(
-                deriviate_of_error[deriviate_of_error > 1]) + 1
+            regularized_rank = _detect_knee_point(
+                values=fro_norms, indices=list(range(len(fro_norms))))
+            regularized_rank = len(regularized_rank)
+            # deriviate_of_error = abs(np.diff(fro_norms))
+            # regularized_rank = len(
+            #     deriviate_of_error[deriviate_of_error > 1]) + 1
         return regularized_rank
 
     def rsvd(self,
-             tensor,
+             tensor: np.array,
              approximation: bool = False,
              regularized_rank: int = None,
              reg_type: str = 'hard_thresholding') -> list:
         """Block Krylov subspace method for computing the SVD of a matrix with a low computational cost.
 
         Args:
-            tensor (array (M, N) array_like):
-            k (int): rank of the decomposition
-            block_size (int): size of the block
-            num_iter (int): number of iterations
+            tensor: matrix to decompose
+            approximation: if True, the matrix approximation will be computed
+            regularized_rank: rank of the matrix approximation
+            reg_type: type of regularization. 'hard_thresholding' or 'explained_dispersion'
 
         Returns:
-            u, s, vt (array_like): decomposition
-
-        Notes:
-        :param reg_type:
-        :param regularized_rank:
-        :param approximation:
+            u, s, vt: decomposition
 
         """
-        # Return classic svd decomposition with choosen type of spectrum thresholding
+        # Return classic svd decomposition with chosen type of spectrum thresholding
         if not approximation:
             # classic svd decomposition
             Ut, St, Vt = np.linalg.svd(tensor, full_matrices=False)
             # Compute low rank.
             low_rank = self._spectrum_regularization(St, reg_type=reg_type)
             if regularized_rank is not None:
                 low_rank = regularized_rank
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/dummy/dummy_operation.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/dummy/dummy_operation.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/filtration/feature_filtration.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/filtration/feature_filtration.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/interfaces/fedot_automl_evaluation_strategy.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/interfaces/fedot_automl_evaluation_strategy.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/interfaces/industrial_model_strategy.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/interfaces/industrial_model_strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Optional
 
+import numpy as np
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.operations.evaluation.evaluation_interfaces import EvaluationStrategy
-# from fedot.core.operations.evaluation.operation_implementations.data_operations.sklearn_transformations import *
 from fedot.core.operations.evaluation.time_series import FedotTsForecastingStrategy
 from fedot.core.operations.operation_parameters import OperationParameters
 
 from fedot_ind.core.models.nn.network_impl.patch_tst import PatchTSTModel
 from fedot_ind.core.operation.interfaces.industrial_preprocessing_strategy import \
     (IndustrialCustomPreprocessingStrategy, MultiDimPreprocessingStrategy)
 from fedot_ind.core.repository.model_repository import FORECASTING_MODELS, NEURAL_MODEL, SKLEARN_CLF_MODELS, \
     SKLEARN_REG_MODELS
+from scipy.stats import kurtosis
+from scipy.stats import skew
 
 
 class FedotNNClassificationStrategy(EvaluationStrategy):
     __operations_by_types = NEURAL_MODEL
 
     def _convert_to_operation(self, operation_type: str):
         if operation_type in self.__operations_by_types.keys():
@@ -73,18 +75,15 @@
 
 
 class IndustrialSkLearnEvaluationStrategy(IndustrialCustomPreprocessingStrategy):
 
     def __init__(self, operation_type: str, params: Optional[OperationParameters] = None):
         super().__init__(operation_type, params)
         self.operation_impl = self._convert_to_operation(operation_type)
-        self.multi_dim_dispatcher = MultiDimPreprocessingStrategy(self.operation_impl,
-                                                                  operation_type,
-                                                                  params,
-                                                                  mode='one_dimensional')
+        self.multi_dim_dispatcher.mode = 'one_dimensional'
 
     def fit(self, train_data: InputData):
         train_data = self.multi_dim_dispatcher._convert_input_data(train_data)
         return self.multi_dim_dispatcher.fit(train_data)
 
     def predict(self, trained_operation, predict_data: InputData, output_mode: str = 'default') -> OutputData:
         predict_data = self.multi_dim_dispatcher._convert_input_data(predict_data)
@@ -116,29 +115,40 @@
 
     def predict_for_fit(self, trained_operation, predict_data: InputData, output_mode: str = 'labels') -> OutputData:
         predict_data = self.multi_dim_dispatcher._convert_input_data(predict_data)
         return self.multi_dim_dispatcher.predict_for_fit(trained_operation, predict_data, output_mode='labels')
 
 
 class IndustrialSkLearnForecastingStrategy(IndustrialSkLearnEvaluationStrategy):
-    """ Strategy for applying regression algorithms from Sklearn library """
+    """ Strategy for applying forecasting algorithms """
     _operations_by_types = FORECASTING_MODELS
 
     def __init__(self, operation_type: str, params: Optional[OperationParameters] = None):
         super().__init__(operation_type, params)
+        self.multi_dim_dispatcher.mode = 'channel_independent'
+        self.multi_dim_dispatcher.concat_func = np.vstack
+        self.ensemble_func = np.sum
+
+    def fit(self, train_data: InputData):
+        train_data = self.multi_dim_dispatcher._convert_input_data(train_data)
+        return self.multi_dim_dispatcher.fit(train_data)
 
     def predict(self, trained_operation, predict_data: InputData, output_mode: str = 'labels') -> OutputData:
-        predict_data = self.multi_dim_dispatcher._convert_input_data(
-            predict_data, mode=self.multi_dim_dispatcher.mode)
-        return self.multi_dim_dispatcher.predict(trained_operation, predict_data, output_mode='labels')
+        predict_data = self.multi_dim_dispatcher._convert_input_data(predict_data, mode=self.multi_dim_dispatcher.mode)
+        predict_output = self.multi_dim_dispatcher.predict(trained_operation, predict_data, output_mode='labels')
+        predict_output.predict = self.ensemble_func(predict_output.predict, axis=0)
+        return predict_output
 
     def predict_for_fit(self, trained_operation, predict_data: InputData, output_mode: str = 'labels') -> OutputData:
         predict_data = self.multi_dim_dispatcher._convert_input_data(
             predict_data, mode=self.multi_dim_dispatcher.mode)
-        return self.multi_dim_dispatcher.predict_for_fit(trained_operation, predict_data, output_mode='labels')
+        predict_output = self.multi_dim_dispatcher.predict_for_fit(trained_operation, predict_data,
+                                                                   output_mode='labels')
+        predict_output.predict = self.ensemble_func(predict_output.predict, axis=0)
+        return predict_output
 
 
 class IndustrialCustomRegressionStrategy(IndustrialSkLearnEvaluationStrategy):
     _operations_by_types = SKLEARN_REG_MODELS
 
     def __init__(self, operation_type: str, params: Optional[OperationParameters] = None):
         super().__init__(operation_type, params)
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/interfaces/industrial_preprocessing_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from inspect import signature
 from typing import Optional
 
 import numpy as np
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.operations.evaluation.evaluation_interfaces import convert_to_multivariate_model, EvaluationStrategy, \
     is_multi_output_task
-# from fedot.core.operations.evaluation.operation_implementations.data_operations.sklearn_transformations import \
-#     *
 from fedot.core.operations.operation_parameters import OperationParameters
 from fedot.core.repository.dataset_types import DataTypesEnum
 from fedot.core.repository.operation_types_repository import get_operation_type_from_id, OperationTypesRepository
 from fedot.utilities.random import ImplementationRandomStateHandler
 
 from fedot_ind.core.architecture.preprocessing.data_convertor import ConditionConverter, FedotConverter, NumpyConverter
 from fedot_ind.core.repository.IndustrialOperationParameters import IndustrialOperationParameters
@@ -20,18 +18,20 @@
     INDUSTRIAL_CLF_PREPROC_MODEL, INDUSTRIAL_PREPROC_MODEL
 
 
 class MultiDimPreprocessingStrategy(EvaluationStrategy):
     def __init__(self, operation_impl,
                  operation_type: str,
                  params: Optional[OperationParameters] = None,
-                 mode: str = 'one_dimensional'):
+                 mode: str = 'one_dimensional'
+                 ):
         self.operation_impl = operation_impl
         super().__init__(operation_type, params)
         self.output_mode = 'labels'
+        self.concat_func = np.hstack
         self.mode = mode
 
     @property
     def implementation_info(self) -> str:
         return str(self._convert_to_operation(self.operation_type))
 
     def __convert_input_data(self, input_data):
@@ -44,16 +44,15 @@
     def __operation_multidim_adapter(self, trained_operation, predict_data):
         if not self.operation_condition.is_operation_is_list_container:
             prediction = trained_operation.transform(predict_data) if self.operation_condition.is_transform_input_fedot \
                 else trained_operation.transform(predict_data.features)
         elif self.operation_condition.have_predict_atr and self.operation_condition.is_operation_is_list_container:
             prediction = trained_operation
         else:
-            prediction = self._predict_for_ndim(
-                predict_data, trained_operation)
+            prediction = self._predict_for_ndim(predict_data, trained_operation)
         return prediction
 
     def _convert_to_output(self,
                            prediction,
                            predict_data: InputData,
                            output_data_type: DataTypesEnum = DataTypesEnum.table,
                            output_mode: str = 'default') -> OutputData:
@@ -93,27 +92,30 @@
 
         # check model methods and method input type
 
         if self.operation_condition_for_channel_independent.have_transform_method:
             if self.operation_condition_for_channel_independent.is_transform_input_fedot:
                 prediction = list(operation.transform(
                     data) for operation, data in zip(trained_operation, test_data))
-                prediction = [pred.predict if type(
-                    pred) is not np.ndarray else pred for pred in prediction]
+                if self.operation_type == 'lagged' or self.operation_type == 'sparse_lagged':
+                    prediction = prediction
+                else:
+                    prediction = [pred.predict if type(
+                        pred) is not np.ndarray else pred for pred in prediction]
             else:
                 prediction = list(
                     operation.transform(data.features) for operation, data in zip(trained_operation, test_data))
         elif self.operation_condition_for_channel_independent.have_predict_method:
             prediction = list(operation.predict(data)
                               for operation, data in zip(trained_operation, test_data))
-            prediction = [pred.predict for pred in prediction if type(
-                pred) is not np.array]
 
-        prediction = NumpyConverter(data=np.hstack(
-            prediction)).convert_to_torch_format()
+            prediction = [pred.predict for pred in prediction if type(pred) is not np.array]
+
+        if not isinstance(prediction[0], OutputData):
+            prediction = NumpyConverter(data=self.concat_func(prediction)).convert_to_torch_format()
         return prediction
 
     def _custom_fit(self, train_data):
         operation_implementation = self.operation_impl(self.params_for_fit)
         operation_implementation.fit(train_data)
         return operation_implementation
 
@@ -132,46 +134,57 @@
         if is_model_not_support_multi and is_multi_target:
             # Manually wrap the regressor into multi-output model
             operation_implementation = convert_to_multivariate_model(operation_implementation,
                                                                      train_data)
         else:
             sig = signature(operation_implementation.fit).parameters
             if len(sig) > 1:
-                operation_implementation.fit(
-                    train_data.features, train_data.target)
+                operation_implementation.fit(train_data.features, train_data.target)
             else:
                 operation_implementation.fit(train_data)
         return operation_implementation
 
-    def fit(self, train_data: InputData):
-        # init operation_impl model abstraction
+    def _init_impl(self, channel_params):
         try:
-            operation_implementation = self.operation_impl(
-                **self.params_for_fit.to_dict())
+            operation_implementation = self.operation_impl(**channel_params.to_dict())
         except Exception:
-            operation_implementation = self.operation_impl(self.params_for_fit)
+            operation_implementation = self.operation_impl(channel_params)
+        return operation_implementation
+
+    def fit(self, train_data: InputData):
+        # init operation_impl model abstraction
+        if isinstance(self.params_for_fit, list):
+            operation_implementation = [self._init_impl(channel_params) for channel_params in self.params_for_fit]
+        else:
+            operation_implementation = self._init_impl(self.params_for_fit)
+
         # Create model and data condition checker
-        self.operation_condition = ConditionConverter(
-            train_data, operation_implementation, self.mode)
+        self.operation_condition = ConditionConverter(train_data, operation_implementation, self.mode)
         # If model is classical sklearn model we use one_dimensional mode
         if self.operation_condition.is_one_dim_operation:
             return self.fit_one_sample(operation_implementation, train_data)
         # Elif model could be use for each dimension(channel) independently we use channel_independent mode
         elif self.operation_condition.is_channel_independent_operation:
             # Create independent copy of model for each channel
-            trained_operation = [deepcopy(operation_implementation) if self.operation_condition.is_list_container
-                                 else deepcopy(operation_implementation) for i in range(len(train_data))]
-            train_data = train_data if self.operation_condition.is_list_container else [
-                train_data]
+            if self.operation_condition.is_operation_is_list_container:
+                trained_operation = operation_implementation
+            else:
+                trained_operation = [deepcopy(operation_implementation) if self.operation_condition.is_list_container
+                                     else deepcopy(operation_implementation) for i in range(len(train_data))]
+
+            train_data = train_data if self.operation_condition.is_list_container else [train_data]
 
             # Check if model have both or just one method (fit and transform_for_fit). For some model one of this method
             # could be not finished to use right now.
             if self.operation_condition.have_fit_method:
                 operation_implementation = [operation.fit(data) for operation, data in zip(
                     trained_operation, train_data)]
+
+                if not type(operation_implementation[0]) == type(trained_operation[0]):
+                    operation_implementation = trained_operation
                 fit_method_is_not_implemented = operation_implementation[0] is None
             elif self.operation_condition.have_transform_method:
                 operation_implementation = [operation.transform_for_fit(data) for operation, data in zip(
                     trained_operation, train_data)]
 
             if fit_method_is_not_implemented:
                 operation_implementation = [operation.transform_for_fit(data) for operation, data in zip(
@@ -197,26 +210,24 @@
                                                                      predict_data=predict_data,
                                                                      output_mode=output_mode)
             else:
                 prediction = self._sklearn_compatible_prediction(trained_operation=trained_operation,
                                                                  predict_data=predict_data,
                                                                  output_mode=output_mode)
         elif self.operation_condition.is_channel_independent_operation:
-            prediction = self.__operation_multidim_adapter(
-                trained_operation, predict_data)
+            prediction = self.__operation_multidim_adapter(trained_operation, predict_data)
         elif self.operation_condition.is_multi_dimensional_operation:
             if self.operation_condition.have_predict_for_fit_method:
                 prediction = trained_operation.predict_for_fit(
                     predict_data, output_mode)
             else:
                 prediction = trained_operation.predict(
                     predict_data, output_mode)
 
-        converted = self._convert_to_output(
-            prediction, predict_data_copy, data_type, output_mode)
+        converted = self._convert_to_output(prediction, predict_data_copy, data_type, output_mode)
         return converted
 
     def predict(self, trained_operation, predict_data: InputData, output_mode: str = 'default') -> OutputData:
         data_type, predict_data_copy = FedotConverter(
             predict_data).unwrap_list_to_output()
 
         # Create data condition checker
@@ -238,16 +249,18 @@
 
 
 class IndustrialCustomPreprocessingStrategy:
     _operations_by_types = FEDOT_PREPROC_MODEL
 
     def __init__(self, operation_type: str, params: Optional[OperationParameters] = None):
         self.operation_impl = self._convert_to_operation(operation_type)
-        params = IndustrialOperationParameters().from_params(operation_type, params) if params \
-            else IndustrialOperationParameters().from_operation_type(operation_type)
+        if params is None or operation_type == 'xgboost':
+            params = IndustrialOperationParameters().from_operation_type(operation_type)
+        else:
+            params = IndustrialOperationParameters().from_params(operation_type, params)
         self.multi_dim_dispatcher = MultiDimPreprocessingStrategy(self.operation_impl,
                                                                   operation_type,
                                                                   params=params,
                                                                   mode='channel_independent')
         self.operation_id = operation_type
         self.output_mode = False
 
@@ -302,51 +315,61 @@
         operation_implementation = self.operation_impl(self.params_for_fit)
         with ImplementationRandomStateHandler(implementation=operation_implementation):
             operation_implementation.fit(train_data)
         return operation_implementation
 
     def predict(self, trained_operation, predict_data: InputData, output_mode: str = 'default') -> OutputData:
         prediction = trained_operation.transform(predict_data)
-        converted = self.multi_dim_dispatcher._convert_to_output(
-            prediction, predict_data)
+        converted = self.multi_dim_dispatcher._convert_to_output(prediction, predict_data)
         return converted
 
     def predict_for_fit(self, trained_operation, predict_data: InputData, output_mode: str = 'default') -> OutputData:
         prediction = trained_operation.transform_for_fit(predict_data)
-        converted = self.multi_dim_dispatcher._convert_to_output(
-            prediction, predict_data)
+        converted = self.multi_dim_dispatcher._convert_to_output(prediction, predict_data)
         return converted
 
 
 class IndustrialForecastingPreprocessingStrategy(IndustrialCustomPreprocessingStrategy):
     _operations_by_types = FORECASTING_PREPROC
 
     def __init__(self, operation_type: str, params: Optional[OperationParameters] = None):
         params = IndustrialOperationParameters().from_params(operation_type, params) if params \
             else IndustrialOperationParameters().from_operation_type(operation_type)
         super().__init__(operation_type, params)
+        self.multi_dim_dispatcher.concat_func = np.vstack
+        self.ensemble_func = np.sum
+
+    def _check_exog_params(self, fit_output):
+        if self.operation_type == 'exog_ts':
+            for output in fit_output:
+                output.supplementary_data.is_main_target = False
+        return fit_output
 
     def fit(self, train_data: InputData):
         train_data = self.multi_dim_dispatcher._convert_input_data(train_data)
-        return self.multi_dim_dispatcher.fit(train_data)
+        fit_output = self.multi_dim_dispatcher.fit(train_data)
+        fit_output = self._check_exog_params(fit_output)
+        return fit_output
 
     def predict(self, trained_operation,
                 predict_data: InputData,
                 output_mode: str = 'default'):
-        converted_predict_data = self.multi_dim_dispatcher._convert_input_data(
-            predict_data)
-        return self.multi_dim_dispatcher.predict(trained_operation, converted_predict_data, output_mode=output_mode)
+        converted_predict_data = self.multi_dim_dispatcher._convert_input_data(predict_data)
+        predict_output = self.multi_dim_dispatcher.predict(trained_operation, converted_predict_data,
+                                                           output_mode=output_mode)
+        return predict_output
 
     def predict_for_fit(self, trained_operation,
                         predict_data: InputData,
                         output_mode: str = 'default') -> OutputData:
-        converted_predict_data = self.multi_dim_dispatcher._convert_input_data(
-            predict_data)
-        return self.multi_dim_dispatcher.predict_for_fit(trained_operation, converted_predict_data,
-                                                         output_mode=output_mode)
+        converted_predict_data = self.multi_dim_dispatcher._convert_input_data(predict_data)
+        predict_output = self.multi_dim_dispatcher.predict_for_fit(trained_operation,
+                                                                   converted_predict_data,
+                                                                   output_mode=output_mode)
+        return predict_output
 
 
 class IndustrialClassificationPreprocessingStrategy(IndustrialCustomPreprocessingStrategy):
     _operations_by_types = INDUSTRIAL_CLF_PREPROC_MODEL
 
     def __init__(self, operation_type: str, params: Optional[OperationParameters] = None):
         super().__init__(operation_type, params)
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/basis/abstract_basis.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/basis/abstract_basis.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/basis/eigen_basis.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/basis/eigen_basis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import Optional, TypeVar
-
 import tensorly as tl
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.operations.operation_parameters import OperationParameters
 from fedot.core.repository.dataset_types import DataTypesEnum
 from joblib import delayed, Parallel
 from pymonad.either import Either
 from pymonad.list import ListMonad
 from tensorly.decomposition import parafac
+from typing import Optional, TypeVar
 
 from fedot_ind.core.architecture.preprocessing.data_convertor import DataConverter, NumpyConverter
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
 from fedot_ind.core.operation.decomposition.matrix_decomposition.power_iteration_decomposition import RSVDDecomposition
 from fedot_ind.core.operation.transformation.basis.abstract_basis import BasisDecompositionImplementation
 from fedot_ind.core.operation.transformation.data.hankel import HankelMatrix
 from fedot_ind.core.operation.transformation.regularization.spectrum import reconstruct_basis, \
@@ -33,15 +32,16 @@
 
     def __init__(self, params: Optional[OperationParameters] = None):
         super().__init__(params)
         self.window_size = params.get('window_size', 20)
         self.low_rank_approximation = params.get(
             'low_rank_approximation', True)
         self.tensor_approximation = params.get('tensor_approximation', False)
-        self.rank_regularization = params.get('rank_regularization', 'hard_thresholding')
+        self.rank_regularization = params.get(
+            'rank_regularization', 'hard_thresholding')
         self.logging_params.update({'WS': self.window_size})
         self.explained_dispersion = []
         self.SV_threshold = None
         self.svd_estimator = RSVDDecomposition()
 
     def __repr__(self):
         return 'EigenBasisImplementation'
@@ -50,15 +50,16 @@
         number_of_dim = list(range(features.shape[1]))
         predict = []
         if self.SV_threshold is None:
             self.SV_threshold = max(self.get_threshold(data=features), 2)
             self.logging_params.update({'SV_thr': self.SV_threshold})
 
         if len(number_of_dim) == 1:
-            predict = [self._transform_one_sample(signal) for signal in features[:, 0, :]]
+            predict = [self._transform_one_sample(
+                signal) for signal in features[:, 0, :]]
             predict = [[np.array(v) if len(v) > 1 else v[0] for v in predict]]
         else:
             for dimension in number_of_dim:
                 parallel = Parallel(n_jobs=self.n_processes,
                                     verbose=0, pre_dispatch="2*n_jobs")
                 v = parallel(delayed(self._transform_one_sample)(sample)
                              for sample in features[:, dimension, :])
@@ -153,18 +154,18 @@
         svd_numbers = []
 
         def mode_func(x):
             return max(set(x), key=x.count)
 
         number_of_dim = list(range(data.shape[1]))
         if len(number_of_dim) == 1:
-            try:
-                svd_numbers = [self._transform_one_sample(signal, svd_flag=True) for signal in data[:, 0, :]]
-            except Exception:
-                _ = 1
+            svd_numbers = [self._transform_one_sample(
+                signal, svd_flag=True) for signal in data[:, 0, :]]
+            if len(svd_numbers) == 0:
+                raise ValueError('Error in spectrum calculation')
         else:
             for dimension in number_of_dim:
                 dimension_rank = []
                 for signal in data[:, dimension, :]:
                     dimension_rank.append(
                         self._transform_one_sample(signal, svd_flag=True))
             svd_numbers.append(mode_func(dimension_rank))
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/basis/fourier.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/basis/fourier.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/basis/wavelet.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/basis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/data/eigen.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/data/eigen.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/data/hankel.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/data/hankel.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/data/kernel_matrix.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/data/kernel_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,26 @@
         self.rec_metric = rec_metric
 
     def ts_to_recurrence_matrix(self,
                                 threshold=None):
         distance_matrix = pdist(metric=self.rec_metric, X=self.time_series.T)
         distance_matrix = np.ones(
             shape=distance_matrix.shape[0]) - distance_matrix
-        distance_matrix = self.binarization(distance_matrix, threshold=threshold)
+        distance_matrix = self.binarization(
+            distance_matrix, threshold=threshold)
         self.recurrence_matrix = squareform(distance_matrix)
         return self.recurrence_matrix
 
     def ts_to_3d_recurrence_matrix(self):
         cosine_matrix = pdist(metric='cosine', X=self.time_series.T)
         euclidean_matrix = pdist(metric='euclidean', X=self.time_series.T)
         canberra_matrix = pdist(metric='canberra', X=self.time_series.T)
 
-        squared_matrices = list(map(squareform, [cosine_matrix, euclidean_matrix, canberra_matrix]))
+        squared_matrices = list(
+            map(squareform, [cosine_matrix, euclidean_matrix, canberra_matrix]))
         dimensions = list(map(self.colorise, squared_matrices))
         self.recurrence_matrix = np.stack(dimensions, axis=2)
         return self.recurrence_matrix
 
     def colorise(self, distance_matrix):
         """Instead of binarisation, we colorize the distance matrix by scaling the values to [0, 255].
         Also convert the matrix to uint8 type – this is the format that PIL uses to display images.
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/data/point_cloud.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/data/point_cloud.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/regularization/spectrum.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/regularization/spectrum.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/splitter.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/splitter.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/window_cutter.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/window_cutter.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/operation/transformation/window_selector.py` & `fedot_ind-0.4.2/fedot_ind/core/operation/transformation/window_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,28 +215,28 @@
             window_size = 2 ** exp
 
             if window_size < self.window_min:
                 exp += 1
                 continue
 
             score = 1 - (self.suss_score(time_series, window_size,
-                         stats) - min_score) / (max_score - min_score)
+                                         stats) - min_score) / (max_score - min_score)
 
             if score > threshold:
                 break
 
             exp += 1
 
         lbound, ubound = max(self.window_min, 2 ** (exp - 1)), 2 ** exp + 1
 
         # binary search (to find window size in interval)
         while lbound <= ubound:
             window_size = int((lbound + ubound) / 2)
             score = 1 - (self.suss_score(time_series, window_size,
-                         stats) - min_score) / (max_score - min_score)
+                                         stats) - min_score) / (max_score - min_score)
 
             if score < threshold:
                 lbound = window_size + 1
             elif score > threshold:
                 ubound = window_size - 1
             else:
                 break
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py` & `fedot_ind-0.4.2/fedot_ind/core/optimizer/IndustrialEvoOptimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,11 +21,12 @@
 
         # graph_optimizer_params.mutation_types.remove(MutationTypesEnum.single_drop)
         # graph_generation_params.verifier._rules.append(has_no_data_flow_conflicts_in_industrial_pipeline)
         # graph_generation_params.verifier._rules.remove(has_no_conflicts_with_data_flow)
 
         super().__init__(objective, initial_graphs, requirements,
                          graph_generation_params, graph_optimizer_params)
+        self.operators.remove(self.crossover)
         self.eval_dispatcher = IndustrialDispatcher(adapter=graph_generation_params.adapter,
                                                     n_jobs=requirements.n_jobs,
                                                     graph_cleanup_fn=_try_unfit_graph,
                                                     delegate_evaluator=graph_generation_params.remote_evaluator)
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/repository/IndustrialDispatcher.py` & `fedot_ind-0.4.2/fedot_ind/core/repository/IndustrialDispatcher.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/repository/IndustrialOperationParameters.py` & `fedot_ind-0.4.2/fedot_ind/core/repository/IndustrialOperationParameters.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/repository/constanst_repository.py` & `fedot_ind-0.4.2/fedot_ind/core/repository/constanst_repository.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import math
 from enum import Enum
-from functools import partial
 from multiprocessing import cpu_count
 
 import numpy as np
 import pywt
+from MKLpy.algorithms import FHeuristic, RMKL, MEMO, CKA, PWMK
 from fedot.core.pipelines.pipeline_builder import PipelineBuilder
 from fedot.core.repository.dataset_types import DataTypesEnum
 from fedot.core.repository.metrics_repository import ClassificationMetricsEnum, RegressionMetricsEnum
 from fedot.core.repository.tasks import Task, TaskTypesEnum, TsForecastingParams
-from golem.core.tuning.iopt_tuner import IOptTuner
 from golem.core.tuning.optuna_tuner import OptunaTuner
+from scipy.spatial.distance import euclidean, cosine, cityblock, correlation, chebyshev, \
+    minkowski
 from torch import nn
-from golem.core.tuning.simultaneous import SimultaneousTuner
-from golem.core.tuning.sequential import SequentialTuner
-from fedot_ind.core.metrics.metrics_implementation import calculate_classification_metric, calculate_regression_metric
+
+from fedot_ind.core.metrics.metrics_implementation import calculate_classification_metric, calculate_regression_metric, \
+    calculate_forecasting_metric
 from fedot_ind.core.models.nn.network_modules.losses import CenterLoss, CenterPlusLoss, ExpWeightedLoss, FocalLoss, \
     HuberLoss, LogCoshLoss, MaskedLossWrapper, RMSELoss, SMAPELoss, TweedieLoss
 from fedot_ind.core.models.quantile.stat_features import autocorrelation, ben_corr, crest_factor, energy, \
     hjorth_complexity, hjorth_mobility, hurst_exponent, interquartile_range, kurtosis, mean_ema, mean_moving_median, \
     mean_ptp_distance, n_peaks, pfd, ptp_amp, q25, q5, q75, q95, shannon_entropy, skewness, slope, zero_crossing_rate
 from fedot_ind.core.models.topological.topofeatures import *
 from fedot_ind.core.models.topological.topofeatures import AverageHoleLifetimeFeature, \
@@ -43,14 +44,39 @@
     }
     BATCH_SIZE_FOR_FEDOT_WORKER = 1000
     FEDOT_WORKER_NUM = 5
     FEDOT_WORKER_TIMEOUT_PARTITION = 4
     PATIENCE_FOR_EARLY_STOP = 15
 
 
+class KernelsConstant(Enum):
+    KERNEL_ALGO = {
+        'one_step_heur': FHeuristic,
+        'two_step_rmkl': RMKL,
+        'two_step_memo': MEMO,
+        'one_step_cka': CKA,
+        'one_step_pwmk': PWMK,
+    }
+    KERNEL_BASELINE_FEATURE_GENERATORS = {
+        # 'minirocket_extractor': PipelineBuilder().add_node('minirocket_extractor'),
+        'quantile_extractor': PipelineBuilder().add_node('quantile_extractor'),
+        'topological_extractor': PipelineBuilder().add_node('topological_extractor'),
+        'wavelet_extractor': PipelineBuilder().add_node('wavelet_basis').add_node('quantile_extractor'),
+        'fourier_extractor': PipelineBuilder().add_node('fourier_basis').add_node('quantile_extractor'),
+        'eigen_extractor': PipelineBuilder().add_node('eigen_basis').add_node('quantile_extractor')}
+
+    KERNEL_BASELINE_NODE_LIST = {
+        # 'minirocket_extractor': (None, 'minirocket_extractor'),
+        'quantile_extractor': (None,  'quantile_extractor'),
+        'topological_extractor': (None, 'topological_extractor'),
+        'wavelet_extractor': ('wavelet_basis', 'quantile_extractor'),
+        'fourier_extractor': ('fourier_basis', 'quantile_extractor'),
+        'eigen_extractor': ('eigen_basis', 'quantile_extractor')}
+
+
 class DataTypeConstant(Enum):
     MULTI_ARRAY = DataTypesEnum.image
     MATRIX = DataTypesEnum.table
     TRAJECTORY_MATRIX = HankelMatrix
 
 
 class FeatureConstant(Enum):
@@ -84,14 +110,24 @@
         'mean_moving_median_': mean_moving_median,
         'hjorth_mobility_': hjorth_mobility,
         'hjorth_complexity_': hjorth_complexity,
         'hurst_exponent_': hurst_exponent,
         'petrosian_fractal_dimension_': pfd
     }
 
+    METRICS_DICT = {'euclidean': euclidean,
+                    'cosine': cosine,
+                    'cityblock': cityblock,
+                    'correlation': correlation,
+                    'chebyshev': chebyshev,
+                    # 'jensenshannon': jensenshannon,
+                    # 'mahalanobis': mahalanobis,
+                    'minkowski': minkowski
+                    }
+
     PERSISTENCE_DIAGRAM_FEATURES = {'HolesNumberFeature': HolesNumberFeature(),
                                     'MaxHoleLifeTimeFeature': MaxHoleLifeTimeFeature(),
                                     'RelevantHolesNumber': RelevantHolesNumber(),
                                     'AverageHoleLifetimeFeature': AverageHoleLifetimeFeature(),
                                     'SumHoleLifetimeFeature': SumHoleLifetimeFeature(),
                                     'PersistenceEntropyFeature': PersistenceEntropyFeature(),
                                     'SimultaneousAliveHolesFeature': SimultaneousAliveHolesFeature(),
@@ -114,47 +150,41 @@
 class FedotOperationConstant(Enum):
     EXCLUDED_OPERATION = ['fast_ica']
     FEDOT_TASK = {'classification': Task(TaskTypesEnum.classification),
                   'regression': Task(TaskTypesEnum.regression),
                   'ts_forecasting': Task(TaskTypesEnum.ts_forecasting,
                                          TsForecastingParams(forecast_length=1))}
     EXCLUDED_OPERATION_MUTATION = {
-        'regression': ['one_hot_encoding',
-                       'label_encoding',
-                       'isolation_forest_class',
-                       'tst_model',
-                       'omniscale_model',
-                       'isolation_forest_reg',
-                       'inception_model',
-                       'xcm_model',
+        'regression': ['inception_model',
                        'resnet_model',
-                       'signal_extractor',
-                       'recurrence_extractor'
+                       'recurrence_extractor',
                        ],
         'ts_forecasting': [
-            'one_hot_encoding',
-            'label_encoding',
-            'isolation_forest_class'
             'xgbreg',
             'sgdr',
+            'kernel_pca',
+            'resample',
+            'inception_model',
+            'simple_imputation',
+            'channel_filtration',
+            'recurrence_extractor',
+            'quantile_extractor',
+            'riemann_extractor',
+            'minirocket_extractor',
             'treg',
             'knnreg',
+            'resnet_model',
             'dtreg'
         ],
         'classification': [
-            'isolation_forest_reg',
-            'tst_model',
             'resnet_model',
-            'xcm_model',
-            'one_hot_encoding',
-            'label_encoding',
-            'isolation_forest_class',
-            'signal_extractor',
             'knnreg',
-            'recurrence_extractor'
+            'recurrence_extractor',
+            'bernb',
+            'qda',
         ]}
     FEDOT_API_PARAMS = default_param_values_dict = dict(problem=None,
                                                         task_params=None,
                                                         timeout=None,
                                                         n_jobs=-1,
                                                         logging_level=50,
                                                         seed=42,
@@ -183,23 +213,27 @@
                                                         use_meta_rules=False,
                                                         cache_dir=None,
                                                         keep_history=True,
                                                         history_dir=None,
                                                         with_tuning=True
                                                         )
     FEDOT_GET_METRICS = {'regression': calculate_regression_metric,
+                         'ts_forecasting': calculate_forecasting_metric,
                          'classification': calculate_classification_metric}
     FEDOT_TUNING_METRICS = {'classification': ClassificationMetricsEnum.accuracy,
+                            'ts_forecasting': RegressionMetricsEnum.RMSE,
                             'regression': RegressionMetricsEnum.RMSE}
-    FEDOT_TUNER_STRATEGY = {'sequential': partial(SequentialTuner, inverse_node_order=True),
-                            'simultaneous': SimultaneousTuner,
-                          #  'IOptTuner': IOptTuner,
-                            'optuna': OptunaTuner}
+    FEDOT_TUNER_STRATEGY = {
+        # 'sequential': partial(SequentialTuner, inverse_node_order=True),
+        # 'simultaneous': SimultaneousTuner,
+        #  'IOptTuner': IOptTuner,
+        'optuna': OptunaTuner
+    }
     FEDOT_HEAD_ENSEMBLE = {'regression': 'treg',
-                           'classification': 'logit'}
+                           'classification': 'xgboost'}
     FEDOT_ATOMIZE_OPERATION = {'regression': 'fedot_regr',
                                'classification': 'fedot_cls'}
     AVAILABLE_CLS_OPERATIONS = [
         'rf',
         'logit',
         'scaling',
         'normalization',
@@ -214,17 +248,28 @@
         'xgbreg',
         'dtreg',
         'treg',
         'kernel_pca'
     ]
 
     FEDOT_ASSUMPTIONS = {
-        'classification': PipelineBuilder().add_node('quantile_extractor').add_node('logit'),
+        'classification': PipelineBuilder().add_node('channel_filtration').
+        add_node('quantile_extractor').add_node('xgboost'),
         'regression': PipelineBuilder().add_node('quantile_extractor').add_node('treg'),
-        'ts_forecasting': PipelineBuilder().add_node('ssa_forecaster')
+        'ts_forecasting': PipelineBuilder().add_node('eigen_basis', params={'low_rank_approximation': False,
+                                                                            'rank_regularization': 'explained_dispersion'}).add_node(
+            'ar')}
+
+    FEDOT_TS_FORECASTING_ASSUMPTIONS = {
+        # 'lagged_ridge': PipelineBuilder().add_node('lagged').add_node('ridge'),
+        'eigen_ar': PipelineBuilder().add_node('eigen_basis',
+                                               params={'low_rank_approximation': False,
+                                                       'rank_regularization': 'explained_dispersion'}).add_node('ar'),
+       # 'topological_ridge': PipelineBuilder().add_node('lagged').add_node('topological_extractor').add_node('ridge'),
+       'glm': PipelineBuilder().add_node('glm')
     }
 
     FEDOT_ENSEMBLE_ASSUMPTIONS = {
         'classification': PipelineBuilder().add_node('logit'),
         'regression': PipelineBuilder().add_node('treg')
     }
 
@@ -244,23 +289,23 @@
     }
 
 
 class TorchLossesConstant(Enum):
     CROSS_ENTROPY = nn.CrossEntropyLoss
     MULTI_CLASS_CROSS_ENTROPY = nn.BCEWithLogitsLoss
     MSE = nn.MSELoss
-    RMSE = RMSELoss()
-    SMAPE = SMAPELoss()
-    TWEEDIE_LOSS = TweedieLoss()
-    FOCAL_LOSS = FocalLoss()
+    RMSE = RMSELoss
+    SMAPE = SMAPELoss
+    TWEEDIE_LOSS = TweedieLoss
+    FOCAL_LOSS = FocalLoss
     CENTER_PLUS_LOSS = CenterPlusLoss
     CENTER_LOSS = CenterLoss
     MASK_LOSS = MaskedLossWrapper
-    LOG_COSH_LOSS = LogCoshLoss()
-    HUBER_LOSS = HuberLoss()
+    LOG_COSH_LOSS = LogCoshLoss
+    HUBER_LOSS = HuberLoss
     EXPONENTIAL_WEIGHTED_LOSS = ExpWeightedLoss
 
 
 class BenchmarkDatasets(Enum):
     MULTI_REG_BENCH = [
         "AppliancesEnergy",
         "AustraliaRainfall",
@@ -569,28 +614,34 @@
 PERSISTENCE_DIAGRAM_FEATURES = FeatureConstant.PERSISTENCE_DIAGRAM_FEATURES.value
 PERSISTENCE_DIAGRAM_EXTRACTOR = FeatureConstant.PERSISTENCE_DIAGRAM_EXTRACTOR.value
 DISCRETE_WAVELETS = FeatureConstant.DISCRETE_WAVELETS.value
 CONTINUOUS_WAVELETS = FeatureConstant.CONTINUOUS_WAVELETS.value
 WAVELET_SCALES = FeatureConstant.WAVELET_SCALES.value
 SINGULAR_VALUE_MEDIAN_THR = FeatureConstant.SINGULAR_VALUE_MEDIAN_THR.value
 SINGULAR_VALUE_BETA_THR = FeatureConstant.SINGULAR_VALUE_BETA_THR
+DISTANCE_METRICS = FeatureConstant.METRICS_DICT.value
+
+KERNEL_ALGO = KernelsConstant.KERNEL_ALGO.value
+KERNEL_BASELINE_FEATURE_GENERATORS = KernelsConstant.KERNEL_BASELINE_FEATURE_GENERATORS.value
+KERNEL_BASELINE_NODE_LIST = KernelsConstant.KERNEL_BASELINE_NODE_LIST.value
 
 AVAILABLE_REG_OPERATIONS = FedotOperationConstant.AVAILABLE_REG_OPERATIONS.value
 AVAILABLE_CLS_OPERATIONS = FedotOperationConstant.AVAILABLE_CLS_OPERATIONS.value
 EXCLUDED_OPERATION = FedotOperationConstant.EXCLUDED_OPERATION.value
 EXCLUDED_OPERATION_MUTATION = FedotOperationConstant.EXCLUDED_OPERATION_MUTATION.value
 FEDOT_HEAD_ENSEMBLE = FedotOperationConstant.FEDOT_HEAD_ENSEMBLE.value
 FEDOT_TASK = FedotOperationConstant.FEDOT_TASK.value
 FEDOT_ATOMIZE_OPERATION = FedotOperationConstant.FEDOT_ATOMIZE_OPERATION.value
 FEDOT_GET_METRICS = FedotOperationConstant.FEDOT_GET_METRICS.value
 FEDOT_TUNING_METRICS = FedotOperationConstant.FEDOT_TUNING_METRICS.value
 FEDOT_ASSUMPTIONS = FedotOperationConstant.FEDOT_ASSUMPTIONS.value
 FEDOT_API_PARAMS = FedotOperationConstant.FEDOT_API_PARAMS.value
 FEDOT_ENSEMBLE_ASSUMPTIONS = FedotOperationConstant.FEDOT_ENSEMBLE_ASSUMPTIONS.value
 FEDOT_TUNER_STRATEGY = FedotOperationConstant.FEDOT_TUNER_STRATEGY.value
+FEDOT_TS_FORECASTING_ASSUMPTIONS = FedotOperationConstant.FEDOT_TS_FORECASTING_ASSUMPTIONS.value
 
 CPU_NUMBERS = ComputationalConstant.CPU_NUMBERS.value
 BATCH_SIZE_FOR_FEDOT_WORKER = ComputationalConstant.BATCH_SIZE_FOR_FEDOT_WORKER.value
 FEDOT_WORKER_NUM = ComputationalConstant.FEDOT_WORKER_NUM.value
 FEDOT_WORKER_TIMEOUT_PARTITION = ComputationalConstant.FEDOT_WORKER_TIMEOUT_PARTITION.value
 PATIENCE_FOR_EARLY_STOP = ComputationalConstant.PATIENCE_FOR_EARLY_STOP.value
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/repository/data/default_operation_params.json` & `fedot_ind-0.4.2/fedot_ind/core/repository/data/default_operation_params.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8910256410256411%*

 * *Differences: {"'ar'": "{'trend': 'c'}",*

 * * "'channel_filtration'": "OrderedDict([('distance', 'euclidean'), ('shrink', 1e-05), "*

 * *                         "('centroid_metric', 'euclidean'), ('selection_strategy', 'pairwise')])",*

 * * "'chronos_extractor'": "OrderedDict([('num_features', 10000)])",*

 * * "'riemann_extractor'": "OrderedDict([('n_filter', 4), ('estimator', 'scm'), ('tangent_metric', "*

 * *                        "'riemann'), ('SPD_metric', 'riemann')])",*

 * * "'topological_extractor'": "OrderedDict([('n_jobs', 2), ('window_si […]*

```diff
@@ -1,11 +1,12 @@
 {
     "ar": {
         "lag_1": 7,
-        "lag_2": 12
+        "lag_2": 12,
+        "trend": "c"
     },
     "arima": {
         "d": 0,
         "p": 2,
         "q": 2
     },
     "catboost": {
@@ -24,14 +25,23 @@
         "cnn2_output_size": 64,
         "hidden_size": 200,
         "learning_rate": 0.001,
         "loss": "mse",
         "num_epochs": 50,
         "optimizer": "adamw"
     },
+    "channel_filtration": {
+        "centroid_metric": "euclidean",
+        "distance": "euclidean",
+        "selection_strategy": "pairwise",
+        "shrink": 1e-05
+    },
+    "chronos_extractor": {
+        "num_features": 10000
+    },
     "cut": {
         "cut_part": 0.5
     },
     "diff_filter": {
         "order": 1,
         "poly_degree": 2,
         "window_size": 3
@@ -173,29 +183,35 @@
     },
     "rfr": {
         "bootstrap": false,
         "max_features": 0.9,
         "min_samples_leaf": 5,
         "min_samples_split": 5
     },
+    "riemann_extractor": {
+        "SPD_metric": "riemann",
+        "estimator": "scm",
+        "n_filter": 4,
+        "tangent_metric": "riemann"
+    },
     "sparse_lagged": {
         "n_components": 0.5,
         "sparse_transform": true,
         "use_svd": false,
         "window_size": 10
     },
     "ssa_forecaster": {
         "history_lookback": 30,
         "window_size_method": "hac"
     },
     "tfidf": {
         "max_df": 0.9,
         "min_df": 0.1
     },
-    "topological_features": {
+    "topological_extractor": {
         "max_homology_dimension": 1,
         "metric": "euclidean",
         "n_jobs": 2,
         "window_size_as_share": 0.33
     },
     "tpot_class": {
         "generations": 3,
@@ -222,11 +238,13 @@
         "model_name": "glove-twitter-25"
     },
     "xcm_model": {
         "batch_size": 32,
         "epochs": 100
     },
     "xgboost": {
-        "eval_metric": "mlogloss",
-        "nthread": -1
+        "learning_rate": 0.1,
+        "max_depth": 5,
+        "n_estimators": 500,
+        "random_state": 42
     }
 }
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/repository/data/industrial_data_operation_repository.json` & `fedot_ind-0.4.2/fedot_ind/core/repository/data/industrial_data_operation_repository.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9654224537037037%*

 * *Differences: {"'metadata'": "{'industrial_preprocessing': {'tasks': '[TaskTypesEnum.classification, "*

 * *               "TaskTypesEnum.regression, TaskTypesEnum.ts_forecasting]', 'input_type': "*

 * *               "'[DataTypesEnum.image, DataTypesEnum.table, DataTypesEnum.ts]', 'output_type': "*

 * *               "'[DataTypesEnum.image, DataTypesEnum.table, DataTypesEnum.ts]'}}",*

 * * "'operations'": "{'eigen_basis': {'tags': {insert: [(1, 'non_lagged'), (2, 'ts_to_ts')]}}, "*

 * *                 "'wavelet_basis': {'tags': {insert: [(1, ' […]*

```diff
@@ -86,22 +86,22 @@
         },
         "industrial_preprocessing": {
             "accepted_node_types": [
                 "any"
             ],
             "description": "Implementations of industrial preprocessing operations",
             "forbidden_node_types": "[]",
-            "input_type": "[DataTypesEnum.image, DataTypesEnum.table]",
-            "output_type": "[DataTypesEnum.image, DataTypesEnum.table]",
+            "input_type": "[DataTypesEnum.image, DataTypesEnum.table, DataTypesEnum.ts]",
+            "output_type": "[DataTypesEnum.image, DataTypesEnum.table, DataTypesEnum.ts]",
             "strategies": [
                 "fedot_ind.core.operation.interfaces.industrial_preprocessing_strategy",
                 "IndustrialPreprocessingStrategy"
             ],
             "tags": [],
-            "tasks": "[TaskTypesEnum.classification, TaskTypesEnum.regression]"
+            "tasks": "[TaskTypesEnum.classification, TaskTypesEnum.regression, TaskTypesEnum.ts_forecasting]"
         },
         "industrial_preprocessing_forecasting": {
             "accepted_node_types": [
                 "any"
             ],
             "description": "Implementations of industrial preprocessing operations",
             "forbidden_node_types": "[]",
@@ -204,15 +204,36 @@
     "operations": {
         "cat_features": {
             "meta": "industrial_preprocessing",
             "presets": [
                 "fast_train"
             ],
             "tags": [
-                "cat_features"
+                "cat_features",
+                "non_applicable_for_ts"
+            ]
+        },
+        "channel_filtration": {
+            "meta": "industrial_preprocessing",
+            "presets": [
+                "fast_train"
+            ],
+            "tags": [
+                "extractor",
+                "non_applicable_for_ts"
+            ]
+        },
+        "chronos_extractor": {
+            "meta": "industrial_preprocessing",
+            "presets": [
+                "fast_train"
+            ],
+            "tags": [
+                "extractor",
+                "non_applicable_for_ts"
             ]
         },
         "class_decompose": {
             "meta": "classification_preprocessing",
             "presets": [
                 "fast_train",
                 "*tree"
@@ -308,30 +329,23 @@
             ],
             "tags": [
                 "differential",
                 "non_lagged",
                 "ts_to_ts"
             ]
         },
-        "dimension_reduction": {
-            "meta": "industrial_preprocessing",
-            "presets": [
-                "fast_train"
-            ],
-            "tags": [
-                "extractor"
-            ]
-        },
         "eigen_basis": {
             "meta": "industrial_preprocessing",
             "presets": [
                 "fast_train"
             ],
             "tags": [
-                "basis"
+                "basis",
+                "non_lagged",
+                "ts_to_ts"
             ]
         },
         "exog_ts": {
             "meta": "custom_time_series_transformation",
             "tags": [
                 "simple",
                 "non_lagged",
@@ -354,15 +368,16 @@
         },
         "fourier_basis": {
             "meta": "industrial_preprocessing",
             "presets": [
                 "fast_train"
             ],
             "tags": [
-                "basis"
+                "basis",
+                "non_applicable_for_ts"
             ]
         },
         "gaussian_filter": {
             "input_type": "[DataTypesEnum.multi_ts, DataTypesEnum.ts]",
             "meta": "custom_time_series_transformation",
             "presets": [
                 "fast_train",
@@ -432,15 +447,16 @@
         },
         "minirocket_extractor": {
             "meta": "industrial_preprocessing",
             "presets": [
                 "fast_train"
             ],
             "tags": [
-                "extractor"
+                "extractor",
+                "non_applicable_for_ts"
             ]
         },
         "normalization": {
             "meta": "custom_preprocessing",
             "presets": [
                 "fast_train",
                 "ts",
@@ -524,15 +540,16 @@
         },
         "recurrence_extractor": {
             "meta": "industrial_preprocessing",
             "presets": [
                 "fast_train"
             ],
             "tags": [
-                "extractor"
+                "extractor",
+                "non_applicable_for_ts"
             ]
         },
         "resample": {
             "meta": "classification_preprocessing",
             "tags": [
                 "imbalanced"
             ]
@@ -569,14 +586,24 @@
                 "non_linear",
                 "feature_selection",
                 "non_applicable_for_ts",
                 "non-default",
                 "non_applicable_for_ts"
             ]
         },
+        "riemann_extractor": {
+            "meta": "industrial_preprocessing",
+            "presets": [
+                "fast_train"
+            ],
+            "tags": [
+                "extractor",
+                "non_applicable_for_ts"
+            ]
+        },
         "scaling": {
             "meta": "custom_preprocessing",
             "presets": [
                 "fast_train",
                 "ts",
                 "*tree"
             ],
@@ -634,30 +661,31 @@
         },
         "tfidf": {
             "meta": "text_preprocessing_sklearn",
             "tags": [
                 "non-default"
             ]
         },
-        "topological_features": {
+        "topological_extractor": {
             "meta": "custom_preprocessing",
             "presets": [
                 "fast_train"
             ],
             "tags": [
                 "extractor"
             ]
         },
         "wavelet_basis": {
             "meta": "industrial_preprocessing",
             "presets": [
                 "fast_train"
             ],
             "tags": [
-                "basis"
+                "basis",
+                "non_applicable_for_ts"
             ]
         },
         "word2vec_pretrained": {
             "meta": "text_classification_gensim",
             "tags": [
                 "non-default"
             ]
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/repository/data/industrial_model_repository.json` & `fedot_ind-0.4.2/fedot_ind/core/repository/data/industrial_model_repository.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998697916666667%*

 * *Differences: {"'operations'": "{'ar': {'tags': {delete: [4]}}, 'glm': {'tags': {delete: [3]}}}"}*

```diff
@@ -231,16 +231,15 @@
                 "fast_train",
                 "ts"
             ],
             "tags": [
                 "simple",
                 "interpretable",
                 "non_lagged",
-                "linear",
-                "correct_params"
+                "linear"
             ]
         },
         "arima": {
             "input_type": "[DataTypesEnum.ts]",
             "meta": "ts_model",
             "presets": [
                 "ts"
@@ -391,15 +390,14 @@
                 "fast_train",
                 "ts"
             ],
             "tags": [
                 "simple",
                 "interpretable",
                 "non_lagged",
-                "correct_params",
                 "non_linear"
             ]
         },
         "inception_model": {
             "meta": "fedot_NN_classification",
             "presets": [
                 "best_quality"
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/repository/industrial_implementations/metric.py` & `fedot_ind-0.4.2/fedot_ind/core/repository/industrial_implementations/metric.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/repository/industrial_implementations/optimisation.py` & `fedot_ind-0.4.2/fedot_ind/core/repository/industrial_implementations/optimisation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import itertools
 from copy import deepcopy
 from itertools import chain
 from math import ceil
 from random import choice, sample
 from typing import Sequence
 from typing import Tuple
-
+from fedot.core.pipelines.node import PipelineNode
+from fedot.core.pipelines.pipeline import Pipeline
+from fedot.core.operations.atomized_model import AtomizedModel
 from fedot.core.composer.gp_composer.specific_operators import boosting_mutation, parameter_change_mutation
 from fedot.core.pipelines.adapters import PipelineAdapter
 from fedot.core.pipelines.node import PipelineNode
 from fedot.core.pipelines.pipeline import Pipeline
+from fedot.core.pipelines.pipeline_builder import PipelineBuilder
 from fedot.core.repository.operation_types_repository import get_operations_for_task
 from fedot.core.repository.tasks import Task
 from fedot.core.repository.tasks import TaskTypesEnum
 from golem.core.adapter import register_native
 from golem.core.dag.graph import ReconnectType
 from golem.core.dag.graph_utils import graph_has_cycle
 from golem.core.dag.graph_utils import node_depth, nodes_from_layer
@@ -25,35 +28,36 @@
 from golem.core.optimisers.genetic.operators.mutation import MutationTypesEnum
 from golem.core.optimisers.graph import OptGraph, OptNode
 from golem.core.optimisers.opt_node_factory import OptNodeFactory
 from golem.core.optimisers.optimization_parameters import GraphRequirements
 from golem.core.optimisers.optimizer import AlgorithmParameters
 from golem.core.optimisers.optimizer import GraphGenerationParams
 from golem.utilities.data_structures import ComparableEnum as Enum
-
-from fedot_ind.core.repository.model_repository import AtomizedModel, TEMPORARY_EXCLUDED
+from fedot.core.operations.atomized_model import AtomizedModel as Atom
+from fedot_ind.core.repository.constanst_repository import EXCLUDED_OPERATION_MUTATION
+from fedot_ind.core.repository.model_repository import AtomizedModel, TEMPORARY_EXCLUDED, \
+    default_industrial_availiable_operation
 
 
 class MutationStrengthEnumIndustrial(Enum):
     weak = 1.0
     mean = 3.0
     strong = 5.0
 
 
 class IndustrialMutations:
     def __init__(self, task_type):
         self.node_adapter = PipelineAdapter()
         self.task_type = Task(task_type)
-        self.industrial_data_operations = [*list(AtomizedModel.INDUSTRIAL_PREPROC_MODEL.value.keys()),
-                                           *list(AtomizedModel.INDUSTRIAL_CLF_PREPROC_MODEL.value.keys()),
-                                           *list(AtomizedModel.FEDOT_PREPROC_MODEL.value.keys()),
-                                           *list(AtomizedModel.NEURAL_MODEL.value.keys())]
+        self.excluded_mutation = EXCLUDED_OPERATION_MUTATION[self.task_type.task_type.value]
+        self.industrial_data_operations = default_industrial_availiable_operation(self.task_type.task_type.value)
         self.excluded = [list(TEMPORARY_EXCLUDED[x].keys())
                          for x in TEMPORARY_EXCLUDED.keys()]
         self.excluded = (list(itertools.chain(*self.excluded)))
+        self.excluded = self.excluded + self.excluded_mutation
         self.industrial_data_operations = [operation for operation in self.industrial_data_operations if operation
                                            not in self.excluded]
 
     def transform_to_pipeline_node(self, node):
         return self.node_adapter._transform_to_pipeline_node(node)
 
     def transform_to_opt_node(self, node):
@@ -142,15 +146,15 @@
         # add as child
         old_node_children = graph.node_children(node_to_mutate)
         new_node_child = choice(
             old_node_children) if old_node_children else None
 
         while True:
             new_node = node_factory.get_node(is_primary=False)
-            if new_node.name not in self.industrial_data_operations:
+            if new_node.name in self.industrial_data_operations:
                 break
         if not new_node:
             return graph
 
         new_node = self.transform_to_pipeline_node(new_node)
 
         if graph.depth == 1:
@@ -258,45 +262,58 @@
     def add_preprocessing(self,
                           pipeline: Pipeline, **kwargs) -> Pipeline:
 
         basis_models = get_operations_for_task(
             task=self.task_type, mode='data_operation', tags=["basis"])
         extractors = get_operations_for_task(
             task=self.task_type, mode='data_operation', tags=["extractor"])
-        extractors = [x for x in extractors if x != 'dimension_reduction']
+        extractors = [x for x in extractors if x in self.industrial_data_operations]
         models = get_operations_for_task(task=self.task_type, mode='model')
-        models = [x for x in models if x != 'fedot_cls']
+        models = [x for x in models if x not in self.excluded_mutation]
         basis_model = PipelineNode(choice(basis_models))
         extractor_model = PipelineNode(
             choice(extractors), nodes_from=[basis_model])
         node_to_mutate = list(
             filter(lambda x: x.name in models, pipeline.nodes))[0]
         if node_to_mutate.nodes_from:
             node_to_mutate.nodes_from.append(extractor_model)
         else:
             node_to_mutate.nodes_from = [extractor_model]
         pipeline.nodes.append(basis_model)
         pipeline.nodes.append(extractor_model)
 
         return pipeline
 
+    def add_lagged(self, pipeline: Pipeline, **kwargs) -> Pipeline:
+        lagged = ['lagged', 'ridge']
+        current_operation = list(reversed([x.name for x in pipeline.nodes]))
+        if 'lagged' in current_operation:
+            return pipeline
+        else:
+            pipeline = PipelineBuilder().add_sequence(*lagged, branch_idx=0).\
+                add_sequence(*current_operation, branch_idx=1).join_branches('ridge').build()
+            return pipeline
+
 
 def _get_default_industrial_mutations(task_type: TaskTypesEnum, params) -> Sequence[MutationTypesEnum]:
     ind_mutations = IndustrialMutations(task_type=task_type)
     mutations = [
         parameter_change_mutation,
         ind_mutations.single_change,
         ind_mutations.add_preprocessing,
         # IndustrialMutations().single_drop,
         ind_mutations.single_add
 
     ]
     # TODO remove workaround after boosting mutation fix
     if task_type == TaskTypesEnum.ts_forecasting:
         mutations.append(boosting_mutation)
+        #mutations.append(ind_mutations.add_lagged)
+        mutations.remove(ind_mutations.add_preprocessing)
+        mutations.remove(ind_mutations.single_add)
     # TODO remove workaround after validation fix
     if task_type is not TaskTypesEnum.ts_forecasting:
         mutations.append(MutationTypesEnum.single_edge)
     return mutations
 
 
 class IndustrialCrossover:
@@ -530,21 +547,10 @@
                         f'Basis output should contain feature transformation')
 
         else:
             continue
     return True
 
 
-def _crossover_by_type(self, crossover_type: CrossoverTypesEnum) -> CrossoverCallable:
+def _crossover_by_type(self, crossover_type: CrossoverTypesEnum) -> None:
     ind_crossover = IndustrialCrossover()
-    crossovers = {
-        CrossoverTypesEnum.subtree: ind_crossover.subtree_crossover,
-        CrossoverTypesEnum.one_point: ind_crossover.one_point_crossover,
-        CrossoverTypesEnum.exchange_edges: ind_crossover.exchange_edges_crossover,
-        CrossoverTypesEnum.exchange_parents_one: ind_crossover.exchange_parents_one_crossover,
-        CrossoverTypesEnum.exchange_parents_both: ind_crossover.exchange_parents_both_crossover
-    }
-    if crossover_type in crossovers:
-        return crossovers[crossover_type]
-    else:
-        raise ValueError(
-            f'Required crossover type is not found: {crossover_type}')
+    return None
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/repository/initializer_industrial_models.py` & `fedot_ind-0.4.2/fedot_ind/core/repository/initializer_industrial_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import pathlib
+import types
 
 from fedot.api.api_utils.api_composer import ApiComposer
 from fedot.api.api_utils.api_params_repository import ApiParamsRepository
+import fedot.core.data.data_split as fedot_data_split
 from fedot.core.data.merge.data_merger import ImageDataMerger, TSDataMerger
 from fedot.core.operations.evaluation.operation_implementations.data_operations.ts_transformations import \
     LaggedImplementation, TsSmoothingImplementation
 from fedot.core.operations.operation import Operation
+from fedot.core.optimisers.objective.data_source_splitter import DataSourceSplitter
 from fedot.core.pipelines.tuning.search_space import PipelineSearchSpace
 from fedot.core.pipelines.verification import class_rules
 from fedot.core.repository.operation_types_repository import OperationTypesRepository
 from golem.core.optimisers.genetic.operators.crossover import Crossover
 
 from fedot_ind.api.utils.path_lib import PROJECT_PATH
 from fedot_ind.core.repository.industrial_implementations.abstract import merge_predicts, preprocess_predicts, \
     predict_for_fit, predict, predict_operation, postprocess_predicts, update_column_types, transform_lagged, \
-    transform_lagged_for_fit, transform_smoothing
+    transform_lagged_for_fit, transform_smoothing, _build, split_any, _check_and_correct_window_size, merge_targets, \
+    split_time_series
 from fedot_ind.core.repository.industrial_implementations.optimisation import _get_default_industrial_mutations, \
     MutationStrengthEnumIndustrial, has_no_data_flow_conflicts_in_industrial_pipeline, _crossover_by_type
 from fedot_ind.core.tuning.search_space import get_industrial_search_space
 
 
 class IndustrialModels:
     def __init__(self):
@@ -48,37 +52,46 @@
 
         OperationTypesRepository.__repository_dict__.update(
             {'model': {'file': self.industrial_model_path,
                        'initialized_repo': True,
                        'default_tags': []}})
         OperationTypesRepository.assign_repo(
             'model', self.industrial_model_path)
-
+        # replace mutations
         setattr(PipelineSearchSpace, "get_parameters_dict",
                 get_industrial_search_space)
         setattr(ApiParamsRepository, "_get_default_mutations",
                 _get_default_industrial_mutations)
-        setattr(Crossover, '_crossover_by_type', _crossover_by_type)
-
+        #setattr(Crossover, '_crossover_by_type', _crossover_by_type)
+        # replace data merger
         setattr(ImageDataMerger, "preprocess_predicts", preprocess_predicts)
         setattr(ImageDataMerger, "merge_predicts", merge_predicts)
+        setattr(TSDataMerger, "merge_predicts", merge_predicts)
+        setattr(TSDataMerger, "merge_targets", merge_targets)
         setattr(TSDataMerger, 'postprocess_predicts', postprocess_predicts)
-
+        # replace data split
+        setattr(DataSourceSplitter, "build", _build)
+        setattr(fedot_data_split, "_split_any",  split_any)
+        setattr(fedot_data_split, "_split_time_series", split_time_series)
+        # setattr(TSDataMerger, 'postprocess_predicts', postprocess_predicts)
+        # replace predict operations
         setattr(Operation, "_predict", predict_operation)
         setattr(Operation, "predict", predict)
         setattr(Operation, "predict_for_fit", predict_for_fit)
-
+        # replace ts forecasting operations
         setattr(LaggedImplementation,
                 '_update_column_types', update_column_types)
         setattr(LaggedImplementation, 'transform', transform_lagged)
         setattr(LaggedImplementation, 'transform_for_fit',
                 transform_lagged_for_fit)
+        setattr(LaggedImplementation, '_check_and_correct_window_size',
+                _check_and_correct_window_size)
         setattr(TsSmoothingImplementation, 'transform', transform_smoothing)
 
-        # class_rules.append(has_no_data_flow_conflicts_in_industrial_pipeline)
+        class_rules.append(has_no_data_flow_conflicts_in_industrial_pipeline)
         MutationStrengthEnum = MutationStrengthEnumIndustrial
         return OperationTypesRepository
 
     def __enter__(self):
         """
         Switching to industrial models
         """
@@ -97,15 +110,14 @@
         OperationTypesRepository.assign_repo(
             'model', self.industrial_model_path)
 
         setattr(PipelineSearchSpace, "get_parameters_dict",
                 get_industrial_search_space)
         setattr(ApiComposer, "_get_default_mutations",
                 _get_default_industrial_mutations)
-        class_rules.append(has_no_data_flow_conflicts_in_industrial_pipeline)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """
         Switching to fedot models.
         """
         OperationTypesRepository.__repository_dict__.update(
             {'data_operation': {'file': self.base_data_operation_path,
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/repository/model_repository.py` & `fedot_ind-0.4.2/fedot_ind/core/repository/model_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,95 +9,98 @@
     IsolationForestClassImplementation, IsolationForestRegImplementation
 from fedot.core.operations.evaluation.operation_implementations.data_operations.sklearn_imbalanced_class import \
     ResampleImplementation
 from fedot.core.operations.evaluation.operation_implementations.data_operations.sklearn_selectors import \
     LinearClassFSImplementation, NonLinearClassFSImplementation
 from fedot.core.operations.evaluation.operation_implementations.data_operations.sklearn_transformations import \
     *
-from fedot.core.operations.evaluation.operation_implementations. \
-    data_operations.topological.fast_topological_extractor import \
+
+from fedot.core.operations.evaluation.operation_implementations.data_operations.topological.fast_topological_extractor import \
     TopologicalFeaturesImplementation
-    # FastTopologicalFeaturesImplementation
 from fedot.core.operations.evaluation.operation_implementations.data_operations.ts_transformations import \
     ExogDataTransformationImplementation, GaussianFilterImplementation, LaggedTransformationImplementation, \
     SparseLaggedTransformationImplementation, TsSmoothingImplementation
 from fedot.core.operations.evaluation.operation_implementations.models.knn import FedotKnnClassImplementation, \
     FedotKnnRegImplementation
 from fedot.core.operations.evaluation.operation_implementations.models.ts_implementations.arima import \
     STLForecastARIMAImplementation
 from fedot.core.operations.evaluation.operation_implementations.models.ts_implementations.cgru import \
     CGRUImplementation
-from fedot.core.operations.evaluation.operation_implementations.models.ts_implementations.naive import \
-    RepeatLastValueImplementation
 from fedot.core.operations.evaluation.operation_implementations.models.ts_implementations.statsmodels import \
     AutoRegImplementation, ExpSmoothingImplementation, GLMImplementation
-from sklearn.ensemble import AdaBoostRegressor, ExtraTreesRegressor, GradientBoostingRegressor, \
+from sklearn.ensemble import AdaBoostRegressor, ExtraTreesRegressor, GradientBoostingRegressor, GradientBoostingClassifier, \
     RandomForestClassifier, RandomForestRegressor
 from sklearn.linear_model import (
     Lasso as SklearnLassoReg,
     LinearRegression as SklearnLinReg,
     LogisticRegression as SklearnLogReg,
     Ridge as SklearnRidgeReg,
     SGDRegressor as SklearnSGD
 )
+
 from sklearn.naive_bayes import BernoulliNB as SklearnBernoulliNB, MultinomialNB as SklearnMultinomialNB
 from sklearn.neural_network import MLPClassifier
 from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 from xgboost import XGBClassifier, XGBRegressor
 
+from fedot_ind.core.models.manifold.riemann_embeding import RiemannExtractor
+from fedot_ind.core.models.nn.network_impl.chronos_tst import ChronosExtractor
 from fedot_ind.core.models.nn.network_impl.explainable_convolution_model import XCModel
 from fedot_ind.core.models.nn.network_impl.inception import InceptionTimeModel
 from fedot_ind.core.models.nn.network_impl.mini_rocket import MiniRocketExtractor
 from fedot_ind.core.models.nn.network_impl.omni_scale import OmniScaleModel
 from fedot_ind.core.models.nn.network_impl.resnet import ResNetModel
 from fedot_ind.core.models.nn.network_impl.tst import TSTModel
 from fedot_ind.core.models.quantile.quantile_extractor import QuantileExtractor
 from fedot_ind.core.models.recurrence.reccurence_extractor import RecurrenceExtractor
-from fedot_ind.core.models.topological.topological_extractor import TopologicalExtractor
-from fedot_ind.core.models.ts_forecasting.ssa_forecaster import SSAForecasterImplementation
+from fedot_ind.core.models.ts_forecasting.glm import GLMIndustrial
 from fedot_ind.core.operation.dummy.dummy_operation import DummyOperation
+from fedot_ind.core.operation.filtration.channel_filtration import ChannelCentroidFilter
 from fedot_ind.core.operation.filtration.feature_filtration import FeatureFilter
 from fedot_ind.core.operation.transformation.basis.eigen_basis import EigenBasisImplementation
 from fedot_ind.core.operation.transformation.basis.fourier import FourierBasisImplementation
 from fedot_ind.core.operation.transformation.basis.wavelet import WaveletBasisImplementation
 from fedot_ind.core.repository.constanst_repository import EXCLUDED_OPERATION_MUTATION
 
 TEMPORARY_EXCLUDED = {
     'INDUSTRIAL_CLF_PREPROC_MODEL': {
         'rfe_lin_class': LinearClassFSImplementation,
         'rfe_non_lin_class': NonLinearClassFSImplementation,
     },
     'FEDOT_PREPROC_MODEL': {'pca': PCAImplementation,
                             'fast_ica': FastICAImplementation,
                             'poly_features': PolyFeaturesImplementation,
-                            'topological_extractor': TopologicalExtractor,
                             'exog_ts': ExogDataTransformationImplementation,
                             # categorical encoding
                             'one_hot_encoding': OneHotEncodingImplementation,
                             'label_encoding': LabelEncodingImplementation
                             },
-    'INDUSTRIAL_PREPROC_MODEL': {'cat_features': DummyOperation,
-                                 'dimension_reduction': FeatureFilter,
-                                 # 'signal_extractor': SignalExtractor,
-                                 # isolation_forest forest
-                                 'isolation_forest_class': IsolationForestClassImplementation,
-                                 'isolation_forest_reg': IsolationForestRegImplementation,
-                                 },
+    'FORECASTING_PREPROC': {'exog_ts': ExogDataTransformationImplementation},
+    'INDUSTRIAL_PREPROC_MODEL': {
+        'cat_features': DummyOperation,
+        'dimension_reduction': FeatureFilter,
+        # 'signal_extractor': SignalExtractor,
+        # isolation_forest forest
+        'isolation_forest_class': IsolationForestClassImplementation,
+        'isolation_forest_reg': IsolationForestRegImplementation,
+        # 'chronos_extractor': ChronosExtractor,
+        'riemann_extractor': RiemannExtractor,
+    },
     'SKLEARN_REG_MODELS': {
         'gbr': GradientBoostingRegressor,
         'rfr': RandomForestRegressor,
         'adareg': AdaBoostRegressor,
         'linear': SklearnLinReg,
         'knnreg': FedotKnnRegImplementation,
     },
     'SKLEARN_CLF_MODELS': {'bernb': SklearnBernoulliNB,
                            'multinb': SklearnMultinomialNB,
                            'knn': FedotKnnClassImplementation
                            },
-    'NEURAL_MODELS': {'resnet_model': ResNetModel,
+    'NEURAL_MODELS': {'omniscale_model': OmniScaleModel,
                       # transformer models
                       'tst_model': TSTModel,
                       # explainable models
                       'xcm_model': XCModel
                       }
 }
 
@@ -108,15 +111,15 @@
         'class_decompose': DecomposerClassImplementation,
         # for imbalanced data
         'resample': ResampleImplementation,
 
     }
     SKLEARN_CLF_MODELS = {
         # boosting models (bid datasets)
-        'xgboost': XGBClassifier,
+        'xgboost': GradientBoostingClassifier,
         # solo linear models
         'logit': SklearnLogReg,
         # solo tree models
         'dt': DecisionTreeClassifier,
         # ensemble tree models
         'rf': RandomForestClassifier,
         # solo nn models
@@ -127,27 +130,32 @@
         'scaling': ScalingImplementation,
         'normalization': NormalizationImplementation,
         # missing data
         'simple_imputation': ImputationImplementation,
         # dimension reduction
         'kernel_pca': KernelPCAImplementation,
         # feature generation
-        'topological_features': TopologicalFeaturesImplementation,
-
+        'topological_extractor': TopologicalFeaturesImplementation
     }
     INDUSTRIAL_PREPROC_MODEL = {
+        # data filtration
+        'channel_filtration': ChannelCentroidFilter,
         # data projection onto different basis
         'eigen_basis': EigenBasisImplementation,
         'wavelet_basis': WaveletBasisImplementation,
         'fourier_basis': FourierBasisImplementation,
         # feature extraction algorithm
         'recurrence_extractor': RecurrenceExtractor,
         'quantile_extractor': QuantileExtractor,
+        'riemann_extractor': RiemannExtractor,
+        # feature generation
+        'topological_extractor': TopologicalFeaturesImplementation,
         # nn feature extraction algorithm
         'minirocket_extractor': MiniRocketExtractor,
+        # 'chronos_extractor': ChronosExtractor,
         # isolation_forest forest
         'isolation_forest_class': IsolationForestClassImplementation,
         'isolation_forest_reg': IsolationForestRegImplementation,
     }
 
     SKLEARN_REG_MODELS = {
         # boosting models (bid datasets)
@@ -164,24 +172,23 @@
 
     FORECASTING_MODELS = {
         # boosting models (bid datasets)
         'ar': AutoRegImplementation,
         'stl_arima': STLForecastARIMAImplementation,
         'ets': ExpSmoothingImplementation,
         'cgru': CGRUImplementation,
-        'glm': GLMImplementation,
-        'locf': RepeatLastValueImplementation,
-        'ssa_forecaster': SSAForecasterImplementation
+        'glm': GLMIndustrial
     }
 
     FORECASTING_PREPROC = {
         'lagged': LaggedTransformationImplementation,
         'sparse_lagged': SparseLaggedTransformationImplementation,
         'smoothing': TsSmoothingImplementation,
-        'gaussian_filter': GaussianFilterImplementation
+        'gaussian_filter': GaussianFilterImplementation,
+        'exog_ts': ExogDataTransformationImplementation,
     }
 
     NEURAL_MODEL = {
         # fundamental models
         'inception_model': InceptionTimeModel,
         'omniscale_model': OmniScaleModel,
         'resnet_model': ResNetModel,
@@ -196,24 +203,27 @@
     operation_dict = {'regression': SKLEARN_REG_MODELS.keys(),
                       'ts_forecasting': FORECASTING_MODELS.keys(),
                       'classification': SKLEARN_CLF_MODELS.keys()}
 
     if problem == 'ts_forecasting':
         available_operations = [operation_dict[problem],
                                 FORECASTING_PREPROC.keys(),
-                                SKLEARN_REG_MODELS.keys()
+                                SKLEARN_REG_MODELS.keys(),
+                                INDUSTRIAL_PREPROC_MODEL.keys(),
                                 ]
     else:
         available_operations = [operation_dict[problem],
                                 NEURAL_MODEL.keys(),
                                 INDUSTRIAL_PREPROC_MODEL.keys(),
                                 FEDOT_PREPROC_MODEL.keys()]
 
-    available_operations = list(chain(*[list(x) for x in available_operations]))
-    excluded_operations = list(chain(*[list(TEMPORARY_EXCLUDED[x]) for x in TEMPORARY_EXCLUDED.keys()]))
+    available_operations = list(
+        chain(*[list(x) for x in available_operations]))
+    excluded_operations = list(
+        chain(*[list(TEMPORARY_EXCLUDED[x]) for x in TEMPORARY_EXCLUDED.keys()]))
     available_operations = [x for x in available_operations
                             if x not in EXCLUDED_OPERATION_MUTATION[problem] and x not in excluded_operations]
     return available_operations
 
 
 INDUSTRIAL_PREPROC_MODEL = AtomizedModel.INDUSTRIAL_PREPROC_MODEL.value
 INDUSTRIAL_CLF_PREPROC_MODEL = AtomizedModel.INDUSTRIAL_CLF_PREPROC_MODEL.value
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/core/tuning/search_space.py` & `fedot_ind-0.4.2/fedot_ind/core/tuning/search_space.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from functools import partial
 
 from hyperopt import hp
 
+from fedot_ind.core.repository.constanst_repository import DISTANCE_METRICS
+
 NESTED_PARAMS_LABEL = 'nested_label'
 
 industrial_search_space = {
     'eigen_basis':
         {'window_size': {'hyperopt-dist': hp.choice, 'sampling-scope': [[x for x in range(5, 50, 5)]]},
          'stride': {'hyperopt-dist': hp.choice, 'sampling-scope': [[x for x in range(1, 10, 1)]]},
          'rank_regularization': {'hyperopt-dist': hp.choice, 'sampling-scope': [
@@ -19,26 +21,54 @@
                        'sampling-scope': [10000, 50000]}},
     'topological_extractor':
         {'window_size': {'hyperopt-dist': hp.choice, 'sampling-scope': [[x for x in range(5, 50, 5)]]},
          'stride': {'hyperopt-dist': hp.choice, 'sampling-scope': [[x for x in range(1, 10, 1)]]}},
     'quantile_extractor':
         {'stride': {'hyperopt-dist': hp.choice, 'sampling-scope': [[x for x in range(1, 10, 1)]]},
          'window_size': {'hyperopt-dist': hp.choice, 'sampling-scope': [[x for x in range(0, 50, 3)]]}},
+    'riemann_extractor':
+        {'estimator': {'hyperopt-dist': hp.choice, 'sampling-scope': [['corr',
+                                                                       'cov', 'lwf', 'mcd', 'hub']]},
+         'tangent_metric': {'hyperopt-dist': hp.choice, 'sampling-scope': [[
+             'euclid',
+             'logeuclid',
+             'riemann'
+         ]]},
+         'SPD_metric': {'hyperopt-dist': hp.choice, 'sampling-scope': [[
+             # 'ale',
+             # 'alm',
+             'euclid',
+             'identity',
+             'logeuclid', 'riemann']]}},
     'recurrence_extractor':
         {'window_size': {'hyperopt-dist': hp.choice, 'sampling-scope': [[x for x in range(5, 50, 5)]]},
          'stride': {'hyperopt-dist': hp.choice, 'sampling-scope': [[x for x in range(1, 10, 1)]]},
          # 'rec_metric': (hp.choice, [['chebyshev', 'cosine', 'euclidean', 'mahalanobis']])
          },
     'signal_extractor':
         {'n_components': {'hyperopt-dist': hp.uniformint, 'sampling-scope': [2, 10]},
          'wavelet': {'hyperopt-dist': hp.choice,
                      'sampling-scope': [['mexh', 'morl', 'db5', 'sym5']]}},
+    'channel_filtration':
+        {'distance': {'hyperopt-dist': hp.choice,
+                      'sampling-scope': [['manhattan', 'euclidean', 'chebyshev']]},
+         'centroid_metric': {'hyperopt-dist': hp.choice,
+                             'sampling-scope': [['manhattan', 'euclidean', 'chebyshev']]},
+         'sample_metric': {'hyperopt-dist': hp.choice,
+                           'sampling-scope': [list(DISTANCE_METRICS.keys())]},
+
+         'selection_strategy': {'hyperopt-dist': hp.choice,
+                                'sampling-scope': [['sum', 'pairwise']]}
+         },
     'minirocket_extractor':
         {'num_features': {'hyperopt-dist': hp.choice,
                           'sampling-scope': [[x for x in range(5000, 20000, 1000)]]}},
+    'chronos_extractor':
+        {'num_features': {'hyperopt-dist': hp.choice,
+                          'sampling-scope': [[x for x in range(5000, 20000, 1000)]]}},
     'patch_tst_model':
         {'epochs': {'hyperopt-dist': hp.choice, 'sampling-scope': [[x for x in range(10, 100, 10)]]},
          'batch_size': {'hyperopt-dist': hp.choice, 'sampling-scope': [[x for x in range(8, 64, 6)]]},
          'activation': {'hyperopt-dist': hp.choice,
                         'sampling-scope': [
                             ['LeakyReLU', 'ELU', 'SwishBeta', 'ReLU', 'Tanh', 'Softmax', 'SmeLU', 'Mish']]}},
     'omniscale_model':
@@ -197,30 +227,42 @@
                 'type': 'continuous'},
             'min_child_weight': {
                 'hyperopt-dist': hp.uniformint,
                 'sampling-scope': [1, 21],
                 'type': 'discrete'},
         },
         'xgboost': {
+            'n_estimators': {
+                'hyperopt-dist': hp.uniformint,
+                'sampling-scope': [100, 3000],
+                'type': 'discrete'},
             'max_depth': {
                 'hyperopt-dist': hp.uniformint,
-                'sampling-scope': [1, 7],
+                'sampling-scope': [3, 10],
                 'type': 'discrete'},
             'learning_rate': {
                 'hyperopt-dist': hp.loguniform,
                 'sampling-scope': [1e-3, 1],
                 'type': 'continuous'},
             'subsample': {
                 'hyperopt-dist': hp.uniform,
                 'sampling-scope': [0.05, 0.99],
                 'type': 'continuous'},
-            'min_child_weight': {
-                'hyperopt-dist': hp.uniformint,
-                'sampling-scope': [1, 21],
-                'type': 'discrete'}
+            'min_weight_fraction_leaf': {
+                'hyperopt-dist': hp.uniform,
+                'sampling-scope': [0.0, 0.5],
+                'type': 'continuous'},
+            'min_samples_leaf': {
+                'hyperopt-dist': hp.uniform,
+                'sampling-scope': [0.0, 1],
+                'type': 'continuous'},
+            'min_samples_split': {
+                'hyperopt-dist': hp.uniform,
+                'sampling-scope': [0.0, 1.0],
+                'type': 'continuous'}
         },
         'svr': {
             'C': {
                 'hyperopt-dist': hp.uniform,
                 'sampling-scope': [1e-4, 25.0],
                 'type': 'continuous'},
             'epsilon': {
@@ -363,14 +405,19 @@
                 'hyperopt-dist': hp.uniform,
                 'sampling-scope': [2, 200],
                 'type': 'continuous'},
             'lag_2': {
                 'hyperopt-dist': hp.uniform,
                 'sampling-scope': [2, 800],
                 'type': 'continuous'}
+            ,
+            'trend': {
+                'hyperopt-dist': hp.choice,
+                'sampling-scope': [['n', 'c', 't', 'ct']],
+                'type': 'categorical'}
         },
         'ets': {
             'error': {
                 'hyperopt-dist': hp.choice,
                 'sampling-scope': [["add", "mul"]],
                 'type': 'categorical'},
             'trend': {
@@ -453,15 +500,15 @@
                 'sampling-scope': [['adamw', 'sgd']],
                 'type': 'categorical'},
             'loss': {
                 'hyperopt-dist': hp.choice,
                 'sampling-scope': [['mae', 'mse']],
                 'type': 'categorical'},
         },
-        'topological_features': {
+        'topological_extractor': {
             'window_size_as_share': {
                 'hyperopt-dist': hp.uniform,
                 'sampling-scope': [0.1, 0.9],
                 'type': 'continuous'
             },
             'max_homology_dimension': {
                 'hyperopt-dist': hp.uniformint,
@@ -485,124 +532,14 @@
                 'sampling-scope': [1, 20],
                 'type': 'discrete'},
             'kernel': {
                 'hyperopt-dist': hp.choice,
                 'sampling-scope': [['linear', 'poly', 'rbf', 'sigmoid', 'cosine', 'precomputed']],
                 'type': 'categorical'}
         },
-        'fast_ica': {
-            'n_components': {
-                'hyperopt-dist': hp.uniformint,
-                'sampling-scope': [1, 20],
-                'type': 'discrete'},
-            'fun': {
-                'hyperopt-dist': hp.choice,
-                'sampling-scope': [['logcosh', 'exp', 'cube']],
-                'type': 'categorical'}
-        },
-        'ransac_lin_reg': {
-            'min_samples': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [0.1, 0.9],
-                'type': 'continuous'},
-            'residual_threshold': {
-                'hyperopt-dist': hp.loguniform,
-                'sampling-scope': [0.1, 1000],
-                'type': 'continuous'},
-            'max_trials': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [50, 500],
-                'type': 'continuous'},
-            'max_skips': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [50, 500000],
-                'type': 'continuous'}
-        },
-        'ransac_non_lin_reg': {
-            'min_samples': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [0.1, 0.9],
-                'type': 'continuous'},
-            'residual_threshold': {
-                'hyperopt-dist': hp.loguniform,
-                'sampling-scope': [0.1, 1000],
-                'type': 'continuous'},
-            'max_trials': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [50, 500],
-                'type': 'continuous'},
-            'max_skips': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [50, 500000],
-                'type': 'continuous'}
-        },
-        'isolation_forest_reg': {
-            'max_samples': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [0.05, 0.99],
-                'type': 'continuous'},
-            'max_features': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [0.05, 0.99],
-                'type': 'continuous'},
-            'bootstrap': {
-                'hyperopt-dist': hp.choice,
-                'sampling-scope': [[True, False]],
-                'type': 'categorical'}
-        },
-        'isolation_forest_class': {
-            'max_samples': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [0.05, 0.99],
-                'type': 'continuous'},
-            'max_features': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [0.05, 0.99],
-                'type': 'continuous'},
-            'bootstrap': {
-                'hyperopt-dist': hp.choice,
-                'sampling-scope': [[True, False]],
-                'type': 'categorical'}
-        },
-        'rfe_lin_reg': {
-            'n_features_to_select': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [0.5, 0.9],
-                'type': 'continuous'},
-            'step': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [0.1, 0.2],
-                'type': 'continuous'}
-        },
-        'rfe_non_lin_reg': {
-            'n_features_to_select': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [0.5, 0.9],
-                'type': 'continuous'},
-            'step': {
-                'hyperopt-dist': hp.uniform,
-                'sampling-scope': [0.1, 0.2],
-                'type': 'continuous'}
-        },
-        'poly_features': {
-            'degree': {
-                'hyperopt-dist': hp.uniformint,
-                'sampling-scope': [2, 5],
-                'type': 'discrete'},
-            'interaction_only': {
-                'hyperopt-dist': hp.choice,
-                'sampling-scope': [[True, False]],
-                'type': 'categorical'}
-        },
-        'polyfit': {
-            'degree': {
-                'hyperopt-dist': hp.uniformint,
-                'sampling-scope': [1, 6],
-                'type': 'discrete'}
-        },
         'lagged': {
             'window_size': {
                 'hyperopt-dist': hp.uniformint,
                 'sampling-scope': [5, 500],
                 'type': 'discrete'}
         },
         'sparse_lagged': {
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/tools/explain/distances.py` & `fedot_ind-0.4.2/fedot_ind/tools/explain/distances.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/tools/explain/explain.py` & `fedot_ind-0.4.2/fedot_ind/tools/explain/explain.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/tools/loader.py` & `fedot_ind-0.4.2/fedot_ind/tools/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 import shutil
 import urllib.request as request
 import zipfile
 from pathlib import Path
 
 import chardet
 import pandas as pd
+from datasets import load_dataset
 from datasetsforecast.m3 import M3
 # from datasetsforecast.m4 import M4
 from datasetsforecast.m5 import M5
 from scipy.io.arff import loadarff
-from sktime.datasets._data_io import load_from_tsfile_to_dataframe
+from sktime.datasets import load_from_tsfile_to_dataframe
 from tqdm import tqdm
 
 from fedot_ind.api.utils.path_lib import PROJECT_PATH
-from fedot_ind.core.repository.constanst_repository import M4_PREFIX
 from fedot_ind.core.architecture.settings.computational import backend_methods as np
+from fedot_ind.core.repository.constanst_repository import M4_PREFIX
 
 
 class DataLoader:
     """Class for reading data files and downloading from UCR archive if not found locally.
     At the moment supports ``.ts``, ``.txt``, ``.tsv``, and ``.arff`` formats.
 
     Args:
@@ -35,29 +36,30 @@
     def __init__(self, dataset_name: str, folder: str = None):
         self.logger = logging.getLogger('DataLoader')
         self.dataset_name = dataset_name
         self.folder = folder
         self.forecast_data_source = {'M3': M3.load,
                                      # 'M4': M4.load,
                                      'M4': self.local_m4_load,
-                                     'M5': M5.load
+                                     'M5': M5.load,
+                                     'monash_tsf': load_dataset
                                      }
 
-    def load_forecast_data(self):
-        loader = self.forecast_data_source['M4']
+    def load_forecast_data(self, folder=None):
+        loader = self.forecast_data_source[folder]
         group_df = loader(directory='data',
                           group=f'{M4_PREFIX[self.dataset_name[0]]}')
         # 'M3_Monthly_M10'
         ts_df = group_df[group_df['label'] == self.dataset_name]
         del ts_df['label']
         ts_df = ts_df.set_index(
             'datetime') if 'datetime' in ts_df.columns else ts_df.set_index('idx')
-        return ts_df
+        return ts_df, None
 
-    def local_m4_load(self, directory, group):
+    def local_m4_load(self, directory='data', group=None):
         path_to_result = PROJECT_PATH + '/examples/data/forecasting/'
         for result_cvs in os.listdir(path_to_result):
             if result_cvs.__contains__(group):
                 return pd.read_csv(Path(path_to_result, result_cvs))
 
     def load_data(self, shuffle=True) -> tuple:
         """Load data for classification experiment locally or externally from UCR archive.
@@ -87,25 +89,38 @@
 
             url = f"http://www.timeseriesclassification.com/aeon-toolkit/{dataset_name}.zip"
             request.urlretrieve(url, download_path + filename)
             try:
                 zipfile.ZipFile(
                     download_path + filename).extractall(temp_data_path + dataset_name)
             except zipfile.BadZipFile:
-                self.logger.error(
+                raise FileNotFoundError(
                     f'Cannot extract data: {dataset_name} dataset not found in UCR archive')
-                return None, None
 
             self.logger.info(f'{dataset_name} data downloaded. Unpacking...')
             train_data, test_data = self.extract_data(
                 dataset_name, temp_data_path)
 
             shutil.rmtree(cache_path)
-            return train_data, test_data
+
+            # if type(train_data[0])
+
+            # return train_data, test_data
         self.logger.info('Data read successfully from local folder')
+
+        if isinstance(train_data[0].iloc[0, 0], pd.Series):
+            def convert(arr):
+                """Transform pd.Series values to np.ndarray"""
+                return np.array([d.values for d in arr])
+
+            train_data = (np.apply_along_axis(
+                convert, 1, train_data[0]), train_data[1])
+            test_data = (np.apply_along_axis(
+                convert, 1, test_data[0]), test_data[1])
+
         return train_data, test_data
 
     def read_train_test_files(self, data_path, dataset_name, shuffle=True):
 
         file_path = data_path + '/' + dataset_name + f'/{dataset_name}_TRAIN'
         # If data unpacked as .tsv file
         if os.path.isfile(file_path + '.tsv'):
@@ -135,14 +150,19 @@
         elif os.path.isfile(file_path + '.arff'):
             self.logger.info(
                 f'Reading data from {data_path + "/" + dataset_name}')
             x_train, y_train, x_test, y_test = self.read_arff_files(
                 dataset_name, data_path)
             is_multi = True
 
+        elif os.path.isfile(file_path + '.csv'):
+            self.logger.info(
+                f'Reading data from {data_path + "/" + dataset_name}')
+            df = pd.read_csv(file_path + '.csv')
+
         else:
             self.logger.error(
                 f'Data not found in {data_path + "/" + dataset_name}')
             return None, None, None
 
         y_train, y_test = convert_type(y_train, y_test)
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/tools/synthetic/anomalies.py` & `fedot_ind-0.4.2/fedot_ind/tools/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/tools/synthetic/anomaly_generator.py` & `fedot_ind-0.4.2/fedot_ind/tools/synthetic/anomaly_generator.py`

 * *Files identical despite different names*

### Comparing `fedot_ind-0.4.1.2/fedot_ind/tools/synthetic/ts_datasets_generator.py` & `fedot_ind-0.4.2/fedot_ind/tools/synthetic/ts_datasets_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,11 +87,11 @@
         ts_frame.reset_index(drop=True, inplace=True)
         X_train, X_test, y_train, y_test = train_test_split(
             ts_frame, labels, test_size=self.test_size, random_state=42, shuffle=True)
         return (X_train, y_train), (X_test, y_test)
 
     def create_features(self, n_samples, ts_length, multivariate):
         features = pd.DataFrame(np.random.random((n_samples, ts_length)))
-        # TODO: add option to select dimentions
+        # TODO: add option to select dimensions
         if multivariate:
-            features = features.apply(lambda x: pd.Series([x, x, x]), axis=1)
+            features = np.random.rand(n_samples, 3, ts_length)
         return features
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind/tools/synthetic/ts_generator.py` & `fedot_ind-0.4.2/fedot_ind/tools/synthetic/ts_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         if window_size < order + 2:
             raise TypeError(
                 "window_size is too small for the polynomials order")
         order_range = range(order + 1)
         half_window = (window_size - 1) // 2
         # precompute coefficients
         b = np.mat([[k ** i for i in order_range]
-                   for k in range(-half_window, half_window + 1)])
+                    for k in range(-half_window, half_window + 1)])
         m = np.linalg.pinv(b).A[deriv] * rate ** deriv * factorial(deriv)
         # pad the signal at the extremes with
         # values taken from the signal itself
         firstvals = y[0] - np.abs(y[1:half_window + 1][::-1] - y[0])
         lastvals = y[-1] + np.abs(y[-half_window - 1:-1][::-1] - y[-1])
         y = np.concatenate((firstvals, y, lastvals))
         return np.convolve(m[::-1], y, mode='valid')
```

### Comparing `fedot_ind-0.4.1.2/fedot_ind.egg-info/PKG-INFO` & `fedot_ind-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 Metadata-Version: 2.1
-Name: fedot_ind
-Version: 0.4.1.2
-Summary: Automated machine learning framework for time series analysis
-Home-page: https://github.com/aimclub/Fedot.Industrial
+Name: fedot-ind
+Version: 0.4.2
+Summary: Time series analysis framework
+License: BSD 3-Clause
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
-License: BSD 3-Clause
-Keywords: automated machine learning,time series analysis,anomaly detection,classification
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.9,<3.12
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyMonad (==2.4.0)
+Requires-Dist: PyWavelets (==1.4.1)
+Requires-Dist: catboost (==1.1.1) ; sys_platform == "darwin"
+Requires-Dist: chardet (>=5.2.0,<5.3.0)
+Requires-Dist: datasets (>=2.18.0,<3.0.0)
+Requires-Dist: datasetsforecast (>=0.0.8,<0.1.0)
+Requires-Dist: distributed (>=2023.12.0,<2023.13.0)
+Requires-Dist: fastai (>=2.7.14,<2.8.0)
+Requires-Dist: fastcore (>=1.5.29,<1.6.0)
+Requires-Dist: fedot (>=0.7.3.1,<0.8.0.0)
+Requires-Dist: giotto_tda (==0.6.0)
+Requires-Dist: librosa (>=0.10.1,<0.11.0)
+Requires-Dist: matplotlib (>=3.8.2,<3.9.0)
+Requires-Dist: mklpy (==0.6)
+Requires-Dist: pillow (>=10.2.0,<10.3.0)
+Requires-Dist: pyriemann (>=0.5,<0.6)
+Requires-Dist: ripser (==0.6.4)
+Requires-Dist: scipy (>=1.10.0)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
+Requires-Dist: sktime (>=0.16.1)
+Requires-Dist: statsforecast (==1.5.0)
+Requires-Dist: tensorly (==0.8.1)
+Requires-Dist: torch (>=2.2.0,<2.3.0)
+Requires-Dist: torchvision (>=0.17.0,<0.18.0)
+Requires-Dist: tqdm (>=4.65.2,<4.66.0)
 Description-Content-Type: text/x-rst
-License-File: LICENSE.md
-Requires-Dist: fedot
-Requires-Dist: catboost==1.1.1; sys_platform == "darwin"
-Requires-Dist: MKLpy==0.6
-Requires-Dist: PyMonad==2.4.0
-Requires-Dist: PyWavelets==1.4.1
-Requires-Dist: giotto_tda==0.6.0
-Requires-Dist: ripser==0.6.4
-Requires-Dist: fastcore
-Requires-Dist: fastai
-Requires-Dist: distributed
-Requires-Dist: datasetsforecast
-Requires-Dist: tensorly==0.8.1
-Requires-Dist: torch==2.0.0
-Requires-Dist: torchvision==0.15.1
-Requires-Dist: statsforecast==1.5.0
-Requires-Dist: chardet
 
 .. image:: /docs/img/fedot-industrial.png
     :width: 600px
     :align: center
     :alt: Fedot Industrial logo
 
 
@@ -90,15 +97,15 @@
     :target: https://mybinder.org/v2/gh/aimclub/Fedot.Industrial/HEAD
 
 .. |downloads| image:: https://static.pepy.tech/personalized-badge/fedot-ind?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
     :target: https://pepy.tech/project/fedot-ind
     :alt: Downloads
 
 .. |support| image:: https://img.shields.io/badge/Telegram-Group-blue.svg
-    :target: https://t.me/fedotindustrial_support
+    :target: https://t.me/FEDOT_helpdesk
     :alt: Support
 
 .. |rus| image:: https://img.shields.io/badge/lang-ru-yellow.svg
     :target: /README.rst
 
 .. |eng| image:: https://img.shields.io/badge/lang-eng-green.svg
     :target: /README_en.rst
@@ -483,7 +490,8 @@
 
 
 .. _AutoML framework FEDOT: https://github.com/aimclub/FEDOT
 .. _UCR archive: https://www.cs.ucr.edu/~eamonn/time_series_data/
 .. _main branch: https://github.com/aimclub/Fedot.Industrial
 .. _readthedocs: https://fedotindustrial.readthedocs.io/en/latest/
 .. _examples: https://github.com/aimclub/Fedot.Industrial/tree/main/examples
+
```

