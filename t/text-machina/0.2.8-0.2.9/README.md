# Comparing `tmp/text_machina-0.2.8.tar.gz` & `tmp/text_machina-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_machina-0.2.8.tar", last modified: Fri Apr 26 08:57:45 2024, max compression
+gzip compressed data, was "text_machina-0.2.9.tar", last modified: Tue Apr 30 16:11:59 2024, max compression
```

## Comparing `text_machina-0.2.8.tar` & `text_machina-0.2.9.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.825627 text_machina-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    19133 2024-04-26 08:57:41.000000 text_machina-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-04-26 08:57:45.825627 text_machina-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-04-26 08:57:41.000000 text_machina-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 08:57:45.825627 text_machina-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-26 08:57:41.000000 text_machina-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.801627 text_machina-0.2.8/text_machina/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.805627 text_machina-0.2.8/text_machina/src/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.805627 text_machina-0.2.8/text_machina/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/common/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.805627 text_machina-0.2.8/text_machina/src/constrainers/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/constrainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/constrainers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/constrainers/length.py
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.805627 text_machina-0.2.8/text_machina/src/exploration/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/exploration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/exploration/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/exploration/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/exploration/boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/exploration/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/exploration/mixcase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.809627 text_machina-0.2.8/text_machina/src/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/entity_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/noun_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/sentence_gap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/sentence_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/sentence_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/sentence_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/word_gap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/word_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/extractors/word_prefix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.809627 text_machina-0.2.8/text_machina/src/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/generators/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/generators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/generators/boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/generators/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26488 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/generators/mixcase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.809627 text_machina-0.2.8/text_machina/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/metrics/mauve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/metrics/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/metrics/repetition_diversity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/metrics/simple_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/metrics/token_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.813627 text_machina-0.2.8/text_machina/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/ai21.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/azure_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/hf_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/hf_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/inference_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/models/vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)    14789 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.813627 text_machina-0.2.8/text_machina/src/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/ai21.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/azure_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/hf_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/hf_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/inference_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/tokenizers/vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/src/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-26 08:57:41.000000 text_machina-0.2.8/text_machina/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:57:45.813627 text_machina-0.2.8/text_machina.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-04-26 08:57:45.000000 text_machina-0.2.8/text_machina.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-26 08:57:45.000000 text_machina-0.2.8/text_machina.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:57:45.000000 text_machina-0.2.8/text_machina.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 08:57:45.000000 text_machina-0.2.8/text_machina.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-26 08:57:45.000000 text_machina-0.2.8/text_machina.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 08:57:45.000000 text_machina-0.2.8/text_machina.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.077530 text_machina-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    19133 2024-04-30 16:11:54.000000 text_machina-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-04-30 16:11:59.077530 text_machina-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-04-30 16:11:54.000000 text_machina-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:11:59.077530 text_machina-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-30 16:11:54.000000 text_machina-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.057530 text_machina-0.2.9/text_machina/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.061530 text_machina-0.2.9/text_machina/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.061530 text_machina-0.2.9/text_machina/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/common/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.061530 text_machina-0.2.9/text_machina/src/constrainers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/constrainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/constrainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/constrainers/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.061530 text_machina-0.2.9/text_machina/src/exploration/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/exploration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/exploration/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/exploration/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/exploration/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/exploration/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/exploration/mixcase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.065530 text_machina-0.2.9/text_machina/src/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/entity_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/noun_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/sentence_gap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/sentence_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/sentence_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/sentence_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/word_gap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/word_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/extractors/word_prefix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.065530 text_machina-0.2.9/text_machina/src/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/generators/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/generators/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/generators/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26488 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/generators/mixcase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.065530 text_machina-0.2.9/text_machina/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/metrics/mauve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/metrics/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/metrics/repetition_diversity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/metrics/simple_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/metrics/token_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.069530 text_machina-0.2.9/text_machina/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/ai21.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/azure_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/hf_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/hf_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/inference_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/models/vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14789 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.069530 text_machina-0.2.9/text_machina/src/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/ai21.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/azure_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/hf_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/hf_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/inference_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/tokenizers/vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/src/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-30 16:11:54.000000 text_machina-0.2.9/text_machina/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:11:59.069530 text_machina-0.2.9/text_machina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-04-30 16:11:59.000000 text_machina-0.2.9/text_machina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-30 16:11:59.000000 text_machina-0.2.9/text_machina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:11:59.000000 text_machina-0.2.9/text_machina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 16:11:59.000000 text_machina-0.2.9/text_machina.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-30 16:11:59.000000 text_machina-0.2.9/text_machina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 16:11:59.000000 text_machina-0.2.9/text_machina.egg-info/top_level.txt
```

### Comparing `text_machina-0.2.8/LICENSE` & `text_machina-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/PKG-INFO` & `text_machina-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-machina
-Version: 0.2.8
+Version: 0.2.9
 Summary: Text Machina: Seamless Generation of Machine-Generated Text Datasets
 Home-page: https://github.com/Genaios/TextMachina
 Author: Genaios
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `text_machina-0.2.8/README.md` & `text_machina-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/setup.py` & `text_machina-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/cli.py` & `text_machina-0.2.9/text_machina/cli.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/cli_utils.py` & `text_machina-0.2.9/text_machina/cli_utils.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/__init__.py` & `text_machina-0.2.9/text_machina/src/__init__.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/common/exceptions.py` & `text_machina-0.2.9/text_machina/src/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/common/logging.py` & `text_machina-0.2.9/text_machina/src/common/logging.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/common/utils.py` & `text_machina-0.2.9/text_machina/src/common/utils.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/config.py` & `text_machina-0.2.9/text_machina/src/config.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/constrainers/__init__.py` & `text_machina-0.2.9/text_machina/src/constrainers/__init__.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/constrainers/base.py` & `text_machina-0.2.9/text_machina/src/constrainers/base.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/constrainers/length.py` & `text_machina-0.2.9/text_machina/src/constrainers/length.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/data.py` & `text_machina-0.2.9/text_machina/src/data.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/exploration/__init__.py` & `text_machina-0.2.9/text_machina/src/exploration/__init__.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/exploration/attribution.py` & `text_machina-0.2.9/text_machina/src/exploration/attribution.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/exploration/base.py` & `text_machina-0.2.9/text_machina/src/exploration/base.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/exploration/boundary.py` & `text_machina-0.2.9/text_machina/src/exploration/boundary.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/exploration/detection.py` & `text_machina-0.2.9/text_machina/src/exploration/detection.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/exploration/mixcase.py` & `text_machina-0.2.9/text_machina/src/exploration/mixcase.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/__init__.py` & `text_machina-0.2.9/text_machina/src/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/auxiliary.py` & `text_machina-0.2.9/text_machina/src/extractors/auxiliary.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/base.py` & `text_machina-0.2.9/text_machina/src/extractors/base.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/combined.py` & `text_machina-0.2.9/text_machina/src/extractors/combined.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/dummy.py` & `text_machina-0.2.9/text_machina/src/extractors/dummy.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/entity_list.py` & `text_machina-0.2.9/text_machina/src/extractors/entity_list.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/noun_list.py` & `text_machina-0.2.9/text_machina/src/extractors/noun_list.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/sentence_gap.py` & `text_machina-0.2.9/text_machina/src/extractors/sentence_gap.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/sentence_masking.py` & `text_machina-0.2.9/text_machina/src/extractors/sentence_masking.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/sentence_prefix.py` & `text_machina-0.2.9/text_machina/src/extractors/sentence_prefix.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/sentence_rewriting.py` & `text_machina-0.2.9/text_machina/src/extractors/sentence_rewriting.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/types.py` & `text_machina-0.2.9/text_machina/src/extractors/types.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/utils.py` & `text_machina-0.2.9/text_machina/src/extractors/utils.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/word_gap.py` & `text_machina-0.2.9/text_machina/src/extractors/word_gap.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/word_masking.py` & `text_machina-0.2.9/text_machina/src/extractors/word_masking.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/extractors/word_prefix.py` & `text_machina-0.2.9/text_machina/src/extractors/word_prefix.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/generators/__init__.py` & `text_machina-0.2.9/text_machina/src/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/generators/attribution.py` & `text_machina-0.2.9/text_machina/src/generators/attribution.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/generators/base.py` & `text_machina-0.2.9/text_machina/src/generators/base.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/generators/boundary.py` & `text_machina-0.2.9/text_machina/src/generators/boundary.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/generators/detection.py` & `text_machina-0.2.9/text_machina/src/generators/detection.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/generators/mixcase.py` & `text_machina-0.2.9/text_machina/src/generators/mixcase.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/metrics/__init__.py` & `text_machina-0.2.9/text_machina/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/metrics/base.py` & `text_machina-0.2.9/text_machina/src/metrics/base.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/metrics/mauve.py` & `text_machina-0.2.9/text_machina/src/metrics/mauve.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/metrics/perplexity.py` & `text_machina-0.2.9/text_machina/src/metrics/perplexity.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/metrics/repetition_diversity.py` & `text_machina-0.2.9/text_machina/src/metrics/repetition_diversity.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/metrics/simple_model.py` & `text_machina-0.2.9/text_machina/src/metrics/simple_model.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/metrics/token_classification.py` & `text_machina-0.2.9/text_machina/src/metrics/token_classification.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/models/__init__.py` & `text_machina-0.2.9/text_machina/src/models/__init__.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/models/ai21.py` & `text_machina-0.2.9/text_machina/src/models/ai21.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/models/anthropic.py` & `text_machina-0.2.9/text_machina/src/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/models/azure_openai.py` & `text_machina-0.2.9/text_machina/src/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/models/base.py` & `text_machina-0.2.9/text_machina/src/models/base.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/models/bedrock.py` & `text_machina-0.2.9/text_machina/src/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/models/cohere.py` & `text_machina-0.2.9/text_machina/src/models/cohere.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/models/hf_local.py` & `text_machina-0.2.9/text_machina/src/models/hf_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, List
 
 from tqdm import tqdm
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from ..config import ModelConfig
 from .base import TextGenerationModel
-from .types import QUANTIZATION_CONFIGS
+from .types import QUANTIZATION_CONFIGS, CompletionType
 
 
 class HuggingFaceLocalModel(TextGenerationModel):
     """
     Generates completions using HuggingFace's models locally deployed.
     """
 
@@ -52,14 +52,24 @@
         prompts: List[str],
         generation_config: Dict,
     ) -> List[str]:
         """
         Overriden method to generate completions using
         HuggingFace's `generate` method with batches
         """
+        if self.model_config.api_type == CompletionType.CHAT:
+            prompts = [
+                self.tokenizer.apply_chat_template(
+                    [{"role": "user", "content": prompt}],
+                    add_generation_prompt=True,
+                    tokenize=False,
+                )
+                for prompt in prompts
+            ]
+
         tokenized_prompts = self.tokenizer(
             prompts, truncation=True, padding=True, return_tensors="pt"
         )
         completions = []
         for batch_idx in tqdm(
             range(0, len(prompts), self.batch_size),
             desc=f"Generating locally with {self.model_name}",
```

