# Comparing `tmp/lm-buddy-0.4.1.tar.gz` & `tmp/lm-buddy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm-buddy-0.4.1.tar", last modified: Mon Apr  1 21:22:26 2024, max compression
+gzip compressed data, was "lm-buddy-0.9.0.tar", last modified: Thu Apr  4 18:54:27 2024, max compression
```

## Comparing `lm-buddy-0.4.1.tar` & `lm-buddy-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18120 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.679905 lm-buddy-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.683905 lm-buddy-0.4.1/src/lm_buddy/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/buddy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.683905 lm-buddy-0.4.1/src/lm_buddy/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/cli/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/cli/finetune.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.687904 lm-buddy-0.4.1/src/lm_buddy/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.687904 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/adapter_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/asset_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/model_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/tokenizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/trainer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/vllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.687904 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/artifact_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/artifact_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/artifact_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/run_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/run_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.687904 lm-buddy-0.4.1/src/lm_buddy/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.687904 lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/lm_harness.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/lm_harness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/src/lm_buddy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18120 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:27.700981 lm-buddy-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18267 2024-04-04 18:54:27.700981 lm-buddy-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:54:27.700981 lm-buddy-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:27.688981 lm-buddy-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:27.692981 lm-buddy-0.9.0/src/lm_buddy/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/buddy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:27.692981 lm-buddy-0.9.0/src/lm_buddy/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/cli/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/cli/finetune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:27.696981 lm-buddy-0.9.0/src/lm_buddy/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/configs/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/configs/huggingface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:27.696981 lm-buddy-0.9.0/src/lm_buddy/configs/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/configs/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/configs/jobs/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/configs/jobs/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/configs/jobs/lm_harness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/configs/jobs/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/configs/jobs/ragas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/configs/vllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/configs/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:27.696981 lm-buddy-0.9.0/src/lm_buddy/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/jobs/asset_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/jobs/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:27.696981 lm-buddy-0.9.0/src/lm_buddy/jobs/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/jobs/evaluation/lm_harness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/jobs/evaluation/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/jobs/evaluation/ragas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/jobs/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:27.696981 lm-buddy-0.9.0/src/lm_buddy/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/tracking/artifact_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/src/lm_buddy/tracking/run_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:27.696981 lm-buddy-0.9.0/src/lm_buddy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18267 2024-04-04 18:54:27.000000 lm-buddy-0.9.0/src/lm_buddy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-04 18:54:27.000000 lm-buddy-0.9.0/src/lm_buddy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:54:27.000000 lm-buddy-0.9.0/src/lm_buddy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 18:54:27.000000 lm-buddy-0.9.0/src/lm_buddy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-04 18:54:27.000000 lm-buddy-0.9.0/src/lm_buddy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 18:54:27.000000 lm-buddy-0.9.0/src/lm_buddy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:54:27.696981 lm-buddy-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 18:54:24.000000 lm-buddy-0.9.0/tests/test_utils.py
```

### Comparing `lm-buddy-0.4.1/LICENSE.md` & `lm-buddy-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.1/PKG-INFO` & `lm-buddy-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lm-buddy
-Version: 0.4.1
+Version: 0.9.0
 Summary: Ray-centric library for finetuning and evaluation of (large) language models.
-Author-email: Sean Friedowitz <sean@mozilla.ai>, Aaron Gonzales <aaron@mozilla.ai>, Vicki Boykis <vicki@mozilla.ai>, Davide Eynard <davide@mozilla.ai>
+Author-email: Sean Friedowitz <sean@mozilla.ai>, Aaron Gonzales <aaron@mozilla.ai>, Vicki Boykis <vicki@mozilla.ai>, Davide Eynard <davide@mozilla.ai>, Imtihan Ahmed <imtihan@mozilla.ai>
 License: 
                                       Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -225,15 +225,18 @@
 Requires-Dist: accelerate==0.26.1
 Requires-Dist: peft==0.7.1
 Requires-Dist: trl==0.7.10
 Requires-Dist: bitsandbytes==0.42.0
 Requires-Dist: lm-eval==0.4.2
 Requires-Dist: einops==0.7.0
 Requires-Dist: fschat==0.2.36
-Requires-Dist: openai==1.3.9
+Requires-Dist: openai==1.14.3
+Requires-Dist: ragas==0.1.5
+Requires-Dist: langchain-community==0.0.29
+Requires-Dist: langchain_openai==0.1.1
 Provides-Extra: ruff
 Requires-Dist: ruff==0.2.1; extra == "ruff"
 Provides-Extra: test
 Requires-Dist: pytest==7.4.3; extra == "test"
 Requires-Dist: pytest-cov==4.1.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: Sphinx==7.2.6; extra == "docs"
```

### Comparing `lm-buddy-0.4.1/README.md` & `lm-buddy-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.1/pyproject.toml` & `lm-buddy-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lm-buddy"
-version = "0.4.1"
+version = "0.9.0"
 authors = [
     { name = "Sean Friedowitz", email = "sean@mozilla.ai" },
     { name = "Aaron Gonzales", email = "aaron@mozilla.ai" },
     { name = "Vicki Boykis", email = "vicki@mozilla.ai" },
     { name = "Davide Eynard", email = "davide@mozilla.ai" },
+    { name = "Imtihan Ahmed", email = "imtihan@mozilla.ai" },
 ]
 description = "Ray-centric library for finetuning and evaluation of (large) language models."
 readme = "README.md"
 license = { file = "LICENSE.md" }
 
 requires-python = ">=3.10,<3.11"
 
@@ -35,15 +36,18 @@
     "peft==0.7.1",
     "trl==0.7.10",
     "bitsandbytes==0.42.0",
     # Evaluation frameworks
     "lm-eval==0.4.2",
     "einops==0.7.0",
     "fschat==0.2.36",
