# Comparing `tmp/openparse-0.5.5.tar.gz` & `tmp/openparse-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openparse-0.5.5.tar", last modified: Sun Apr 28 17:39:34 2024, max compression
+gzip compressed data, was "openparse-0.5.6.tar", last modified: Thu May  2 00:35:24 2024, max compression
```

## Comparing `openparse-0.5.5.tar` & `openparse-0.5.6.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-28 17:39:30.000000 openparse-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-28 17:39:34.749753 openparse-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-28 17:39:30.000000 openparse-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-28 17:39:30.000000 openparse-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 17:39:34.749753 openparse-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.737753 openparse-0.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.737753 openparse-0.5.5/src/evals/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:39:30.000000 openparse-0.5.5/src/evals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-28 17:39:30.000000 openparse-0.5.5/src/evals/run_evals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.741752 openparse-0.5.5/src/openparse/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/doc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.741752 openparse-0.5.5/src/openparse/processing/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/processing/basic_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/processing/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/processing/semantic_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.741752 openparse-0.5.5/src/openparse/tables/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.741752 openparse-0.5.5/src/openparse/tables/pymupdf/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/pymupdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/pymupdf/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/openparse/tables/table_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/table_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/table_transformers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/table_transformers/ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/table_transformers/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/openparse/tables/unitable/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/tabular_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/unitable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/openparse/text/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/openparse/text/pdfminer/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/pdfminer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/pdfminer/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/openparse/text/pymupdf/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/pymupdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/pymupdf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/openparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/processing/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/processing/test_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/tables/pymupdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/pymupdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/pymupdf/test_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/tables/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/transformers/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/transformers/test_ml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/tables/unitable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/unitable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   190851 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/unitable/sample_pred_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/unitable/test_pred_to_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/test_doc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/test_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.737753 openparse-0.5.5/src/tests/text/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/text/pdf_miner/
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/text/pdf_miner/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.995381 openparse-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-02 00:35:15.000000 openparse-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-05-02 00:35:24.995381 openparse-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-05-02 00:35:15.000000 openparse-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-02 00:35:15.000000 openparse-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:35:24.995381 openparse-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.979381 openparse-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.983381 openparse-0.5.6/src/evals/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:35:15.000000 openparse-0.5.6/src/evals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-02 00:35:16.000000 openparse-0.5.6/src/evals/run_evals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.983381 openparse-0.5.6/src/openparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/doc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.983381 openparse-0.5.6/src/openparse/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/processing/basic_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/processing/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/processing/semantic_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.987381 openparse-0.5.6/src/openparse/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.987381 openparse-0.5.6/src/openparse/tables/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/pymupdf/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.987381 openparse-0.5.6/src/openparse/tables/table_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/table_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/table_transformers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/table_transformers/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/table_transformers/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.987381 openparse-0.5.6/src/openparse/tables/unitable/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/unitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/unitable/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/unitable/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/unitable/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/unitable/tabular_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/unitable/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/unitable/unitable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/unitable/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/tables/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.987381 openparse-0.5.6/src/openparse/text/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/text/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.987381 openparse-0.5.6/src/openparse/text/pdfminer/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/text/pdfminer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/text/pdfminer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.991381 openparse-0.5.6/src/openparse/text/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/text/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/text/pymupdf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-02 00:35:16.000000 openparse-0.5.6/src/openparse/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.991381 openparse-0.5.6/src/openparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-05-02 00:35:24.000000 openparse-0.5.6/src/openparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-02 00:35:24.000000 openparse-0.5.6/src/openparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:35:24.000000 openparse-0.5.6/src/openparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 00:35:24.000000 openparse-0.5.6/src/openparse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 00:35:24.000000 openparse-0.5.6/src/openparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 00:35:24.000000 openparse-0.5.6/src/openparse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.991381 openparse-0.5.6/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.991381 openparse-0.5.6/src/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/processing/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/processing/test_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.991381 openparse-0.5.6/src/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.991381 openparse-0.5.6/src/tests/tables/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/tables/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/tables/pymupdf/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.991381 openparse-0.5.6/src/tests/tables/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/tables/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/tables/transformers/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/tables/transformers/test_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.991381 openparse-0.5.6/src/tests/tables/unitable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/tables/unitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190851 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/tables/unitable/sample_pred_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/tables/unitable/test_pred_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/test_doc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/test_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.979381 openparse-0.5.6/src/tests/text/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:35:24.991381 openparse-0.5.6/src/tests/text/pdf_miner/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-02 00:35:16.000000 openparse-0.5.6/src/tests/text/pdf_miner/test_core.py
```

### Comparing `openparse-0.5.5/LICENSE` & `openparse-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/PKG-INFO` & `openparse-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.5.5
+Version: 0.5.6
 Summary: Streamlines the process of preparing documents for LLM's.
 Author-email: Sergey Filimonov <hello@sergey.fyi>
