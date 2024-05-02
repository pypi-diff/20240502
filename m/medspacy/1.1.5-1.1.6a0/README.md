# Comparing `tmp/medspacy-1.1.5.tar.gz` & `tmp/medspacy-1.1.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medspacy-1.1.5.tar", last modified: Fri Jan  5 22:34:18 2024, max compression
+gzip compressed data, was "medspacy-1.1.6a0.tar", last modified: Thu May  2 06:35:54 2024, max compression
```

## Comparing `medspacy-1.1.5.tar` & `medspacy-1.1.6a0.tar`

### file list

```diff
@@ -1,150 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.650109 medspacy-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-05 22:34:14.000000 medspacy-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-01-05 22:34:18.650109 medspacy-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-01-05 22:34:14.000000 medspacy-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.630109 medspacy-1.1.5/medspacy/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9472 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.646109 medspacy-1.1.5/medspacy/common/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/common/base_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/common/medspacy_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/common/regex_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/common/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.646109 medspacy-1.1.5/medspacy/context/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/context/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/context/context_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/context/context_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/context/context_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/context/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/custom_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.646109 medspacy-1.1.5/medspacy/io/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/io/config_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/io/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/io/db_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/io/db_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/io/db_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/io/doc_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/io/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/ner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.650109 medspacy-1.1.5/medspacy/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/postprocess/postprocessing_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/postprocess/postprocessing_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/postprocess/postprocessing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/postprocess/postprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.650109 medspacy-1.1.5/medspacy/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/preprocess/preprocessing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/preprocess/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.650109 medspacy-1.1.5/medspacy/section_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/section_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/section_detection/section.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/section_detection/section_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    21792 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/section_detection/sectionizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/section_detection/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/sentence_splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.650109 medspacy-1.1.5/medspacy/target_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/target_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/target_matcher/concept_tagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/target_matcher/target_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/target_matcher/target_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-01-05 22:34:14.000000 medspacy-1.1.5/medspacy/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.650109 medspacy-1.1.5/medspacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-01-05 22:34:18.000000 medspacy-1.1.5/medspacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-01-05 22:34:18.000000 medspacy-1.1.5/medspacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 22:34:18.000000 medspacy-1.1.5/medspacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-05 22:34:18.000000 medspacy-1.1.5/medspacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-05 22:34:18.000000 medspacy-1.1.5/medspacy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-05 22:34:14.000000 medspacy-1.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.634109 medspacy-1.1.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-05 22:34:14.000000 medspacy-1.1.5/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-05 22:34:14.000000 medspacy-1.1.5/requirements/requirements_tests.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.634109 medspacy-1.1.5/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    28157 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/context_rules.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.626109 medspacy-1.1.5/resources/quickumls/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.634109 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.634109 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.638109 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.638109 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.638109 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.646109 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
--rw-r--r--   0 runner    (1001) docker     (127)    23496 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/rush_rules.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-01-05 22:34:14.000000 medspacy-1.1.5/resources/section_patterns.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-05 22:34:18.650109 medspacy-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-01-05 22:34:14.000000 medspacy-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:18.650109 medspacy-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 22:34:14.000000 medspacy-1.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-01-05 22:34:14.000000 medspacy-1.1.5/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-01-05 22:34:14.000000 medspacy-1.1.5/tests/test_medspacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-01-05 22:34:14.000000 medspacy-1.1.5/tests/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.763316 medspacy-1.1.6a0/medspacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.775316 medspacy-1.1.6a0/medspacy/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/common/base_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/common/medspacy_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/common/regex_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/common/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.779316 medspacy-1.1.6a0/medspacy/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/context_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/context_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/context_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/context/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/custom_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.779316 medspacy-1.1.6a0/medspacy/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/config_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/db_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/db_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/db_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/doc_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/io/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/ner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.779316 medspacy-1.1.6a0/medspacy/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/postprocess/postprocessing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/postprocess/postprocessing_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/postprocess/postprocessing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/postprocess/postprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.779316 medspacy-1.1.6a0/medspacy/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/preprocess/preprocessing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/preprocess/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.779316 medspacy-1.1.6a0/medspacy/section_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/section_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/section_detection/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/section_detection/section_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21792 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/section_detection/sectionizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/section_detection/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/sentence_splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/medspacy/target_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/target_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/target_matcher/concept_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/target_matcher/target_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/target_matcher/target_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/medspacy/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/medspacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-02 06:35:54.000000 medspacy-1.1.6a0/medspacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-05-02 06:35:54.000000 medspacy-1.1.6a0/medspacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:35:54.000000 medspacy-1.1.6a0/medspacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 06:35:54.000000 medspacy-1.1.6a0/medspacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 06:35:54.000000 medspacy-1.1.6a0/medspacy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/requirements/requirements_tests.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.763316 medspacy-1.1.6a0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/context_rules.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.759316 medspacy-1.1.6a0/resources/quickumls/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.763316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.763316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.771316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.771316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.771316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.775316 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+-rw-r--r--   0 runner    (1001) docker     (127)    23496 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/rush_rules.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/resources/section_patterns.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:35:54.783316 medspacy-1.1.6a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/tests/test_medspacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-02 06:35:50.000000 medspacy-1.1.6a0/tests/test_notebooks.py
```

### Comparing `medspacy-1.1.5/LICENSE` & `medspacy-1.1.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/PKG-INFO` & `medspacy-1.1.6a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medspacy
-Version: 1.1.5
+Version: 1.1.6a0
 Summary: Library for clinical NLP with spaCy.
 Author: medSpaCy
 License: MIT License
         
         Copyright (c) 2020 medspacy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spacy<3.6,>=3.4.1
 Requires-Dist: PyRuSH>=1.0.8
 Requires-Dist: pysbd==0.3.4
 Requires-Dist: jsonschema
