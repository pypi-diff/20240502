# Comparing `tmp/llm-dataset-converter-0.2.0.tar.gz` & `tmp/llm-dataset-converter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-dataset-converter-0.2.0.tar", last modified: Tue Feb 27 03:38:10 2024, max compression
+gzip compressed data, was "llm-dataset-converter-0.2.1.tar", last modified: Thu May  2 02:48:29 2024, max compression
```

## Comparing `llm-dataset-converter-0.2.0.tar` & `llm-dataset-converter-0.2.1.tar`

### file list

```diff
@@ -1,110 +1,113 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.186697 llm-dataset-converter-0.2.0/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5683 2024-02-27 03:35:42.000000 llm-dataset-converter-0.2.0/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1326 2024-02-27 03:36:56.000000 llm-dataset-converter-0.2.0/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 llm-dataset-converter-0.2.0/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8911 2024-02-27 03:38:10.186697 llm-dataset-converter-0.2.0/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    25253 2024-02-23 01:27:10.000000 llm-dataset-converter-0.2.0/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-02-27 03:38:10.186697 llm-dataset-converter-0.2.0/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2744 2024-02-21 21:39:48.000000 llm-dataset-converter-0.2.0/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.166697 llm-dataset-converter-0.2.0/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.170697 llm-dataset-converter-0.2.0/src/ldc/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-14 22:03:25.000000 llm-dataset-converter-0.2.0/src/ldc/__init__.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.170697 llm-dataset-converter-0.2.0/src/ldc/api/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       78 2024-02-20 02:26:03.000000 llm-dataset-converter-0.2.0/src/ldc/api/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      740 2024-02-04 22:38:10.000000 llm-dataset-converter-0.2.0/src/ldc/api/_downloader.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      513 2024-02-05 03:13:29.000000 llm-dataset-converter-0.2.0/src/ldc/api/_filter.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10115 2024-02-21 01:05:00.000000 llm-dataset-converter-0.2.0/src/ldc/api/_io.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4518 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/api/pretrain.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.170697 llm-dataset-converter-0.2.0/src/ldc/api/supervised/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2024-02-20 01:36:43.000000 llm-dataset-converter-0.2.0/src/ldc/api/supervised/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5031 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/api/supervised/classification.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4930 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/api/supervised/pairs.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4644 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/api/translation.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5697 2024-02-13 01:26:36.000000 llm-dataset-converter-0.2.0/src/ldc/core.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.170697 llm-dataset-converter-0.2.0/src/ldc/downloader/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       37 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.0/src/ldc/downloader/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5145 2024-02-20 02:25:09.000000 llm-dataset-converter-0.2.0/src/ldc/downloader/_huggingface.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.178697 llm-dataset-converter-0.2.0/src/ldc/filter/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1332 2024-02-21 00:27:06.000000 llm-dataset-converter-0.2.0/src/ldc/filter/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7928 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_assemble_sentences.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6817 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_change_case.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6756 2024-02-21 01:05:00.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_file_filter.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8537 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_find_substr.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7714 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_keyword.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3362 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_llama2_to_pairs.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3694 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_max_records.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8496 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_metadata.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3716 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_pairs_to_llama2.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4040 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_pairs_to_pretrain.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5430 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_pretrain_sentences_to_classification.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6427 2024-02-21 03:31:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_pretrain_sentences_to_pairs.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3863 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_randomize_records.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4963 2024-02-21 01:05:00.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_record_files.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5367 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_record_window.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8294 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_remove_blocks.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6684 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_remove_empty.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7236 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_remove_patterns.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7948 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_replace_patterns.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3675 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_reset_ids.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3049 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_skip_duplicate_ids.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6152 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_skip_duplicate_text.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5184 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_split.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6277 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_tee.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8252 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_text_length.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10413 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_text_stats.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3555 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_to_llama2_format.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4763 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_translation_to_pairs.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3323 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.0/src/ldc/filter/_translation_to_pretrain.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2923 2023-10-26 00:16:47.000000 llm-dataset-converter-0.2.0/src/ldc/help.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.182697 llm-dataset-converter-0.2.0/src/ldc/pretrain/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      383 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.0/src/ldc/pretrain/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    24425 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/pretrain/_csv.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    13314 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/pretrain/_jsonlines.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4207 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.0/src/ldc/pretrain/_max_length.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10502 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/pretrain/_parquet.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5020 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.0/src/ldc/pretrain/_sentences.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1785 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.0/src/ldc/pretrain/_split.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    18316 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/pretrain/_txt.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6763 2024-02-20 02:25:09.000000 llm-dataset-converter-0.2.0/src/ldc/registry.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.182697 llm-dataset-converter-0.2.0/src/ldc/supervised/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-11 04:18:56.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/__init__.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.182697 llm-dataset-converter-0.2.0/src/ldc/supervised/classification/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      343 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/classification/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3739 2024-02-20 01:43:12.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/classification/_classification_label_map.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    25935 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/classification/_csv.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    14372 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/classification/_jsonlines.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    11640 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/classification/_parquet.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.182697 llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      349 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7984 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_alpaca.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    28132 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_csv.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    15436 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_jsonlines.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    12975 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_parquet.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6051 2024-02-22 22:49:44.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_update_pair_data.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    15245 2024-02-22 22:27:21.000000 llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_xtuner.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     9488 2024-02-04 22:55:45.000000 llm-dataset-converter-0.2.0/src/ldc/text_utils.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.186697 llm-dataset-converter-0.2.0/src/ldc/tool/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-14 22:03:25.000000 llm-dataset-converter-0.2.0/src/ldc/tool/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8605 2024-02-23 01:25:19.000000 llm-dataset-converter-0.2.0/src/ldc/tool/append.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7292 2024-02-21 21:28:28.000000 llm-dataset-converter-0.2.0/src/ldc/tool/convert.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3280 2024-02-20 02:25:09.000000 llm-dataset-converter-0.2.0/src/ldc/tool/download.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3783 2024-02-20 02:26:04.000000 llm-dataset-converter-0.2.0/src/ldc/tool/file_encoding.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7104 2024-02-04 23:37:50.000000 llm-dataset-converter-0.2.0/src/ldc/tool/find.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7164 2024-02-04 22:50:20.000000 llm-dataset-converter-0.2.0/src/ldc/tool/help.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5520 2024-02-05 00:23:10.000000 llm-dataset-converter-0.2.0/src/ldc/tool/paste.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.186697 llm-dataset-converter-0.2.0/src/ldc/translation/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      416 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.0/src/ldc/translation/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    24334 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/translation/_csv.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    11743 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/translation/_jsonlines.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3908 2024-02-20 01:45:23.000000 llm-dataset-converter-0.2.0/src/ldc/translation/_language.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10918 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/translation/_parquet.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3203 2024-02-20 01:44:40.000000 llm-dataset-converter-0.2.0/src/ldc/translation/_require_languages.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    16837 2024-02-20 23:12:19.000000 llm-dataset-converter-0.2.0/src/ldc/translation/_txt.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      931 2024-02-04 22:44:57.000000 llm-dataset-converter-0.2.0/src/ldc/utils.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-02-27 03:38:10.186697 llm-dataset-converter-0.2.0/src/llm_dataset_converter.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8911 2024-02-27 03:38:10.000000 llm-dataset-converter-0.2.0/src/llm_dataset_converter.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2998 2024-02-27 03:38:10.000000 llm-dataset-converter-0.2.0/src/llm_dataset_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-02-27 03:38:10.000000 llm-dataset-converter-0.2.0/src/llm_dataset_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1101 2024-02-27 03:38:10.000000 llm-dataset-converter-0.2.0/src/llm_dataset_converter.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       88 2024-02-27 03:38:10.000000 llm-dataset-converter-0.2.0/src/llm_dataset_converter.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        4 2024-02-27 03:38:10.000000 llm-dataset-converter-0.2.0/src/llm_dataset_converter.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.155106 llm-dataset-converter-0.2.1/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6205 2024-05-02 02:47:22.000000 llm-dataset-converter-0.2.1/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1326 2024-02-27 03:36:56.000000 llm-dataset-converter-0.2.1/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 llm-dataset-converter-0.2.1/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     9521 2024-05-02 02:48:29.155106 llm-dataset-converter-0.2.1/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    26691 2024-05-01 21:39:25.000000 llm-dataset-converter-0.2.1/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-05-02 02:48:29.155106 llm-dataset-converter-0.2.1/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1784 2024-05-02 02:47:22.000000 llm-dataset-converter-0.2.1/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.135106 llm-dataset-converter-0.2.1/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.139106 llm-dataset-converter-0.2.1/src/ldc/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-14 22:03:25.000000 llm-dataset-converter-0.2.1/src/ldc/__init__.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.139106 llm-dataset-converter-0.2.1/src/ldc/api/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       78 2024-02-20 02:26:03.000000 llm-dataset-converter-0.2.1/src/ldc/api/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      740 2024-02-04 22:38:10.000000 llm-dataset-converter-0.2.1/src/ldc/api/_downloader.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      513 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.1/src/ldc/api/_filter.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10115 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.1/src/ldc/api/_io.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4518 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/api/pretrain.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.139106 llm-dataset-converter-0.2.1/src/ldc/api/supervised/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2024-02-20 01:36:43.000000 llm-dataset-converter-0.2.1/src/ldc/api/supervised/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5031 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.1/src/ldc/api/supervised/classification.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4930 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/api/supervised/pairs.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4644 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/api/translation.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      732 2024-05-01 00:00:52.000000 llm-dataset-converter-0.2.1/src/ldc/class_lister.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6705 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.1/src/ldc/core.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.139106 llm-dataset-converter-0.2.1/src/ldc/downloader/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       37 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.1/src/ldc/downloader/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5145 2024-02-20 02:25:09.000000 llm-dataset-converter-0.2.1/src/ldc/downloader/_huggingface.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.147106 llm-dataset-converter-0.2.1/src/ldc/filter/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1525 2024-02-29 00:29:25.000000 llm-dataset-converter-0.2.1/src/ldc/filter/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8050 2024-02-28 21:04:31.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_assemble_sentences.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6900 2024-02-28 21:33:27.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_change_case.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6756 2024-02-21 01:05:00.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_file_filter.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8622 2024-02-28 21:33:27.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_find_substr.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8853 2024-02-29 00:25:34.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_inspect.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7806 2024-02-28 21:33:27.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_keyword.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3362 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_llama2_to_pairs.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3694 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_max_records.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8496 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_metadata.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4725 2024-02-28 20:24:40.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_metadata_from_name.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3716 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_pairs_to_llama2.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4040 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_pairs_to_pretrain.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5430 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_pretrain_sentences_to_classification.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6427 2024-02-21 03:31:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_pretrain_sentences_to_pairs.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3863 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_randomize_records.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4963 2024-02-21 01:05:00.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_record_files.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5367 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_record_window.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8417 2024-02-28 21:47:45.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_remove_blocks.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6807 2024-02-28 21:47:45.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_remove_empty.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7363 2024-02-28 21:50:46.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_remove_patterns.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8077 2024-02-28 21:50:46.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_replace_patterns.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3675 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_reset_ids.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3049 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_skip_duplicate_ids.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6269 2024-02-28 21:55:59.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_skip_duplicate_text.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4994 2024-02-28 20:24:40.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_split.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6087 2024-02-28 20:24:40.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_tee.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8340 2024-02-28 21:55:59.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_text_length.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10587 2024-02-28 21:57:24.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_text_stats.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3555 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_to_llama2_format.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4763 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_translation_to_pairs.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3323 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_translation_to_pretrain.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2923 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.1/src/ldc/help.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.147106 llm-dataset-converter-0.2.1/src/ldc/pretrain/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      383 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    24508 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_csv.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    13378 2024-03-13 03:11:44.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_jsonlines.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4207 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_max_length.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10566 2024-03-13 03:11:44.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_parquet.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5020 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_sentences.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1785 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_split.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    18354 2024-03-13 03:11:44.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_txt.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6875 2024-05-01 05:10:47.000000 llm-dataset-converter-0.2.1/src/ldc/registry.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.147106 llm-dataset-converter-0.2.1/src/ldc/supervised/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-11 04:18:56.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/__init__.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.147106 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      343 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3739 2024-02-20 01:43:12.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_classification_label_map.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    26056 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_csv.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    14455 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_jsonlines.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    11723 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_parquet.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.151106 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      349 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7984 2024-03-13 03:03:11.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_alpaca.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    28291 2024-03-13 03:03:10.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_csv.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    15538 2024-03-13 03:03:10.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_jsonlines.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    13077 2024-03-13 03:04:17.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_parquet.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6051 2024-02-22 22:49:44.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_update_pair_data.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    15245 2024-03-13 03:04:56.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_xtuner.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10910 2024-03-13 03:40:26.000000 llm-dataset-converter-0.2.1/src/ldc/text_utils.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.151106 llm-dataset-converter-0.2.1/src/ldc/tool/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-14 22:03:25.000000 llm-dataset-converter-0.2.1/src/ldc/tool/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8605 2024-02-23 01:25:19.000000 llm-dataset-converter-0.2.1/src/ldc/tool/append.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7292 2024-02-21 21:28:28.000000 llm-dataset-converter-0.2.1/src/ldc/tool/convert.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3280 2024-02-20 02:25:09.000000 llm-dataset-converter-0.2.1/src/ldc/tool/download.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3783 2024-02-20 02:26:04.000000 llm-dataset-converter-0.2.1/src/ldc/tool/file_encoding.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7104 2024-02-04 23:37:50.000000 llm-dataset-converter-0.2.1/src/ldc/tool/find.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7313 2024-05-01 05:12:36.000000 llm-dataset-converter-0.2.1/src/ldc/tool/help.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5520 2024-02-05 00:23:10.000000 llm-dataset-converter-0.2.1/src/ldc/tool/paste.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.151106 llm-dataset-converter-0.2.1/src/ldc/translation/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      416 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.1/src/ldc/translation/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    24398 2024-03-13 03:16:06.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_csv.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    11807 2024-03-13 03:22:55.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_jsonlines.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3908 2024-02-20 01:45:23.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_language.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10982 2024-03-13 03:22:55.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_parquet.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3203 2024-02-20 01:44:40.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_require_languages.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    16901 2024-03-13 03:16:06.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_txt.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      931 2024-02-04 22:44:57.000000 llm-dataset-converter-0.2.1/src/ldc/utils.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.155106 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     9521 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3087 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      371 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       88 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        4 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/top_level.txt
```

### Comparing `llm-dataset-converter-0.2.0/CHANGES.rst` & `llm-dataset-converter-0.2.1/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 =========
 