+License: MIT
 Project-URL: homepage, https://github.com/Filimoa/open-parse
 Project-URL: repository, https://github.com/Filimoa/open-parse
 Project-URL: documentation, https://filimoa.github.io/open-parse
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyMuPDF>=1.23.2
```

### Comparing `openparse-0.5.5/README.md` & `openparse-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/pyproject.toml` & `openparse-0.5.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
-requires = ["setuptools>=42", "wheel"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openparse"
 description = "Streamlines the process of preparing documents for LLM's."
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.5.5"
+license = { text = "MIT" }
+version = "0.5.6"
 authors = [{name = "Sergey Filimonov", email = "hello@sergey.fyi"}]
 dependencies = [
     "PyMuPDF >= 1.23.2",
     "pillow >= 8.3",
     "pydantic >= 2.0",
     "pypdf >= 4.0.0",
     "pdfminer.six >= 20200401",
```

### Comparing `openparse-0.5.5/src/evals/run_evals.py` & `openparse-0.5.6/src/evals/run_evals.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/__init__.py` & `openparse-0.5.6/src/openparse/__init__.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/_types.py` & `openparse-0.5.6/src/openparse/_types.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/cli.py` & `openparse-0.5.6/src/openparse/cli.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/config.py` & `openparse-0.5.6/src/openparse/config.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/doc_parser.py` & `openparse-0.5.6/src/openparse/doc_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,14 +113,18 @@
             nodes=nodes,
             filename=Path(file).name,
             num_pages=doc.num_pages,
             coordinate_system=consts.COORDINATE_SYSTEM,
             table_parsing_kwargs=(
                 table_args_obj.model_dump() if table_args_obj else None
             ),
+            creation_date=doc.file_metadata.get("creation_date"),
+            last_modified_date=doc.file_metadata.get("last_modified_date"),
+            last_accessed_date=doc.file_metadata.get("last_accessed_date"),
+            file_size=doc.file_metadata.get("file_size"),
         )
         return parsed_doc
 
     @staticmethod
     def _elems_to_nodes(
         elems: Union[List[TextElement], List[TableElement]],
     ) -> List[Node]:
```

### Comparing `openparse-0.5.5/src/openparse/pdf.py` & `openparse-0.5.6/src/openparse/pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import os
+import mimetypes
+import datetime as dt
 import random
 import io
 from pathlib import Path
-from typing import Iterator, List, Literal, Optional, Union, Tuple, Any
-
+from typing import Iterator, List, Literal, Optional, Union, Tuple, Any, Dict
 from pydantic import BaseModel
 from pdfminer.high_level import extract_pages
 from pdfminer.layout import LTPage
 from pypdf import PdfReader, PdfWriter
 
 from openparse.schemas import Bbox, Node
-from openparse import consts
 
 
 class _BboxWithColor(BaseModel):
     color: Tuple[float, float, float]
     bbox: Bbox
     annotation_text: Optional[Any] = None
 
@@ -56,21 +57,49 @@
                     )
                 )
 
                 text = f"continued ..."
     return res
 
 