-Requires-Dist: medspacy_quickumls==3.0
+Requires-Dist: medspacy_quickumls==3.1
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
 
 # medspacy
 Library for clinical NLP with spaCy.
```

### Comparing `medspacy-1.1.5/README.md` & `medspacy-1.1.6a0/README.md`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/_extensions.py` & `medspacy-1.1.6a0/medspacy/_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module will set extension attributes and methods for medspaCy. Examples include custom methods like span._.window()"""
 from spacy.tokens import Doc, Span, Token
 
 from .common.util import span_contains
 
 # from .io.doc_consumer import ALLOWED_DATA_TYPES
 
-ALLOWED_DATA_TYPES = ("ents", "section", "context", "doc")
+ALLOWED_DATA_TYPES = ("ents", "group", "section", "context", "doc")
 
 
 def set_extensions():
     """Set custom medspaCy extensions for Token, Span, and Doc classes."""
     set_token_extensions()
     set_span_extensions()
     set_doc_extensions()
```

### Comparing `medspacy-1.1.5/medspacy/common/base_rule.py` & `medspacy-1.1.6a0/medspacy/common/base_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/common/medspacy_matcher.py` & `medspacy-1.1.6a0/medspacy/common/medspacy_matcher.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/common/regex_matcher.py` & `medspacy-1.1.6a0/medspacy/common/regex_matcher.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/common/util.py` & `medspacy-1.1.6a0/medspacy/common/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/context/context.py` & `medspacy-1.1.6a0/medspacy/context/context.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/context/context_graph.py` & `medspacy-1.1.6a0/medspacy/context/context_graph.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/context/context_modifier.py` & `medspacy-1.1.6a0/medspacy/context/context_modifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,15 @@
                 self._start,
             )
             if (
                 self.max_scope is not None
                 and (self._scope_end - self._scope_start) > self.max_scope
             ):
                 self._scope_start = self._start - self.max_scope
+        
         else:  # bidirectional
             self._scope_start, self._scope_end = (
                 full_scope_span.start,
                 full_scope_span.end,
             )
 
             # Set the max scope on either side
