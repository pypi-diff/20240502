# Comparing `tmp/signxai-1.1.7.tar.gz` & `tmp/signxai-1.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signxai-1.1.7.tar", last modified: Thu Apr 11 12:39:08 2024, max compression
+gzip compressed data, was "signxai-1.1.7.1.tar", last modified: Thu May  2 14:28:32 2024, max compression
```

## Comparing `signxai-1.1.7.tar` & `signxai-1.1.7.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.619897 signxai-1.1.7/
--rw-rw-r--   0 nils      (1000) nils      (1000)     2182 2023-09-21 10:27:45.000000 signxai-1.1.7/LICENSE
--rw-rw-r--   0 nils      (1000) nils      (1000)       33 2023-09-21 10:27:45.000000 signxai-1.1.7/MANIFEST.in
--rw-r--r--   0 nils      (1000) nils      (1000)     5671 2024-04-11 12:39:08.619897 signxai-1.1.7/PKG-INFO
--rw-r--r--   0 nils      (1000) nils      (1000)     4726 2023-09-11 10:28:19.000000 signxai-1.1.7/README.md
--rw-rw-r--   0 nils      (1000) nils      (1000)       38 2024-04-11 12:39:08.619897 signxai-1.1.7/setup.cfg
--rw-r--r--   0 nils      (1000) nils      (1000)     2054 2024-04-11 12:38:54.000000 signxai-1.1.7/setup.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.571897 signxai-1.1.7/signxai/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.583897 signxai-1.1.7/signxai/examples/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/examples/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1595 2024-04-03 13:56:13.000000 signxai-1.1.7/signxai/examples/mnist.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1602 2023-11-01 13:52:51.000000 signxai-1.1.7/signxai/examples/vgg16.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.587897 signxai-1.1.7/signxai/methods/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)     4610 2023-09-22 12:44:38.000000 signxai-1.1.7/signxai/methods/grad_cam.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1499 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/guided_backprop.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.591897 signxai-1.1.7/signxai/methods/innvestigate/
--rw-r--r--   0 nils      (1000) nils      (1000)      216 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.599897 signxai-1.1.7/signxai/methods/innvestigate/analyzer/
--rw-r--r--   0 nils      (1000) nils      (1000)     4442 2023-11-01 13:51:48.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)    20907 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/base.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.599897 signxai-1.1.7/signxai/methods/innvestigate/analyzer/canonization/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/canonization/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)    15327 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/deeplift.py
--rw-r--r--   0 nils      (1000) nils      (1000)     7094 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/deeptaylor.py
--rw-r--r--   0 nils      (1000) nils      (1000)    14700 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/gradient_based.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1948 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/misc.py
--rw-r--r--   0 nils      (1000) nils      (1000)     8539 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/pattern_based.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.603897 signxai-1.1.7/signxai/methods/innvestigate/analyzer/relevance_based/
--rw-r--r--   0 nils      (1000) nils      (1000)       65 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/relevance_based/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)    24163 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py
--rw-r--r--   0 nils      (1000) nils      (1000)    52929 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py
--rw-r--r--   0 nils      (1000) nils      (1000)     3842 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/relevance_based/utils.py
--rw-r--r--   0 nils      (1000) nils      (1000)    26365 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/reverse_map.py
--rw-r--r--   0 nils      (1000) nils      (1000)    13638 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/analyzer/wrapper.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.603897 signxai-1.1.7/signxai/methods/innvestigate/applications/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/applications/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)    10473 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/applications/imagenet.py
--rw-r--r--   0 nils      (1000) nils      (1000)     4256 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/applications/mnist.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.607897 signxai-1.1.7/signxai/methods/innvestigate/backend/
--rw-r--r--   0 nils      (1000) nils      (1000)     1234 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/backend/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/backend/tensorflow.py
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/backend/torch.py
--rw-r--r--   0 nils      (1000) nils      (1000)    19365 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/layers.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.607897 signxai-1.1.7/signxai/methods/innvestigate/tests/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.611897 signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)     4878 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_base.py
--rw-r--r--   0 nils      (1000) nils      (1000)     3948 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1847 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py
--rw-r--r--   0 nils      (1000) nils      (1000)     7771 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1511 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_init.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1303 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_misc.py
--rw-r--r--   0 nils      (1000) nils      (1000)     3025 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py
--rw-r--r--   0 nils      (1000) nils      (1000)    10210 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py
--rw-r--r--   0 nils      (1000) nils      (1000)     3790 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.611897 signxai-1.1.7/signxai/methods/innvestigate/tests/tools/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/tools/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)    12358 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/tools/test_pattern.py
--rw-r--r--   0 nils      (1000) nils      (1000)     3969 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/tools/test_perturbate.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.611897 signxai-1.1.7/signxai/methods/innvestigate/tests/utils/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/utils/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.611897 signxai-1.1.7/signxai/methods/innvestigate/tests/utils/keras/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/utils/keras/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1759 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/utils/keras/test_graph.py
--rw-r--r--   0 nils      (1000) nils      (1000)      967 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/utils/test_visualizations.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.611897 signxai-1.1.7/signxai/methods/innvestigate/tests/utils/tests/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/utils/tests/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1189 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.615897 signxai-1.1.7/signxai/methods/innvestigate/tools/
--rw-r--r--   0 nils      (1000) nils      (1000)      225 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tools/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)    19540 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tools/pattern.py
--rw-r--r--   0 nils      (1000) nils      (1000)    18118 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/tools/perturbate.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.615897 signxai-1.1.7/signxai/methods/innvestigate/utils/
--rw-r--r--   0 nils      (1000) nils      (1000)     5791 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.615897 signxai-1.1.7/signxai/methods/innvestigate/utils/keras/
--rw-r--r--   0 nils      (1000) nils      (1000)     2318 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/keras/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)     5921 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/keras/backend.py
--rw-r--r--   0 nils      (1000) nils      (1000)    12830 2023-09-21 10:33:03.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/keras/checks.py
--rw-r--r--   0 nils      (1000) nils      (1000)    43869 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/keras/graph.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.615897 signxai-1.1.7/signxai/methods/innvestigate/utils/tests/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/tests/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.619897 signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/
--rw-r--r--   0 nils      (1000) nils      (1000)     2457 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)     3322 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/cnn.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1383 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/helper.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1313 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/mlp.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1634 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/special.py
--rw-r--r--   0 nils      (1000) nils      (1000)     1592 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/trivia.py
--rw-r--r--   0 nils      (1000) nils      (1000)     2818 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/tests/dryrun.py
--rw-r--r--   0 nils      (1000) nils      (1000)     4925 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/innvestigate/utils/visualizations.py
--rw-r--r--   0 nils      (1000) nils      (1000)      253 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/methods/signed.py
--rw-r--r--   0 nils      (1000) nils      (1000)    26122 2023-09-22 12:45:20.000000 signxai-1.1.7/signxai/methods/wrappers.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.619897 signxai-1.1.7/signxai/utils/
--rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/utils/__init__.py
--rw-r--r--   0 nils      (1000) nils      (1000)     2093 2023-09-11 10:28:20.000000 signxai-1.1.7/signxai/utils/utils.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-04-11 12:39:08.619897 signxai-1.1.7/signxai.egg-info/
--rw-r--r--   0 nils      (1000) nils      (1000)     5671 2024-04-11 12:39:08.000000 signxai-1.1.7/signxai.egg-info/PKG-INFO
--rw-rw-r--   0 nils      (1000) nils      (1000)     3732 2024-04-11 12:39:08.000000 signxai-1.1.7/signxai.egg-info/SOURCES.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)        1 2024-04-11 12:39:08.000000 signxai-1.1.7/signxai.egg-info/dependency_links.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)       91 2024-04-11 12:39:08.000000 signxai-1.1.7/signxai.egg-info/requires.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)        8 2024-04-11 12:39:08.000000 signxai-1.1.7/signxai.egg-info/top_level.txt
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.899238 signxai-1.1.7.1/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2182 2023-09-21 10:27:45.000000 signxai-1.1.7.1/LICENSE
+-rw-rw-r--   0 nils      (1000) nils      (1000)       33 2023-09-21 10:27:45.000000 signxai-1.1.7.1/MANIFEST.in
+-rw-r--r--   0 nils      (1000) nils      (1000)    17252 2024-05-02 14:28:32.899238 signxai-1.1.7.1/PKG-INFO
+-rw-r--r--   0 nils      (1000) nils      (1000)    16305 2024-04-30 15:01:54.000000 signxai-1.1.7.1/README.md
+-rw-rw-r--   0 nils      (1000) nils      (1000)       38 2024-05-02 14:28:32.899238 signxai-1.1.7.1/setup.cfg
+-rw-r--r--   0 nils      (1000) nils      (1000)     2056 2024-05-02 14:27:19.000000 signxai-1.1.7.1/setup.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.894238 signxai-1.1.7.1/signxai/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.895238 signxai-1.1.7.1/signxai/examples/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/examples/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1595 2024-04-03 13:56:13.000000 signxai-1.1.7.1/signxai/examples/mnist.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1602 2023-11-01 13:52:51.000000 signxai-1.1.7.1/signxai/examples/vgg16.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.895238 signxai-1.1.7.1/signxai/methods/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     4610 2023-09-22 12:44:38.000000 signxai-1.1.7.1/signxai/methods/grad_cam.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1499 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/guided_backprop.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.895238 signxai-1.1.7.1/signxai/methods/innvestigate/
+-rw-r--r--   0 nils      (1000) nils      (1000)      216 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.896238 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/
+-rw-r--r--   0 nils      (1000) nils      (1000)     4442 2023-11-01 13:51:48.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    20907 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/base.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.896238 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/canonization/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/canonization/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    15327 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/deeplift.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     7094 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/deeptaylor.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    14700 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/gradient_based.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1948 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/misc.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     8539 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/pattern_based.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.896238 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/relevance_based/
+-rw-r--r--   0 nils      (1000) nils      (1000)       65 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/relevance_based/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    24163 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    52929 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     3842 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/relevance_based/utils.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    26365 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/reverse_map.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    13638 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/wrapper.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.896238 signxai-1.1.7.1/signxai/methods/innvestigate/applications/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/applications/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    10473 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/applications/imagenet.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     4256 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/applications/mnist.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.897238 signxai-1.1.7.1/signxai/methods/innvestigate/backend/
+-rw-r--r--   0 nils      (1000) nils      (1000)     1234 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/backend/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/backend/tensorflow.py
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/backend/torch.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    19365 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/layers.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.897238 signxai-1.1.7.1/signxai/methods/innvestigate/tests/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.897238 signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     4878 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_base.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     3948 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1847 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     7771 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1511 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_init.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1303 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_misc.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     3025 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    10210 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     3790 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.897238 signxai-1.1.7.1/signxai/methods/innvestigate/tests/tools/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/tools/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    12358 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/tools/test_pattern.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     3969 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/tools/test_perturbate.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.898238 signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.898238 signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/keras/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/keras/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1759 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/keras/test_graph.py
+-rw-r--r--   0 nils      (1000) nils      (1000)      967 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/test_visualizations.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.898238 signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/tests/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/tests/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1189 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.898238 signxai-1.1.7.1/signxai/methods/innvestigate/tools/
+-rw-r--r--   0 nils      (1000) nils      (1000)      225 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tools/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    19540 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tools/pattern.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    18118 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/tools/perturbate.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.898238 signxai-1.1.7.1/signxai/methods/innvestigate/utils/
+-rw-r--r--   0 nils      (1000) nils      (1000)     5791 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.898238 signxai-1.1.7.1/signxai/methods/innvestigate/utils/keras/
+-rw-r--r--   0 nils      (1000) nils      (1000)     2318 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/keras/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     5921 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/keras/backend.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    12957 2024-04-30 10:32:46.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/keras/checks.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    43869 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/keras/graph.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.898238 signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.899238 signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/
+-rw-r--r--   0 nils      (1000) nils      (1000)     2457 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     3322 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/cnn.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1383 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/helper.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1313 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/mlp.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1634 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/special.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     1592 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/trivia.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     2818 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/dryrun.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     4925 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/innvestigate/utils/visualizations.py
+-rw-r--r--   0 nils      (1000) nils      (1000)      253 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/methods/signed.py
+-rw-r--r--   0 nils      (1000) nils      (1000)    26122 2023-09-22 12:45:20.000000 signxai-1.1.7.1/signxai/methods/wrappers.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.899238 signxai-1.1.7.1/signxai/utils/
+-rw-r--r--   0 nils      (1000) nils      (1000)        0 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/utils/__init__.py
+-rw-r--r--   0 nils      (1000) nils      (1000)     2093 2023-09-11 10:28:20.000000 signxai-1.1.7.1/signxai/utils/utils.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2024-05-02 14:28:32.899238 signxai-1.1.7.1/signxai.egg-info/
+-rw-r--r--   0 nils      (1000) nils      (1000)    17252 2024-05-02 14:28:32.000000 signxai-1.1.7.1/signxai.egg-info/PKG-INFO
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3732 2024-05-02 14:28:32.000000 signxai-1.1.7.1/signxai.egg-info/SOURCES.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)        1 2024-05-02 14:28:32.000000 signxai-1.1.7.1/signxai.egg-info/dependency_links.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)       91 2024-05-02 14:28:32.000000 signxai-1.1.7.1/signxai.egg-info/requires.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)        8 2024-05-02 14:28:32.000000 signxai-1.1.7.1/signxai.egg-info/top_level.txt
```

### Comparing `signxai-1.1.7/LICENSE` & `signxai-1.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/setup.py` & `signxai-1.1.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='signxai',
-    version='1.1.7',
+    version='1.1.7.1',
     packages=['signxai.methods', 'signxai.methods.innvestigate', 'signxai.methods.innvestigate.tests', 'signxai.methods.innvestigate.tests.tools',
               'signxai.methods.innvestigate.tests.utils', 'signxai.methods.innvestigate.tests.utils.keras',
               'signxai.methods.innvestigate.tests.utils.tests', 'signxai.methods.innvestigate.tests.analyzer',
               'signxai.methods.innvestigate.tools', 'signxai.methods.innvestigate.utils', 'signxai.methods.innvestigate.utils.keras',
               'signxai.methods.innvestigate.utils.tests', 'signxai.methods.innvestigate.utils.tests.cases',
               'signxai.methods.innvestigate.backend', 'signxai.methods.innvestigate.analyzer',
               'signxai.methods.innvestigate.analyzer.canonization', 'signxai.methods.innvestigate.analyzer.relevance_based',
```

### Comparing `signxai-1.1.7/signxai/examples/mnist.py` & `signxai-1.1.7.1/signxai/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/examples/vgg16.py` & `signxai-1.1.7.1/signxai/examples/vgg16.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/grad_cam.py` & `signxai-1.1.7.1/signxai/methods/grad_cam.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/guided_backprop.py` & `signxai-1.1.7.1/signxai/methods/guided_backprop.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/__init__.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/base.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/base.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/deeplift.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/deeplift.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/deeptaylor.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/deeptaylor.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/gradient_based.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/gradient_based.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/misc.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/misc.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/pattern_based.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/pattern_based.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/relevance_based/utils.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/relevance_based/utils.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/reverse_map.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/reverse_map.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/analyzer/wrapper.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/analyzer/wrapper.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/applications/imagenet.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/applications/imagenet.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/applications/mnist.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/applications/mnist.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/backend/__init__.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/layers.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/layers.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_base.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_base.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_init.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_init.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_misc.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_misc.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/tools/test_pattern.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/tools/test_pattern.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/tools/test_perturbate.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/tools/test_perturbate.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/utils/keras/test_graph.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/keras/test_graph.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/utils/test_visualizations.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tools/pattern.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tools/pattern.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/tools/perturbate.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/tools/perturbate.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/__init__.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/keras/__init__.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/keras/backend.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/keras/backend.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/keras/checks.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/keras/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         'Minimum',
         'Multiply',
         'Subtract',
         'AlphaDropout',
         'GaussianDropout',
         'GaussianNoise',
         'BatchNormalization',
+        'BatchNorm',
         'AveragePooling1D',
         'AveragePooling2D',
         'AveragePooling3D',
         'GlobalAveragePooling1D',
         'GlobalAveragePooling2D',
         'GlobalAveragePooling3D',
         'GlobalMaxPooling1D',
@@ -177,14 +178,15 @@
         'ActivityRegularization',
         'Dropout',
         'Flatten',
         'Reshape',
         'Add',
         'GaussianNoise',
         'BatchNormalization',
+        'BatchNorm',
     )
     return ACTIVATION_SEARCH_SAFE_LAYERS
 
 
 ###############################################################################
 ###############################################################################
 ###############################################################################