+def file_metadata(file_path: Union[str, Path]) -> Dict:
+    """Get some handy metadate from filesystem.
+
+    Args:
+        file_path: str: file path in str
+    """
+    return {
+        "file_path": file_path,
+        "file_name": os.path.basename(file_path),
+        "file_type": mimetypes.guess_type(file_path)[0],
+        "file_size": os.path.getsize(file_path),
+        "creation_date": dt.datetime.fromtimestamp(
+            Path(file_path).stat().st_ctime
+        ).strftime("%Y-%m-%d"),
+        "last_modified_date": dt.datetime.fromtimestamp(
+            Path(file_path).stat().st_mtime
+        ).strftime("%Y-%m-%d"),
+        "last_accessed_date": dt.datetime.fromtimestamp(
+            Path(file_path).stat().st_atime
+        ).strftime("%Y-%m-%d"),
+    }
+
+
 class Pdf:
     """
     Simple utility class for working with PDF files. This class wraps the PdfReader and PdfWriter classes from pypdf.
     """
 
     def __init__(self, file: Union[str, Path, PdfReader]):
-        self.file_path = str(file) if isinstance(file, (str, Path)) else None
+        self.file_path = None
+        self.file_metadata = dict()
+        if isinstance(file, (str, Path)):
+            self.file_path = str(file)
+            self.file_metadata = file_metadata(file)
+
         self.reader = PdfReader(file) if isinstance(file, (str, Path)) else file
         self.writer = PdfWriter()
         for page in self.reader.pages:
             self.writer.add_page(page)
 
         self.num_pages = len(self.reader.pages)
 
@@ -103,18 +132,18 @@
         """
         Transforms the PDF into a PyMuPDF (fitz) document.
         If modifications have been made using PdfWriter, it saves to a temporary file first.
         This function dynamically imports PyMuPDF (fitz), requiring it only if this method is called.
         """
         try:
             import fitz  # type: ignore
-        except ImportError:
+        except ImportError as err:
             raise ImportError(
                 "PyMuPDF (fitz) is not installed. This method requires PyMuPDF."
-            )
+            ) from err
 
         if not self.writer.pages:
             return fitz.open(self.file_path)
 
         byte_stream = io.BytesIO()
         self.writer.write(byte_stream)
         return fitz.open(None, byte_stream)
@@ -122,18 +151,18 @@
     def _draw_bboxes(
         self,
         bboxes_with_color: List[_BboxWithColor],
         coordinates: Literal["top-left", "bottom-left"],
     ):
         try:
             import fitz
-        except ImportError:
+        except ImportError as err:
             raise ImportError(
                 "PyMuPDF (fitz) is not installed. This method requires PyMuPDF."
-            )
+            ) from err
 
         pdf = self.to_pymupdf_doc()
 
         for page in pdf:
             page.wrap_contents()
 
             for bbox_with_color in bboxes_with_color:
@@ -163,23 +192,23 @@
     ):
         """
         Display a single page of a PDF file using IPython.
         Optionally, display a piece of text on top of the bounding box.
         """
         try:
             from IPython.display import Image, display  # type: ignore
-        except ImportError:
+        except ImportError as err:
             raise ImportError(
                 "IPython is required to display PDFs. Please install it with `pip install ipython`."
-            )
+            ) from err
         assert nodes, "At least one node is required."
 
         bboxes = [node.bbox for node in nodes]
         flattened_bboxes = _prepare_bboxes_for_drawing(bboxes, annotations)
-        marked_up_doc = self._draw_bboxes(flattened_bboxes, nodes[0]._coordinates)
+        marked_up_doc = self._draw_bboxes(flattened_bboxes, nodes[0].coordinate_system)
         if not page_nums:
             page_nums = list(range(marked_up_doc.page_count))
         for page_num in page_nums:
             page = marked_up_doc[page_num]
             img_data = page.get_pixmap().tobytes("png")
             display(Image(data=img_data))
 