```

### Comparing `medspacy-1.1.5/medspacy/context/context_rule.py` & `medspacy-1.1.6a0/medspacy/context/context_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """
 
     _ALLOWED_DIRECTIONS = (
         "FORWARD",
         "BACKWARD",
         "BIDIRECTIONAL",
         "TERMINATE",
-        "PSEUDO",
+        "PSEUDO"
     )
     _ALLOWED_KEYS = {
         "literal",
         "direction",
         "pattern",
         "category",
         "metadata",
@@ -207,14 +207,15 @@
     def to_dict(self):
         """
         Converts ConTextItems to a python dictionary. Used when writing context rules to a json file.
 
         Returns:
             The dictionary containing the ConTextRule info.
         """
+
         rule_dict = {}
         for key in self._ALLOWED_KEYS:
             value = self.__dict__.get(key)
             if isinstance(value, set):
                 value = list(value)
             if value is not None:
                 rule_dict[key] = value
```

### Comparing `medspacy-1.1.5/medspacy/context/util.py` & `medspacy-1.1.6a0/medspacy/context/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/custom_tokenizer.py` & `medspacy-1.1.6a0/medspacy/custom_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/io/config_example.py` & `medspacy-1.1.6a0/medspacy/io/config_example.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/io/db_connect.py` & `medspacy-1.1.6a0/medspacy/io/db_connect.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/io/db_reader.py` & `medspacy-1.1.6a0/medspacy/io/db_reader.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/io/db_writer.py` & `medspacy-1.1.6a0/medspacy/io/db_writer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/io/doc_consumer.py` & `medspacy-1.1.6a0/medspacy/io/doc_consumer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Tuple, Dict, Optional
 
 from spacy.language import Language
 from spacy.tokens import Span
 
 from medspacy.context import ConTextModifier
 
-ALLOWED_DATA_TYPES = ("ents", "section", "context", "doc")
+ALLOWED_DATA_TYPES = ("ents", "group", "section", "context", "doc")
 
 DEFAULT_ENT_ATTRS = (
     "text",
     "start_char",
     "end_char",
     "label_",
     "is_negated",
@@ -193,15 +193,15 @@
                     try:
                         val = getattr(ent, attr)
                     except AttributeError:
                         val = getattr(ent._, attr)
                     data["ents"][attr].append(val)
         if "group" in self.dtypes:
             for span in doc.spans[self._span_group_name]:
-                for attr in self.dtype_attrs["ents"]:
+                for attr in self.dtype_attrs["group"]:
                     try:
                         val = getattr(span, attr)
                     except AttributeError:
                         val = getattr(span._, attr)
                     data["group"][attr].append(val)
         if "context" in self.dtypes:
             for (ent, modifier) in doc._.context_graph.edges:
@@ -223,36 +223,49 @@
     def add_context_edge_attributes(
         self, ent: Span, modifier: ConTextModifier, context_data, doc
     ):
         span_tup = modifier.modifier_span
         span = doc[span_tup[0] : span_tup[1]]
         scope_tup = modifier.scope_span
         scope = doc[scope_tup[0] : scope_tup[1]]
-        if "ent_text" in self.dtype_attrs["context"]:
-            context_data["ent_text"].append(ent.text)
-        if "ent_label_" in self.dtype_attrs["context"]:
-            context_data["ent_label_"].append(ent.label_)
-        if "ent_start_char" in self.dtype_attrs["context"]:
-            context_data["ent_start_char"].append(ent.start_char)
-        if "ent_end_char" in self.dtype_attrs["context"]:
-            context_data["ent_end_char"].append(ent.end_char)
-        if "modifier_text" in self.dtype_attrs["context"]:
-            context_data["modifier_text"].append(span.text)
-        if "modifier_category" in self.dtype_attrs["context"]:
-            context_data["modifier_category"].append(modifier.category)
-        if "modifier_direction" in self.dtype_attrs["context"]:
-            context_data["modifier_direction"].append(modifier.direction)
-        if "modifier_start_char" in self.dtype_attrs["context"]:
-            context_data["modifier_start_char"].append(span.start_char)
-        if "modifier_end_char" in self.dtype_attrs["context"]:
-            context_data["modifier_end_char"].append(span.end_char)
-        if "modifier_scope_start_char" in self.dtype_attrs["context"]:
-            context_data["modifier_scope_start_char"].append(scope.start_char)
-        if "modifier_scope_end_char" in self.dtype_attrs["context"]:
-            context_data["modifier_scope_end_char"].append(scope.end_char)
+        for attr in self.dtype_attrs["context"]:
+            if attr == "ent_text":
+                context_data["ent_text"].append(ent.text)
+            elif attr == "ent_label_":
+                context_data["ent_label_"].append(ent.label_)
+            elif attr == "ent_start_char":
+                context_data["ent_start_char"].append(ent.start_char)
+            elif attr == "ent_end_char":
+                context_data["ent_end_char"].append(ent.end_char)
+            elif attr == "modifier_text":
+                context_data["modifier_text"].append(span.text)
+            elif attr == "modifier_category":
+                context_data["modifier_category"].append(modifier.category)
+            elif attr == "modifier_direction":
+               context_data["modifier_direction"].append(modifier.direction)
+            elif attr == "modifier_start_char":
+                context_data["modifier_start_char"].append(span.start_char)
+            elif attr == "modifier_end_char":
+                context_data["modifier_end_char"].append(span.end_char)
+            elif attr == "modifier_scope_start_char":
+                context_data["modifier_scope_start_char"].append(scope.start_char)
+            elif attr == "modifier_scope_end_char":
+                context_data["modifier_scope_end_char"].append(scope.end_char)
+            else:
+            # if specified attribute is not one of these standard values, check the entity to see if it's an entity value
+                try:
+                    val = getattr(ent, attr)
+                except AttributeError:
+                    try:
+                        val = getattr(ent._, attr)
+                    except AttributeError:
+                        raise ValueError(f"Attributes for dtype 'context' must be either "
+                                         f"a registered custom Span attribute (i.e., Span._.attr) or one of these pre-defined values: "
+                                          f"{ALLOWED_CONTEXT_ATTRS}. \nYou passed in '{attr}'")
+                context_data[f"{attr}"].append(val)
 
     def add_section_attributes(self, section, section_data, doc):
         # Allow for null sections
         section_title_tup = section.title_span
         section_body_tup = section.body_span
         section_title = doc[section_title_tup[0] : section_title_tup[1]]
         section_body = doc[section_body_tup[0] : section_body_tup[1]]
```

### Comparing `medspacy-1.1.5/medspacy/io/pipeline.py` & `medspacy-1.1.6a0/medspacy/io/pipeline.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/postprocess/postprocessing_functions.py` & `medspacy-1.1.6a0/medspacy/postprocess/postprocessing_functions.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/postprocess/postprocessing_pattern.py` & `medspacy-1.1.6a0/medspacy/postprocess/postprocessing_pattern.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/postprocess/postprocessing_rule.py` & `medspacy-1.1.6a0/medspacy/postprocess/postprocessing_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/postprocess/postprocessor.py` & `medspacy-1.1.6a0/medspacy/postprocess/postprocessor.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/preprocess/preprocessing_rule.py` & `medspacy-1.1.6a0/medspacy/preprocess/preprocessing_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/preprocess/preprocessor.py` & `medspacy-1.1.6a0/medspacy/preprocess/preprocessor.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/section_detection/section.py` & `medspacy-1.1.6a0/medspacy/section_detection/section.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/section_detection/section_rule.py` & `medspacy-1.1.6a0/medspacy/section_detection/section_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/section_detection/sectionizer.py` & `medspacy-1.1.6a0/medspacy/section_detection/sectionizer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/section_detection/util.py` & `medspacy-1.1.6a0/medspacy/section_detection/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/sentence_splitting.py` & `medspacy-1.1.6a0/medspacy/sentence_splitting.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/target_matcher/concept_tagger.py` & `medspacy-1.1.6a0/medspacy/target_matcher/concept_tagger.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/target_matcher/target_matcher.py` & `medspacy-1.1.6a0/medspacy/target_matcher/target_matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         self,
         nlp: Language,
         name: str = "medspacy_target_matcher",
         rules: Optional[str] = None,
         phrase_matcher_attr: str = "LOWER",
         result_type: Union[Literal["ents", "group"], None] = "ents",
         span_group_name: str = "medspacy_spans",
+        prune: bool = True
     ):
         """
         Creates a new TargetMatcher.
 
         Args:
             nlp: A spaCy Language model.
             name: The name of the TargetMatcher component