### Comparing `text_machina-0.2.8/text_machina/src/models/inference_server.py` & `text_machina-0.2.9/text_machina/src/models/inference_server.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/models/openai.py` & `text_machina-0.2.9/text_machina/src/models/openai.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/models/types.py` & `text_machina-0.2.9/text_machina/src/models/types.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/models/vertex.py` & `text_machina-0.2.9/text_machina/src/models/vertex.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/postprocessing.py` & `text_machina-0.2.9/text_machina/src/postprocessing.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/tokenizers/__init__.py` & `text_machina-0.2.9/text_machina/src/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/tokenizers/ai21.py` & `text_machina-0.2.9/text_machina/src/tokenizers/ai21.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/tokenizers/anthropic.py` & `text_machina-0.2.9/text_machina/src/tokenizers/anthropic.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/tokenizers/azure_openai.py` & `text_machina-0.2.9/text_machina/src/tokenizers/azure_openai.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/tokenizers/base.py` & `text_machina-0.2.9/text_machina/src/tokenizers/base.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/tokenizers/bedrock.py` & `text_machina-0.2.9/text_machina/src/tokenizers/bedrock.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/tokenizers/cohere.py` & `text_machina-0.2.9/text_machina/src/tokenizers/cohere.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/tokenizers/hf_local.py` & `text_machina-0.2.9/text_machina/src/tokenizers/hf_local.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/tokenizers/vertex.py` & `text_machina-0.2.9/text_machina/src/tokenizers/vertex.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/src/types.py` & `text_machina-0.2.9/text_machina/src/types.py`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina/version.py` & `text_machina-0.2.9/text_machina/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 _MAJOR = "0"
 _MINOR = "2"
-_REVISION = "8"
+_REVISION = "9"
 
 VERSION_SHORT = "{0}.{1}".format(_MAJOR, _MINOR)
 VERSION = "{0}.{1}.{2}".format(_MAJOR, _MINOR, _REVISION)
 
 __version__ = VERSION
```

### Comparing `text_machina-0.2.8/text_machina.egg-info/PKG-INFO` & `text_machina-0.2.9/text_machina.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-machina
-Version: 0.2.8
+Version: 0.2.9
 Summary: Text Machina: Seamless Generation of Machine-Generated Text Datasets
 Home-page: https://github.com/Genaios/TextMachina
 Author: Genaios
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `text_machina-0.2.8/text_machina.egg-info/SOURCES.txt` & `text_machina-0.2.9/text_machina.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `text_machina-0.2.8/text_machina.egg-info/requires.txt` & `text_machina-0.2.9/text_machina.egg-info/requires.txt`

 * *Files identical despite different names*