@@ -189,15 +218,15 @@
         output_pdf: Union[str, Path],
         annotations: Optional[List[str]] = None,
     ) -> None:
         assert nodes, "At least one node is required."
 
         bboxes = [node.bbox for node in nodes]
         flattened_bboxes = _prepare_bboxes_for_drawing(bboxes, annotations)
-        marked_up_doc = self._draw_bboxes(flattened_bboxes, nodes[0]._coordinates)
+        marked_up_doc = self._draw_bboxes(flattened_bboxes, nodes[0].coordinate_system)
         marked_up_doc.save(str(output_pdf))
 
     def _flip_coordinates(self, bbox: Bbox) -> Bbox:
         fy0 = bbox.page_height - bbox.y1
         fy1 = bbox.page_height - bbox.y0
         return Bbox(
             page=bbox.page,
```

### Comparing `openparse-0.5.5/src/openparse/processing/__init__.py` & `openparse-0.5.6/src/openparse/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/processing/basic_transforms.py` & `openparse-0.5.6/src/openparse/processing/basic_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,29 @@
 
         updated_nodes = []
         for node in nodes:
             if node.variant == {"table"}:
                 updated_nodes.append(node)
                 continue
 
-            new_elements = [
-                element
-                for element in node.elements
-                if not (
+            new_elements = []
+            for element in node.elements:
+                should_include = not (
                     isinstance(element, TextElement)
                     and self.intersects_any_table(
                         element.bbox, tables_by_page[element.page]
                     )
                 )
-            ]
-            if new_elements:
+                if should_include:
+                    new_elements.append(element)
+
+            if new_elements and len(new_elements) != len(node.elements):
                 updated_nodes.append(Node(elements=tuple(new_elements)))
+            elif len(new_elements) == len(node.elements):
+                updated_nodes.append(node)
 
         return updated_nodes
 
     def intersects_any_table(self, text_bbox: Bbox, table_bboxes: List[Bbox]) -> bool:
         return any(
             self.intersects(text_bbox, table_bbox) for table_bbox in table_bboxes
         )
```

### Comparing `openparse-0.5.5/src/openparse/processing/ingest.py` & `openparse-0.5.6/src/openparse/processing/ingest.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/processing/semantic_transforms.py` & `openparse-0.5.6/src/openparse/processing/semantic_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,18 +57,18 @@
             res.extend(batch_res)
 
         return res
 
     def _create_client(self):
         try:
             from openai import OpenAI
-        except ImportError:
+        except ImportError as err:
             raise ImportError(
                 "You need to install the openai package to use this feature."
-            )
+            ) from err
         return OpenAI(api_key=self.api_key)
 
 
 class CombineNodesSemantically(ProcessingStep):
     """
     Combines nodes that are semantically related.
     """
```

### Comparing `openparse-0.5.5/src/openparse/schemas.py` & `openparse-0.5.6/src/openparse/schemas.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 from collections import defaultdict, namedtuple
 from enum import Enum
+import datetime as dt
+import uuid
 from functools import cached_property
 from typing import Any, List, Literal, Optional, Tuple, Union, Set
 
 from pydantic import BaseModel, ConfigDict, computed_field, model_validator, Field
 
 from openparse import consts
 from openparse.utils import num_tokens
@@ -351,20 +353,39 @@
     elif vertical_distance <= paragraph_threshold:
         return "same-paragraph"
     else:
         return None
 
 
 class Node(BaseModel):
-    elements: Tuple[Union[TextElement, TableElement], ...] = Field(exclude=True)
-    _tokenization_lower_limit: int = consts.TOKENIZATION_LOWER_LIMIT
-    _tokenization_upper_limit: int = consts.TOKENIZATION_UPPER_LIMIT
-    _coordinates: Literal["top-left", "bottom-left"] = (
-        consts.COORDINATE_SYSTEM
+    id_: str = Field(
+        default_factory=lambda: str(uuid.uuid4()),
+        description="Unique ID of the node.",
+        exclude=True,
+    )
+    elements: Tuple[Union[TextElement, TableElement], ...] = Field(
+        exclude=True, frozen=True
+    )
+    tokenization_lower_limit: int = Field(
+        default=consts.TOKENIZATION_LOWER_LIMIT, frozen=True, exclude=True
+    )
+    tokenization_upper_limit: int = Field(
+        default=consts.TOKENIZATION_UPPER_LIMIT, frozen=True, exclude=True
+    )
+    coordinate_system: Literal["top-left", "bottom-left"] = Field(
+        default=consts.COORDINATE_SYSTEM, frozen=True, exclude=True
     )  # controlled globally for now, should be moved into elements
+    embedding: Optional[List[float]] = Field(
+        default=None, description="Embedding of the node."
+    )
+
+    @computed_field  # type: ignore
+    @cached_property
+    def node_id(self) -> str:
+        return self.id_
 
     @computed_field  # type: ignore
     @cached_property
     def variant(self) -> Set[Literal["text", "table"]]:
         return set(e.variant.value for e in self.elements)
 
     @computed_field  # type: ignore
@@ -460,19 +481,19 @@
 
     @cached_property
     def is_stub(self) -> bool:
         return self.tokens < 50
 
     @cached_property
     def is_small(self) -> bool:
-        return self.tokens < self._tokenization_lower_limit
+        return self.tokens < self.tokenization_lower_limit
 
     @cached_property
     def is_large(self) -> bool:
-        return self.tokens > self._tokenization_upper_limit
+        return self.tokens > self.tokenization_upper_limit
 
     @cached_property
     def num_pages(self) -> int:
         return len(set(element.bbox.page for element in self.elements))
 
     @cached_property
     def start_page(self) -> int:
@@ -490,15 +511,15 @@
         nodes = sorted(nodes, key=lambda x: x.reading_order)
 
         Returns a tuple of (min_page, y_position, min_x0) to use as sort keys, where y_position is adjusted based on the coordinate system.
         """
         min_page = min(element.bbox.page for element in self.elements)
         min_x0 = min(element.bbox.x0 for element in self.elements)
 
-        if self._coordinates == "bottom-left":
+        if self.coordinate_system == "bottom-left":
             y_position = -min(element.bbox.y0 for element in self.elements)
         else:
             raise NotImplementedError(
                 "Only 'bottom-left' coordinate system is supported."
             )
 
         return ReadingOrder(min_page=min_page, y_position=y_position, min_x0=min_x0)
@@ -523,19 +544,37 @@
                 )
 
                 if x_overlap and y_overlap:
                     return True
 
         return False
 
+    def to_llama_index(self):
+        try:
+            from llama_index.core.schema import TextNode as LlamaIndexTextNode
+        except ImportError as err:
+            raise ImportError(
+                "llama_index is not installed. Please install it with `pip install llama-index`."
+            ) from err
+        return LlamaIndexTextNode(
+            id_=self.id_,
+            text=self.text,
+            embedding=self.embedding,
+            metadata={"bbox": [b.model_dump(mode="json") for b in self.bbox]},
+            excluded_embed_metadata_keys=["bbox"],
+            excluded_llm_metadata_keys=["bbox"],
+        )
+
     def __lt__(self, other: "Node") -> bool:
         if not isinstance(other, Node):
             return NotImplemented
 
-        assert self._coordinates == other._coordinates, "Coordinate systems must match."
+        assert (
+            self.coordinate_system == other.coordinate_system
+        ), "Coordinate systems must match."
 
         return self.reading_order < other.reading_order
 
     def _repr_markdown_(self):
         """
         When called in a Jupyter environment, this will display the node as Markdown, which Jupyter will then render as HTML.
         """
@@ -548,21 +587,90 @@
         """
         if not isinstance(other, Node):
             return NotImplemented()
 
         new_elems = self.elements + other.elements
         return Node(elements=new_elems)
 
-    model_config = ConfigDict(frozen=True)
-
 
 #######################
 ### PARSED DOCUMENT ###
 #######################
 
 
 class ParsedDocument(BaseModel):
+    id_: str = Field(
+        default_factory=lambda: str(uuid.uuid4()),
+        description="Unique ID of the node.",
+        exclude=True,
+    )
     nodes: List[Node]
     filename: str
     num_pages: int
     coordinate_system: Literal["top-left", "bottom-left"] = "bottom-left"
     table_parsing_kwargs: Optional[dict] = None
+    last_modified_date: Optional[dt.date] = None
+    last_accessed_date: Optional[dt.date] = None
+    creation_date: Optional[dt.date] = None
+    file_size: Optional[int] = None
+
+    @cached_property
+    @computed_field
+    def doc_id(self) -> str:
+        return self.id_
+
+    def to_llama_index_nodes(self):
+        try:
+            from llama_index.core.schema import Document as LlamaIndexDocument
+        except ImportError as err:
+            raise ImportError(
+                "llama_index is not installed. Please install it with `pip install llama-index`."
+            ) from err
+
+        li_doc = LlamaIndexDocument(
+            id_=self.id_,
+            metadata={
+                "file_name": self.filename,
+                "file_size": self.file_size,
+                "creation_date": self.creation_date.isoformat(),
+                "last_modified_date": self.last_modified_date.isoformat(),
+            },
+            excluded_embed_metadata_keys=[
+                "file_size",
+                "creation_date",
+                "last_modified_date",
+            ],
+            excluded_llm_metadata_keys=[
+                "file_name",
+                "file_size",
+                "creation_date",
+                "last_modified_date",
+            ],
+        )
+        li_nodes = self._nodes_to_llama_index(li_doc)
+
+        return li_nodes
+
+    def _nodes_to_llama_index(self, llama_index_doc):
+        try:
+            from llama_index.core.schema import NodeRelationship
+        except ImportError as err:
+            raise ImportError(
+                "llama_index is not installed. Please install it with `pip install llama-index`."
+            ) from err
+
+        li_nodes = [node.to_llama_index() for node in sorted(self.nodes)]
+        for i in range(len(li_nodes) - 1):
+            li_nodes[i].relationships[NodeRelationship.NEXT] = li_nodes[
+                i + 1
+            ].as_related_node_info()
+
+            li_nodes[i + 1].relationships[NodeRelationship.PREVIOUS] = li_nodes[
+                i
+            ].as_related_node_info()
+
+        for li_node in li_nodes:
+            li_node.relationships[NodeRelationship.PARENT] = (
+                llama_index_doc.as_related_node_info()
+            )
+
+        return li_nodes
```

### Comparing `openparse-0.5.5/src/openparse/tables/parse.py` & `openparse-0.5.6/src/openparse/tables/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/pymupdf/parse.py` & `openparse-0.5.6/src/openparse/tables/pymupdf/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/table_transformers/geometry.py` & `openparse-0.5.6/src/openparse/tables/table_transformers/geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/table_transformers/ml.py` & `openparse-0.5.6/src/openparse/tables/table_transformers/ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/table_transformers/schemas.py` & `openparse-0.5.6/src/openparse/tables/table_transformers/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/unitable/config.py` & `openparse-0.5.6/src/openparse/tables/unitable/config.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/unitable/core.py` & `openparse-0.5.6/src/openparse/tables/unitable/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/unitable/schemas.py` & `openparse-0.5.6/src/openparse/tables/unitable/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/unitable/tabular_transformer.py` & `openparse-0.5.6/src/openparse/tables/unitable/tabular_transformer.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/unitable/tokens.py` & `openparse-0.5.6/src/openparse/tables/unitable/tokens.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/unitable/unitable_model.py` & `openparse-0.5.6/src/openparse/tables/unitable/unitable_model.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/unitable/utils.py` & `openparse-0.5.6/src/openparse/tables/unitable/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/tables/utils.py` & `openparse-0.5.6/src/openparse/tables/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/text/parse.py` & `openparse-0.5.6/src/openparse/text/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/text/pdfminer/core.py` & `openparse-0.5.6/src/openparse/text/pdfminer/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/text/pymupdf/core.py` & `openparse-0.5.6/src/openparse/text/pymupdf/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/openparse/version.py` & `openparse-0.5.6/src/openparse/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-OPEN_PARSE_VERSION = "0.5.5"
+OPEN_PARSE_VERSION = "0.5.6"
 
 
 def version_info() -> str:
     """Return complete version information for OpenParse and its dependencies."""
     import importlib.metadata as importlib_metadata
     import platform
     import sys
```

### Comparing `openparse-0.5.5/src/openparse.egg-info/PKG-INFO` & `openparse-0.5.6/src/openparse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.5.5
+Version: 0.5.6
 Summary: Streamlines the process of preparing documents for LLM's.
 Author-email: Sergey Filimonov <hello@sergey.fyi>
+License: MIT
 Project-URL: homepage, https://github.com/Filimoa/open-parse
 Project-URL: repository, https://github.com/Filimoa/open-parse
 Project-URL: documentation, https://filimoa.github.io/open-parse
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyMuPDF>=1.23.2
```

### Comparing `openparse-0.5.5/src/openparse.egg-info/SOURCES.txt` & `openparse-0.5.6/src/openparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/tests/processing/test_pipeline.py` & `openparse-0.5.6/src/tests/processing/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/tests/processing/test_steps.py` & `openparse-0.5.6/src/tests/processing/test_steps.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/tests/tables/pymupdf/test_parse.py` & `openparse-0.5.6/src/tests/tables/pymupdf/test_parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/tests/tables/transformers/test_geometry.py` & `openparse-0.5.6/src/tests/tables/transformers/test_geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/tests/tables/transformers/test_ml.py` & `openparse-0.5.6/src/tests/tables/transformers/test_ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/tests/tables/unitable/sample_pred_outputs.py` & `openparse-0.5.6/src/tests/tables/unitable/sample_pred_outputs.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/tests/tables/unitable/test_pred_to_schema.py` & `openparse-0.5.6/src/tests/tables/unitable/test_pred_to_schema.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/tests/test_doc_parser.py` & `openparse-0.5.6/src/tests/test_doc_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import openparse
 import re
 
 
 def test_parse_doc():
-
     basic_doc_path = "src/evals/data/full-pdfs/mock-1-page-lease.pdf"
     parser = openparse.DocumentParser()
     parsed_basic_doc = parser.parse(basic_doc_path)
     assert len(parsed_basic_doc.nodes) >= 1
     assert parsed_basic_doc.nodes[0].text.startswith("**MOCK LEASE AGREEMENT**")
 
 
@@ -45,7 +44,16 @@
     doc_with_tables_path = "src/evals/data/tables/meta-2022-10k-page-69.pdf"
 
     parser = openparse.DocumentParser(table_args={"parsing_algorithm": "pymupdf"})
 
     parsed_doc2 = parser.parse(doc_with_tables_path)
     assert len(parsed_doc2.nodes) >= 1
     assert parsed_doc2.nodes[-1].text.startswith("<table")
+
+
+def test_to_llama_index_nodes():
+    basic_doc_path = "src/evals/data/full-pdfs/mock-1-page-lease.pdf"
+    parser = openparse.DocumentParser()
+    parsed_basic_doc = parser.parse(basic_doc_path)
+
+    nodes = parsed_basic_doc.to_llama_index_nodes()
+    assert len(nodes) >= 1
```

### Comparing `openparse-0.5.5/src/tests/test_schemas.py` & `openparse-0.5.6/src/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.5/src/tests/text/pdf_miner/test_core.py` & `openparse-0.5.6/src/tests/text/pdf_miner/test_core.py`

 * *Files identical despite different names*