@@ -49,20 +50,21 @@
             span_group_name: The name of the span group used to store results when result_type is "group". Default is
                 "medspacy_spans".
         """
         self.nlp = nlp
         self.name = name
         self._result_type = result_type
         self._span_group_name = span_group_name
+        self._prune = prune
 
         if rules:
             self.add(TargetRule.from_json(rules))
 
         self.__matcher = MedspacyMatcher(
-            nlp, name=name, phrase_matcher_attr=phrase_matcher_attr
+            nlp, name=name, phrase_matcher_attr=phrase_matcher_attr, prune=self._prune
         )
 
     @property
     def rules(self) -> List[TargetRule]:
         """
         Gets the list of TargetRules for the TargetMatcher.
```

### Comparing `medspacy-1.1.5/medspacy/target_matcher/target_rule.py` & `medspacy-1.1.6a0/medspacy/target_matcher/target_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/util.py` & `medspacy-1.1.6a0/medspacy/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/medspacy/visualization.py` & `medspacy-1.1.6a0/medspacy/visualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 def visualize_ent(
     doc: Doc,
     context: bool = True,
     sections: bool = True,
     jupyter: bool = True,
     colors: Dict[str, str] = None,
+    target_span_type: str = "ents",
+    span_group_name: str = "medspacy_spans"
 ) -> str:
     """
     Creates a NER-style visualization for targets and modifiers in Doc.
 
     Args:
         doc: A spacy doc to visualize.
         context: Whether to display the modifiers generated by medSpaCy's cycontext. If the doc has not been processed
@@ -33,15 +35,22 @@
     if not hasattr(doc._, "context_graph"):
         context = False
     if not hasattr(doc._, "sections"):
         sections = False
 
     ents_data = []
 
-    for target in doc.ents:
+    if target_span_type == "ents":
+        targets = doc.ents
+    elif target_span_type == "group":
+        targets = doc.spans[span_group_name]
+    else:
+        raise ValueError("Target span type must be either ents or group.")
+
+    for target in targets:
         ent_data = {
             "start": target.start_char,
             "end": target.end_char,
             "label": target.label_.upper(),
         }
         ents_data.append((ent_data, "ent"))
 
@@ -151,16 +160,31 @@
     token_data_mapping = {}
     for token in doc:
         data = {"text": token.text, "tag": "", "index": token.i}
         token_data.append(data)
         token_data_mapping[token] = data
 
     # Merge phrases
-    targets_and_modifiers = [*doc._.context_graph.targets]
-    targets_and_modifiers += [*doc._.context_graph.modifiers]
+    # targets_and_modifiers = [*doc._.context_graph.targets]
+    existing_tokens = set()
+    targets_and_modifiers = []
+    # Used to prevent duplication of token in targets or modifiers that appear twice due to being in a span group or, appearing twice as a modifier
+    for target_or_modifier in (list(doc._.context_graph.targets) + doc._.context_graph.modifiers):
+        if isinstance (target_or_modifier, Span):
+            span=target_or_modifier
+        else:
+            span=doc[target_or_modifier._start : target_or_modifier._end]
+        already_seen = False 
+        for token in span:
+            if token in existing_tokens:
+                already_seen = True 
+                break 
+        if not already_seen:
+            targets_and_modifiers.append(target_or_modifier)
+            existing_tokens.update({token for token in span}) 
 
     for obj in targets_and_modifiers:
         if isinstance(obj, Span):
             first_token = obj[0]
             data = token_data_mapping[first_token]
             data["tag"] = obj.label_
             if len(obj) > 1:
@@ -202,33 +226,35 @@
         #     token_data.pop(idx + 1)
         #
         # # Lower the index of the following tokens
         # for other_data in token_data[idx + 1 :]:
         #     other_data["index"] -= len(span) - 1
 
     dep_data = {"words": token_data, "arcs": []}
+    
     # Gather the edges between targets and modifiers
     for target, modifier in doc._.context_graph.edges:
         target_data = token_data_mapping[target[0]]
         modifier_data = token_data_mapping[doc[modifier.modifier_span[0]]]
         dep_data["arcs"].append(
             {
                 "start": min(target_data["index"], modifier_data["index"]),
                 "end": max(target_data["index"], modifier_data["index"]),
                 "label": modifier.category,
                 "dir": "right"
                 if target > doc[modifier.modifier_span[0] : modifier.modifier_span[1]]
                 else "left",
             }
         )
+    
     return displacy.render(dep_data, manual=True, jupyter=jupyter)
 
 
 class MedspaCyVisualizerWidget:
-    def __init__(self, docs):
+    def __init__(self, docs, target_span_type: str = "ents", span_group_name: str = "medspacy_spans"):
 
         """Create an IPython Widget Box displaying medspaCy's visualizers.
         The widget allows selecting visualization style ("Ent", "Dep", or "Both")
         and a slider for selecting the index of docs.
 
         For more information on IPython widgets, see:
             https://ipywidgets.readthedocs.io/en/latest/index.html