+0.2.1 (2024-05-02)
+------------------
+
+- filters `split` and `tee` now support `ClassificationData` as well
+- added `metadata-from-name` filter to extract meta-data from the current input file name
+- requiring seppl>=0.1.3 now
+- added `inspect` filter that allows inspecting data interactively as it passes through the pipeline
+- added `empty_str_if_none` helper method to `ldc.text_utils` to ensure no None/null values are output with writers
+- upgraded seppl to 0.2.2 and switched to using `seppl.ClassListerRegistry`
+
+
 0.2.0 (2024-02-27)
 ------------------
 
 - added support for XTuner conversation JSON format: `from-xtuner` and `to-xtuner`
 - added filter `update-pair-data` to allow tweaking or rearranging of the data
 - introduced `ldc.api` module to separate out abstract superclasses and avoid circular imports
 - readers now set the 'file' meta-data value
```

### Comparing `llm-dataset-converter-0.2.0/DESCRIPTION.rst` & `llm-dataset-converter-0.2.1/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/PKG-INFO` & `llm-dataset-converter-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: llm-dataset-converter
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python3 library for converting between various LLM dataset formats.
 Home-page: https://github.com/waikato-llm/llm-dataset-converter
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: The **llm-dataset-converter** allows the conversion between
         various dataset formats for large language models (LLMs).
@@ -63,14 +63,25 @@
                 --output alpaca_data_cleaned-filtered.json
         
         
         
         Changelog
         =========
         
+        0.2.1 (2024-05-02)
+        ------------------
+        
+        - filters `split` and `tee` now support `ClassificationData` as well
+        - added `metadata-from-name` filter to extract meta-data from the current input file name
+        - requiring seppl>=0.1.3 now
+        - added `inspect` filter that allows inspecting data interactively as it passes through the pipeline
+        - added `empty_str_if_none` helper method to `ldc.text_utils` to ensure no None/null values are output with writers
+        - upgraded seppl to 0.2.2 and switched to using `seppl.ClassListerRegistry`
+        
+        
         0.2.0 (2024-02-27)
         ------------------
         
         - added support for XTuner conversation JSON format: `from-xtuner` and `to-xtuner`
         - added filter `update-pair-data` to allow tweaking or rearranging of the data
         - introduced `ldc.api` module to separate out abstract superclasses and avoid circular imports
         - readers now set the 'file' meta-data value
```

### Comparing `llm-dataset-converter-0.2.0/README.md` & `llm-dataset-converter-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -115,22 +115,22 @@
    from-jsonlines-cl, from-jsonlines-pr, from-jsonlines-pt, 
    from-jsonlines-t9n, from-parquet-cl, from-parquet-pr, 
    from-parquet-pt, from-parquet-t9n, from-tsv-cl, from-tsv-pr, 
    from-tsv-pt, from-tsv-t9n, from-txt-pt, from-txt-t9n, from-xtuner
 filters:
    assemble-sentences, change-case, classification-label-map, 
    file-filter, find-substr, keyword, language, llama2-to-pairs, 
-   max-length-pt, max-records, metadata, pairs-to-llama2, 
-   pairs-to-pretrain, pretrain-sentences-to-classification, 
-   pretrain-sentences-to-pairs, randomize-records, record-files, 
-   record-window, remove-blocks, remove-empty, remove-patterns, 
-   replace-patterns, require-languages, reset-ids, sentences-pt, 
-   skip-duplicate-ids, skip-duplicate-text, split, split-pt, tee, 
-   text-length, text-stats, to-llama2-format, translation-to-pairs, 
-   translation-to-pretrain, update-pair-data
+   max-length-pt, max-records, metadata, metadata-from-name, 
+   pairs-to-llama2, pairs-to-pretrain, 
+   pretrain-sentences-to-classification, pretrain-sentences-to-pairs, 
+   randomize-records, record-files, record-window, remove-blocks, 
+   remove-empty, remove-patterns, replace-patterns, require-languages, 
+   reset-ids, sentences-pt, skip-duplicate-ids, skip-duplicate-text, 
+   split, split-pt, tee, text-length, text-stats, to-llama2-format, 
+   translation-to-pairs, translation-to-pretrain, update-pair-data
 writers:
    to-alpaca, to-csv-cl, to-csv-pr, to-csv-pt, to-csv-t9n, 
    to-jsonlines-cl, to-jsonlines-pr, to-jsonlines-pt, to-jsonlines-t9n, 
    to-parquet-cl, to-parquet-pr, to-parquet-pt, to-parquet-t9n, 
    to-tsv-cl, to-tsv-pr, to-tsv-pt, to-tsv-t9n, to-txt-pt, to-txt-t9n, 
    to-xtuner
 
@@ -303,27 +303,27 @@
                         The logging level to use (default: WARN)
 ```
 
 
 ### Generating help screens for plugins
 
 ```