-    "openai==1.3.9",
+    "openai==1.14.3",
+    "ragas==0.1.5",
+    "langchain-community==0.0.29",
+    "langchain_openai==0.1.1",
 ]
 
 [project.optional-dependencies]
 ruff = ["ruff==0.2.1"]
 test = ["pytest==7.4.3", "pytest-cov==4.1.0"]
 docs = [
     "Sphinx==7.2.6",
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/buddy.py` & `lm-buddy-0.9.0/src/lm_buddy/buddy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,72 @@
-from lm_buddy.integrations.wandb import ArtifactLoader, WandbArtifactLoader
-from lm_buddy.jobs._entrypoints import run_finetuning, run_lm_harness, run_prometheus
-from lm_buddy.jobs.common import EvaluationResult, FinetuningResult
-from lm_buddy.jobs.configs import (
+import wandb
+
+from lm_buddy.configs.jobs import (
     EvaluationJobConfig,
     FinetuningJobConfig,
+    JobConfig,
     LMHarnessJobConfig,
     PrometheusJobConfig,
+    RagasJobConfig,
 )
+from lm_buddy.jobs.common import EvaluationResult, FinetuningResult, JobType
+from lm_buddy.jobs.evaluation.lm_harness import run_lm_harness
+from lm_buddy.jobs.evaluation.prometheus import run_prometheus
+from lm_buddy.jobs.evaluation.ragas import run_ragas
+from lm_buddy.jobs.finetuning import run_finetuning
+from lm_buddy.paths import strip_path_prefix
+from lm_buddy.tracking.run_utils import WandbResumeMode
 
 
 class LMBuddy:
     """Your buddy in the (L)LM space.
 
     Simple wrapper around executable functions for tasks available in the library.
     """
 
-    def __init__(self, artifact_loader: ArtifactLoader = WandbArtifactLoader()):
-        self._artifact_loader = artifact_loader
+    # TODO: Store some configuration (e.g., tracking info, name) globally on the buddy
+    def __init__(self):
+        pass
+
+    def _generate_artifact_lineage(
+        self, config: JobConfig, results: list[wandb.Artifact], job_type: JobType
+    ) -> None:
+        """Link input artifacts and log output artifacts to a run.
+
+        A no-op if no tracking config is available.
+        """
+        if config.tracking is not None:
+            with wandb.init(
+                name=config.name,
+                job_type=job_type,
+                resume=WandbResumeMode.ALLOW,
+                **config.tracking.model_dump(),
+            ) as run:
+                for path in config.artifact_paths():
+                    artifact_name = strip_path_prefix(path)
+                    run.use_artifact(artifact_name)
+                for artifact in results:
+                    artifact = run.log_artifact(artifact)
+                    artifact.wait()
 
     def finetune(self, config: FinetuningJobConfig) -> FinetuningResult:
-        """Run a supervised finetuning task with the provided configuration."""
-        finetuning_result = run_finetuning(config, self._artifact_loader)
-        return finetuning_result
+        """Run a supervised finetuning job with the provided configuration."""
+        result = run_finetuning(config)
+        self._generate_artifact_lineage(config, result.artifacts, JobType.FINETUNING)
+        return result
 
     def evaluate(self, config: EvaluationJobConfig) -> EvaluationResult:
-        """Run an evaluation task with the provided configuration.
+        """Run an evaluation job with the provided configuration.
 
         The underlying evaluation framework is determined by the configuration type.
         """
         match config:
             case LMHarnessJobConfig() as lm_harness_config:
-                return run_lm_harness(lm_harness_config, self._artifact_loader)
+                result = run_lm_harness(lm_harness_config)
             case PrometheusJobConfig() as prometheus_config:
-                return run_prometheus(prometheus_config, self._artifact_loader)
+                result = run_prometheus(prometheus_config)
+            case RagasJobConfig() as ragas_config:
+                result = run_ragas(ragas_config)
             case _:
                 raise ValueError(f"Invlid configuration for evaluation: {type(config)}")
+        self._generate_artifact_lineage(config, result.artifacts, JobType.EVALUATION)
+        return result
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/cli/evaluate.py` & `lm-buddy-0.9.0/src/lm_buddy/cli/evaluate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
 
 from lm_buddy import LMBuddy
 from lm_buddy.cli.utils import parse_config_option
-from lm_buddy.jobs.configs import LMHarnessJobConfig, PrometheusJobConfig
+from lm_buddy.configs.jobs import LMHarnessJobConfig, PrometheusJobConfig, RagasJobConfig
 
 
 @click.group(name="evaluate", help="Run an LM Buddy evaluation job.")
 def group() -> None:
     pass
 
 
@@ -20,7 +20,15 @@
 
 @group.command("prometheus", help="Run the prometheus evaluation job.")
 @click.option("--config", type=str)
 def prometheus_command(config: str) -> None:
     config = parse_config_option(PrometheusJobConfig, config)
     buddy = LMBuddy()
     buddy.evaluate(config)
+
+
+@group.command("ragas", help="Run the ragas evaluation job.")
+@click.option("--config", type=str)
+def ragas_command(config: str) -> None:
+    config = parse_config_option(RagasJobConfig, config)
+    buddy = LMBuddy()
+    buddy.evaluate(config)
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/cli/utils.py` & `lm-buddy-0.9.0/src/lm_buddy/cli/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import TypeVar
 
-from lm_buddy.jobs.configs.base import LMBuddyJobConfig
+from lm_buddy.configs.jobs.common import JobConfig
 
-ConfigType = TypeVar("ConfigType", bound=LMBuddyJobConfig)
+ConfigType = TypeVar("ConfigType", bound=JobConfig)
 
 
 def parse_config_option(config_cls: type[ConfigType], config: str) -> ConfigType:
     """Parse the config option string from the CLI.
 
     If it corresponds to a path that exists, attempt to load the config from YAML file.
     If not, attempt to parse it as a JSON string.
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/asset_loader.py` & `lm-buddy-0.9.0/src/lm_buddy/jobs/asset_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,86 +9,81 @@
     AutoModelForCausalLM,
     AutoTokenizer,
     PretrainedConfig,
     PreTrainedModel,
     PreTrainedTokenizer,
 )
 
-from lm_buddy.integrations.huggingface import (
+from lm_buddy.configs.huggingface import (
     AutoModelConfig,
     AutoTokenizerConfig,
     DatasetConfig,
     QuantizationConfig,
 )
-from lm_buddy.integrations.wandb import (
-    ArtifactLoader,
-    WandbArtifactConfig,
-    get_artifact_filesystem_path,
-)
-from lm_buddy.paths import AssetPath, FilePath, HuggingFaceRepoID
-
+from lm_buddy.paths import AssetPath, PathPrefix, strip_path_prefix
+from lm_buddy.tracking.artifact_utils import get_artifact_directory, get_artifact_from_api
 
-def resolve_peft_and_pretrained(path: str) -> tuple[str, str | None]:
-    """Helper method for determining if a path corresponds to a PEFT model.
 
-    A PEFT model contains an `adapter_config.json` in its directory.
-    If this file can be loaded, we know the path is a for a PEFT model.
-    If not, we assume the provided path corresponds to a base HF model.
-
-    Args:
-        path (str): Name/path to a HuggingFace directory
+class HuggingFaceAssetLoader:
+    """Helper class for loading HuggingFace assets from LM Buddy configurations.
 
-    Returns:
-        Tuple of (base model path, optional PEFT path)
+    TODO: We can probably move these to standalone functions now that ArtifactLoader is gone.
+          What if we add other deps (e.g, S3 client in the future?)
     """
-    # We don't know if the checkpoint is adapter weights or merged model weights
-    # Try to load as an adapter and fall back to the checkpoint containing the full model
-    try:
-        peft_config = PeftConfig.from_pretrained(path)
-        return peft_config.base_model_name_or_path, path
-    except ValueError as e:
-        warnings.warn(
-            f"Unable to load model as adapter: {e}. "
-            "This is expected if the checkpoint does not contain adapter weights."
-        )
-        return path, None
 
+    def resolve_asset_path(self, path: AssetPath) -> str:
+        """Resolve an `AssetPath` to a loadable string path.
 
-class HuggingFaceAssetLoader:
-    """Helper class for loading HuggingFace assets from LM Buddy configurations.
+        W&B paths are resolved to file paths given the artifact manifest.
+        The returned string has its `PathPrefix` stripped away..
+        """
+        raw_path = strip_path_prefix(path)
+        if path.startswith((PathPrefix.FILE, PathPrefix.HUGGINGFACE)):
+            return raw_path
+        elif path.startswith(PathPrefix.WANDB):
+            artifact = get_artifact_from_api(raw_path)
+            return str(get_artifact_directory(artifact))
+        else:
+            raise ValueError(f"Unable to resolve asset path from {path}.")
 
-    This class depends on an `ArtifactLoader` in order to resolve actual paths from
-    artifact references.
-    """
+    def resolve_peft_and_pretrained(self, path: AssetPath) -> tuple[str, str | None]:
+        """Helper method for determining if a path corresponds to a PEFT model.
 
-    def __init__(self, artifact_loader: ArtifactLoader):
-        self._artifact_loader = artifact_loader
+        A PEFT model contains an `adapter_config.json` in its directory.
+        If this file can be loaded, we know the path is a for a PEFT model.
+        If not, we assume the provided path corresponds to a base HF model.
 
-    def resolve_asset_path(self, path: AssetPath) -> str:
-        """Resolve the actual HuggingFace name/path from a `LoadableAssetPath`."""
-        match path:
-            case FilePath(value):
-                return str(value)
-            case HuggingFaceRepoID(repo_id):
-                return repo_id
-            case WandbArtifactConfig() as artifact_config:
-                artifact = self._artifact_loader.use_artifact(artifact_config)
-                return str(get_artifact_filesystem_path(artifact))
-            case unknown_path:
-                raise ValueError(f"Unable to resolve asset path from {unknown_path}.")
+        Args:
+            path (AssetPath): Path for the asset with its `PathPrefix` present
+
+        Returns:
+            Tuple of (base model path, optional PEFT path)
+        """
+        # We don't know if the checkpoint is adapter weights or merged model weights
+        # Try to load as an adapter and fall back to the checkpoint containing the full model
+        resolved_path = self.resolve_asset_path(path)
+        try:
+            peft_config = PeftConfig.from_pretrained(resolved_path)
+            return peft_config.base_model_name_or_path, resolved_path
+        except ValueError as e:
+            warnings.warn(
+                f"Unable to load model as adapter: {e}. "
+                "This is expected if the checkpoint does not contain adapter weights."
+            )
+            return resolved_path, None
 
     def load_pretrained_config(
         self,
         config: AutoModelConfig,
     ) -> PretrainedConfig:
         """Load a `PretrainedConfig` from the model configuration.
 
         An exception is raised if the HuggingFace repo does not contain a `config.json` file.
         """
-        config_path = self.resolve_asset_path(config.load_from)
+        config_path = self.resolve_asset_path(config.path)
         return AutoConfig.from_pretrained(pretrained_model_name_or_path=config_path)
 
     def load_pretrained_model(
         self,
         config: AutoModelConfig,
         quantization: QuantizationConfig | None = None,
     ) -> PreTrainedModel:
@@ -108,29 +103,29 @@
                 Accelerator().local_process_index if torch.cuda.is_available() else "cpu"
             )
             device_map = {"": current_device}
             print(f"Setting model device_map = {device_map} to enable quantization")
 
         # TODO: HuggingFace has many AutoModel classes with different "language model heads"
         #   Can we abstract this to load with any type of AutoModel class?
-        model_path = self.resolve_asset_path(config.load_from)
+        model_path = self.resolve_asset_path(config.path)
         return AutoModelForCausalLM.from_pretrained(
             pretrained_model_name_or_path=model_path,
             trust_remote_code=config.trust_remote_code,
             torch_dtype=config.torch_dtype,
             quantization_config=bnb_config,
             device_map=device_map,
         )
 
     def load_pretrained_tokenizer(self, config: AutoTokenizerConfig) -> PreTrainedTokenizer:
         """Load a `PreTrainedTokenizer` from the model configuration.
 
         An exception is raised if the HuggingFace repo does not contain a `tokenizer.json` file.
         """
-        tokenizer_path = self.resolve_asset_path(config.load_from)
+        tokenizer_path = self.resolve_asset_path(config.path)
         tokenizer = AutoTokenizer.from_pretrained(
             pretrained_model_name_or_path=tokenizer_path,
             trust_remote_code=config.trust_remote_code,
             use_fast=config.use_fast,
         )
         if tokenizer.pad_token_id is None:
             # Pad token required for generating consistent batch sizes
@@ -140,17 +135,17 @@
     def load_dataset(self, config: DatasetConfig) -> Dataset:
         """Load a HuggingFace `Dataset` from the dataset configuration.
 
         This method always returns a single `Dataset` object.
         When loading from HuggingFace directly, the `Dataset` is for the provided split.
         When loading from disk, the saved files must be for a dataset else an exception is raised.
         """
-        dataset_path = self.resolve_asset_path(config.load_from)
+        dataset_path = self.resolve_asset_path(config.path)
         # Dataset loading requires a different method if from a HF vs. disk
-        if isinstance(config.load_from, HuggingFaceRepoID):
+        if config.path.startswith(PathPrefix.HUGGINGFACE):
             return load_dataset(dataset_path, split=config.split)
         else:
             match load_from_disk(dataset_path):
                 case Dataset() as dataset:
                     return dataset
                 case other:
                     raise ValueError(
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/integrations/vllm.py` & `lm-buddy-0.9.0/src/lm_buddy/configs/vllm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
+from lm_buddy.configs.common import LMBuddyConfig
 from lm_buddy.paths import AssetPath
-from lm_buddy.types import BaseLMBuddyConfig
 
 
-class InferenceServerConfig(BaseLMBuddyConfig):
+class InferenceServerConfig(LMBuddyConfig):
     """Generic configuration for an externally hosted inference endpoint.
 
     The inference server is defined by an endpoint with the provided `base_url`.
     The model `engine` powering the endpoint can also be specified
     to provide further metadata about the model used for inference
     (e.g., for generating W&B artifact lineages).
 
     Note: This configuration is intended to be generic and not bound to the interface
     of any specific training/evaluation framework. See `LocalChatCompletionConfig`
     or `vLLMCompleptionsConfig` for intended usage alongside a third-party framework.
     """
 
     base_url: str
-    engine: str | AssetPath | None = None
+    engine: AssetPath
 
 
-class VLLMCompletionsConfig(BaseLMBuddyConfig):
+class VLLMCompletionsConfig(LMBuddyConfig):
     """Configuration for a vLLM-based completions service
 
     The "local-chat-completions" model is powered by a self-hosted inference server,
     specified as an `InferenceServerConfig`. Additional arguments are also provided
     to control the tokenizer type and generation parameters.
 
     Note that this is just a subset of the parameters allowed by a vLLM server (see
     https://github.com/vllm-project/vllm/blob/main/vllm/sampling_params.py). If we
     choose to use this configuration to cover for more use cases, it will make sense
     to add the other supported configuration parameters too.
     """
 
     inference: InferenceServerConfig
-
     # vLLM-specific params
     best_of: int | None = None
     max_tokens: int | None = None
     frequency_penalty: float | None = None
     temperature: float | None = None
     top_p: float | None = None
+    top_k: int | None = None
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/artifact_utils.py` & `lm-buddy-0.9.0/src/lm_buddy/tracking/artifact_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from enum import Enum
 from pathlib import Path
 from urllib.parse import ParseResult, urlparse
 
 import pandas as pd
 import wandb
 
+from lm_buddy.paths import PathPrefix
+
 
 class ArtifactType(str, Enum):
     """Enumeration of artifact types used by the LM Buddy."""
 
     DATASET = "dataset"
     MODEL = "model"
     TOKENIZER = "tokenizer"
     EVALUATION = "evaluation"
 
 
-class ArtifactURIScheme(str, Enum):
-    """Enumeration of URI schemes to use in a reference artifact."""
+def default_artifact_name(job_name: str, artifact_type: ArtifactType) -> str:
+    """A default name for an artifact based on the job name and type."""
+    return f"{job_name}-{artifact_type}"
 
-    FILE = "file"
-    HTTP = "http"
-    HTTPS = "https"
-    S3 = "s3"
-    GCS = "gs"
 
+def get_artifact_from_api(artifact_name: str) -> wandb.Artifact:
+    """Retrieve an artifact by fully qualified name from the W&B API.
 
-def default_artifact_name(name: str, artifact_type: ArtifactType) -> str:
-    """A default name for an artifact based on the run name and type."""
-    return f"{name}-{artifact_type}"
+    This does not handle linking the artifact to an active run.
+    For that, use `run.use_artifact(artifact_name)`.
+    """
+    api = wandb.Api()
+    return api.artifact(artifact_name)
 
 
-def get_artifact_filesystem_path(
-    artifact: wandb.Artifact,
-    *,
-    download_root_path: str | None = None,
+def get_artifact_directory(
+    artifact: wandb.Artifact, *, download_root_path: str | None = None
 ) -> Path:
     """Get the directory containing the artifact's data.
 
     If the artifact references data already on the filesystem, simply return that path.
     If not, downloads the artifact (with the specified `download_root_path`)
     and returns the newly created artifact directory path.
     """
@@ -75,15 +75,15 @@
         wandb.Artifact: The generated artifact.
     """
     artifact = wandb.Artifact(name=artifact_name, type=artifact_type)
     if reference:
         # Right now, we are assuming a fixed "file" URI scheme
         # We can pass the URI scheme if necessary later
         artifact.add_reference(
-            uri=f"{ArtifactURIScheme.FILE}://{dir_path}",
+            uri=f"{PathPrefix.FILE}{dir_path}",
             max_objects=max_objects,
             name=entry_name,
         )
     else:
         artifact.add_dir(str(dir_path), name=entry_name)
     return artifact
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/run_config.py` & `lm-buddy-0.9.0/src/lm_buddy/configs/wandb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,76 +1,73 @@
 import os
 import warnings
 
 from pydantic import model_validator
 from wandb.apis.public import Run
 from wandb.util import random_string
 
-from lm_buddy.types import BaseLMBuddyConfig
+from lm_buddy.configs.common import LMBuddyConfig
 
 
-class WandbRunConfig(BaseLMBuddyConfig):
+class WandbRunConfig(LMBuddyConfig):
     """Configuration required to log to a W&B run.
 
-    A W&B Run is uniquely identified by the combination of `entity/project/run_id`.
+    A W&B Run is uniquely identified by the combination of `<entity>/<project>/<id>`.
     The W&B platform will auto-generate values for these variables if they are not provided
     when you initialize a run.
 
     However, based on how these attributes are passed between jobs it is often necessary
     to know the run ID before initializing a run.
     For this reason, the run ID field is made non-optional and auto-generated locally
     if it is not provided.
     """
 
-    __match_args__ = ("run_id", "name", "project", "run_group", "entity")
+    __match_args__ = ("id", "project", "group", "entity")
 
-    run_id: str
-    name: str | None = None
+    id: str
     project: str | None = None
-    run_group: str | None = None
+    group: str | None = None
     entity: str | None = None
 
     @model_validator(mode="before")
     def warn_missing_api_key(cls, values):
         if not os.environ.get("WANDB_API_KEY", None):
             warnings.warn(
                 "Cannot find `WANDB_API_KEY` in your environment. "
                 "Tracking will fail if a default key does not exist on the Ray cluster."
             )
         return values
 
     @model_validator(mode="before")
     def ensure_run_id(cls, values):
-        if values.get("run_id", None) is None:
+        if values.get("id", None) is None:
             # Generate an random 8-digit alphanumeric string, analogous to W&B platform
-            values["run_id"] = random_string(length=8)
+            values["id"] = random_string(length=8)
         return values
 
     @classmethod
     def from_run(cls, run: Run) -> "WandbRunConfig":
         """Extract environment settings from a W&B Run object.
 
         Useful when listing runs from the W&B API and extracting their settings for a job.
         """
         # TODO: Can we get the run group from this when it exists?
         return cls(
-            name=run.name,
             project=run.project,
             entity=run.entity,
-            run_id=run.id,
+            id=run.id,
         )
 
     def wandb_path(self) -> str:
         """String identifier for the asset on the W&B platform."""
-        path = "/".join(x for x in [self.entity, self.project, self.run_id] if x is not None)
+        path = "/".join(x for x in [self.entity, self.project, self.id] if x is not None)
         return path
 
     def env_vars(self) -> dict[str, str]:
         env_vars = {
-            "WANDB_RUN_ID": self.run_id,
-            "WANDB_NAME": self.name,
+            "WANDB_RUN_ID": self.id,
             "WANDB_PROJECT": self.project,
-            "WANDB_RUN_GROUP": self.run_group,
+            "WANDB_RUN_GROUP": self.group,
             "WANDB_ENTITY": self.entity,
             "WANDB_API_KEY": os.environ.get("WANDB_API_KEY", None),
         }
         return {k: v for k, v in env_vars.items() if v is not None}
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/lm_harness.py` & `lm-buddy-0.9.0/src/lm_buddy/jobs/evaluation/lm_harness.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,31 +2,23 @@
 
 import lm_eval
 import pandas as pd
 import torch
 from lm_eval.models.huggingface import HFLM
 from lm_eval.models.openai_completions import OpenaiCompletionsLM
 
-from lm_buddy.integrations.huggingface import (
-    AutoModelConfig,
-    HuggingFaceAssetLoader,
-    resolve_peft_and_pretrained,
-)
-from lm_buddy.integrations.wandb import (
-    ArtifactLoader,
+from lm_buddy.configs.huggingface import AutoModelConfig
+from lm_buddy.configs.jobs.lm_harness import LMHarnessJobConfig, LocalChatCompletionsConfig
+from lm_buddy.jobs.asset_loader import HuggingFaceAssetLoader
+from lm_buddy.jobs.common import EvaluationResult
+from lm_buddy.tracking.artifact_utils import (
     ArtifactType,
-    WandbArtifactConfig,
-    WandbResumeMode,
     build_table_artifact,
     default_artifact_name,
-    wandb_init_from_config,
 )
-from lm_buddy.jobs.common import EvaluationResult, LMBuddyJobType
-from lm_buddy.jobs.configs import LMHarnessJobConfig, LocalChatCompletionsConfig
-from lm_buddy.paths import AssetPath
 
 
 def get_per_task_dataframes(
     results: dict[str, dict[str, Any]],
 ) -> dict[str, pd.DataFrame]:
     """Create a `pd.DataFrame` of numeric metrics for each evaluation task.
 
@@ -38,24 +30,20 @@
     task_dataframes = {}
     for task_name, data in results.items():
         numeric_rows = [(k, v) for k, v in data.items() if isinstance(v, int | float)]
         task_dataframes[task_name] = pd.DataFrame(data=numeric_rows, columns=["metric", "value"])
     return task_dataframes
 
 
-def load_harness_model(
-    config: LMHarnessJobConfig,
-    artifact_loader: ArtifactLoader,
-) -> HFLM | OpenaiCompletionsLM:
+def load_harness_model(config: LMHarnessJobConfig) -> HFLM | OpenaiCompletionsLM:
     # Instantiate the lm-harness LM class based on the provided model config type
-    hf_loader = HuggingFaceAssetLoader(artifact_loader)
+    hf_loader = HuggingFaceAssetLoader()
     match config.model:
         case AutoModelConfig() as model_config:
-            model_path = hf_loader.resolve_asset_path(model_config.load_from)
-            model_path, peft_path = resolve_peft_and_pretrained(model_path)
+            model_path, peft_path = hf_loader.resolve_peft_and_pretrained(model_config.path)
             quantization_kwargs: dict[str, Any] = (
                 config.quantization.model_dump() if config.quantization else {}
             )
             # TODO: Fix this up by passing in the instantiated model directly
             return HFLM(
                 pretrained=model_path,
                 tokenizer=model_path,
@@ -63,77 +51,48 @@
                 device="cuda" if torch.cuda.device_count() > 0 else "cpu",
                 trust_remote_code=config.model.trust_remote_code,
                 dtype=config.model.torch_dtype if config.model.torch_dtype else "auto",
                 **quantization_kwargs,
             )
 
         case LocalChatCompletionsConfig() as local_config:
-            model = local_config.inference.engine
-            if isinstance(model, AssetPath):
-                model = hf_loader.resolve_asset_path(model)
-            # If tokenizer is not provided, it is set to the value of model internally
+            engine_path = hf_loader.resolve_asset_path(local_config.inference.engine)
             return OpenaiCompletionsLM(
-                model=model,
+                model=engine_path,
                 base_url=local_config.inference.base_url,
                 tokenizer_backend=local_config.tokenizer_backend,
                 truncate=local_config.truncate,
                 max_gen_toks=local_config.max_tokens,
             )
 
         case _:
             raise ValueError(f"Unexpected model config type: {type(config.model)}")
 
 
-def run_eval(
-    config: LMHarnessJobConfig,
-    artifact_loader: ArtifactLoader,
-) -> dict[str, list[tuple[str, float]]]:
-    llm = load_harness_model(config, artifact_loader)
+def run_lm_harness(config: LMHarnessJobConfig) -> EvaluationResult:
+    print(f"Running lm-harness evaluation with configuration:\n {config.model_dump_json(indent=2)}")
+
+    llm = load_harness_model(config)
     eval_results = lm_eval.simple_evaluate(
         model=llm,
         tasks=config.evaluation.tasks,
         batch_size=config.evaluation.batch_size,
         num_fewshot=config.evaluation.num_fewshot,
         limit=config.evaluation.limit,
         log_samples=False,
     )
     print(f"Obtained evaluation results: {eval_results}")
-    return get_per_task_dataframes(eval_results["results"])
-
 
-def run_lm_harness(
-    config: LMHarnessJobConfig,
-    artifact_loader: ArtifactLoader,
-) -> EvaluationResult:
-    print(f"Running lm-harness evaluation with configuration:\n {config.model_dump_json(indent=2)}")
+    result_tables = get_per_task_dataframes(eval_results["results"])
 
-    if config.tracking is not None:
-        with wandb_init_from_config(
-            config.tracking,
-            parameters=config.evaluation,  # Log eval settings in W&B run
-            resume=WandbResumeMode.ALLOW,
-            job_type=LMBuddyJobType.EVALUATION,
-        ) as run:
-            eval_tables = run_eval(config, artifact_loader)
-            table_artifact = build_table_artifact(
-                artifact_name=default_artifact_name(run.name, ArtifactType.EVALUATION),
-                artifact_type=ArtifactType.EVALUATION,
-                tables=eval_tables,
-            )
-            print("Logging artifact for evaluation results...")
-            artifact_loader.log_artifact(table_artifact)
-            # Create an artifact config to reference the new table artifact
-            table_artifact_config = WandbArtifactConfig(
-                name=table_artifact.name,
-                project=run.project,
-                entity=run.entity,
-            )
-    else:
-        eval_tables = run_eval(config, artifact_loader)
-        table_artifact_config = None
+    artifact_name = default_artifact_name(config.name, ArtifactType.EVALUATION)
+    table_artifact = build_table_artifact(
+        artifact_name=artifact_name,
+        artifact_type=ArtifactType.EVALUATION,
+        tables=result_tables,
+    )
 
     return EvaluationResult(
-        tables=eval_tables,
-        table_artifact=table_artifact_config,
+        tables=result_tables,
+        artifacts=[table_artifact],
         dataset_path=None,
-        dataset_artifact=None,
     )
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/prometheus.py` & `lm-buddy-0.9.0/src/lm_buddy/jobs/evaluation/prometheus.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 from pathlib import Path
 
 from datasets import load_dataset
 from fastchat.conversation import get_conv_template
 from openai import Completion, OpenAI, OpenAIError
 from tqdm import tqdm
 
-from lm_buddy.integrations.huggingface import AutoTokenizerConfig, HuggingFaceAssetLoader
-from lm_buddy.integrations.wandb import (
-    ArtifactLoader,
+from lm_buddy.configs.huggingface import AutoTokenizerConfig
+from lm_buddy.configs.jobs.prometheus import PrometheusJobConfig
+from lm_buddy.jobs.asset_loader import HuggingFaceAssetLoader
+from lm_buddy.jobs.common import EvaluationResult
+from lm_buddy.preprocessing import format_dataset_with_prompt
+from lm_buddy.tracking.artifact_utils import (
     ArtifactType,
-    WandbArtifactConfig,
     build_directory_artifact,
     default_artifact_name,
-    wandb_init_from_config,
 )
-from lm_buddy.jobs.common import EvaluationResult, LMBuddyJobType
-from lm_buddy.jobs.configs import PrometheusJobConfig
 
 
 @dataclass
 class BadResponseError(Exception):
     def __init__(self, message, error=None):
         self.message = message
         self.error = error
@@ -100,29 +99,32 @@
             )
             current_retry_attempt += 1
             if current_retry_attempt > config.evaluation.max_retries:
                 raise e
     return (feedback, score)
 
 
-def run_eval(
-    config: PrometheusJobConfig,
-    artifact_loader: ArtifactLoader,
-    client: OpenAI,
-) -> Path:
+def run_eval(config: PrometheusJobConfig) -> Path:
+    # Instantiate OpenAI client to speak with the vLLM endpoint
+    client = OpenAI(base_url=config.prometheus.inference.base_url)
+
     # load dataset from W&B artifact
-    hf_loader = HuggingFaceAssetLoader(artifact_loader)
-    data = hf_loader.load_dataset(config.dataset)
+    hf_loader = HuggingFaceAssetLoader()
+    dataset = hf_loader.load_dataset(config.dataset)
+    if config.dataset.prompt_template is not None:
+        dataset = format_dataset_with_prompt(
+            dataset, config.dataset.prompt_template, config.dataset.text_field
+        )
 
     # get the tokenizer
-    tokenizer_config = AutoTokenizerConfig(load_from=config.prometheus.inference.engine)
+    tokenizer_config = AutoTokenizerConfig(path=config.prometheus.inference.engine)
     tokenizer = hf_loader.load_pretrained_tokenizer(tokenizer_config)
 
     # enable / disable tqdm
-    dataset_iterable = tqdm(data) if config.evaluation.enable_tqdm else data
+    dataset_iterable = tqdm(dataset) if config.evaluation.enable_tqdm else dataset
 
     # open the output file for writing and iterate on samples
     tracking_name = config.tracking.name if config.tracking is not None else "output.json"
     output_fname = Path(config.evaluation.output_folder) / tracking_name
     with output_fname.open("w") as file:
         for sample in dataset_iterable:
             # convert instructions from the dataset (`text_field` in a dict) to
@@ -153,47 +155,26 @@
     output_dataset_path = Path(config.evaluation.output_folder) / "hf" / tracking_name
     ds = load_dataset("json", data_files=str(output_fname), split="train")
     ds.save_to_disk(output_dataset_path)
 
     return output_dataset_path
 
 
-def run_prometheus(
-    config: PrometheusJobConfig,
-    artifact_loader: ArtifactLoader,
-) -> EvaluationResult:
-    # Instantiate OpenAI client to speak with the vLLM endpoint
-    client = OpenAI(base_url=config.prometheus.inference.base_url)
-
+def run_prometheus(config: PrometheusJobConfig) -> EvaluationResult:
     # Run eval and store output in local filename
-    if config.tracking:
-        with wandb_init_from_config(config.tracking, job_type=LMBuddyJobType.EVALUATION) as run:
-            output_dataset_path = run_eval(config, artifact_loader, client)
-
-            # Create a directory artifact for the HF dataset
-            dataset_artifact = build_directory_artifact(
-                dir_path=output_dataset_path,
-                artifact_name=default_artifact_name(run.name, artifact_type=ArtifactType.DATASET),
-                artifact_type=ArtifactType.DATASET,
-                reference=False,
-            )
-
-            print("Logging artifact for evaluation dataset...")
-            artifact_loader.log_artifact(dataset_artifact)
+    output_dataset_path = run_eval(config)
+    print(f"Prometheus evaluation dataset stored at {output_dataset_path}")
 
-            # Create a config referencing the new artifact
-            dataset_artifact_config = WandbArtifactConfig(
-                name=dataset_artifact.name,
-                project=run.project,
-                entity=run.entity,
-            )
-    else:
-        output_dataset_path = run_eval(config, artifact_loader, client)
-        dataset_artifact_config = None
+    # Create a directory artifact for the HF dataset
+    artifact_name = default_artifact_name(config.name, artifact_type=ArtifactType.DATASET)
+    dataset_artifact = build_directory_artifact(
+        artifact_name=artifact_name,
+        artifact_type=ArtifactType.DATASET,
+        dir_path=output_dataset_path,
+        reference=False,
+    )
 
-    print(f"Evaluation dataset stored at {output_dataset_path}")
     return EvaluationResult(
-        tables={},
-        table_artifact=None,
-        dataset_artifact=dataset_artifact_config,
+        artifacts=[dataset_artifact],
         dataset_path=output_dataset_path,
+        tables={},
     )
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/jobs/common.py` & `lm-buddy-0.9.0/src/lm_buddy/jobs/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import Any
 
 import pandas as pd
+import wandb
 
-from lm_buddy.integrations.wandb import WandbArtifactConfig
 
-
-class LMBuddyJobType(str, Enum):
+class JobType(str, Enum):
     """Enumeration of logical job types runnable via the LM Buddy."""
 
     PREPROCESSING = "preprocessing"
     FINETUNING = "finetuning"
     EVALUATION = "evaluation"
 
 
 @dataclass
-class FinetuningResult:
+class JobResult:
+    artifacts: list[wandb.Artifact]
+
+
+@dataclass
+class FinetuningResult(JobResult):
     """Result from a finetuning task."""
 
     checkpoint_path: Path | None
-    checkpoint_artifact: WandbArtifactConfig | None
-    metrics: dict[str, Any]
+    metrics: dict[str, Any] | None
     is_adapter: bool
 
 
 @dataclass
-class EvaluationResult:
+class EvaluationResult(JobResult):
     """Result from an evaluation task, containing aggregate metrics and artifacts."""
 
     tables: dict[str, pd.DataFrame]
-    table_artifact: WandbArtifactConfig | None
-    dataset_artifact: WandbArtifactConfig | None
     dataset_path: Path | None
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/jobs/configs/base.py` & `lm-buddy-0.9.0/src/lm_buddy/configs/jobs/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,38 @@
 import contextlib
 import tempfile
+from abc import abstractmethod
 from pathlib import Path
 
+from pydantic import Field
 from pydantic_yaml import parse_yaml_file_as, to_yaml_file
 
-from lm_buddy.types import BaseLMBuddyConfig
+from lm_buddy.configs.common import LMBuddyConfig
+from lm_buddy.configs.wandb import WandbRunConfig
+from lm_buddy.paths import AssetPath, PathPrefix
 
 
-class LMBuddyJobConfig(BaseLMBuddyConfig):
+class JobConfig(LMBuddyConfig):
     """Configuration that comprises the entire input to an LM Buddy job.
 
     This class implements helper methods for de/serializing the configuration from file.
 
     Currently, there is a 1:1 mapping between job entrypoints and job config implementations,
     but this is not rigidly constrained by the interface. This may change in the future.
     """
 
+    name: str = Field(description="Name of the job.")
+    tracking: WandbRunConfig | None = Field(
+        default=None,
+        description=(
+            "Tracking information to associate with the job. "
+            "A new run is created with these details."
+        ),
+    )
+
     @classmethod
     def from_yaml_file(cls, path: Path | str):
         return parse_yaml_file_as(cls, path)
 
     def to_yaml_file(self, path: Path | str):
         to_yaml_file(path, self, exclude_none=True)
 
@@ -34,7 +47,16 @@
         Returns:
             Path to the temporary config file.
         """
         with tempfile.TemporaryDirectory(dir=dir) as tmpdir:
             config_path = Path(tmpdir) / name
             self.to_yaml_file(config_path)
             yield config_path
+
+    @abstractmethod
+    def asset_paths(self) -> set[AssetPath]:
+        """Return a set of all `AssetPath` fields on this config."""
+        pass
+
+    def artifact_paths(self) -> set[AssetPath]:
+        """Return a set of all W&B artifact paths on this config."""
+        return {x for x in self.asset_paths() if x.startswith(PathPrefix.WANDB)}
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/jobs/configs/finetuning.py` & `lm-buddy-0.9.0/src/lm_buddy/configs/jobs/finetuning.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 from pydantic import Field, field_validator, model_validator
 
-from lm_buddy.integrations.huggingface import (
+from lm_buddy.configs.common import LMBuddyConfig
+from lm_buddy.configs.huggingface import (
     AdapterConfig,
     AutoModelConfig,
     AutoTokenizerConfig,
+    DatasetConfig,
     QuantizationConfig,
-    TextDatasetConfig,
     TrainerConfig,
 )
-from lm_buddy.integrations.wandb import WandbRunConfig
-from lm_buddy.jobs.configs import LMBuddyJobConfig
-from lm_buddy.types import BaseLMBuddyConfig
+from lm_buddy.configs.jobs.common import JobConfig
+from lm_buddy.paths import AssetPath
 
 
-class FinetuningRayConfig(BaseLMBuddyConfig):
+class FinetuningRayConfig(LMBuddyConfig):
     """Misc settings passed to Ray train for finetuning.
 
     Includes information for scaling, checkpointing, and runtime storage.
     """
 
     use_gpu: bool = True
     num_workers: int | None = None
     storage_path: str | None = None  # TODO: This should be set globally somehow
 
 
-class FinetuningJobConfig(LMBuddyJobConfig):
+class FinetuningJobConfig(JobConfig):
     """Configuration to submit an LLM finetuning job."""
 
     model: AutoModelConfig
-    dataset: TextDatasetConfig
+    dataset: DatasetConfig
     tokenizer: AutoTokenizerConfig
     quantization: QuantizationConfig | None = None
     adapter: AdapterConfig | None = None
-    tracking: WandbRunConfig | None = None
     trainer: TrainerConfig = Field(default_factory=TrainerConfig)
     ray: FinetuningRayConfig = Field(default_factory=FinetuningRayConfig)
 
     @model_validator(mode="before")
     def ensure_tokenizer_config(cls, values):
         """Set the tokenizer to the model path when not explicitly provided."""
         if values.get("tokenizer") is None:
             values["tokenizer"] = {}
             match values["model"]:
                 case str() as model_path:
-                    values["tokenizer"]["load_from"] = model_path
+                    values["tokenizer"]["path"] = model_path
                 case dict() as model_data:
-                    values["tokenizer"]["load_from"] = model_data["load_from"]
+                    values["tokenizer"]["path"] = model_data["path"]
                 case AutoModelConfig() as model_config:
-                    values["tokenizer"]["load_from"] = model_config.load_from
+                    values["tokenizer"]["path"] = model_config.path
                 # No fallback necessary, downstream validation will flag invalid model types
         return values
 
     @field_validator("model", mode="before")
     def validate_model_arg(cls, x):
         """Allow for passing just a path string as the model argument."""
         if isinstance(x, str):
-            return AutoModelConfig(load_from=x)
+            return AutoModelConfig(path=x)
         return x
 
     @field_validator("tokenizer", mode="before")
     def validate_tokenizer_arg(cls, x):
         """Allow for passing just a path string as the tokenizer argument."""
         if isinstance(x, str):
-            return AutoTokenizerConfig(load_from=x)
+            return AutoTokenizerConfig(path=x)
         return x
+
+    def asset_paths(self) -> list[AssetPath]:
+        return {self.model.path, self.dataset.path, self.tokenizer.path}
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/jobs/configs/lm_harness.py` & `lm-buddy-0.9.0/src/lm_buddy/configs/jobs/lm_harness.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from typing import Literal
 
 from pydantic import conlist, model_validator
 
-from lm_buddy.integrations.huggingface import (
-    AutoModelConfig,
-    QuantizationConfig,
-)
-from lm_buddy.integrations.vllm import InferenceServerConfig
-from lm_buddy.integrations.wandb import WandbRunConfig
-from lm_buddy.jobs.configs import LMBuddyJobConfig
-from lm_buddy.types import BaseLMBuddyConfig
+from lm_buddy.configs.common import LMBuddyConfig
+from lm_buddy.configs.huggingface import AutoModelConfig, QuantizationConfig
+from lm_buddy.configs.jobs.common import JobConfig
+from lm_buddy.configs.vllm import InferenceServerConfig
+from lm_buddy.paths import AssetPath
 
 
-class LocalChatCompletionsConfig(BaseLMBuddyConfig):
+class LocalChatCompletionsConfig(LMBuddyConfig):
     """Configuration for a "local-chat-completions" model in lm-harness.
 
     The "local-chat-completions" model is powered by a self-hosted inference server,
     specified as an `InferenceServerConfig`. Additional arguments are also provided
     to control the tokenizer type and generation parameters.
     """
 
@@ -31,23 +28,31 @@
             raise ValueError(
                 "Inference config `engine` must be provided for use in "
                 "lm-harness 'local-chat-completions' model."
             )
         return config
 
 
-class LMHarnessEvaluationConfig(BaseLMBuddyConfig):
+class LMHarnessEvaluationConfig(LMBuddyConfig):
     """Misc settings provided to an lm-harness evaluation job."""
 
     tasks: conlist(str, min_length=1)
     batch_size: int | None = None
     num_fewshot: int | None = None
     limit: int | float | None = None
 
 
-class LMHarnessJobConfig(LMBuddyJobConfig):
+class LMHarnessJobConfig(JobConfig):
     """Configuration to run an lm-evaluation-harness evaluation job."""
 
     model: AutoModelConfig | LocalChatCompletionsConfig
     evaluation: LMHarnessEvaluationConfig
     quantization: QuantizationConfig | None = None
-    tracking: WandbRunConfig | None = None
+
+    def asset_paths(self) -> list[AssetPath]:
+        match self.model:
+            case AutoModelConfig() as config:
+                return {config.path}
+            case LocalChatCompletionsConfig() as config if config.inference.engine is not None:
+                return {config.inference.engine}
+            case _:
+                return {}
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/jobs/configs/prometheus.py` & `lm-buddy-0.9.0/src/lm_buddy/configs/jobs/prometheus.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from pydantic import Field
 
-from lm_buddy.integrations.huggingface import TextDatasetConfig
-from lm_buddy.integrations.vllm import VLLMCompletionsConfig
-from lm_buddy.integrations.wandb import WandbRunConfig
-from lm_buddy.jobs.configs import LMBuddyJobConfig
-from lm_buddy.types import BaseLMBuddyConfig
+from lm_buddy.configs.common import LMBuddyConfig
+from lm_buddy.configs.huggingface import DatasetConfig
+from lm_buddy.configs.jobs.common import JobConfig
+from lm_buddy.configs.vllm import VLLMCompletionsConfig
+from lm_buddy.paths import AssetPath
 
 
-class PrometheusEvaluationConfig(BaseLMBuddyConfig):
+class PrometheusEvaluationConfig(LMBuddyConfig):
     """Parameters specific to Prometheus evaluation."""
 
     num_answers: int = 3
     max_retries: int = 5
     scores: list = [1, 2, 3, 4, 5]
     min_score: int = 0
     max_score: int = 5
     enable_tqdm: bool = False
     output_folder: str = "/tmp"
     conversation_template: str = "llama-2"
     conversation_system_message: str = "You are a fair evaluator language model."
 
 
-class PrometheusJobConfig(LMBuddyJobConfig):
+class PrometheusJobConfig(JobConfig):
     """Configuration for a Prometheus judge evaluation task."""
 
     prometheus: VLLMCompletionsConfig = Field(
         description="Externally hosted Prometheus judge model."
     )
-    dataset: TextDatasetConfig = Field(
+    dataset: DatasetConfig = Field(
         description="Dataset of text completions to evaluate using the Prometheus judge model."
     )
     evaluation: PrometheusEvaluationConfig = Field(
         default_factory=PrometheusEvaluationConfig,
         description="Settings for the Prometheus evaluation.",
     )
-    tracking: WandbRunConfig | None = None
+
+    def asset_paths(self) -> set[AssetPath]:
+        paths = {self.dataset.path, self.prometheus.inference.engine}
+        return {x for x in paths if x is not None}
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy/paths.py` & `lm-buddy-0.9.0/src/lm_buddy/paths.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,28 @@
+import re
+from enum import Enum
 from pathlib import Path
-from typing import Annotated, Any
+from typing import Annotated
 
+import wandb
 from huggingface_hub.utils import HFValidationError, validate_repo_id
-from pydantic import BeforeValidator
+from pydantic import AfterValidator
+from wandb.sdk.artifacts.exceptions import ArtifactNotLoggedError
 
-from lm_buddy.integrations.wandb import WandbArtifactConfig
-from lm_buddy.types import BaseLMBuddyConfig
 
+class PathPrefix(str, Enum):
+    FILE = "file://"
+    HUGGINGFACE = "hf://"
+    WANDB = "wandb://"
 
-class FilePath(BaseLMBuddyConfig):
-    """Absolute path to an object on the local filesystem."""
 
-    __match_args__ = ("path",)
-
-    path: Path
-
-
-class HuggingFaceRepoID(BaseLMBuddyConfig):
-    """Repository ID on the HuggingFace Hub."""
-
-    __match_args__ = ("repo_id",)
-
-    repo_id: str
+def strip_path_prefix(path: str) -> str:
+    """Strip the 'scheme://' prefix from the start of a string."""
+    pattern = "^\w+\:\/\/"
+    return re.sub(pattern, "", path)
 
 
 def is_valid_huggingface_repo_id(s: str):
     """
     Simple test to check if an HF model is valid using HuggingFace's tools.
     Sadly, theirs throws an exception and has no return.
 
@@ -35,34 +32,45 @@
     try:
         validate_repo_id(s)
         return True
     except HFValidationError:
         return False
 
 
-def validate_asset_path(x: Any) -> Any:
-    match x:
-        case Path() as p:
-            return FilePath(path=p)
-        case str() as s if Path(s).is_absolute():
-            return FilePath(path=s)
-        case str() as s if is_valid_huggingface_repo_id(s):
-            return HuggingFaceRepoID(repo_id=s)
-        case str():
-            raise ValueError(f"{x} is neither a valid HuggingFace repo ID or an absolute path.")
-        case _:
-            # Handled by downstream "after" validators
-            return x
-
-
-AssetPath = Annotated[
-    FilePath | HuggingFaceRepoID | WandbArtifactConfig,
-    BeforeValidator(lambda x: validate_asset_path(x)),
-]
-"""Union type representing the name/path for loading HuggingFace asset.
-
-The path is represented by either a `FileSystemPath`, a `HuggingFaceRepoID`
-or a `WandbArtifactConfig` that can be resolved to a path via the artifact's manifest.
-
-This type is annotated with Pydantic validation logic to convert absolute path strings
-to `FilesystemPath`s and other strings to `HuggingFaceRepoID`s.
-"""
+def validate_asset_path(path: str) -> "AssetPath":
+    raw_path = strip_path_prefix(path)
+    if path.startswith(PathPrefix.FILE):
+        if not Path(raw_path).is_absolute():
+            raise ValueError(f"'{raw_path}' is not an absolute file path.")
+    elif path.startswith(PathPrefix.HUGGINGFACE):
+        if not is_valid_huggingface_repo_id(raw_path):
+            raise ValueError(f"'{raw_path}' is not a valid HuggingFace repo ID.")
+    elif path.startswith(PathPrefix.WANDB):
+        # TODO: Validate the W&B path structure?
+        pass
+    else:
+        allowed_prefixes = {x.value for x in PathPrefix}
+        raise ValueError(f"'{path}' does not begin with an allowed prefix: {allowed_prefixes}")
+    return path
+
+
+AssetPath = Annotated[str, AfterValidator(lambda x: validate_asset_path(x))]
+
+
+def format_file_path(path: str | Path) -> AssetPath:
+    path = Path(path).absolute()
+    return f"{PathPrefix.FILE}{path}"
+
+
+def format_huggingface_path(repo_id: str) -> AssetPath:
+    return f"{PathPrefix.HUGGINGFACE}{repo_id}"
+
+
+def format_artifact_path(artifact: wandb.Artifact) -> AssetPath:
+    try:
+        return f"{PathPrefix.WANDB}{artifact.qualified_name}"
+    except ArtifactNotLoggedError as e:
+        msg = (
+            "Unable to construct an `AssetPath` from artifact missing project/entity fields. "
+            "Make sure to log the artifact before calling this method."
+        )
+        raise ValueError(msg) from e
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy.egg-info/PKG-INFO` & `lm-buddy-0.9.0/src/lm_buddy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lm-buddy
-Version: 0.4.1
+Version: 0.9.0
 Summary: Ray-centric library for finetuning and evaluation of (large) language models.
-Author-email: Sean Friedowitz <sean@mozilla.ai>, Aaron Gonzales <aaron@mozilla.ai>, Vicki Boykis <vicki@mozilla.ai>, Davide Eynard <davide@mozilla.ai>
+Author-email: Sean Friedowitz <sean@mozilla.ai>, Aaron Gonzales <aaron@mozilla.ai>, Vicki Boykis <vicki@mozilla.ai>, Davide Eynard <davide@mozilla.ai>, Imtihan Ahmed <imtihan@mozilla.ai>
 License: 
                                       Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -225,15 +225,18 @@
 Requires-Dist: accelerate==0.26.1
 Requires-Dist: peft==0.7.1
 Requires-Dist: trl==0.7.10
 Requires-Dist: bitsandbytes==0.42.0
 Requires-Dist: lm-eval==0.4.2
 Requires-Dist: einops==0.7.0
 Requires-Dist: fschat==0.2.36
-Requires-Dist: openai==1.3.9
+Requires-Dist: openai==1.14.3
+Requires-Dist: ragas==0.1.5
+Requires-Dist: langchain-community==0.0.29
+Requires-Dist: langchain_openai==0.1.1
 Provides-Extra: ruff
 Requires-Dist: ruff==0.2.1; extra == "ruff"
 Provides-Extra: test
 Requires-Dist: pytest==7.4.3; extra == "test"
 Requires-Dist: pytest-cov==4.1.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: Sphinx==7.2.6; extra == "docs"
```

### Comparing `lm-buddy-0.4.1/src/lm_buddy.egg-info/requires.txt` & `lm-buddy-0.9.0/src/lm_buddy.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 accelerate==0.26.1
 peft==0.7.1
 trl==0.7.10
 bitsandbytes==0.42.0
 lm-eval==0.4.2
 einops==0.7.0
 fschat==0.2.36
-openai==1.3.9
+openai==1.14.3
+ragas==0.1.5
+langchain-community==0.0.29
+langchain_openai==0.1.1
 
 [dev]
 lm-buddy[docs,ruff,test]
 pre-commit==3.6.0
 jupyter==1.0.0
 
 [docs]
```