@@ -237,14 +263,16 @@
             docs: A list of docs processed by a medspaCy pipeline
 
         """
 
         import ipywidgets as widgets
 
         self.docs = docs
+        self.target_span_type = target_span_type 
+        self.span_group_name = span_group_name
         self.slider = widgets.IntSlider(
             value=0,
             min=0,
             max=len(docs) - 1,
             step=1,
             description="Doc:",
             disabled=False,
@@ -290,15 +318,15 @@
 
     def _visualize_doc(self):
         self.output.clear_output()
         doc = self.docs[self.slider.value]
         if self.radio.value.lower() in ("dep", "both"):
             visualize_dep(doc)
         if self.radio.value.lower() in ("ent", "both"):
-            visualize_ent(doc)
+            visualize_ent(doc, target_span_type=self.target_span_type, span_group_name=self.span_group_name)
 
     def _on_click_next(self, b):
         if self.slider.value < len(self.docs) - 1:
             self.slider.value += 1
 
     def _on_click_prev(self, b):
         if self.slider.value > 0:
```

### Comparing `medspacy-1.1.5/medspacy.egg-info/PKG-INFO` & `medspacy-1.1.6a0/medspacy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medspacy
-Version: 1.1.5
+Version: 1.1.6a0
 Summary: Library for clinical NLP with spaCy.
 Author: medSpaCy
 License: MIT License
         
         Copyright (c) 2020 medspacy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spacy<3.6,>=3.4.1
 Requires-Dist: PyRuSH>=1.0.8
 Requires-Dist: pysbd==0.3.4
 Requires-Dist: jsonschema
-Requires-Dist: medspacy_quickumls==3.0
+Requires-Dist: medspacy_quickumls==3.1
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
 
 # medspacy
 Library for clinical NLP with spaCy.
```

### Comparing `medspacy-1.1.5/medspacy.egg-info/SOURCES.txt` & `medspacy-1.1.6a0/medspacy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -118,11 +118,11 @@
 medspacy/section_detection/section_rule.py
 medspacy/section_detection/sectionizer.py
 medspacy/section_detection/util.py
 medspacy/target_matcher/__init__.py
 medspacy/target_matcher/concept_tagger.py
 medspacy/target_matcher/target_matcher.py
 medspacy/target_matcher/target_rule.py
-tests/__init__.py
+requirements/requirements.txt
 tests/test_extensions.py
 tests/test_medspacy.py
 tests/test_notebooks.py
```

### Comparing `medspacy-1.1.5/pyproject.toml` & `medspacy-1.1.6a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 
 #https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html#dynamic-metadata
 [tool.setuptools.dynamic]
-dependencies = {file = ["requirments/requirements.txt"]}
+dependencies = {file = ["requirements/requirements.txt"]}
 version={file = "medspacy/VERSION"}
 readme={file = ['README.md'], content-type = "text/markdown"}
 
 [project.urls]
 Source = "https://github.com/medspacy/medspacy"
 
 [tool.setuptools]
-include-package-data = true
-
+include-package-data = true
```

### Comparing `medspacy-1.1.5/resources/context_rules.json` & `medspacy-1.1.6a0/resources/context_rules.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9901960784313726%*

 * *Differences: {"'context_rules'": "{insert: [(98, OrderedDict([('category', 'NEGATED_EXISTENCE'), ('literal', "*

 * *                    "'are not evident'), ('pattern', None), ('direction', 'BACKWARD')])), (99, "*

 * *                    "OrderedDict([('category', 'NEGATED_EXISTENCE'), ('literal', 'negative on'), "*

 * *                    "('pattern', None), ('direction', 'BACKWARD')]))]}"}*

```diff
@@ -1735,14 +1735,26 @@
         {
             "category": "NEGATED_EXISTENCE",
             "direction": "BACKWARD",
             "literal": ": no",
             "pattern": null
         },
         {
+            "category": "NEGATED_EXISTENCE",
+            "direction": "BACKWARD",
+            "literal": "are not evident",
+            "pattern": null
+        },
+        {
+            "category": "NEGATED_EXISTENCE",
+            "direction": "BACKWARD",
+            "literal": "negative on",
+            "pattern": null
+        },
+        {
             "category": "HISTORICAL",
             "direction": "TERMINATE",
             "literal": "presentation",
             "pattern": [
                 {
                     "LOWER": {
                         "IN": [
```

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy-1.1.6a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/rush_rules.tsv` & `medspacy-1.1.6a0/resources/rush_rules.tsv`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/resources/section_patterns.json` & `medspacy-1.1.6a0/resources/section_patterns.json`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/setup.py` & `medspacy-1.1.6a0/setup.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/tests/test_extensions.py` & `medspacy-1.1.6a0/tests/test_extensions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os, sys
+# recent pytest failed because of project directory is not included in sys.path somehow, might due to other configuration issue. Add this for a temp solution
+sys.path.append(os.getcwd())
 import pytest
 import sys
 
 import medspacy
 
 import spacy
```

### Comparing `medspacy-1.1.5/tests/test_medspacy.py` & `medspacy-1.1.6a0/tests/test_medspacy.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.1.5/tests/test_notebooks.py` & `medspacy-1.1.6a0/tests/test_notebooks.py`

 * *Files identical despite different names*