@@ -265,15 +267,19 @@
         'DepthwiseConv2D'
     )
     return isInstanceOf(layer, CONV_LAYERS)
 
 
 def is_batch_normalization_layer(layer, *args, **kwargs):
     """Checks if layer is a batchnorm layer."""
-    return isInstanceOf(layer, 'BatchNormalization')
+    BN_LAYERS = (
+        'BatchNormalization',
+        'BatchNorm',
+    )
+    return isInstanceOf(layer, BN_LAYERS)
 
 
 def is_add_layer(layer, *args, **kwargs):
     """Checks if layer is an addition-merge layer."""
     return isInstanceOf(layer, 'Add')
 
 
@@ -332,14 +338,15 @@
         'Minimum',
         'Multiply',
         'Subtract',
         'AlphaDropout',
         'GaussianDropout',
         'GaussianNoise',
         'BatchNormalization',
+        'BatchNorm',
         'AveragePooling1D',
         'AveragePooling2D',
         'AveragePooling3D',
         'GlobalAveragePooling1D',
         'GlobalAveragePooling2D',
         'GlobalAveragePooling3D',
         'GlobalMaxPooling1D',
```

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/keras/graph.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/keras/graph.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/__init__.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/cnn.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/cnn.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/helper.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/helper.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/mlp.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/mlp.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/special.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/special.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/tests/cases/trivia.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/cases/trivia.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/tests/dryrun.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/tests/dryrun.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/innvestigate/utils/visualizations.py` & `signxai-1.1.7.1/signxai/methods/innvestigate/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/methods/wrappers.py` & `signxai-1.1.7.1/signxai/methods/wrappers.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai/utils/utils.py` & `signxai-1.1.7.1/signxai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `signxai-1.1.7/signxai.egg-info/SOURCES.txt` & `signxai-1.1.7.1/signxai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