-usage: llm-help [-h] [-m [PACKAGE [PACKAGE ...]]] [-e EXCLUDED_MODULES]
+usage: llm-help [-h] [-c [PACKAGE [PACKAGE ...]]] [-e EXCLUDED_CLASS_LISTERS]
                 [-p NAME] [-f FORMAT] [-L INT] [-o PATH] [-i FILE]
                 [-l {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
 
 Tool for outputting help for plugins in various formats.
 
 optional arguments:
   -h, --help            show this help message and exit
-  -m [PACKAGE [PACKAGE ...]], --modules [PACKAGE [PACKAGE ...]]
-                        The names of the module packages, uses the default
-                        ones if not provided. (default: None)
-  -e EXCLUDED_MODULES, --excluded_modules EXCLUDED_MODULES
-                        The comma-separated list of modules to excluded.
+  -c [PACKAGE [PACKAGE ...]], --custom_class_listers [PACKAGE [PACKAGE ...]]
+                        The names of the custom class listers, uses the
+                        default ones if not provided. (default: None)
+  -e EXCLUDED_CLASS_LISTERS, --excluded_class_listers EXCLUDED_CLASS_LISTERS
+                        The comma-separated list of class listers to excluded.
                         (default: None)
   -p NAME, --plugin_name NAME
                         The name of the plugin to generate the help for,
                         generates it for all if not specified (default: None)
   -f FORMAT, --help_format FORMAT
                         The output format to generate (default: text)
   -L INT, --heading_level INT
@@ -342,28 +342,28 @@
                         The logging level to use. (default: WARN)
 ```
 
 
 ### Plugin registry
 
 ```
-usage: llm-registry [-h] [-m CUSTOM_MODULES] [-e EXCLUDED_MODULES]
-                    [-l {plugins,custom-modules,env-modules,downloaders,readers,filters,writers}]
+usage: llm-registry [-h] [-c CUSTOM_CLASS_LISTERS] [-e EXCLUDED_CLASS_LISTERS]
+                    [-l {plugins,custom-class-listers,env-class-listers,downloaders,readers,filters,writers}]
 
 For inspecting/querying the registry.
 
 optional arguments:
   -h, --help            show this help message and exit
-  -m CUSTOM_MODULES, --custom_modules CUSTOM_MODULES
-                        The comma-separated list of custom modules to use.
+  -c CUSTOM_CLASS_LISTERS, --custom_class_listers CUSTOM_CLASS_LISTERS
+                        The comma-separated list of custom class listers to
+                        use. (default: None)
+  -e EXCLUDED_CLASS_LISTERS, --excluded_class_listers EXCLUDED_CLASS_LISTERS
+                        The comma-separated list of class listers to excluded.
                         (default: None)
-  -e EXCLUDED_MODULES, --excluded_modules EXCLUDED_MODULES
-                        The comma-separated list of modules to excluded.
-                        (default: None)
-  -l {plugins,custom-modules,env-modules,downloaders,readers,filters,writers}, --list {plugins,custom-modules,env-modules,downloaders,readers,filters,writers}
+  -l {plugins,custom-class-listers,env-class-listers,downloaders,readers,filters,writers}, --list {plugins,custom-class-listers,env-class-listers,downloaders,readers,filters,writers}
                         For outputting various lists on stdout. (default:
                         None)
 ```
 
 
 ## Plugins
 
@@ -588,7 +588,58 @@
 
 * [Google integration](https://github.com/waikato-llm/ldc-google)
 * [HTML handling](https://github.com/waikato-llm/ldc-html)
 * [MS Word .docx integration](https://github.com/waikato-llm/ldc-docx)
 * [OpenAI integration](https://github.com/waikato-llm/ldc-openai)
 * [PDF handling](https://github.com/waikato-llm/ldc-pdf)
 * [TinT](https://github.com/waikato-llm/ldc-tint)
+
+
+## Class listers
+
+The *llm-dataset-converter* uses the *class lister registry* provided 
+by the [seppl](https://github.com/waikato-datamining/seppl) library.
+
+Each module defines a function, typically called `list_classes` that returns
+a dictionary of names of superclasses associated with a list of modules that
+should be scanned for derived classes. Here is an example:
+
+```python
+from typing import List, Dict
+
+
+def list_classes() -> Dict[str, List[str]]:
+    return {
+        "ldc.api.Downloader": [
+            "mod.ule1",
+        ],
+        "ldc.api.Reader": [
+            "mod.ule2",
+            "mod.ule3",
+        ],
+        "ldc.api.Filter": [
+            "mod.ule4",
+        ],
+        "seppl.io.Writer": [
+            "mod.ule5",
+        ],
+    }
+```
+
+Such a class lister gets referenced in the `entry_points` section of the `setup.py` file:
+
+```python
+    entry_points={
+        "class_lister": [
+            "unique_string=module_name:function_name",
+        ],
+    },
+```
+
+`:function_name` can be omitted if `:list_classes`.
+
+The following environment variables can be used to influence the class listers:
+
+* `LDC_CLASS_LISTERS`
+* `LDC_CLASS_LISTERS_EXCL`
+
+Each variable is a comma-separated list of `module_name:function_name`, defining the class listers.
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/api/_downloader.py` & `llm-dataset-converter-0.2.1/src/ldc/api/_downloader.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/api/_filter.py` & `llm-dataset-converter-0.2.1/src/ldc/api/_filter.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/api/_io.py` & `llm-dataset-converter-0.2.1/src/ldc/api/_io.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/api/pretrain.py` & `llm-dataset-converter-0.2.1/src/ldc/api/pretrain.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/api/supervised/classification.py` & `llm-dataset-converter-0.2.1/src/ldc/api/supervised/classification.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/api/supervised/pairs.py` & `llm-dataset-converter-0.2.1/src/ldc/api/supervised/pairs.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/api/translation.py` & `llm-dataset-converter-0.2.1/src/ldc/api/translation.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/core.py` & `llm-dataset-converter-0.2.1/src/ldc/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import argparse
 import logging
 
-from typing import List, Union
+from typing import List, Union, Optional
 
 import seppl
 
 from seppl import Plugin, get_class_name
 from seppl import check_compatibility as seppl_check_compatibility
 
 
@@ -57,15 +58,17 @@
                       + COMPARISON_MATCHES + ": regexp match"
 
 LOCATION_ANY = "any"
 LOCATION_INSTRUCTION = "instruction"
 LOCATION_INPUT = "input"
 LOCATION_OUTPUT = "output"
 LOCATION_CONTENT = "content"
-LOCATIONS = [LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT]
+LOCATION_TEXT = "text"
+LOCATIONS = [LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, LOCATION_TEXT]
+LOCATIONS_CLASSIFICATION = [LOCATION_ANY, LOCATION_TEXT]
 LOCATIONS_PAIRS = [LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT]
 LOCATIONS_PRETRAIN = [LOCATION_ANY, LOCATION_CONTENT]
 LOCATIONS_TRANSLATION = [LOCATION_ANY, LOCATION_CONTENT]
 
 
 DEFAULT_END_CHARS = ".!?;:)"
 """ the default end characters for a sentence. """
@@ -169,14 +172,33 @@
 
     if domain in DOMAIN_SUFFIX_LOOKUP:
         return DOMAIN_SUFFIX_LOOKUP[domain]
     else:
         return domain
 
 
+def add_location_argument(parser: argparse.ArgumentParser, help_str: str, default: Optional[str] = LOCATION_ANY):
+    """
+    Adds the location option to the parser.
+
+    :param parser: the parser to add to
+    :type parser: argparse.ArgumentParser
+    :param help_str: the help string preceding the classification/pairs/etc help
+    :type help_str: str
+    :param default: the default location to use
+    :type default: str
+    """
+    parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=default,
+                        help=help_str + "; "
+                             + "classification: " + "|".join(LOCATIONS_CLASSIFICATION)
+                             + ", pairs: " + "|".join(LOCATIONS_PAIRS)
+                             + ", pretrain: " + "|".join(LOCATIONS_PRETRAIN)
+                             + ", translation: " + "|".join(LOCATIONS_PRETRAIN))
+
+
 def locations_match(locations: Union[str, List[str]], required: Union[str, List[str]]) -> bool:
     """
     Checks whether at least one of locations is present in the required list.
 
     :param locations: the location(s) to check
     :type locations: str or list
     :param required: the required location(s)
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/downloader/_huggingface.py` & `llm-dataset-converter-0.2.1/src/ldc/downloader/_huggingface.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/__init__.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from ._assemble_sentences import AssembleSentences
 from ._change_case import ChangeCase, CASES, CASE_UNCHANGED, CASE_LOWER, CASE_UPPER, CASE_TITLE
 from ._file_filter import FileFilter
 from ._find_substr import FindSubstring
+from ._inspect import Inspect, MODES, MODE_NONINTERACTIVE, MODE_INTERACTIVE, OUTPUTS, OUTPUT_STDOUT, OUTPUT_STDERR, OUTPUT_LOGGER, OUTPUT_FILE
 from ._keyword import Keyword
 from ._llama2_to_pairs import Llama2ToPairs
 from ._max_records import MaxRecords
 from ._metadata import MetaData
+from ._metadata_from_name import MetaDataFromName
 from ._pairs_to_llama2 import PairsToLlama2
 from ._pairs_to_pretrain import PairsToPretrain
 from ._pretrain_sentences_to_classification import PretrainSentencesToClassification
 from ._pretrain_sentences_to_pairs import PretrainSentencesToPairs
 from ._randomize_records import RandomizeRecords
 from ._record_files import RecordFiles
 from ._record_window import RecordWindow
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_assemble_sentences.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_assemble_sentences.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import argparse
 import copy
 from typing import List, Union
 
 from wai.logging import LOGGING_WARNING
-from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DEFAULT_END_CHARS, DEFAULT_QUOTE_CHARS
-from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
-    LOCATIONS, LOCATIONS_PAIRS, LOCATIONS_PRETRAIN, locations_match
+
+from ldc.api import Filter
 from ldc.api.pretrain import PretrainData
+from ldc.api.supervised.classification import ClassificationData
 from ldc.api.supervised.pairs import PairData
 from ldc.api.translation import TranslationData
-from ldc.api import Filter
+from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION
+from ldc.core import DEFAULT_END_CHARS, DEFAULT_QUOTE_CHARS
+from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
+    LOCATION_TEXT, LOCATIONS, locations_match, add_location_argument
 from ldc.text_utils import assemble_preformatted, split_into_sentences, combine_sentences
 
 
 class AssembleSentences(Filter):
     """
     For keeping sentences together, e.g., when reading preformatted text.
     """
@@ -71,48 +74,46 @@
     def domains(self) -> List[str]:
         """
         Returns the domains of the filter.
 
         :return: the domains
         :rtype: list
         """
-        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]
+        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]
 
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
         """
         parser = super()._create_argparser()
         parser.add_argument("-c", "--end_chars", type=str, help="The characters signifying the end of a sentence.", default=DEFAULT_END_CHARS, required=False)
         parser.add_argument("-q", "--quote_chars", type=str, help="The characters that represent quotes.", default=DEFAULT_QUOTE_CHARS, required=False)
         parser.add_argument("-m", "--max_sentences", type=int, help="The maximum number of sentences per line.", default=1, required=False)
-        parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=LOCATION_ANY, help="Where to look for the keywords; pairs: " + ",".join(
-            LOCATIONS_PAIRS) + ", pretrain: " + ",".join(LOCATIONS_PRETRAIN) + ", translation: " + ",".join(
-            LOCATIONS_PRETRAIN))
+        add_location_argument(parser, "Where to assemble the sentences")
         parser.add_argument("-g", "--language", type=str, help="The languages to inspect; inspects all if not specified", required=False, nargs="*")
         return parser
 
     def _apply_args(self, ns: argparse.Namespace):
         """
         Initializes the object with the arguments of the parsed namespace.
 
@@ -170,14 +171,17 @@
         if isinstance(data, PairData):
             if locations_match(self.location, LOCATION_INSTRUCTION):
                 data.instruction = self._assemble_sentences(data.instruction)
             if locations_match(self.location, LOCATION_INPUT):
                 data.input = self._assemble_sentences(data.input)
             if locations_match(self.location, LOCATION_OUTPUT):
                 data.output = self._assemble_sentences(data.output)
+        elif isinstance(data, ClassificationData):
+            if locations_match(self.location, LOCATION_TEXT):
+                data.text = self._assemble_sentences(data.text)
         elif isinstance(data, PretrainData):
             if locations_match(self.location, LOCATION_CONTENT):
                 data.content = self._assemble_sentences(data.content)
         elif isinstance(data, TranslationData):
             if self.languages is None:
                 for k in data.translations:
                     data.translations[k] = self._assemble_sentences(data.translations[k])
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_change_case.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_change_case.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import argparse
 from typing import List, Union
 
 from wai.logging import LOGGING_WARNING
-from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION
+from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION
 from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
-    LOCATIONS, LOCATIONS_PAIRS, LOCATIONS_PRETRAIN, locations_match
+    LOCATION_TEXT, LOCATIONS, locations_match, add_location_argument
 from ldc.api.pretrain import PretrainData
+from ldc.api.supervised.classification import ClassificationData
 from ldc.api.supervised.pairs import PairData
 from ldc.api.translation import TranslationData
 from ldc.api import Filter
 
 CASE_UNCHANGED = "unchanged"
 CASE_LOWER = "lower"
 CASE_UPPER = "upper"
@@ -79,46 +80,44 @@
     def domains(self) -> List[str]:
         """
         Returns the domains of the filter.
 
         :return: the domains
         :rtype: list
         """
-        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]
+        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]
 
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
         """
         parser = super()._create_argparser()
         parser.add_argument("-c", "--case", choices=CASES, default=CASE_LOWER, help="How to change the case of the text")
-        parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=LOCATION_ANY, help="Where to look for the keywords; pairs: " + ",".join(
-            LOCATIONS_PAIRS) + ", pretrain: " + ",".join(LOCATIONS_PRETRAIN) + ", translation: " + ",".join(
-            LOCATIONS_PRETRAIN))
+        add_location_argument(parser, "Which data to update")
         parser.add_argument("-g", "--language", type=str, help="The languages to inspect; inspects all if not specified", required=False, nargs="*")
         return parser
 
     def _apply_args(self, ns: argparse.Namespace):
         """
         Initializes the object with the arguments of the parsed namespace.
 
@@ -169,14 +168,17 @@
         if isinstance(data, PairData):
             if locations_match(self.location, LOCATION_INSTRUCTION):
                 data.instruction = self._change_case(data.instruction)
             if locations_match(self.location, LOCATION_INPUT):
                 data.input = self._change_case(data.input)
             if locations_match(self.location, LOCATION_OUTPUT):
                 data.output = self._change_case(data.output)
+        elif isinstance(data, ClassificationData):
+            if locations_match(self.location, LOCATION_TEXT):
+                data.text = self._change_case(data.text)
         elif isinstance(data, PretrainData):
             if locations_match(self.location, LOCATION_CONTENT):
                 data.content = self._change_case(data.content)
         elif isinstance(data, TranslationData):
             if self.languages is None:
                 for k in data.translations:
                     data.translations[k] = self._change_case(data.translations[k])
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_file_filter.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_file_filter.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_find_substr.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_find_substr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import argparse
 import re
 from typing import List, Union
 
 from wai.logging import LOGGING_WARNING
-from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION
+from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION
 from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
-    LOCATIONS, LOCATIONS_PAIRS, LOCATIONS_PRETRAIN, locations_match
+    LOCATION_TEXT, LOCATIONS, locations_match, add_location_argument
 from ldc.api.pretrain import PretrainData
+from ldc.api.supervised.classification import ClassificationData
 from ldc.api.supervised.pairs import PairData
 from ldc.api.translation import TranslationData
 from ldc.api import Filter, FILTER_ACTIONS, FILTER_ACTION_DISCARD, FILTER_ACTION_KEEP
 
 
 class FindSubstring(Filter):
     """
@@ -75,47 +76,45 @@
     def domains(self) -> List[str]:
         """
         Returns the domains of the filter.
 
         :return: the domains
         :rtype: list
         """
-        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]
+        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]
 
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
         """
         parser = super()._create_argparser()
         parser.add_argument("-s", "--sub_string", type=str, help="The substrings to look for (lower case)", required=True, nargs="+")
         parser.add_argument("-r", "--is_regexp", action="store_true", help="Whether the sub-strings represent regular expressions", required=False)
-        parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=LOCATION_ANY, help="Where to look for the substrings; pairs: " + ",".join(
-            LOCATIONS_PAIRS) + ", pretrain: " + ",".join(LOCATIONS_PRETRAIN) + ", translation: " + ",".join(
-            LOCATIONS_PRETRAIN))
+        add_location_argument(parser, "Where to look for the substrings")
         parser.add_argument("-g", "--language", type=str, help="The languages to inspect; inspects all if not specified", required=False, nargs="*")
         parser.add_argument("-a", "--action", choices=FILTER_ACTIONS, default=FILTER_ACTION_KEEP, help="How to react when a substring is found")
         return parser
 
     def _apply_args(self, ns: argparse.Namespace):
         """
         Initializes the object with the arguments of the parsed namespace.
@@ -158,14 +157,17 @@
         if isinstance(data, PairData):
             if locations_match(self.location, LOCATION_INSTRUCTION):
                 result.append(data.instruction.lower())
             if locations_match(self.location, LOCATION_INPUT):
                 result.append(data.input.lower())
             if locations_match(self.location, LOCATION_OUTPUT):
                 result.append(data.output.lower())
+        elif isinstance(data, ClassificationData):
+            if locations_match(self.location, LOCATION_TEXT):
+                result.append(data.text.lower())
         elif isinstance(data, PretrainData):
             if locations_match(self.location, LOCATION_CONTENT):
                 result.append(data.content.lower())
         elif isinstance(data, TranslationData):
             if self.languages is None:
                 for k in data.translations:
                     result.append(data.translations[k].lower())
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_keyword.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_keyword.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import argparse
 from typing import List, Set, Union
 
 from wai.logging import LOGGING_WARNING
-from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION
+from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION
 from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
-    LOCATIONS, LOCATIONS_PAIRS, LOCATIONS_PRETRAIN, locations_match
+    LOCATION_TEXT, LOCATIONS, locations_match, add_location_argument
 from ldc.api.pretrain import PretrainData
+from ldc.api.supervised.classification import ClassificationData
 from ldc.api.supervised.pairs import PairData
 from ldc.api.translation import TranslationData
 from ldc.api import Filter, FILTER_ACTIONS, FILTER_ACTION_DISCARD, FILTER_ACTION_KEEP
 
 
 class Keyword(Filter):
     """
@@ -70,46 +71,44 @@
     def domains(self) -> List[str]:
         """
         Returns the domains of the filter.
 
         :return: the domains
         :rtype: list
         """
-        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]
+        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]
 
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
         """
         parser = super()._create_argparser()
         parser.add_argument("-k", "--keyword", type=str, help="The keywords to look for (lower case)", required=True, nargs="+")
-        parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=LOCATION_ANY, help="Where to look for the keywords; pairs: " + ",".join(
-            LOCATIONS_PAIRS) + ", pretrain: " + ",".join(LOCATIONS_PRETRAIN) + ", translation: " + ",".join(
-            LOCATIONS_PRETRAIN))
+        add_location_argument(parser, "Where to look for the keywords")
         parser.add_argument("-g", "--language", type=str, help="The languages to inspect; inspects all if not specified", required=False, nargs="*")
         parser.add_argument("-a", "--action", choices=FILTER_ACTIONS, default=FILTER_ACTION_KEEP, help="How to react when a keyword is encountered")
         return parser
 
     def _apply_args(self, ns: argparse.Namespace):
         """
         Initializes the object with the arguments of the parsed namespace.
@@ -150,14 +149,17 @@
         if isinstance(data, PairData):
             if locations_match(self.location, LOCATION_INSTRUCTION):
                 words.update(data.instruction.lower().split())
             if locations_match(self.location, LOCATION_INPUT):
                 words.update(data.input.lower().split())
             if locations_match(self.location, LOCATION_OUTPUT):
                 words.update(data.output.lower().split())
+        elif isinstance(data, ClassificationData):
+            if locations_match(self.location, LOCATION_TEXT):
+                words.update(data.text.lower().split())
         elif isinstance(data, PretrainData):
             if locations_match(self.location, LOCATION_CONTENT):
                 words.update(data.content.lower().split())
         elif isinstance(data, TranslationData):
             if self.languages is None:
                 for k in data.translations:
                     words.update(data.translations[k].lower().split())
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_llama2_to_pairs.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_llama2_to_pairs.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_max_records.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_max_records.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_metadata.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_metadata.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_pairs_to_llama2.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_pairs_to_llama2.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_pairs_to_pretrain.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_pairs_to_pretrain.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_pretrain_sentences_to_classification.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_pretrain_sentences_to_classification.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_pretrain_sentences_to_pairs.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_pretrain_sentences_to_pairs.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_randomize_records.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_randomize_records.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_record_files.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_record_files.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_record_window.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_record_window.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_remove_blocks.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_remove_blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import argparse
 import copy
 from typing import List, Tuple, Union
 
 from wai.logging import LOGGING_WARNING
-from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION
+from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION
 from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
-    LOCATIONS, LOCATIONS_PAIRS, LOCATIONS_PRETRAIN, locations_match
+    LOCATION_TEXT, LOCATIONS, locations_match, add_location_argument
 from ldc.api.pretrain import PretrainData
+from ldc.api.supervised.classification import ClassificationData
 from ldc.api.supervised.pairs import PairData
 from ldc.api.translation import TranslationData
 from ldc.text_utils import remove_blocks
 from ldc.api import Filter
 
 
 class RemoveBlocks(Filter):
@@ -69,47 +70,45 @@
     def domains(self) -> List[str]:
         """
         Returns the domains of the filter.
 
         :return: the domains
         :rtype: list
         """
-        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]
+        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]
 
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
         """
         parser = super()._create_argparser()
         parser.add_argument("--block_removal_start", type=str, help="The starting strings for blocks to remove", required=False, nargs="*")
         parser.add_argument("--block_removal_end", type=str, help="The ending strings for blocks to remove", required=False, nargs="*")
-        parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=LOCATION_ANY, help="Where to look for the keywords; pairs: " + ",".join(
-            LOCATIONS_PAIRS) + ", pretrain: " + ",".join(LOCATIONS_PRETRAIN) + ", translation: " + ",".join(
-            LOCATIONS_PRETRAIN))
+        add_location_argument(parser, "Where to remove the blocks")
         parser.add_argument("-g", "--language", type=str, help="The languages to inspect; inspects all if not specified", required=False, nargs="*")
         return parser
 
     def _apply_args(self, ns: argparse.Namespace):
         """
         Initializes the object with the arguments of the parsed namespace.
 
@@ -171,14 +170,18 @@
                 removed += r
             if locations_match(self.location, LOCATION_INPUT):
                 data.input, r = self._remove_blocks(data.input)
                 removed += r
             if locations_match(self.location, LOCATION_OUTPUT):
                 data.output, r = self._remove_blocks(data.output)
                 removed += r
+        elif isinstance(data, ClassificationData):
+            if locations_match(self.location, LOCATION_TEXT):
+                data.text, r = self._remove_blocks(data.text)
+                removed += r
         elif isinstance(data, PretrainData):
             if locations_match(self.location, LOCATION_CONTENT):
                 data.content, r = self._remove_blocks(data.content)
                 removed += r
         elif isinstance(data, TranslationData):
             if self.languages is None:
                 for k in data.translations:
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_remove_empty.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_remove_empty.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import argparse
 import copy
 from typing import List, Tuple, Union
 
 from wai.logging import LOGGING_WARNING
-from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION
+from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION
 from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
-    LOCATIONS, LOCATIONS_PAIRS, LOCATIONS_PRETRAIN, locations_match
+    LOCATION_TEXT, LOCATIONS, locations_match, add_location_argument
 from ldc.api.pretrain import PretrainData
+from ldc.api.supervised.classification import ClassificationData
 from ldc.api.supervised.pairs import PairData
 from ldc.api.translation import TranslationData
 from ldc.text_utils import remove_empty
 from ldc.api import Filter
 
 
 class RemoveEmpty(Filter):
@@ -62,45 +63,43 @@
     def domains(self) -> List[str]:
         """
         Returns the domains of the filter.
 
         :return: the domains
         :rtype: list
         """
-        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]
+        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]
 
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
         """
         parser = super()._create_argparser()
-        parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=LOCATION_ANY, help="Where to look for the keywords; pairs: " + ",".join(
-            LOCATIONS_PAIRS) + ", pretrain: " + ",".join(LOCATIONS_PRETRAIN) + ", translation: " + ",".join(
-            LOCATIONS_PRETRAIN))
+        add_location_argument(parser, "Where to remove empty lines")
         parser.add_argument("-g", "--language", type=str, help="The languages to inspect; inspects all if not specified", required=False, nargs="*")
         return parser
 
     def _apply_args(self, ns: argparse.Namespace):
         """
         Initializes the object with the arguments of the parsed namespace.
 
@@ -153,14 +152,18 @@
                 removed += r
             if locations_match(self.location, LOCATION_INPUT):
                 data.input, r = self._remove_empty(data.input)
                 removed += r
             if locations_match(self.location, LOCATION_OUTPUT):
                 data.output, r = self._remove_empty(data.output)
                 removed += r
+        elif isinstance(data, ClassificationData):
+            if locations_match(self.location, LOCATION_TEXT):
+                data.text, r = self._remove_empty(data.text)
+                removed += r
         elif isinstance(data, PretrainData):
             if locations_match(self.location, LOCATION_CONTENT):
                 data.content, r = self._remove_empty(data.content)
                 removed += r
         elif isinstance(data, TranslationData):
             if self.languages is None:
                 for k in data.translations:
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_remove_patterns.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_remove_patterns.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import argparse
 import copy
 from typing import List, Tuple, Union
 
 from wai.logging import LOGGING_WARNING
-from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION
+from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION
 from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
-    LOCATIONS, LOCATIONS_PAIRS, LOCATIONS_PRETRAIN, locations_match
+    LOCATION_TEXT, LOCATIONS, locations_match, add_location_argument
 from ldc.api.pretrain import PretrainData
+from ldc.api.supervised.classification import ClassificationData
 from ldc.api.supervised.pairs import PairData
 from ldc.api.translation import TranslationData
 from ldc.text_utils import remove_patterns
 from ldc.api import Filter
 
 
 class RemovePatterns(Filter):
@@ -66,46 +67,44 @@
     def domains(self) -> List[str]:
         """
         Returns the domains of the filter.
 
         :return: the domains
         :rtype: list
         """
-        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]
+        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]
 
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
         """
         parser = super()._create_argparser()
         parser.add_argument("-r", "--expr_remove", type=str, default=None, help="Regular expressions for removing sub-strings from the text (gets applied before skipping empty lines); uses re.sub(...).", nargs="*")
-        parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=LOCATION_ANY, help="Where to look for the keywords; pairs: " + ",".join(
-            LOCATIONS_PAIRS) + ", pretrain: " + ",".join(LOCATIONS_PRETRAIN) + ", translation: " + ",".join(
-            LOCATIONS_PRETRAIN))
+        add_location_argument(parser, "Where to remove the patterns")
         parser.add_argument("-g", "--language", type=str, help="The languages to inspect; inspects all if not specified", required=False, nargs="*")
         return parser
 
     def _apply_args(self, ns: argparse.Namespace):
         """
         Initializes the object with the arguments of the parsed namespace.
 
@@ -155,14 +154,18 @@
                 removed += r
             if locations_match(self.location, LOCATION_INPUT):
                 data.input, r = self._remove_patterns(data.input)
                 removed += r
             if locations_match(self.location, LOCATION_OUTPUT):
                 data.output, r = self._remove_patterns(data.output)
                 removed += r
+        elif isinstance(data, ClassificationData):
+            if locations_match(self.location, LOCATION_TEXT):
+                data.text, r = self._remove_patterns(data.text)
+                removed += r
         elif isinstance(data, PretrainData):
             if locations_match(self.location, LOCATION_CONTENT):
                 data.content, r = self._remove_patterns(data.content)
                 removed += r
         elif isinstance(data, TranslationData):
             if self.languages is None:
                 for k in data.translations:
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_replace_patterns.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_replace_patterns.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import argparse
 import copy
 from typing import List, Tuple, Union
 
 from wai.logging import LOGGING_WARNING
-from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION
+from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION
 from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
-    LOCATIONS, LOCATIONS_PAIRS, LOCATIONS_PRETRAIN, locations_match
+    LOCATION_TEXT, LOCATIONS, locations_match, add_location_argument
 from ldc.api.pretrain import PretrainData
+from ldc.api.supervised.classification import ClassificationData
 from ldc.api.supervised.pairs import PairData
 from ldc.api.translation import TranslationData
 from ldc.text_utils import replace_patterns
 from ldc.api import Filter
 
 
 class ReplacePatterns(Filter):
@@ -69,47 +70,45 @@
     def domains(self) -> List[str]:
         """
         Returns the domains of the filter.
 
         :return: the domains
         :rtype: list
         """
-        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]
+        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]
 
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
         """
         parser = super()._create_argparser()
         parser.add_argument("-f", "--find", type=str, default=None, help="Regular expressions for replacing sub-strings in the text (gets applied before skipping empty lines); uses re.sub(...).", nargs="*")
         parser.add_argument("-r", "--replace", type=str, default=None, help="The corresponding replacement strings.", nargs="*")
-        parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=LOCATION_ANY, help="Where to look for the keywords; pairs: " + ",".join(
-            LOCATIONS_PAIRS) + ", pretrain: " + ",".join(LOCATIONS_PRETRAIN) + ", translation: " + ",".join(
-            LOCATIONS_PRETRAIN))
+        add_location_argument(parser, "Where to replace the patterns")
         parser.add_argument("-g", "--language", type=str, help="The languages to inspect; inspects all if not specified", required=False, nargs="*")
         return parser
 
     def _apply_args(self, ns: argparse.Namespace):
         """
         Initializes the object with the arguments of the parsed namespace.
 
@@ -166,14 +165,18 @@
                 removed += r
             if locations_match(self.location, LOCATION_INPUT):
                 data.input, r = self._replace_patterns(data.input)
                 removed += r
             if locations_match(self.location, LOCATION_OUTPUT):
                 data.output, r = self._replace_patterns(data.output)
                 removed += r
+        elif isinstance(data, ClassificationData):
+            if locations_match(self.location, LOCATION_TEXT):
+                data.text, r = self._replace_patterns(data.text)
+                removed += r
         elif isinstance(data, PretrainData):
             if locations_match(self.location, LOCATION_CONTENT):
                 data.content, r = self._replace_patterns(data.content)
                 removed += r
         elif isinstance(data, TranslationData):
             if self.languages is None:
                 for k in data.translations:
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_reset_ids.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_reset_ids.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_skip_duplicate_ids.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_skip_duplicate_ids.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_skip_duplicate_text.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_skip_duplicate_text.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import argparse
 from typing import List, Union
 
 from wai.logging import LOGGING_WARNING
-from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION
+from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION
 from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
-    LOCATIONS, LOCATIONS_PAIRS, LOCATIONS_PRETRAIN, locations_match
+    LOCATION_TEXT, LOCATIONS, locations_match, add_location_argument
 from ldc.api.pretrain import PretrainData
+from ldc.api.supervised.classification import ClassificationData
 from ldc.api.supervised.pairs import PairData
 from ldc.api.translation import TranslationData
 from ldc.api import Filter
 
 
 class SkipDuplicateText(Filter):
     """
@@ -59,45 +60,43 @@
     def domains(self) -> List[str]:
         """
         Returns the domains of the handler.
 
         :return: the domains
         :rtype: list
         """
-        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]
+        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]
 
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
         """
         parser = super()._create_argparser()
-        parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=LOCATION_ANY, help="Where to look for the keywords; pairs: " + ",".join(
-            LOCATIONS_PAIRS) + ", pretrain: " + ",".join(LOCATIONS_PRETRAIN) + ", translation: " + ",".join(
-            LOCATIONS_PRETRAIN))
+        add_location_argument(parser, "Which portion to take into account for detecting duplicate text")
         parser.add_argument("-g", "--language", type=str, help="The languages to inspect; inspects all if not specified", required=False, nargs="*")
         return parser
 
     def _apply_args(self, ns: argparse.Namespace):
         """
         Initializes the object with the arguments of the parsed namespace.
 
@@ -132,14 +131,17 @@
         if isinstance(data, PairData):
             if locations_match(self.location, LOCATION_INSTRUCTION):
                 words.append(data.instruction.lower())
             if locations_match(self.location, LOCATION_INPUT):
                 words.append(data.input.lower())
             if locations_match(self.location, LOCATION_OUTPUT):
                 words.append(data.output.lower())
+        elif isinstance(data, ClassificationData):
+            if locations_match(self.location, LOCATION_TEXT):
+                words.append(data.text.lower())
         elif isinstance(data, PretrainData):
             if locations_match(self.location, LOCATION_CONTENT):
                 words.append(data.content.lower())
         elif isinstance(data, TranslationData):
             if self.languages is None:
                 for k in data.translations:
                     words.append(data.translations[k].lower())
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_split.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_split.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import argparse
 from typing import List
 
 from wai.logging import LOGGING_WARNING
-from seppl import MetaDataHandler, get_metadata
-from seppl.io import Splitter
-from ldc.core import DOMAIN_ANY
-from ldc.api.pretrain import PretrainData
-from ldc.api.supervised.pairs import PairData
-from ldc.api.translation import TranslationData
+
 from ldc.api import Filter
+from ldc.core import DOMAIN_ANY
+from seppl import MetaDataHandler, get_metadata, AnyData
+from seppl.io import Splitter
 
 META_SPLIT = "split"
 """ the key for storing the split name in the meta-data. """
 
 
 class Split(Filter):
     """
@@ -68,24 +66,24 @@
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [AnyData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [AnyData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_tee.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_tee.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import argparse
 from typing import List
 
 from wai.logging import LOGGING_WARNING
-from seppl import split_args, split_cmdline, Plugin
-from seppl.io import Writer, BatchWriter, StreamWriter
-from ldc.core import DOMAIN_ANY
-from ldc.api.pretrain import PretrainData
-from ldc.api.supervised.pairs import PairData
-from ldc.api.translation import TranslationData
+
 from ldc.api import Filter, MultiFilter
+from ldc.core import DOMAIN_ANY
+from seppl import split_args, split_cmdline, Plugin, AnyData
+from seppl.io import Writer, BatchWriter, StreamWriter
 
 
 class Tee(Filter):
     """
     Forwards the data coming through to the sub-flow.
     """
 
@@ -64,24 +62,24 @@
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [AnyData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [AnyData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_text_length.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_text_length.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import argparse
 from typing import List, Optional, Union
 
 from wai.logging import LOGGING_WARNING
-from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION
+from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION
 from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
-    LOCATIONS, LOCATIONS_PAIRS, LOCATIONS_PRETRAIN, LOCATIONS_TRANSLATION, locations_match
+    LOCATION_TEXT, LOCATIONS, locations_match, add_location_argument
 from ldc.api.pretrain import PretrainData
+from ldc.api.supervised.classification import ClassificationData
 from ldc.api.supervised.pairs import PairData
 from ldc.api.translation import TranslationData
 from ldc.api import Filter
 
 
 class TextLength(Filter):
     """
@@ -68,45 +69,45 @@
     def domains(self) -> List[str]:
         """
         Returns the domains of the filter.
 
         :return: the domains
         :rtype: list
         """
-        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]
+        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]
 
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
         """
         parser = super()._create_argparser()
         parser.add_argument("-m", "--min_length", type=int, help="The minimum text length, ignored if <0", default=-1, required=False)
         parser.add_argument("-M", "--max_length", type=int, help="The maximum text length, ignored if <0", default=-1, required=False)
-        parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=LOCATION_ANY, help="Where to look for the text; pairs: " + ",".join(LOCATIONS_PAIRS) + ", pretrain: " + ",".join(LOCATIONS_PRETRAIN) + ", translation: " + ",".join(LOCATIONS_TRANSLATION))
+        add_location_argument(parser, "Where to apply the checks")
         parser.add_argument("-g", "--language", type=str, help="The languages to inspect; inspects all if not specified", required=False, nargs="*")
         return parser
 
     def _apply_args(self, ns: argparse.Namespace):
         """
         Initializes the object with the arguments of the parsed namespace.
 
@@ -164,14 +165,17 @@
         if isinstance(data, PairData):
             if locations_match(self.location, LOCATION_INSTRUCTION):
                 self._add_length(data.instruction, lengths)
             if locations_match(self.location, LOCATION_INPUT):
                 self._add_length(data.input, lengths)
             if locations_match(self.location, LOCATION_OUTPUT):
                 self._add_length(data.output, lengths)
+        elif isinstance(data, ClassificationData):
+            if locations_match(self.location, LOCATION_TEXT):
+                self._add_length(data.text, lengths)
         elif isinstance(data, PretrainData):
             if locations_match(self.location, LOCATION_CONTENT):
                 self._add_length(data.content, lengths)
         elif isinstance(data, TranslationData):
             if self.languages is None:
                 for k in data.translations:
                     self._add_length(data.translations[k], lengths)
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_text_stats.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_text_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import sys
 import yaml
 
 from dataclasses import dataclass, field
 from typing import List, Dict, Union
 
 from wai.logging import LOGGING_WARNING
-from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION
+from ldc.core import DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION
 from ldc.core import LOCATION_ANY, LOCATION_INSTRUCTION, LOCATION_INPUT, LOCATION_OUTPUT, LOCATION_CONTENT, \
-    LOCATIONS, LOCATIONS_PAIRS, LOCATIONS_PRETRAIN, LOCATIONS_TRANSLATION, locations_match
+    LOCATION_TEXT, LOCATIONS, locations_match, add_location_argument
 from ldc.api.pretrain import PretrainData
+from ldc.api.supervised.classification import ClassificationData
 from ldc.api.supervised.pairs import PairData
 from ldc.api.translation import TranslationData
 from ldc.api import Filter
 
 
 @dataclass
 class Statistics:
@@ -111,45 +112,45 @@
     def domains(self) -> List[str]:
         """
         Returns the domains of the filter.
 
         :return: the domains
         :rtype: list
         """
-        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]
+        return [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]
 
     def accepts(self) -> List:
         """
         Returns the list of classes that are accepted.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def generates(self) -> List:
         """
         Returns the list of classes that get produced.
 
         :return: the list of classes
         :rtype: list
         """
-        return [PairData, PretrainData, TranslationData]
+        return [PairData, PretrainData, TranslationData, ClassificationData]
 
     def _create_argparser(self) -> argparse.ArgumentParser:
         """
         Creates an argument parser. Derived classes need to fill in the options.
 
         :return: the parser
         :rtype: argparse.ArgumentParser
         """
         parser = super()._create_argparser()
         parser.add_argument("-o", "--output", type=str, help="The JSON file to store the statistics in; outputs a textual representation on stdout when missing", required=False, default=None)
         parser.add_argument("-d", "--detailed", action="store_true", help="Whether to output more detailed statistics, e.g., the counts per string length", required=False)
-        parser.add_argument("-L", "--location", choices=LOCATIONS, nargs="*", default=LOCATION_ANY, help="Where to look for the text; pairs: " + ",".join(LOCATIONS_PAIRS) + ", pretrain: " + ",".join(LOCATIONS_PRETRAIN) + ", translation: " + ",".join(LOCATIONS_TRANSLATION))
+        add_location_argument(parser, "Which text to use")
         parser.add_argument("-g", "--language", type=str, help="The languages to inspect; inspects all if not specified", required=False, nargs="*")
         return parser
 
     def _apply_args(self, ns: argparse.Namespace):
         """
         Initializes the object with the arguments of the parsed namespace.
 
@@ -199,15 +200,15 @@
         :param location: the location where the string was taken from
         :type location: str
         :param language: the language this string was taken from (if applicable)
         :type language: str
         :param s: the string to use for the update
         :type s: str
         """
-        if domain not in [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION]:
+        if domain not in [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_TRANSLATION, DOMAIN_CLASSIFICATION]:
             raise Exception("Unhandled domain: %s" % domain)
 
         # per domain
         if domain not in self._stats:
             self._stats[domain] = Statistics()
         self._update_container(self._stats[domain], s)
 
@@ -217,15 +218,15 @@
                 self._stats[domain].stats = dict()
                 self._stats[domain].stats_name = "languages"
             if language not in self._stats[domain].stats:
                 self._stats[domain].stats[language] = Statistics()
             self._update_container(self._stats[domain].stats[language], s)
 
         # per location
-        if domain == DOMAIN_PAIRS:
+        if domain in [DOMAIN_PAIRS, DOMAIN_PRETRAIN, DOMAIN_CLASSIFICATION]:
             if self._stats[domain].stats is None:
                 self._stats[domain].stats = dict()
             self._stats[domain].stats_name = "locations"
             if location not in self._stats[domain].stats:
                 self._stats[domain].stats[location] = Statistics()
             self._update_container(self._stats[domain].stats[location], s)
 
@@ -239,14 +240,17 @@
         if isinstance(data, PairData):
             if locations_match(self.location, LOCATION_INSTRUCTION):
                 self._update(DOMAIN_PAIRS, LOCATION_INSTRUCTION, "", data.instruction)
             if locations_match(self.location, LOCATION_INPUT):
                 self._update(DOMAIN_PAIRS, LOCATION_INPUT, "", data.input)
             if locations_match(self.location, LOCATION_OUTPUT):
                 self._update(DOMAIN_PAIRS, LOCATION_OUTPUT, "", data.output)
+        elif isinstance(data, ClassificationData):
+            if locations_match(self.location, LOCATION_TEXT):
+                self._update(DOMAIN_CLASSIFICATION, LOCATION_TEXT, "", data.text)
         elif isinstance(data, PretrainData):
             if locations_match(self.location, LOCATION_CONTENT):
                 self._update(DOMAIN_PRETRAIN, LOCATION_CONTENT, "", data.content)
         elif isinstance(data, TranslationData):
             if self.languages is None:
                 for k in data.translations:
                     self._update(DOMAIN_TRANSLATION, "", k, data.translations[k])
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_to_llama2_format.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_to_llama2_format.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_translation_to_pairs.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_translation_to_pairs.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/filter/_translation_to_pretrain.py` & `llm-dataset-converter-0.2.1/src/ldc/filter/_translation_to_pretrain.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/help.py` & `llm-dataset-converter-0.2.1/src/ldc/help.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/pretrain/_csv.py` & `llm-dataset-converter-0.2.1/src/ldc/pretrain/_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import open_file, generate_output
 from ldc.api.pretrain import PretrainData, PretrainReader, BatchPretrainWriter
 from ldc.utils import str_to_column_index
+from ldc.text_utils import empty_str_if_none
 
 
 class AbstractCsvLikePretrainReader(PretrainReader, abc.ABC):
     """
     Ancestor for readers of CSV-like files.
     """
 
@@ -336,17 +337,17 @@
                 if self.col_id is not None:
                     row.append(self.col_id)
                 row.append(self.col_content)
                 self._output_writer.writerow(row)
 
         for item in data:
             if self.split_lines:
-                lines = item.content.split("\n")
+                lines = empty_str_if_none(item.content).split("\n")
             else:
-                lines = [item.content]
+                lines = [empty_str_if_none(item.content)]
             for i, line in enumerate(lines):
                 row = []
                 if self.col_id is not None:
                     if (item.meta is not None) and ("id" in item.meta):
                         id_ = item.meta["id"]
                         if self.split_lines:
                             id_ += "-" + str(i)
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/pretrain/_jsonlines.py` & `llm-dataset-converter-0.2.1/src/ldc/pretrain/_jsonlines.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import open_file, generate_output, is_compressed
 from ldc.api.pretrain import PretrainData, PretrainReader, StreamPretrainWriter
+from ldc.text_utils import empty_str_if_none
 
 
 class JsonLinesPretrainReader(PretrainReader):
     """
     Reader for the JsonLines JSON format.
     """
 
@@ -282,15 +283,15 @@
         :type output: str
         :param mode: the file mode to use
         :type mode: str
         """
         with open(output, mode) as fp:
             writer = jsonlines.Writer(fp)
             for item in data:
-                d = {self.att_content: item.content}
+                d = {self.att_content: empty_str_if_none(item.content)}
                 if self.att_id is not None:
                     if (item.meta is not None) and ("id" in item.meta):
                         d[self.att_id] = item.meta["id"]
                 try:
                     writer.write(d)
                 except KeyboardInterrupt as e:
                     raise e
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/pretrain/_max_length.py` & `llm-dataset-converter-0.2.1/src/ldc/pretrain/_max_length.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/pretrain/_parquet.py` & `llm-dataset-converter-0.2.1/src/ldc/pretrain/_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import generate_output
 from ldc.api.pretrain import PretrainData, PretrainReader, BatchPretrainWriter
+from ldc.text_utils import empty_str_if_none
 
 
 class ParquetPretrainReader(PretrainReader):
     """
     Reader for Parquet database files.
     """
 
@@ -255,15 +256,15 @@
             self.finalize()
             self._current_output = generate_output(self.session.current_input, self.target, ".parquet", self.session.options.compression)
             self.logger().info("Writing to: " + self._current_output)
             # create dictionary
             d_content = []
             d_ids = []
             for row in data:
-                d_content.append(row.content)
+                d_content.append(empty_str_if_none(row.content))
                 if self.col_id is not None:
                     if (row.meta is not None) and ("id" in row.meta):
                         d_ids.append(row.meta["id"])
                     else:
                         d_ids.append(None)
             d = dict()
             if self.col_content is not None:
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/pretrain/_sentences.py` & `llm-dataset-converter-0.2.1/src/ldc/pretrain/_sentences.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/pretrain/_split.py` & `llm-dataset-converter-0.2.1/src/ldc/pretrain/_split.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/pretrain/_txt.py` & `llm-dataset-converter-0.2.1/src/ldc/pretrain/_txt.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix, DEFAULT_END_CHARS, DEFAULT_QUOTE_CHARS
 from ldc.api import open_file, generate_output, is_compressed
 from ldc.api.pretrain import PretrainData, PretrainReader, StreamPretrainWriter
 from ldc.text_utils import assemble_preformatted, split_into_sentences, combine_sentences, remove_empty, \
-    remove_patterns, remove_blocks
+    remove_patterns, remove_blocks, empty_str_if_none
 
 METADATA_LINE = "line"
 
 
 class TxtPretrainReader(PretrainReader):
     """
     Reader for plain text files.
@@ -420,15 +420,15 @@
                     except:
                         fname = str(d.meta["id"]) + ".txt"
                 else:
                     fname = self._fname_format % self.session.count
                 output = generate_output(fname, self.target, ".txt", self.session.options.compression)
                 self.logger().info("Writing to: %s" % output)
                 with open(output, "w") as fp:
-                    fp.write(d.content)
+                    fp.write(empty_str_if_none(d.content))
 
     def finalize(self):
         """
         Finishes the processing, e.g., for closing files or databases.
         """
         super().finalize()
         if len(self._buffer) > 0:
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/registry.py` & `llm-dataset-converter-0.2.1/src/ldc/registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,46 @@
 import argparse
 import logging
 import os
 import traceback
 
 from typing import Dict, List, Optional
 
-from seppl import Registry, Plugin, MODE_DYNAMIC, get_class_name
-from ldc.api._downloader import Downloader
-from seppl.io import Filter, Reader, Writer
-
-# the entry points defined in setup.py
-ENTRY_POINT_DOWNLOADERS = "ldc.downloaders"
-ENTRY_POINT_READERS = "ldc.readers"
-ENTRY_POINT_FILTERS = "ldc.filters"
-ENTRY_POINT_WRITERS = "ldc.writers"
-
-# environment variable with comma-separated list of modules to inspect for readers, filters, writers
-ENV_LDC_MODULES = "LDC_MODULES"
-
-# environment variable with comma-separated list of modules to exclude from inspection of readers, filters, writers
-ENV_LDC_MODULES_EXCL = "LDC_MODULES_EXCL"
-
-# the default modules to inspect (for development)
-# can be overridden with LDC_MODULES environment variable
-DEFAULT_LDC_MODULES = ",".join([
-    "ldc.downloader",
-    "ldc.filter",
-    "ldc.pretrain",
-    "ldc.supervised.classification",
-    "ldc.supervised.pairs",
-    "ldc.translation",
-])
-
-REGISTRY = Registry(mode=MODE_DYNAMIC, default_modules=DEFAULT_LDC_MODULES,
-                    env_modules=ENV_LDC_MODULES, excluded_env_modules=ENV_LDC_MODULES_EXCL,
-                    enforce_uniqueness=True)
+from seppl import Plugin, get_class_name, ClassListerRegistry
 
 LLM_REGISTRY = "llm-registry"
 
 _logger = None
 
 
+# environment variable with comma-separated list of class listers
+ENV_LDC_CLASS_LISTERS = "LDC_CLASS_LISTERS"
+
+# environment variable with comma-separated list of class listers to exclude from using
+ENV_LDC_CLASS_LISTERS_EXCL = "LDC_CLASS_LISTERS_EXCL"
+
+DEFAULT_LDC_CLASSLISTERS = [
+    "ldc.class_lister"
+]
+
+REGISTRY = ClassListerRegistry(default_class_listers=DEFAULT_LDC_CLASSLISTERS,
+                               env_class_listers=ENV_LDC_CLASS_LISTERS,
+                               env_excluded_class_listers=ENV_LDC_CLASS_LISTERS_EXCL)
+
 LIST_PLUGINS = "plugins"
 LIST_DOWNLOADERS = "downloaders"
 LIST_READERS = "readers"
 LIST_FILTERS = "filters"
 LIST_WRITERS = "writers"
-LIST_CUSTOM_MODULES = "custom-modules"
-LIST_ENV_MODULES = "env-modules"
+LIST_CUSTOM_CLASS_LISTERS = "custom-class-listers"
+LIST_ENV_CLASS_LISTERS = "env-class-listers"
 LIST_TYPES = [
     LIST_PLUGINS,
-    LIST_CUSTOM_MODULES,
-    LIST_ENV_MODULES,
+    LIST_CUSTOM_CLASS_LISTERS,
+    LIST_ENV_CLASS_LISTERS,
     LIST_DOWNLOADERS,
     LIST_READERS,
     LIST_FILTERS,
     LIST_WRITERS,
 ]
 
 
@@ -75,45 +60,45 @@
 def available_downloaders() -> Dict[str, Plugin]:
     """
     Returns all available downloaders.
 
     :return: the dict of downloader objects
     :rtype: dict
     """
-    return REGISTRY.plugins(ENTRY_POINT_DOWNLOADERS, Downloader)
+    return REGISTRY.plugins("ldc.api.Downloader", fail_if_empty=False)
 
 
 def available_readers() -> Dict[str, Plugin]:
     """
     Returns all available readers.
 
     :return: the dict of reader objects
     :rtype: dict
     """
-    return REGISTRY.plugins(ENTRY_POINT_READERS, Reader)
+    return REGISTRY.plugins("ldc.api.Reader", fail_if_empty=False)
 
 
 def available_writers() -> Dict[str, Plugin]:
     """
     Returns all available writers.
 
     :return: the dict of writer objects
     :rtype: dict
     """
-    return REGISTRY.plugins(ENTRY_POINT_WRITERS, Writer)
+    return REGISTRY.plugins("seppl.io.Writer", fail_if_empty=False)
 
 
 def available_filters() -> Dict[str, Plugin]:
     """
     Returns all available filters.
 
     :return: the dict of filter objects
     :rtype: dict
     """
-    return REGISTRY.plugins(ENTRY_POINT_FILTERS, Filter)
+    return REGISTRY.plugins("ldc.api.Filter", fail_if_empty=False)
 
 
 def available_plugins() -> Dict[str, Plugin]:
     """
     Returns all available plugins.
 
     :return: the dict of plugin objects
@@ -123,36 +108,40 @@
     result.update(available_downloaders())
     result.update(available_readers())
     result.update(available_filters())
     result.update(available_writers())
     return result
 
 
-def register_plugins(modules: List[str] = None, excluded_modules: List[str] = None):
+def register_plugins(custom_class_listers: List[str] = None, excluded_class_listers: List[str] = None):
     """
     Registers all plugins.
 
-    :param modules: the list of modules to use instead of env variable or default modules
-    :type modules: list
-    :param excluded_modules: the list of modules to exclude
-    :type excluded_modules: list
+    :param custom_class_listers: the list of custom class listers to use instead of env variable or default class listers
+    :type custom_class_listers: list
+    :param excluded_class_listers: the list of class listers to exclude
+    :type excluded_class_listers: list
     """
-    REGISTRY.custom_modules = modules
-    REGISTRY.excluded_modules = excluded_modules
+    REGISTRY.custom_class_listers = custom_class_listers
+    REGISTRY.excluded_class_listers = excluded_class_listers
     available_plugins()
 
 
-def _list(list_type: str, custom_modules: Optional[List[str]] = None, excluded_modules: Optional[List[str]] = None):
+def _list(list_type: str, custom_class_listers: Optional[List[str]] = None, excluded_class_listers: Optional[List[str]] = None):
     """
     Lists various things on stdout.
 
     :param list_type: the type of list to generate
     :type list_type: str
+    :param custom_class_listers: the list of class listers to use instead of env variable or default class listers
+    :type custom_class_listers: list
+    :param excluded_class_listers: the list of class listers to exclude
+    :type excluded_class_listers: list
     """
-    register_plugins(modules=custom_modules, excluded_modules=excluded_modules)
+    register_plugins(custom_class_listers=custom_class_listers, excluded_class_listers=excluded_class_listers)
 
     if list_type in [LIST_PLUGINS, LIST_DOWNLOADERS, LIST_READERS, LIST_FILTERS, LIST_WRITERS]:
         if list_type == LIST_PLUGINS:
             plugins = available_plugins()
         elif list_type == LIST_DOWNLOADERS:
             plugins = available_downloaders()
         elif list_type == LIST_READERS:
@@ -162,58 +151,58 @@
         elif list_type == LIST_WRITERS:
             plugins = available_readers()
         else:
             raise Exception("Unhandled type: %s" % list_type)
         print("name: class")
         for name in plugins:
             print("%s: %s" % (name, get_class_name(plugins[name])))
-    elif list_type == LIST_CUSTOM_MODULES:
-        modules = REGISTRY.custom_modules
-        print("custom modules:")
-        if modules is None:
+    elif list_type == LIST_CUSTOM_CLASS_LISTERS:
+        class_listers = REGISTRY.custom_class_listers
+        print("custom class listers:")
+        if class_listers is None:
             print("-none")
         else:
-            for m in modules:
+            for m in class_listers:
                 print(m)
-    elif list_type == LIST_ENV_MODULES:
-        print("env modules:")
-        if REGISTRY.env_modules is None:
+    elif list_type == LIST_ENV_CLASS_LISTERS:
+        print("env class listers:")
+        if REGISTRY.env_class_listers is None:
             print("-none-")
         else:
-            modules = os.getenv(REGISTRY.env_modules)
-            if modules is None:
-                print("-none listed in env var %s-" % REGISTRY.env_modules)
+            class_listers = os.getenv(REGISTRY.env_class_listers)
+            if class_listers is None:
+                print("-none listed in env var %s-" % REGISTRY.env_class_listers)
             else:
-                modules = modules.split(",")
-                for m in modules:
+                class_listers = class_listers.split(",")
+                for m in class_listers:
                     print(m)
 
 
 def main(args=None):
     """
     The main method for parsing command-line arguments.
 
     :param args: the commandline arguments, uses sys.argv if not supplied
     :type args: list
     """
     parser = argparse.ArgumentParser(
         description="For inspecting/querying the registry.",
         prog=LLM_REGISTRY,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument("-m", "--custom_modules", type=str, default=None, help="The comma-separated list of custom modules to use.", required=False)
-    parser.add_argument("-e", "--excluded_modules", type=str, default=None, help="The comma-separated list of modules to excluded.", required=False)
+    parser.add_argument("-c", "--custom_class_listers", type=str, default=None, help="The comma-separated list of custom class listers to use.", required=False)
+    parser.add_argument("-e", "--excluded_class_listers", type=str, default=None, help="The comma-separated list of class listers to excluded.", required=False)
     parser.add_argument("-l", "--list", choices=LIST_TYPES, default=None, help="For outputting various lists on stdout.", required=False)
     parsed = parser.parse_args(args=args)
 
-    custom_modules = None
-    if parsed.custom_modules is not None:
-        custom_modules = parsed.custom_modules.split(",")
+    custom_class_listers = None
+    if parsed.custom_class_listers is not None:
+        custom_class_listers = parsed.custom_class_listers.split(",")
 
     if parsed.list is not None:
-        _list(parsed.list, custom_modules=custom_modules)
+        _list(parsed.list, custom_class_listers=custom_class_listers)
 
 
 def sys_main() -> int:
     """
     Runs the main function using the system cli arguments, and
     returns a system error code.
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/supervised/classification/_classification_label_map.py` & `llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_classification_label_map.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/supervised/classification/_csv.py` & `llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import open_file, generate_output
 from ldc.api.supervised.classification import ClassificationData, ClassificationReader, BatchClassificationWriter
 from ldc.utils import str_to_column_index
+from ldc.text_utils import empty_str_if_none
 
 
 class AbstractCsvLikeClassificationReader(ClassificationReader, abc.ABC):
     """
     Ancestor for readers of CSV-like files.
     """
 
@@ -360,20 +361,20 @@
             row = []
             if self.col_id is not None:
                 if (item.meta is not None) and ("id" in item.meta):
                     row.append(item.meta["id"])
                 else:
                     row.append(None)
             if self.no_header:
-                row.extend([item.text, item.label])
+                row.extend([empty_str_if_none(item.text), empty_str_if_none(item.label)])
             else:
                 if self.col_text is not None:
-                    row.append(item.text)
+                    row.append(empty_str_if_none(item.text))
                 if self.col_label is not None:
-                    row.append(item.label)
+                    row.append(empty_str_if_none(item.label))
             try:
                 self._output_writer.writerow(row)
             except:
                 print("Failed to write row: %s" % str(row), file=sys.stderr)
                 traceback.print_exc()
 
     def finalize(self):
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/supervised/classification/_jsonlines.py` & `llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_jsonlines.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import open_file, generate_output, is_compressed
 from ldc.api.supervised.classification import ClassificationData, ClassificationReader, StreamClassificationWriter
+from ldc.text_utils import empty_str_if_none
 
 
 class JsonLinesClassificationReader(ClassificationReader):
     """
     Reader for the JsonLines JSON format.
     """
 
@@ -300,17 +301,17 @@
         :type mode: str
         """
         with open(output, mode) as fp:
             writer = jsonlines.Writer(fp)
             for item in data:
                 d = dict()
                 if self.att_text is not None:
-                    d[self.att_text] = item.text
+                    d[self.att_text] = empty_str_if_none(item.text)
                 if self.att_label is not None:
-                    d[self.att_label] = item.label
+                    d[self.att_label] = empty_str_if_none(item.label)
                 if self.att_id is not None:
                     if (item.meta is not None) and ("id" in item.meta):
                         d[self.att_id] = item.meta["id"]
                 try:
                     writer.write(d)
                 except KeyboardInterrupt as e:
                     raise e
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/supervised/classification/_parquet.py` & `llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import generate_output
 from ldc.api.supervised.classification import ClassificationData, ClassificationReader, BatchClassificationWriter
+from ldc.text_utils import empty_str_if_none
 
 
 class ParquetClassificationReader(ClassificationReader):
     """
     Reader for Parquet database files.
     """
 
@@ -272,16 +273,16 @@
             self._current_output = generate_output(self.session.current_input, self.target, ".parquet", self.session.options.compression)
             self.logger().info("Writing to: " + self._current_output)
             # create dictionary
             d_text = []
             d_label = []
             d_ids = []
             for row in data:
-                d_text.append(row.text)
-                d_label.append(row.label)
+                d_text.append(empty_str_if_none(row.text))
+                d_label.append(empty_str_if_none(row.label))
                 if self.col_id is not None:
                     if (row.meta is not None) and ("id" in row.meta):
                         d_ids.append(row.meta["id"])
                     else:
                         d_ids.append(None)
             d = dict()
             if self.col_text is not None:
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_alpaca.py` & `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_alpaca.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_csv.py` & `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import open_file, generate_output
 from ldc.api.supervised.pairs import PairData, PairReader, BatchPairWriter
 from ldc.utils import str_to_column_index
+from ldc.text_utils import empty_str_if_none
 
 
 class AbstractCsvLikePairsReader(PairReader, abc.ABC):
     """
     Ancestor for readers of CSV-like files.
     """
 
@@ -380,22 +381,22 @@
             row = []
             if self.col_id is not None:
                 if (item.meta is not None) and ("id" in item.meta):
                     row.append(item.meta["id"])
                 else:
                     row.append(None)
             if self.no_header:
-                row.extend([item.instruction, item.input, item.output])
+                row.extend([empty_str_if_none(item.instruction), empty_str_if_none(item.input), empty_str_if_none(item.output)])
             else:
                 if self.col_instruction is not None:
-                    row.append(item.instruction)
+                    row.append(empty_str_if_none(item.instruction))
                 if self.col_input is not None:
-                    row.append(item.input)
+                    row.append(empty_str_if_none(item.input))
                 if self.col_output is not None:
-                    row.append(item.output)
+                    row.append(empty_str_if_none(item.output))
             try:
                 self._output_writer.writerow(row)
             except:
                 print("Failed to write row: %s" % str(row), file=sys.stderr)
                 traceback.print_exc()
 
     def finalize(self):
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_jsonlines.py` & `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_jsonlines.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import open_file, generate_output, is_compressed
 from ldc.api.supervised.pairs import PairData, PairReader, StreamPairWriter
+from ldc.text_utils import empty_str_if_none
 
 
 class JsonLinesPairReader(PairReader):
     """
     Reader for the JsonLines JSON format.
     """
 
@@ -314,19 +315,19 @@
         :type mode: str
         """
         with open(output, mode) as fp:
             writer = jsonlines.Writer(fp)
             for item in data:
                 d = dict()
                 if self.att_instruction is not None:
-                    d[self.att_instruction] = item.instruction
+                    d[self.att_instruction] = empty_str_if_none(item.instruction)
                 if self.att_input is not None:
-                    d[self.att_input] = item.input
+                    d[self.att_input] = empty_str_if_none(item.input)
                 if self.att_output is not None:
-                    d[self.att_output] = item.output
+                    d[self.att_output] = empty_str_if_none(item.output)
                 if self.att_id is not None:
                     if (item.meta is not None) and ("id" in item.meta):
                         d[self.att_id] = item.meta["id"]
                 try:
                     writer.write(d)
                 except KeyboardInterrupt as e:
                     raise e
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_parquet.py` & `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import generate_output
 from ldc.api.supervised.pairs import PairData, PairReader, BatchPairWriter
+from ldc.text_utils import empty_str_if_none
 
 
 class ParquetPairsReader(PairReader):
     """
     Reader for Parquet database files.
     """
 
@@ -287,17 +288,17 @@
             self.logger().info("Writing to: " + self._current_output)
             # create dictionary
             d_instruction = []
             d_input = []
             d_output = []
             d_ids = []
             for row in data:
-                d_instruction.append(row.instruction)
-                d_input.append(row.input)
-                d_output.append(row.output)
+                d_instruction.append(empty_str_if_none(row.instruction))
+                d_input.append(empty_str_if_none(row.input))
+                d_output.append(empty_str_if_none(row.output))
                 if self.col_id is not None:
                     if (row.meta is not None) and ("id" in row.meta):
                         d_ids.append(row.meta["id"])
                     else:
                         d_ids.append(None)
             d = dict()
             if self.col_instruction is not None:
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_update_pair_data.py` & `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_update_pair_data.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/supervised/pairs/_xtuner.py` & `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_xtuner.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/text_utils.py` & `llm-dataset-converter-0.2.1/src/ldc/text_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import copy
 import re
 import string
-from typing import List, Tuple
+from typing import List, Tuple, Optional, Dict, Union
 
 from ldc.core import DEFAULT_END_CHARS, DEFAULT_QUOTE_CHARS
 
 
 def prune_lines(lines: List[str], min_len: int = 1) -> List[str]:
     """
     Removes lines that only consist of too few characters.
@@ -319,7 +320,58 @@
             new_line = re.sub(f, replace[n], new_line)
         if lines[i] != new_line:
             result.append(new_line)
             affected += 1
         else:
             result.append(lines[i])
     return result, affected
+
+
+def empty_str_if_none(s: Union[Optional[str], List[str], Dict[str, str]]) -> Union[str, List[str], Dict[str, str]]:
+    """
+    If the provided string or values in the list/dict are None, the function will
+    update them with an empty string (returns new object, does not modify inpyt).
+
+    :param s: the string/list/dict to check
+    :type s: str
+    :return: the processed string/list/dict
+    :rtype: str or list or dict
+    """
+    if s is None:
+        return ""
+
+    result = s
+
+    if isinstance(s, str):
+        return s
+
+    elif isinstance(s, list):
+        update = False
+        for item in s:
+            if item is None:
+                update = True
+                break
+        if update:
+            result = list()
+            for item in s:
+                if item is None:
+                    result.append("")
+                else:
+                    result.append(item)
+
+    elif isinstance(s, dict):
+        update = False
+        for k in s:
+            if s[k] is None:
+                update = True
+                break
+        if update:
+            result = dict()
+            for k in s:
+                if s[k] is None:
+                    result[k] = ""
+                else:
+                    result[k] = s[k]
+            return result
+    else:
+        raise Exception("Must be either string, list or dict: %s" % str(type(s)))
+    return result
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/tool/append.py` & `llm-dataset-converter-0.2.1/src/ldc/tool/append.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/tool/convert.py` & `llm-dataset-converter-0.2.1/src/ldc/tool/convert.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/tool/download.py` & `llm-dataset-converter-0.2.1/src/ldc/tool/download.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/tool/file_encoding.py` & `llm-dataset-converter-0.2.1/src/ldc/tool/file_encoding.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/tool/find.py` & `llm-dataset-converter-0.2.1/src/ldc/tool/find.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/tool/help.py` & `llm-dataset-converter-0.2.1/src/ldc/tool/help.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,35 +43,35 @@
         for name in plugin_names:
             lines.append("- %s" % name)
         lines.append("")
     else:
         raise Exception("Unsupported format for index: %s" % help_format)
 
 
-def output_help(modules: List[str] = None, excluded_modules: Optional[List[str]] = None, plugin_name: str = None,
+def output_help(custom_class_listers: List[str] = None, excluded_class_listers: Optional[List[str]] = None, plugin_name: str = None,
                 help_format: str = HELP_FORMAT_TEXT, heading_level: int = 1, output: str = None, index: str = None):
     """
     Generates and outputs the help screen for the plugin.
 
-    :param modules: the modules to generate the entry points for
-    :type modules: list
-    :param excluded_modules: the list of modules to exclude
-    :type excluded_modules: list
+    :param custom_class_listers: the class listers to use
+    :type custom_class_listers: list
+    :param excluded_class_listers: the list of class listers to exclude
+    :type excluded_class_listers: list
     :param plugin_name: the plugin to generate the help for, None if for all
     :type plugin_name: str
     :param help_format: the format to output
     :type help_format: str
     :param heading_level: the heading level to use (markdown)
     :type heading_level: int
     :param output: the dir/file to save the output to, uses stdout if None
     :type output: str
     :param index: the index file to generate in the output directory, ignored if None
     :type index: str
     """
-    register_plugins(modules=modules, excluded_modules=excluded_modules)
+    register_plugins(custom_class_listers=custom_class_listers, excluded_class_listers=excluded_class_listers)
     if help_format not in HELP_FORMATS:
         raise Exception("Unknown help format: %s" % help_format)
     if (plugin_name is None) and ((output is None) or (not os.path.isdir(output))):
         raise Exception("When generating the help for all plugins, the output must be a directory: %s" % output)
     if plugin_name is None:
         plugin_names = available_plugins().keys()
     else:
@@ -115,25 +115,25 @@
     :type args: list
     """
     init_logging(env_var=ENV_LLM_LOGLEVEL)
     parser = argparse.ArgumentParser(
         description="Tool for outputting help for plugins in various formats.",
         prog=HELP,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument("-m", "--modules", metavar="PACKAGE", help="The names of the module packages, uses the default ones if not provided.", default=None, type=str, required=False, nargs="*")
-    parser.add_argument("-e", "--excluded_modules", type=str, default=None, help="The comma-separated list of modules to excluded.", required=False)
+    parser.add_argument("-c", "--custom_class_listers", metavar="PACKAGE", help="The names of the custom class listers, uses the default ones if not provided.", default=None, type=str, required=False, nargs="*")
+    parser.add_argument("-e", "--excluded_class_listers", type=str, default=None, help="The comma-separated list of class listers to excluded.", required=False)
     parser.add_argument("-p", "--plugin_name", metavar="NAME", help="The name of the plugin to generate the help for, generates it for all if not specified", default=None, type=str, required=False)
     parser.add_argument("-f", "--help_format", metavar="FORMAT", help="The output format to generate", choices=HELP_FORMATS, default=HELP_FORMAT_TEXT, required=False)
     parser.add_argument("-L", "--heading_level", metavar="INT", help="The level to use for the heading", default=1, type=int, required=False)
     parser.add_argument("-o", "--output", metavar="PATH", help="The directory or file to store the help in; outputs it to stdout if not supplied; if pointing to a directory, automatically generates file name from plugin name and help format", type=str, default=None, required=False)
     parser.add_argument("-i", "--index", metavar="FILE", help="The file in the output directory to generate with an overview of all plugins, grouped by type (in markdown format, links them to the other generated files)", type=str, default=None, required=False)
     add_logging_level(parser)
     parsed = parser.parse_args(args=args)
     set_logging_level(_logger, parsed.logging_level)
-    output_help(modules=parsed.modules, excluded_modules=parsed.excluded_modules,
+    output_help(custom_class_listers=parsed.custom_class_listers, excluded_class_listers=parsed.excluded_class_listers,
                 plugin_name=parsed.plugin_name, help_format=parsed.help_format,
                 heading_level=parsed.heading_level, output=parsed.output,
                 index=parsed.index)
 
 
 def sys_main() -> int:
     """
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/tool/paste.py` & `llm-dataset-converter-0.2.1/src/ldc/tool/paste.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/translation/_csv.py` & `llm-dataset-converter-0.2.1/src/ldc/translation/_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import open_file, generate_output
 from ldc.api.translation import TranslationData, TranslationReader, BatchTranslationWriter
 from ldc.utils import str_to_column_index
+from ldc.text_utils import empty_str_if_none
 
 
 class AbstractCsvLikeTranslationReader(TranslationReader, abc.ABC):
     """
     Ancestor for readers of CSV-like files.
     """
 
@@ -342,15 +343,15 @@
             if not self.no_col_id:
                 if (item.meta is not None) and ("id" in item.meta):
                     row.append(item.meta["id"])
                 else:
                     row.append(None)
             for lang in self.languages:
                 if lang in item.translations:
-                    row.append(item.translations[lang])
+                    row.append(empty_str_if_none(item.translations[lang]))
                 else:
                     row.append(None)
             try:
                 self._output_writer.writerow(row)
             except:
                 print("Failed to write row: %s" % str(row), file=sys.stderr)
                 traceback.print_exc()
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/translation/_jsonlines.py` & `llm-dataset-converter-0.2.1/src/ldc/translation/_jsonlines.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import open_file, generate_output, is_compressed
 from ldc.api.translation import TranslationData, TranslationReader, StreamTranslationWriter
+from ldc.text_utils import empty_str_if_none
 
 DATA_EXAMPLE = '{ "translation": { "en": "Others have dismissed him as a joke.", "ro": "Alții l-au numit o glumă." } }'
 DATA_DEFINITION_URL = "https://github.com/huggingface/transformers/blob/main/examples/pytorch/translation/README.md"
 
 
 class JsonLinesTranslationReader(TranslationReader):
     """
@@ -252,15 +253,15 @@
         :type output: str
         :param mode: the file mode to use
         :type mode: str
         """
         with open(output, mode) as fp:
             writer = jsonlines.Writer(fp)
             for item in data:
-                d = {"translation": item.translations}
+                d = {"translation": empty_str_if_none(item.translations)}
                 try:
                     writer.write(d)
                 except KeyboardInterrupt as e:
                     raise e
                 except:
                     self.logger().exception("Failed to write record: %s" % str(d))
             writer.close()
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/translation/_language.py` & `llm-dataset-converter-0.2.1/src/ldc/translation/_language.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/translation/_parquet.py` & `llm-dataset-converter-0.2.1/src/ldc/translation/_parquet.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import generate_output
 from ldc.api.translation import TranslationData, TranslationReader, BatchTranslationWriter
+from ldc.text_utils import empty_str_if_none
 
 DATA_EXAMPLE = '{ "en": "Others have dismissed him as a joke.", "ro": "Alții l-au numit o glumă." }'
 
 
 class ParquetTranslationReader(TranslationReader):
     """
     Reader for Parquet database files.
@@ -260,15 +261,15 @@
             self.finalize()
             self._current_output = generate_output(self.session.current_input, self.target, ".parquet", self.session.options.compression)
             self.logger().info("Writing to: " + self._current_output)
             # create dictionary
             d_content = []
             d_ids = []
             for row in data:
-                d_content.append(json.dumps(row.translations, ensure_ascii=False))
+                d_content.append(json.dumps(empty_str_if_none(row.translations), ensure_ascii=False))
                 if self.col_id is not None:
                     if (row.meta is not None) and ("id" in row.meta):
                         d_ids.append(row.meta["id"])
                     else:
                         d_ids.append(None)
             d = dict()
             if self.col_content is not None:
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/translation/_require_languages.py` & `llm-dataset-converter-0.2.1/src/ldc/translation/_require_languages.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/ldc/translation/_txt.py` & `llm-dataset-converter-0.2.1/src/ldc/translation/_txt.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from wai.logging import LOGGING_WARNING
 from seppl import add_metadata
 from seppl.io import locate_files
 from ldc.core import domain_suffix
 from ldc.api import open_file, generate_output, is_compressed
 from ldc.api.translation import TranslationData, TranslationReader, StreamTranslationWriter
 from ldc.utils import str_to_column_index
+from ldc.text_utils import empty_str_if_none
 
 
 PH_TAB = "{TAB}"
 """ placeholder for tab. """
 
 PH_LANG = "{LANG}"
 """ placeholder for the language. """
@@ -337,15 +338,15 @@
         :param data: the translation data to write
         :type data: TranslationData
         """
         for lang in data.translations.keys():
             line = self.line_format
             line = line.replace(PH_LANG, lang)
             line = line.replace(PH_ID, str(id))
-            line = line.replace(PH_CONTENT, data.translations[lang])
+            line = line.replace(PH_CONTENT, empty_str_if_none(data.translations[lang]))
             fp.write(line)
             fp.write("\n")
 
     def _get_id(self, data: TranslationData) -> Union[str, int]:
         """
         Returns the ID for the record.
```

### Comparing `llm-dataset-converter-0.2.0/src/ldc/utils.py` & `llm-dataset-converter-0.2.1/src/ldc/utils.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.0/src/llm_dataset_converter.egg-info/PKG-INFO` & `llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: llm-dataset-converter
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python3 library for converting between various LLM dataset formats.
 Home-page: https://github.com/waikato-llm/llm-dataset-converter
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: The **llm-dataset-converter** allows the conversion between
         various dataset formats for large language models (LLMs).
@@ -63,14 +63,25 @@
                 --output alpaca_data_cleaned-filtered.json
         
         
         
         Changelog
         =========
         
+        0.2.1 (2024-05-02)
+        ------------------
+        
+        - filters `split` and `tee` now support `ClassificationData` as well
+        - added `metadata-from-name` filter to extract meta-data from the current input file name
+        - requiring seppl>=0.1.3 now
+        - added `inspect` filter that allows inspecting data interactively as it passes through the pipeline
+        - added `empty_str_if_none` helper method to `ldc.text_utils` to ensure no None/null values are output with writers
+        - upgraded seppl to 0.2.2 and switched to using `seppl.ClassListerRegistry`
+        
+        
         0.2.0 (2024-02-27)
         ------------------
         
         - added support for XTuner conversation JSON format: `from-xtuner` and `to-xtuner`
         - added filter `update-pair-data` to allow tweaking or rearranging of the data
         - introduced `ldc.api` module to separate out abstract superclasses and avoid circular imports
         - readers now set the 'file' meta-data value
```

### Comparing `llm-dataset-converter-0.2.0/src/llm_dataset_converter.egg-info/SOURCES.txt` & `llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 CHANGES.rst
 DESCRIPTION.rst
 MANIFEST.in
 README.md
 setup.py
 src/ldc/__init__.py
+src/ldc/class_lister.py
 src/ldc/core.py
 src/ldc/help.py
 src/ldc/registry.py
 src/ldc/text_utils.py
 src/ldc/utils.py
 src/ldc/api/__init__.py
 src/ldc/api/_downloader.py
@@ -21,18 +22,20 @@
 src/ldc/downloader/__init__.py
 src/ldc/downloader/_huggingface.py
 src/ldc/filter/__init__.py
 src/ldc/filter/_assemble_sentences.py
 src/ldc/filter/_change_case.py
 src/ldc/filter/_file_filter.py
 src/ldc/filter/_find_substr.py
+src/ldc/filter/_inspect.py
 src/ldc/filter/_keyword.py
 src/ldc/filter/_llama2_to_pairs.py
 src/ldc/filter/_max_records.py
 src/ldc/filter/_metadata.py
+src/ldc/filter/_metadata_from_name.py
 src/ldc/filter/_pairs_to_llama2.py
 src/ldc/filter/_pairs_to_pretrain.py
 src/ldc/filter/_pretrain_sentences_to_classification.py
 src/ldc/filter/_pretrain_sentences_to_pairs.py
 src/ldc/filter/_randomize_records.py
 src/ldc/filter/_record_files.py
 src/ldc/filter/_record_window.py
```

