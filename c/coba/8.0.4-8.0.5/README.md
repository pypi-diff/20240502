# Comparing `tmp/coba-8.0.4.tar.gz` & `tmp/coba-8.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coba-8.0.4.tar", last modified: Tue Apr 30 15:53:38 2024, max compression
+gzip compressed data, was "coba-8.0.5.tar", last modified: Thu May  2 00:29:21 2024, max compression
```

## Comparing `coba-8.0.4.tar` & `coba-8.0.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.672798 coba-8.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:53:34.000000 coba-8.0.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-30 15:53:34.000000 coba-8.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-30 15:53:38.672798 coba-8.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-30 15:53:34.000000 coba-8.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.664798 coba-8.0.4/coba/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-30 15:53:34.000000 coba-8.0.4/coba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-30 15:53:34.000000 coba-8.0.4/coba/backports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.664798 coba-8.0.4/coba/context/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-30 15:53:34.000000 coba-8.0.4/coba/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-04-30 15:53:34.000000 coba-8.0.4/coba/context/cachers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-30 15:53:34.000000 coba-8.0.4/coba/context/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-30 15:53:34.000000 coba-8.0.4/coba/context/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 15:53:34.000000 coba-8.0.4/coba/contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-04-30 15:53:34.000000 coba-8.0.4/coba/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.668798 coba-8.0.4/coba/environments/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45104 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    63249 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/openml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/serialized.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/supervised.py
--rw-r--r--   0 runner    (1001) docker     (127)    28215 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/synthetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-30 15:53:34.000000 coba-8.0.4/coba/environments/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.668798 coba-8.0.4/coba/evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-30 15:53:34.000000 coba-8.0.4/coba/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-04-30 15:53:34.000000 coba-8.0.4/coba/evaluators/offline.py
--rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-04-30 15:53:34.000000 coba-8.0.4/coba/evaluators/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-30 15:53:34.000000 coba-8.0.4/coba/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.668798 coba-8.0.4/coba/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 15:53:34.000000 coba-8.0.4/coba/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-04-30 15:53:34.000000 coba-8.0.4/coba/experiments/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-30 15:53:34.000000 coba-8.0.4/coba/experiments/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-30 15:53:34.000000 coba-8.0.4/coba/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.668798 coba-8.0.4/coba/learners/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/bandit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/corral.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/lints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/linucb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/misguided.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    31782 2024-04-30 15:53:34.000000 coba-8.0.4/coba/learners/vowpal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-30 15:53:34.000000 coba-8.0.4/coba/multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.672798 coba-8.0.4/coba/pipes/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14927 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/lines.py
--rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19967 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/rows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/sinks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-30 15:53:34.000000 coba-8.0.4/coba/pipes/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21025 2024-04-30 15:53:34.000000 coba-8.0.4/coba/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-04-30 15:53:34.000000 coba-8.0.4/coba/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-30 15:53:34.000000 coba-8.0.4/coba/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-30 15:53:34.000000 coba-8.0.4/coba/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.672798 coba-8.0.4/coba/results/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-30 15:53:34.000000 coba-8.0.4/coba/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    85885 2024-04-30 15:53:34.000000 coba-8.0.4/coba/results/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-30 15:53:34.000000 coba-8.0.4/coba/results/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17102 2024-04-30 15:53:34.000000 coba-8.0.4/coba/safety.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-30 15:53:34.000000 coba-8.0.4/coba/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-30 15:53:34.000000 coba-8.0.4/coba/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:53:38.672798 coba-8.0.4/coba.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 15:53:38.000000 coba-8.0.4/coba.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 15:53:34.000000 coba-8.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:53:38.672798 coba-8.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:21.607781 coba-8.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:29:17.000000 coba-8.0.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-02 00:29:17.000000 coba-8.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-02 00:29:21.607781 coba-8.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-02 00:29:17.000000 coba-8.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:21.599781 coba-8.0.5/coba/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-02 00:29:17.000000 coba-8.0.5/coba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-02 00:29:17.000000 coba-8.0.5/coba/backports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:21.603781 coba-8.0.5/coba/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-02 00:29:17.000000 coba-8.0.5/coba/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-05-02 00:29:17.000000 coba-8.0.5/coba/context/cachers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-05-02 00:29:17.000000 coba-8.0.5/coba/context/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-05-02 00:29:17.000000 coba-8.0.5/coba/context/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-02 00:29:17.000000 coba-8.0.5/coba/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-02 00:29:17.000000 coba-8.0.5/coba/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:21.603781 coba-8.0.5/coba/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-02 00:29:17.000000 coba-8.0.5/coba/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45104 2024-05-02 00:29:17.000000 coba-8.0.5/coba/environments/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62651 2024-05-02 00:29:17.000000 coba-8.0.5/coba/environments/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-05-02 00:29:17.000000 coba-8.0.5/coba/environments/openml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-02 00:29:17.000000 coba-8.0.5/coba/environments/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-02 00:29:17.000000 coba-8.0.5/coba/environments/serialized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-02 00:29:17.000000 coba-8.0.5/coba/environments/supervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28215 2024-05-02 00:29:17.000000 coba-8.0.5/coba/environments/synthetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-02 00:29:17.000000 coba-8.0.5/coba/environments/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:21.603781 coba-8.0.5/coba/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-02 00:29:17.000000 coba-8.0.5/coba/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-02 00:29:17.000000 coba-8.0.5/coba/evaluators/offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-05-02 00:29:17.000000 coba-8.0.5/coba/evaluators/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-02 00:29:17.000000 coba-8.0.5/coba/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:21.603781 coba-8.0.5/coba/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-02 00:29:17.000000 coba-8.0.5/coba/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-05-02 00:29:17.000000 coba-8.0.5/coba/experiments/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-05-02 00:29:17.000000 coba-8.0.5/coba/experiments/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-02 00:29:17.000000 coba-8.0.5/coba/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:21.607781 coba-8.0.5/coba/learners/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-02 00:29:17.000000 coba-8.0.5/coba/learners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-02 00:29:17.000000 coba-8.0.5/coba/learners/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-02 00:29:17.000000 coba-8.0.5/coba/learners/corral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-02 00:29:17.000000 coba-8.0.5/coba/learners/lints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-02 00:29:17.000000 coba-8.0.5/coba/learners/linucb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-02 00:29:17.000000 coba-8.0.5/coba/learners/misguided.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-02 00:29:17.000000 coba-8.0.5/coba/learners/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31782 2024-05-02 00:29:17.000000 coba-8.0.5/coba/learners/vowpal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-02 00:29:17.000000 coba-8.0.5/coba/multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:21.607781 coba-8.0.5/coba/pipes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-02 00:29:17.000000 coba-8.0.5/coba/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-02 00:29:17.000000 coba-8.0.5/coba/pipes/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14927 2024-05-02 00:29:17.000000 coba-8.0.5/coba/pipes/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-05-02 00:29:17.000000 coba-8.0.5/coba/pipes/lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-05-02 00:29:17.000000 coba-8.0.5/coba/pipes/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-05-02 00:29:17.000000 coba-8.0.5/coba/pipes/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19967 2024-05-02 00:29:17.000000 coba-8.0.5/coba/pipes/rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-02 00:29:17.000000 coba-8.0.5/coba/pipes/sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-05-02 00:29:17.000000 coba-8.0.5/coba/pipes/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-02 00:29:17.000000 coba-8.0.5/coba/pipes/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21025 2024-05-02 00:29:17.000000 coba-8.0.5/coba/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-05-02 00:29:17.000000 coba-8.0.5/coba/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-02 00:29:17.000000 coba-8.0.5/coba/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-02 00:29:17.000000 coba-8.0.5/coba/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:21.607781 coba-8.0.5/coba/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-02 00:29:17.000000 coba-8.0.5/coba/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86418 2024-05-02 00:29:17.000000 coba-8.0.5/coba/results/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-02 00:29:17.000000 coba-8.0.5/coba/results/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17102 2024-05-02 00:29:17.000000 coba-8.0.5/coba/safety.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-02 00:29:17.000000 coba-8.0.5/coba/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-02 00:29:17.000000 coba-8.0.5/coba/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:21.607781 coba-8.0.5/coba.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-02 00:29:21.000000 coba-8.0.5/coba.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-02 00:29:21.000000 coba-8.0.5/coba.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:29:21.000000 coba-8.0.5/coba.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 00:29:21.000000 coba-8.0.5/coba.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 00:29:21.000000 coba-8.0.5/coba.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 00:29:21.000000 coba-8.0.5/coba.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-02 00:29:17.000000 coba-8.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:29:21.607781 coba-8.0.5/setup.cfg
```

### Comparing `coba-8.0.4/LICENSE` & `coba-8.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/PKG-INFO` & `coba-8.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 8.0.4
+Version: 8.0.5
 Summary: A contextual bandit research package
 Author-email: Mark Rucker <rucker.mark@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://coba-docs.readthedocs.io/
 Project-URL: Documentation, https://coba-docs.readthedocs.io/
 Project-URL: Repository, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coba-8.0.4/README.md` & `coba-8.0.5/README.md`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/__init__.py` & `coba-8.0.5/coba/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from coba.statistics import mean
 
 from coba.primitives import is_batch, Context, Action, Actions, Categorical, Dense, Sparse
 from coba.primitives import Learner, Environment, Interaction, Evaluator, Rewards, Namespaces
 from coba.primitives import LoggedInteraction, SimulatedInteraction, GroundedInteraction
 from coba.primitives import L1Reward, HammingReward, DiscreteReward
 
-__version__ = "8.0.4"
+__version__ = "8.0.5"
```

### Comparing `coba-8.0.4/coba/context/cachers.py` & `coba-8.0.5/coba/context/cachers.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/context/core.py` & `coba-8.0.5/coba/context/core.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/context/loggers.py` & `coba-8.0.5/coba/context/loggers.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/encodings.py` & `coba-8.0.5/coba/encodings.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/environments/__init__.py` & `coba-8.0.5/coba/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/environments/core.py` & `coba-8.0.5/coba/environments/core.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/environments/filters.py` & `coba-8.0.5/coba/environments/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 import pickle
 import warnings
 import copy
 
 from math import isnan
-from statistics import median, stdev, mode
+from statistics import median, stdev, mode, fmean
 from numbers import Number
 from zlib import crc32
 from operator import eq, methodcaller, itemgetter
 from collections import defaultdict
 from functools import lru_cache
 from itertools import islice, chain, tee, compress, repeat
 from typing import Optional, Sequence, Union, Iterable, Any, Tuple, Callable, Mapping, Literal
@@ -132,77 +132,74 @@
         if isinstance(first_context, primitives.Sparse) and self._target=="context" and self._shift != 0:
             raise CobaException("Shift is required to be 0 for sparse environments. Otherwise the environment will become dense.")
 
         is_dense_context  = isinstance(first_context, primitives.Dense)
         is_sparse_context = isinstance(first_context, primitives.Sparse)
         is_value_context  = not (is_dense_context or is_sparse_context)
 
-        #get the values we wish to scale
-        if self._target == "context" :
-            if is_dense_context:
-                potential_cols = [i for i,v in enumerate(first['context']) if isinstance(v,(int,float))]
-                if len(potential_cols) == 0:
-                    unscaled = []
-                elif len(potential_cols) == 1:
-                    unscaled = [ tuple(map(itemgetter(*potential_cols),map(itemgetter("context"),fitting_interactions))) ]
-                else:
-                    unscaled = list(zip(*map(itemgetter(*potential_cols),map(itemgetter("context"),fitting_interactions))))
-            elif is_sparse_context:
-                unscalable_cols = {k for k,v in first['context'].items() if not isinstance(v,(int,float))}
-                unscaled = defaultdict(list)
-                for interaction in fitting_interactions:
-                    context = interaction['context']
-                    for k in context.keys()-unscalable_cols:
-                        unscaled[k].append(context[k])
-            elif is_value_context:
-                unscaled = [interaction['context'] for interaction in fitting_interactions]
-
-        #determine the scale and shift values
-        if self._target == "context":
-            if is_dense_context:
-                shifts_scales = []
-                for i,col in zip(potential_cols,unscaled):
-                    shift_scale = self._get_shift_and_scale(col)
-                    if shift_scale is not None:
-                        shifts_scales.append((i,)+shift_scale)
-            elif is_sparse_context:
-                shifts_scales = {}
-                for k,col in unscaled.items():
-                    vals = col + [0]*(len(fitting_interactions)-len(col))
-                    shift_scale = self._get_shift_and_scale(vals)
-                    if shift_scale is not None:
-                        shifts_scales[k] = shift_scale
-            elif is_value_context:
-                shifts_scales = self._get_shift_and_scale(unscaled)
+        fitting_contexts = list(map(itemgetter('context'),fitting_interactions))
 
-        #now scale
-        if not shifts_scales:
+        #get the potential keys to scale
+        potential_keys = None
+        if is_dense_context:
+            potential_keys = [i for i,v in enumerate(first_context) if isinstance(v,(int,float))]
+        if is_sparse_context:
+            unscalable_cols = {k for k,v in first_context.items() if not isinstance(v,(int,float))}
+            potential_keys  = set().union(*map(methodcaller("keys"),fitting_contexts)) - unscalable_cols
+        if is_value_context:
+            potential_keys = [0]
+
+        if not potential_keys:
+            yield from chain(fitting_interactions,remaining_interactions)
+            return
+
+        #get the potential columns to scale
+        if is_dense_context and len(potential_keys) == 1:
+            cols = [map(itemgetter(potential_keys[0]),fitting_contexts)]
+        if is_dense_context and len(potential_keys) >= 2:
+            cols = zip(*map(itemgetter(*potential_keys),fitting_contexts))
+        if is_sparse_context:
+            cols = [ map(methodcaller("get",k,0), fitting_contexts) for k in potential_keys]
+        if is_value_context:
+            cols = [fitting_contexts]
+
+        #get the shift/scale values for columns
+        scaling_vals = list(map(self._get_shift_and_scale,cols))
+        if all((v is None for v in scaling_vals)):
             yield from chain(fitting_interactions, remaining_interactions)
-        elif self._target == "context":
-            if is_dense_context:
-                for interaction in chain(fitting_interactions, remaining_interactions):
-                    context = interaction['context']
-                    for i,shift,scale in shifts_scales:
-                        context[i] = (context[i]+shift)*scale
-                    yield interaction
-            elif is_sparse_context:
-                for interaction in chain(fitting_interactions, remaining_interactions):
-                    new = interaction # Mutable copies
-                    context = new['context']
-                    for k in shifts_scales.keys() & context.keys():
-                        (shift,scale) = shifts_scales[k]
-                        context[k] = (context[k]+shift)*scale
-                    yield new
-            elif is_value_context:
-                (shift,scale) = shifts_scales
-                for interaction in chain(fitting_interactions, remaining_interactions):
-                    new = interaction.copy()
-                    if new['context'] is not None:
-                        new['context'] = (new['context']+shift)*scale
-                    yield new
+            return
+
+        scaling_keys = compress(potential_keys,scaling_vals)
+        scaling_vals = compress(scaling_vals,scaling_vals)
+
+        #now shift and scale
+        if is_dense_context:
+            scaling_tuples = list(zip(scaling_keys,scaling_vals))
+            for interaction in chain(fitting_interactions, remaining_interactions):
+                context = interaction['context']
+                for i,(shift,scale) in scaling_tuples:
+                    context[i] = (context[i]+shift)*scale
+                yield interaction
+
+        if is_sparse_context:
+            scaling_dict = dict(zip(scaling_keys,scaling_vals))
+            for interaction in chain(fitting_interactions, remaining_interactions):
+                context = interaction['context']
+                for k in scaling_dict.keys() & context.keys():
+                    (shift,scale) = scaling_dict[k]
+                    context[k] = (context[k]+shift)*scale
+                yield interaction
+
+        elif is_value_context:
+            (shift,scale) = list(scaling_vals)[0]
+            for interaction in chain(fitting_interactions, remaining_interactions):
+                new = interaction.copy()
+                if new['context'] is not None:
+                    new['context'] = (new['context']+shift)*scale
+                yield new
 
     def _get_shift_and_scale(self,values) -> Tuple[float,float]:
         try:
             values = [v for v in values if v is not None]
             shift = self._shift_value(values)
             scale = self._scale_value(values,shift)
 
@@ -218,17 +215,17 @@
         except (TypeError,ValueError):
             return None
 
     def _shift_value(self, values) -> float:
         shift = self._shift
         if shift == "min":
             return -min(values)
-        elif shift == "mean":
-            return -sum(values)/len(values) #mean() is very slow due to calculations for precision
-        elif shift == "med" or shift == "median":
+        if shift == "mean":
+            return -fmean(values)
+        if shift == "med" or shift == "median":
             return -median(values)
         return shift
 
     def _scale_value(self, values, shift) -> float:
         scale     = self._scale
         scale_num = scale
         scale_den = 1
@@ -240,15 +237,15 @@
             scale_num = 1
             scale_den = stdev(values)
         elif scale == "iqr":
             scale_num = 1
             scale_den = iqr(values)
         elif scale == "maxabs":
             scale_num = 1
-            scale_den = max([abs(v+shift) for v in values])
+            scale_den = max(map(abs,map(shift.__add__,values)))
 
         return scale_num if scale_den < .000001 else scale_num/scale_den
 
 class Impute(EnvironmentFilter):
     """Impute missing values (nan) in Interaction contexts."""
 
     def __init__(self,
```

### Comparing `coba-8.0.4/coba/environments/openml.py` & `coba-8.0.5/coba/environments/openml.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/environments/results.py` & `coba-8.0.5/coba/environments/results.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/environments/serialized.py` & `coba-8.0.5/coba/environments/serialized.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/environments/supervised.py` & `coba-8.0.5/coba/environments/supervised.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/environments/synthetics.py` & `coba-8.0.5/coba/environments/synthetics.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/environments/templates.py` & `coba-8.0.5/coba/environments/templates.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/evaluators/offline.py` & `coba-8.0.5/coba/evaluators/offline.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/evaluators/sequential.py` & `coba-8.0.5/coba/evaluators/sequential.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/exceptions.py` & `coba-8.0.5/coba/exceptions.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/experiments/core.py` & `coba-8.0.5/coba/experiments/core.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/experiments/process.py` & `coba-8.0.5/coba/experiments/process.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/json.py` & `coba-8.0.5/coba/json.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/learners/__init__.py` & `coba-8.0.5/coba/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/learners/bandit.py` & `coba-8.0.5/coba/learners/bandit.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/learners/corral.py` & `coba-8.0.5/coba/learners/corral.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/learners/lints.py` & `coba-8.0.5/coba/learners/lints.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/learners/linucb.py` & `coba-8.0.5/coba/learners/linucb.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/learners/misguided.py` & `coba-8.0.5/coba/learners/misguided.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/learners/utilities.py` & `coba-8.0.5/coba/learners/utilities.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/learners/vowpal.py` & `coba-8.0.5/coba/learners/vowpal.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/multiprocessing.py` & `coba-8.0.5/coba/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/pipes/__init__.py` & `coba-8.0.5/coba/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/pipes/core.py` & `coba-8.0.5/coba/pipes/core.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/pipes/filters.py` & `coba-8.0.5/coba/pipes/filters.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/pipes/lines.py` & `coba-8.0.5/coba/pipes/lines.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/pipes/multiprocessing.py` & `coba-8.0.5/coba/pipes/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/pipes/readers.py` & `coba-8.0.5/coba/pipes/readers.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/pipes/rows.py` & `coba-8.0.5/coba/pipes/rows.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/pipes/sinks.py` & `coba-8.0.5/coba/pipes/sinks.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/pipes/sources.py` & `coba-8.0.5/coba/pipes/sources.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/pipes/utilities.py` & `coba-8.0.5/coba/pipes/utilities.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/primitives.py` & `coba-8.0.5/coba/primitives.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/random.py` & `coba-8.0.5/coba/random.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/register.py` & `coba-8.0.5/coba/register.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/registry.py` & `coba-8.0.5/coba/registry.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/results/core.py` & `coba-8.0.5/coba/results/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -3058,2311 +3058,2345 @@
 0000bf10: 7561 746f 7273 2c69 6e74 6572 6163 7469  uators,interacti
 0000bf20: 6f6e 7329 0a0a 2020 2020 6465 6620 7768  ons)..    def wh
 0000bf30: 6572 655f 6265 7374 2873 656c 662c 0a20  ere_best(self,. 
 0000bf40: 2020 2020 2020 206c 3a55 6e69 6f6e 5b73         l:Union[s
 0000bf50: 7472 2c20 5365 7175 656e 6365 5b73 7472  tr, Sequence[str
 0000bf60: 5d5d 2c0a 2020 2020 2020 2020 703a 556e  ]],.        p:Un
 0000bf70: 696f 6e5b 7374 722c 2053 6571 7565 6e63  ion[str, Sequenc
-0000bf80: 655b 7374 725d 5d20 3d20 2765 6e76 6972  e[str]] = 'envir
-0000bf90: 6f6e 6d65 6e74 5f69 6427 2c0a 2020 2020  onment_id',.    
-0000bfa0: 2020 2020 793a 7374 7220 3d20 2772 6577      y:str = 'rew
-0000bfb0: 6172 6427 2c0a 2020 2020 2020 2020 6e3a  ard',.        n:
-0000bfc0: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-0000bfd0: 2020 2020 6675 6c6c 5f6c 3a55 6e69 6f6e      full_l:Union
-0000bfe0: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
-0000bff0: 7472 5d5d 3d27 6c65 6172 6e65 725f 6964  tr]]='learner_id
-0000c000: 272c 0a20 2020 2020 2020 2066 756c 6c5f  ',.        full_
-0000c010: 703a 556e 696f 6e5b 7374 722c 2053 6571  p:Union[str, Seq
-0000c020: 7565 6e63 655b 7374 725d 5d3d 2765 6e76  uence[str]]='env
-0000c030: 6972 6f6e 6d65 6e74 5f69 6427 2920 2d3e  ironment_id') ->
-0000c040: 2027 5265 7375 6c74 273a 0a20 2020 2020   'Result':.     
-0000c050: 2020 2022 2222 5365 6c65 6374 2074 6865     """Select the
-0000c060: 2062 6573 7420 7065 7266 6f72 6d69 6e67   best performing
-0000c070: 2060 6c60 206f 7665 7220 6070 602e 0a0a   `l` over `p`...
-0000c080: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000c090: 2020 2020 2020 2020 2020 6c3a 2054 6865            l: The
-0000c0a0: 2068 7970 6572 7061 7261 6d65 7465 7220   hyperparameter 
-0000c0b0: 7661 6c75 6573 2077 6520 7769 7368 2074  values we wish t
-0000c0c0: 6f20 6f70 7469 6d69 7a65 2e0a 2020 2020  o optimize..    
-0000c0d0: 2020 2020 2020 2020 703a 2054 6865 2067          p: The g
-0000c0e0: 726f 7570 696e 6720 7661 7269 6162 6c65  rouping variable
-0000c0f0: 2077 6520 7769 7368 2074 6f20 6f70 7469   we wish to opti
-0000c100: 6d69 7a65 206f 7665 722e 0a20 2020 2020  mize over..     
-0000c110: 2020 2020 2020 2079 3a20 5468 6520 7661         y: The va
-0000c120: 7269 6162 6c65 2077 6520 7769 7368 2074  riable we wish t
-0000c130: 6f20 6f70 7469 6d69 7a65 2e0a 2020 2020  o optimize..    
-0000c140: 2020 2020 2020 2020 6e3a 2054 6865 206e          n: The n
-0000c150: 756d 6265 7220 6f66 2069 6e74 6572 6163  umber of interac
-0000c160: 7469 6f6e 7320 7765 2077 6973 6820 746f  tions we wish to
-0000c170: 2063 6f6e 7369 6465 722e 0a20 2020 2020   consider..     
-0000c180: 2020 2020 2020 2066 756c 6c5f 6c3a 2054         full_l: T
-0000c190: 6865 2074 7275 6520 6c6f 7765 7374 206c  he true lowest l
-0000c1a0: 6576 656c 206c 6162 656c 2028 652e 672e  evel label (e.g.
-0000c1b0: 2c20 6c65 6172 6e65 725f 6964 290a 2020  , learner_id).  
-0000c1c0: 2020 2020 2020 2020 2020 6675 6c6c 5f70            full_p
-0000c1d0: 3a20 5468 6520 7472 7565 206c 6f77 6573  : The true lowes
-0000c1e0: 7420 6c65 7665 6c20 7061 6972 2028 652e  t level pair (e.
-0000c1f0: 672e 2c20 656e 7669 726f 6e6d 656e 745f  g., environment_
-0000c200: 6964 290a 0a20 2020 2020 2020 2052 6574  id)..        Ret
-0000c210: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-0000c220: 2020 4120 5265 7375 6c74 2077 6974 6820    A Result with 
-0000c230: 6675 6c6c 2060 6c60 2061 6e64 2060 7060  full `l` and `p`
-0000c240: 2074 6861 7420 6973 2074 6865 206f 7074   that is the opt
-0000c250: 696d 616c 206f 7665 720a 2020 2020 2020  imal over.      
-0000c260: 2020 2020 2020 2020 2020 6066 756c 6c5f            `full_
-0000c270: 6c60 2061 6e64 2060 6675 6c6c 5f70 602e  l` and `full_p`.
-0000c280: 2046 6f72 2065 7861 6d70 6c65 2077 6520   For example we 
-0000c290: 636f 756c 6420 7361 7920 606c 600a 2020  could say `l`.  
-0000c2a0: 2020 2020 2020 2020 2020 2020 2020 6973                is
-0000c2b0: 2027 6661 6d69 6c79 2720 7768 696c 6520   'family' while 
-0000c2c0: 6066 756c 6c5f 6c60 2069 7320 276c 6561  `full_l` is 'lea
-0000c2d0: 726e 6572 5f69 6427 2e20 5468 6973 2077  rner_id'. This w
-0000c2e0: 6f75 6c64 0a20 2020 2020 2020 2020 2020  ould.           
-0000c2f0: 2020 2020 2070 6963 6b20 7468 6520 6265       pick the be
-0000c300: 7374 2070 6572 666f 726d 696e 6720 6c65  st performing le
-0000c310: 6172 6e65 7220 6772 6f75 7065 6420 6279  arner grouped by
-0000c320: 2066 616d 696c 7920 666f 720a 2020 2020   family for.    
-0000c330: 2020 2020 2020 2020 2020 2020 6561 6368              each
-0000c340: 2060 7060 2e0a 0a20 2020 2020 2020 2022   `p`...        "
-0000c350: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
-0000c360: 726e 2073 656c 662e 6669 6c74 6572 5f62  rn self.filter_b
-0000c370: 6573 7428 6c2c 702c 792c 6e2c 6675 6c6c  est(l,p,y,n,full
-0000c380: 5f6c 2c66 756c 6c5f 7029 0a0a 2020 2020  _l,full_p)..    
-0000c390: 6465 6620 7768 6572 655f 6669 6e28 7365  def where_fin(se
-0000c3a0: 6c66 2c0a 2020 2020 2020 2020 6e3a 2055  lf,.        n: U
-0000c3b0: 6e69 6f6e 5b69 6e74 2c4c 6974 6572 616c  nion[int,Literal
-0000c3c0: 5b27 6d69 6e27 5d5d 203d 204e 6f6e 652c  ['min']] = None,
-0000c3d0: 0a20 2020 2020 2020 206c 3a20 556e 696f  .        l: Unio
-0000c3e0: 6e5b 7374 722c 2053 6571 7565 6e63 655b  n[str, Sequence[
-0000c3f0: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
-0000c400: 2020 2020 2020 703a 2055 6e69 6f6e 5b73        p: Union[s
-0000c410: 7472 2c20 5365 7175 656e 6365 5b73 7472  tr, Sequence[str
-0000c420: 5d5d 203d 204e 6f6e 6529 202d 3e20 2752  ]] = None) -> 'R
-0000c430: 6573 756c 7427 3a0a 2020 2020 2020 2020  esult':.        
-0000c440: 2222 2246 696c 7465 7220 7468 6520 7265  """Filter the re
-0000c450: 7375 6c74 7320 646f 776e 2074 6f20 6576  sults down to ev
-0000c460: 656e 206f 7574 636f 6d65 7320 736f 2074  en outcomes so t
-0000c470: 6861 7420 706c 6f74 7465 6420 7265 7375  hat plotted resu
-0000c480: 6c74 7320 7769 6c6c 2062 6520 6d65 616e  lts will be mean
-0000c490: 696e 6766 756c 2e0a 0a20 2020 2020 2020  ingful...       
-0000c4a0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0000c4b0: 2020 206e 3a20 5468 6520 6e75 6d62 6572     n: The number
-0000c4c0: 206f 6620 696e 7465 7261 6374 696f 6e73   of interactions
-0000c4d0: 2061 2073 7065 6369 6669 6320 6576 616c   a specific eval
-0000c4e0: 7561 7469 6f6e 206d 7573 7420 6861 7665  uation must have
-0000c4f0: 2028 4e6f 6e65 2069 6e64 6963 6174 6573   (None indicates
-0000c500: 206e 6f20 636f 6e73 7472 6169 6e74 292e   no constraint).
-0000c510: 0a20 2020 2020 2020 2020 2020 206c 3a20  .            l: 
-0000c520: 5468 6520 6c65 7665 6c20 6174 2077 6869  The level at whi
-0000c530: 6368 2077 6520 7769 7368 2074 6f20 636f  ch we wish to co
-0000c540: 6d70 6172 6520 6576 616c 6174 696f 6e20  mpare evalation 
-0000c550: 6f75 7463 6f6d 6573 2028 652e 672e 2c20  outcomes (e.g., 
-0000c560: 276c 6561 726e 6572 5f69 6427 292e 0a20  'learner_id').. 
-0000c570: 2020 2020 2020 2020 2020 2070 3a20 5468             p: Th
-0000c580: 6520 7061 6972 7320 7468 6174 206d 7573  e pairs that mus
-0000c590: 7420 6578 6973 7420 6163 726f 7373 2061  t exist across a
-0000c5a0: 6c6c 2060 6c60 2069 6e20 6f72 6465 7220  ll `l` in order 
-0000c5b0: 746f 2062 6520 696e 636c 7564 6564 2028  to be included (
-0000c5c0: 652e 672e 2c20 2765 6e76 6972 6f6e 6d65  e.g., 'environme
-0000c5d0: 6e74 5f69 6427 292e 0a0a 2020 2020 2020  nt_id')...      
-0000c5e0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000c5f0: 2020 2020 2020 2041 2060 5265 7375 6c74         A `Result
-0000c600: 6020 7768 6572 6520 616e 2060 6c60 2065  ` where an `l` e
-0000c610: 7869 7374 7320 666f 7220 6576 6572 7920  xists for every 
-0000c620: 6070 6020 616e 6420 616c 6c20 6070 6020  `p` and all `p` 
-0000c630: 6861 7665 2027 6e27 2069 6e74 6572 6163  have 'n' interac
-0000c640: 7469 6f6e 732e 0a20 2020 2020 2020 2022  tions..        "
-0000c650: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
-0000c660: 726e 2073 656c 662e 6669 6c74 6572 5f66  rn self.filter_f
-0000c670: 696e 286e 2c6c 2c70 290a 0a20 2020 2064  in(n,l,p)..    d
-0000c680: 6566 2077 6865 7265 2873 656c 662c 202a  ef where(self, *
-0000c690: 2a6b 7761 7267 7329 202d 3e20 2752 6573  *kwargs) -> 'Res
-0000c6a0: 756c 7427 3a0a 2020 2020 2020 2020 2222  ult':.        ""
-0000c6b0: 2253 656c 6563 7420 6c65 6172 6e65 7273  "Select learners
-0000c6c0: 2f65 6e76 6972 6f6e 6d65 6e74 732f 6576  /environments/ev
-0000c6d0: 616c 7561 746f 7273 2e0a 0a20 2020 2020  aluators...     
-0000c6e0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000c6f0: 2020 2020 206b 7761 7267 733a 2041 6e79       kwargs: Any
-0000c700: 2063 6f6c 756d 6e20 696e 2065 6e76 6972   column in envir
-0000c710: 6f6e 6d65 6e74 732c 206c 6561 726e 6572  onments, learner
-0000c720: 732c 2061 6e64 2065 7661 6c75 6174 6f72  s, and evaluator
-0000c730: 7320 746f 2066 696c 7465 7220 6f6e 2e20  s to filter on. 
-0000c740: 4279 0a20 2020 2020 2020 2020 2020 2020  By.             
-0000c750: 2020 2064 6566 6175 6c74 2063 6f6d 7061     default compa
-0000c760: 7269 736f 6e20 6f70 6572 6174 6f72 7320  rison operators 
-0000c770: 6172 6520 6569 7468 6572 2027 6571 7561  are either 'equa
-0000c780: 6c27 206f 7220 2769 6e27 2e20 466f 7220  l' or 'in'. For 
-0000c790: 6578 616d 706c 652c 0a20 2020 2020 2020  example,.       
-0000c7a0: 2020 2020 2020 2020 2077 6865 7265 2865           where(e
-0000c7b0: 6e76 6972 6f6e 6d65 6e74 5f69 643d 3129  nvironment_id=1)
-0000c7c0: 2077 6f75 6c64 2072 6574 7572 6e20 6120   would return a 
-0000c7d0: 5265 7375 6c74 2077 6865 7265 2065 6e76  Result where env
-0000c7e0: 6972 6f6e 6d65 6e74 7320 6f6e 6c79 2063  ironments only c
-0000c7f0: 6f6e 7461 696e 730a 2020 2020 2020 2020  ontains.        
-0000c800: 2020 2020 2020 2020 656e 7669 726f 6e6d          environm
-0000c810: 656e 745f 6964 2031 2e20 4f6e 2074 6865  ent_id 1. On the
-0000c820: 206f 7468 6572 2068 616e 6420 7768 6572   other hand wher
-0000c830: 6528 656e 7669 726f 6e6d 656e 745f 6964  e(environment_id
-0000c840: 3d5b 312c 325d 2920 776f 756c 6420 7265  =[1,2]) would re
-0000c850: 7475 726e 2061 0a20 2020 2020 2020 2020  turn a.         
-0000c860: 2020 2020 2020 2052 6573 756c 7420 7768         Result wh
-0000c870: 6572 6520 656e 7669 726f 6e6d 656e 7473  ere environments
-0000c880: 2063 6f6e 7461 696e 7320 656e 7669 726f   contains enviro
-0000c890: 6e6d 656e 745f 6964 2031 2061 6e64 2032  nment_id 1 and 2
-0000c8a0: 2e20 5468 6520 6b65 7977 6f72 6473 206d  . The keywords m
-0000c8b0: 7573 740a 2020 2020 2020 2020 2020 2020  ust.            
-0000c8c0: 2020 2020 696e 6469 6361 7465 2061 2063      indicate a c
-0000c8d0: 6f6c 756d 6e20 6e61 6d65 2069 6e20 6569  olumn name in ei
-0000c8e0: 7468 6572 2065 6e76 6972 6f6e 6d65 6e74  ther environment
-0000c8f0: 732c 206c 6561 726e 6572 732c 2065 7661  s, learners, eva
-0000c900: 6c75 6174 6f72 732c 206f 720a 2020 2020  luators, or.    
-0000c910: 2020 2020 2020 2020 2020 2020 696e 7465              inte
-0000c920: 7261 6374 696f 6e73 2e20 5375 7070 6f72  ractions. Suppor
-0000c930: 7465 6420 636f 6d70 6172 6973 6f6e 206f  ted comparison o
-0000c940: 7065 7261 746f 7273 2061 7265 2027 3d27  perators are '='
-0000c950: 2c27 213d 272c 273c 3d27 2c27 3c27 2c27  ,'!=','<=','<','
-0000c960: 3e27 2c27 3e3d 272c 0a20 2020 2020 2020  >','>=',.       
-0000c970: 2020 2020 2020 2020 2027 6d61 7463 6827           'match'
-0000c980: 2c27 696e 272c 2721 696e 272e 2054 6f20  ,'in','!in'. To 
-0000c990: 696e 6469 6361 7465 2061 6e20 6578 706c  indicate an expl
-0000c9a0: 6963 6974 206f 7065 7261 746f 7220 7573  icit operator us
-0000c9b0: 6520 6120 6469 6374 696f 6e61 7279 2e20  e a dictionary. 
-0000c9c0: 466f 720a 2020 2020 2020 2020 2020 2020  For.            
-0000c9d0: 2020 2020 6578 616d 706c 652c 2077 6865      example, whe
-0000c9e0: 7265 2865 6e76 6972 6f6e 6d65 6e74 5f69  re(environment_i
-0000c9f0: 643d 7b27 3c3d 273a 3130 307d 2920 776f  d={'<=':100}) wo
-0000ca00: 756c 6420 7265 7475 726e 2061 2052 6573  uld return a Res
-0000ca10: 756c 7420 7769 7468 2061 6c6c 0a20 2020  ult with all.   
-0000ca20: 2020 2020 2020 2020 2020 2020 2065 6e76               env
-0000ca30: 6972 6f6e 6d65 6e74 7320 7768 6f73 6520  ironments whose 
-0000ca40: 656e 7669 726f 6e6d 656e 745f 6964 203c  environment_id <
-0000ca50: 3d20 3130 302e 2049 6e63 6c75 6469 6e67  = 100. Including
-0000ca60: 206d 756c 7469 706c 6520 6b77 6172 6773   multiple kwargs
-0000ca70: 2069 6e20 610a 2020 2020 2020 2020 2020   in a.          
-0000ca80: 2020 2020 2020 7369 6e67 6c65 2077 6865        single whe
-0000ca90: 7265 2061 7070 6c69 6573 2061 6e20 6f72  re applies an or
-0000caa0: 2063 6f6e 6a75 6374 696f 6e2e 2043 6861   conjuction. Cha
-0000cab0: 696e 696e 6720 7768 6572 6520 7374 6174  ining where stat
-0000cac0: 656d 656e 7473 2069 7320 6571 7569 7661  ements is equiva
-0000cad0: 6c65 6e74 0a20 2020 2020 2020 2020 2020  lent.           
-0000cae0: 2020 2020 2074 6f20 616e 2061 6e64 2063       to an and c
-0000caf0: 6f6e 6a75 6374 6f72 2e0a 0a20 2020 2020  onjuctor...     
-0000cb00: 2020 2052 6575 7472 6e73 3a0a 2020 2020     Reutrns:.    
-0000cb10: 2020 2020 2020 2020 4120 6052 6573 756c          A `Resul
-0000cb20: 7460 2077 686f 7365 2065 6e76 6972 6f6e  t` whose environ
-0000cb30: 6d65 6e74 732c 206c 6561 726e 6572 732c  ments, learners,
-0000cb40: 2065 7661 6c75 6174 6f72 732c 2061 6e64   evaluators, and
-0000cb50: 2069 6e74 6572 6163 7469 6f6e 7320 7361   interactions sa
-0000cb60: 7469 7366 7920 7468 650a 2020 2020 2020  tisfy the.      
-0000cb70: 2020 2020 2020 2020 2020 7768 6572 6520            where 
-0000cb80: 7365 6c65 6374 6f72 732e 0a20 2020 2020  selectors..     
-0000cb90: 2020 2022 2222 0a20 2020 2020 2020 2065     """.        e
-0000cba0: 6e76 5f6b 7761 7267 7320 3d20 7b7d 0a20  nv_kwargs = {}. 
-0000cbb0: 2020 2020 2020 206c 726e 5f6b 7761 7267         lrn_kwarg
-0000cbc0: 7320 3d20 7b7d 0a20 2020 2020 2020 2076  s = {}.        v
-0000cbd0: 616c 5f6b 7761 7267 7320 3d20 7b7d 0a20  al_kwargs = {}. 
-0000cbe0: 2020 2020 2020 2069 6e74 5f6b 7761 7267         int_kwarg
-0000cbf0: 7320 3d20 7b7d 0a0a 2020 2020 2020 2020  s = {}..        
-0000cc00: 666f 7220 6b65 792c 6172 6720 696e 206b  for key,arg in k
-0000cc10: 7761 7267 732e 6974 656d 7328 293a 0a20  wargs.items():. 
-0000cc20: 2020 2020 2020 2020 2020 2069 6620 6b65             if ke
-0000cc30: 7920 696e 2073 656c 662e 656e 7669 726f  y in self.enviro
-0000cc40: 6e6d 656e 7473 2e63 6f6c 756d 6e73 3a0a  nments.columns:.
-0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc60: 656e 765f 6b77 6172 6773 5b6b 6579 5d20  env_kwargs[key] 
-0000cc70: 3d20 6172 670a 2020 2020 2020 2020 2020  = arg.          
-0000cc80: 2020 656c 6966 206b 6579 2069 6e20 7365    elif key in se
-0000cc90: 6c66 2e6c 6561 726e 6572 732e 636f 6c75  lf.learners.colu
-0000cca0: 6d6e 733a 0a20 2020 2020 2020 2020 2020  mns:.           
-0000ccb0: 2020 2020 206c 726e 5f6b 7761 7267 735b       lrn_kwargs[
-0000ccc0: 6b65 795d 203d 2061 7267 0a20 2020 2020  key] = arg.     
-0000ccd0: 2020 2020 2020 2065 6c69 6620 6b65 7920         elif key 
-0000cce0: 696e 2073 656c 662e 6576 616c 7561 746f  in self.evaluato
-0000ccf0: 7273 2e63 6f6c 756d 6e73 3a0a 2020 2020  rs.columns:.    
-0000cd00: 2020 2020 2020 2020 2020 2020 7661 6c5f              val_
-0000cd10: 6b77 6172 6773 5b6b 6579 5d20 3d20 6172  kwargs[key] = ar
-0000cd20: 670a 2020 2020 2020 2020 2020 2020 656c  g.            el
-0000cd30: 6966 206b 6579 2069 6e20 7365 6c66 2e69  if key in self.i
-0000cd40: 6e74 6572 6163 7469 6f6e 732e 636f 6c75  nteractions.colu
-0000cd50: 6d6e 733a 0a20 2020 2020 2020 2020 2020  mns:.           
-0000cd60: 2020 2020 2069 6e74 5f6b 7761 7267 735b       int_kwargs[
-0000cd70: 6b65 795d 203d 2061 7267 0a20 2020 2020  key] = arg.     
-0000cd80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000cd90: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000cda0: 7365 2043 6f62 6145 7863 6570 7469 6f6e  se CobaException
-0000cdb0: 2822 416e 2075 6e72 6563 6f67 6e69 7a65  ("An unrecognize
-0000cdc0: 6420 636f 6c75 6d6e 2077 6173 2070 726f  d column was pro
-0000cdd0: 7669 6465 6420 746f 2060 7768 6572 6560  vided to `where`
-0000cde0: 2066 6f72 2066 696c 7465 7269 6e67 2e22   for filtering."
-0000cdf0: 290a 0a20 2020 2020 2020 206f 7574 203d  )..        out =
-0000ce00: 2073 656c 660a 0a20 2020 2020 2020 2069   self..        i
-0000ce10: 6620 656e 765f 6b77 6172 6773 3a20 6f75  f env_kwargs: ou
-0000ce20: 7420 3d20 6f75 742e 6669 6c74 6572 5f65  t = out.filter_e
-0000ce30: 6e76 282a 2a65 6e76 5f6b 7761 7267 7329  nv(**env_kwargs)
-0000ce40: 0a20 2020 2020 2020 2069 6620 6c72 6e5f  .        if lrn_
-0000ce50: 6b77 6172 6773 3a20 6f75 7420 3d20 6f75  kwargs: out = ou
-0000ce60: 742e 6669 6c74 6572 5f6c 726e 282a 2a6c  t.filter_lrn(**l
-0000ce70: 726e 5f6b 7761 7267 7329 0a20 2020 2020  rn_kwargs).     
-0000ce80: 2020 2069 6620 7661 6c5f 6b77 6172 6773     if val_kwargs
-0000ce90: 3a20 6f75 7420 3d20 6f75 742e 6669 6c74  : out = out.filt
-0000cea0: 6572 5f76 616c 282a 2a76 616c 5f6b 7761  er_val(**val_kwa
-0000ceb0: 7267 7329 0a20 2020 2020 2020 2069 6620  rgs).        if 
-0000cec0: 696e 745f 6b77 6172 6773 3a20 6f75 7420  int_kwargs: out 
-0000ced0: 3d20 6f75 742e 6669 6c74 6572 5f69 6e74  = out.filter_int
-0000cee0: 282a 2a69 6e74 5f6b 7761 7267 7329 0a0a  (**int_kwargs)..
-0000cef0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-0000cf00: 7574 0a0a 2020 2020 6465 6620 7261 775f  ut..    def raw_
-0000cf10: 6c65 6172 6e65 7273 2873 656c 662c 0a20  learners(self,. 
-0000cf20: 2020 2020 2020 2078 2020 203a 2055 6e69         x   : Uni
-0000cf30: 6f6e 5b73 7472 2c20 5365 7175 656e 6365  on[str, Sequence
-0000cf40: 5b73 7472 5d5d 203d 2027 696e 6465 7827  [str]] = 'index'
-0000cf50: 2c0a 2020 2020 2020 2020 7920 2020 3a20  ,.        y   : 
-0000cf60: 7374 7220 2020 2020 2020 2020 2020 2020  str             
-0000cf70: 2020 2020 2020 2020 2020 3d20 2772 6577            = 'rew
-0000cf80: 6172 6427 2c0a 2020 2020 2020 2020 6c20  ard',.        l 
-0000cf90: 2020 3a20 556e 696f 6e5b 7374 722c 2053    : Union[str, S
-0000cfa0: 6571 7565 6e63 655b 7374 725d 5d20 3d20  equence[str]] = 
-0000cfb0: 2766 756c 6c5f 6e61 6d65 272c 0a20 2020  'full_name',.   
-0000cfc0: 2020 2020 2070 2020 203a 2055 6e69 6f6e       p   : Union
-0000cfd0: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
-0000cfe0: 7472 5d5d 203d 2027 656e 7669 726f 6e6d  tr]] = 'environm
-0000cff0: 656e 745f 6964 272c 0a20 2020 2020 2020  ent_id',.       
-0000d000: 2073 7061 6e3a 2069 6e74 203d 204e 6f6e   span: int = Non
-0000d010: 6529 202d 3e20 5461 626c 653a 0a20 2020  e) -> Table:.   
-0000d020: 2020 2020 2022 2222 4120 5461 626c 6520       """A Table 
-0000d030: 7769 7468 2074 6865 2072 6177 2064 6174  with the raw dat
-0000d040: 6120 7573 6564 2066 6f72 2070 6c6f 745f  a used for plot_
-0000d050: 6c65 6172 6e65 7273 2e0a 0a20 2020 2020  learners...     
-0000d060: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000d070: 2020 2020 2078 3a20 5468 6520 7661 7269       x: The vari
-0000d080: 6162 6c65 7320 746f 2070 6c6f 7420 6f6e  ables to plot on
-0000d090: 2074 6865 2078 2d61 7869 732e 0a20 2020   the x-axis..   
-0000d0a0: 2020 2020 2020 2020 2079 3a20 5468 6520           y: The 
-0000d0b0: 7661 7269 6162 6c65 2074 6f20 706c 6f74  variable to plot
-0000d0c0: 206f 6e20 7468 6520 792d 6178 6973 2e0a   on the y-axis..
-0000d0d0: 2020 2020 2020 2020 2020 2020 6c3a 2054              l: T
-0000d0e0: 6865 206c 6162 656c 7320 746f 2075 7365  he labels to use
-0000d0f0: 2069 6e20 7468 6520 706c 6f74 206c 6567   in the plot leg
-0000d100: 656e 642e 0a20 2020 2020 2020 2020 2020  end..           
-0000d110: 2070 3a20 5468 6520 7061 6972 696e 6773   p: The pairings
-0000d120: 2074 6f20 7265 7175 6972 6520 6163 726f   to require acro
-0000d130: 7373 2061 6c6c 206c 2e20 4966 204e 6f6e  ss all l. If Non
-0000d140: 6520 6e6f 2070 6169 7269 6e67 2063 6865  e no pairing che
-0000d150: 636b 7320 6172 6520 7065 7266 6f72 6d65  cks are performe
-0000d160: 642e 0a20 2020 2020 2020 2020 2020 2073  d..            s
-0000d170: 7061 6e3a 2054 6865 2073 697a 6520 6f66  pan: The size of
-0000d180: 2074 6865 2072 6f6c 6c69 6e67 2061 7665   the rolling ave
-0000d190: 7261 6765 2028 4e6f 6e65 206d 6561 6e73  rage (None means
-0000d1a0: 2070 726f 6772 6573 7369 7665 206d 6561   progressive mea
-0000d1b0: 6e2e 290a 0a20 2020 2020 2020 2052 6575  n.)..        Reu
-0000d1c0: 7472 6e73 3a0a 2020 2020 2020 2020 2020  trns:.          
-0000d1d0: 2020 4120 5461 626c 6520 7769 7468 2074    A Table with t
-0000d1e0: 6865 2072 6177 2064 6174 6120 7573 6564  he raw data used
-0000d1f0: 2074 6f20 636f 6e73 7472 7563 7420 706c   to construct pl
-0000d200: 6f74 5f6c 6561 726e 6572 732e 0a20 2020  ot_learners..   
-0000d210: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000d220: 2020 6966 2070 3a20 706c 6f74 7461 626c    if p: plottabl
-0000d230: 6520 3d20 7365 6c66 2e5f 706c 6f74 7461  e = self._plotta
-0000d240: 626c 6528 782c 7929 2e5f 6669 6e69 7368  ble(x,y)._finish
-0000d250: 6564 2878 2c79 2c6c 2c70 290a 2020 2020  ed(x,y,l,p).    
-0000d260: 2020 2020 656c 7365 3a20 706c 6f74 7461      else: plotta
-0000d270: 626c 6520 3d20 7365 6c66 2e5f 706c 6f74  ble = self._plot
-0000d280: 7461 626c 6528 782c 7929 0a0a 2020 2020  table(x,y)..    
-0000d290: 2020 2020 726f 7773 203d 2070 6c6f 7474      rows = plott
-0000d2a0: 6162 6c65 2e5f 6772 6f75 7065 645f 7973  able._grouped_ys
-0000d2b0: 286c 2c78 2c79 3d79 2c73 7061 6e3d 7370  (l,x,y=y,span=sp
-0000d2c0: 616e 290a 0a20 2020 2020 2020 2058 7320  an)..        Xs 
-0000d2d0: 3d20 7365 7428 6d61 7028 6974 656d 6765  = set(map(itemge
-0000d2e0: 7474 6572 2831 292c 726f 7773 2929 0a0a  tter(1),rows))..
-0000d2f0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000d300: 2020 2020 2020 2020 2058 7320 3d20 6469           Xs = di
-0000d310: 6374 287a 6970 2873 6f72 7465 6428 5873  ct(zip(sorted(Xs
-0000d320: 292c 636f 756e 7428 2929 290a 2020 2020  ),count())).    
-0000d330: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-0000d340: 2020 2020 2020 2020 5873 203d 2064 6963          Xs = dic
-0000d350: 7428 7a69 7028 736f 7274 6564 2858 732c  t(zip(sorted(Xs,
-0000d360: 6b65 793d 7374 7229 2c63 6f75 6e74 2829  key=str),count()
-0000d370: 2929 0a0a 2020 2020 2020 2020 7472 793a  ))..        try:
-0000d380: 0a20 2020 2020 2020 2020 2020 2072 6f77  .            row
-0000d390: 7320 3d20 736f 7274 6564 2872 6f77 7329  s = sorted(rows)
-0000d3a0: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
-0000d3b0: 0a20 2020 2020 2020 2020 2020 2073 6f72  .            sor
-0000d3c0: 7465 645f 203d 2046 616c 7365 0a20 2020  ted_ = False.   
-0000d3d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000d3e0: 2020 2020 2020 2073 6f72 7465 645f 203d         sorted_ =
-0000d3f0: 2054 7275 650a 0a20 2020 2020 2020 2064   True..        d
-0000d400: 6174 6120 3d20 7b27 7827 3a20 6c69 7374  ata = {'x': list
-0000d410: 2858 732e 6b65 7973 2829 297d 0a20 2020  (Xs.keys())}.   
-0000d420: 2020 2020 2066 6f72 205f 6c2c 2067 726f       for _l, gro
-0000d430: 7570 2069 6e20 6772 6f75 7065 7228 726f  up in grouper(ro
-0000d440: 7773 2c20 6b65 793d 6974 656d 6765 7474  ws, key=itemgett
-0000d450: 6572 2830 292c 2076 616c 3d69 7465 6d67  er(0), val=itemg
-0000d460: 6574 7465 7228 736c 6963 6528 312c 4e6f  etter(slice(1,No
-0000d470: 6e65 2929 2c20 736f 7274 6564 5f3d 736f  ne)), sorted_=so
-0000d480: 7274 6564 5f29 3a0a 2020 2020 2020 2020  rted_):.        
-0000d490: 2020 2020 5920 3d20 5b5b 666c 6f61 7428      Y = [[float(
-0000d4a0: 276e 616e 2729 5d5d 2a6c 656e 2858 7329  'nan')]]*len(Xs)
-0000d4b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000d4c0: 205f 782c 2067 726f 7570 2069 6e20 6772   _x, group in gr
-0000d4d0: 6f75 7065 7228 6772 6f75 702c 206b 6579  ouper(group, key
-0000d4e0: 3d69 7465 6d67 6574 7465 7228 3029 2c20  =itemgetter(0), 
-0000d4f0: 7661 6c3d 6974 656d 6765 7474 6572 2831  val=itemgetter(1
-0000d500: 292c 2073 6f72 7465 645f 3d73 6f72 7465  ), sorted_=sorte
-0000d510: 645f 293a 0a20 2020 2020 2020 2020 2020  d_):.           
-0000d520: 2020 2020 2059 5b58 735b 5f78 5d5d 203d       Y[Xs[_x]] =
-0000d530: 206c 6973 7428 6368 6169 6e2e 6672 6f6d   list(chain.from
-0000d540: 5f69 7465 7261 626c 6528 6772 6f75 7029  _iterable(group)
-0000d550: 290a 2020 2020 2020 2020 2020 2020 6461  ).            da
-0000d560: 7461 5b5f 6c5d 203d 2059 0a20 2020 2020  ta[_l] = Y.     
-0000d570: 2020 2072 6574 7572 6e20 5461 626c 6528     return Table(
-0000d580: 6461 7461 290a 0a20 2020 2064 6566 2072  data)..    def r
-0000d590: 6177 5f63 6f6e 7472 6173 7428 7365 6c66  aw_contrast(self
-0000d5a0: 2c0a 2020 2020 2020 2020 6c31 2020 3a20  ,.        l1  : 
-0000d5b0: 416e 792c 0a20 2020 2020 2020 206c 3220  Any,.        l2 
-0000d5c0: 203a 2041 6e79 2c0a 2020 2020 2020 2020   : Any,.        
-0000d5d0: 7820 2020 3a20 556e 696f 6e5b 7374 722c  x   : Union[str,
-0000d5e0: 2053 6571 7565 6e63 655b 7374 725d 5d20   Sequence[str]] 
-0000d5f0: 3d20 2765 6e76 6972 6f6e 6d65 6e74 5f69  = 'environment_i
-0000d600: 6427 2c0a 2020 2020 2020 2020 7920 2020  d',.        y   
-0000d610: 3a20 7374 7220 2020 2020 2020 2020 2020  : str           
-0000d620: 2020 2020 2020 2020 2020 2020 3d20 2772              = 'r
-0000d630: 6577 6172 6427 2c0a 2020 2020 2020 2020  eward',.        
-0000d640: 6c20 2020 3a20 556e 696f 6e5b 7374 722c  l   : Union[str,
-0000d650: 2053 6571 7565 6e63 655b 7374 725d 5d20   Sequence[str]] 
-0000d660: 3d20 276c 6561 726e 6572 5f69 6427 2c0a  = 'learner_id',.
-0000d670: 2020 2020 2020 2020 7020 2020 3a20 556e          p   : Un
-0000d680: 696f 6e5b 7374 722c 2053 6571 7565 6e63  ion[str, Sequenc
-0000d690: 655b 7374 725d 5d20 3d20 2765 6e76 6972  e[str]] = 'envir
-0000d6a0: 6f6e 6d65 6e74 5f69 6427 2c0a 2020 2020  onment_id',.    
-0000d6b0: 2020 2020 7370 616e 3a20 696e 7420 3d20      span: int = 
-0000d6c0: 4e6f 6e65 2920 2d3e 2054 6162 6c65 3a0a  None) -> Table:.
-0000d6d0: 2020 2020 2020 2020 2222 2241 2054 6162          """A Tab
-0000d6e0: 6c65 2077 6974 6820 7468 6520 7261 7720  le with the raw 
-0000d6f0: 6461 7461 2070 6c6f 745f 636f 6e74 7261  data plot_contra
-0000d700: 7374 2e0a 0a20 2020 2020 2020 2041 7267  st...        Arg
-0000d710: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
-0000d720: 313a 2054 6865 2066 6972 7374 2060 6c60  1: The first `l`
-0000d730: 2076 616c 7565 2074 6f20 636f 6e74 7261   value to contra
-0000d740: 7374 2e0a 2020 2020 2020 2020 2020 2020  st..            
-0000d750: 6c32 3a20 7468 6520 7365 636f 6e64 2060  l2: the second `
-0000d760: 6c60 2076 616c 7565 2074 6f20 636f 6e74  l` value to cont
-0000d770: 7261 7374 2e0a 2020 2020 2020 2020 2020  rast..          
-0000d780: 2020 783a 2054 6865 2076 6172 6961 626c    x: The variabl
-0000d790: 6573 2074 6f20 706c 6f74 206f 6e20 7468  es to plot on th
-0000d7a0: 6520 782d 6178 6973 2e0a 2020 2020 2020  e x-axis..      
-0000d7b0: 2020 2020 2020 793a 2054 6865 2076 6172        y: The var
-0000d7c0: 6961 626c 6520 746f 2070 6c6f 7420 6f6e  iable to plot on
-0000d7d0: 2074 6865 2079 2d61 7869 732e 0a20 2020   the y-axis..   
-0000d7e0: 2020 2020 2020 2020 206c 3a20 5468 6520           l: The 
-0000d7f0: 636f 6c75 6d6e 206e 616d 6573 2074 6861  column names tha
-0000d800: 7420 6c31 2061 6e64 206c 3220 7265 7072  t l1 and l2 repr
-0000d810: 6573 656e 742e 0a20 2020 2020 2020 2020  esent..         
-0000d820: 2020 2070 3a20 5468 6520 7061 6972 696e     p: The pairin
-0000d830: 6773 2074 6f20 7265 7175 6972 6520 6163  gs to require ac
-0000d840: 726f 7373 2061 6c6c 206c 3120 616e 6420  ross all l1 and 
-0000d850: 6c32 2e0a 2020 2020 2020 2020 2020 2020  l2..            
-0000d860: 7370 616e 3a20 5468 6520 7369 7a65 206f  span: The size o
-0000d870: 6620 7468 6520 726f 6c6c 696e 6720 6176  f the rolling av
-0000d880: 6572 6167 6520 284e 6f6e 6520 6d65 616e  erage (None mean
-0000d890: 7320 7072 6f67 7265 7373 6976 6520 6d65  s progressive me
-0000d8a0: 616e 292e 0a0a 2020 2020 2020 2020 4578  an)...        Ex
-0000d8b0: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-0000d8c0: 2020 2020 7261 775f 636f 6e74 7261 7374      raw_contrast
-0000d8d0: 2831 2c32 2c78 3d27 656e 7669 726f 6e6d  (1,2,x='environm
-0000d8e0: 656e 745f 6964 272c 793d 2772 6577 6172  ent_id',y='rewar
-0000d8f0: 6427 2c6c 3d27 6c65 6172 6e65 725f 6964  d',l='learner_id
-0000d900: 272c 703d 2765 6e76 6972 6f6e 6d65 6e74  ',p='environment
-0000d910: 5f69 6427 290a 2020 2020 2020 2020 2020  _id').          
-0000d920: 2020 776f 756c 6420 636f 6e74 7261 7374    would contrast
-0000d930: 206c 6561 726e 6572 5f69 643d 3120 616e   learner_id=1 an
-0000d940: 6420 6c65 6172 6e65 725f 6964 3d32 2069  d learner_id=2 i
-0000d950: 6e20 7465 726d 7320 6f66 2072 6577 6172  n terms of rewar
-0000d960: 6420 6f6e 2061 6c6c 2065 6e76 6972 6f6e  d on all environ
-0000d970: 6d65 6e74 5f69 6473 2e0a 0a20 2020 2020  ment_ids...     
-0000d980: 2020 2052 6575 7472 6e73 3a0a 2020 2020     Reutrns:.    
-0000d990: 2020 2020 2020 2020 4120 5461 626c 6520          A Table 
-0000d9a0: 7769 7468 2074 6865 2072 6177 2064 6174  with the raw dat
-0000d9b0: 6120 7573 6564 2074 6f20 636f 6e73 7472  a used to constr
-0000d9c0: 7563 7420 706c 6f74 5f63 6f6e 7472 6173  uct plot_contras
-0000d9d0: 742e 0a20 2020 2020 2020 2022 2222 0a0a  t..        """..
-0000d9e0: 2020 2020 2020 2020 6f67 5f6c 203d 2028          og_l = (
-0000d9f0: 6c31 2c6c 3229 0a0a 2020 2020 2020 2020  l1,l2)..        
-0000da00: 6c69 7374 5f6c 696b 653d 286c 6973 742c  list_like=(list,
-0000da10: 7475 706c 6529 0a0a 2020 2020 2020 2020  tuple)..        
-0000da20: 6966 2020 2020 2069 7369 6e73 7461 6e63  if     isinstanc
-0000da30: 6528 6c2c 6c69 7374 5f6c 696b 6529 2061  e(l,list_like) a
-0000da40: 6e64 206e 6f74 2069 7369 6e73 7461 6e63  nd not isinstanc
-0000da50: 6528 6c31 5b30 5d2c 6c69 7374 5f6c 696b  e(l1[0],list_lik
-0000da60: 6529 3a20 6c31 203d 205b 6c31 5d0a 2020  e): l1 = [l1].  
-0000da70: 2020 2020 2020 6966 2020 2020 2069 7369        if     isi
-0000da80: 6e73 7461 6e63 6528 6c2c 6c69 7374 5f6c  nstance(l,list_l
-0000da90: 696b 6529 2061 6e64 206e 6f74 2069 7369  ike) and not isi
-0000daa0: 6e73 7461 6e63 6528 6c32 5b30 5d2c 6c69  nstance(l2[0],li
-0000dab0: 7374 5f6c 696b 6529 3a20 6c32 203d 205b  st_like): l2 = [
-0000dac0: 6c32 5d0a 2020 2020 2020 2020 6966 206e  l2].        if n
-0000dad0: 6f74 2069 7369 6e73 7461 6e63 6528 6c2c  ot isinstance(l,
-0000dae0: 6c69 7374 5f6c 696b 6529 2061 6e64 206e  list_like) and n
-0000daf0: 6f74 2069 7369 6e73 7461 6e63 6528 6c31  ot isinstance(l1
-0000db00: 2020 202c 6c69 7374 5f6c 696b 6529 3a20     ,list_like): 
-0000db10: 6c31 203d 205b 6c31 5d0a 2020 2020 2020  l1 = [l1].      
-0000db20: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-0000db30: 6e63 6528 6c2c 6c69 7374 5f6c 696b 6529  nce(l,list_like)
-0000db40: 2061 6e64 206e 6f74 2069 7369 6e73 7461   and not isinsta
-0000db50: 6e63 6528 6c32 2020 202c 6c69 7374 5f6c  nce(l2   ,list_l
-0000db60: 696b 6529 3a20 6c32 203d 205b 6c32 5d0a  ike): l2 = [l2].
-0000db70: 0a20 2020 2020 2020 2069 6620 616e 7928  .        if any(
-0000db80: 5f6c 3120 696e 206c 3220 666f 7220 5f6c  _l1 in l2 for _l
-0000db90: 3120 696e 206c 3129 3a0a 2020 2020 2020  1 in l1):.      
-0000dba0: 2020 2020 2020 7261 6973 6520 436f 6261        raise Coba
-0000dbb0: 4578 6365 7074 696f 6e28 2241 2076 616c  Exception("A val
-0000dbc0: 7565 2063 616e 6e6f 7420 6265 2069 6e20  ue cannot be in 
-0000dbd0: 626f 7468 2060 6c31 6020 616e 6420 606c  both `l1` and `l
-0000dbe0: 3260 2e20 506c 6561 7365 206d 616b 6520  2`. Please make 
-0000dbf0: 6120 6368 616e 6765 2061 6e64 2072 756e  a change and run
-0000dc00: 2069 7420 6167 6169 6e2e 2229 0a0a 2020   it again.")..  
-0000dc10: 2020 2020 2020 706c 6f74 7461 626c 6520        plottable 
-0000dc20: 3d20 7365 6c66 2e5f 706c 6f74 7461 626c  = self._plottabl
-0000dc30: 6528 782c 7929 0a0a 2020 2020 2020 2020  e(x,y)..        
-0000dc40: 4c31 2c4c 3220 3d20 5b5d 2c5b 5d0a 2020  L1,L2 = [],[].  
-0000dc50: 2020 2020 2020 666f 7220 4c20 696e 2063        for L in c
-0000dc60: 6861 696e 286c 312c 6c32 293a 0a20 2020  hain(l1,l2):.   
-0000dc70: 2020 2020 2020 2020 2073 7562 706c 6f74           subplot
-0000dc80: 203d 2070 6c6f 7474 6162 6c65 0a20 2020   = plottable.   
-0000dc90: 2020 2020 2020 2020 2077 6865 7265 7320           wheres 
-0000dca0: 3d20 5b20 286c 2c4c 2920 5d20 6966 2069  = [ (l,L) ] if i
-0000dcb0: 7369 6e73 7461 6e63 6528 6c2c 7374 7229  sinstance(l,str)
-0000dcc0: 2065 6c73 6520 7a69 7028 6c2c 4c29 0a0a   else zip(l,L)..
-0000dcd0: 2020 2020 2020 2020 2020 2020 6f6c 645f              old_
-0000dce0: 6c6f 6767 6572 203d 2043 6f62 6143 6f6e  logger = CobaCon
-0000dcf0: 7465 7874 2e6c 6f67 6765 720a 2020 2020  text.logger.    
-0000dd00: 2020 2020 2020 2020 436f 6261 436f 6e74          CobaCont
-0000dd10: 6578 742e 6c6f 6767 6572 203d 204e 756c  ext.logger = Nul
-0000dd20: 6c4c 6f67 6765 7228 290a 2020 2020 2020  lLogger().      
-0000dd30: 2020 2020 2020 666f 7220 6c5f 2c76 5f20        for l_,v_ 
-0000dd40: 696e 2077 6865 7265 733a 2073 7562 706c  in wheres: subpl
-0000dd50: 6f74 203d 2073 7562 706c 6f74 2e77 6865  ot = subplot.whe
-0000dd60: 7265 282a 2a7b 6c5f 3a76 5f7d 290a 2020  re(**{l_:v_}).  
-0000dd70: 2020 2020 2020 2020 2020 436f 6261 436f            CobaCo
-0000dd80: 6e74 6578 742e 6c6f 6767 6572 203d 206f  ntext.logger = o
-0000dd90: 6c64 5f6c 6f67 6765 720a 0a20 2020 2020  ld_logger..     
-0000dda0: 2020 2020 2020 2023 7765 2061 7265 2061         #we are a
-0000ddb0: 7373 756d 696e 6720 6174 2074 6869 7320  ssuming at this 
-0000ddc0: 706f 696e 7420 7468 6174 206f 6e6c 7920  point that only 
-0000ddd0: 7661 6c69 640a 2020 2020 2020 2020 2020  valid.          
-0000dde0: 2020 2360 6c60 2061 7265 206c 6566 7420    #`l` are left 
-0000ddf0: 7768 6963 6820 6973 6e27 7420 6e65 6365  which isn't nece
-0000de00: 7373 6172 696c 7920 7468 6520 6361 7365  ssarily the case
-0000de10: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-0000de20: 7565 7320 3d20 7375 6270 6c6f 742e 5f67  ues = subplot._g
-0000de30: 726f 7570 6564 5f79 7328 702c 782c 793d  rouped_ys(p,x,y=
-0000de40: 792c 6361 7264 3d27 5327 2c73 7061 6e3d  y,card='S',span=
-0000de50: 7370 616e 290a 0a20 2020 2020 2020 2020  span)..         
-0000de60: 2020 2069 6620 4c20 696e 206c 313a 204c     if L in l1: L
-0000de70: 312e 6578 7465 6e64 2876 616c 7565 7329  1.extend(values)
-0000de80: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000de90: 6520 2020 2020 203a 204c 322e 6578 7465  e      : L2.exte
-0000dea0: 6e64 2876 616c 7565 7329 0a0a 2020 2020  nd(values)..    
-0000deb0: 2020 2020 2357 6520 6861 7665 2074 6f20      #We have to 
-0000dec0: 6d61 7465 7269 616c 697a 6520 6265 6361  materialize beca
-0000ded0: 7573 6520 7765 2063 616e 2774 2072 656c  use we can't rel
-0000dee0: 7920 6f6e 2073 6f72 7469 6e67 0a20 2020  y on sorting.   
-0000def0: 2020 2020 2050 3120 3d20 7b6b 3a6c 6973       P1 = {k:lis
-0000df00: 7428 7629 2066 6f72 206b 2c76 2069 6e20  t(v) for k,v in 
-0000df10: 6772 6f75 7065 7228 4c31 2c6b 6579 3d69  grouper(L1,key=i
-0000df20: 7465 6d67 6574 7465 7228 3029 297d 0a20  temgetter(0))}. 
-0000df30: 2020 2020 2020 2050 3220 3d20 7b6b 3a6c         P2 = {k:l
-0000df40: 6973 7428 7629 2066 6f72 206b 2c76 2069  ist(v) for k,v i
-0000df50: 6e20 6772 6f75 7065 7228 4c32 2c6b 6579  n grouper(L2,key
-0000df60: 3d69 7465 6d67 6574 7465 7228 3029 297d  =itemgetter(0))}
-0000df70: 0a0a 2020 2020 2020 2020 6465 6620 6d61  ..        def ma
-0000df80: 6b65 7828 7831 2c78 3229 3a20 7265 7475  kex(x1,x2): retu
-0000df90: 726e 2078 3120 6966 2078 3120 3d3d 2078  rn x1 if x1 == x
-0000dfa0: 3220 656c 7365 2066 227b 7832 7d2d 7b78  2 else f"{x2}-{x
-0000dfb0: 317d 220a 0a20 2020 2020 2020 2058 5920  1}"..        XY 
-0000dfc0: 3d20 6465 6661 756c 7464 6963 7428 6c69  = defaultdict(li
-0000dfd0: 7374 290a 2020 2020 2020 2020 666f 7220  st).        for 
-0000dfe0: 6b20 696e 2050 312e 6b65 7973 2829 2026  k in P1.keys() &
-0000dff0: 2050 322e 6b65 7973 2829 3a0a 2020 2020   P2.keys():.    
-0000e000: 2020 2020 2020 2020 6966 2078 203d 3d20          if x == 
-0000e010: 2769 6e64 6578 273a 0a20 2020 2020 2020  'index':.       
-0000e020: 2020 2020 2020 2020 2066 6f72 2067 315f           for g1_
-0000e030: 2c20 6732 5f20 696e 207a 6970 2850 315b  , g2_ in zip(P1[
-0000e040: 6b5d 2c50 325b 6b5d 293a 0a20 2020 2020  k],P2[k]):.     
-0000e050: 2020 2020 2020 2020 2020 2020 2020 2058                 X
-0000e060: 595b 6731 5f5b 315d 5d2e 6170 7065 6e64  Y[g1_[1]].append
-0000e070: 2828 6731 5f5b 325d 2c67 325f 5b32 5d29  ((g1_[2],g2_[2])
-0000e080: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0000e090: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000e0a0: 2020 2020 666f 7220 6731 5f2c 6732 5f20      for g1_,g2_ 
-0000e0b0: 696e 2070 726f 6475 6374 2850 315b 6b5d  in product(P1[k]
-0000e0c0: 2c50 325b 6b5d 293a 0a20 2020 2020 2020  ,P2[k]):.       
-0000e0d0: 2020 2020 2020 2020 2020 2020 2058 595b               XY[
-0000e0e0: 6d61 6b65 7828 6731 5f5b 315d 2c67 325f  makex(g1_[1],g2_
-0000e0f0: 5b31 5d29 5d2e 6170 7065 6e64 2828 6731  [1])].append((g1
-0000e100: 5f5b 325d 2c67 325f 5b32 5d29 290a 0a20  _[2],g2_[2])).. 
-0000e110: 2020 2020 2020 2069 6620 6e6f 7420 5859         if not XY
-0000e120: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000e130: 6973 6520 436f 6261 4578 6365 7074 696f  ise CobaExceptio
-0000e140: 6e28 6622 5765 2077 6572 6520 756e 6162  n(f"We were unab
-0000e150: 6c65 2074 6f20 6372 6561 7465 2061 6e79  le to create any
-0000e160: 2070 6169 7269 6e67 7320 746f 2063 6f6e   pairings to con
-0000e170: 7472 6173 742e 204d 616b 6520 7375 7265  trast. Make sure
-0000e180: 206c 313d 7b6f 675f 6c5b 305d 7d20 616e   l1={og_l[0]} an
-0000e190: 6420 6c32 3d7b 6f67 5f6c 5b31 5d7d 2069  d l2={og_l[1]} i
-0000e1a0: 7320 636f 7272 6563 742e 2229 0a0a 2020  s correct.")..  
-0000e1b0: 2020 2020 2020 6c31 5f6c 6162 656c 203d        l1_label =
-0000e1c0: 2073 656c 662e 5f6c 726e 5f63 6163 6865   self._lrn_cache
-0000e1d0: 5b6c 315b 305d 5d5b 2766 756c 6c5f 6e61  [l1[0]]['full_na
-0000e1e0: 6d65 275d 2069 6620 6c3d 3d27 6c65 6172  me'] if l=='lear
-0000e1f0: 6e65 725f 6964 2720 656c 7365 2027 6c31  ner_id' else 'l1
-0000e200: 270a 2020 2020 2020 2020 6c32 5f6c 6162  '.        l2_lab
-0000e210: 656c 203d 2073 656c 662e 5f6c 726e 5f63  el = self._lrn_c
-0000e220: 6163 6865 5b6c 325b 305d 5d5b 2766 756c  ache[l2[0]]['ful
-0000e230: 6c5f 6e61 6d65 275d 2069 6620 6c3d 3d27  l_name'] if l=='
-0000e240: 6c65 6172 6e65 725f 6964 2720 656c 7365  learner_id' else
-0000e250: 2027 6c32 270a 0a20 2020 2020 2020 2058   'l2'..        X
-0000e260: 2c59 203d 207a 6970 282a 736f 7274 6564  ,Y = zip(*sorted
-0000e270: 2858 592e 6974 656d 7328 2929 290a 0a20  (XY.items())).. 
-0000e280: 2020 2020 2020 2072 6574 7572 6e20 5461         return Ta
-0000e290: 626c 6528 7b27 7827 3a20 582c 2028 6c31  ble({'x': X, (l1
-0000e2a0: 5f6c 6162 656c 2c6c 325f 6c61 6265 6c29  _label,l2_label)
-0000e2b0: 3a20 5920 7d29 0a0a 2020 2020 6465 6620  : Y })..    def 
-0000e2c0: 706c 6f74 5f6c 6561 726e 6572 7328 7365  plot_learners(se
-0000e2d0: 6c66 2c0a 2020 2020 2020 2020 7820 2020  lf,.        x   
-0000e2e0: 2020 2020 3a20 556e 696f 6e5b 7374 722c      : Union[str,
-0000e2f0: 2053 6571 7565 6e63 655b 7374 725d 5d20   Sequence[str]] 
-0000e300: 3d20 2769 6e64 6578 272c 0a20 2020 2020  = 'index',.     
-0000e310: 2020 2079 2020 2020 2020 203a 2073 7472     y       : str
-0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e330: 2020 2020 2020 203d 2027 7265 7761 7264         = 'reward
-0000e340: 272c 0a20 2020 2020 2020 206c 2020 2020  ',.        l    
-0000e350: 2020 203a 2055 6e69 6f6e 5b73 7472 2c20     : Union[str, 
-0000e360: 5365 7175 656e 6365 5b73 7472 5d5d 203d  Sequence[str]] =
-0000e370: 2027 6675 6c6c 5f6e 616d 6527 2c0a 2020   'full_name',.  
-0000e380: 2020 2020 2020 7020 2020 2020 2020 3a20        p       : 
-0000e390: 556e 696f 6e5b 7374 722c 2053 6571 7565  Union[str, Seque
-0000e3a0: 6e63 655b 7374 725d 5d20 3d20 2765 6e76  nce[str]] = 'env
-0000e3b0: 6972 6f6e 6d65 6e74 5f69 6427 2c0a 2020  ironment_id',.  
-0000e3c0: 2020 2020 2020 7370 616e 2020 2020 3a20        span    : 
-0000e3d0: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-0000e3e0: 2020 2020 6572 7220 2020 2020 3a20 556e      err     : Un
-0000e3f0: 696f 6e5b 4c69 7465 7261 6c5b 2773 6527  ion[Literal['se'
-0000e400: 2c27 7364 272c 2762 7327 2c27 6269 275d  ,'sd','bs','bi']
-0000e410: 2c20 506f 696e 7441 6e64 496e 7465 7276  , PointAndInterv
-0000e420: 616c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  al] = None,.    
-0000e430: 2020 2020 6572 7265 7665 7279 3a20 696e      errevery: in
-0000e440: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-0000e450: 2020 6c61 6265 6c73 2020 3a20 5365 7175    labels  : Sequ
-0000e460: 656e 6365 5b73 7472 5d20 3d20 4e6f 6e65  ence[str] = None
-0000e470: 2c0a 2020 2020 2020 2020 636f 6c6f 7273  ,.        colors
-0000e480: 2020 3a20 556e 696f 6e5b 696e 742c 5365    : Union[int,Se
-0000e490: 7175 656e 6365 5b55 6e69 6f6e 5b73 7472  quence[Union[str
-0000e4a0: 2c69 6e74 5d5d 5d20 3d20 4e6f 6e65 2c0a  ,int]]] = None,.
-0000e4b0: 2020 2020 2020 2020 7469 746c 6520 2020          title   
-0000e4c0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-0000e4d0: 2020 2020 2020 786c 6162 656c 2020 3a20        xlabel  : 
-0000e4e0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0000e4f0: 2020 2020 796c 6162 656c 2020 3a20 7374      ylabel  : st
-0000e500: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-0000e510: 2020 786c 696d 2020 2020 3a20 5475 706c    xlim    : Tupl
-0000e520: 655b 4f70 7469 6f6e 616c 5b4e 756d 6265  e[Optional[Numbe
-0000e530: 725d 2c4f 7074 696f 6e61 6c5b 4e75 6d62  r],Optional[Numb
-0000e540: 6572 5d5d 203d 204e 6f6e 652c 0a20 2020  er]] = None,.   
-0000e550: 2020 2020 2079 6c69 6d20 2020 203a 2054       ylim    : T
-0000e560: 7570 6c65 5b4f 7074 696f 6e61 6c5b 4e75  uple[Optional[Nu
-0000e570: 6d62 6572 5d2c 4f70 7469 6f6e 616c 5b4e  mber],Optional[N
-0000e580: 756d 6265 725d 5d20 3d20 4e6f 6e65 2c0a  umber]] = None,.
-0000e590: 2020 2020 2020 2020 7874 6963 6b73 2020          xticks  
-0000e5a0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
-0000e5b0: 2020 2020 2020 2079 7469 636b 7320 203a         yticks  :
-0000e5c0: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
-0000e5d0: 2020 2020 2020 6c65 6765 6e64 2020 3a20        legend  : 
-0000e5e0: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-0000e5f0: 2020 2020 2061 6c70 6861 2020 203a 2066       alpha   : f
-0000e600: 6c6f 6174 203d 2031 2c0a 2020 2020 2020  loat = 1,.      
-0000e610: 2020 786f 7264 6572 2020 3a20 4c69 7465    xorder  : Lite
-0000e620: 7261 6c5b 272b 272c 272d 275d 203d 204e  ral['+','-'] = N
-0000e630: 6f6e 652c 0a20 2020 2020 2020 2074 6f70  one,.        top
-0000e640: 5f6e 2020 203a 2069 6e74 203d 204e 6f6e  _n   : int = Non
-0000e650: 652c 0a20 2020 2020 2020 206f 7574 2020  e,.        out  
-0000e660: 2020 203a 2055 6e69 6f6e 5b4e 6f6e 652c     : Union[None,
-0000e670: 4c69 7465 7261 6c5b 2773 6372 6565 6e27  Literal['screen'
-0000e680: 5d2c 7374 725d 203d 2027 7363 7265 656e  ],str] = 'screen
-0000e690: 272c 0a20 2020 2020 2020 2061 7820 3d20  ',.        ax = 
-0000e6a0: 4e6f 6e65 2920 2d3e 204e 6f6e 653a 0a20  None) -> None:. 
-0000e6b0: 2020 2020 2020 2022 2222 506c 6f74 2074         """Plot t
-0000e6c0: 6865 2070 6572 666f 726d 616e 6365 206f  he performance o
-0000e6d0: 6620 6d75 6c74 6970 6c65 206c 6561 726e  f multiple learn
-0000e6e0: 6572 7320 6f6e 206d 756c 7469 706c 6520  ers on multiple 
-0000e6f0: 656e 7669 726f 6e6d 656e 7473 2e20 4974  environments. It
-0000e700: 2067 6976 6573 2061 2073 656e 7365 206f   gives a sense o
-0000e710: 6620 7468 650a 2020 2020 2020 2020 6578  f the.        ex
-0000e720: 7065 6374 6564 2070 6572 666f 726d 616e  pected performan
-0000e730: 6365 2066 6f72 2064 6966 6665 7265 6e74  ce for different
-0000e740: 206c 6561 726e 6572 7320 6163 726f 7373   learners across
-0000e750: 2069 6e64 6570 656e 6465 6e74 2065 6e76   independent env
-0000e760: 6972 6f6e 6d65 6e74 732e 2054 6869 7320  ironments. This 
-0000e770: 706c 6f74 2069 730a 2020 2020 2020 2020  plot is.        
-0000e780: 7661 6c75 6162 6c65 2069 6e20 6761 696e  valuable in gain
-0000e790: 696e 6720 696e 7369 6768 7420 696e 746f  ing insight into
-0000e7a0: 2068 6f77 2076 6172 696f 7573 206c 6561   how various lea
-0000e7b0: 726e 6572 7320 7065 7266 6f72 6d20 696e  rners perform in
-0000e7c0: 2063 6f6d 7061 7269 736f 6e20 746f 206f   comparison to o
-0000e7d0: 6e65 2061 6e6f 7468 6572 2e0a 0a20 2020  ne another...   
-0000e7e0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000e7f0: 2020 2020 2020 2078 3a20 5468 6520 7661         x: The va
-0000e800: 6c75 6573 2074 6f20 706c 6f74 206f 6e20  lues to plot on 
-0000e810: 7468 6520 782d 6178 6973 2e0a 2020 2020  the x-axis..    
-0000e820: 2020 2020 2020 2020 793a 2054 6865 2076          y: The v
-0000e830: 616c 7565 2074 6f20 706c 6f74 206f 6e20  alue to plot on 
-0000e840: 7468 6520 792d 6178 6973 2e0a 2020 2020  the y-axis..    
-0000e850: 2020 2020 2020 2020 6c3a 2054 6865 2076          l: The v
-0000e860: 616c 7565 7320 746f 2070 6c6f 7420 696e  alues to plot in
-0000e870: 2074 6865 206c 6567 656e 642e 0a20 2020   the legend..   
-0000e880: 2020 2020 2020 2020 2070 3a20 5468 6520           p: The 
-0000e890: 7061 6972 7320 7468 6174 206d 7573 7420  pairs that must 
-0000e8a0: 6578 6973 7420 6163 726f 7373 2061 6c6c  exist across all
-0000e8b0: 2069 7465 6d73 2069 6e20 7468 6520 6c65   items in the le
-0000e8c0: 6765 6e64 2069 6e20 6f72 6465 7220 746f  gend in order to
-0000e8d0: 2062 6520 696e 636c 7564 6564 2e0a 2020   be included..  
-0000e8e0: 2020 2020 2020 2020 2020 2020 2020 4966                If
-0000e8f0: 204e 6f6e 6520 6e6f 2070 6169 7269 6e67   None no pairing
-0000e900: 2020 6368 6563 6b73 2061 7265 2070 6572    checks are per
-0000e910: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
-0000e920: 2020 2020 7370 616e 3a20 5468 6520 6e75      span: The nu
-0000e930: 6d62 6572 206f 6620 7920 7661 6c75 6573  mber of y values
-0000e940: 2074 6f20 736d 6f6f 7468 2074 6f67 6574   to smooth toget
-0000e950: 6865 7220 7768 656e 2072 6570 6f72 7469  her when reporti
-0000e960: 6e67 2079 2e20 4966 2074 6869 7320 6973  ng y. If this is
-0000e970: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0000e980: 2020 2020 2020 7468 656e 2074 6865 2061        then the a
-0000e990: 7665 7261 6765 206f 6620 616c 6c20 7920  verage of all y 
-0000e9a0: 7661 6c75 6573 2075 7020 746f 2063 7572  values up to cur
-0000e9b0: 7265 6e74 2069 7320 7368 6f77 6e20 6f74  rent is shown ot
-0000e9c0: 6865 7277 6973 6520 6120 6d6f 7669 6e67  herwise a moving
-0000e9d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e9e0: 2061 7665 7261 6765 2077 6974 6820 7769   average with wi
-0000e9f0: 6e64 6f77 2073 697a 6520 6f66 2073 7061  ndow size of spa
-0000ea00: 6e20 2874 6865 2077 696e 646f 7720 7769  n (the window wi
-0000ea10: 6c6c 2062 6520 736d 616c 6c65 7220 7468  ll be smaller th
-0000ea20: 616e 2073 7061 6e20 696e 6974 6961 6c6c  an span initiall
-0000ea30: 7929 2e0a 2020 2020 2020 2020 2020 2020  y)..            
-0000ea40: 6572 723a 2054 6869 7320 6465 7465 726d  err: This determ
-0000ea50: 696e 6573 2077 6861 7420 6b69 6e64 206f  ines what kind o
-0000ea60: 6620 6572 726f 7220 6261 7273 2074 6f20  f error bars to 
-0000ea70: 706c 6f74 2028 6966 2061 6e79 292e 2049  plot (if any). I
-0000ea80: 6620 604e 6f6e 6560 2074 6865 6e20 6e6f  f `None` then no
-0000ea90: 2062 6172 730a 2020 2020 2020 2020 2020   bars.          
-0000eaa0: 2020 2020 2020 6172 6520 706c 6f74 7465        are plotte
-0000eab0: 642c 2069 6620 2773 6527 2074 6865 2073  d, if 'se' the s
-0000eac0: 7461 6e64 6172 6420 6572 726f 7220 6973  tandard error is
-0000ead0: 2073 686f 776e 2c20 616e 6420 6966 2027   shown, and if '
-0000eae0: 7364 2720 7468 6520 7374 616e 6461 7264  sd' the standard
-0000eaf0: 2064 6576 6961 7469 6f6e 0a20 2020 2020   deviation.     
-0000eb00: 2020 2020 2020 2020 2020 2069 7320 7368             is sh
-0000eb10: 6f77 6e2e 0a20 2020 2020 2020 2020 2020  own..           
-0000eb20: 2065 7272 6576 6572 793a 2054 6869 7320   errevery: This 
-0000eb30: 6465 7465 726d 696e 6573 2074 6865 2066  determines the f
-0000eb40: 7265 7175 656e 6379 206f 6620 6572 726f  requency of erro
-0000eb50: 7262 6172 732e 2049 6620 604e 6f6e 6560  rbars. If `None`
-0000eb60: 2074 6865 7920 6170 7065 6172 2035 2520   they appear 5% 
-0000eb70: 6f66 2074 6865 0a20 2020 2020 2020 2020  of the.         
-0000eb80: 2020 2020 2020 2074 696d 652e 0a20 2020         time..   
-0000eb90: 2020 2020 2020 2020 206c 6162 656c 733a           labels:
-0000eba0: 2054 6865 206c 6567 656e 6420 6c61 6265   The legend labe
-0000ebb0: 6c73 2074 6f20 7573 6520 696e 2074 6865  ls to use in the
-0000ebc0: 2070 6c6f 742e 2054 6865 7365 2073 686f   plot. These sho
-0000ebd0: 756c 6420 6265 2069 6e20 6f72 6465 7220  uld be in order 
-0000ebe0: 6f66 2074 6865 2061 6374 7561 6c0a 2020  of the actual.  
-0000ebf0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-0000ec00: 6765 6e64 206c 6162 656c 732e 0a20 2020  gend labels..   
-0000ec10: 2020 2020 2020 2020 2063 6f6c 6f72 733a           colors:
-0000ec20: 2054 6865 2063 6f6c 6f72 7320 7573 6564   The colors used
-0000ec30: 2074 6f20 706c 6f74 2074 6865 206c 6561   to plot the lea
-0000ec40: 726e 6572 7320 706c 6f74 2e0a 2020 2020  rners plot..    
-0000ec50: 2020 2020 2020 2020 7469 746c 6520 3a20          title : 
-0000ec60: 5468 6520 7469 746c 6520 6769 7665 2074  The title give t
-0000ec70: 6865 2070 6c6f 742e 0a20 2020 2020 2020  he plot..       
-0000ec80: 2020 2020 2078 6c61 6265 6c3a 2054 6865       xlabel: The
-0000ec90: 206c 6162 656c 206f 6e20 7468 6520 782d   label on the x-
-0000eca0: 6178 6973 2e0a 2020 2020 2020 2020 2020  axis..          
-0000ecb0: 2020 796c 6162 656c 3a20 5468 6520 6c61    ylabel: The la
-0000ecc0: 6265 6c20 6f6e 2074 6865 2079 2d61 7869  bel on the y-axi
-0000ecd0: 732e 0a20 2020 2020 2020 2020 2020 2078  s..            x
-0000ece0: 6c69 6d3a 2044 6566 696e 6520 7468 6520  lim: Define the 
-0000ecf0: 782d 6178 6973 206c 696d 6974 7320 746f  x-axis limits to
-0000ed00: 2070 6c6f 742e 2049 6620 604e 6f6e 6560   plot. If `None`
-0000ed10: 2074 6865 2078 2d61 7869 7320 6c69 6d69   the x-axis limi
-0000ed20: 7473 2077 696c 6c20 6265 2069 6e66 6572  ts will be infer
-0000ed30: 7265 642e 0a20 2020 2020 2020 2020 2020  red..           
-0000ed40: 2079 6c69 6d3a 2044 6566 696e 6520 7468   ylim: Define th
-0000ed50: 6520 792d 6178 6973 206c 696d 6974 7320  e y-axis limits 
-0000ed60: 746f 2070 6c6f 742e 2049 6620 604e 6f6e  to plot. If `Non
-0000ed70: 6560 2074 6865 2079 2d61 7869 7320 6c69  e` the y-axis li
-0000ed80: 6d69 7473 2077 696c 6c20 6265 2069 6e66  mits will be inf
-0000ed90: 6572 7265 642e 0a20 2020 2020 2020 2020  erred..         
-0000eda0: 2020 2078 7469 636b 733a 2057 6865 7468     xticks: Wheth
-0000edb0: 6572 2074 6865 2078 2d61 7869 7320 6c61  er the x-axis la
-0000edc0: 6265 6c73 2073 686f 756c 6420 6265 2064  bels should be d
-0000edd0: 7261 776e 2e0a 2020 2020 2020 2020 2020  rawn..          
-0000ede0: 2020 7974 6963 6b73 3a20 5768 6574 6865    yticks: Whethe
-0000edf0: 7220 7468 6520 792d 6178 6973 206c 6162  r the y-axis lab
-0000ee00: 656c 7320 7368 6f75 6c64 2062 6520 6472  els should be dr
-0000ee10: 6177 6e2e 0a20 2020 2020 2020 2020 2020  awn..           
-0000ee20: 206c 6567 656e 643a 2057 6865 7468 6572   legend: Whether
-0000ee30: 2074 6865 206c 6567 656e 6420 666f 7220   the legend for 
-0000ee40: 7468 6520 706c 6f74 2073 686f 756c 6420  the plot should 
-0000ee50: 6265 2064 7261 776e 2e0a 2020 2020 2020  be drawn..      
-0000ee60: 2020 2020 2020 616c 7068 613a 2054 6865        alpha: The
-0000ee70: 206f 7061 6369 7479 206f 6620 6472 6177   opacity of draw
-0000ee80: 6e20 6461 7461 2e0a 2020 2020 2020 2020  n data..        
-0000ee90: 2020 2020 786f 7264 6572 3a20 496e 6469      xorder: Indi
-0000eea0: 6361 7465 7320 7768 6574 6865 7220 7468  cates whether th
-0000eeb0: 6520 782d 6178 6973 2073 686f 756c 6420  e x-axis should 
-0000eec0: 6265 2069 6e20 6173 6365 6e64 696e 6720  be in ascending 
-0000eed0: 282b 2920 6f72 2064 6573 6365 6e64 6569  (+) or descendei
-0000eee0: 6e67 2028 2d29 206f 7264 6572 2e0a 2020  ng (-) order..  
-0000eef0: 2020 2020 2020 2020 2020 746f 705f 6e3a            top_n:
-0000ef00: 204f 6e6c 7920 706c 6f74 2074 6865 2074   Only plot the t
-0000ef10: 6f70 5f6e 206c 6561 726e 6572 732e 2049  op_n learners. I
-0000ef20: 6620 604e 6f6e 6560 2061 6c6c 206c 6561  f `None` all lea
-0000ef30: 726e 6572 7320 7769 6c6c 2062 6520 706c  rners will be pl
-0000ef40: 6f74 7465 642e 2049 6620 6e65 6761 7469  otted. If negati
-0000ef50: 7665 0a20 2020 2020 2020 2020 2020 2020  ve.             
-0000ef60: 2020 2074 6865 2062 6f74 746f 6d20 7769     the bottom wi
-0000ef70: 6c6c 2062 6520 706c 6f74 7465 642e 0a20  ll be plotted.. 
-0000ef80: 2020 2020 2020 2020 2020 206f 7574 3a20             out: 
-0000ef90: 496e 6469 6361 7465 2077 6865 7265 2074  Indicate where t
-0000efa0: 6865 2070 6c6f 7420 7368 6f75 6c64 2062  he plot should b
-0000efb0: 6520 7365 6e74 2074 6f20 6166 7465 7220  e sent to after 
-0000efc0: 706c 6f74 7469 6e67 2069 7320 6669 6e69  plotting is fini
-0000efd0: 7368 6564 2e20 5661 6c69 6420 7661 6c75  shed. Valid valu
-0000efe0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-0000eff0: 2020 2061 7265 2027 7363 7265 656e 2720     are 'screen' 
-0000f000: 746f 2073 686f 7720 6974 206f 6e20 7363  to show it on sc
-0000f010: 7265 656e 2c20 6120 7061 7468 2074 6f20  reen, a path to 
-0000f020: 7361 7665 2074 6f20 6469 736b 2c20 6f72  save to disk, or
-0000f030: 204e 6f6e 6520 6966 2074 6865 2070 6c6f   None if the plo
-0000f040: 7420 7368 6f75 6c64 0a20 2020 2020 2020  t should.       
-0000f050: 2020 2020 2020 2020 206e 6f74 2062 6520           not be 
-0000f060: 6f75 7470 7574 2061 6e79 7768 6572 6520  output anywhere 
-0000f070: 2869 2e65 2e2c 206b 6570 7420 696e 206d  (i.e., kept in m
-0000f080: 656d 6f72 7929 2069 6e20 6f72 6465 7220  emory) in order 
-0000f090: 746f 206b 6565 7020 6564 6974 696e 6720  to keep editing 
-0000f0a0: 7468 6520 706c 6f74 2061 6674 6572 0a20  the plot after. 
-0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000f0c0: 6869 7320 6361 6c6c 2e0a 2020 2020 2020  his call..      
-0000f0d0: 2020 2020 2020 6178 3a20 5072 6f76 6964        ax: Provid
-0000f0e0: 6520 616e 206f 7074 696f 6e61 6c20 6178  e an optional ax
-0000f0f0: 6573 2074 6861 7420 7468 6520 706c 6f74  es that the plot
-0000f100: 2077 696c 6c20 6265 2064 7261 776e 2074   will be drawn t
-0000f110: 6f2e 2049 6620 6e6f 7420 7072 6f76 6964  o. If not provid
-0000f120: 6564 2061 206e 6577 0a20 2020 2020 2020  ed a new.       
-0000f130: 2020 2020 2020 2020 2066 6967 7572 652f           figure/
-0000f140: 6178 6573 2069 7320 6372 6561 7465 642e  axes is created.
-0000f150: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000f160: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000f170: 2020 2020 2020 786c 696d 203d 2078 6c69        xlim = xli
-0000f180: 6d20 6f72 205b 4e6f 6e65 2c4e 6f6e 655d  m or [None,None]
-0000f190: 0a20 2020 2020 2020 2020 2020 2079 6c69  .            yli
-0000f1a0: 6d20 3d20 796c 696d 206f 7220 5b4e 6f6e  m = ylim or [Non
-0000f1b0: 652c 4e6f 6e65 5d0a 0a20 2020 2020 2020  e,None]..       
-0000f1c0: 2020 2020 2072 6177 5f64 6174 6120 3d20       raw_data = 
-0000f1d0: 7365 6c66 2e72 6177 5f6c 6561 726e 6572  self.raw_learner
-0000f1e0: 7328 782c 792c 6c2c 702c 7370 616e 290a  s(x,y,l,p,span).
-0000f1f0: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
-0000f200: 6576 6572 7920 3d20 6572 7265 7665 7279  every = errevery
-0000f210: 206f 7220 6d61 7828 696e 7428 7261 775f   or max(int(raw_
-0000f220: 6461 7461 5b27 7827 5d5b 2d31 5d2a 302e  data['x'][-1]*0.
-0000f230: 3035 292c 3129 2069 6620 7820 3d3d 2027  05),1) if x == '
-0000f240: 696e 6465 7827 2065 6c73 6520 310a 2020  index' else 1.  
-0000f250: 2020 2020 2020 2020 2020 7374 796c 6520            style 
-0000f260: 2020 203d 2022 2d22 2069 6620 7820 3d3d     = "-" if x ==
-0000f270: 2027 696e 6465 7827 2065 6c73 6520 222e   'index' else ".
-0000f280: 220a 2020 2020 2020 2020 2020 2020 6572  ".            er
-0000f290: 7220 2020 2020 203d 2073 656c 662e 5f63  r      = self._c
-0000f2a0: 6f6e 6669 6465 6e63 6528 6572 722c 2065  onfidence(err, e
-0000f2b0: 7272 6576 6572 7929 0a0a 2020 2020 2020  rrevery)..      
-0000f2c0: 2020 2020 2020 595f 636f 756e 7420 3d20        Y_count = 
-0000f2d0: 5b5d 0a20 2020 2020 2020 2020 2020 206c  [].            l
-0000f2e0: 696e 6573 3a20 4c69 7374 5b50 6f69 6e74  ines: List[Point
-0000f2f0: 735d 203d 205b 5d0a 2020 2020 2020 2020  s] = [].        
-0000f300: 2020 2020 666f 7220 5f6c 2069 6e20 7261      for _l in ra
-0000f310: 775f 6461 7461 2e63 6f6c 756d 6e73 5b31  w_data.columns[1
-0000f320: 3a5d 3a0a 2020 2020 2020 2020 2020 2020  :]:.            
-0000f330: 2020 2020 636f 6c6f 7220 3d20 7365 6c66      color = self
-0000f340: 2e5f 6765 745f 636f 6c6f 7228 636f 6c6f  ._get_color(colo
-0000f350: 7273 2c20 2020 6c65 6e28 6c69 6e65 7329  rs,   len(lines)
-0000f360: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f370: 2020 6c61 6265 6c20 3d20 7365 6c66 2e5f    label = self._
-0000f380: 6765 745f 6c61 6265 6c28 6c61 6265 6c73  get_label(labels
-0000f390: 2c5f 6c2c 6c65 6e28 6c69 6e65 7329 290a  ,_l,len(lines)).
-0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3b0: 595f 636f 756e 742e 6170 7065 6e64 2830  Y_count.append(0
-0000f3c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f3d0: 2020 6c69 6e65 732e 6170 7065 6e64 2850    lines.append(P
-0000f3e0: 6f69 6e74 7328 7374 796c 653d 7374 796c  oints(style=styl
-0000f3f0: 652c 636f 6c6f 723d 636f 6c6f 722c 6c61  e,color=color,la
-0000f400: 6265 6c3d 6c61 6265 6c2c 616c 7068 613d  bel=label,alpha=
-0000f410: 616c 7068 6129 290a 2020 2020 2020 2020  alpha)).        
-0000f420: 2020 2020 2020 2020 666f 7220 5f78 692c          for _xi,
-0000f430: 2028 5f78 2c20 5929 2069 6e20 656e 756d   (_x, Y) in enum
-0000f440: 6572 6174 6528 7a69 7028 2a72 6177 5f64  erate(zip(*raw_d
-0000f450: 6174 615b 5b27 7827 2c5f 6c5d 5d29 293a  ata[['x',_l]])):
-0000f460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f470: 2020 2020 2059 5f63 6f75 6e74 5b2d 315d       Y_count[-1]
-0000f480: 203d 206d 6178 2859 5f63 6f75 6e74 5b2d   = max(Y_count[-
-0000f490: 315d 2c6c 656e 2859 2929 0a20 2020 2020  1],len(Y)).     
-0000f4a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000f4b0: 696e 6573 5b2d 315d 2e61 6464 285f 7820  ines[-1].add(_x 
-0000f4c0: 6966 205f 7820 6973 206e 6f74 204e 6f6e  if _x is not Non
-0000f4d0: 6520 656c 7365 2027 4e6f 6e65 272c 202a  e else 'None', *
-0000f4e0: 6572 7228 592c 205f 7869 2929 0a0a 2020  err(Y, _xi))..  
-0000f4f0: 2020 2020 2020 2020 2020 6c69 6e65 7320            lines 
-0000f500: 203d 2073 6f72 7465 6428 6c69 6e65 732c   = sorted(lines,
-0000f510: 206b 6579 3d6c 616d 6264 6120 6c69 6e65   key=lambda line
-0000f520: 3a20 6c69 6e65 2e59 5b2d 315d 2c20 7265  : line.Y[-1], re
-0000f530: 7665 7273 653d 5472 7565 290a 2020 2020  verse=True).    
-0000f540: 2020 2020 2020 2020 6c61 6265 6c73 203d          labels =
-0000f550: 205b 6c2e 6c61 6265 6c20 6f72 2073 7472   [l.label or str
-0000f560: 286c 2e6c 6162 656c 2920 666f 7220 6c20  (l.label) for l 
-0000f570: 696e 206c 696e 6573 5d0a 2020 2020 2020  in lines].      
-0000f580: 2020 2020 2020 636f 6c6f 7273 203d 205b        colors = [
-0000f590: 6c2e 636f 6c6f 7220 2020 2020 2020 2020  l.color         
-0000f5a0: 2020 2020 2020 2020 666f 7220 6c20 696e          for l in
-0000f5b0: 206c 696e 6573 5d0a 2020 2020 2020 2020   lines].        
-0000f5c0: 2020 2020 786c 6162 656c 203d 2078 6c61      xlabel = xla
-0000f5d0: 6265 6c20 6f72 2028 2249 6e74 6572 6163  bel or ("Interac
-0000f5e0: 7469 6f6e 2220 6966 2078 3d3d 2769 6e64  tion" if x=='ind
-0000f5f0: 6578 2720 656c 7365 2078 5b30 5d20 6966  ex' else x[0] if
-0000f600: 206c 656e 2878 2920 3d3d 2031 2065 6c73   len(x) == 1 els
-0000f610: 6520 7829 0a20 2020 2020 2020 2020 2020  e x).           
-0000f620: 2079 6c61 6265 6c20 3d20 796c 6162 656c   ylabel = ylabel
-0000f630: 206f 7220 2822 5265 7761 7264 2220 6966   or ("Reward" if
-0000f640: 2079 3d3d 2772 6577 6172 6427 2065 6c73   y=='reward' els
-0000f650: 6520 792e 7265 706c 6163 6528 225f 7063  e y.replace("_pc
-0000f660: 7422 2c22 2050 6572 6365 6e74 2229 290a  t"," Percent")).
-0000f670: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000f680: 6c65 6e28 7365 7428 595f 636f 756e 7429  len(set(Y_count)
-0000f690: 2920 3d3d 2031 3a20 595f 636f 756e 7420  ) == 1: Y_count 
-0000f6a0: 3d20 595f 636f 756e 745b 305d 0a0a 2020  = Y_count[0]..  
-0000f6b0: 2020 2020 2020 2020 2020 795f 6c6f 6361            y_loca
-0000f6c0: 7469 6f6e 203d 2022 546f 7461 6c22 2069  tion = "Total" i
-0000f6d0: 6620 7820 213d 2027 696e 6465 7827 2065  f x != 'index' e
-0000f6e0: 6c73 6520 2222 0a20 2020 2020 2020 2020  lse "".         
-0000f6f0: 2020 2079 5f61 7667 5f74 7970 6520 3d20     y_avg_type = 
-0000f700: 2822 496e 7374 616e 7422 2069 6620 7370  ("Instant" if sp
-0000f710: 616e 203d 3d20 3120 656c 7365 2066 2253  an == 1 else f"S
-0000f720: 7061 6e20 7b73 7061 6e7d 2220 6966 2073  pan {span}" if s
-0000f730: 7061 6e20 656c 7365 2022 5072 6f67 7265  pan else "Progre
-0000f740: 7373 6976 6522 290a 2020 2020 2020 2020  ssive").        
-0000f750: 2020 2020 795f 7361 6d70 6c65 7320 203d      y_samples  =
-0000f760: 2066 2228 7b59 5f63 6f75 6e74 7d20 456e   f"({Y_count} En
-0000f770: 7669 726f 6e6d 656e 7473 2922 0a20 2020  vironments)".   
-0000f780: 2020 2020 2020 2020 2074 6974 6c65 2020           title  
-0000f790: 2020 2020 3d20 7469 746c 6520 6966 2074      = title if t
-0000f7a0: 6974 6c65 2069 7320 6e6f 7420 4e6f 6e65  itle is not None
-0000f7b0: 2065 6c73 6520 2827 2027 2e6a 6f69 6e28   else (' '.join(
-0000f7c0: 6669 6c74 6572 284e 6f6e 652c 5b79 5f6c  filter(None,[y_l
-0000f7d0: 6f63 6174 696f 6e2c 2079 5f61 7667 5f74  ocation, y_avg_t
-0000f7e0: 7970 652c 2079 6c61 6265 6c2c 2079 5f73  ype, ylabel, y_s
-0000f7f0: 616d 706c 6573 5d29 2929 0a0a 2020 2020  amples])))..    
-0000f800: 2020 2020 2020 2020 7872 6f74 6174 696f          xrotatio
-0000f810: 6e20 3d20 3930 2069 6620 2878 2021 3d20  n = 90 if (x != 
-0000f820: 2769 6e64 6578 2720 6f72 2078 6f72 6465  'index' or xorde
-0000f830: 7229 2061 6e64 206c 656e 286c 696e 6573  r) and len(lines
-0000f840: 5b30 5d2e 5829 3e35 2065 6c73 6520 300a  [0].X)>5 else 0.
-0000f850: 2020 2020 2020 2020 2020 2020 7972 6f74              yrot
-0000f860: 6174 696f 6e20 3d20 300a 0a20 2020 2020  ation = 0..     
-0000f870: 2020 2020 2020 2069 6620 746f 705f 6e3a         if top_n:
-0000f880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f890: 2069 6620 6162 7328 746f 705f 6e29 203e   if abs(top_n) >
-0000f8a0: 206c 656e 286c 696e 6573 293a 2074 6f70   len(lines): top
-0000f8b0: 5f6e 203d 206c 656e 286c 696e 6573 292a  _n = len(lines)*
-0000f8c0: 6162 7328 746f 705f 6e29 2f74 6f70 5f6e  abs(top_n)/top_n
-0000f8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f8e0: 2069 6620 746f 705f 6e20 3e20 303a 206c   if top_n > 0: l
-0000f8f0: 696e 6573 203d 205b 7265 706c 6163 6528  ines = [replace(
-0000f900: 6c2c 636f 6c6f 723d 7365 6c66 2e5f 6765  l,color=self._ge
-0000f910: 745f 636f 6c6f 7228 636f 6c6f 7273 2c69  t_color(colors,i
-0000f920: 292c 6c61 6265 6c3d 7365 6c66 2e5f 6765  ),label=self._ge
-0000f930: 745f 6c61 6265 6c28 6c61 6265 6c73 2c6c  t_label(labels,l
-0000f940: 2e6c 6162 656c 2c69 2929 2066 6f72 2069  .label,i)) for i
-0000f950: 2c6c 2069 6e20 656e 756d 6572 6174 6528  ,l in enumerate(
-0000f960: 6c69 6e65 735b 3a74 6f70 5f6e 5d2c 3020  lines[:top_n],0 
-0000f970: 2020 2029 205d 0a20 2020 2020 2020 2020     ) ].         
-0000f980: 2020 2020 2020 2069 6620 746f 705f 6e20         if top_n 
-0000f990: 3c20 303a 206c 696e 6573 203d 205b 7265  < 0: lines = [re
-0000f9a0: 706c 6163 6528 6c2c 636f 6c6f 723d 7365  place(l,color=se
-0000f9b0: 6c66 2e5f 6765 745f 636f 6c6f 7228 636f  lf._get_color(co
-0000f9c0: 6c6f 7273 2c69 292c 6c61 6265 6c3d 7365  lors,i),label=se
-0000f9d0: 6c66 2e5f 6765 745f 6c61 6265 6c28 6c61  lf._get_label(la
-0000f9e0: 6265 6c73 2c6c 2e6c 6162 656c 2c69 2929  bels,l.label,i))
-0000f9f0: 2066 6f72 2069 2c6c 2069 6e20 656e 756d   for i,l in enum
-0000fa00: 6572 6174 6528 6c69 6e65 735b 746f 705f  erate(lines[top_
-0000fa10: 6e3a 5d2c 746f 705f 6e29 205d 0a0a 2020  n:],top_n) ]..  
-0000fa20: 2020 2020 2020 2020 2020 616c 6c5f 7820            all_x 
-0000fa30: 3d20 6469 6374 2e66 726f 6d6b 6579 7328  = dict.fromkeys(
-0000fa40: 6368 6169 6e2e 6672 6f6d 5f69 7465 7261  chain.from_itera
-0000fa50: 626c 6528 6c69 6e65 2e58 2066 6f72 206c  ble(line.X for l
-0000fa60: 696e 6520 696e 206c 696e 6573 2929 0a20  ine in lines)). 
-0000fa70: 2020 2020 2020 2020 2020 2078 6f72 6465             xorde
-0000fa80: 7265 6420 3d20 6c69 7374 2861 6c6c 5f78  red = list(all_x
-0000fa90: 2e6b 6579 7328 2929 2069 6620 6e6f 7420  .keys()) if not 
-0000faa0: 786f 7264 6572 2065 6c73 6520 736f 7274  xorder else sort
-0000fab0: 6564 2861 6c6c 5f78 2c20 7265 7665 7273  ed(all_x, revers
-0000fac0: 653d 786f 7264 6572 3d3d 272d 2729 0a0a  e=xorder=='-')..
-0000fad0: 2020 2020 2020 2020 2020 2020 6966 2078              if x
-0000fae0: 203d 3d20 2769 6e64 6578 2720 616e 6420   == 'index' and 
-0000faf0: 786f 7264 6572 2069 6e20 5b27 2b27 2c4e  xorder in ['+',N
-0000fb00: 6f6e 655d 3a20 786f 7264 6572 6564 203d  one]: xordered =
-0000fb10: 204e 6f6e 650a 0a20 2020 2020 2020 2020   None..         
-0000fb20: 2020 2073 656c 662e 5f70 6c6f 7474 6572     self._plotter
-0000fb30: 2e70 6c6f 7428 6178 2c20 6c69 6e65 732c  .plot(ax, lines,
-0000fb40: 2074 6974 6c65 2c20 786c 6162 656c 2c20   title, xlabel, 
-0000fb50: 796c 6162 656c 2c20 786c 696d 2c20 796c  ylabel, xlim, yl
-0000fb60: 696d 2c20 7874 6963 6b73 2c20 7974 6963  im, xticks, ytic
-0000fb70: 6b73 2c20 6c65 6765 6e64 2c20 7872 6f74  ks, legend, xrot
-0000fb80: 6174 696f 6e2c 2079 726f 7461 7469 6f6e  ation, yrotation
-0000fb90: 2c20 786f 7264 6572 6564 2c20 6f75 7429  , xordered, out)
-0000fba0: 0a0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-0000fbb0: 2043 6f62 6145 7863 6570 7469 6f6e 2061   CobaException a
-0000fbc0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-0000fbd0: 2043 6f62 6143 6f6e 7465 7874 2e6c 6f67   CobaContext.log
-0000fbe0: 6765 722e 6c6f 6728 7374 7228 6529 290a  ger.log(str(e)).
-0000fbf0: 0a20 2020 2064 6566 2070 6c6f 745f 636f  .    def plot_co
-0000fc00: 6e74 7261 7374 2873 656c 662c 0a20 2020  ntrast(self,.   
-0000fc10: 2020 2020 206c 3120 2020 2020 203a 2041       l1      : A
-0000fc20: 6e79 2c0a 2020 2020 2020 2020 6c32 2020  ny,.        l2  
-0000fc30: 2020 2020 3a20 416e 792c 0a20 2020 2020      : Any,.     
-0000fc40: 2020 2078 2020 2020 2020 203a 2055 6e69     x       : Uni
-0000fc50: 6f6e 5b73 7472 2c20 5365 7175 656e 6365  on[str, Sequence
-0000fc60: 5b73 7472 5d5d 203d 2022 656e 7669 726f  [str]] = "enviro
-0000fc70: 6e6d 656e 745f 6964 222c 0a20 2020 2020  nment_id",.     
-0000fc80: 2020 2079 2020 2020 2020 203a 2073 7472     y       : str
-0000fc90: 203d 2022 7265 7761 7264 222c 0a20 2020   = "reward",.   
-0000fca0: 2020 2020 206c 2020 2020 2020 203a 2055       l       : U
-0000fcb0: 6e69 6f6e 5b73 7472 2c20 5365 7175 656e  nion[str, Sequen
-0000fcc0: 6365 5b73 7472 5d5d 203d 2027 6c65 6172  ce[str]] = 'lear
-0000fcd0: 6e65 725f 6964 272c 0a20 2020 2020 2020  ner_id',.       
-0000fce0: 2070 2020 2020 2020 203a 2055 6e69 6f6e   p       : Union
-0000fcf0: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
-0000fd00: 7472 5d5d 203d 2027 656e 7669 726f 6e6d  tr]] = 'environm
-0000fd10: 656e 745f 6964 272c 0a20 2020 2020 2020  ent_id',.       
-0000fd20: 206d 6f64 6520 2020 203a 2055 6e69 6f6e   mode    : Union
-0000fd30: 5b4c 6974 6572 616c 5b22 6469 6666 222c  [Literal["diff",
-0000fd40: 2270 726f 6222 5d2c 2043 616c 6c61 626c  "prob"], Callabl
-0000fd50: 655b 5b66 6c6f 6174 2c66 6c6f 6174 5d2c  e[[float,float],
-0000fd60: 666c 6f61 745d 5d20 3d20 2264 6966 6622  float]] = "diff"
-0000fd70: 2c0a 2020 2020 2020 2020 7370 616e 2020  ,.        span  
-0000fd80: 2020 3a20 696e 7420 3d20 4e6f 6e65 2c0a    : int = None,.
-0000fd90: 2020 2020 2020 2020 6572 7220 2020 2020          err     
-0000fda0: 3a20 556e 696f 6e5b 4c69 7465 7261 6c5b  : Union[Literal[
-0000fdb0: 2773 6527 2c27 7364 272c 2762 7327 2c27  'se','sd','bs','
-0000fdc0: 6269 275d 2c20 506f 696e 7441 6e64 496e  bi'], PointAndIn
-0000fdd0: 7465 7276 616c 5d20 3d20 4e6f 6e65 2c0a  terval] = None,.
-0000fde0: 2020 2020 2020 2020 6572 7265 7665 7279          errevery
-0000fdf0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-0000fe00: 2020 2020 2020 6c61 6265 6c73 2020 3a20        labels  : 
-0000fe10: 5365 7175 656e 6365 5b73 7472 5d20 3d20  Sequence[str] = 
-0000fe20: 4e6f 6e65 2c0a 2020 2020 2020 2020 636f  None,.        co
-0000fe30: 6c6f 7273 2020 3a20 5365 7175 656e 6365  lors  : Sequence
-0000fe40: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000fe50: 2020 2020 2020 7469 746c 6520 2020 3a20        title   : 
-0000fe60: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0000fe70: 2020 2020 786c 6162 656c 2020 3a20 7374      xlabel  : st
-0000fe80: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-0000fe90: 2020 796c 6162 656c 2020 3a20 7374 7220    ylabel  : str 
-0000fea0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000feb0: 786c 696d 2020 2020 3a20 5475 706c 655b  xlim    : Tuple[
-0000fec0: 4f70 7469 6f6e 616c 5b4e 756d 6265 725d  Optional[Number]
-0000fed0: 2c4f 7074 696f 6e61 6c5b 4e75 6d62 6572  ,Optional[Number
-0000fee0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-0000fef0: 2020 2079 6c69 6d20 2020 203a 2054 7570     ylim    : Tup
-0000ff00: 6c65 5b4f 7074 696f 6e61 6c5b 4e75 6d62  le[Optional[Numb
-0000ff10: 6572 5d2c 4f70 7469 6f6e 616c 5b4e 756d  er],Optional[Num
-0000ff20: 6265 725d 5d20 3d20 4e6f 6e65 2c0a 2020  ber]] = None,.  
-0000ff30: 2020 2020 2020 7874 6963 6b73 2020 3a20        xticks  : 
-0000ff40: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-0000ff50: 2020 2020 2079 7469 636b 7320 203a 2062       yticks  : b
-0000ff60: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
-0000ff70: 2020 2020 6c65 6765 6e64 2020 3a20 626f      legend  : bo
-0000ff80: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
-0000ff90: 2020 2061 6c70 6861 2020 203a 2066 6c6f     alpha   : flo
-0000ffa0: 6174 203d 2031 2c0a 2020 2020 2020 2020  at = 1,.        
-0000ffb0: 786f 7264 6572 2020 3a20 4c69 7465 7261  xorder  : Litera
-0000ffc0: 6c5b 272b 272c 272d 275d 203d 204e 6f6e  l['+','-'] = Non
-0000ffd0: 652c 0a20 2020 2020 2020 2062 6f75 6e64  e,.        bound
-0000ffe0: 6172 793a 2062 6f6f 6c20 3d20 5472 7565  ary: bool = True
-0000fff0: 2c0a 2020 2020 2020 2020 6f75 7420 2020  ,.        out   
-00010000: 2020 3a20 556e 696f 6e5b 4e6f 6e65 2c4c    : Union[None,L
-00010010: 6974 6572 616c 5b27 7363 7265 656e 275d  iteral['screen']
-00010020: 2c73 7472 5d20 3d20 2773 6372 6565 6e27  ,str] = 'screen'
-00010030: 2c0a 2020 2020 2020 2020 6178 203d 204e  ,.        ax = N
-00010040: 6f6e 6529 202d 3e20 4e6f 6e65 3a0a 2020  one) -> None:.  
-00010050: 2020 2020 2020 2222 2250 6c6f 7420 6120        """Plot a 
-00010060: 6469 7265 6374 2063 6f6e 7472 6173 7420  direct contrast 
-00010070: 6f66 2074 6865 2070 6572 666f 726d 616e  of the performan
-00010080: 6365 2066 6f72 2074 776f 206c 6561 726e  ce for two learn
-00010090: 6572 732e 0a0a 2020 2020 2020 2020 4172  ers...        Ar
-000100a0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-000100b0: 6c31 3a20 5468 6520 6669 7273 7420 7365  l1: The first se
-000100c0: 7420 6f66 2070 6172 616d 6574 6572 2076  t of parameter v
-000100d0: 616c 7565 7320 7765 2077 616e 7420 746f  alues we want to
-000100e0: 2063 6f6e 7472 6173 742e 0a20 2020 2020   contrast..     
-000100f0: 2020 2020 2020 206c 323a 2054 6865 2073         l2: The s
-00010100: 6563 6f6e 6420 7365 7420 6f66 2070 6172  econd set of par
-00010110: 616d 6574 6572 2076 616c 7565 7320 7765  ameter values we
-00010120: 2077 616e 7420 746f 2063 6f6e 7472 6173   want to contras
-00010130: 742e 0a20 2020 2020 2020 2020 2020 2078  t..            x
-00010140: 3a20 5468 6520 7661 6c75 6520 746f 2070  : The value to p
-00010150: 6c6f 7420 6f6e 2074 6865 2078 2d61 7869  lot on the x-axi
-00010160: 732e 2054 6869 7320 6361 6e20 6569 7468  s. This can eith
-00010170: 6572 2062 6520 696e 6465 7820 6f72 2065  er be index or e
-00010180: 6e76 6972 6f6e 6d65 6e74 2063 6f6c 756d  nvironment colum
-00010190: 6e73 2074 6f20 6772 6f75 7020 6279 2e0a  ns to group by..
-000101a0: 2020 2020 2020 2020 2020 2020 793a 2054              y: T
-000101b0: 6865 2076 616c 7565 2074 6f20 706c 6f74  he value to plot
-000101c0: 206f 6e20 7468 6520 792d 6178 6973 2e0a   on the y-axis..
-000101d0: 2020 2020 2020 2020 2020 2020 6c3a 2054              l: T
-000101e0: 6865 206c 6576 656c 2061 7420 7768 6963  he level at whic
-000101f0: 6820 7765 2077 616e 7420 746f 2063 6f6e  h we want to con
-00010200: 7472 6173 742e 0a20 2020 2020 2020 2020  trast..         
-00010210: 2020 2070 3a20 5468 6520 7061 6972 7320     p: The pairs 
-00010220: 7468 6174 206d 7573 7420 6578 6973 7420  that must exist 
-00010230: 6163 726f 7373 2061 6c6c 2063 6f6d 7061  across all compa
-00010240: 7269 736f 6e20 6c65 7665 6c73 2069 6e20  rison levels in 
-00010250: 6f72 6465 7220 746f 2062 6520 696e 636c  order to be incl
-00010260: 7564 6564 2e0a 2020 2020 2020 2020 2020  uded..          
-00010270: 2020 6d6f 6465 3a20 2764 6966 6627 202d    mode: 'diff' -
-00010280: 2d20 706c 6f74 2074 6865 2070 6169 7277  - plot the pairw
-00010290: 6973 6520 6469 6666 6572 656e 6365 3b20  ise difference; 
-000102a0: 2770 726f 6227 2070 6c6f 7420 7468 6520  'prob' plot the 
-000102b0: 7072 6f62 6162 696c 6974 7920 6f66 206c  probability of l
-000102c0: 3120 6265 6174 696e 6720 6c32 2e0a 2020  1 beating l2..  
-000102d0: 2020 2020 2020 2020 2020 7370 616e 3a20            span: 
-000102e0: 5468 6520 6e75 6d62 6572 206f 6620 7920  The number of y 
-000102f0: 7661 6c75 6573 2074 6f20 736d 6f6f 7468  values to smooth
-00010300: 2074 6f67 6574 6865 7220 7768 656e 2072   together when r
-00010310: 6570 6f72 7469 6e67 2079 2e20 4966 2074  eporting y. If t
-00010320: 6869 7320 6973 204e 6f6e 6520 7468 656e  his is None then
-00010330: 2074 6865 2061 7665 7261 6765 206f 6620   the average of 
-00010340: 616c 6c20 790a 2020 2020 2020 2020 2020  all y.          
-00010350: 2020 2020 2020 7661 6c75 6573 2075 7020        values up 
-00010360: 746f 2063 7572 7265 6e74 2069 7320 7368  to current is sh
-00010370: 6f77 6e20 6f74 6865 7277 6973 6520 6120  own otherwise a 
-00010380: 6d6f 7669 6e67 2061 7665 7261 6765 2077  moving average w
-00010390: 6974 6820 7769 6e64 6f77 2073 697a 6520  ith window size 
-000103a0: 6f66 2073 7061 6e20 2874 6865 2077 696e  of span (the win
-000103b0: 646f 7720 7769 6c6c 2062 650a 2020 2020  dow will be.    
-000103c0: 2020 2020 2020 2020 2020 2020 736d 616c              smal
-000103d0: 6c65 7220 7468 616e 2073 7061 6e20 696e  ler than span in
-000103e0: 6974 6961 6c6c 7929 2e0a 2020 2020 2020  itially)..      
-000103f0: 2020 2020 2020 6572 723a 2054 6869 7320        err: This 
-00010400: 6465 7465 726d 696e 6573 2077 6861 7420  determines what 
-00010410: 6b69 6e64 206f 6620 6572 726f 7220 6261  kind of error ba
-00010420: 7273 2074 6f20 706c 6f74 2028 6966 2061  rs to plot (if a
-00010430: 6e79 292e 2049 6620 604e 6f6e 6560 2074  ny). If `None` t
-00010440: 6865 6e20 6e6f 2062 6172 7320 6172 6520  hen no bars are 
-00010450: 706c 6f74 7465 642c 2069 6620 2773 6527  plotted, if 'se'
-00010460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010470: 2074 6865 2073 7461 6e64 6172 6420 6572   the standard er
-00010480: 726f 7220 6973 2073 686f 776e 2c20 616e  ror is shown, an
-00010490: 6420 6966 2027 7364 2720 7468 6520 7374  d if 'sd' the st
-000104a0: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
-000104b0: 2069 7320 7368 6f77 6e2e 0a20 2020 2020   is shown..     
-000104c0: 2020 2020 2020 2065 7272 6576 6572 793a         errevery:
-000104d0: 2054 6869 7320 6465 7465 726d 696e 6573   This determines
-000104e0: 2074 6865 2066 7265 7175 656e 6379 206f   the frequency o
-000104f0: 6620 6572 726f 7262 6172 732e 2049 6620  f errorbars. If 
-00010500: 604e 6f6e 6560 2074 6865 7920 6170 7065  `None` they appe
-00010510: 6172 2035 2520 6f66 2074 6865 2074 696d  ar 5% of the tim
-00010520: 652e 0a20 2020 2020 2020 2020 2020 206c  e..            l
-00010530: 6162 656c 733a 2054 6865 206c 6567 656e  abels: The legen
-00010540: 6420 6c61 6265 6c73 2074 6f20 7573 6520  d labels to use 
-00010550: 696e 2074 6865 2070 6c6f 742e 2054 6865  in the plot. The
-00010560: 7365 2073 686f 756c 6420 6265 2069 6e20  se should be in 
-00010570: 6f72 6465 7220 6f66 2074 6865 2061 6374  order of the act
-00010580: 7561 6c20 6c65 6765 6e64 206c 6162 656c  ual legend label
-00010590: 732e 0a20 2020 2020 2020 2020 2020 2074  s..            t
-000105a0: 6974 6c65 203a 2054 6865 2074 6974 6c65  itle : The title
-000105b0: 2067 6976 6520 7468 6520 706c 6f74 2e0a   give the plot..
-000105c0: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-000105d0: 7273 3a20 5468 6520 636f 6c6f 7273 2075  rs: The colors u
-000105e0: 7365 6420 746f 2070 6c6f 7420 7468 6520  sed to plot the 
-000105f0: 6c65 6172 6e65 7273 2070 6c6f 742e 0a20  learners plot.. 
-00010600: 2020 2020 2020 2020 2020 2078 6c61 6265             xlabe
-00010610: 6c3a 2054 6865 206c 6162 656c 206f 6e20  l: The label on 
-00010620: 7468 6520 782d 6178 6973 2e0a 2020 2020  the x-axis..    
-00010630: 2020 2020 2020 2020 796c 6162 656c 3a20          ylabel: 
-00010640: 5468 6520 6c61 6265 6c20 6f6e 2074 6865  The label on the
-00010650: 2079 2d61 7869 732e 0a20 2020 2020 2020   y-axis..       
-00010660: 2020 2020 206c 6567 656e 643a 2057 6865       legend: Whe
-00010670: 7468 6572 2074 6865 206c 6567 656e 6420  ther the legend 
-00010680: 666f 7220 7468 6520 706c 6f74 2073 686f  for the plot sho
-00010690: 756c 6420 6265 2064 7261 776e 2e0a 2020  uld be drawn..  
-000106a0: 2020 2020 2020 2020 2020 616c 7068 613a            alpha:
-000106b0: 2054 6865 206f 7061 6369 7479 206f 6620   The opacity of 
-000106c0: 6472 6177 6e20 6461 7461 2e0a 2020 2020  drawn data..    
-000106d0: 2020 2020 2020 2020 786c 696d 3a20 4465          xlim: De
-000106e0: 6669 6e65 2074 6865 2078 2d61 7869 7320  fine the x-axis 
-000106f0: 6c69 6d69 7473 2074 6f20 706c 6f74 2e20  limits to plot. 
-00010700: 4966 2060 4e6f 6e65 6020 7468 6520 782d  If `None` the x-
-00010710: 6178 6973 206c 696d 6974 7320 7769 6c6c  axis limits will
-00010720: 2062 6520 696e 6665 7272 6564 2e0a 2020   be inferred..  
-00010730: 2020 2020 2020 2020 2020 796c 696d 3a20            ylim: 
-00010740: 4465 6669 6e65 2074 6865 2079 2d61 7869  Define the y-axi
-00010750: 7320 6c69 6d69 7473 2074 6f20 706c 6f74  s limits to plot
-00010760: 2e20 4966 2060 4e6f 6e65 6020 7468 6520  . If `None` the 
-00010770: 792d 6178 6973 206c 696d 6974 7320 7769  y-axis limits wi
-00010780: 6c6c 2062 6520 696e 6665 7272 6564 2e0a  ll be inferred..
-00010790: 2020 2020 2020 2020 2020 2020 7874 6963              xtic
-000107a0: 6b73 3a20 5768 6574 6865 7220 7468 6520  ks: Whether the 
-000107b0: 782d 6178 6973 206c 6162 656c 7320 7368  x-axis labels sh
-000107c0: 6f75 6c64 2062 6520 6472 6177 6e2e 0a20  ould be drawn.. 
-000107d0: 2020 2020 2020 2020 2020 2079 7469 636b             ytick
-000107e0: 733a 2057 6865 7468 6572 2074 6865 2079  s: Whether the y
-000107f0: 2d61 7869 7320 6c61 6265 6c73 2073 686f  -axis labels sho
-00010800: 756c 6420 6265 2064 7261 776e 2e0a 2020  uld be drawn..  
-00010810: 2020 2020 2020 2020 2020 786f 7264 6572            xorder
-00010820: 3a20 496e 6469 6361 7465 7320 7768 6574  : Indicates whet
-00010830: 6865 7220 7468 6520 782d 6178 6973 2073  her the x-axis s
-00010840: 686f 756c 6420 6265 2069 6e20 6173 6365  hould be in asce
-00010850: 6e64 696e 6720 282b 2920 6f72 2064 6573  nding (+) or des
-00010860: 6365 6e64 6569 6e67 2028 2d29 206f 7264  cendeing (-) ord
-00010870: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
-00010880: 626f 756e 6461 7279 3a20 5768 6574 6865  boundary: Whethe
-00010890: 7220 7765 2077 616e 7420 746f 2070 6c6f  r we want to plo
-000108a0: 7420 7468 6520 626f 756e 6461 7279 206c  t the boundary l
-000108b0: 696e 6520 6265 7477 6565 6e20 7768 6963  ine between whic
-000108c0: 6820 7365 7420 6973 2074 6865 2062 6573  h set is the bes
-000108d0: 7420 7065 7266 6f72 6d69 6e67 2e0a 2020  t performing..  
-000108e0: 2020 2020 2020 2020 2020 6f75 743a 2049            out: I
-000108f0: 6e64 6963 6174 6520 7768 6572 6520 7468  ndicate where th
-00010900: 6520 706c 6f74 2073 686f 756c 6420 6265  e plot should be
-00010910: 2073 656e 7420 746f 2061 6674 6572 2070   sent to after p
-00010920: 6c6f 7474 696e 6720 6973 2066 696e 6973  lotting is finis
-00010930: 6865 642e 2056 616c 6964 2076 616c 7565  hed. Valid value
-00010940: 7320 6172 650a 2020 2020 2020 2020 2020  s are.          
-00010950: 2020 2020 2020 2773 6372 6565 6e27 2074        'screen' t
-00010960: 6f20 7368 6f77 2069 7420 6f6e 2073 6372  o show it on scr
-00010970: 6565 6e2c 2061 2070 6174 6820 746f 2073  een, a path to s
-00010980: 6176 6520 746f 2064 6973 6b2c 206f 7220  ave to disk, or 
-00010990: 4e6f 6e65 2069 6620 7468 6520 706c 6f74  None if the plot
-000109a0: 2073 686f 756c 6420 6e6f 7420 6265 0a20   should not be. 
-000109b0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000109c0: 7574 7075 7420 616e 7977 6865 7265 2028  utput anywhere (
-000109d0: 692e 652e 2c20 6b65 7074 2069 6e20 6d65  i.e., kept in me
-000109e0: 6d6f 7279 2920 696e 206f 7264 6572 2074  mory) in order t
-000109f0: 6f20 6b65 6570 2065 6469 7469 6e67 2074  o keep editing t
-00010a00: 6865 2070 6c6f 7420 6166 7465 7220 7468  he plot after th
-00010a10: 6973 2063 616c 6c2e 0a20 2020 2020 2020  is call..       
-00010a20: 2020 2020 2061 783a 2050 726f 7669 6465       ax: Provide
-00010a30: 2061 6e20 6f70 7469 6f6e 616c 2061 7865   an optional axe
-00010a40: 7320 7468 6174 2074 6865 2070 6c6f 7420  s that the plot 
-00010a50: 7769 6c6c 2062 6520 6472 6177 6e20 746f  will be drawn to
-00010a60: 2e20 4966 206e 6f74 2070 726f 7669 6465  . If not provide
-00010a70: 6420 6120 6e65 7720 6669 6775 7265 2f61  d a new figure/a
-00010a80: 7865 7320 6973 2063 7265 6174 6564 2e0a  xes is created..
-00010a90: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00010aa0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00010ab0: 2020 2020 2020 786c 696d 203d 2078 6c69        xlim = xli
-00010ac0: 6d20 6f72 205b 4e6f 6e65 2c4e 6f6e 655d  m or [None,None]
-00010ad0: 0a20 2020 2020 2020 2020 2020 2079 6c69  .            yli
-00010ae0: 6d20 3d20 796c 696d 206f 7220 5b4e 6f6e  m = ylim or [Non
-00010af0: 652c 4e6f 6e65 5d0a 0a20 2020 2020 2020  e,None]..       
-00010b00: 2020 2020 2072 6177 5f64 6174 6120 3d20       raw_data = 
-00010b10: 7365 6c66 2e72 6177 5f63 6f6e 7472 6173  self.raw_contras
-00010b20: 7428 6c31 2c6c 322c 782c 792c 6c2c 702c  t(l1,l2,x,y,l,p,
-00010b30: 7370 616e 290a 0a20 2020 2020 2020 2020  span)..         
-00010b40: 2020 206c 6973 745f 6c69 6b65 3d28 6c69     list_like=(li
-00010b50: 7374 2c74 7570 6c65 290a 0a20 2020 2020  st,tuple)..     
-00010b60: 2020 2020 2020 2069 6620 2020 2020 6973         if     is
-00010b70: 696e 7374 616e 6365 286c 2c6c 6973 745f  instance(l,list_
-00010b80: 6c69 6b65 2920 616e 6420 6e6f 7420 6973  like) and not is
-00010b90: 696e 7374 616e 6365 286c 315b 305d 2c6c  instance(l1[0],l
-00010ba0: 6973 745f 6c69 6b65 293a 206c 3120 3d20  ist_like): l1 = 
-00010bb0: 5b6c 315d 0a20 2020 2020 2020 2020 2020  [l1].           
-00010bc0: 2069 6620 2020 2020 6973 696e 7374 616e   if     isinstan
-00010bd0: 6365 286c 2c6c 6973 745f 6c69 6b65 2920  ce(l,list_like) 
-00010be0: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
-00010bf0: 6365 286c 325b 305d 2c6c 6973 745f 6c69  ce(l2[0],list_li
-00010c00: 6b65 293a 206c 3220 3d20 5b6c 325d 0a20  ke): l2 = [l2]. 
-00010c10: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00010c20: 7420 6973 696e 7374 616e 6365 286c 2c6c  t isinstance(l,l
-00010c30: 6973 745f 6c69 6b65 2920 616e 6420 6e6f  ist_like) and no
-00010c40: 7420 6973 696e 7374 616e 6365 286c 3120  t isinstance(l1 
-00010c50: 2020 2c6c 6973 745f 6c69 6b65 293a 206c    ,list_like): l
-00010c60: 3120 3d20 5b6c 315d 0a20 2020 2020 2020  1 = [l1].       
-00010c70: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-00010c80: 7374 616e 6365 286c 2c6c 6973 745f 6c69  stance(l,list_li
-00010c90: 6b65 2920 616e 6420 6e6f 7420 6973 696e  ke) and not isin
-00010ca0: 7374 616e 6365 286c 3220 2020 2c6c 6973  stance(l2   ,lis
-00010cb0: 745f 6c69 6b65 293a 206c 3220 3d20 5b6c  t_like): l2 = [l
-00010cc0: 325d 0a0a 2020 2020 2020 2020 2020 2020  2]..            
-00010cd0: 636f 6e74 7261 7374 6572 203d 2028 6c61  contraster = (la
-00010ce0: 6d62 6461 2074 3a20 745b 315d 2d74 5b30  mbda t: t[1]-t[0
-00010cf0: 5d29 2069 6620 6d6f 6465 203d 3d20 2764  ]) if mode == 'd
-00010d00: 6966 6627 2065 6c73 6520 286c 616d 6264  iff' else (lambd
-00010d10: 6120 743a 2069 6e74 2828 745b 315d 2d74  a t: int((t[1]-t
-00010d20: 5b30 5d29 3e30 2929 2069 6620 6d6f 6465  [0])>0)) if mode
-00010d30: 3d3d 2770 726f 6227 2065 6c73 6520 6d6f  =='prob' else mo
-00010d40: 6465 0a20 2020 2020 2020 2020 2020 205f  de.            _
-00010d50: 626f 756e 6461 7279 2020 3d20 3020 6966  boundary  = 0 if
-00010d60: 206d 6f64 6520 3d3d 2027 6469 6666 2720   mode == 'diff' 
-00010d70: 656c 7365 202e 350a 0a20 2020 2020 2020  else .5..       
-00010d80: 2020 2020 2065 7272 6576 6572 7920 3d20       errevery = 
-00010d90: 6572 7265 7665 7279 206f 7220 6d61 7828  errevery or max(
-00010da0: 696e 7428 7261 775f 6461 7461 5b27 7827  int(raw_data['x'
-00010db0: 5d5b 2d31 5d2a 302e 3035 292c 3129 2069  ][-1]*0.05),1) i
-00010dc0: 6620 7820 3d3d 2027 696e 6465 7827 2065  f x == 'index' e
-00010dd0: 6c73 6520 310a 2020 2020 2020 2020 2020  lse 1.          
-00010de0: 2020 7374 796c 6520 2020 203d 2022 2d22    style    = "-"
-00010df0: 2069 6620 7820 3d3d 2027 696e 6465 7827   if x == 'index'
-00010e00: 2065 6c73 6520 222e 220a 2020 2020 2020   else ".".      
-00010e10: 2020 2020 2020 6572 7220 2020 2020 203d        err      =
-00010e20: 2073 656c 662e 5f63 6f6e 6669 6465 6e63   self._confidenc
-00010e30: 6528 6572 722c 2065 7272 6576 6572 7929  e(err, errevery)
-00010e40: 0a0a 2020 2020 2020 2020 2020 2020 585f  ..            X_
-00010e50: 595f 5945 203d 205b 5d0a 2020 2020 2020  Y_YE = [].      
-00010e60: 2020 2020 2020 666f 7220 5f78 692c 2028        for _xi, (
-00010e70: 5f78 2c20 7061 6972 7329 2069 6e20 656e  _x, pairs) in en
-00010e80: 756d 6572 6174 6528 7261 775f 6461 7461  umerate(raw_data
-00010e90: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00010ea0: 2020 2058 5f59 5f59 452e 6170 7065 6e64     X_Y_YE.append
-00010eb0: 2828 5f78 2c29 2b65 7272 286c 6973 7428  ((_x,)+err(list(
-00010ec0: 6d61 7028 636f 6e74 7261 7374 6572 2c70  map(contraster,p
-00010ed0: 6169 7273 2929 2c5f 7869 2929 0a0a 2020  airs)),_xi))..  
-00010ee0: 2020 2020 2020 2020 2020 6c31 5f6c 6162            l1_lab
-00010ef0: 656c 2c6c 325f 6c61 6265 6c20 3d20 7261  el,l2_label = ra
-00010f00: 775f 6461 7461 2e63 6f6c 756d 6e73 5b31  w_data.columns[1
-00010f10: 5d0a 0a20 2020 2020 2020 2020 2020 2069  ]..            i
-00010f20: 6620 7820 3d3d 2027 696e 6465 7827 3a0a  f x == 'index':.
-00010f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f40: 582c 592c 5945 203d 207a 6970 282a 585f  X,Y,YE = zip(*X_
-00010f50: 595f 5945 290a 2020 2020 2020 2020 2020  Y_YE).          
-00010f60: 2020 2020 2020 636f 6c6f 7220 203d 2073        color  = s
-00010f70: 656c 662e 5f67 6574 5f63 6f6c 6f72 2863  elf._get_color(c
-00010f80: 6f6c 6f72 732c 2020 2020 2020 2020 2020  olors,          
-00010f90: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00010fa0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010fb0: 2020 6966 206d 6f64 6520 3d3d 2022 6469    if mode == "di
-00010fc0: 6666 223a 0a20 2020 2020 2020 2020 2020  ff":.           
-00010fd0: 2020 2020 2020 2020 206c 6162 656c 2020           label  
-00010fe0: 3d20 7365 6c66 2e5f 6765 745f 6c61 6265  = self._get_labe
-00010ff0: 6c28 6c61 6265 6c73 2c66 277b 6c32 5f6c  l(labels,f'{l2_l
-00011000: 6162 656c 7d20 e280 9420 7b6c 315f 6c61  abel} ... {l1_la
-00011010: 6265 6c7d 272c 3029 0a20 2020 2020 2020  bel}',0).       
-00011020: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011040: 2020 206c 6162 656c 2020 3d20 7365 6c66     label  = self
-00011050: 2e5f 6765 745f 6c61 6265 6c28 6c61 6265  ._get_label(labe
-00011060: 6c73 2c66 2750 5b7b 6c32 5f6c 6162 656c  ls,f'P[{l2_label
-00011070: 7d20 3e20 7b6c 315f 6c61 6265 6c7d 5d27  } > {l1_label}]'
-00011080: 2c30 290a 0a20 2020 2020 2020 2020 2020  ,0)..           
-00011090: 2020 2020 206c 6162 656c 2020 3d20 6622       label  = f"
-000110a0: 7b6c 6162 656c 7d22 2069 6620 6c65 6765  {label}" if lege
-000110b0: 6e64 2065 6c73 6520 4e6f 6e65 0a20 2020  nd else None.   
-000110c0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-000110d0: 6573 2020 3d20 5b50 6f69 6e74 7328 582c  es  = [Points(X,
-000110e0: 2059 2c20 4e6f 6e65 2c20 5945 2c20 7374   Y, None, YE, st
-000110f0: 796c 653d 7374 796c 652c 206c 6162 656c  yle=style, label
-00011100: 3d6c 6162 656c 2c20 636f 6c6f 723d 636f  =label, color=co
-00011110: 6c6f 722c 2061 6c70 6861 3d61 6c70 6861  lor, alpha=alpha
-00011120: 295d 0a0a 2020 2020 2020 2020 2020 2020  )]..            
-00011130: 656c 6966 2078 203d 3d20 6c3a 0a20 2020  elif x == l:.   
-00011140: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00011150: 6c65 6e28 6c31 2920 3e20 3120 616e 6420  len(l1) > 1 and 
-00011160: 6c65 6e28 6c32 2920 3d3d 2031 3a0a 2020  len(l2) == 1:.  
-00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011180: 2020 2353 6f72 7420 6279 206c 312e 2057    #Sort by l1. W
-00011190: 6520 6173 7375 6d65 205f 7820 6973 2066  e assume _x is f
-000111a0: 227b 6c32 7d2d 7b6c 317d 222e 0a20 2020  "{l2}-{l1}"..   
+0000bf80: 655b 7374 725d 5d20 3d20 4e6f 6e65 2c0a  e[str]] = None,.
+0000bf90: 2020 2020 2020 2020 793a 7374 7220 3d20          y:str = 
+0000bfa0: 2772 6577 6172 6427 2c0a 2020 2020 2020  'reward',.      
+0000bfb0: 2020 6e3a 696e 7420 3d20 4e6f 6e65 2c0a    n:int = None,.
+0000bfc0: 2020 2020 2020 2020 6675 6c6c 5f6c 3a55          full_l:U
+0000bfd0: 6e69 6f6e 5b73 7472 2c20 5365 7175 656e  nion[str, Sequen
+0000bfe0: 6365 5b73 7472 5d5d 3d27 6c65 6172 6e65  ce[str]]='learne
+0000bff0: 725f 6964 272c 0a20 2020 2020 2020 2066  r_id',.        f
+0000c000: 756c 6c5f 703a 556e 696f 6e5b 7374 722c  ull_p:Union[str,
+0000c010: 2053 6571 7565 6e63 655b 7374 725d 5d3d   Sequence[str]]=
+0000c020: 2765 6e76 6972 6f6e 6d65 6e74 5f69 6427  'environment_id'
+0000c030: 2920 2d3e 2027 5265 7375 6c74 273a 0a20  ) -> 'Result':. 
+0000c040: 2020 2020 2020 2022 2222 5365 6c65 6374         """Select
+0000c050: 2074 6865 2062 6573 7420 7065 7266 6f72   the best perfor
+0000c060: 6d69 6e67 2060 6c60 206f 7665 7220 6070  ming `l` over `p
+0000c070: 602e 0a0a 2020 2020 2020 2020 4172 6773  `...        Args
+0000c080: 3a0a 2020 2020 2020 2020 2020 2020 6c3a  :.            l:
+0000c090: 2054 6865 2068 7970 6572 7061 7261 6d65   The hyperparame
+0000c0a0: 7465 7220 7661 6c75 6573 2077 6520 7769  ter values we wi
+0000c0b0: 7368 2074 6f20 6f70 7469 6d69 7a65 2e0a  sh to optimize..
+0000c0c0: 2020 2020 2020 2020 2020 2020 703a 2054              p: T
+0000c0d0: 6865 2067 726f 7570 696e 6720 7661 7269  he grouping vari
+0000c0e0: 6162 6c65 2077 6520 7769 7368 2074 6f20  able we wish to 
+0000c0f0: 6f70 7469 6d69 7a65 206f 7665 7220 2864  optimize over (d
+0000c100: 6566 6175 6c74 7320 746f 2066 756c 6c5f  efaults to full_
+0000c110: 7029 2e0a 2020 2020 2020 2020 2020 2020  p)..            
+0000c120: 793a 2054 6865 2076 6172 6961 626c 6520  y: The variable 
+0000c130: 7765 2077 6973 6820 746f 206f 7074 696d  we wish to optim
+0000c140: 697a 652e 0a20 2020 2020 2020 2020 2020  ize..           
+0000c150: 206e 3a20 5468 6520 6e75 6d62 6572 206f   n: The number o
+0000c160: 6620 696e 7465 7261 6374 696f 6e73 2077  f interactions w
+0000c170: 6520 7769 7368 2074 6f20 636f 6e73 6964  e wish to consid
+0000c180: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
+0000c190: 6675 6c6c 5f6c 3a20 5468 6520 7472 7565  full_l: The true
+0000c1a0: 206c 6f77 6573 7420 6c65 7665 6c20 6c61   lowest level la
+0000c1b0: 6265 6c20 2865 2e67 2e2c 206c 6561 726e  bel (e.g., learn
+0000c1c0: 6572 5f69 6429 2e0a 2020 2020 2020 2020  er_id)..        
+0000c1d0: 2020 2020 6675 6c6c 5f70 3a20 5468 6520      full_p: The 
+0000c1e0: 7472 7565 206c 6f77 6573 7420 6c65 7665  true lowest leve
+0000c1f0: 6c20 7061 6972 2028 652e 672e 2c20 656e  l pair (e.g., en
+0000c200: 7669 726f 6e6d 656e 745f 6964 292e 0a0a  vironment_id)...
+0000c210: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0000c220: 0a20 2020 2020 2020 2020 2020 2041 2052  .            A R
+0000c230: 6573 756c 7420 7769 7468 2060 6c60 2061  esult with `l` a
+0000c240: 6e64 2060 7060 2074 6861 7420 6973 2074  nd `p` that is t
+0000c250: 6865 206f 7074 696d 616c 206f 7665 720a  he optimal over.
+0000c260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c270: 6066 756c 6c5f 6c60 2061 6e64 2060 6675  `full_l` and `fu
+0000c280: 6c6c 5f70 602e 2046 6f72 2065 7861 6d70  ll_p`. For examp
+0000c290: 6c65 2077 6520 636f 756c 6420 7361 7920  le we could say 
+0000c2a0: 606c 600a 2020 2020 2020 2020 2020 2020  `l`.            
+0000c2b0: 2020 2020 6973 2027 6661 6d69 6c79 2720      is 'family' 
+0000c2c0: 7768 696c 6520 6066 756c 6c5f 6c60 2069  while `full_l` i
+0000c2d0: 7320 276c 6561 726e 6572 5f69 6427 2e20  s 'learner_id'. 
+0000c2e0: 5468 6973 2077 6f75 6c64 0a20 2020 2020  This would.     
+0000c2f0: 2020 2020 2020 2020 2020 2070 6963 6b20             pick 
+0000c300: 7468 6520 6265 7374 2070 6572 666f 726d  the best perform
+0000c310: 696e 6720 6c65 6172 6e65 7220 6772 6f75  ing learner grou
+0000c320: 7065 6420 6279 2066 616d 696c 7920 666f  ped by family fo
+0000c330: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0000c340: 2020 6561 6368 2060 7060 2e0a 0a20 2020    each `p`...   
+0000c350: 2020 2020 204e 6f74 6573 3a0a 2020 2020       Notes:.    
+0000c360: 2020 2020 2020 2020 416e 6f74 6865 7220          Another 
+0000c370: 7761 7920 746f 2074 6869 6e6b 206f 6620  way to think of 
+0000c380: 6974 2069 7320 756e 6465 7220 7468 6520  it is under the 
+0000c390: 6772 6f75 7020 606c 6020 7069 636b 2074  group `l` pick t
+0000c3a0: 6865 0a20 2020 2020 2020 2020 2020 2060  he.            `
+0000c3b0: 6675 6c6c 5f6c 6020 7769 7468 2074 6865  full_l` with the
+0000c3c0: 2062 6573 7420 6176 6572 6167 6520 7065   best average pe
+0000c3d0: 7266 6f72 6d61 6e63 6520 6f76 6572 2060  rformance over `
+0000c3e0: 7060 2e20 5468 650a 2020 2020 2020 2020  p`. The.        
+0000c3f0: 2020 2020 7661 6c75 6520 6f66 2060 6675      value of `fu
+0000c400: 6c6c 5f70 6020 6973 206e 6f74 2075 7365  ll_p` is not use
+0000c410: 6420 746f 2073 656c 6563 7420 7468 6520  d to select the 
+0000c420: 6265 7374 2e20 4974 2069 7320 6f6e 6c79  best. It is only
+0000c430: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+0000c440: 6420 746f 206d 616b 6520 7375 7265 2074  d to make sure t
+0000c450: 6865 2066 696e 616c 2073 656c 6563 7469  he final selecti
+0000c460: 6f6e 2069 7320 7661 6c69 6420 2869 2e65  on is valid (i.e
+0000c470: 2e20 6f6e 6520 6066 756c 6c5f 7060 0a20  . one `full_p`. 
+0000c480: 2020 2020 2020 2020 2020 2065 7869 7374             exist
+0000c490: 7320 666f 7220 6576 6572 7920 606c 6020  s for every `l` 
+0000c4a0: 6174 2074 6865 2065 6e64 206f 6620 7468  at the end of th
+0000c4b0: 6520 7365 6c65 6374 696f 6e20 7072 6f63  e selection proc
+0000c4c0: 6573 7329 2e0a 2020 2020 2020 2020 2222  ess)..        ""
+0000c4d0: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000c4e0: 6e20 7365 6c66 2e66 696c 7465 725f 6265  n self.filter_be
+0000c4f0: 7374 286c 2c70 2c79 2c6e 2c66 756c 6c5f  st(l,p,y,n,full_
+0000c500: 6c2c 6675 6c6c 5f70 290a 0a20 2020 2064  l,full_p)..    d
+0000c510: 6566 2077 6865 7265 5f66 696e 2873 656c  ef where_fin(sel
+0000c520: 662c 0a20 2020 2020 2020 206e 3a20 556e  f,.        n: Un
+0000c530: 696f 6e5b 696e 742c 4c69 7465 7261 6c5b  ion[int,Literal[
+0000c540: 276d 696e 275d 5d20 3d20 4e6f 6e65 2c0a  'min']] = None,.
+0000c550: 2020 2020 2020 2020 6c3a 2055 6e69 6f6e          l: Union
+0000c560: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
+0000c570: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
+0000c580: 2020 2020 2070 3a20 556e 696f 6e5b 7374       p: Union[st
+0000c590: 722c 2053 6571 7565 6e63 655b 7374 725d  r, Sequence[str]
+0000c5a0: 5d20 3d20 4e6f 6e65 2920 2d3e 2027 5265  ] = None) -> 'Re
+0000c5b0: 7375 6c74 273a 0a20 2020 2020 2020 2022  sult':.        "
+0000c5c0: 2222 4669 6c74 6572 2074 6865 2072 6573  ""Filter the res
+0000c5d0: 756c 7473 2064 6f77 6e20 746f 2065 7665  ults down to eve
+0000c5e0: 6e20 6f75 7463 6f6d 6573 2073 6f20 7468  n outcomes so th
+0000c5f0: 6174 2070 6c6f 7474 6564 2072 6573 756c  at plotted resul
+0000c600: 7473 2077 696c 6c20 6265 206d 6561 6e69  ts will be meani
+0000c610: 6e67 6675 6c2e 0a0a 2020 2020 2020 2020  ngful...        
+0000c620: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+0000c630: 2020 6e3a 2054 6865 206e 756d 6265 7220    n: The number 
+0000c640: 6f66 2069 6e74 6572 6163 7469 6f6e 7320  of interactions 
+0000c650: 6120 7370 6563 6966 6963 2065 7661 6c75  a specific evalu
+0000c660: 6174 696f 6e20 6d75 7374 2068 6176 6520  ation must have 
+0000c670: 284e 6f6e 6520 696e 6469 6361 7465 7320  (None indicates 
+0000c680: 6e6f 2063 6f6e 7374 7261 696e 7429 2e0a  no constraint)..
+0000c690: 2020 2020 2020 2020 2020 2020 6c3a 2054              l: T
+0000c6a0: 6865 206c 6576 656c 2061 7420 7768 6963  he level at whic
+0000c6b0: 6820 7765 2077 6973 6820 746f 2063 6f6d  h we wish to com
+0000c6c0: 7061 7265 2065 7661 6c61 7469 6f6e 206f  pare evalation o
+0000c6d0: 7574 636f 6d65 7320 2865 2e67 2e2c 2027  utcomes (e.g., '
+0000c6e0: 6c65 6172 6e65 725f 6964 2729 2e0a 2020  learner_id')..  
+0000c6f0: 2020 2020 2020 2020 2020 703a 2054 6865            p: The
+0000c700: 2070 6169 7273 2074 6861 7420 6d75 7374   pairs that must
+0000c710: 2065 7869 7374 2061 6372 6f73 7320 616c   exist across al
+0000c720: 6c20 606c 6020 696e 206f 7264 6572 2074  l `l` in order t
+0000c730: 6f20 6265 2069 6e63 6c75 6465 6420 2865  o be included (e
+0000c740: 2e67 2e2c 2027 656e 7669 726f 6e6d 656e  .g., 'environmen
+0000c750: 745f 6964 2729 2e0a 0a20 2020 2020 2020  t_id')...       
+0000c760: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000c770: 2020 2020 2020 4120 6052 6573 756c 7460        A `Result`
+0000c780: 2077 6865 7265 2061 6e20 606c 6020 6578   where an `l` ex
+0000c790: 6973 7473 2066 6f72 2065 7665 7279 2060  ists for every `
+0000c7a0: 7060 2061 6e64 2061 6c6c 2060 7060 2068  p` and all `p` h
+0000c7b0: 6176 6520 276e 2720 696e 7465 7261 6374  ave 'n' interact
+0000c7c0: 696f 6e73 2e0a 2020 2020 2020 2020 2222  ions..        ""
+0000c7d0: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000c7e0: 6e20 7365 6c66 2e66 696c 7465 725f 6669  n self.filter_fi
+0000c7f0: 6e28 6e2c 6c2c 7029 0a0a 2020 2020 6465  n(n,l,p)..    de
+0000c800: 6620 7768 6572 6528 7365 6c66 2c20 2a2a  f where(self, **
+0000c810: 6b77 6172 6773 2920 2d3e 2027 5265 7375  kwargs) -> 'Resu
+0000c820: 6c74 273a 0a20 2020 2020 2020 2022 2222  lt':.        """
+0000c830: 5365 6c65 6374 206c 6561 726e 6572 732f  Select learners/
+0000c840: 656e 7669 726f 6e6d 656e 7473 2f65 7661  environments/eva
+0000c850: 6c75 6174 6f72 732e 0a0a 2020 2020 2020  luators...      
+0000c860: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000c870: 2020 2020 6b77 6172 6773 3a20 416e 7920      kwargs: Any 
+0000c880: 636f 6c75 6d6e 2069 6e20 656e 7669 726f  column in enviro
+0000c890: 6e6d 656e 7473 2c20 6c65 6172 6e65 7273  nments, learners
+0000c8a0: 2c20 616e 6420 6576 616c 7561 746f 7273  , and evaluators
+0000c8b0: 2074 6f20 6669 6c74 6572 206f 6e2e 2042   to filter on. B
+0000c8c0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+0000c8d0: 2020 6465 6661 756c 7420 636f 6d70 6172    default compar
+0000c8e0: 6973 6f6e 206f 7065 7261 746f 7273 2061  ison operators a
+0000c8f0: 7265 2065 6974 6865 7220 2765 7175 616c  re either 'equal
+0000c900: 2720 6f72 2027 696e 272e 2046 6f72 2065  ' or 'in'. For e
+0000c910: 7861 6d70 6c65 2c0a 2020 2020 2020 2020  xample,.        
+0000c920: 2020 2020 2020 2020 7768 6572 6528 656e          where(en
+0000c930: 7669 726f 6e6d 656e 745f 6964 3d31 2920  vironment_id=1) 
+0000c940: 776f 756c 6420 7265 7475 726e 2061 2052  would return a R
+0000c950: 6573 756c 7420 7768 6572 6520 656e 7669  esult where envi
+0000c960: 726f 6e6d 656e 7473 206f 6e6c 7920 636f  ronments only co
+0000c970: 6e74 6169 6e73 0a20 2020 2020 2020 2020  ntains.         
+0000c980: 2020 2020 2020 2065 6e76 6972 6f6e 6d65         environme
+0000c990: 6e74 5f69 6420 312e 204f 6e20 7468 6520  nt_id 1. On the 
+0000c9a0: 6f74 6865 7220 6861 6e64 2077 6865 7265  other hand where
+0000c9b0: 2865 6e76 6972 6f6e 6d65 6e74 5f69 643d  (environment_id=
+0000c9c0: 5b31 2c32 5d29 2077 6f75 6c64 2072 6574  [1,2]) would ret
+0000c9d0: 7572 6e20 610a 2020 2020 2020 2020 2020  urn a.          
+0000c9e0: 2020 2020 2020 5265 7375 6c74 2077 6865        Result whe
+0000c9f0: 7265 2065 6e76 6972 6f6e 6d65 6e74 7320  re environments 
+0000ca00: 636f 6e74 6169 6e73 2065 6e76 6972 6f6e  contains environ
+0000ca10: 6d65 6e74 5f69 6420 3120 616e 6420 322e  ment_id 1 and 2.
+0000ca20: 2054 6865 206b 6579 776f 7264 7320 6d75   The keywords mu
+0000ca30: 7374 0a20 2020 2020 2020 2020 2020 2020  st.             
+0000ca40: 2020 2069 6e64 6963 6174 6520 6120 636f     indicate a co
+0000ca50: 6c75 6d6e 206e 616d 6520 696e 2065 6974  lumn name in eit
+0000ca60: 6865 7220 656e 7669 726f 6e6d 656e 7473  her environments
+0000ca70: 2c20 6c65 6172 6e65 7273 2c20 6576 616c  , learners, eval
+0000ca80: 7561 746f 7273 2c20 6f72 0a20 2020 2020  uators, or.     
+0000ca90: 2020 2020 2020 2020 2020 2069 6e74 6572             inter
+0000caa0: 6163 7469 6f6e 732e 2053 7570 706f 7274  actions. Support
+0000cab0: 6564 2063 6f6d 7061 7269 736f 6e20 6f70  ed comparison op
+0000cac0: 6572 6174 6f72 7320 6172 6520 273d 272c  erators are '=',
+0000cad0: 2721 3d27 2c27 3c3d 272c 273c 272c 273e  '!=','<=','<','>
+0000cae0: 272c 273e 3d27 2c0a 2020 2020 2020 2020  ','>=',.        
+0000caf0: 2020 2020 2020 2020 276d 6174 6368 272c          'match',
+0000cb00: 2769 6e27 2c27 2169 6e27 2e20 546f 2069  'in','!in'. To i
+0000cb10: 6e64 6963 6174 6520 616e 2065 7870 6c69  ndicate an expli
+0000cb20: 6369 7420 6f70 6572 6174 6f72 2075 7365  cit operator use
+0000cb30: 2061 2064 6963 7469 6f6e 6172 792e 2046   a dictionary. F
+0000cb40: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
+0000cb50: 2020 2065 7861 6d70 6c65 2c20 7768 6572     example, wher
+0000cb60: 6528 656e 7669 726f 6e6d 656e 745f 6964  e(environment_id
+0000cb70: 3d7b 273c 3d27 3a31 3030 7d29 2077 6f75  ={'<=':100}) wou
+0000cb80: 6c64 2072 6574 7572 6e20 6120 5265 7375  ld return a Resu
+0000cb90: 6c74 2077 6974 6820 616c 6c0a 2020 2020  lt with all.    
+0000cba0: 2020 2020 2020 2020 2020 2020 656e 7669              envi
+0000cbb0: 726f 6e6d 656e 7473 2077 686f 7365 2065  ronments whose e
+0000cbc0: 6e76 6972 6f6e 6d65 6e74 5f69 6420 3c3d  nvironment_id <=
+0000cbd0: 2031 3030 2e20 496e 636c 7564 696e 6720   100. Including 
+0000cbe0: 6d75 6c74 6970 6c65 206b 7761 7267 7320  multiple kwargs 
+0000cbf0: 696e 2061 0a20 2020 2020 2020 2020 2020  in a.           
+0000cc00: 2020 2020 2073 696e 676c 6520 7768 6572       single wher
+0000cc10: 6520 6170 706c 6965 7320 616e 206f 7220  e applies an or 
+0000cc20: 636f 6e6a 7563 7469 6f6e 2e20 4368 6169  conjuction. Chai
+0000cc30: 6e69 6e67 2077 6865 7265 2073 7461 7465  ning where state
+0000cc40: 6d65 6e74 7320 6973 2065 7175 6976 616c  ments is equival
+0000cc50: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
+0000cc60: 2020 2020 746f 2061 6e20 616e 6420 636f      to an and co
+0000cc70: 6e6a 7563 746f 722e 0a0a 2020 2020 2020  njuctor...      
+0000cc80: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000cc90: 2020 2020 2020 2041 2060 5265 7375 6c74         A `Result
+0000cca0: 6020 7768 6f73 6520 656e 7669 726f 6e6d  ` whose environm
+0000ccb0: 656e 7473 2c20 6c65 6172 6e65 7273 2c20  ents, learners, 
+0000ccc0: 6576 616c 7561 746f 7273 2c20 616e 6420  evaluators, and 
+0000ccd0: 696e 7465 7261 6374 696f 6e73 2073 6174  interactions sat
+0000cce0: 6973 6679 2074 6865 0a20 2020 2020 2020  isfy the.       
+0000ccf0: 2020 2020 2020 2020 2077 6865 7265 2073           where s
+0000cd00: 656c 6563 746f 7273 2e0a 2020 2020 2020  electors..      
+0000cd10: 2020 2222 220a 2020 2020 2020 2020 656e    """.        en
+0000cd20: 765f 6b77 6172 6773 203d 207b 7d0a 2020  v_kwargs = {}.  
+0000cd30: 2020 2020 2020 6c72 6e5f 6b77 6172 6773        lrn_kwargs
+0000cd40: 203d 207b 7d0a 2020 2020 2020 2020 7661   = {}.        va
+0000cd50: 6c5f 6b77 6172 6773 203d 207b 7d0a 2020  l_kwargs = {}.  
+0000cd60: 2020 2020 2020 696e 745f 6b77 6172 6773        int_kwargs
+0000cd70: 203d 207b 7d0a 0a20 2020 2020 2020 2066   = {}..        f
+0000cd80: 6f72 206b 6579 2c61 7267 2069 6e20 6b77  or key,arg in kw
+0000cd90: 6172 6773 2e69 7465 6d73 2829 3a0a 2020  args.items():.  
+0000cda0: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+0000cdb0: 2069 6e20 7365 6c66 2e65 6e76 6972 6f6e   in self.environ
+0000cdc0: 6d65 6e74 732e 636f 6c75 6d6e 733a 0a20  ments.columns:. 
+0000cdd0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000cde0: 6e76 5f6b 7761 7267 735b 6b65 795d 203d  nv_kwargs[key] =
+0000cdf0: 2061 7267 0a20 2020 2020 2020 2020 2020   arg.           
+0000ce00: 2065 6c69 6620 6b65 7920 696e 2073 656c   elif key in sel
+0000ce10: 662e 6c65 6172 6e65 7273 2e63 6f6c 756d  f.learners.colum
+0000ce20: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000ce30: 2020 2020 6c72 6e5f 6b77 6172 6773 5b6b      lrn_kwargs[k
+0000ce40: 6579 5d20 3d20 6172 670a 2020 2020 2020  ey] = arg.      
+0000ce50: 2020 2020 2020 656c 6966 206b 6579 2069        elif key i
+0000ce60: 6e20 7365 6c66 2e65 7661 6c75 6174 6f72  n self.evaluator
+0000ce70: 732e 636f 6c75 6d6e 733a 0a20 2020 2020  s.columns:.     
+0000ce80: 2020 2020 2020 2020 2020 2076 616c 5f6b             val_k
+0000ce90: 7761 7267 735b 6b65 795d 203d 2061 7267  wargs[key] = arg
+0000cea0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000ceb0: 6620 6b65 7920 696e 2073 656c 662e 696e  f key in self.in
+0000cec0: 7465 7261 6374 696f 6e73 2e63 6f6c 756d  teractions.colum
+0000ced0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000cee0: 2020 2020 696e 745f 6b77 6172 6773 5b6b      int_kwargs[k
+0000cef0: 6579 5d20 3d20 6172 670a 2020 2020 2020  ey] = arg.      
+0000cf00: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000cf10: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000cf20: 6520 436f 6261 4578 6365 7074 696f 6e28  e CobaException(
+0000cf30: 2241 6e20 756e 7265 636f 676e 697a 6564  "An unrecognized
+0000cf40: 2063 6f6c 756d 6e20 7761 7320 7072 6f76   column was prov
+0000cf50: 6964 6564 2074 6f20 6077 6865 7265 6020  ided to `where` 
+0000cf60: 666f 7220 6669 6c74 6572 696e 672e 2229  for filtering.")
+0000cf70: 0a0a 2020 2020 2020 2020 6f75 7420 3d20  ..        out = 
+0000cf80: 7365 6c66 0a0a 2020 2020 2020 2020 6966  self..        if
+0000cf90: 2065 6e76 5f6b 7761 7267 733a 206f 7574   env_kwargs: out
+0000cfa0: 203d 206f 7574 2e66 696c 7465 725f 656e   = out.filter_en
+0000cfb0: 7628 2a2a 656e 765f 6b77 6172 6773 290a  v(**env_kwargs).
+0000cfc0: 2020 2020 2020 2020 6966 206c 726e 5f6b          if lrn_k
+0000cfd0: 7761 7267 733a 206f 7574 203d 206f 7574  wargs: out = out
+0000cfe0: 2e66 696c 7465 725f 6c72 6e28 2a2a 6c72  .filter_lrn(**lr
+0000cff0: 6e5f 6b77 6172 6773 290a 2020 2020 2020  n_kwargs).      
+0000d000: 2020 6966 2076 616c 5f6b 7761 7267 733a    if val_kwargs:
+0000d010: 206f 7574 203d 206f 7574 2e66 696c 7465   out = out.filte
+0000d020: 725f 7661 6c28 2a2a 7661 6c5f 6b77 6172  r_val(**val_kwar
+0000d030: 6773 290a 2020 2020 2020 2020 6966 2069  gs).        if i
+0000d040: 6e74 5f6b 7761 7267 733a 206f 7574 203d  nt_kwargs: out =
+0000d050: 206f 7574 2e66 696c 7465 725f 696e 7428   out.filter_int(
+0000d060: 2a2a 696e 745f 6b77 6172 6773 290a 0a20  **int_kwargs).. 
+0000d070: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
+0000d080: 740a 0a20 2020 2064 6566 2072 6177 5f6c  t..    def raw_l
+0000d090: 6561 726e 6572 7328 7365 6c66 2c0a 2020  earners(self,.  
+0000d0a0: 2020 2020 2020 7820 2020 3a20 556e 696f        x   : Unio
+0000d0b0: 6e5b 7374 722c 2053 6571 7565 6e63 655b  n[str, Sequence[
+0000d0c0: 7374 725d 5d20 3d20 2769 6e64 6578 272c  str]] = 'index',
+0000d0d0: 0a20 2020 2020 2020 2079 2020 203a 2073  .        y   : s
+0000d0e0: 7472 2020 2020 2020 2020 2020 2020 2020  tr              
+0000d0f0: 2020 2020 2020 2020 203d 2027 7265 7761           = 'rewa
+0000d100: 7264 272c 0a20 2020 2020 2020 206c 2020  rd',.        l  
+0000d110: 203a 2055 6e69 6f6e 5b73 7472 2c20 5365   : Union[str, Se
+0000d120: 7175 656e 6365 5b73 7472 5d5d 203d 2027  quence[str]] = '
+0000d130: 6675 6c6c 5f6e 616d 6527 2c0a 2020 2020  full_name',.    
+0000d140: 2020 2020 7020 2020 3a20 556e 696f 6e5b      p   : Union[
+0000d150: 7374 722c 2053 6571 7565 6e63 655b 7374  str, Sequence[st
+0000d160: 725d 5d20 3d20 2765 6e76 6972 6f6e 6d65  r]] = 'environme
+0000d170: 6e74 5f69 6427 2c0a 2020 2020 2020 2020  nt_id',.        
+0000d180: 7370 616e 3a20 696e 7420 3d20 4e6f 6e65  span: int = None
+0000d190: 2920 2d3e 2054 6162 6c65 3a0a 2020 2020  ) -> Table:.    
+0000d1a0: 2020 2020 2222 2241 2054 6162 6c65 2077      """A Table w
+0000d1b0: 6974 6820 7468 6520 7261 7720 6461 7461  ith the raw data
+0000d1c0: 2075 7365 6420 666f 7220 706c 6f74 5f6c   used for plot_l
+0000d1d0: 6561 726e 6572 732e 0a0a 2020 2020 2020  earners...      
+0000d1e0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000d1f0: 2020 2020 783a 2054 6865 2076 6172 6961      x: The varia
+0000d200: 626c 6573 2074 6f20 706c 6f74 206f 6e20  bles to plot on 
+0000d210: 7468 6520 782d 6178 6973 2e0a 2020 2020  the x-axis..    
+0000d220: 2020 2020 2020 2020 793a 2054 6865 2076          y: The v
+0000d230: 6172 6961 626c 6520 746f 2070 6c6f 7420  ariable to plot 
+0000d240: 6f6e 2074 6865 2079 2d61 7869 732e 0a20  on the y-axis.. 
+0000d250: 2020 2020 2020 2020 2020 206c 3a20 5468             l: Th
+0000d260: 6520 6c61 6265 6c73 2074 6f20 7573 6520  e labels to use 
+0000d270: 696e 2074 6865 2070 6c6f 7420 6c65 6765  in the plot lege
+0000d280: 6e64 2e0a 2020 2020 2020 2020 2020 2020  nd..            
+0000d290: 703a 2054 6865 2070 6169 7269 6e67 7320  p: The pairings 
+0000d2a0: 746f 2072 6571 7569 7265 2061 6372 6f73  to require acros
+0000d2b0: 7320 616c 6c20 6c2e 2049 6620 4e6f 6e65  s all l. If None
+0000d2c0: 206e 6f20 7061 6972 696e 6720 6368 6563   no pairing chec
+0000d2d0: 6b73 2061 7265 2070 6572 666f 726d 6564  ks are performed
+0000d2e0: 2e0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
+0000d2f0: 616e 3a20 5468 6520 7369 7a65 206f 6620  an: The size of 
+0000d300: 7468 6520 726f 6c6c 696e 6720 6176 6572  the rolling aver
+0000d310: 6167 6520 284e 6f6e 6520 6d65 616e 7320  age (None means 
+0000d320: 7072 6f67 7265 7373 6976 6520 6d65 616e  progressive mean
+0000d330: 2e29 0a0a 2020 2020 2020 2020 5265 7475  .)..        Retu
+0000d340: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000d350: 2041 2054 6162 6c65 2077 6974 6820 7468   A Table with th
+0000d360: 6520 7261 7720 6461 7461 2075 7365 6420  e raw data used 
+0000d370: 746f 2063 6f6e 7374 7275 6374 2070 6c6f  to construct plo
+0000d380: 745f 6c65 6172 6e65 7273 2e0a 2020 2020  t_learners..    
+0000d390: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+0000d3a0: 2069 6620 703a 2070 6c6f 7474 6162 6c65   if p: plottable
+0000d3b0: 203d 2073 656c 662e 5f70 6c6f 7474 6162   = self._plottab
+0000d3c0: 6c65 2878 2c79 292e 5f66 696e 6973 6865  le(x,y)._finishe
+0000d3d0: 6428 782c 792c 6c2c 7029 0a20 2020 2020  d(x,y,l,p).     
+0000d3e0: 2020 2065 6c73 653a 2070 6c6f 7474 6162     else: plottab
+0000d3f0: 6c65 203d 2073 656c 662e 5f70 6c6f 7474  le = self._plott
+0000d400: 6162 6c65 2878 2c79 290a 0a20 2020 2020  able(x,y)..     
+0000d410: 2020 2072 6f77 7320 3d20 706c 6f74 7461     rows = plotta
+0000d420: 626c 652e 5f67 726f 7570 6564 5f79 7328  ble._grouped_ys(
+0000d430: 6c2c 782c 793d 792c 7370 616e 3d73 7061  l,x,y=y,span=spa
+0000d440: 6e29 0a0a 2020 2020 2020 2020 5873 203d  n)..        Xs =
+0000d450: 2073 6574 286d 6170 2869 7465 6d67 6574   set(map(itemget
+0000d460: 7465 7228 3129 2c72 6f77 7329 290a 0a20  ter(1),rows)).. 
+0000d470: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000d480: 2020 2020 2020 2020 5873 203d 2064 6963          Xs = dic
+0000d490: 7428 7a69 7028 736f 7274 6564 2858 7329  t(zip(sorted(Xs)
+0000d4a0: 2c63 6f75 6e74 2829 2929 0a20 2020 2020  ,count())).     
+0000d4b0: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+0000d4c0: 2020 2020 2020 2058 7320 3d20 6469 6374         Xs = dict
+0000d4d0: 287a 6970 2873 6f72 7465 6428 5873 2c6b  (zip(sorted(Xs,k
+0000d4e0: 6579 3d73 7472 292c 636f 756e 7428 2929  ey=str),count())
+0000d4f0: 290a 0a20 2020 2020 2020 2074 7279 3a0a  )..        try:.
+0000d500: 2020 2020 2020 2020 2020 2020 726f 7773              rows
+0000d510: 203d 2073 6f72 7465 6428 726f 7773 290a   = sorted(rows).
+0000d520: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
+0000d530: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+0000d540: 6564 5f20 3d20 4661 6c73 650a 2020 2020  ed_ = False.    
+0000d550: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000d560: 2020 2020 2020 736f 7274 6564 5f20 3d20        sorted_ = 
+0000d570: 5472 7565 0a0a 2020 2020 2020 2020 6461  True..        da
+0000d580: 7461 203d 207b 2778 273a 206c 6973 7428  ta = {'x': list(
+0000d590: 5873 2e6b 6579 7328 2929 7d0a 2020 2020  Xs.keys())}.    
+0000d5a0: 2020 2020 666f 7220 5f6c 2c20 6772 6f75      for _l, grou
+0000d5b0: 7020 696e 2067 726f 7570 6572 2872 6f77  p in grouper(row
+0000d5c0: 732c 206b 6579 3d69 7465 6d67 6574 7465  s, key=itemgette
+0000d5d0: 7228 3029 2c20 7661 6c3d 6974 656d 6765  r(0), val=itemge
+0000d5e0: 7474 6572 2873 6c69 6365 2831 2c4e 6f6e  tter(slice(1,Non
+0000d5f0: 6529 292c 2073 6f72 7465 645f 3d73 6f72  e)), sorted_=sor
+0000d600: 7465 645f 293a 0a20 2020 2020 2020 2020  ted_):.         
+0000d610: 2020 2059 203d 205b 5b66 6c6f 6174 2827     Y = [[float('
+0000d620: 6e61 6e27 295d 5d2a 6c65 6e28 5873 290a  nan')]]*len(Xs).
+0000d630: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000d640: 5f78 2c20 6772 6f75 7020 696e 2067 726f  _x, group in gro
+0000d650: 7570 6572 2867 726f 7570 2c20 6b65 793d  uper(group, key=
+0000d660: 6974 656d 6765 7474 6572 2830 292c 2076  itemgetter(0), v
+0000d670: 616c 3d69 7465 6d67 6574 7465 7228 3129  al=itemgetter(1)
+0000d680: 2c20 736f 7274 6564 5f3d 736f 7274 6564  , sorted_=sorted
+0000d690: 5f29 3a0a 2020 2020 2020 2020 2020 2020  _):.            
+0000d6a0: 2020 2020 595b 5873 5b5f 785d 5d20 3d20      Y[Xs[_x]] = 
+0000d6b0: 6c69 7374 2863 6861 696e 2e66 726f 6d5f  list(chain.from_
+0000d6c0: 6974 6572 6162 6c65 2867 726f 7570 2929  iterable(group))
+0000d6d0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000d6e0: 615b 5f6c 5d20 3d20 590a 2020 2020 2020  a[_l] = Y.      
+0000d6f0: 2020 7265 7475 726e 2054 6162 6c65 2864    return Table(d
+0000d700: 6174 6129 0a0a 2020 2020 6465 6620 7261  ata)..    def ra
+0000d710: 775f 636f 6e74 7261 7374 2873 656c 662c  w_contrast(self,
+0000d720: 0a20 2020 2020 2020 206c 3120 203a 2041  .        l1  : A
+0000d730: 6e79 2c0a 2020 2020 2020 2020 6c32 2020  ny,.        l2  
+0000d740: 3a20 416e 792c 0a20 2020 2020 2020 2078  : Any,.        x
+0000d750: 2020 203a 2055 6e69 6f6e 5b73 7472 2c20     : Union[str, 
+0000d760: 5365 7175 656e 6365 5b73 7472 5d5d 203d  Sequence[str]] =
+0000d770: 2027 656e 7669 726f 6e6d 656e 745f 6964   'environment_id
+0000d780: 272c 0a20 2020 2020 2020 2079 2020 203a  ',.        y   :
+0000d790: 2073 7472 2020 2020 2020 2020 2020 2020   str            
+0000d7a0: 2020 2020 2020 2020 2020 203d 2027 7265             = 're
+0000d7b0: 7761 7264 272c 0a20 2020 2020 2020 206c  ward',.        l
+0000d7c0: 2020 203a 2055 6e69 6f6e 5b73 7472 2c20     : Union[str, 
+0000d7d0: 5365 7175 656e 6365 5b73 7472 5d5d 203d  Sequence[str]] =
+0000d7e0: 2027 6c65 6172 6e65 725f 6964 272c 0a20   'learner_id',. 
+0000d7f0: 2020 2020 2020 2070 2020 203a 2055 6e69         p   : Uni
+0000d800: 6f6e 5b73 7472 2c20 5365 7175 656e 6365  on[str, Sequence
+0000d810: 5b73 7472 5d5d 203d 2027 656e 7669 726f  [str]] = 'enviro
+0000d820: 6e6d 656e 745f 6964 272c 0a20 2020 2020  nment_id',.     
+0000d830: 2020 2073 7061 6e3a 2069 6e74 203d 204e     span: int = N
+0000d840: 6f6e 6529 202d 3e20 5461 626c 653a 0a20  one) -> Table:. 
+0000d850: 2020 2020 2020 2022 2222 4120 5461 626c         """A Tabl
+0000d860: 6520 7769 7468 2074 6865 2072 6177 2064  e with the raw d
+0000d870: 6174 6120 706c 6f74 5f63 6f6e 7472 6173  ata plot_contras
+0000d880: 742e 0a0a 2020 2020 2020 2020 4172 6773  t...        Args
+0000d890: 3a0a 2020 2020 2020 2020 2020 2020 6c31  :.            l1
+0000d8a0: 3a20 5468 6520 6669 7273 7420 606c 6020  : The first `l` 
+0000d8b0: 7661 6c75 6520 746f 2063 6f6e 7472 6173  value to contras
+0000d8c0: 742e 0a20 2020 2020 2020 2020 2020 206c  t..            l
+0000d8d0: 323a 2074 6865 2073 6563 6f6e 6420 606c  2: the second `l
+0000d8e0: 6020 7661 6c75 6520 746f 2063 6f6e 7472  ` value to contr
+0000d8f0: 6173 742e 0a20 2020 2020 2020 2020 2020  ast..           
+0000d900: 2078 3a20 5468 6520 7661 7269 6162 6c65   x: The variable
+0000d910: 7320 746f 2070 6c6f 7420 6f6e 2074 6865  s to plot on the
+0000d920: 2078 2d61 7869 732e 0a20 2020 2020 2020   x-axis..       
+0000d930: 2020 2020 2079 3a20 5468 6520 7661 7269       y: The vari
+0000d940: 6162 6c65 2074 6f20 706c 6f74 206f 6e20  able to plot on 
+0000d950: 7468 6520 792d 6178 6973 2e0a 2020 2020  the y-axis..    
+0000d960: 2020 2020 2020 2020 6c3a 2054 6865 2063          l: The c
+0000d970: 6f6c 756d 6e20 6e61 6d65 7320 7468 6174  olumn names that
+0000d980: 206c 3120 616e 6420 6c32 2072 6570 7265   l1 and l2 repre
+0000d990: 7365 6e74 2e0a 2020 2020 2020 2020 2020  sent..          
+0000d9a0: 2020 703a 2054 6865 2070 6169 7269 6e67    p: The pairing
+0000d9b0: 7320 746f 2072 6571 7569 7265 2061 6372  s to require acr
+0000d9c0: 6f73 7320 616c 6c20 6c31 2061 6e64 206c  oss all l1 and l
+0000d9d0: 322e 0a20 2020 2020 2020 2020 2020 2073  2..            s
+0000d9e0: 7061 6e3a 2054 6865 2073 697a 6520 6f66  pan: The size of
+0000d9f0: 2074 6865 2072 6f6c 6c69 6e67 2061 7665   the rolling ave
+0000da00: 7261 6765 2028 4e6f 6e65 206d 6561 6e73  rage (None means
+0000da10: 2070 726f 6772 6573 7369 7665 206d 6561   progressive mea
+0000da20: 6e29 2e0a 0a20 2020 2020 2020 2045 7861  n)...        Exa
+0000da30: 6d70 6c65 733a 0a20 2020 2020 2020 2020  mples:.         
+0000da40: 2020 2072 6177 5f63 6f6e 7472 6173 7428     raw_contrast(
+0000da50: 312c 322c 783d 2765 6e76 6972 6f6e 6d65  1,2,x='environme
+0000da60: 6e74 5f69 6427 2c79 3d27 7265 7761 7264  nt_id',y='reward
+0000da70: 272c 6c3d 276c 6561 726e 6572 5f69 6427  ',l='learner_id'
+0000da80: 2c70 3d27 656e 7669 726f 6e6d 656e 745f  ,p='environment_
+0000da90: 6964 2729 0a20 2020 2020 2020 2020 2020  id').           
+0000daa0: 2077 6f75 6c64 2063 6f6e 7472 6173 7420   would contrast 
+0000dab0: 6c65 6172 6e65 725f 6964 3d31 2061 6e64  learner_id=1 and
+0000dac0: 206c 6561 726e 6572 5f69 643d 3220 696e   learner_id=2 in
+0000dad0: 2074 6572 6d73 206f 6620 7265 7761 7264   terms of reward
+0000dae0: 206f 6e20 616c 6c20 656e 7669 726f 6e6d   on all environm
+0000daf0: 656e 745f 6964 732e 0a0a 2020 2020 2020  ent_ids...      
+0000db00: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000db10: 2020 2020 2020 2041 2054 6162 6c65 2077         A Table w
+0000db20: 6974 6820 7468 6520 7261 7720 6461 7461  ith the raw data
+0000db30: 2075 7365 6420 746f 2063 6f6e 7374 7275   used to constru
+0000db40: 6374 2070 6c6f 745f 636f 6e74 7261 7374  ct plot_contrast
+0000db50: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+0000db60: 2020 2020 2020 206f 675f 6c20 3d20 286c         og_l = (l
+0000db70: 312c 6c32 290a 0a20 2020 2020 2020 206c  1,l2)..        l
+0000db80: 6973 745f 6c69 6b65 3d28 6c69 7374 2c74  ist_like=(list,t
+0000db90: 7570 6c65 290a 0a20 2020 2020 2020 2069  uple)..        i
+0000dba0: 6620 2020 2020 6973 696e 7374 616e 6365  f     isinstance
+0000dbb0: 286c 2c6c 6973 745f 6c69 6b65 2920 616e  (l,list_like) an
+0000dbc0: 6420 6e6f 7420 6973 696e 7374 616e 6365  d not isinstance
+0000dbd0: 286c 315b 305d 2c6c 6973 745f 6c69 6b65  (l1[0],list_like
+0000dbe0: 293a 206c 3120 3d20 5b6c 315d 0a20 2020  ): l1 = [l1].   
+0000dbf0: 2020 2020 2069 6620 2020 2020 6973 696e       if     isin
+0000dc00: 7374 616e 6365 286c 2c6c 6973 745f 6c69  stance(l,list_li
+0000dc10: 6b65 2920 616e 6420 6e6f 7420 6973 696e  ke) and not isin
+0000dc20: 7374 616e 6365 286c 325b 305d 2c6c 6973  stance(l2[0],lis
+0000dc30: 745f 6c69 6b65 293a 206c 3220 3d20 5b6c  t_like): l2 = [l
+0000dc40: 325d 0a20 2020 2020 2020 2069 6620 6e6f  2].        if no
+0000dc50: 7420 6973 696e 7374 616e 6365 286c 2c6c  t isinstance(l,l
+0000dc60: 6973 745f 6c69 6b65 2920 616e 6420 6e6f  ist_like) and no
+0000dc70: 7420 6973 696e 7374 616e 6365 286c 3120  t isinstance(l1 
+0000dc80: 2020 2c6c 6973 745f 6c69 6b65 293a 206c    ,list_like): l
+0000dc90: 3120 3d20 5b6c 315d 0a20 2020 2020 2020  1 = [l1].       
+0000dca0: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+0000dcb0: 6365 286c 2c6c 6973 745f 6c69 6b65 2920  ce(l,list_like) 
+0000dcc0: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
+0000dcd0: 6365 286c 3220 2020 2c6c 6973 745f 6c69  ce(l2   ,list_li
+0000dce0: 6b65 293a 206c 3220 3d20 5b6c 325d 0a0a  ke): l2 = [l2]..
+0000dcf0: 2020 2020 2020 2020 6966 2061 6e79 285f          if any(_
+0000dd00: 6c31 2069 6e20 6c32 2066 6f72 205f 6c31  l1 in l2 for _l1
+0000dd10: 2069 6e20 6c31 293a 0a20 2020 2020 2020   in l1):.       
+0000dd20: 2020 2020 2072 6169 7365 2043 6f62 6145       raise CobaE
+0000dd30: 7863 6570 7469 6f6e 2822 4120 7661 6c75  xception("A valu
+0000dd40: 6520 6361 6e6e 6f74 2062 6520 696e 2062  e cannot be in b
+0000dd50: 6f74 6820 606c 3160 2061 6e64 2060 6c32  oth `l1` and `l2
+0000dd60: 602e 2050 6c65 6173 6520 6d61 6b65 2061  `. Please make a
+0000dd70: 2063 6861 6e67 6520 616e 6420 7275 6e20   change and run 
+0000dd80: 6974 2061 6761 696e 2e22 290a 0a20 2020  it again.")..   
+0000dd90: 2020 2020 2070 6c6f 7474 6162 6c65 203d       plottable =
+0000dda0: 2073 656c 662e 5f70 6c6f 7474 6162 6c65   self._plottable
+0000ddb0: 2878 2c79 290a 0a20 2020 2020 2020 204c  (x,y)..        L
+0000ddc0: 312c 4c32 203d 205b 5d2c 5b5d 0a20 2020  1,L2 = [],[].   
+0000ddd0: 2020 2020 2066 6f72 204c 2069 6e20 6368       for L in ch
+0000dde0: 6169 6e28 6c31 2c6c 3229 3a0a 2020 2020  ain(l1,l2):.    
+0000ddf0: 2020 2020 2020 2020 7375 6270 6c6f 7420          subplot 
+0000de00: 3d20 706c 6f74 7461 626c 650a 2020 2020  = plottable.    
+0000de10: 2020 2020 2020 2020 7768 6572 6573 203d          wheres =
+0000de20: 205b 2028 6c2c 4c29 205d 2069 6620 6973   [ (l,L) ] if is
+0000de30: 696e 7374 616e 6365 286c 2c73 7472 2920  instance(l,str) 
+0000de40: 656c 7365 207a 6970 286c 2c4c 290a 0a20  else zip(l,L).. 
+0000de50: 2020 2020 2020 2020 2020 206f 6c64 5f6c             old_l
+0000de60: 6f67 6765 7220 3d20 436f 6261 436f 6e74  ogger = CobaCont
+0000de70: 6578 742e 6c6f 6767 6572 0a20 2020 2020  ext.logger.     
+0000de80: 2020 2020 2020 2043 6f62 6143 6f6e 7465         CobaConte
+0000de90: 7874 2e6c 6f67 6765 7220 3d20 4e75 6c6c  xt.logger = Null
+0000dea0: 4c6f 6767 6572 2829 0a20 2020 2020 2020  Logger().       
+0000deb0: 2020 2020 2066 6f72 206c 5f2c 765f 2069       for l_,v_ i
+0000dec0: 6e20 7768 6572 6573 3a20 7375 6270 6c6f  n wheres: subplo
+0000ded0: 7420 3d20 7375 6270 6c6f 742e 7768 6572  t = subplot.wher
+0000dee0: 6528 2a2a 7b6c 5f3a 765f 7d29 0a20 2020  e(**{l_:v_}).   
+0000def0: 2020 2020 2020 2020 2043 6f62 6143 6f6e           CobaCon
+0000df00: 7465 7874 2e6c 6f67 6765 7220 3d20 6f6c  text.logger = ol
+0000df10: 645f 6c6f 6767 6572 0a0a 2020 2020 2020  d_logger..      
+0000df20: 2020 2020 2020 2377 6520 6172 6520 6173        #we are as
+0000df30: 7375 6d69 6e67 2061 7420 7468 6973 2070  suming at this p
+0000df40: 6f69 6e74 2074 6861 7420 6f6e 6c79 2076  oint that only v
+0000df50: 616c 6964 0a20 2020 2020 2020 2020 2020  alid.           
+0000df60: 2023 606c 6020 6172 6520 6c65 6674 2077   #`l` are left w
+0000df70: 6869 6368 2069 736e 2774 206e 6563 6573  hich isn't neces
+0000df80: 7361 7269 6c79 2074 6865 2063 6173 650a  sarily the case.
+0000df90: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+0000dfa0: 6573 203d 2073 7562 706c 6f74 2e5f 6772  es = subplot._gr
+0000dfb0: 6f75 7065 645f 7973 2870 2c78 2c79 3d79  ouped_ys(p,x,y=y
+0000dfc0: 2c63 6172 643d 2753 272c 7370 616e 3d73  ,card='S',span=s
+0000dfd0: 7061 6e29 0a0a 2020 2020 2020 2020 2020  pan)..          
+0000dfe0: 2020 6966 204c 2069 6e20 6c31 3a20 4c31    if L in l1: L1
+0000dff0: 2e65 7874 656e 6428 7661 6c75 6573 290a  .extend(values).
+0000e000: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000e010: 2020 2020 2020 3a20 4c32 2e65 7874 656e        : L2.exten
+0000e020: 6428 7661 6c75 6573 290a 0a20 2020 2020  d(values)..     
+0000e030: 2020 2023 5765 2068 6176 6520 746f 206d     #We have to m
+0000e040: 6174 6572 6961 6c69 7a65 2062 6563 6175  aterialize becau
+0000e050: 7365 2077 6520 6361 6e27 7420 7265 6c79  se we can't rely
+0000e060: 206f 6e20 736f 7274 696e 670a 2020 2020   on sorting.    
+0000e070: 2020 2020 5031 203d 207b 6b3a 6c69 7374      P1 = {k:list
+0000e080: 2876 2920 666f 7220 6b2c 7620 696e 2067  (v) for k,v in g
+0000e090: 726f 7570 6572 284c 312c 6b65 793d 6974  rouper(L1,key=it
+0000e0a0: 656d 6765 7474 6572 2830 2929 7d0a 2020  emgetter(0))}.  
+0000e0b0: 2020 2020 2020 5032 203d 207b 6b3a 6c69        P2 = {k:li
+0000e0c0: 7374 2876 2920 666f 7220 6b2c 7620 696e  st(v) for k,v in
+0000e0d0: 2067 726f 7570 6572 284c 322c 6b65 793d   grouper(L2,key=
+0000e0e0: 6974 656d 6765 7474 6572 2830 2929 7d0a  itemgetter(0))}.
+0000e0f0: 0a20 2020 2020 2020 2064 6566 206d 616b  .        def mak
+0000e100: 6578 2878 312c 7832 293a 2072 6574 7572  ex(x1,x2): retur
+0000e110: 6e20 7831 2069 6620 7831 203d 3d20 7832  n x1 if x1 == x2
+0000e120: 2065 6c73 6520 6622 7b78 327d 2d7b 7831   else f"{x2}-{x1
+0000e130: 7d22 0a0a 2020 2020 2020 2020 5859 203d  }"..        XY =
+0000e140: 2064 6566 6175 6c74 6469 6374 286c 6973   defaultdict(lis
+0000e150: 7429 0a20 2020 2020 2020 2066 6f72 206b  t).        for k
+0000e160: 2069 6e20 5031 2e6b 6579 7328 2920 2620   in P1.keys() & 
+0000e170: 5032 2e6b 6579 7328 293a 0a20 2020 2020  P2.keys():.     
+0000e180: 2020 2020 2020 2069 6620 7820 3d3d 2027         if x == '
+0000e190: 696e 6465 7827 3a0a 2020 2020 2020 2020  index':.        
+0000e1a0: 2020 2020 2020 2020 666f 7220 6731 5f2c          for g1_,
+0000e1b0: 2067 325f 2069 6e20 7a69 7028 5031 5b6b   g2_ in zip(P1[k
+0000e1c0: 5d2c 5032 5b6b 5d29 3a0a 2020 2020 2020  ],P2[k]):.      
+0000e1d0: 2020 2020 2020 2020 2020 2020 2020 5859                XY
+0000e1e0: 5b67 315f 5b31 5d5d 2e61 7070 656e 6428  [g1_[1]].append(
+0000e1f0: 2867 315f 5b32 5d2c 6732 5f5b 325d 2929  (g1_[2],g2_[2]))
+0000e200: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000e210: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000e220: 2020 2066 6f72 2067 315f 2c67 325f 2069     for g1_,g2_ i
+0000e230: 6e20 7072 6f64 7563 7428 5031 5b6b 5d2c  n product(P1[k],
+0000e240: 5032 5b6b 5d29 3a0a 2020 2020 2020 2020  P2[k]):.        
+0000e250: 2020 2020 2020 2020 2020 2020 5859 5b6d              XY[m
+0000e260: 616b 6578 2867 315f 5b31 5d2c 6732 5f5b  akex(g1_[1],g2_[
+0000e270: 315d 295d 2e61 7070 656e 6428 2867 315f  1])].append((g1_
+0000e280: 5b32 5d2c 6732 5f5b 325d 2929 0a0a 2020  [2],g2_[2]))..  
+0000e290: 2020 2020 2020 6966 206e 6f74 2058 593a        if not XY:
+0000e2a0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000e2b0: 7365 2043 6f62 6145 7863 6570 7469 6f6e  se CobaException
+0000e2c0: 2866 2257 6520 7765 7265 2075 6e61 626c  (f"We were unabl
+0000e2d0: 6520 746f 2063 7265 6174 6520 616e 7920  e to create any 
+0000e2e0: 7061 6972 696e 6773 2074 6f20 636f 6e74  pairings to cont
+0000e2f0: 7261 7374 2e20 4d61 6b65 2073 7572 6520  rast. Make sure 
+0000e300: 6c31 3d7b 6f67 5f6c 5b30 5d7d 2061 6e64  l1={og_l[0]} and
+0000e310: 206c 323d 7b6f 675f 6c5b 315d 7d20 6973   l2={og_l[1]} is
+0000e320: 2063 6f72 7265 6374 2e22 290a 0a20 2020   correct.")..   
+0000e330: 2020 2020 206c 315f 6c61 6265 6c20 3d20       l1_label = 
+0000e340: 7365 6c66 2e5f 6c72 6e5f 6361 6368 655b  self._lrn_cache[
+0000e350: 6c31 5b30 5d5d 5b27 6675 6c6c 5f6e 616d  l1[0]]['full_nam
+0000e360: 6527 5d20 6966 206c 3d3d 276c 6561 726e  e'] if l=='learn
+0000e370: 6572 5f69 6427 2065 6c73 6520 276c 3127  er_id' else 'l1'
+0000e380: 0a20 2020 2020 2020 206c 325f 6c61 6265  .        l2_labe
+0000e390: 6c20 3d20 7365 6c66 2e5f 6c72 6e5f 6361  l = self._lrn_ca
+0000e3a0: 6368 655b 6c32 5b30 5d5d 5b27 6675 6c6c  che[l2[0]]['full
+0000e3b0: 5f6e 616d 6527 5d20 6966 206c 3d3d 276c  _name'] if l=='l
+0000e3c0: 6561 726e 6572 5f69 6427 2065 6c73 6520  earner_id' else 
+0000e3d0: 276c 3227 0a0a 2020 2020 2020 2020 582c  'l2'..        X,
+0000e3e0: 5920 3d20 7a69 7028 2a73 6f72 7465 6428  Y = zip(*sorted(
+0000e3f0: 5859 2e69 7465 6d73 2829 2929 0a0a 2020  XY.items()))..  
+0000e400: 2020 2020 2020 7265 7475 726e 2054 6162        return Tab
+0000e410: 6c65 287b 2778 273a 2058 2c20 286c 315f  le({'x': X, (l1_
+0000e420: 6c61 6265 6c2c 6c32 5f6c 6162 656c 293a  label,l2_label):
+0000e430: 2059 207d 290a 0a20 2020 2064 6566 2070   Y })..    def p
+0000e440: 6c6f 745f 6c65 6172 6e65 7273 2873 656c  lot_learners(sel
+0000e450: 662c 0a20 2020 2020 2020 2078 2020 2020  f,.        x    
+0000e460: 2020 203a 2055 6e69 6f6e 5b73 7472 2c20     : Union[str, 
+0000e470: 5365 7175 656e 6365 5b73 7472 5d5d 203d  Sequence[str]] =
+0000e480: 2027 696e 6465 7827 2c0a 2020 2020 2020   'index',.      
+0000e490: 2020 7920 2020 2020 2020 3a20 7374 7220    y       : str 
+0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4b0: 2020 2020 2020 3d20 2772 6577 6172 6427        = 'reward'
+0000e4c0: 2c0a 2020 2020 2020 2020 6c20 2020 2020  ,.        l     
+0000e4d0: 2020 3a20 556e 696f 6e5b 7374 722c 2053    : Union[str, S
+0000e4e0: 6571 7565 6e63 655b 7374 725d 5d20 3d20  equence[str]] = 
+0000e4f0: 2766 756c 6c5f 6e61 6d65 272c 0a20 2020  'full_name',.   
+0000e500: 2020 2020 2070 2020 2020 2020 203a 2055       p       : U
+0000e510: 6e69 6f6e 5b73 7472 2c20 5365 7175 656e  nion[str, Sequen
+0000e520: 6365 5b73 7472 5d5d 203d 2027 656e 7669  ce[str]] = 'envi
+0000e530: 726f 6e6d 656e 745f 6964 272c 0a20 2020  ronment_id',.   
+0000e540: 2020 2020 2073 7061 6e20 2020 203a 2069       span    : i
+0000e550: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+0000e560: 2020 2065 7272 2020 2020 203a 2055 6e69     err     : Uni
+0000e570: 6f6e 5b4c 6974 6572 616c 5b27 7365 272c  on[Literal['se',
+0000e580: 2773 6427 2c27 6273 272c 2762 6927 5d2c  'sd','bs','bi'],
+0000e590: 2050 6f69 6e74 416e 6449 6e74 6572 7661   PointAndInterva
+0000e5a0: 6c5d 203d 204e 6f6e 652c 0a20 2020 2020  l] = None,.     
+0000e5b0: 2020 2065 7272 6576 6572 793a 2069 6e74     errevery: int
+0000e5c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000e5d0: 206c 6162 656c 7320 203a 2053 6571 7565   labels  : Seque
+0000e5e0: 6e63 655b 7374 725d 203d 204e 6f6e 652c  nce[str] = None,
+0000e5f0: 0a20 2020 2020 2020 2063 6f6c 6f72 7320  .        colors 
+0000e600: 203a 2055 6e69 6f6e 5b69 6e74 2c53 6571   : Union[int,Seq
+0000e610: 7565 6e63 655b 556e 696f 6e5b 7374 722c  uence[Union[str,
+0000e620: 696e 745d 5d5d 203d 204e 6f6e 652c 0a20  int]]] = None,. 
+0000e630: 2020 2020 2020 2074 6974 6c65 2020 203a         title   :
+0000e640: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0000e650: 2020 2020 2078 6c61 6265 6c20 203a 2073       xlabel  : s
+0000e660: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0000e670: 2020 2079 6c61 6265 6c20 203a 2073 7472     ylabel  : str
+0000e680: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000e690: 2078 6c69 6d20 2020 203a 2054 7570 6c65   xlim    : Tuple
+0000e6a0: 5b4f 7074 696f 6e61 6c5b 4e75 6d62 6572  [Optional[Number
+0000e6b0: 5d2c 4f70 7469 6f6e 616c 5b4e 756d 6265  ],Optional[Numbe
+0000e6c0: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
+0000e6d0: 2020 2020 796c 696d 2020 2020 3a20 5475      ylim    : Tu
+0000e6e0: 706c 655b 4f70 7469 6f6e 616c 5b4e 756d  ple[Optional[Num
+0000e6f0: 6265 725d 2c4f 7074 696f 6e61 6c5b 4e75  ber],Optional[Nu
+0000e700: 6d62 6572 5d5d 203d 204e 6f6e 652c 0a20  mber]] = None,. 
+0000e710: 2020 2020 2020 2078 7469 636b 7320 203a         xticks  :
+0000e720: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
+0000e730: 2020 2020 2020 7974 6963 6b73 2020 3a20        yticks  : 
+0000e740: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
+0000e750: 2020 2020 206c 6567 656e 6420 203a 2062       legend  : b
+0000e760: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+0000e770: 2020 2020 616c 7068 6120 2020 3a20 666c      alpha   : fl
+0000e780: 6f61 7420 3d20 312c 0a20 2020 2020 2020  oat = 1,.       
+0000e790: 2078 6f72 6465 7220 203a 204c 6974 6572   xorder  : Liter
+0000e7a0: 616c 5b27 2b27 2c27 2d27 5d20 3d20 4e6f  al['+','-'] = No
+0000e7b0: 6e65 2c0a 2020 2020 2020 2020 746f 705f  ne,.        top_
+0000e7c0: 6e20 2020 3a20 696e 7420 3d20 4e6f 6e65  n   : int = None
+0000e7d0: 2c0a 2020 2020 2020 2020 6f75 7420 2020  ,.        out   
+0000e7e0: 2020 3a20 556e 696f 6e5b 4e6f 6e65 2c4c    : Union[None,L
+0000e7f0: 6974 6572 616c 5b27 7363 7265 656e 275d  iteral['screen']
+0000e800: 2c73 7472 5d20 3d20 2773 6372 6565 6e27  ,str] = 'screen'
+0000e810: 2c0a 2020 2020 2020 2020 6178 203d 204e  ,.        ax = N
+0000e820: 6f6e 6529 202d 3e20 4e6f 6e65 3a0a 2020  one) -> None:.  
+0000e830: 2020 2020 2020 2222 2250 6c6f 7420 7468        """Plot th
+0000e840: 6520 7065 7266 6f72 6d61 6e63 6520 6f66  e performance of
+0000e850: 206d 756c 7469 706c 6520 6c65 6172 6e65   multiple learne
+0000e860: 7273 206f 6e20 6d75 6c74 6970 6c65 2065  rs on multiple e
+0000e870: 6e76 6972 6f6e 6d65 6e74 732e 2049 7420  nvironments. It 
+0000e880: 6769 7665 7320 6120 7365 6e73 6520 6f66  gives a sense of
+0000e890: 2074 6865 0a20 2020 2020 2020 2065 7870   the.        exp
+0000e8a0: 6563 7465 6420 7065 7266 6f72 6d61 6e63  ected performanc
+0000e8b0: 6520 666f 7220 6469 6666 6572 656e 7420  e for different 
+0000e8c0: 6c65 6172 6e65 7273 2061 6372 6f73 7320  learners across 
+0000e8d0: 696e 6465 7065 6e64 656e 7420 656e 7669  independent envi
+0000e8e0: 726f 6e6d 656e 7473 2e20 5468 6973 2070  ronments. This p
+0000e8f0: 6c6f 7420 6973 0a20 2020 2020 2020 2076  lot is.        v
+0000e900: 616c 7561 626c 6520 696e 2067 6169 6e69  aluable in gaini
+0000e910: 6e67 2069 6e73 6967 6874 2069 6e74 6f20  ng insight into 
+0000e920: 686f 7720 7661 7269 6f75 7320 6c65 6172  how various lear
+0000e930: 6e65 7273 2070 6572 666f 726d 2069 6e20  ners perform in 
+0000e940: 636f 6d70 6172 6973 6f6e 2074 6f20 6f6e  comparison to on
+0000e950: 6520 616e 6f74 6865 722e 0a0a 2020 2020  e another...    
+0000e960: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000e970: 2020 2020 2020 783a 2054 6865 2076 616c        x: The val
+0000e980: 7565 7320 746f 2070 6c6f 7420 6f6e 2074  ues to plot on t
+0000e990: 6865 2078 2d61 7869 732e 0a20 2020 2020  he x-axis..     
+0000e9a0: 2020 2020 2020 2079 3a20 5468 6520 7661         y: The va
+0000e9b0: 6c75 6520 746f 2070 6c6f 7420 6f6e 2074  lue to plot on t
+0000e9c0: 6865 2079 2d61 7869 732e 0a20 2020 2020  he y-axis..     
+0000e9d0: 2020 2020 2020 206c 3a20 5468 6520 7661         l: The va
+0000e9e0: 6c75 6573 2074 6f20 706c 6f74 2069 6e20  lues to plot in 
+0000e9f0: 7468 6520 6c65 6765 6e64 2e0a 2020 2020  the legend..    
+0000ea00: 2020 2020 2020 2020 703a 2054 6865 2070          p: The p
+0000ea10: 6169 7273 2074 6861 7420 6d75 7374 2065  airs that must e
+0000ea20: 7869 7374 2061 6372 6f73 7320 616c 6c20  xist across all 
+0000ea30: 6974 656d 7320 696e 2074 6865 206c 6567  items in the leg
+0000ea40: 656e 6420 696e 206f 7264 6572 2074 6f20  end in order to 
+0000ea50: 6265 2069 6e63 6c75 6465 642e 0a20 2020  be included..   
+0000ea60: 2020 2020 2020 2020 2020 2020 2049 6620               If 
+0000ea70: 4e6f 6e65 206e 6f20 7061 6972 696e 6720  None no pairing 
+0000ea80: 2063 6865 636b 7320 6172 6520 7065 7266   checks are perf
+0000ea90: 6f72 6d65 642e 0a20 2020 2020 2020 2020  ormed..         
+0000eaa0: 2020 2073 7061 6e3a 2054 6865 206e 756d     span: The num
+0000eab0: 6265 7220 6f66 2079 2076 616c 7565 7320  ber of y values 
+0000eac0: 746f 2073 6d6f 6f74 6820 746f 6765 7468  to smooth togeth
+0000ead0: 6572 2077 6865 6e20 7265 706f 7274 696e  er when reportin
+0000eae0: 6720 792e 2049 6620 7468 6973 2069 7320  g y. If this is 
+0000eaf0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+0000eb00: 2020 2020 2074 6865 6e20 7468 6520 6176       then the av
+0000eb10: 6572 6167 6520 6f66 2061 6c6c 2079 2076  erage of all y v
+0000eb20: 616c 7565 7320 7570 2074 6f20 6375 7272  alues up to curr
+0000eb30: 656e 7420 6973 2073 686f 776e 206f 7468  ent is shown oth
+0000eb40: 6572 7769 7365 2061 206d 6f76 696e 670a  erwise a moving.
+0000eb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb60: 6176 6572 6167 6520 7769 7468 2077 696e  average with win
+0000eb70: 646f 7720 7369 7a65 206f 6620 7370 616e  dow size of span
+0000eb80: 2028 7468 6520 7769 6e64 6f77 2077 696c   (the window wil
+0000eb90: 6c20 6265 2073 6d61 6c6c 6572 2074 6861  l be smaller tha
+0000eba0: 6e20 7370 616e 2069 6e69 7469 616c 6c79  n span initially
+0000ebb0: 292e 0a20 2020 2020 2020 2020 2020 2065  )..            e
+0000ebc0: 7272 3a20 5468 6973 2064 6574 6572 6d69  rr: This determi
+0000ebd0: 6e65 7320 7768 6174 206b 696e 6420 6f66  nes what kind of
+0000ebe0: 2065 7272 6f72 2062 6172 7320 746f 2070   error bars to p
+0000ebf0: 6c6f 7420 2869 6620 616e 7929 2e20 4966  lot (if any). If
+0000ec00: 2060 4e6f 6e65 6020 7468 656e 206e 6f20   `None` then no 
+0000ec10: 6261 7273 0a20 2020 2020 2020 2020 2020  bars.           
+0000ec20: 2020 2020 2061 7265 2070 6c6f 7474 6564       are plotted
+0000ec30: 2c20 6966 2027 7365 2720 7468 6520 7374  , if 'se' the st
+0000ec40: 616e 6461 7264 2065 7272 6f72 2069 7320  andard error is 
+0000ec50: 7368 6f77 6e2c 2061 6e64 2069 6620 2773  shown, and if 's
+0000ec60: 6427 2074 6865 2073 7461 6e64 6172 6420  d' the standard 
+0000ec70: 6465 7669 6174 696f 6e0a 2020 2020 2020  deviation.      
+0000ec80: 2020 2020 2020 2020 2020 6973 2073 686f            is sho
+0000ec90: 776e 2e0a 2020 2020 2020 2020 2020 2020  wn..            
+0000eca0: 6572 7265 7665 7279 3a20 5468 6973 2064  errevery: This d
+0000ecb0: 6574 6572 6d69 6e65 7320 7468 6520 6672  etermines the fr
+0000ecc0: 6571 7565 6e63 7920 6f66 2065 7272 6f72  equency of error
+0000ecd0: 6261 7273 2e20 4966 2060 4e6f 6e65 6020  bars. If `None` 
+0000ece0: 7468 6579 2061 7070 6561 7220 3525 206f  they appear 5% o
+0000ecf0: 6620 7468 650a 2020 2020 2020 2020 2020  f the.          
+0000ed00: 2020 2020 2020 7469 6d65 2e0a 2020 2020        time..    
+0000ed10: 2020 2020 2020 2020 6c61 6265 6c73 3a20          labels: 
+0000ed20: 5468 6520 6c65 6765 6e64 206c 6162 656c  The legend label
+0000ed30: 7320 746f 2075 7365 2069 6e20 7468 6520  s to use in the 
+0000ed40: 706c 6f74 2e20 5468 6573 6520 7368 6f75  plot. These shou
+0000ed50: 6c64 2062 6520 696e 206f 7264 6572 206f  ld be in order o
+0000ed60: 6620 7468 6520 6163 7475 616c 0a20 2020  f the actual.   
+0000ed70: 2020 2020 2020 2020 2020 2020 206c 6567               leg
+0000ed80: 656e 6420 6c61 6265 6c73 2e0a 2020 2020  end labels..    
+0000ed90: 2020 2020 2020 2020 636f 6c6f 7273 3a20          colors: 
+0000eda0: 5468 6520 636f 6c6f 7273 2075 7365 6420  The colors used 
+0000edb0: 746f 2070 6c6f 7420 7468 6520 6c65 6172  to plot the lear
+0000edc0: 6e65 7273 2070 6c6f 742e 0a20 2020 2020  ners plot..     
+0000edd0: 2020 2020 2020 2074 6974 6c65 203a 2054         title : T
+0000ede0: 6865 2074 6974 6c65 2067 6976 6520 7468  he title give th
+0000edf0: 6520 706c 6f74 2e0a 2020 2020 2020 2020  e plot..        
+0000ee00: 2020 2020 786c 6162 656c 3a20 5468 6520      xlabel: The 
+0000ee10: 6c61 6265 6c20 6f6e 2074 6865 2078 2d61  label on the x-a
+0000ee20: 7869 732e 0a20 2020 2020 2020 2020 2020  xis..           
+0000ee30: 2079 6c61 6265 6c3a 2054 6865 206c 6162   ylabel: The lab
+0000ee40: 656c 206f 6e20 7468 6520 792d 6178 6973  el on the y-axis
+0000ee50: 2e0a 2020 2020 2020 2020 2020 2020 786c  ..            xl
+0000ee60: 696d 3a20 4465 6669 6e65 2074 6865 2078  im: Define the x
+0000ee70: 2d61 7869 7320 6c69 6d69 7473 2074 6f20  -axis limits to 
+0000ee80: 706c 6f74 2e20 4966 2060 4e6f 6e65 6020  plot. If `None` 
+0000ee90: 7468 6520 782d 6178 6973 206c 696d 6974  the x-axis limit
+0000eea0: 7320 7769 6c6c 2062 6520 696e 6665 7272  s will be inferr
+0000eeb0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+0000eec0: 796c 696d 3a20 4465 6669 6e65 2074 6865  ylim: Define the
+0000eed0: 2079 2d61 7869 7320 6c69 6d69 7473 2074   y-axis limits t
+0000eee0: 6f20 706c 6f74 2e20 4966 2060 4e6f 6e65  o plot. If `None
+0000eef0: 6020 7468 6520 792d 6178 6973 206c 696d  ` the y-axis lim
+0000ef00: 6974 7320 7769 6c6c 2062 6520 696e 6665  its will be infe
+0000ef10: 7272 6564 2e0a 2020 2020 2020 2020 2020  rred..          
+0000ef20: 2020 7874 6963 6b73 3a20 5768 6574 6865    xticks: Whethe
+0000ef30: 7220 7468 6520 782d 6178 6973 206c 6162  r the x-axis lab
+0000ef40: 656c 7320 7368 6f75 6c64 2062 6520 6472  els should be dr
+0000ef50: 6177 6e2e 0a20 2020 2020 2020 2020 2020  awn..           
+0000ef60: 2079 7469 636b 733a 2057 6865 7468 6572   yticks: Whether
+0000ef70: 2074 6865 2079 2d61 7869 7320 6c61 6265   the y-axis labe
+0000ef80: 6c73 2073 686f 756c 6420 6265 2064 7261  ls should be dra
+0000ef90: 776e 2e0a 2020 2020 2020 2020 2020 2020  wn..            
+0000efa0: 6c65 6765 6e64 3a20 5768 6574 6865 7220  legend: Whether 
+0000efb0: 7468 6520 6c65 6765 6e64 2066 6f72 2074  the legend for t
+0000efc0: 6865 2070 6c6f 7420 7368 6f75 6c64 2062  he plot should b
+0000efd0: 6520 6472 6177 6e2e 0a20 2020 2020 2020  e drawn..       
+0000efe0: 2020 2020 2061 6c70 6861 3a20 5468 6520       alpha: The 
+0000eff0: 6f70 6163 6974 7920 6f66 2064 7261 776e  opacity of drawn
+0000f000: 2064 6174 612e 0a20 2020 2020 2020 2020   data..         
+0000f010: 2020 2078 6f72 6465 723a 2049 6e64 6963     xorder: Indic
+0000f020: 6174 6573 2077 6865 7468 6572 2074 6865  ates whether the
+0000f030: 2078 2d61 7869 7320 7368 6f75 6c64 2062   x-axis should b
+0000f040: 6520 696e 2061 7363 656e 6469 6e67 2028  e in ascending (
+0000f050: 2b29 206f 7220 6465 7363 656e 6465 696e  +) or descendein
+0000f060: 6720 282d 2920 6f72 6465 722e 0a20 2020  g (-) order..   
+0000f070: 2020 2020 2020 2020 2074 6f70 5f6e 3a20           top_n: 
+0000f080: 4f6e 6c79 2070 6c6f 7420 7468 6520 746f  Only plot the to
+0000f090: 705f 6e20 6c65 6172 6e65 7273 2e20 4966  p_n learners. If
+0000f0a0: 2060 4e6f 6e65 6020 616c 6c20 6c65 6172   `None` all lear
+0000f0b0: 6e65 7273 2077 696c 6c20 6265 2070 6c6f  ners will be plo
+0000f0c0: 7474 6564 2e20 4966 206e 6567 6174 6976  tted. If negativ
+0000f0d0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000f0e0: 2020 7468 6520 626f 7474 6f6d 2077 696c    the bottom wil
+0000f0f0: 6c20 6265 2070 6c6f 7474 6564 2e0a 2020  l be plotted..  
+0000f100: 2020 2020 2020 2020 2020 6f75 743a 2049            out: I
+0000f110: 6e64 6963 6174 6520 7768 6572 6520 7468  ndicate where th
+0000f120: 6520 706c 6f74 2073 686f 756c 6420 6265  e plot should be
+0000f130: 2073 656e 7420 746f 2061 6674 6572 2070   sent to after p
+0000f140: 6c6f 7474 696e 6720 6973 2066 696e 6973  lotting is finis
+0000f150: 6865 642e 2056 616c 6964 2076 616c 7565  hed. Valid value
+0000f160: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000f170: 2020 6172 6520 2773 6372 6565 6e27 2074    are 'screen' t
+0000f180: 6f20 7368 6f77 2069 7420 6f6e 2073 6372  o show it on scr
+0000f190: 6565 6e2c 2061 2070 6174 6820 746f 2073  een, a path to s
+0000f1a0: 6176 6520 746f 2064 6973 6b2c 206f 7220  ave to disk, or 
+0000f1b0: 4e6f 6e65 2069 6620 7468 6520 706c 6f74  None if the plot
+0000f1c0: 2073 686f 756c 640a 2020 2020 2020 2020   should.        
+0000f1d0: 2020 2020 2020 2020 6e6f 7420 6265 206f          not be o
+0000f1e0: 7574 7075 7420 616e 7977 6865 7265 2028  utput anywhere (
+0000f1f0: 692e 652e 2c20 6b65 7074 2069 6e20 6d65  i.e., kept in me
+0000f200: 6d6f 7279 2920 696e 206f 7264 6572 2074  mory) in order t
+0000f210: 6f20 6b65 6570 2065 6469 7469 6e67 2074  o keep editing t
+0000f220: 6865 2070 6c6f 7420 6166 7465 720a 2020  he plot after.  
+0000f230: 2020 2020 2020 2020 2020 2020 2020 7468                th
+0000f240: 6973 2063 616c 6c2e 0a20 2020 2020 2020  is call..       
+0000f250: 2020 2020 2061 783a 2050 726f 7669 6465       ax: Provide
+0000f260: 2061 6e20 6f70 7469 6f6e 616c 2061 7865   an optional axe
+0000f270: 7320 7468 6174 2074 6865 2070 6c6f 7420  s that the plot 
+0000f280: 7769 6c6c 2062 6520 6472 6177 6e20 746f  will be drawn to
+0000f290: 2e20 4966 206e 6f74 2070 726f 7669 6465  . If not provide
+0000f2a0: 6420 6120 6e65 770a 2020 2020 2020 2020  d a new.        
+0000f2b0: 2020 2020 2020 2020 6669 6775 7265 2f61          figure/a
+0000f2c0: 7865 7320 6973 2063 7265 6174 6564 2e0a  xes is created..
+0000f2d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000f2e0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000f2f0: 2020 2020 2078 6c69 6d20 3d20 786c 696d       xlim = xlim
+0000f300: 206f 7220 5b4e 6f6e 652c 4e6f 6e65 5d0a   or [None,None].
+0000f310: 2020 2020 2020 2020 2020 2020 796c 696d              ylim
+0000f320: 203d 2079 6c69 6d20 6f72 205b 4e6f 6e65   = ylim or [None
+0000f330: 2c4e 6f6e 655d 0a0a 2020 2020 2020 2020  ,None]..        
+0000f340: 2020 2020 7261 775f 6461 7461 203d 2073      raw_data = s
+0000f350: 656c 662e 7261 775f 6c65 6172 6e65 7273  elf.raw_learners
+0000f360: 2878 2c79 2c6c 2c70 2c73 7061 6e29 0a0a  (x,y,l,p,span)..
+0000f370: 2020 2020 2020 2020 2020 2020 6572 7265              erre
+0000f380: 7665 7279 203d 2065 7272 6576 6572 7920  very = errevery 
+0000f390: 6f72 206d 6178 2869 6e74 2872 6177 5f64  or max(int(raw_d
+0000f3a0: 6174 615b 2778 275d 5b2d 315d 2a30 2e30  ata['x'][-1]*0.0
+0000f3b0: 3529 2c31 2920 6966 2078 203d 3d20 2769  5),1) if x == 'i
+0000f3c0: 6e64 6578 2720 656c 7365 2031 0a20 2020  ndex' else 1.   
+0000f3d0: 2020 2020 2020 2020 2073 7479 6c65 2020           style  
+0000f3e0: 2020 3d20 222d 2220 6966 2078 203d 3d20    = "-" if x == 
+0000f3f0: 2769 6e64 6578 2720 656c 7365 2022 2e22  'index' else "."
+0000f400: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
+0000f410: 2020 2020 2020 3d20 7365 6c66 2e5f 636f        = self._co
+0000f420: 6e66 6964 656e 6365 2865 7272 2c20 6572  nfidence(err, er
+0000f430: 7265 7665 7279 290a 0a20 2020 2020 2020  revery)..       
+0000f440: 2020 2020 2059 5f63 6f75 6e74 203d 205b       Y_count = [
+0000f450: 5d0a 2020 2020 2020 2020 2020 2020 6c69  ].            li
+0000f460: 6e65 733a 204c 6973 745b 506f 696e 7473  nes: List[Points
+0000f470: 5d20 3d20 5b5d 0a20 2020 2020 2020 2020  ] = [].         
+0000f480: 2020 2066 6f72 205f 6c20 696e 2072 6177     for _l in raw
+0000f490: 5f64 6174 612e 636f 6c75 6d6e 735b 313a  _data.columns[1:
+0000f4a0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0000f4b0: 2020 2063 6f6c 6f72 203d 2073 656c 662e     color = self.
+0000f4c0: 5f67 6574 5f63 6f6c 6f72 2863 6f6c 6f72  _get_color(color
+0000f4d0: 732c 2020 206c 656e 286c 696e 6573 2929  s,   len(lines))
+0000f4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f4f0: 206c 6162 656c 203d 2073 656c 662e 5f67   label = self._g
+0000f500: 6574 5f6c 6162 656c 286c 6162 656c 732c  et_label(labels,
+0000f510: 5f6c 2c6c 656e 286c 696e 6573 2929 0a20  _l,len(lines)). 
+0000f520: 2020 2020 2020 2020 2020 2020 2020 2059                 Y
+0000f530: 5f63 6f75 6e74 2e61 7070 656e 6428 3029  _count.append(0)
+0000f540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f550: 206c 696e 6573 2e61 7070 656e 6428 506f   lines.append(Po
+0000f560: 696e 7473 2873 7479 6c65 3d73 7479 6c65  ints(style=style
+0000f570: 2c63 6f6c 6f72 3d63 6f6c 6f72 2c6c 6162  ,color=color,lab
+0000f580: 656c 3d6c 6162 656c 2c61 6c70 6861 3d61  el=label,alpha=a
+0000f590: 6c70 6861 2929 0a20 2020 2020 2020 2020  lpha)).         
+0000f5a0: 2020 2020 2020 2066 6f72 205f 7869 2c20         for _xi, 
+0000f5b0: 285f 782c 2059 2920 696e 2065 6e75 6d65  (_x, Y) in enume
+0000f5c0: 7261 7465 287a 6970 282a 7261 775f 6461  rate(zip(*raw_da
+0000f5d0: 7461 5b5b 2778 272c 5f6c 5d5d 2929 3a0a  ta[['x',_l]])):.
+0000f5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5f0: 2020 2020 595f 636f 756e 745b 2d31 5d20      Y_count[-1] 
+0000f600: 3d20 6d61 7828 595f 636f 756e 745b 2d31  = max(Y_count[-1
+0000f610: 5d2c 6c65 6e28 5929 290a 2020 2020 2020  ],len(Y)).      
+0000f620: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000f630: 6e65 735b 2d31 5d2e 6164 6428 5f78 2069  nes[-1].add(_x i
+0000f640: 6620 5f78 2069 7320 6e6f 7420 4e6f 6e65  f _x is not None
+0000f650: 2065 6c73 6520 274e 6f6e 6527 2c20 2a65   else 'None', *e
+0000f660: 7272 2859 2c20 5f78 6929 290a 0a20 2020  rr(Y, _xi))..   
+0000f670: 2020 2020 2020 2020 206c 696e 6573 2020           lines  
+0000f680: 3d20 736f 7274 6564 286c 696e 6573 2c20  = sorted(lines, 
+0000f690: 6b65 793d 6c61 6d62 6461 206c 696e 653a  key=lambda line:
+0000f6a0: 206c 696e 652e 595b 2d31 5d2c 2072 6576   line.Y[-1], rev
+0000f6b0: 6572 7365 3d54 7275 6529 0a20 2020 2020  erse=True).     
+0000f6c0: 2020 2020 2020 206c 6162 656c 7320 3d20         labels = 
+0000f6d0: 5b6c 2e6c 6162 656c 206f 7220 7374 7228  [l.label or str(
+0000f6e0: 6c2e 6c61 6265 6c29 2066 6f72 206c 2069  l.label) for l i
+0000f6f0: 6e20 6c69 6e65 735d 0a20 2020 2020 2020  n lines].       
+0000f700: 2020 2020 2063 6f6c 6f72 7320 3d20 5b6c       colors = [l
+0000f710: 2e63 6f6c 6f72 2020 2020 2020 2020 2020  .color          
+0000f720: 2020 2020 2020 2066 6f72 206c 2069 6e20         for l in 
+0000f730: 6c69 6e65 735d 0a20 2020 2020 2020 2020  lines].         
+0000f740: 2020 2078 6c61 6265 6c20 3d20 786c 6162     xlabel = xlab
+0000f750: 656c 206f 7220 2822 496e 7465 7261 6374  el or ("Interact
+0000f760: 696f 6e22 2069 6620 783d 3d27 696e 6465  ion" if x=='inde
+0000f770: 7827 2065 6c73 6520 785b 305d 2069 6620  x' else x[0] if 
+0000f780: 6c65 6e28 7829 203d 3d20 3120 656c 7365  len(x) == 1 else
+0000f790: 2078 290a 2020 2020 2020 2020 2020 2020   x).            
+0000f7a0: 796c 6162 656c 203d 2079 6c61 6265 6c20  ylabel = ylabel 
+0000f7b0: 6f72 2028 2252 6577 6172 6422 2069 6620  or ("Reward" if 
+0000f7c0: 793d 3d27 7265 7761 7264 2720 656c 7365  y=='reward' else
+0000f7d0: 2079 2e72 6570 6c61 6365 2822 5f70 6374   y.replace("_pct
+0000f7e0: 222c 2220 5065 7263 656e 7422 2929 0a0a  "," Percent"))..
+0000f7f0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+0000f800: 656e 2873 6574 2859 5f63 6f75 6e74 2929  en(set(Y_count))
+0000f810: 203d 3d20 313a 2059 5f63 6f75 6e74 203d   == 1: Y_count =
+0000f820: 2059 5f63 6f75 6e74 5b30 5d0a 0a20 2020   Y_count[0]..   
+0000f830: 2020 2020 2020 2020 2079 5f6c 6f63 6174           y_locat
+0000f840: 696f 6e20 3d20 2254 6f74 616c 2220 6966  ion = "Total" if
+0000f850: 2078 2021 3d20 2769 6e64 6578 2720 656c   x != 'index' el
+0000f860: 7365 2022 220a 2020 2020 2020 2020 2020  se "".          
+0000f870: 2020 795f 6176 675f 7479 7065 203d 2028    y_avg_type = (
+0000f880: 2249 6e73 7461 6e74 2220 6966 2073 7061  "Instant" if spa
+0000f890: 6e20 3d3d 2031 2065 6c73 6520 6622 5370  n == 1 else f"Sp
+0000f8a0: 616e 207b 7370 616e 7d22 2069 6620 7370  an {span}" if sp
+0000f8b0: 616e 2065 6c73 6520 2250 726f 6772 6573  an else "Progres
+0000f8c0: 7369 7665 2229 0a20 2020 2020 2020 2020  sive").         
+0000f8d0: 2020 2079 5f73 616d 706c 6573 2020 3d20     y_samples  = 
+0000f8e0: 6622 287b 595f 636f 756e 747d 2045 6e76  f"({Y_count} Env
+0000f8f0: 6972 6f6e 6d65 6e74 7329 220a 2020 2020  ironments)".    
+0000f900: 2020 2020 2020 2020 7469 746c 6520 2020          title   
+0000f910: 2020 203d 2074 6974 6c65 2069 6620 7469     = title if ti
+0000f920: 746c 6520 6973 206e 6f74 204e 6f6e 6520  tle is not None 
+0000f930: 656c 7365 2028 2720 272e 6a6f 696e 2866  else (' '.join(f
+0000f940: 696c 7465 7228 4e6f 6e65 2c5b 795f 6c6f  ilter(None,[y_lo
+0000f950: 6361 7469 6f6e 2c20 795f 6176 675f 7479  cation, y_avg_ty
+0000f960: 7065 2c20 796c 6162 656c 2c20 795f 7361  pe, ylabel, y_sa
+0000f970: 6d70 6c65 735d 2929 290a 0a20 2020 2020  mples])))..     
+0000f980: 2020 2020 2020 2078 726f 7461 7469 6f6e         xrotation
+0000f990: 203d 2039 3020 6966 2028 7820 213d 2027   = 90 if (x != '
+0000f9a0: 696e 6465 7827 206f 7220 786f 7264 6572  index' or xorder
+0000f9b0: 2920 616e 6420 6c65 6e28 6c69 6e65 735b  ) and len(lines[
+0000f9c0: 305d 2e58 293e 3520 656c 7365 2030 0a20  0].X)>5 else 0. 
+0000f9d0: 2020 2020 2020 2020 2020 2079 726f 7461             yrota
+0000f9e0: 7469 6f6e 203d 2030 0a0a 2020 2020 2020  tion = 0..      
+0000f9f0: 2020 2020 2020 6966 2074 6f70 5f6e 3a0a        if top_n:.
+0000fa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa10: 6966 2061 6273 2874 6f70 5f6e 2920 3e20  if abs(top_n) > 
+0000fa20: 6c65 6e28 6c69 6e65 7329 3a20 746f 705f  len(lines): top_
+0000fa30: 6e20 3d20 6c65 6e28 6c69 6e65 7329 2a61  n = len(lines)*a
+0000fa40: 6273 2874 6f70 5f6e 292f 746f 705f 6e0a  bs(top_n)/top_n.
+0000fa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa60: 6966 2074 6f70 5f6e 203e 2030 3a20 6c69  if top_n > 0: li
+0000fa70: 6e65 7320 3d20 5b72 6570 6c61 6365 286c  nes = [replace(l
+0000fa80: 2c63 6f6c 6f72 3d73 656c 662e 5f67 6574  ,color=self._get
+0000fa90: 5f63 6f6c 6f72 2863 6f6c 6f72 732c 6929  _color(colors,i)
+0000faa0: 2c6c 6162 656c 3d73 656c 662e 5f67 6574  ,label=self._get
+0000fab0: 5f6c 6162 656c 286c 6162 656c 732c 6c2e  _label(labels,l.
+0000fac0: 6c61 6265 6c2c 6929 2920 666f 7220 692c  label,i)) for i,
+0000fad0: 6c20 696e 2065 6e75 6d65 7261 7465 286c  l in enumerate(l
+0000fae0: 696e 6573 5b3a 746f 705f 6e5d 2c30 2020  ines[:top_n],0  
+0000faf0: 2020 2920 5d0a 2020 2020 2020 2020 2020    ) ].          
+0000fb00: 2020 2020 2020 6966 2074 6f70 5f6e 203c        if top_n <
+0000fb10: 2030 3a20 6c69 6e65 7320 3d20 5b72 6570   0: lines = [rep
+0000fb20: 6c61 6365 286c 2c63 6f6c 6f72 3d73 656c  lace(l,color=sel
+0000fb30: 662e 5f67 6574 5f63 6f6c 6f72 2863 6f6c  f._get_color(col
+0000fb40: 6f72 732c 6929 2c6c 6162 656c 3d73 656c  ors,i),label=sel
+0000fb50: 662e 5f67 6574 5f6c 6162 656c 286c 6162  f._get_label(lab
+0000fb60: 656c 732c 6c2e 6c61 6265 6c2c 6929 2920  els,l.label,i)) 
+0000fb70: 666f 7220 692c 6c20 696e 2065 6e75 6d65  for i,l in enume
+0000fb80: 7261 7465 286c 696e 6573 5b74 6f70 5f6e  rate(lines[top_n
+0000fb90: 3a5d 2c74 6f70 5f6e 2920 5d0a 0a20 2020  :],top_n) ]..   
+0000fba0: 2020 2020 2020 2020 2061 6c6c 5f78 203d           all_x =
+0000fbb0: 2064 6963 742e 6672 6f6d 6b65 7973 2863   dict.fromkeys(c
+0000fbc0: 6861 696e 2e66 726f 6d5f 6974 6572 6162  hain.from_iterab
+0000fbd0: 6c65 286c 696e 652e 5820 666f 7220 6c69  le(line.X for li
+0000fbe0: 6e65 2069 6e20 6c69 6e65 7329 290a 2020  ne in lines)).  
+0000fbf0: 2020 2020 2020 2020 2020 786f 7264 6572            xorder
+0000fc00: 6564 203d 206c 6973 7428 616c 6c5f 782e  ed = list(all_x.
+0000fc10: 6b65 7973 2829 2920 6966 206e 6f74 2078  keys()) if not x
+0000fc20: 6f72 6465 7220 656c 7365 2073 6f72 7465  order else sorte
+0000fc30: 6428 616c 6c5f 782c 2072 6576 6572 7365  d(all_x, reverse
+0000fc40: 3d78 6f72 6465 723d 3d27 2d27 290a 0a20  =xorder=='-').. 
+0000fc50: 2020 2020 2020 2020 2020 2069 6620 7820             if x 
+0000fc60: 3d3d 2027 696e 6465 7827 2061 6e64 2078  == 'index' and x
+0000fc70: 6f72 6465 7220 696e 205b 272b 272c 4e6f  order in ['+',No
+0000fc80: 6e65 5d3a 2078 6f72 6465 7265 6420 3d20  ne]: xordered = 
+0000fc90: 4e6f 6e65 0a0a 2020 2020 2020 2020 2020  None..          
+0000fca0: 2020 7365 6c66 2e5f 706c 6f74 7465 722e    self._plotter.
+0000fcb0: 706c 6f74 2861 782c 206c 696e 6573 2c20  plot(ax, lines, 
+0000fcc0: 7469 746c 652c 2078 6c61 6265 6c2c 2079  title, xlabel, y
+0000fcd0: 6c61 6265 6c2c 2078 6c69 6d2c 2079 6c69  label, xlim, yli
+0000fce0: 6d2c 2078 7469 636b 732c 2079 7469 636b  m, xticks, ytick
+0000fcf0: 732c 206c 6567 656e 642c 2078 726f 7461  s, legend, xrota
+0000fd00: 7469 6f6e 2c20 7972 6f74 6174 696f 6e2c  tion, yrotation,
+0000fd10: 2078 6f72 6465 7265 642c 206f 7574 290a   xordered, out).
+0000fd20: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000fd30: 436f 6261 4578 6365 7074 696f 6e20 6173  CobaException as
+0000fd40: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+0000fd50: 436f 6261 436f 6e74 6578 742e 6c6f 6767  CobaContext.logg
+0000fd60: 6572 2e6c 6f67 2873 7472 2865 2929 0a0a  er.log(str(e))..
+0000fd70: 2020 2020 6465 6620 706c 6f74 5f63 6f6e      def plot_con
+0000fd80: 7472 6173 7428 7365 6c66 2c0a 2020 2020  trast(self,.    
+0000fd90: 2020 2020 6c31 2020 2020 2020 3a20 416e      l1      : An
+0000fda0: 792c 0a20 2020 2020 2020 206c 3220 2020  y,.        l2   
+0000fdb0: 2020 203a 2041 6e79 2c0a 2020 2020 2020     : Any,.      
+0000fdc0: 2020 7820 2020 2020 2020 3a20 556e 696f    x       : Unio
+0000fdd0: 6e5b 7374 722c 2053 6571 7565 6e63 655b  n[str, Sequence[
+0000fde0: 7374 725d 5d20 3d20 2265 6e76 6972 6f6e  str]] = "environ
+0000fdf0: 6d65 6e74 5f69 6422 2c0a 2020 2020 2020  ment_id",.      
+0000fe00: 2020 7920 2020 2020 2020 3a20 7374 7220    y       : str 
+0000fe10: 3d20 2272 6577 6172 6422 2c0a 2020 2020  = "reward",.    
+0000fe20: 2020 2020 6c20 2020 2020 2020 3a20 556e      l       : Un
+0000fe30: 696f 6e5b 7374 722c 2053 6571 7565 6e63  ion[str, Sequenc
+0000fe40: 655b 7374 725d 5d20 3d20 276c 6561 726e  e[str]] = 'learn
+0000fe50: 6572 5f69 6427 2c0a 2020 2020 2020 2020  er_id',.        
+0000fe60: 7020 2020 2020 2020 3a20 556e 696f 6e5b  p       : Union[
+0000fe70: 7374 722c 2053 6571 7565 6e63 655b 7374  str, Sequence[st
+0000fe80: 725d 5d20 3d20 2765 6e76 6972 6f6e 6d65  r]] = 'environme
+0000fe90: 6e74 5f69 6427 2c0a 2020 2020 2020 2020  nt_id',.        
+0000fea0: 6d6f 6465 2020 2020 3a20 556e 696f 6e5b  mode    : Union[
+0000feb0: 4c69 7465 7261 6c5b 2264 6966 6622 2c22  Literal["diff","
+0000fec0: 7072 6f62 225d 2c20 4361 6c6c 6162 6c65  prob"], Callable
+0000fed0: 5b5b 666c 6f61 742c 666c 6f61 745d 2c66  [[float,float],f
+0000fee0: 6c6f 6174 5d5d 203d 2022 6469 6666 222c  loat]] = "diff",
+0000fef0: 0a20 2020 2020 2020 2073 7061 6e20 2020  .        span   
+0000ff00: 203a 2069 6e74 203d 204e 6f6e 652c 0a20   : int = None,. 
+0000ff10: 2020 2020 2020 2065 7272 2020 2020 203a         err     :
+0000ff20: 2055 6e69 6f6e 5b4c 6974 6572 616c 5b27   Union[Literal['
+0000ff30: 7365 272c 2773 6427 2c27 6273 272c 2762  se','sd','bs','b
+0000ff40: 6927 5d2c 2050 6f69 6e74 416e 6449 6e74  i'], PointAndInt
+0000ff50: 6572 7661 6c5d 203d 204e 6f6e 652c 0a20  erval] = None,. 
+0000ff60: 2020 2020 2020 2065 7272 6576 6572 793a         errevery:
+0000ff70: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+0000ff80: 2020 2020 206c 6162 656c 7320 203a 2053       labels  : S
+0000ff90: 6571 7565 6e63 655b 7374 725d 203d 204e  equence[str] = N
+0000ffa0: 6f6e 652c 0a20 2020 2020 2020 2063 6f6c  one,.        col
+0000ffb0: 6f72 7320 203a 2053 6571 7565 6e63 655b  ors  : Sequence[
+0000ffc0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0000ffd0: 2020 2020 2074 6974 6c65 2020 203a 2073       title   : s
+0000ffe0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0000fff0: 2020 2078 6c61 6265 6c20 203a 2073 7472     xlabel  : str
+00010000: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00010010: 2079 6c61 6265 6c20 203a 2073 7472 203d   ylabel  : str =
+00010020: 204e 6f6e 652c 0a20 2020 2020 2020 2078   None,.        x
+00010030: 6c69 6d20 2020 203a 2054 7570 6c65 5b4f  lim    : Tuple[O
+00010040: 7074 696f 6e61 6c5b 4e75 6d62 6572 5d2c  ptional[Number],
+00010050: 4f70 7469 6f6e 616c 5b4e 756d 6265 725d  Optional[Number]
+00010060: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00010070: 2020 796c 696d 2020 2020 3a20 5475 706c    ylim    : Tupl
+00010080: 655b 4f70 7469 6f6e 616c 5b4e 756d 6265  e[Optional[Numbe
+00010090: 725d 2c4f 7074 696f 6e61 6c5b 4e75 6d62  r],Optional[Numb
+000100a0: 6572 5d5d 203d 204e 6f6e 652c 0a20 2020  er]] = None,.   
+000100b0: 2020 2020 2078 7469 636b 7320 203a 2062       xticks  : b
+000100c0: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+000100d0: 2020 2020 7974 6963 6b73 2020 3a20 626f      yticks  : bo
+000100e0: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
+000100f0: 2020 206c 6567 656e 6420 203a 2062 6f6f     legend  : boo
+00010100: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
+00010110: 2020 616c 7068 6120 2020 3a20 666c 6f61    alpha   : floa
+00010120: 7420 3d20 312c 0a20 2020 2020 2020 2078  t = 1,.        x
+00010130: 6f72 6465 7220 203a 204c 6974 6572 616c  order  : Literal
+00010140: 5b27 2b27 2c27 2d27 5d20 3d20 4e6f 6e65  ['+','-'] = None
+00010150: 2c0a 2020 2020 2020 2020 626f 756e 6461  ,.        bounda
+00010160: 7279 3a20 626f 6f6c 203d 2054 7275 652c  ry: bool = True,
+00010170: 0a20 2020 2020 2020 206f 7574 2020 2020  .        out    
+00010180: 203a 2055 6e69 6f6e 5b4e 6f6e 652c 4c69   : Union[None,Li
+00010190: 7465 7261 6c5b 2773 6372 6565 6e27 5d2c  teral['screen'],
+000101a0: 7374 725d 203d 2027 7363 7265 656e 272c  str] = 'screen',
+000101b0: 0a20 2020 2020 2020 2061 7820 3d20 4e6f  .        ax = No
+000101c0: 6e65 2920 2d3e 204e 6f6e 653a 0a20 2020  ne) -> None:.   
+000101d0: 2020 2020 2022 2222 506c 6f74 2061 2064       """Plot a d
+000101e0: 6972 6563 7420 636f 6e74 7261 7374 206f  irect contrast o
+000101f0: 6620 7468 6520 7065 7266 6f72 6d61 6e63  f the performanc
+00010200: 6520 666f 7220 7477 6f20 6c65 6172 6e65  e for two learne
+00010210: 7273 2e0a 0a20 2020 2020 2020 2041 7267  rs...        Arg
+00010220: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
+00010230: 313a 2054 6865 2066 6972 7374 2073 6574  1: The first set
+00010240: 206f 6620 7061 7261 6d65 7465 7220 7661   of parameter va
+00010250: 6c75 6573 2077 6520 7761 6e74 2074 6f20  lues we want to 
+00010260: 636f 6e74 7261 7374 2e0a 2020 2020 2020  contrast..      
+00010270: 2020 2020 2020 6c32 3a20 5468 6520 7365        l2: The se
+00010280: 636f 6e64 2073 6574 206f 6620 7061 7261  cond set of para
+00010290: 6d65 7465 7220 7661 6c75 6573 2077 6520  meter values we 
+000102a0: 7761 6e74 2074 6f20 636f 6e74 7261 7374  want to contrast
+000102b0: 2e0a 2020 2020 2020 2020 2020 2020 783a  ..            x:
+000102c0: 2054 6865 2076 616c 7565 2074 6f20 706c   The value to pl
+000102d0: 6f74 206f 6e20 7468 6520 782d 6178 6973  ot on the x-axis
+000102e0: 2e20 5468 6973 2063 616e 2065 6974 6865  . This can eithe
+000102f0: 7220 6265 2069 6e64 6578 206f 7220 656e  r be index or en
+00010300: 7669 726f 6e6d 656e 7420 636f 6c75 6d6e  vironment column
+00010310: 7320 746f 2067 726f 7570 2062 792e 0a20  s to group by.. 
+00010320: 2020 2020 2020 2020 2020 2079 3a20 5468             y: Th
+00010330: 6520 7661 6c75 6520 746f 2070 6c6f 7420  e value to plot 
+00010340: 6f6e 2074 6865 2079 2d61 7869 732e 0a20  on the y-axis.. 
+00010350: 2020 2020 2020 2020 2020 206c 3a20 5468             l: Th
+00010360: 6520 6c65 7665 6c20 6174 2077 6869 6368  e level at which
+00010370: 2077 6520 7761 6e74 2074 6f20 636f 6e74   we want to cont
+00010380: 7261 7374 2e0a 2020 2020 2020 2020 2020  rast..          
+00010390: 2020 703a 2054 6865 2070 6169 7273 2074    p: The pairs t
+000103a0: 6861 7420 6d75 7374 2065 7869 7374 2061  hat must exist a
+000103b0: 6372 6f73 7320 616c 6c20 636f 6d70 6172  cross all compar
+000103c0: 6973 6f6e 206c 6576 656c 7320 696e 206f  ison levels in o
+000103d0: 7264 6572 2074 6f20 6265 2069 6e63 6c75  rder to be inclu
+000103e0: 6465 642e 0a20 2020 2020 2020 2020 2020  ded..           
+000103f0: 206d 6f64 653a 2027 6469 6666 2720 2d2d   mode: 'diff' --
+00010400: 2070 6c6f 7420 7468 6520 7061 6972 7769   plot the pairwi
+00010410: 7365 2064 6966 6665 7265 6e63 653b 2027  se difference; '
+00010420: 7072 6f62 2720 706c 6f74 2074 6865 2070  prob' plot the p
+00010430: 726f 6261 6269 6c69 7479 206f 6620 6c31  robability of l1
+00010440: 2062 6561 7469 6e67 206c 322e 0a20 2020   beating l2..   
+00010450: 2020 2020 2020 2020 2073 7061 6e3a 2054           span: T
+00010460: 6865 206e 756d 6265 7220 6f66 2079 2076  he number of y v
+00010470: 616c 7565 7320 746f 2073 6d6f 6f74 6820  alues to smooth 
+00010480: 746f 6765 7468 6572 2077 6865 6e20 7265  together when re
+00010490: 706f 7274 696e 6720 792e 2049 6620 7468  porting y. If th
+000104a0: 6973 2069 7320 4e6f 6e65 2074 6865 6e20  is is None then 
+000104b0: 7468 6520 6176 6572 6167 6520 6f66 2061  the average of a
+000104c0: 6c6c 2079 0a20 2020 2020 2020 2020 2020  ll y.           
+000104d0: 2020 2020 2076 616c 7565 7320 7570 2074       values up t
+000104e0: 6f20 6375 7272 656e 7420 6973 2073 686f  o current is sho
+000104f0: 776e 206f 7468 6572 7769 7365 2061 206d  wn otherwise a m
+00010500: 6f76 696e 6720 6176 6572 6167 6520 7769  oving average wi
+00010510: 7468 2077 696e 646f 7720 7369 7a65 206f  th window size o
+00010520: 6620 7370 616e 2028 7468 6520 7769 6e64  f span (the wind
+00010530: 6f77 2077 696c 6c20 6265 0a20 2020 2020  ow will be.     
+00010540: 2020 2020 2020 2020 2020 2073 6d61 6c6c             small
+00010550: 6572 2074 6861 6e20 7370 616e 2069 6e69  er than span ini
+00010560: 7469 616c 6c79 292e 0a20 2020 2020 2020  tially)..       
+00010570: 2020 2020 2065 7272 3a20 5468 6973 2064       err: This d
+00010580: 6574 6572 6d69 6e65 7320 7768 6174 206b  etermines what k
+00010590: 696e 6420 6f66 2065 7272 6f72 2062 6172  ind of error bar
+000105a0: 7320 746f 2070 6c6f 7420 2869 6620 616e  s to plot (if an
+000105b0: 7929 2e20 4966 2060 4e6f 6e65 6020 7468  y). If `None` th
+000105c0: 656e 206e 6f20 6261 7273 2061 7265 2070  en no bars are p
+000105d0: 6c6f 7474 6564 2c20 6966 2027 7365 270a  lotted, if 'se'.
+000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105f0: 7468 6520 7374 616e 6461 7264 2065 7272  the standard err
+00010600: 6f72 2069 7320 7368 6f77 6e2c 2061 6e64  or is shown, and
+00010610: 2069 6620 2773 6427 2074 6865 2073 7461   if 'sd' the sta
+00010620: 6e64 6172 6420 6465 7669 6174 696f 6e20  ndard deviation 
+00010630: 6973 2073 686f 776e 2e0a 2020 2020 2020  is shown..      
+00010640: 2020 2020 2020 6572 7265 7665 7279 3a20        errevery: 
+00010650: 5468 6973 2064 6574 6572 6d69 6e65 7320  This determines 
+00010660: 7468 6520 6672 6571 7565 6e63 7920 6f66  the frequency of
+00010670: 2065 7272 6f72 6261 7273 2e20 4966 2060   errorbars. If `
+00010680: 4e6f 6e65 6020 7468 6579 2061 7070 6561  None` they appea
+00010690: 7220 3525 206f 6620 7468 6520 7469 6d65  r 5% of the time
+000106a0: 2e0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+000106b0: 6265 6c73 3a20 5468 6520 6c65 6765 6e64  bels: The legend
+000106c0: 206c 6162 656c 7320 746f 2075 7365 2069   labels to use i
+000106d0: 6e20 7468 6520 706c 6f74 2e20 5468 6573  n the plot. Thes
+000106e0: 6520 7368 6f75 6c64 2062 6520 696e 206f  e should be in o
+000106f0: 7264 6572 206f 6620 7468 6520 6163 7475  rder of the actu
+00010700: 616c 206c 6567 656e 6420 6c61 6265 6c73  al legend labels
+00010710: 2e0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
+00010720: 746c 6520 3a20 5468 6520 7469 746c 6520  tle : The title 
+00010730: 6769 7665 2074 6865 2070 6c6f 742e 0a20  give the plot.. 
+00010740: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+00010750: 733a 2054 6865 2063 6f6c 6f72 7320 7573  s: The colors us
+00010760: 6564 2074 6f20 706c 6f74 2074 6865 206c  ed to plot the l
+00010770: 6561 726e 6572 7320 706c 6f74 2e0a 2020  earners plot..  
+00010780: 2020 2020 2020 2020 2020 786c 6162 656c            xlabel
+00010790: 3a20 5468 6520 6c61 6265 6c20 6f6e 2074  : The label on t
+000107a0: 6865 2078 2d61 7869 732e 0a20 2020 2020  he x-axis..     
+000107b0: 2020 2020 2020 2079 6c61 6265 6c3a 2054         ylabel: T
+000107c0: 6865 206c 6162 656c 206f 6e20 7468 6520  he label on the 
+000107d0: 792d 6178 6973 2e0a 2020 2020 2020 2020  y-axis..        
+000107e0: 2020 2020 6c65 6765 6e64 3a20 5768 6574      legend: Whet
+000107f0: 6865 7220 7468 6520 6c65 6765 6e64 2066  her the legend f
+00010800: 6f72 2074 6865 2070 6c6f 7420 7368 6f75  or the plot shou
+00010810: 6c64 2062 6520 6472 6177 6e2e 0a20 2020  ld be drawn..   
+00010820: 2020 2020 2020 2020 2061 6c70 6861 3a20           alpha: 
+00010830: 5468 6520 6f70 6163 6974 7920 6f66 2064  The opacity of d
+00010840: 7261 776e 2064 6174 612e 0a20 2020 2020  rawn data..     
+00010850: 2020 2020 2020 2078 6c69 6d3a 2044 6566         xlim: Def
+00010860: 696e 6520 7468 6520 782d 6178 6973 206c  ine the x-axis l
+00010870: 696d 6974 7320 746f 2070 6c6f 742e 2049  imits to plot. I
+00010880: 6620 604e 6f6e 6560 2074 6865 2078 2d61  f `None` the x-a
+00010890: 7869 7320 6c69 6d69 7473 2077 696c 6c20  xis limits will 
+000108a0: 6265 2069 6e66 6572 7265 642e 0a20 2020  be inferred..   
+000108b0: 2020 2020 2020 2020 2079 6c69 6d3a 2044           ylim: D
+000108c0: 6566 696e 6520 7468 6520 792d 6178 6973  efine the y-axis
+000108d0: 206c 696d 6974 7320 746f 2070 6c6f 742e   limits to plot.
+000108e0: 2049 6620 604e 6f6e 6560 2074 6865 2079   If `None` the y
+000108f0: 2d61 7869 7320 6c69 6d69 7473 2077 696c  -axis limits wil
+00010900: 6c20 6265 2069 6e66 6572 7265 642e 0a20  l be inferred.. 
+00010910: 2020 2020 2020 2020 2020 2078 7469 636b             xtick
+00010920: 733a 2057 6865 7468 6572 2074 6865 2078  s: Whether the x
+00010930: 2d61 7869 7320 6c61 6265 6c73 2073 686f  -axis labels sho
+00010940: 756c 6420 6265 2064 7261 776e 2e0a 2020  uld be drawn..  
+00010950: 2020 2020 2020 2020 2020 7974 6963 6b73            yticks
+00010960: 3a20 5768 6574 6865 7220 7468 6520 792d  : Whether the y-
+00010970: 6178 6973 206c 6162 656c 7320 7368 6f75  axis labels shou
+00010980: 6c64 2062 6520 6472 6177 6e2e 0a20 2020  ld be drawn..   
+00010990: 2020 2020 2020 2020 2078 6f72 6465 723a           xorder:
+000109a0: 2049 6e64 6963 6174 6573 2077 6865 7468   Indicates wheth
+000109b0: 6572 2074 6865 2078 2d61 7869 7320 7368  er the x-axis sh
+000109c0: 6f75 6c64 2062 6520 696e 2061 7363 656e  ould be in ascen
+000109d0: 6469 6e67 2028 2b29 206f 7220 6465 7363  ding (+) or desc
+000109e0: 656e 6465 696e 6720 282d 2920 6f72 6465  endeing (-) orde
+000109f0: 722e 0a20 2020 2020 2020 2020 2020 2062  r..            b
+00010a00: 6f75 6e64 6172 793a 2057 6865 7468 6572  oundary: Whether
+00010a10: 2077 6520 7761 6e74 2074 6f20 706c 6f74   we want to plot
+00010a20: 2074 6865 2062 6f75 6e64 6172 7920 6c69   the boundary li
+00010a30: 6e65 2062 6574 7765 656e 2077 6869 6368  ne between which
+00010a40: 2073 6574 2069 7320 7468 6520 6265 7374   set is the best
+00010a50: 2070 6572 666f 726d 696e 672e 0a20 2020   performing..   
+00010a60: 2020 2020 2020 2020 206f 7574 3a20 496e           out: In
+00010a70: 6469 6361 7465 2077 6865 7265 2074 6865  dicate where the
+00010a80: 2070 6c6f 7420 7368 6f75 6c64 2062 6520   plot should be 
+00010a90: 7365 6e74 2074 6f20 6166 7465 7220 706c  sent to after pl
+00010aa0: 6f74 7469 6e67 2069 7320 6669 6e69 7368  otting is finish
+00010ab0: 6564 2e20 5661 6c69 6420 7661 6c75 6573  ed. Valid values
+00010ac0: 2061 7265 0a20 2020 2020 2020 2020 2020   are.           
+00010ad0: 2020 2020 2027 7363 7265 656e 2720 746f       'screen' to
+00010ae0: 2073 686f 7720 6974 206f 6e20 7363 7265   show it on scre
+00010af0: 656e 2c20 6120 7061 7468 2074 6f20 7361  en, a path to sa
+00010b00: 7665 2074 6f20 6469 736b 2c20 6f72 204e  ve to disk, or N
+00010b10: 6f6e 6520 6966 2074 6865 2070 6c6f 7420  one if the plot 
+00010b20: 7368 6f75 6c64 206e 6f74 2062 650a 2020  should not be.  
+00010b30: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00010b40: 7470 7574 2061 6e79 7768 6572 6520 2869  tput anywhere (i
+00010b50: 2e65 2e2c 206b 6570 7420 696e 206d 656d  .e., kept in mem
+00010b60: 6f72 7929 2069 6e20 6f72 6465 7220 746f  ory) in order to
+00010b70: 206b 6565 7020 6564 6974 696e 6720 7468   keep editing th
+00010b80: 6520 706c 6f74 2061 6674 6572 2074 6869  e plot after thi
+00010b90: 7320 6361 6c6c 2e0a 2020 2020 2020 2020  s call..        
+00010ba0: 2020 2020 6178 3a20 5072 6f76 6964 6520      ax: Provide 
+00010bb0: 616e 206f 7074 696f 6e61 6c20 6178 6573  an optional axes
+00010bc0: 2074 6861 7420 7468 6520 706c 6f74 2077   that the plot w
+00010bd0: 696c 6c20 6265 2064 7261 776e 2074 6f2e  ill be drawn to.
+00010be0: 2049 6620 6e6f 7420 7072 6f76 6964 6564   If not provided
+00010bf0: 2061 206e 6577 2066 6967 7572 652f 6178   a new figure/ax
+00010c00: 6573 2069 7320 6372 6561 7465 642e 0a20  es is created.. 
+00010c10: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00010c20: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00010c30: 2020 2020 2078 6c69 6d20 3d20 786c 696d       xlim = xlim
+00010c40: 206f 7220 5b4e 6f6e 652c 4e6f 6e65 5d0a   or [None,None].
+00010c50: 2020 2020 2020 2020 2020 2020 796c 696d              ylim
+00010c60: 203d 2079 6c69 6d20 6f72 205b 4e6f 6e65   = ylim or [None
+00010c70: 2c4e 6f6e 655d 0a0a 2020 2020 2020 2020  ,None]..        
+00010c80: 2020 2020 7261 775f 6461 7461 203d 2073      raw_data = s
+00010c90: 656c 662e 7261 775f 636f 6e74 7261 7374  elf.raw_contrast
+00010ca0: 286c 312c 6c32 2c78 2c79 2c6c 2c70 2c73  (l1,l2,x,y,l,p,s
+00010cb0: 7061 6e29 0a0a 2020 2020 2020 2020 2020  pan)..          
+00010cc0: 2020 6c69 7374 5f6c 696b 653d 286c 6973    list_like=(lis
+00010cd0: 742c 7475 706c 6529 0a0a 2020 2020 2020  t,tuple)..      
+00010ce0: 2020 2020 2020 6966 2020 2020 2069 7369        if     isi
+00010cf0: 6e73 7461 6e63 6528 6c2c 6c69 7374 5f6c  nstance(l,list_l
+00010d00: 696b 6529 2061 6e64 206e 6f74 2069 7369  ike) and not isi
+00010d10: 6e73 7461 6e63 6528 6c31 5b30 5d2c 6c69  nstance(l1[0],li
+00010d20: 7374 5f6c 696b 6529 3a20 6c31 203d 205b  st_like): l1 = [
+00010d30: 6c31 5d0a 2020 2020 2020 2020 2020 2020  l1].            
+00010d40: 6966 2020 2020 2069 7369 6e73 7461 6e63  if     isinstanc
+00010d50: 6528 6c2c 6c69 7374 5f6c 696b 6529 2061  e(l,list_like) a
+00010d60: 6e64 206e 6f74 2069 7369 6e73 7461 6e63  nd not isinstanc
+00010d70: 6528 6c32 5b30 5d2c 6c69 7374 5f6c 696b  e(l2[0],list_lik
+00010d80: 6529 3a20 6c32 203d 205b 6c32 5d0a 2020  e): l2 = [l2].  
+00010d90: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00010da0: 2069 7369 6e73 7461 6e63 6528 6c2c 6c69   isinstance(l,li
+00010db0: 7374 5f6c 696b 6529 2061 6e64 206e 6f74  st_like) and not
+00010dc0: 2069 7369 6e73 7461 6e63 6528 6c31 2020   isinstance(l1  
+00010dd0: 202c 6c69 7374 5f6c 696b 6529 3a20 6c31   ,list_like): l1
+00010de0: 203d 205b 6c31 5d0a 2020 2020 2020 2020   = [l1].        
+00010df0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+00010e00: 7461 6e63 6528 6c2c 6c69 7374 5f6c 696b  tance(l,list_lik
+00010e10: 6529 2061 6e64 206e 6f74 2069 7369 6e73  e) and not isins
+00010e20: 7461 6e63 6528 6c32 2020 202c 6c69 7374  tance(l2   ,list
+00010e30: 5f6c 696b 6529 3a20 6c32 203d 205b 6c32  _like): l2 = [l2
+00010e40: 5d0a 0a20 2020 2020 2020 2020 2020 2063  ]..            c
+00010e50: 6f6e 7472 6173 7465 7220 3d20 286c 616d  ontraster = (lam
+00010e60: 6264 6120 743a 2074 5b31 5d2d 745b 305d  bda t: t[1]-t[0]
+00010e70: 2920 6966 206d 6f64 6520 3d3d 2027 6469  ) if mode == 'di
+00010e80: 6666 2720 656c 7365 2028 6c61 6d62 6461  ff' else (lambda
+00010e90: 2074 3a20 696e 7428 2874 5b31 5d2d 745b   t: int((t[1]-t[
+00010ea0: 305d 293e 3029 2920 6966 206d 6f64 653d  0])>0)) if mode=
+00010eb0: 3d27 7072 6f62 2720 656c 7365 206d 6f64  ='prob' else mod
+00010ec0: 650a 2020 2020 2020 2020 2020 2020 5f62  e.            _b
+00010ed0: 6f75 6e64 6172 7920 203d 2030 2069 6620  oundary  = 0 if 
+00010ee0: 6d6f 6465 203d 3d20 2764 6966 6627 2065  mode == 'diff' e
+00010ef0: 6c73 6520 2e35 0a0a 2020 2020 2020 2020  lse .5..        
+00010f00: 2020 2020 6572 7265 7665 7279 203d 2065      errevery = e
+00010f10: 7272 6576 6572 7920 6f72 206d 6178 2869  rrevery or max(i
+00010f20: 6e74 2872 6177 5f64 6174 615b 2778 275d  nt(raw_data['x']
+00010f30: 5b2d 315d 2a30 2e30 3529 2c31 2920 6966  [-1]*0.05),1) if
+00010f40: 2078 203d 3d20 2769 6e64 6578 2720 656c   x == 'index' el
+00010f50: 7365 2031 0a20 2020 2020 2020 2020 2020  se 1.           
+00010f60: 2073 7479 6c65 2020 2020 3d20 222d 2220   style    = "-" 
+00010f70: 6966 2078 203d 3d20 2769 6e64 6578 2720  if x == 'index' 
+00010f80: 656c 7365 2022 2e22 0a20 2020 2020 2020  else ".".       
+00010f90: 2020 2020 2065 7272 2020 2020 2020 3d20       err      = 
+00010fa0: 7365 6c66 2e5f 636f 6e66 6964 656e 6365  self._confidence
+00010fb0: 2865 7272 2c20 6572 7265 7665 7279 290a  (err, errevery).
+00010fc0: 0a20 2020 2020 2020 2020 2020 2058 5f59  .            X_Y
+00010fd0: 5f59 4520 3d20 5b5d 0a20 2020 2020 2020  _YE = [].       
+00010fe0: 2020 2020 2066 6f72 205f 7869 2c20 285f       for _xi, (_
+00010ff0: 782c 2070 6169 7273 2920 696e 2065 6e75  x, pairs) in enu
+00011000: 6d65 7261 7465 2872 6177 5f64 6174 6129  merate(raw_data)
+00011010: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011020: 2020 585f 595f 5945 2e61 7070 656e 6428    X_Y_YE.append(
+00011030: 285f 782c 292b 6572 7228 6c69 7374 286d  (_x,)+err(list(m
+00011040: 6170 2863 6f6e 7472 6173 7465 722c 7061  ap(contraster,pa
+00011050: 6972 7329 292c 5f78 6929 290a 0a20 2020  irs)),_xi))..   
+00011060: 2020 2020 2020 2020 206c 315f 6c61 6265           l1_labe
+00011070: 6c2c 6c32 5f6c 6162 656c 203d 2072 6177  l,l2_label = raw
+00011080: 5f64 6174 612e 636f 6c75 6d6e 735b 315d  _data.columns[1]
+00011090: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000110a0: 2078 203d 3d20 2769 6e64 6578 273a 0a20   x == 'index':. 
+000110b0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+000110c0: 2c59 2c59 4520 3d20 7a69 7028 2a58 5f59  ,Y,YE = zip(*X_Y
+000110d0: 5f59 4529 0a20 2020 2020 2020 2020 2020  _YE).           
+000110e0: 2020 2020 2063 6f6c 6f72 2020 3d20 7365       color  = se
+000110f0: 6c66 2e5f 6765 745f 636f 6c6f 7228 636f  lf._get_color(co
+00011100: 6c6f 7273 2c20 2020 2020 2020 2020 2020  lors,           
+00011110: 2020 2020 2020 2020 2020 2020 2020 3029                0)
+00011120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011130: 2069 6620 6d6f 6465 203d 3d20 2264 6966   if mode == "dif
+00011140: 6622 3a0a 2020 2020 2020 2020 2020 2020  f":.            
+00011150: 2020 2020 2020 2020 6c61 6265 6c20 203d          label  =
+00011160: 2073 656c 662e 5f67 6574 5f6c 6162 656c   self._get_label
+00011170: 286c 6162 656c 732c 6627 7b6c 325f 6c61  (labels,f'{l2_la
+00011180: 6265 6c7d 20e2 8094 207b 6c31 5f6c 6162  bel} ... {l1_lab
+00011190: 656c 7d27 2c30 290a 2020 2020 2020 2020  el}',0).        
+000111a0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
 000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111c0: 206c 325f 6c65 6e20 3d20 6c65 6e28 7374   l2_len = len(st
-000111d0: 7228 6c32 5b30 5d29 290a 2020 2020 2020  r(l2[0])).      
-000111e0: 2020 2020 2020 2020 2020 2020 2020 6c31                l1
-000111f0: 203d 206c 6973 7428 6d61 7028 7374 722c   = list(map(str,
-00011200: 6c31 2929 0a20 2020 2020 2020 2020 2020  l1)).           
-00011210: 2020 2020 2020 2020 2058 5f59 5f59 4520           X_Y_YE 
-00011220: 3d20 736f 7274 6564 2858 5f59 5f59 452c  = sorted(X_Y_YE,
-00011230: 206b 6579 3d6c 616d 6264 6120 6974 656d   key=lambda item
-00011240: 733a 206c 312e 696e 6465 7828 6974 656d  s: l1.index(item
-00011250: 735b 305d 5b6c 325f 6c65 6e2b 313a 5d29  s[0][l2_len+1:])
-00011260: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011270: 2020 656c 6966 206c 656e 286c 3229 203e    elif len(l2) >
-00011280: 2031 2061 6e64 206c 656e 286c 3129 203d   1 and len(l1) =
-00011290: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-000112a0: 2020 2020 2020 2020 2023 536f 7274 2062           #Sort b
-000112b0: 7920 6c32 2e20 5765 2061 7373 756d 6520  y l2. We assume 
-000112c0: 5f78 2069 7320 6622 7b6c 327d 2d7b 6c31  _x is f"{l2}-{l1
-000112d0: 7d22 2e0a 2020 2020 2020 2020 2020 2020  }"..            
-000112e0: 2020 2020 2020 2020 6c31 5f6c 656e 203d          l1_len =
-000112f0: 206c 656e 2873 7472 286c 315b 305d 2929   len(str(l1[0]))
-00011300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011310: 2020 2020 206c 3220 3d20 6c69 7374 286d       l2 = list(m
-00011320: 6170 2873 7472 2c6c 3229 290a 2020 2020  ap(str,l2)).    
+000111c0: 2020 6c61 6265 6c20 203d 2073 656c 662e    label  = self.
+000111d0: 5f67 6574 5f6c 6162 656c 286c 6162 656c  _get_label(label
+000111e0: 732c 6627 505b 7b6c 325f 6c61 6265 6c7d  s,f'P[{l2_label}
+000111f0: 203e 207b 6c31 5f6c 6162 656c 7d5d 272c   > {l1_label}]',
+00011200: 3029 0a0a 2020 2020 2020 2020 2020 2020  0)..            
+00011210: 2020 2020 6c61 6265 6c20 203d 2066 227b      label  = f"{
+00011220: 6c61 6265 6c7d 2220 6966 206c 6567 656e  label}" if legen
+00011230: 6420 656c 7365 204e 6f6e 650a 2020 2020  d else None.    
+00011240: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+00011250: 7320 203d 205b 506f 696e 7473 2858 2c20  s  = [Points(X, 
+00011260: 592c 204e 6f6e 652c 2059 452c 2073 7479  Y, None, YE, sty
+00011270: 6c65 3d73 7479 6c65 2c20 6c61 6265 6c3d  le=style, label=
+00011280: 6c61 6265 6c2c 2063 6f6c 6f72 3d63 6f6c  label, color=col
+00011290: 6f72 2c20 616c 7068 613d 616c 7068 6129  or, alpha=alpha)
+000112a0: 5d0a 0a20 2020 2020 2020 2020 2020 2065  ]..            e
+000112b0: 6c69 6620 7820 3d3d 206c 3a0a 2020 2020  lif x == l:.    
+000112c0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+000112d0: 656e 286c 3129 203e 2031 2061 6e64 206c  en(l1) > 1 and l
+000112e0: 656e 286c 3229 203d 3d20 313a 0a20 2020  en(l2) == 1:.   
+000112f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011300: 2023 536f 7274 2062 7920 6c31 2e20 5765   #Sort by l1. We
+00011310: 2061 7373 756d 6520 5f78 2069 7320 6622   assume _x is f"
+00011320: 7b6c 327d 2d7b 6c31 7d22 2e0a 2020 2020  {l2}-{l1}"..    
 00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011340: 585f 595f 5945 203d 2073 6f72 7465 6428  X_Y_YE = sorted(
-00011350: 585f 595f 5945 2c20 6b65 793d 6c61 6d62  X_Y_YE, key=lamb
-00011360: 6461 2069 7465 6d73 3a20 6c32 2e69 6e64  da items: l2.ind
-00011370: 6578 2869 7465 6d73 5b30 5d5b 3a2d 286c  ex(items[0][:-(l
-00011380: 315f 6c65 6e2b 3129 5d29 290a 2020 2020  1_len+1)])).    
-00011390: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000113a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000113b0: 2020 2020 2020 585f 595f 5945 203d 2073        X_Y_YE = s
-000113c0: 6f72 7465 6428 585f 595f 5945 290a 0a20  orted(X_Y_YE).. 
-000113d0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
-000113e0: 2c59 2c59 4520 3d20 7a69 7028 2a58 5f59  ,Y,YE = zip(*X_Y
-000113f0: 5f59 4529 0a20 2020 2020 2020 2020 2020  _YE).           
-00011400: 2020 2020 2063 6f6c 6f72 2020 3d20 7365       color  = se
-00011410: 6c66 2e5f 6765 745f 636f 6c6f 7228 636f  lf._get_color(co
-00011420: 6c6f 7273 2c20 3029 0a20 2020 2020 2020  lors, 0).       
-00011430: 2020 2020 2020 2020 206c 696e 6573 2020           lines  
-00011440: 3d20 5b50 6f69 6e74 7328 582c 2059 2c20  = [Points(X, Y, 
-00011450: 4e6f 6e65 2c20 5945 2c20 7374 796c 653d  None, YE, style=
-00011460: 7374 796c 652c 206c 6162 656c 3d4e 6f6e  style, label=Non
-00011470: 652c 2063 6f6c 6f72 3d63 6f6c 6f72 2c20  e, color=color, 
-00011480: 616c 7068 613d 616c 7068 6129 5d0a 0a20  alpha=alpha)].. 
-00011490: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000114a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000114b0: 2075 7070 6572 203d 206c 616d 6264 6120   upper = lambda 
-000114c0: 792c 7965 3a20 792b 7965 5b31 5d20 6966  y,ye: y+ye[1] if
-000114d0: 2069 7369 6e73 7461 6e63 6528 7965 2c28   isinstance(ye,(
-000114e0: 6c69 7374 2c74 7570 6c65 2929 2065 6c73  list,tuple)) els
-000114f0: 6520 792b 7965 0a20 2020 2020 2020 2020  e y+ye.         
-00011500: 2020 2020 2020 206c 6f77 6572 203d 206c         lower = l
-00011510: 616d 6264 6120 792c 7965 3a20 792d 7965  ambda y,ye: y-ye
-00011520: 5b30 5d20 6966 2069 7369 6e73 7461 6e63  [0] if isinstanc
-00011530: 6528 7965 2c28 6c69 7374 2c74 7570 6c65  e(ye,(list,tuple
-00011540: 2929 2065 6c73 6520 792d 7965 0a20 2020  )) else y-ye.   
-00011550: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00011560: 7020 203d 206c 616d 6264 6120 5f78 3a20  p  = lambda _x: 
-00011570: 7374 7228 5f78 2920 6966 206e 6f74 2078  str(_x) if not x
-00011580: 6f72 6465 7220 656c 7365 205f 780a 0a20  order else _x.. 
-00011590: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000115a0: 7370 6c69 7420 696e 746f 2077 696e 2c74  split into win,t
-000115b0: 6965 2c6c 6f73 730a 2020 2020 2020 2020  ie,loss.        
-000115c0: 2020 2020 2020 2020 6c31 5f77 696e 203d          l1_win =
-000115d0: 205b 2870 7265 7028 7829 2c79 2c79 6529   [(prep(x),y,ye)
-000115e0: 2066 6f72 2078 2c79 2c79 6520 696e 2058   for x,y,ye in X
-000115f0: 5f59 5f59 4520 6966 2075 7070 6572 2879  _Y_YE if upper(y
-00011600: 2c79 6529 203c 2020 5f62 6f75 6e64 6172  ,ye) <  _boundar
-00011610: 7920 2020 2020 2020 2020 2020 2020 2020  y               
-00011620: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-00011630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011640: 6e6f 5f77 696e 203d 205b 2870 7265 7028  no_win = [(prep(
-00011650: 7829 2c79 2c79 6529 2066 6f72 2078 2c79  x),y,ye) for x,y
-00011660: 2c79 6520 696e 2058 5f59 5f59 4520 6966  ,ye in X_Y_YE if
-00011670: 206c 6f77 6572 2879 2c79 6529 203c 3d20   lower(y,ye) <= 
-00011680: 5f62 6f75 6e64 6172 7920 616e 6420 5f62  _boundary and _b
-00011690: 6f75 6e64 6172 7920 3c3d 2075 7070 6572  oundary <= upper
-000116a0: 2879 2c79 6529 5d0a 2020 2020 2020 2020  (y,ye)].        
-000116b0: 2020 2020 2020 2020 6c32 5f77 696e 203d          l2_win =
-000116c0: 205b 2870 7265 7028 7829 2c79 2c79 6529   [(prep(x),y,ye)
-000116d0: 2066 6f72 2078 2c79 2c79 6520 696e 2058   for x,y,ye in X
-000116e0: 5f59 5f59 4520 6966 2020 2020 2020 2020  _Y_YE if        
-000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011700: 2020 2020 2020 5f62 6f75 6e64 6172 7920        _boundary 
-00011710: 3c20 206c 6f77 6572 2879 2c79 6529 5d0a  <  lower(y,ye)].
-00011720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011730: 2023 736f 7274 2062 7920 6f72 6465 7220   #sort by order 
-00011740: 6f66 206d 6167 6e69 7475 6465 0a20 2020  of magnitude.   
-00011750: 2020 2020 2020 2020 2020 2020 206c 315f               l1_
-00011760: 7769 6e20 3d20 736f 7274 6564 286c 315f  win = sorted(l1_
-00011770: 7769 6e2c 6b65 793d 6974 656d 6765 7474  win,key=itemgett
-00011780: 6572 2831 2929 0a20 2020 2020 2020 2020  er(1)).         
-00011790: 2020 2020 2020 206e 6f5f 7769 6e20 3d20         no_win = 
-000117a0: 736f 7274 6564 286e 6f5f 7769 6e2c 6b65  sorted(no_win,ke
-000117b0: 793d 6974 656d 6765 7474 6572 2831 2929  y=itemgetter(1))
-000117c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000117d0: 206c 325f 7769 6e20 3d20 736f 7274 6564   l2_win = sorted
-000117e0: 286c 325f 7769 6e2c 6b65 793d 6974 656d  (l2_win,key=item
-000117f0: 6765 7474 6572 2831 2929 0a0a 2020 2020  getter(1))..    
-00011800: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-00011810: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
-00011820: 2020 2020 2020 2020 582c 592c 5945 203d          X,Y,YE =
-00011830: 207a 6970 282a 6c31 5f77 696e 2920 6966   zip(*l1_win) if
-00011840: 206c 315f 7769 6e20 656c 7365 2028 2829   l1_win else (()
-00011850: 2c28 292c 4e6f 6e65 290a 2020 2020 2020  ,(),None).      
-00011860: 2020 2020 2020 2020 2020 636f 6c6f 7220            color 
-00011870: 203d 2073 656c 662e 5f67 6574 5f63 6f6c   = self._get_col
-00011880: 6f72 2863 6f6c 6f72 732c 2020 2020 2020  or(colors,      
-00011890: 2020 2030 290a 2020 2020 2020 2020 2020     0).          
-000118a0: 2020 2020 2020 6c61 6265 6c20 203d 2073        label  = s
-000118b0: 656c 662e 5f67 6574 5f6c 6162 656c 286c  elf._get_label(l
-000118c0: 6162 656c 732c 6c31 5f6c 6162 656c 2c30  abels,l1_label,0
-000118d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000118e0: 2020 6c61 6265 6c20 203d 2066 227b 6c61    label  = f"{la
-000118f0: 6265 6c7d 2028 7b6c 656e 2858 297d 2922  bel} ({len(X)})"
-00011900: 2069 6620 6c65 6765 6e64 2065 6c73 6520   if legend else 
-00011910: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00011920: 2020 2020 206c 696e 6573 2e61 7070 656e       lines.appen
-00011930: 6428 506f 696e 7473 2858 2c20 592c 204e  d(Points(X, Y, N
-00011940: 6f6e 652c 2059 452c 2073 7479 6c65 3d73  one, YE, style=s
-00011950: 7479 6c65 2c20 6c61 6265 6c3d 6c61 6265  tyle, label=labe
-00011960: 6c2c 2063 6f6c 6f72 3d63 6f6c 6f72 2c20  l, color=color, 
-00011970: 616c 7068 613d 616c 7068 6129 290a 0a20  alpha=alpha)).. 
-00011980: 2020 2020 2020 2020 2020 2020 2020 2058                 X
-00011990: 2c59 2c59 4520 3d20 7a69 7028 2a6e 6f5f  ,Y,YE = zip(*no_
-000119a0: 7769 6e29 2069 6620 6e6f 5f77 696e 2065  win) if no_win e
-000119b0: 6c73 6520 2828 292c 2829 2c4e 6f6e 6529  lse ((),(),None)
-000119c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000119d0: 2063 6f6c 6f72 2020 3d20 7365 6c66 2e5f   color  = self._
-000119e0: 6765 745f 636f 6c6f 7228 636f 6c6f 7273  get_color(colors
-000119f0: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
-00011a00: 2020 2020 206c 6162 656c 2020 3d20 2754       label  = 'T
-00011a10: 6965 270a 2020 2020 2020 2020 2020 2020  ie'.            
-00011a20: 2020 2020 6c61 6265 6c20 203d 2066 227b      label  = f"{
-00011a30: 6c61 6265 6c7d 2028 7b6c 656e 2858 297d  label} ({len(X)}
-00011a40: 2922 2069 6620 6c65 6765 6e64 2065 6c73  )" if legend els
-00011a50: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
-00011a60: 2020 2020 2020 206c 696e 6573 2e61 7070         lines.app
-00011a70: 656e 6428 506f 696e 7473 2858 2c20 592c  end(Points(X, Y,
-00011a80: 204e 6f6e 652c 2059 452c 2073 7479 6c65   None, YE, style
-00011a90: 3d73 7479 6c65 2c20 6c61 6265 6c3d 6c61  =style, label=la
-00011aa0: 6265 6c2c 2063 6f6c 6f72 3d63 6f6c 6f72  bel, color=color
-00011ab0: 2c20 616c 7068 613d 616c 7068 6129 290a  , alpha=alpha)).
-00011ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011ad0: 2058 2c59 2c59 4520 3d20 7a69 7028 2a6c   X,Y,YE = zip(*l
-00011ae0: 325f 7769 6e29 2069 6620 6c32 5f77 696e  2_win) if l2_win
-00011af0: 2065 6c73 6520 2828 292c 2829 2c4e 6f6e   else ((),(),Non
-00011b00: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00011b10: 2020 2063 6f6c 6f72 2020 3d20 7365 6c66     color  = self
-00011b20: 2e5f 6765 745f 636f 6c6f 7228 636f 6c6f  ._get_color(colo
-00011b30: 7273 2c20 2020 2020 2020 2020 3229 0a20  rs,         2). 
-00011b40: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00011b50: 6162 656c 2020 3d20 7365 6c66 2e5f 6765  abel  = self._ge
-00011b60: 745f 6c61 6265 6c28 6c61 6265 6c73 2c6c  t_label(labels,l
-00011b70: 325f 6c61 6265 6c2c 3129 0a20 2020 2020  2_label,1).     
-00011b80: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00011b90: 2020 3d20 6622 7b6c 6162 656c 7d20 287b    = f"{label} ({
-00011ba0: 6c65 6e28 5829 7d29 2220 6966 206c 6567  len(X)})" if leg
-00011bb0: 656e 6420 656c 7365 204e 6f6e 650a 2020  end else None.  
-00011bc0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-00011bd0: 6e65 732e 6170 7065 6e64 2850 6f69 6e74  nes.append(Point
-00011be0: 7328 582c 2059 2c20 4e6f 6e65 2c20 5945  s(X, Y, None, YE
-00011bf0: 2c20 7374 796c 653d 7374 796c 652c 206c  , style=style, l
-00011c00: 6162 656c 3d6c 6162 656c 2c20 636f 6c6f  abel=label, colo
-00011c10: 723d 636f 6c6f 722c 2061 6c70 6861 3d61  r=color, alpha=a
-00011c20: 6c70 6861 2929 0a0a 2020 2020 2020 2020  lpha))..        
-00011c30: 2020 2020 7872 6f74 6174 696f 6e20 3d20      xrotation = 
-00011c40: 3930 2069 6620 2878 2021 3d20 2769 6e64  90 if (x != 'ind
-00011c50: 6578 2720 6f72 2078 6f72 6465 7229 2061  ex' or xorder) a
-00011c60: 6e64 206c 656e 2858 5f59 5f59 4529 3e35  nd len(X_Y_YE)>5
-00011c70: 2065 6c73 6520 300a 2020 2020 2020 2020   else 0.        
-00011c80: 2020 2020 7972 6f74 6174 696f 6e20 3d20      yrotation = 
-00011c90: 300a 0a20 2020 2020 2020 2020 2020 205f  0..            _
-00011ca0: 5920 3d20 7261 775f 6461 7461 5b72 6177  Y = raw_data[raw
-00011cb0: 5f64 6174 612e 636f 6c75 6d6e 735b 315d  _data.columns[1]
-00011cc0: 5d5b 305d 0a0a 2020 2020 2020 2020 2020  ][0]..          
-00011cd0: 2020 786c 6162 656c 203d 2078 6c61 6265    xlabel = xlabe
-00011ce0: 6c20 6f72 2028 2249 6e74 6572 6163 7469  l or ("Interacti
-00011cf0: 6f6e 2220 6966 2078 3d3d 2769 6e64 6578  on" if x=='index
-00011d00: 2720 656c 7365 2078 5b30 5d20 6966 206c  ' else x[0] if l
-00011d10: 656e 2878 2920 3d3d 2031 2065 6c73 6520  en(x) == 1 else 
-00011d20: 7829 0a20 2020 2020 2020 2020 2020 2079  x).            y
-00011d30: 6c61 6265 6c20 3d20 796c 6162 656c 206f  label = ylabel o
-00011d40: 7220 2866 2224 5c44 656c 7461 2420 7b79  r (f"$\Delta$ {y
-00011d50: 7d22 2069 6620 6d6f 6465 3d3d 2264 6966  }" if mode=="dif
-00011d60: 6622 2065 6c73 6520 6622 5028 245c 4465  f" else f"P($\De
-00011d70: 6c74 6124 207b 797d 203e 2030 2922 290a  lta$ {y} > 0)").
-00011d80: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-00011d90: 6520 203d 2074 6974 6c65 2069 6620 7469  e  = title if ti
-00011da0: 746c 6520 6973 206e 6f74 204e 6f6e 6520  tle is not None 
-00011db0: 656c 7365 2028 6622 7b79 6c61 6265 6c7d  else (f"{ylabel}
-00011dc0: 2028 7b6c 656e 285f 5929 7d20 456e 7669   ({len(_Y)} Envi
-00011dd0: 726f 6e6d 656e 7473 2922 290a 0a20 2020  ronments)")..   
-00011de0: 2020 2020 2020 2020 2061 6c6c 5f78 203d           all_x =
-00011df0: 2064 6963 742e 6672 6f6d 6b65 7973 2863   dict.fromkeys(c
-00011e00: 6861 696e 2e66 726f 6d5f 6974 6572 6162  hain.from_iterab
-00011e10: 6c65 286c 696e 652e 5820 666f 7220 6c69  le(line.X for li
-00011e20: 6e65 2069 6e20 6c69 6e65 7329 290a 2020  ne in lines)).  
-00011e30: 2020 2020 2020 2020 2020 786f 7264 6572            xorder
-00011e40: 6564 203d 206c 6973 7428 616c 6c5f 782e  ed = list(all_x.
-00011e50: 6b65 7973 2829 2920 6966 206e 6f74 2078  keys()) if not x
-00011e60: 6f72 6465 7220 656c 7365 2073 6f72 7465  order else sorte
-00011e70: 6428 616c 6c5f 782c 2072 6576 6572 7365  d(all_x, reverse
-00011e80: 3d78 6f72 6465 723d 3d27 2d27 290a 0a20  =xorder=='-').. 
-00011e90: 2020 2020 2020 2020 2020 2069 6620 626f             if bo
-00011ea0: 756e 6461 7279 3a0a 2020 2020 2020 2020  undary:.        
-00011eb0: 2020 2020 2020 2020 6c69 6e65 732e 6170          lines.ap
-00011ec0: 7065 6e64 2850 6f69 6e74 7328 2878 6f72  pend(Points((xor
-00011ed0: 6465 7265 645b 305d 2c78 6f72 6465 7265  dered[0],xordere
-00011ee0: 645b 2d31 5d29 2c28 5f62 6f75 6e64 6172  d[-1]),(_boundar
-00011ef0: 792c 5f62 6f75 6e64 6172 7929 2c20 4e6f  y,_boundary), No
-00011f00: 6e65 2c20 4e6f 6e65 202c 2022 2338 3838  ne, None , "#888
-00011f10: 222c 2031 2c20 4e6f 6e65 2c20 272d 272c  ", 1, None, '-',
-00011f20: 2e35 2929 0a0a 2020 2020 2020 2020 2020  .5))..          
-00011f30: 2020 6966 2078 203d 3d20 2769 6e64 6578    if x == 'index
-00011f40: 2720 616e 6420 786f 7264 6572 2069 6e20  ' and xorder in 
-00011f50: 5b27 2b27 2c4e 6f6e 655d 3a0a 2020 2020  ['+',None]:.    
-00011f60: 2020 2020 2020 2020 2020 2020 786f 7264              xord
-00011f70: 6572 6564 203d 204e 6f6e 650a 0a20 2020  ered = None..   
-00011f80: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
-00011f90: 6c6f 7474 6572 2e70 6c6f 7428 6178 2c20  lotter.plot(ax, 
-00011fa0: 6c69 6e65 732c 2074 6974 6c65 2c20 786c  lines, title, xl
-00011fb0: 6162 656c 2c20 796c 6162 656c 2c20 786c  abel, ylabel, xl
-00011fc0: 696d 2c20 796c 696d 2c20 7874 6963 6b73  im, ylim, xticks
-00011fd0: 2c20 7974 6963 6b73 2c20 6c65 6765 6e64  , yticks, legend
-00011fe0: 2c20 7872 6f74 6174 696f 6e2c 2079 726f  , xrotation, yro
-00011ff0: 7461 7469 6f6e 2c20 786f 7264 6572 6564  tation, xordered
-00012000: 2c20 6f75 7429 0a0a 2020 2020 2020 2020  , out)..        
-00012010: 6578 6365 7074 2043 6f62 6145 7863 6570  except CobaExcep
-00012020: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
-00012030: 2020 2020 2020 2043 6f62 6143 6f6e 7465         CobaConte
-00012040: 7874 2e6c 6f67 6765 722e 6c6f 6728 7374  xt.logger.log(st
-00012050: 7228 6529 290a 0a20 2020 2064 6566 205f  r(e))..    def _
-00012060: 5f73 7472 5f5f 2873 656c 6629 202d 3e20  _str__(self) -> 
-00012070: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
-00012080: 7572 6e20 7374 7228 7b22 4c65 6172 6e65  urn str({"Learne
-00012090: 7273 223a 206c 656e 2873 656c 662e 5f6c  rs": len(self._l
-000120a0: 6561 726e 6572 7329 2c20 2245 6e76 6972  earners), "Envir
-000120b0: 6f6e 6d65 6e74 7322 3a20 6c65 6e28 7365  onments": len(se
-000120c0: 6c66 2e5f 656e 7669 726f 6e6d 656e 7473  lf._environments
-000120d0: 292c 2022 496e 7465 7261 6374 696f 6e73  ), "Interactions
-000120e0: 223a 206c 656e 2873 656c 662e 5f69 6e74  ": len(self._int
-000120f0: 6572 6163 7469 6f6e 7329 207d 290a 0a20  eractions) }).. 
-00012100: 2020 2064 6566 205f 5f65 715f 5f28 7365     def __eq__(se
-00012110: 6c66 2c20 6f3a 206f 626a 6563 7429 202d  lf, o: object) -
-00012120: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-00012130: 7265 7475 726e 2069 7369 6e73 7461 6e63  return isinstanc
-00012140: 6528 6f2c 5265 7375 6c74 2920 5c0a 2020  e(o,Result) \.  
-00012150: 2020 2020 2020 2020 2061 6e64 206f 2e65           and o.e
-00012160: 6e76 6972 6f6e 6d65 6e74 7320 3d3d 2073  nvironments == s
-00012170: 656c 662e 656e 7669 726f 6e6d 656e 7473  elf.environments
-00012180: 205c 0a20 2020 2020 2020 2020 2020 616e   \.           an
-00012190: 6420 6f2e 6c65 6172 6e65 7273 203d 3d20  d o.learners == 
-000121a0: 7365 6c66 2e6c 6561 726e 6572 7320 5c0a  self.learners \.
-000121b0: 2020 2020 2020 2020 2020 2061 6e64 206f             and o
-000121c0: 2e65 7661 6c75 6174 6f72 7320 3d3d 2073  .evaluators == s
-000121d0: 656c 662e 6576 616c 7561 746f 7273 0a0a  elf.evaluators..
-000121e0: 2020 2020 6465 6620 5f69 7079 7468 6f6e      def _ipython
-000121f0: 5f64 6973 706c 6179 5f28 7365 6c66 293a  _display_(self):
-00012200: 0a20 2020 2020 2020 2023 7072 6574 7479  .        #pretty
-00012210: 2070 7269 6e74 2069 6e20 6a75 7079 7465   print in jupyte
-00012220: 7220 6e6f 7465 626f 6f6b 2028 6874 7470  r notebook (http
-00012230: 733a 2f2f 6970 7974 686f 6e2e 7265 6164  s://ipython.read
-00012240: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
-00012250: 6162 6c65 2f63 6f6e 6669 672f 696e 7465  able/config/inte
-00012260: 6772 6174 696e 672e 6874 6d6c 290a 2020  grating.html).  
-00012270: 2020 2020 2020 7072 696e 7428 7374 7228        print(str(
-00012280: 7365 6c66 2929 0a0a 2020 2020 6465 6620  self))..    def 
-00012290: 5f67 6574 5f63 6f6c 6f72 2873 656c 662c  _get_color(self,
-000122a0: 2063 6f6c 6f72 733a 556e 696f 6e5b 4e6f   colors:Union[No
-000122b0: 6e65 2c53 6571 7565 6e63 655b 556e 696f  ne,Sequence[Unio
-000122c0: 6e5b 7374 722c 696e 745d 5d5d 2c20 693a  n[str,int]]], i:
-000122d0: 696e 7429 202d 3e20 556e 696f 6e5b 7374  int) -> Union[st
-000122e0: 722c 696e 745d 3a0a 2020 2020 2020 2020  r,int]:.        
-000122f0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00012300: 2072 6574 7572 6e20 636f 6c6f 7273 2069   return colors i
-00012310: 6620 6973 696e 7374 616e 6365 2863 6f6c  f isinstance(col
-00012320: 6f72 732c 7374 7229 2065 6c73 6520 636f  ors,str) else co
-00012330: 6c6f 7273 5b69 5d20 6966 2063 6f6c 6f72  lors[i] if color
-00012340: 7320 656c 7365 2069 0a20 2020 2020 2020  s else i.       
-00012350: 2065 7863 6570 7420 496e 6465 7845 7272   except IndexErr
-00012360: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00012370: 7265 7475 726e 2069 2b6d 6178 2863 6f6c  return i+max(col
-00012380: 6f72 7329 2069 6620 6973 696e 7374 616e  ors) if isinstan
-00012390: 6365 2863 6f6c 6f72 735b 305d 2c28 696e  ce(colors[0],(in
-000123a0: 742c 666c 6f61 7429 2920 656c 7365 2069  t,float)) else i
-000123b0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-000123c0: 5479 7065 4572 726f 723a 0a20 2020 2020  TypeError:.     
-000123d0: 2020 2020 2020 2072 6574 7572 6e20 692b         return i+
-000123e0: 636f 6c6f 7273 0a0a 2020 2020 6465 6620  colors..    def 
-000123f0: 5f67 6574 5f6c 6162 656c 2873 656c 662c  _get_label(self,
-00012400: 206c 6162 656c 733a 5365 7175 656e 6365   labels:Sequence
-00012410: 5b73 7472 5d2c 206c 6162 656c 3a73 7472  [str], label:str
-00012420: 2c20 693a 696e 7429 202d 3e20 7374 723a  , i:int) -> str:
-00012430: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00012440: 2020 2020 2020 2020 2020 6c61 6265 6c20            label 
-00012450: 3d20 6c61 6265 6c73 2069 6620 6973 696e  = labels if isin
-00012460: 7374 616e 6365 286c 6162 656c 732c 7374  stance(labels,st
-00012470: 7229 2065 6c73 6520 6c61 6265 6c73 5b69  r) else labels[i
-00012480: 5d20 6966 206c 6162 656c 7320 656c 7365  ] if labels else
-00012490: 206c 6162 656c 0a20 2020 2020 2020 2065   label.        e
-000124a0: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
-000124b0: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-000124c0: 7265 7475 726e 2073 7472 286c 6162 656c  return str(label
-000124d0: 290a 0a20 2020 2064 6566 205f 706c 6f74  )..    def _plot
-000124e0: 7461 626c 6528 7365 6c66 2c20 783a 5365  table(self, x:Se
-000124f0: 7175 656e 6365 5b73 7472 5d2c 2079 3a73  quence[str], y:s
-00012500: 7472 2920 2d3e 2027 5265 7375 6c74 273a  tr) -> 'Result':
-00012510: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00012520: 2069 7369 6e73 7461 6e63 6528 782c 7374   isinstance(x,st
-00012530: 7229 2061 6e64 2027 696e 6465 7827 2069  r) and 'index' i
-00012540: 6e20 7820 616e 6420 6c65 6e28 7829 203e  n x and len(x) >
-00012550: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00012560: 7261 6973 6520 436f 6261 4578 6365 7074  raise CobaExcept
-00012570: 696f 6e28 2754 6865 2078 2d61 7869 7320  ion('The x-axis 
-00012580: 6361 6e6e 6f74 2063 6f6e 7461 696e 2062  cannot contain b
-00012590: 6f74 6820 696e 6465 7865 7320 616e 6420  oth indexes and 
-000125a0: 7061 7261 6d65 7465 7273 2e27 290a 0a20  parameters.').. 
-000125b0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
-000125c0: 6c66 2e69 6e74 6572 6163 7469 6f6e 7329  lf.interactions)
-000125d0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-000125e0: 2020 2072 6169 7365 2043 6f62 6145 7863     raise CobaExc
-000125f0: 6570 7469 6f6e 2822 5468 6973 2072 6573  eption("This res
-00012600: 756c 7420 646f 6573 206e 6f74 2063 6f6e  ult does not con
-00012610: 7461 696e 2061 6e79 2064 6174 6120 746f  tain any data to
-00012620: 2070 6c6f 742e 2229 0a0a 2020 2020 2020   plot.")..      
-00012630: 2020 6966 2079 206e 6f74 2069 6e20 7365    if y not in se
-00012640: 6c66 2e69 6e74 6572 6163 7469 6f6e 732e  lf.interactions.
-00012650: 636f 6c75 6d6e 733a 0a20 2020 2020 2020  columns:.       
-00012660: 2020 2020 2072 6169 7365 2043 6f62 6145       raise CobaE
-00012670: 7863 6570 7469 6f6e 2866 2254 6869 7320  xception(f"This 
-00012680: 7265 7375 6c74 2064 6f65 7320 6e6f 7420  result does not 
-00012690: 636f 6e74 6169 6e20 636f 6c75 6d6e 2027  contain column '
-000126a0: 7b79 7d27 2069 6e20 696e 7465 7261 6374  {y}' in interact
-000126b0: 696f 6e73 2e22 290a 0a20 2020 2020 2020  ions.")..       
-000126c0: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
-000126d0: 2020 6465 6620 5f66 696e 6973 6865 6428    def _finished(
-000126e0: 7365 6c66 2c20 783a 5365 7175 656e 6365  self, x:Sequence
-000126f0: 5b73 7472 5d2c 2079 3a73 7472 2c20 6c3a  [str], y:str, l:
-00012700: 5365 7175 656e 6365 5b73 7472 5d2c 2070  Sequence[str], p
-00012710: 3a53 6571 7565 6e63 655b 7374 725d 2920  :Sequence[str]) 
-00012720: 2d3e 2027 5265 7375 6c74 273a 0a20 2020  -> 'Result':.   
-00012730: 2020 2020 206f 6e6c 795f 6669 6e69 7368       only_finish
-00012740: 6564 203d 2073 656c 662e 5f66 696c 7465  ed = self._filte
-00012750: 725f 6669 6e28 276d 696e 2720 6966 2078  r_fin('min' if x
-00012760: 203d 3d20 2769 6e64 6578 2720 656c 7365   == 'index' else
-00012770: 204e 6f6e 652c 206c 2c20 7029 0a20 2020   None, l, p).   
-00012780: 2020 2020 2069 6620 6c65 6e28 6f6e 6c79       if len(only
-00012790: 5f66 696e 6973 6865 642e 6c65 6172 6e65  _finished.learne
-000127a0: 7273 2920 3d3d 2030 3a0a 2020 2020 2020  rs) == 0:.      
-000127b0: 2020 2020 2020 7261 6973 6520 436f 6261        raise Coba
-000127c0: 4578 6365 7074 696f 6e28 6622 5468 6973  Exception(f"This
-000127d0: 2072 6573 756c 7420 646f 6573 206e 6f74   result does not
-000127e0: 2063 6f6e 7461 696e 2061 207b 707d 2074   contain a {p} t
-000127f0: 6861 7420 6861 7320 6265 656e 2066 696e  hat has been fin
-00012800: 6973 6865 6420 666f 7220 6576 6572 7920  ished for every 
-00012810: 7b6c 7d2e 2229 0a20 2020 2020 2020 2072  {l}.").        r
-00012820: 6574 7572 6e20 6f6e 6c79 5f66 696e 6973  eturn only_finis
-00012830: 6865 640a 0a20 2020 2064 6566 205f 636f  hed..    def _co
-00012840: 6e66 6964 656e 6365 2873 656c 662c 2065  nfidence(self, e
-00012850: 7272 3a20 556e 696f 6e5b 7374 722c 506f  rr: Union[str,Po
-00012860: 696e 7441 6e64 496e 7465 7276 616c 5d2c  intAndInterval],
-00012870: 2065 7272 6576 6572 793a 696e 7420 3d20   errevery:int = 
-00012880: 3129 3a0a 0a20 2020 2020 2020 2069 6620  1):..        if 
-00012890: 6572 7220 3d3d 2027 7365 273a 0a20 2020  err == 'se':.   
-000128a0: 2020 2020 2020 2020 2063 6920 3d20 5374           ci = St
-000128b0: 6445 7272 4349 282e 3935 290a 2020 2020  dErrCI(.95).    
-000128c0: 2020 2020 656c 6966 2065 7272 203d 3d20      elif err == 
-000128d0: 2762 7327 3a0a 2020 2020 2020 2020 2020  'bs':.          
-000128e0: 2020 6369 203d 2042 6f6f 7473 7472 6170    ci = Bootstrap
-000128f0: 4349 282e 3935 2c20 6d65 616e 290a 2020  CI(.95, mean).  
-00012900: 2020 2020 2020 656c 6966 2065 7272 203d        elif err =
-00012910: 3d20 2762 6927 3a0a 2020 2020 2020 2020  = 'bi':.        
-00012920: 2020 2020 6369 203d 2042 696e 6f6d 6961      ci = Binomia
-00012930: 6c43 4928 2777 696c 736f 6e27 290a 2020  lCI('wilson').  
-00012940: 2020 2020 2020 656c 6966 2065 7272 203d        elif err =
-00012950: 3d20 2773 6427 3a0a 2020 2020 2020 2020  = 'sd':.        
-00012960: 2020 2020 6369 203d 2053 7464 4465 7643      ci = StdDevC
-00012970: 4928 290a 2020 2020 2020 2020 656c 6966  I().        elif
-00012980: 2065 7272 2069 7320 4e6f 6e65 206f 7220   err is None or 
-00012990: 6973 696e 7374 616e 6365 2865 7272 2c73  isinstance(err,s
-000129a0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-000129b0: 2063 6920 3d20 4e6f 6e65 0a20 2020 2020   ci = None.     
-000129c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000129d0: 2020 2020 2063 6920 3d20 6572 720a 0a20       ci = err.. 
-000129e0: 2020 2020 2020 2064 6566 2063 616c 635f         def calc_
-000129f0: 6369 285a 3a53 6571 7565 6e63 655b 666c  ci(Z:Sequence[fl
-00012a00: 6f61 745d 2c20 693a 696e 7420 3d20 2d31  oat], i:int = -1
-00012a10: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00012a20: 6620 6369 2069 7320 4e6f 6e65 3a0a 2020  f ci is None:.  
-00012a30: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00012a40: 7475 726e 2028 6d65 616e 285a 292c 3029  turn (mean(Z),0)
-00012a50: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00012a60: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00012a70: 2020 2073 6b69 705f 6572 7220 3d20 2869     skip_err = (i
-00012a80: 2b31 2925 6572 7265 7665 7279 0a20 2020  +1)%errevery.   
-00012a90: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00012aa0: 7572 6e20 2863 692e 706f 696e 7428 5a29  urn (ci.point(Z)
-00012ab0: 2c20 2830 2c30 2929 2069 6620 736b 6970  , (0,0)) if skip
-00012ac0: 5f65 7272 2065 6c73 6520 6369 2e70 6f69  _err else ci.poi
-00012ad0: 6e74 5f69 6e74 6572 7661 6c28 5a29 0a0a  nt_interval(Z)..
-00012ae0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00012af0: 616c 635f 6369 0a0a 2020 2020 6465 6620  alc_ci..    def 
-00012b00: 5f67 726f 7570 6564 5f79 7328 7365 6c66  _grouped_ys(self
-00012b10: 2c20 2a6b 6579 733a 2073 7472 2c20 793a  , *keys: str, y:
-00012b20: 4f70 7469 6f6e 616c 5b73 7472 5d2c 2066  Optional[str], f
-00012b30: 756e 633a 204c 6974 6572 616c 5b27 6c61  unc: Literal['la
-00012b40: 7374 272c 276c 6973 7427 5d20 3d20 4e6f  st','list'] = No
-00012b50: 6e65 2c20 6361 7264 3a20 4c69 7465 7261  ne, card: Litera
-00012b60: 6c5b 2747 272c 2753 275d 203d 2027 4727  l['G','S'] = 'G'
-00012b70: 2c20 7370 616e 3a4f 7074 696f 6e61 6c5b  , span:Optional[
-00012b80: 696e 745d 3d31 2920 2d3e 2053 6571 7565  int]=1) -> Seque
-00012b90: 6e63 655b 5475 706c 655d 3a0a 0a20 2020  nce[Tuple]:..   
-00012ba0: 2020 2020 2065 6e76 5f63 6163 6865 203d       env_cache =
-00012bb0: 2073 656c 662e 5f65 6e76 5f63 6163 6865   self._env_cache
-00012bc0: 0a20 2020 2020 2020 206c 726e 5f63 6163  .        lrn_cac
-00012bd0: 6865 203d 2073 656c 662e 5f6c 726e 5f63  he = self._lrn_c
-00012be0: 6163 6865 0a20 2020 2020 2020 2076 616c  ache.        val
-00012bf0: 5f63 6163 6865 203d 2073 656c 662e 5f76  _cache = self._v
-00012c00: 616c 5f63 6163 6865 0a0a 2020 2020 2020  al_cache..      
-00012c10: 2020 6e65 6564 5f68 6173 6865 7220 3d20    need_hasher = 
-00012c20: 4e6f 6e65 0a0a 2020 2020 2020 2020 4420  None..        D 
-00012c30: 3d20 6469 6374 2829 2069 6620 6361 7264  = dict() if card
-00012c40: 203d 3d20 2753 2720 656c 7365 2064 6566   == 'S' else def
-00012c50: 6175 6c74 6469 6374 286c 6973 7429 0a0a  aultdict(list)..
-00012c60: 2020 2020 2020 2020 6465 6620 6973 5f69          def is_i
-00012c70: 636f 6c28 6b65 7929 3a0a 2020 2020 2020  col(key):.      
-00012c80: 2020 2020 2020 7265 7475 726e 206b 6579        return key
-00012c90: 206e 6f74 2069 6e20 5b27 656e 7669 726f   not in ['enviro
-00012ca0: 6e6d 656e 745f 6964 272c 276c 6561 726e  nment_id','learn
-00012cb0: 6572 5f69 6427 2c27 6576 616c 7561 746f  er_id','evaluato
-00012cc0: 725f 6964 275d 2061 6e64 206b 6579 2069  r_id'] and key i
-00012cd0: 6e20 7365 6c66 2e69 6e74 6572 6163 7469  n self.interacti
-00012ce0: 6f6e 732e 636f 6c75 6d6e 730a 0a20 2020  ons.columns..   
-00012cf0: 2020 2020 2064 6566 2067 6574 5f69 636f       def get_ico
-00012d00: 6c73 286b 6579 7329 3a0a 2020 2020 2020  ls(keys):.      
-00012d10: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
-00012d20: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
-00012d30: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00012d40: 616e 6365 286b 6579 2c28 6c69 7374 2c74  ance(key,(list,t
-00012d50: 7570 6c65 2929 3a0a 2020 2020 2020 2020  uple)):.        
-00012d60: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-00012d70: 6420 6672 6f6d 2067 6574 5f69 636f 6c73  d from get_icols
-00012d80: 286b 6579 290a 2020 2020 2020 2020 2020  (key).          
-00012d90: 2020 2020 2020 656c 6966 2069 735f 6963        elif is_ic
-00012da0: 6f6c 286b 6579 293a 0a20 2020 2020 2020  ol(key):.       
-00012db0: 2020 2020 2020 2020 2020 2020 2079 6965               yie
-00012dc0: 6c64 206b 6579 0a0a 2020 2020 2020 2020  ld key..        
-00012dd0: 6465 6620 6d61 6b65 5f67 6574 7328 636f  def make_gets(co
-00012de0: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-00012df0: 2066 6f72 2063 6f6c 2069 6e20 636f 6c73   for col in cols
-00012e00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012e10: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00012e20: 636f 6c2c 2874 7570 6c65 2c6c 6973 7429  col,(tuple,list)
-00012e30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00012e40: 2020 2020 2020 2079 6965 6c64 206c 616d         yield lam
-00012e50: 6264 6120 652c 6c2c 762c 732c 4e2c 473d  bda e,l,v,s,N,G=
-00012e60: 6c69 7374 286d 616b 655f 6765 7473 2863  list(make_gets(c
-00012e70: 6f6c 2929 3a20 7a69 7028 2a6d 6170 286d  ol)): zip(*map(m
-00012e80: 6574 686f 6463 616c 6c65 7228 275f 5f63  ethodcaller('__c
-00012e90: 616c 6c5f 5f27 2c65 2c6c 2c76 2c73 2c4e  all__',e,l,v,s,N
-00012ea0: 292c 4729 2920 6966 204e 2021 3d20 3020  ),G)) if N != 0 
-00012eb0: 656c 7365 2074 7570 6c65 286d 6170 286d  else tuple(map(m
-00012ec0: 6574 686f 6463 616c 6c65 7228 275f 5f63  ethodcaller('__c
-00012ed0: 616c 6c5f 5f27 2c65 2c6c 2c76 2c73 2c4e  all__',e,l,v,s,N
-00012ee0: 292c 4729 290a 2020 2020 2020 2020 2020  ),G)).          
-00012ef0: 2020 2020 2020 656c 6966 2063 6f6c 2069        elif col i
-00012f00: 6e20 7365 6c66 2e65 6e76 6972 6f6e 6d65  n self.environme
-00012f10: 6e74 732e 636f 6c75 6d6e 733a 0a20 2020  nts.columns:.   
-00012f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f30: 2079 6965 6c64 206c 616d 6264 6120 652c   yield lambda e,
-00012f40: 6c2c 762c 732c 4e2c 636f 6c3d 636f 6c3a  l,v,s,N,col=col:
-00012f50: 2072 6570 6561 7428 655b 636f 6c5d 2c4e   repeat(e[col],N
-00012f60: 2920 6966 204e 2021 3d20 3020 656c 7365  ) if N != 0 else
-00012f70: 2065 5b63 6f6c 5d0a 2020 2020 2020 2020   e[col].        
-00012f80: 2020 2020 2020 2020 656c 6966 2063 6f6c          elif col
-00012f90: 2069 6e20 7365 6c66 2e6c 6561 726e 6572   in self.learner
-00012fa0: 732e 636f 6c75 6d6e 7320 6f72 2063 6f6c  s.columns or col
-00012fb0: 203d 3d20 2766 756c 6c5f 6e61 6d65 273a   == 'full_name':
-00012fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012fd0: 2020 2020 2079 6965 6c64 206c 616d 6264       yield lambd
-00012fe0: 6120 652c 6c2c 762c 732c 4e2c 636f 6c3d  a e,l,v,s,N,col=
-00012ff0: 636f 6c3a 2072 6570 6561 7428 6c5b 636f  col: repeat(l[co
-00013000: 6c5d 2c4e 2920 6966 204e 2021 3d20 3020  l],N) if N != 0 
-00013010: 656c 7365 206c 5b63 6f6c 5d0a 2020 2020  else l[col].    
-00013020: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00013030: 2063 6f6c 2069 6e20 7365 6c66 2e65 7661   col in self.eva
-00013040: 6c75 6174 6f72 732e 636f 6c75 6d6e 733a  luators.columns:
-00013050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013060: 2020 2020 2079 6965 6c64 206c 616d 6264       yield lambd
-00013070: 6120 652c 6c2c 762c 732c 4e2c 636f 6c3d  a e,l,v,s,N,col=
-00013080: 636f 6c3a 2072 6570 6561 7428 765b 636f  col: repeat(v[co
-00013090: 6c5d 2c4e 2920 6966 204e 2021 3d20 3020  l],N) if N != 0 
-000130a0: 656c 7365 2076 5b63 6f6c 5d0a 2020 2020  else v[col].    
-000130b0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000130c0: 2063 6f6c 2069 6e20 7365 6c66 2e69 6e74   col in self.int
-000130d0: 6572 6163 7469 6f6e 732e 636f 6c75 6d6e  eractions.column
-000130e0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000130f0: 2020 2020 2020 2079 6965 6c64 206c 616d         yield lam
-00013100: 6264 6120 652c 6c2c 762c 732c 4e2c 636f  bda e,l,v,s,N,co
-00013110: 6c3d 636f 6c3a 2069 7465 7228 732e 706f  l=col: iter(s.po
-00013120: 7028 2929 0a0a 2020 2020 2020 2020 6765  p())..        ge
-00013130: 7473 2020 3d20 6c69 7374 286d 616b 655f  ts  = list(make_
-00013140: 6765 7473 286b 6579 7329 290a 2020 2020  gets(keys)).    
-00013150: 2020 2020 6963 6f6c 7320 3d20 6c69 7374      icols = list
-00013160: 2867 6574 5f69 636f 6c73 286b 6579 7329  (get_icols(keys)
-00013170: 290a 2020 2020 2020 2020 6963 6f6c 732e  ).        icols.
-00013180: 7265 7665 7273 6528 290a 0a20 2020 2020  reverse()..     
-00013190: 2020 2069 6620 793a 2069 636f 6c73 202b     if y: icols +
-000131a0: 3d20 5b79 5d0a 2020 2020 2020 2020 666f  = [y].        fo
-000131b0: 7220 2865 6964 2c6c 6964 2c76 6964 292c  r (eid,lid,vid),
-000131c0: 2073 656c 2069 6e20 7365 6c66 2e69 6e74   sel in self.int
-000131d0: 6572 6163 7469 6f6e 732e 6772 6f75 7062  eractions.groupb
-000131e0: 7928 332c 6963 6f6c 7329 3a0a 0a20 2020  y(3,icols):..   
-000131f0: 2020 2020 2020 2020 2065 6e76 203d 2065           env = e
-00013200: 6e76 5f63 6163 6865 5b65 6964 5d0a 2020  nv_cache[eid].  
-00013210: 2020 2020 2020 2020 2020 6c72 6e20 3d20            lrn = 
-00013220: 6c72 6e5f 6361 6368 655b 6c69 645d 0a20  lrn_cache[lid]. 
-00013230: 2020 2020 2020 2020 2020 2076 616c 203d             val =
-00013240: 2076 616c 5f63 6163 6865 5b76 6964 5d0a   val_cache[vid].
-00013250: 0a20 2020 2020 2020 2020 2020 2059 203d  .            Y =
-00013260: 2073 656c 2e70 6f70 2829 2069 6620 7920   sel.pop() if y 
-00013270: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
-00013280: 2020 2020 2020 4e20 3d20 3020 6966 206e        N = 0 if n
-00013290: 6f74 2073 656c 2065 6c73 6520 6c65 6e28  ot sel else len(
-000132a0: 7365 6c5b 305d 290a 0a20 2020 2020 2020  sel[0])..       
-000132b0: 2020 2020 206f 7574 7320 3d20 7475 706c       outs = tupl
-000132c0: 6528 6d61 7028 6d65 7468 6f64 6361 6c6c  e(map(methodcall
-000132d0: 6572 2827 5f5f 6361 6c6c 5f5f 272c 656e  er('__call__',en
-000132e0: 762c 6c72 6e2c 7661 6c2c 7365 6c2c 4e29  v,lrn,val,sel,N)
-000132f0: 2c67 6574 7329 290a 0a20 2020 2020 2020  ,gets))..       
-00013300: 2020 2020 2069 6620 4e20 213d 2030 3a20       if N != 0: 
-00013310: 6f75 7473 203d 207a 6970 282a 6f75 7473  outs = zip(*outs
-00013320: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00013330: 204e 203d 3d20 3020 616e 6420 6675 6e63   N == 0 and func
-00013340: 2069 7320 4e6f 6e65 2061 6e64 2079 2069   is None and y i
-00013350: 7320 6e6f 7420 4e6f 6e65 3a20 6675 6e63  s not None: func
-00013360: 203d 2027 6c61 7374 270a 0a20 2020 2020   = 'last'..     
-00013370: 2020 2020 2020 2069 6620 6e65 6564 5f68         if need_h
-00013380: 6173 6865 7220 6973 204e 6f6e 653a 0a20  asher is None:. 
-00013390: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000133a0: 7574 2c20 6f75 7473 203d 2028 6f75 7473  ut, outs = (outs
-000133b0: 2c20 6f75 7473 2920 6966 204e 203d 3d20  , outs) if N == 
-000133c0: 3020 656c 7365 2070 6565 6b5f 6669 7273  0 else peek_firs
-000133d0: 7428 6f75 7473 290a 2020 2020 2020 2020  t(outs).        
-000133e0: 2020 2020 2020 2020 6e65 6564 5f68 6173          need_has
-000133f0: 6865 7220 3d20 7472 795f 656c 7365 286c  her = try_else(l
-00013400: 616d 6264 613a 206e 6f74 2062 6f6f 6c28  ambda: not bool(
-00013410: 6861 7368 286f 7574 2929 2c20 5472 7565  hash(out)), True
-00013420: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013430: 2020 6966 206e 6565 645f 6861 7368 6572    if need_hasher
-00013440: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013450: 2020 2020 2020 7261 6973 6520 436f 6261        raise Coba
-00013460: 4578 6365 7074 696f 6e28 2252 6573 756c  Exception("Resul
-00013470: 7420 7265 7175 6972 6573 2061 6c6c 2064  t requires all d
-00013480: 6174 6120 746f 2062 6520 6861 7368 6162  ata to be hashab
-00013490: 6c65 2e22 290a 0a20 2020 2020 2020 2020  le.")..         
-000134a0: 2020 2069 6620 4e20 3d3d 2030 3a0a 2020     if N == 0:.  
-000134b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000134c0: 2079 2069 7320 4e6f 6e65 3a0a 2020 2020   y is None:.    
-000134d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134e0: 7620 3d20 4e6f 6e65 0a20 2020 2020 2020  v = None.       
-000134f0: 2020 2020 2020 2020 2065 6c69 6620 6675           elif fu
-00013500: 6e63 203d 3d20 276c 6173 7427 3a0a 2020  nc == 'last':.  
-00013510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013520: 2020 7620 3d20 595b 2d31 5d20 6966 2073    v = Y[-1] if s
-00013530: 7061 6e20 3d3d 2031 2065 6c73 6520 6d65  pan == 1 else me
-00013540: 616e 2859 5b2d 7370 616e 3a5d 2920 6966  an(Y[-span:]) if
-00013550: 2073 7061 6e20 656c 7365 206d 6561 6e28   span else mean(
-00013560: 5929 0a20 2020 2020 2020 2020 2020 2020  Y).             
-00013570: 2020 2065 6c69 6620 6675 6e63 203d 3d20     elif func == 
-00013580: 276c 6973 7427 3a0a 2020 2020 2020 2020  'list':.        
-00013590: 2020 2020 2020 2020 2020 2020 7620 3d20              v = 
-000135a0: 590a 2020 2020 2020 2020 2020 2020 2020  Y.              
-000135b0: 2020 6966 2063 6172 6420 3d3d 2027 4727    if card == 'G'
-000135c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000135d0: 2020 2020 2020 445b 6f75 7473 5d2e 6170        D[outs].ap
-000135e0: 7065 6e64 2876 290a 2020 2020 2020 2020  pend(v).        
-000135f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00013600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013610: 2020 445b 6f75 7473 5d20 3d20 760a 2020    D[outs] = v.  
-00013620: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00013630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013640: 6966 2079 2069 7320 4e6f 6e65 3a0a 2020  if y is None:.  
-00013650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013660: 2020 7620 3d20 7265 7065 6174 284e 6f6e    v = repeat(Non
-00013670: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00013680: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00013690: 2020 2020 2020 2020 2020 2020 2076 203d               v =
-000136a0: 206d 6f76 696e 675f 6176 6572 6167 6528   moving_average(
-000136b0: 592c 7370 616e 290a 2020 2020 2020 2020  Y,span).        
-000136c0: 2020 2020 2020 2020 6966 2063 6172 6420          if card 
-000136d0: 3d3d 2027 4727 3a0a 2020 2020 2020 2020  == 'G':.        
-000136e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000136f0: 6f2c 795f 2069 6e20 7a69 7028 6f75 7473  o,y_ in zip(outs
-00013700: 2c76 293a 0a20 2020 2020 2020 2020 2020  ,v):.           
-00013710: 2020 2020 2020 2020 2020 2020 2044 5b6f               D[o
-00013720: 5d2e 6170 7065 6e64 2879 5f29 0a20 2020  ].append(y_).   
-00013730: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00013740: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00013750: 2020 2020 2020 2044 2e75 7064 6174 6528         D.update(
-00013760: 7a69 7028 6f75 7473 2c76 2929 0a0a 2020  zip(outs,v))..  
-00013770: 2020 2020 2020 7265 7475 726e 205b 6b20        return [k 
-00013780: 2b20 2876 2c29 2066 6f72 206b 2c76 2069  + (v,) for k,v i
-00013790: 6e20 442e 6974 656d 7328 295d 0a0a 2020  n D.items()]..  
-000137a0: 2020 6465 6620 5f67 6c6f 6261 6c5f 6e28    def _global_n(
-000137b0: 7365 6c66 2c20 6e3a 2055 6e69 6f6e 5b69  self, n: Union[i
-000137c0: 6e74 2c4c 6974 6572 616c 5b27 6d69 6e27  nt,Literal['min'
-000137d0: 5d5d 293a 0a0a 2020 2020 2020 2020 656e  ]]):..        en
-000137e0: 7669 726f 6e6d 656e 7473 203d 2073 656c  vironments = sel
-000137f0: 662e 656e 7669 726f 6e6d 656e 7473 0a20  f.environments. 
-00013800: 2020 2020 2020 206c 6561 726e 6572 7320         learners 
-00013810: 2020 2020 3d20 7365 6c66 2e6c 6561 726e      = self.learn
-00013820: 6572 730a 2020 2020 2020 2020 6576 616c  ers.        eval
-00013830: 7561 746f 7273 2020 203d 2073 656c 662e  uators   = self.
-00013840: 6576 616c 7561 746f 7273 0a20 2020 2020  evaluators.     
-00013850: 2020 2069 6e74 6572 6163 7469 6f6e 7320     interactions 
-00013860: 3d20 7365 6c66 2e69 6e74 6572 6163 7469  = self.interacti
-00013870: 6f6e 730a 0a20 2020 2020 2020 2065 6e76  ons..        env
-00013880: 5f6c 656e 6774 6873 203d 205b 5d0a 2020  _lengths = [].  
-00013890: 2020 2020 2020 746f 5f64 726f 7020 2020        to_drop   
-000138a0: 2020 3d20 5b5d 0a20 2020 2020 2020 2074    = [].        t
-000138b0: 6f5f 6b65 6570 2020 2020 203d 205b 5d0a  o_keep     = [].
-000138c0: 2020 2020 2020 2020 6966 206e 203d 3d20          if n == 
-000138d0: 276d 696e 273a 0a20 2020 2020 2020 2020  'min':.         
-000138e0: 2020 2066 6f72 2065 6e76 5f69 6478 2c20     for env_idx, 
-000138f0: 656e 765f 6c65 6e20 696e 2073 656c 662e  env_len in self.
-00013900: 696e 7465 7261 6374 696f 6e73 2e67 726f  interactions.gro
-00013910: 7570 6279 2833 2c27 636f 756e 7427 293a  upby(3,'count'):
-00013920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013930: 2065 6e76 5f6c 656e 6774 6873 2e61 7070   env_lengths.app
-00013940: 656e 6428 656e 765f 6c65 6e29 0a20 2020  end(env_len).   
-00013950: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00013960: 2020 2020 2020 2066 6f72 2065 6e76 5f69         for env_i
-00013970: 6478 2c20 656e 765f 6c65 6e20 696e 2073  dx, env_len in s
-00013980: 656c 662e 696e 7465 7261 6374 696f 6e73  elf.interactions
-00013990: 2e67 726f 7570 6279 2833 2c27 636f 756e  .groupby(3,'coun
-000139a0: 7427 293a 0a20 2020 2020 2020 2020 2020  t'):.           
-000139b0: 2020 2020 2069 6620 656e 765f 6c65 6e20       if env_len 
-000139c0: 3c20 6e3a 0a20 2020 2020 2020 2020 2020  < n:.           
-000139d0: 2020 2020 2020 2020 2074 6f5f 6472 6f70           to_drop
-000139e0: 2e61 7070 656e 6428 656e 765f 6964 7829  .append(env_idx)
-000139f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013a00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00013a10: 2020 2020 2020 2020 2020 2065 6e76 5f6c             env_l
-00013a20: 656e 6774 6873 2e61 7070 656e 6428 656e  engths.append(en
-00013a30: 765f 6c65 6e29 0a20 2020 2020 2020 2020  v_len).         
-00013a40: 2020 2020 2020 2020 2020 2074 6f5f 6b65             to_ke
-00013a50: 6570 2e61 7070 656e 6428 656e 765f 6964  ep.append(env_id
-00013a60: 7829 0a0a 2020 2020 2020 2020 6966 2074  x)..        if t
-00013a70: 6f5f 6472 6f70 3a0a 2020 2020 2020 2020  o_drop:.        
-00013a80: 2020 2020 6e5f 6472 6f70 7065 6420 3d20      n_dropped = 
-00013a90: 6c65 6e28 746f 5f64 726f 7029 0a20 2020  len(to_drop).   
-00013aa0: 2020 2020 2020 2020 2069 6e74 6572 6163           interac
-00013ab0: 7469 6f6e 7320 3d20 5461 626c 6528 5669  tions = Table(Vi
-00013ac0: 6577 2869 6e74 6572 6163 7469 6f6e 732e  ew(interactions.
-00013ad0: 5f64 6174 612c 7365 6c66 2e5f 7265 6d6f  _data,self._remo
-00013ae0: 7665 2874 6f5f 6472 6f70 2c6e 2929 2c20  ve(to_drop,n)), 
-00013af0: 696e 7465 7261 6374 696f 6e73 2e63 6f6c  interactions.col
-00013b00: 756d 6e73 2c20 696e 7465 7261 6374 696f  umns, interactio
-00013b10: 6e73 2e69 6e64 6578 6573 290a 2020 2020  ns.indexes).    
-00013b20: 2020 2020 2020 2020 6966 206e 5f64 726f          if n_dro
-00013b30: 7070 6564 3d3d 313a 2043 6f62 6143 6f6e  pped==1: CobaCon
-00013b40: 7465 7874 2e6c 6f67 6765 722e 6c6f 6728  text.logger.log(
-00013b50: 6622 5765 2072 656d 6f76 6564 207b 6e5f  f"We removed {n_
-00013b60: 6472 6f70 7065 647d 206c 6561 726e 6572  dropped} learner
-00013b70: 2065 7661 6c75 6174 696f 6e20 6265 6361   evaluation beca
-00013b80: 7573 6520 6974 2077 6173 2073 686f 7274  use it was short
-00013b90: 6572 2074 6861 6e20 7b6e 7d20 696e 7465  er than {n} inte
-00013ba0: 7261 6374 696f 6e73 2e22 290a 2020 2020  ractions.").    
-00013bb0: 2020 2020 2020 2020 6966 206e 5f64 726f          if n_dro
-00013bc0: 7070 6564 3e3d 323a 2043 6f62 6143 6f6e  pped>=2: CobaCon
-00013bd0: 7465 7874 2e6c 6f67 6765 722e 6c6f 6728  text.logger.log(
-00013be0: 6622 5765 2072 656d 6f76 6564 207b 6e5f  f"We removed {n_
-00013bf0: 6472 6f70 7065 647d 206c 6561 726e 6572  dropped} learner
-00013c00: 2065 7661 6c75 6174 696f 6e73 2062 6563   evaluations bec
-00013c10: 6175 7365 2074 6865 7920 7765 7265 2073  ause they were s
-00013c20: 686f 7274 6572 2074 6861 6e20 7b6e 7d20  horter than {n} 
-00013c30: 696e 7465 7261 6374 696f 6e73 2e22 290a  interactions.").
-00013c40: 0a20 2020 2020 2020 2065 6e76 5f6c 656e  .        env_len
-00013c50: 6774 6873 203d 2063 6f6c 6c65 6374 696f  gths = collectio
-00013c60: 6e73 2e43 6f75 6e74 6572 2865 6e76 5f6c  ns.Counter(env_l
-00013c70: 656e 6774 6873 290a 2020 2020 2020 2020  engths).        
-00013c80: 7368 6f72 7465 6e5f 746f 203d 206d 696e  shorten_to = min
-00013c90: 2865 6e76 5f6c 656e 6774 6873 2920 6966  (env_lengths) if
-00013ca0: 206e 3d3d 276d 696e 2720 616e 6420 656e   n=='min' and en
-00013cb0: 765f 6c65 6e67 7468 7320 656c 7365 206e  v_lengths else n
-00013cc0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00013cd0: 656e 765f 6c65 6e67 7468 7329 203e 2031  env_lengths) > 1
-00013ce0: 206f 7220 656e 765f 6c65 6e67 7468 732e   or env_lengths.
-00013cf0: 7661 6c75 6573 2829 2021 3d20 7b73 686f  values() != {sho
-00013d00: 7274 656e 5f74 6f7d 3a0a 2020 2020 2020  rten_to}:.      
-00013d10: 2020 2020 2020 6e5f 7368 6f72 7465 6e65        n_shortene
-00013d20: 6420 3d20 7375 6d28 7620 666f 7220 6b2c  d = sum(v for k,
-00013d30: 7620 696e 2065 6e76 5f6c 656e 6774 6873  v in env_lengths
-00013d40: 2e69 7465 6d73 2829 2069 6620 6b20 3e20  .items() if k > 
-00013d50: 7368 6f72 7465 6e5f 746f 290a 2020 2020  shorten_to).    
-00013d60: 2020 2020 2020 2020 696e 7465 7261 6374          interact
-00013d70: 696f 6e73 203d 2069 6e74 6572 6163 7469  ions = interacti
-00013d80: 6f6e 732e 7768 6572 6528 696e 6465 783d  ons.where(index=
-00013d90: 7b27 3c3d 273a 7368 6f72 7465 6e5f 746f  {'<=':shorten_to
-00013da0: 7d29 2023 2e34 0a20 2020 2020 2020 2020  }) #.4.         
-00013db0: 2020 2069 6620 6e5f 7368 6f72 7465 6e65     if n_shortene
-00013dc0: 643d 3d31 3a20 436f 6261 436f 6e74 6578  d==1: CobaContex
-00013dd0: 742e 6c6f 6767 6572 2e6c 6f67 2866 2257  t.logger.log(f"W
-00013de0: 6520 7368 6f72 7465 6e65 6420 7b6e 5f73  e shortened {n_s
-00013df0: 686f 7274 656e 6564 7d20 6c65 6172 6e65  hortened} learne
-00013e00: 7220 6576 616c 7561 7469 6f6e 2062 6563  r evaluation bec
-00013e10: 6175 7365 2069 7420 7761 7320 6c6f 6e67  ause it was long
-00013e20: 6572 2074 6861 6e20 7468 6520 7368 6f72  er than the shor
-00013e30: 7465 7374 2065 6e76 6972 6f6e 6d65 6e74  test environment
-00013e40: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-00013e50: 6966 206e 5f73 686f 7274 656e 6564 3e3d  if n_shortened>=
-00013e60: 323a 2043 6f62 6143 6f6e 7465 7874 2e6c  2: CobaContext.l
-00013e70: 6f67 6765 722e 6c6f 6728 6622 5765 2073  ogger.log(f"We s
-00013e80: 686f 7274 656e 6564 207b 6e5f 7368 6f72  hortened {n_shor
-00013e90: 7465 6e65 647d 206c 6561 726e 6572 2065  tened} learner e
-00013ea0: 7661 6c75 6174 696f 6e73 2062 6563 6175  valuations becau
-00013eb0: 7365 2074 6865 7920 7765 7265 206c 6f6e  se they were lon
-00013ec0: 6765 7220 7468 616e 2074 6865 2073 686f  ger than the sho
-00013ed0: 7274 6573 7420 656e 7669 726f 6e6d 656e  rtest environmen
-00013ee0: 742e 2229 0a0a 2020 2020 2020 2020 6b65  t.")..        ke
-00013ef0: 6570 5f65 6e76 732c 6b65 6570 5f6c 726e  ep_envs,keep_lrn
-00013f00: 732c 6b65 6570 5f76 616c 7320 3d20 6d61  s,keep_vals = ma
-00013f10: 7028 7365 742c 7a69 7028 2a74 6f5f 6b65  p(set,zip(*to_ke
-00013f20: 6570 2929 2069 6620 746f 5f6b 6565 7020  ep)) if to_keep 
-00013f30: 656c 7365 2028 5b5d 2c5b 5d2c 5b5d 290a  else ([],[],[]).
-00013f40: 0a20 2020 2020 2020 2069 6620 746f 5f64  .        if to_d
-00013f50: 726f 7020 616e 6420 6c65 6e28 6b65 6570  rop and len(keep
-00013f60: 5f65 6e76 7329 2021 3d20 6c65 6e28 656e  _envs) != len(en
-00013f70: 7669 726f 6e6d 656e 7473 293a 0a20 2020  vironments):.   
-00013f80: 2020 2020 2020 2020 2065 6e76 6972 6f6e           environ
-00013f90: 6d65 6e74 7320 3d20 656e 7669 726f 6e6d  ments = environm
-00013fa0: 656e 7473 2e77 6865 7265 2865 6e76 6972  ents.where(envir
-00013fb0: 6f6e 6d65 6e74 5f69 643d 6b65 6570 5f65  onment_id=keep_e
-00013fc0: 6e76 7329 0a0a 2020 2020 2020 2020 6966  nvs)..        if
-00013fd0: 2074 6f5f 6472 6f70 2061 6e64 206c 656e   to_drop and len
-00013fe0: 286b 6565 705f 6c72 6e73 2920 213d 206c  (keep_lrns) != l
-00013ff0: 656e 286c 6561 726e 6572 7329 3a0a 2020  en(learners):.  
-00014000: 2020 2020 2020 2020 2020 6c65 6172 6e65            learne
-00014010: 7273 203d 206c 6561 726e 6572 732e 7768  rs = learners.wh
-00014020: 6572 6528 6c65 6172 6e65 725f 6964 3d6b  ere(learner_id=k
-00014030: 6565 705f 6c72 6e73 290a 0a20 2020 2020  eep_lrns)..     
-00014040: 2020 2069 6620 746f 5f64 726f 7020 616e     if to_drop an
-00014050: 6420 6c65 6e28 6b65 6570 5f76 616c 7329  d len(keep_vals)
-00014060: 2021 3d20 6c65 6e28 6576 616c 7561 746f   != len(evaluato
-00014070: 7273 293a 0a20 2020 2020 2020 2020 2020  rs):.           
-00014080: 2065 7661 6c75 6174 6f72 7320 3d20 6576   evaluators = ev
-00014090: 616c 7561 746f 7273 2e77 6865 7265 2865  aluators.where(e
-000140a0: 7661 6c75 6174 6f72 5f69 643d 6b65 6570  valuator_id=keep
-000140b0: 5f76 616c 7329 0a0a 2020 2020 2020 2020  _vals)..        
-000140c0: 7265 7475 726e 2052 6573 756c 7428 656e  return Result(en
-000140d0: 7669 726f 6e6d 656e 7473 2c20 6c65 6172  vironments, lear
-000140e0: 6e65 7273 2c20 6576 616c 7561 746f 7273  ners, evaluators
-000140f0: 2c20 696e 7465 7261 6374 696f 6e73 2c20  , interactions, 
-00014100: 7365 6c66 2e65 7870 6572 696d 656e 7429  self.experiment)
-00014110: 0a0a 2020 2020 6465 6620 5f67 726f 7570  ..    def _group
-00014120: 5f70 2873 656c 662c 206c 3a55 6e69 6f6e  _p(self, l:Union
-00014130: 5b73 7472 2c20 5365 7175 656e 6365 5b73  [str, Sequence[s
-00014140: 7472 5d5d 2c20 703a 556e 696f 6e5b 7374  tr]], p:Union[st
-00014150: 722c 2053 6571 7565 6e63 655b 7374 725d  r, Sequence[str]
-00014160: 5d29 3a0a 0a20 2020 2020 2020 2065 6e76  ]):..        env
-00014170: 6972 6f6e 6d65 6e74 7320 3d20 7365 6c66  ironments = self
-00014180: 2e65 6e76 6972 6f6e 6d65 6e74 730a 2020  .environments.  
-00014190: 2020 2020 2020 6c65 6172 6e65 7273 2020        learners  
-000141a0: 2020 203d 2073 656c 662e 6c65 6172 6e65     = self.learne
-000141b0: 7273 0a20 2020 2020 2020 2065 7661 6c75  rs.        evalu
-000141c0: 6174 6f72 7320 2020 3d20 7365 6c66 2e65  ators   = self.e
-000141d0: 7661 6c75 6174 6f72 730a 2020 2020 2020  valuators.      
-000141e0: 2020 696e 7465 7261 6374 696f 6e73 203d    interactions =
-000141f0: 2073 656c 662e 696e 7465 7261 6374 696f   self.interactio
-00014200: 6e73 0a0a 2020 2020 2020 2020 696e 6465  ns..        inde
-00014210: 7865 7320 203d 206c 6973 7428 7365 6c66  xes  = list(self
-00014220: 2e5f 6772 6f75 7065 645f 7973 2870 2c6c  ._grouped_ys(p,l
-00014230: 2c27 656e 7669 726f 6e6d 656e 745f 6964  ,'environment_id
-00014240: 272c 276c 6561 726e 6572 5f69 6427 2c27  ','learner_id','
-00014250: 6576 616c 7561 746f 725f 6964 272c 793d  evaluator_id',y=
-00014260: 4e6f 6e65 2c63 6172 643d 2753 2729 290a  None,card='S')).
-00014270: 2020 2020 2020 2020 6e5f 6c65 7665 6c73          n_levels
-00014280: 203d 206c 656e 2873 6574 286d 6170 2869   = len(set(map(i
-00014290: 7465 6d67 6574 7465 7228 3129 2c69 6e64  temgetter(1),ind
-000142a0: 6578 6573 2929 290a 0a20 2020 2020 2020  exes)))..       
-000142b0: 2074 6f5f 6b65 6570 2c20 746f 5f72 656d   to_keep, to_rem
-000142c0: 6f76 652c 206e 5f6c 6172 6765 722c 206e  ove, n_larger, n
-000142d0: 5f73 6d61 6c6c 6572 203d 205b 5d2c 205b  _smaller = [], [
-000142e0: 5d2c 2030 2c20 300a 2020 2020 2020 2020  ], 0, 0.        
-000142f0: 666f 7220 5f2c 2067 726f 7570 2069 6e20  for _, group in 
-00014300: 6772 6f75 7062 7928 696e 6465 7865 732c  groupby(indexes,
-00014310: 6b65 793d 6974 656d 6765 7474 6572 2830  key=itemgetter(0
-00014320: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00014330: 6772 6f75 7020 3d20 6c69 7374 2867 726f  group = list(gro
-00014340: 7570 290a 2020 2020 2020 2020 2020 2020  up).            
-00014350: 6966 206c 656e 2867 726f 7570 2920 3e20  if len(group) > 
-00014360: 6e5f 6c65 7665 6c73 3a0a 2020 2020 2020  n_levels:.      
-00014370: 2020 2020 2020 2020 2020 6e5f 6c61 7267            n_larg
-00014380: 6572 202b 3d20 310a 2020 2020 2020 2020  er += 1.        
-00014390: 2020 2020 2020 2020 746f 5f72 656d 6f76          to_remov
-000143a0: 652e 6578 7465 6e64 2867 5b32 3a35 5d20  e.extend(g[2:5] 
-000143b0: 666f 7220 6720 696e 2067 726f 7570 290a  for g in group).
-000143c0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000143d0: 206c 656e 2867 726f 7570 2920 3c20 6e5f   len(group) < n_
-000143e0: 6c65 7665 6c73 3a0a 2020 2020 2020 2020  levels:.        
-000143f0: 2020 2020 2020 2020 6e5f 736d 616c 6c65          n_smalle
-00014400: 7220 2b3d 2031 0a20 2020 2020 2020 2020  r += 1.         
-00014410: 2020 2020 2020 2074 6f5f 7265 6d6f 7665         to_remove
-00014420: 2e65 7874 656e 6428 675b 323a 355d 2066  .extend(g[2:5] f
-00014430: 6f72 2067 2069 6e20 6772 6f75 7029 0a20  or g in group). 
-00014440: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00014450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014460: 2074 6f5f 6b65 6570 2e65 7874 656e 6428   to_keep.extend(
-00014470: 675b 323a 355d 2066 6f72 2067 2069 6e20  g[2:5] for g in 
-00014480: 6772 6f75 7029 0a0a 2020 2020 2020 2020  group)..        
-00014490: 6966 206e 5f6c 6172 6765 723a 0a20 2020  if n_larger:.   
-000144a0: 2020 2020 2020 2020 2043 6f62 6143 6f6e           CobaCon
-000144b0: 7465 7874 2e6c 6f67 6765 722e 6c6f 6728  text.logger.log(
-000144c0: 6622 5765 2072 656d 6f76 6564 207b 6e5f  f"We removed {n_
-000144d0: 6c61 7267 6572 7d20 7b70 7d20 6265 6361  larger} {p} beca
-000144e0: 7573 6520 6d6f 7265 2074 6861 6e20 6f6e  use more than on
-000144f0: 6520 6578 6973 7465 6420 666f 7220 6561  e existed for ea
-00014500: 6368 207b 6c7d 2e22 290a 0a20 2020 2020  ch {l}.")..     
-00014510: 2020 2069 6620 6e5f 736d 616c 6c65 723a     if n_smaller:
-00014520: 0a20 2020 2020 2020 2020 2020 2043 6f62  .            Cob
-00014530: 6143 6f6e 7465 7874 2e6c 6f67 6765 722e  aContext.logger.
-00014540: 6c6f 6728 6622 5765 2072 656d 6f76 6564  log(f"We removed
-00014550: 207b 6e5f 736d 616c 6c65 727d 207b 707d   {n_smaller} {p}
-00014560: 2062 6563 6175 7365 207b 2774 6865 7927   because {'they'
-00014570: 2069 6620 6e5f 736d 616c 6c65 723e 3120   if n_smaller>1 
-00014580: 656c 7365 2027 6974 277d 2064 6964 206e  else 'it'} did n
-00014590: 6f74 2065 7869 7374 2066 6f72 2065 7665  ot exist for eve
-000145a0: 7279 207b 6c7d 2e22 290a 0a20 2020 2020  ry {l}.")..     
-000145b0: 2020 2069 6620 746f 5f72 656d 6f76 653a     if to_remove:
-000145c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000145d0: 6563 7420 3d20 7365 6c66 2e5f 7265 6d6f  ect = self._remo
-000145e0: 7665 2874 6f5f 7265 6d6f 7665 290a 2020  ve(to_remove).  
-000145f0: 2020 2020 2020 2020 2020 696e 7465 7261            intera
-00014600: 6374 696f 6e73 203d 2054 6162 6c65 2856  ctions = Table(V
-00014610: 6965 7728 696e 7465 7261 6374 696f 6e73  iew(interactions
-00014620: 2e5f 6461 7461 2c73 656c 6563 7429 2c20  ._data,select), 
-00014630: 696e 7465 7261 6374 696f 6e73 2e63 6f6c  interactions.col
-00014640: 756d 6e73 2c20 696e 7465 7261 6374 696f  umns, interactio
-00014650: 6e73 2e69 6e64 6578 6573 290a 0a20 2020  ns.indexes)..   
-00014660: 2020 2020 2065 5f6b 6565 702c 6c5f 6b65       e_keep,l_ke
-00014670: 6570 2c76 5f6b 6565 7020 3d20 6d61 7028  ep,v_keep = map(
-00014680: 7365 742c 7a69 7028 2a74 6f5f 6b65 6570  set,zip(*to_keep
-00014690: 2929 2069 6620 746f 5f6b 6565 7020 656c  )) if to_keep el
-000146a0: 7365 2028 5b5d 2c5b 5d2c 5b5d 290a 2020  se ([],[],[]).  
-000146b0: 2020 2020 2020 6966 206c 656e 2865 5f6b        if len(e_k
-000146c0: 6565 7029 2021 3d20 6c65 6e28 656e 7669  eep) != len(envi
-000146d0: 726f 6e6d 656e 7473 293a 2065 6e76 6972  ronments): envir
-000146e0: 6f6e 6d65 6e74 7320 3d20 656e 7669 726f  onments = enviro
-000146f0: 6e6d 656e 7473 2e77 6865 7265 2865 6e76  nments.where(env
-00014700: 6972 6f6e 6d65 6e74 5f69 643d 655f 6b65  ironment_id=e_ke
-00014710: 6570 290a 2020 2020 2020 2020 6966 206c  ep).        if l
-00014720: 656e 286c 5f6b 6565 7029 2021 3d20 6c65  en(l_keep) != le
-00014730: 6e28 6c65 6172 6e65 7273 2920 2020 203a  n(learners)    :
-00014740: 206c 6561 726e 6572 7320 2020 2020 3d20   learners     = 
-00014750: 6c65 6172 6e65 7273 2020 2020 2e77 6865  learners    .whe
-00014760: 7265 286c 6561 726e 6572 5f69 6420 2020  re(learner_id   
-00014770: 203d 6c5f 6b65 6570 290a 2020 2020 2020   =l_keep).      
-00014780: 2020 6966 206c 656e 2876 5f6b 6565 7029    if len(v_keep)
-00014790: 2021 3d20 6c65 6e28 6576 616c 7561 746f   != len(evaluato
-000147a0: 7273 2920 203a 2065 7661 6c75 6174 6f72  rs)  : evaluator
-000147b0: 7320 2020 3d20 6576 616c 7561 746f 7273  s   = evaluators
-000147c0: 2020 2e77 6865 7265 2865 7661 6c75 6174    .where(evaluat
-000147d0: 6f72 5f69 6420 203d 765f 6b65 6570 290a  or_id  =v_keep).
-000147e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000147f0: 5265 7375 6c74 2865 6e76 6972 6f6e 6d65  Result(environme
-00014800: 6e74 732c 206c 6561 726e 6572 732c 2065  nts, learners, e
-00014810: 7661 6c75 6174 6f72 732c 2069 6e74 6572  valuators, inter
-00014820: 6163 7469 6f6e 732c 2073 656c 662e 6578  actions, self.ex
-00014830: 7065 7269 6d65 6e74 290a 0a20 2020 2064  periment)..    d
-00014840: 6566 205f 6669 6c74 6572 5f66 696e 2873  ef _filter_fin(s
-00014850: 656c 662c 0a20 2020 2020 2020 206e 3a20  elf,.        n: 
-00014860: 556e 696f 6e5b 696e 742c 4c69 7465 7261  Union[int,Litera
-00014870: 6c5b 276d 696e 275d 2c20 4e6f 6e65 5d2c  l['min'], None],
-00014880: 0a20 2020 2020 2020 206c 3a20 556e 696f  .        l: Unio
-00014890: 6e5b 7374 722c 2053 6571 7565 6e63 655b  n[str, Sequence[
-000148a0: 7374 725d 2c20 4e6f 6e65 5d2c 0a20 2020  str], None],.   
-000148b0: 2020 2020 2070 3a20 556e 696f 6e5b 7374       p: Union[st
-000148c0: 722c 2053 6571 7565 6e63 655b 7374 725d  r, Sequence[str]
-000148d0: 2c20 4e6f 6e65 5d29 202d 3e20 2752 6573  , None]) -> 'Res
-000148e0: 756c 7427 3a0a 2020 2020 2020 2020 2222  ult':.        ""
-000148f0: 2246 696c 7465 7220 7468 6520 7265 7375  "Filter the resu
-00014900: 6c74 7320 646f 776e 2074 6f20 6576 656e  lts down to even
-00014910: 206f 7574 636f 6d65 7320 736f 2074 6861   outcomes so tha
-00014920: 7420 706c 6f74 7465 6420 7265 7375 6c74  t plotted result
-00014930: 7320 7769 6c6c 2062 6520 6d65 616e 696e  s will be meanin
-00014940: 6766 756c 2e0a 0a20 2020 2020 2020 2041  gful...        A
-00014950: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00014960: 206e 3a20 5468 6520 6e75 6d62 6572 206f   n: The number o
-00014970: 6620 696e 7465 7261 6374 696f 6e73 2061  f interactions a
-00014980: 2073 7065 6369 6669 6320 6576 616c 7561   specific evalua
-00014990: 7469 6f6e 206d 7573 7420 6861 7665 2028  tion must have (
-000149a0: 4e6f 6e65 2069 6e64 6963 6174 6573 206e  None indicates n
-000149b0: 6f20 636f 6e73 7472 6169 6e74 292e 0a20  o constraint).. 
-000149c0: 2020 2020 2020 2020 2020 206c 3a20 5468             l: Th
-000149d0: 6520 6c65 7665 6c20 6174 2077 6869 6368  e level at which
-000149e0: 2077 6520 7769 7368 2074 6f20 636f 6d70   we wish to comp
-000149f0: 6172 6520 6576 616c 6174 696f 6e20 6f75  are evalation ou
-00014a00: 7463 6f6d 6573 2e0a 2020 2020 2020 2020  tcomes..        
-00014a10: 2020 2020 703a 2054 6865 2070 6169 7273      p: The pairs
-00014a20: 2074 6861 7420 6d75 7374 2065 7869 7374   that must exist
-00014a30: 2061 6372 6f73 7320 616c 6c20 636f 6d70   across all comp
-00014a40: 6172 6973 6f6e 206c 6576 656c 7320 696e  arison levels in
-00014a50: 206f 7264 6572 2074 6f20 6265 2069 6e63   order to be inc
-00014a60: 6c75 6465 642e 0a20 2020 2020 2020 2022  luded..        "
-00014a70: 2222 0a0a 2020 2020 2020 2020 7265 7375  ""..        resu
-00014a80: 6c74 203d 2073 656c 662e 636f 7079 2829  lt = self.copy()
-00014a90: 0a20 2020 2020 2020 2069 6620 6c20 6f72  .        if l or
-00014aa0: 2070 3a20 7265 7375 6c74 203d 2072 6573   p: result = res
-00014ab0: 756c 742e 5f67 726f 7570 5f70 286c 2c70  ult._group_p(l,p
-00014ac0: 290a 2020 2020 2020 2020 6966 206e 2020  ).        if n  
-00014ad0: 2020 203a 2072 6573 756c 7420 3d20 7265     : result = re
-00014ae0: 7375 6c74 2e5f 676c 6f62 616c 5f6e 286e  sult._global_n(n
-00014af0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00014b00: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-00014b10: 205f 7265 6d6f 7665 2873 656c 662c 2069   _remove(self, i
-00014b20: 6473 3a20 5365 7175 656e 6365 5b54 7570  ds: Sequence[Tup
-00014b30: 6c65 5b69 6e74 2c69 6e74 2c69 6e74 5d5d  le[int,int,int]]
-00014b40: 2c20 6e3d 3029 202d 3e20 5365 7175 656e  , n=0) -> Sequen
-00014b50: 6365 5b69 6e74 5d3a 0a20 2020 2020 2020  ce[int]:.       
-00014b60: 2023 7468 6973 2069 7320 6d75 6368 2066   #this is much f
-00014b70: 6173 7465 7220 7468 616e 2061 6e79 2062  aster than any b
-00014b80: 7569 6c74 2069 6e20 5461 626c 6520 6d65  uilt in Table me
-00014b90: 7468 6f64 730a 2020 2020 2020 2020 2374  thods.        #t
-00014ba0: 6f20 776f 726b 2069 6e74 6572 6163 7469  o work interacti
-00014bb0: 6f6e 7320 6d75 7374 2062 6520 736f 7274  ons must be sort
-00014bc0: 6564 2062 7920 656e 765f 6964 2c6c 726e  ed by env_id,lrn
-00014bd0: 5f69 642c 7661 6c5f 6964 0a20 2020 2020  _id,val_id.     
-00014be0: 2020 206c 6f63 2020 2020 2020 2020 2020     loc          
-00014bf0: 2020 3d20 300a 2020 2020 2020 2020 7365    = 0.        se
-00014c00: 6c65 6374 2020 2020 2020 2020 203d 205b  lect         = [
-00014c10: 5d0a 2020 2020 2020 2020 6e5f 696e 7465  ].        n_inte
-00014c20: 7261 6374 696f 6e73 203d 206c 656e 2873  ractions = len(s
-00014c30: 656c 662e 696e 7465 7261 6374 696f 6e73  elf.interactions
-00014c40: 290a 2020 2020 2020 2020 656e 765f 6964  ).        env_id
-00014c50: 732c 6c72 6e5f 6964 732c 7661 6c5f 6964  s,lrn_ids,val_id
-00014c60: 7320 3d20 7365 6c66 2e69 6e74 6572 6163  s = self.interac
-00014c70: 7469 6f6e 735b 5b27 656e 7669 726f 6e6d  tions[['environm
-00014c80: 656e 745f 6964 272c 276c 6561 726e 6572  ent_id','learner
-00014c90: 5f69 6427 2c27 6576 616c 7561 746f 725f  _id','evaluator_
-00014ca0: 6964 275d 5d0a 2020 2020 2020 2020 6964  id']].        id
-00014cb0: 7320 3d20 736f 7274 6564 2869 6473 290a  s = sorted(ids).
-00014cc0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00014cd0: 2072 616e 6765 286c 656e 2869 6473 2929   range(len(ids))
-00014ce0: 3a0a 2020 2020 2020 2020 2020 2020 652c  :.            e,
-00014cf0: 6c2c 7620 3d20 6964 735b 695d 0a20 2020  l,v = ids[i].   
-00014d00: 2020 2020 2020 2020 206c 6f31 203d 206d           lo1 = m
-00014d10: 795f 6269 7365 6374 5f6c 6566 7420 2865  y_bisect_left (e
-00014d20: 6e76 5f69 6473 2c65 2c6c 6f63 2c6e 5f69  nv_ids,e,loc,n_i
-00014d30: 6e74 6572 6163 7469 6f6e 7329 0a20 2020  nteractions).   
-00014d40: 2020 2020 2020 2020 2068 6931 203d 206d           hi1 = m
-00014d50: 795f 6269 7365 6374 5f72 6967 6874 2865  y_bisect_right(e
-00014d60: 6e76 5f69 6473 2c65 2c6c 6f63 2c6e 5f69  nv_ids,e,loc,n_i
-00014d70: 6e74 6572 6163 7469 6f6e 7329 0a20 2020  nteractions).   
-00014d80: 2020 2020 2020 2020 2069 6620 6c6f 313d           if lo1=
-00014d90: 3d68 6931 3a20 636f 6e74 696e 7565 2023  =hi1: continue #
-00014da0: 7468 6520 6769 7665 6e20 6964 7320 6172  the given ids ar
-00014db0: 656e 2774 2069 6e20 696e 7465 7261 6374  en't in interact
-00014dc0: 696f 6e73 0a20 2020 2020 2020 2020 2020  ions.           
-00014dd0: 206c 6f32 203d 206d 795f 6269 7365 6374   lo2 = my_bisect
-00014de0: 5f6c 6566 7420 286c 726e 5f69 6473 2c6c  _left (lrn_ids,l
-00014df0: 2c6c 6f31 2c68 6931 290a 2020 2020 2020  ,lo1,hi1).      
-00014e00: 2020 2020 2020 6869 3220 3d20 6d79 5f62        hi2 = my_b
-00014e10: 6973 6563 745f 7269 6768 7428 6c72 6e5f  isect_right(lrn_
-00014e20: 6964 732c 6c2c 6c6f 312c 6869 3129 0a20  ids,l,lo1,hi1). 
-00014e30: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
-00014e40: 323d 3d68 6932 3a20 636f 6e74 696e 7565  2==hi2: continue
-00014e50: 0a20 2020 2020 2020 2020 2020 206c 6f33  .            lo3
-00014e60: 203d 206d 795f 6269 7365 6374 5f6c 6566   = my_bisect_lef
-00014e70: 7420 2876 616c 5f69 6473 2c76 2c6c 6f32  t (val_ids,v,lo2
-00014e80: 2c68 6932 290a 2020 2020 2020 2020 2020  ,hi2).          
-00014e90: 2020 6869 3320 3d20 6d79 5f62 6973 6563    hi3 = my_bisec
-00014ea0: 745f 7269 6768 7428 7661 6c5f 6964 732c  t_right(val_ids,
-00014eb0: 762c 6c6f 322c 6869 3229 0a20 2020 2020  v,lo2,hi2).     
-00014ec0: 2020 2020 2020 2069 6620 6c6f 333d 3d68         if lo3==h
-00014ed0: 6933 3a20 636f 6e74 696e 7565 0a20 2020  i3: continue.   
-00014ee0: 2020 2020 2020 2020 2073 656c 6563 742e           select.
-00014ef0: 6578 7465 6e64 2872 616e 6765 286c 6f63  extend(range(loc
-00014f00: 2c6c 6f33 2b28 6e20 6966 2068 6933 2d6c  ,lo3+(n if hi3-l
-00014f10: 6f33 3e6e 2065 6c73 6520 3029 2929 0a20  o3>n else 0))). 
-00014f20: 2020 2020 2020 2020 2020 206c 6f63 203d             loc =
-00014f30: 2068 6933 0a0a 2020 2020 2020 2020 7365   hi3..        se
-00014f40: 6c65 6374 2e65 7874 656e 6428 7261 6e67  lect.extend(rang
-00014f50: 6528 6c6f 632c 6e5f 696e 7465 7261 6374  e(loc,n_interact
-00014f60: 696f 6e73 2929 0a20 2020 2020 2020 2072  ions)).        r
-00014f70: 6574 7572 6e20 7365 6c65 6374 0a         eturn select.
+00011340: 6c32 5f6c 656e 203d 206c 656e 2873 7472  l2_len = len(str
+00011350: 286c 325b 305d 2929 0a20 2020 2020 2020  (l2[0])).       
+00011360: 2020 2020 2020 2020 2020 2020 206c 3120               l1 
+00011370: 3d20 6c69 7374 286d 6170 2873 7472 2c6c  = list(map(str,l
+00011380: 3129 290a 2020 2020 2020 2020 2020 2020  1)).            
+00011390: 2020 2020 2020 2020 585f 595f 5945 203d          X_Y_YE =
+000113a0: 2073 6f72 7465 6428 585f 595f 5945 2c20   sorted(X_Y_YE, 
+000113b0: 6b65 793d 6c61 6d62 6461 2069 7465 6d73  key=lambda items
+000113c0: 3a20 6c31 2e69 6e64 6578 2869 7465 6d73  : l1.index(items
+000113d0: 5b30 5d5b 6c32 5f6c 656e 2b31 3a5d 2929  [0][l2_len+1:]))
+000113e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000113f0: 2065 6c69 6620 6c65 6e28 6c32 2920 3e20   elif len(l2) > 
+00011400: 3120 616e 6420 6c65 6e28 6c31 2920 3d3d  1 and len(l1) ==
+00011410: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00011420: 2020 2020 2020 2020 2353 6f72 7420 6279          #Sort by
+00011430: 206c 322e 2057 6520 6173 7375 6d65 205f   l2. We assume _
+00011440: 7820 6973 2066 227b 6c32 7d2d 7b6c 317d  x is f"{l2}-{l1}
+00011450: 222e 0a20 2020 2020 2020 2020 2020 2020  "..             
+00011460: 2020 2020 2020 206c 315f 6c65 6e20 3d20         l1_len = 
+00011470: 6c65 6e28 7374 7228 6c31 5b30 5d29 290a  len(str(l1[0])).
+00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011490: 2020 2020 6c32 203d 206c 6973 7428 6d61      l2 = list(ma
+000114a0: 7028 7374 722c 6c32 2929 0a20 2020 2020  p(str,l2)).     
+000114b0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+000114c0: 5f59 5f59 4520 3d20 736f 7274 6564 2858  _Y_YE = sorted(X
+000114d0: 5f59 5f59 452c 206b 6579 3d6c 616d 6264  _Y_YE, key=lambd
+000114e0: 6120 6974 656d 733a 206c 322e 696e 6465  a items: l2.inde
+000114f0: 7828 6974 656d 735b 305d 5b3a 2d28 6c31  x(items[0][:-(l1
+00011500: 5f6c 656e 2b31 295d 2929 0a20 2020 2020  _len+1)])).     
+00011510: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00011520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011530: 2020 2020 2058 5f59 5f59 4520 3d20 736f       X_Y_YE = so
+00011540: 7274 6564 2858 5f59 5f59 4529 0a0a 2020  rted(X_Y_YE)..  
+00011550: 2020 2020 2020 2020 2020 2020 2020 582c                X,
+00011560: 592c 5945 203d 207a 6970 282a 585f 595f  Y,YE = zip(*X_Y_
+00011570: 5945 290a 2020 2020 2020 2020 2020 2020  YE).            
+00011580: 2020 2020 636f 6c6f 7220 203d 2073 656c      color  = sel
+00011590: 662e 5f67 6574 5f63 6f6c 6f72 2863 6f6c  f._get_color(col
+000115a0: 6f72 732c 2030 290a 2020 2020 2020 2020  ors, 0).        
+000115b0: 2020 2020 2020 2020 6c69 6e65 7320 203d          lines  =
+000115c0: 205b 506f 696e 7473 2858 2c20 592c 204e   [Points(X, Y, N
+000115d0: 6f6e 652c 2059 452c 2073 7479 6c65 3d73  one, YE, style=s
+000115e0: 7479 6c65 2c20 6c61 6265 6c3d 4e6f 6e65  tyle, label=None
+000115f0: 2c20 636f 6c6f 723d 636f 6c6f 722c 2061  , color=color, a
+00011600: 6c70 6861 3d61 6c70 6861 295d 0a0a 2020  lpha=alpha)]..  
+00011610: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011630: 7570 7065 7220 3d20 6c61 6d62 6461 2079  upper = lambda y
+00011640: 2c79 653a 2079 2b79 655b 315d 2069 6620  ,ye: y+ye[1] if 
+00011650: 6973 696e 7374 616e 6365 2879 652c 286c  isinstance(ye,(l
+00011660: 6973 742c 7475 706c 6529 2920 656c 7365  ist,tuple)) else
+00011670: 2079 2b79 650a 2020 2020 2020 2020 2020   y+ye.          
+00011680: 2020 2020 2020 6c6f 7765 7220 3d20 6c61        lower = la
+00011690: 6d62 6461 2079 2c79 653a 2079 2d79 655b  mbda y,ye: y-ye[
+000116a0: 305d 2069 6620 6973 696e 7374 616e 6365  0] if isinstance
+000116b0: 2879 652c 286c 6973 742c 7475 706c 6529  (ye,(list,tuple)
+000116c0: 2920 656c 7365 2079 2d79 650a 2020 2020  ) else y-ye.    
+000116d0: 2020 2020 2020 2020 2020 2020 7072 6570              prep
+000116e0: 2020 3d20 6c61 6d62 6461 205f 783a 2073    = lambda _x: s
+000116f0: 7472 285f 7829 2069 6620 6e6f 7420 786f  tr(_x) if not xo
+00011700: 7264 6572 2065 6c73 6520 5f78 0a0a 2020  rder else _x..  
+00011710: 2020 2020 2020 2020 2020 2020 2020 2373                #s
+00011720: 706c 6974 2069 6e74 6f20 7769 6e2c 7469  plit into win,ti
+00011730: 652c 6c6f 7373 0a20 2020 2020 2020 2020  e,loss.         
+00011740: 2020 2020 2020 206c 315f 7769 6e20 3d20         l1_win = 
+00011750: 5b28 7072 6570 2878 292c 792c 7965 2920  [(prep(x),y,ye) 
+00011760: 666f 7220 782c 792c 7965 2069 6e20 585f  for x,y,ye in X_
+00011770: 595f 5945 2069 6620 7570 7065 7228 792c  Y_YE if upper(y,
+00011780: 7965 2920 3c20 205f 626f 756e 6461 7279  ye) <  _boundary
+00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117a0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+000117b0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000117c0: 6f5f 7769 6e20 3d20 5b28 7072 6570 2878  o_win = [(prep(x
+000117d0: 292c 792c 7965 2920 666f 7220 782c 792c  ),y,ye) for x,y,
+000117e0: 7965 2069 6e20 585f 595f 5945 2069 6620  ye in X_Y_YE if 
+000117f0: 6c6f 7765 7228 792c 7965 2920 3c3d 205f  lower(y,ye) <= _
+00011800: 626f 756e 6461 7279 2061 6e64 205f 626f  boundary and _bo
+00011810: 756e 6461 7279 203c 3d20 7570 7065 7228  undary <= upper(
+00011820: 792c 7965 295d 0a20 2020 2020 2020 2020  y,ye)].         
+00011830: 2020 2020 2020 206c 325f 7769 6e20 3d20         l2_win = 
+00011840: 5b28 7072 6570 2878 292c 792c 7965 2920  [(prep(x),y,ye) 
+00011850: 666f 7220 782c 792c 7965 2069 6e20 585f  for x,y,ye in X_
+00011860: 595f 5945 2069 6620 2020 2020 2020 2020  Y_YE if         
+00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011880: 2020 2020 205f 626f 756e 6461 7279 203c       _boundary <
+00011890: 2020 6c6f 7765 7228 792c 7965 295d 0a0a    lower(y,ye)]..
+000118a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118b0: 2373 6f72 7420 6279 206f 7264 6572 206f  #sort by order o
+000118c0: 6620 6d61 676e 6974 7564 650a 2020 2020  f magnitude.    
+000118d0: 2020 2020 2020 2020 2020 2020 6c31 5f77              l1_w
+000118e0: 696e 203d 2073 6f72 7465 6428 6c31 5f77  in = sorted(l1_w
+000118f0: 696e 2c6b 6579 3d69 7465 6d67 6574 7465  in,key=itemgette
+00011900: 7228 3129 290a 2020 2020 2020 2020 2020  r(1)).          
+00011910: 2020 2020 2020 6e6f 5f77 696e 203d 2073        no_win = s
+00011920: 6f72 7465 6428 6e6f 5f77 696e 2c6b 6579  orted(no_win,key
+00011930: 3d69 7465 6d67 6574 7465 7228 3129 290a  =itemgetter(1)).
+00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011950: 6c32 5f77 696e 203d 2073 6f72 7465 6428  l2_win = sorted(
+00011960: 6c32 5f77 696e 2c6b 6579 3d69 7465 6d67  l2_win,key=itemg
+00011970: 6574 7465 7228 3129 290a 0a20 2020 2020  etter(1))..     
+00011980: 2020 2020 2020 2020 2020 206c 696e 6573             lines
+00011990: 203d 205b 5d0a 0a20 2020 2020 2020 2020   = []..         
+000119a0: 2020 2020 2020 2058 2c59 2c59 4520 3d20         X,Y,YE = 
+000119b0: 7a69 7028 2a6c 315f 7769 6e29 2069 6620  zip(*l1_win) if 
+000119c0: 6c31 5f77 696e 2065 6c73 6520 2828 292c  l1_win else ((),
+000119d0: 2829 2c4e 6f6e 6529 0a20 2020 2020 2020  (),None).       
+000119e0: 2020 2020 2020 2020 2063 6f6c 6f72 2020           color  
+000119f0: 3d20 7365 6c66 2e5f 6765 745f 636f 6c6f  = self._get_colo
+00011a00: 7228 636f 6c6f 7273 2c20 2020 2020 2020  r(colors,       
+00011a10: 2020 3029 0a20 2020 2020 2020 2020 2020    0).           
+00011a20: 2020 2020 206c 6162 656c 2020 3d20 7365       label  = se
+00011a30: 6c66 2e5f 6765 745f 6c61 6265 6c28 6c61  lf._get_label(la
+00011a40: 6265 6c73 2c6c 315f 6c61 6265 6c2c 3029  bels,l1_label,0)
+00011a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011a60: 206c 6162 656c 2020 3d20 6622 7b6c 6162   label  = f"{lab
+00011a70: 656c 7d20 287b 6c65 6e28 5829 7d29 2220  el} ({len(X)})" 
+00011a80: 6966 206c 6567 656e 6420 656c 7365 204e  if legend else N
+00011a90: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00011aa0: 2020 2020 6c69 6e65 732e 6170 7065 6e64      lines.append
+00011ab0: 2850 6f69 6e74 7328 582c 2059 2c20 4e6f  (Points(X, Y, No
+00011ac0: 6e65 2c20 5945 2c20 7374 796c 653d 7374  ne, YE, style=st
+00011ad0: 796c 652c 206c 6162 656c 3d6c 6162 656c  yle, label=label
+00011ae0: 2c20 636f 6c6f 723d 636f 6c6f 722c 2061  , color=color, a
+00011af0: 6c70 6861 3d61 6c70 6861 2929 0a0a 2020  lpha=alpha))..  
+00011b00: 2020 2020 2020 2020 2020 2020 2020 582c                X,
+00011b10: 592c 5945 203d 207a 6970 282a 6e6f 5f77  Y,YE = zip(*no_w
+00011b20: 696e 2920 6966 206e 6f5f 7769 6e20 656c  in) if no_win el
+00011b30: 7365 2028 2829 2c28 292c 4e6f 6e65 290a  se ((),(),None).
+00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b50: 636f 6c6f 7220 203d 2073 656c 662e 5f67  color  = self._g
+00011b60: 6574 5f63 6f6c 6f72 2863 6f6c 6f72 732c  et_color(colors,
+00011b70: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
+00011b80: 2020 2020 6c61 6265 6c20 203d 2027 5469      label  = 'Ti
+00011b90: 6527 0a20 2020 2020 2020 2020 2020 2020  e'.             
+00011ba0: 2020 206c 6162 656c 2020 3d20 6622 7b6c     label  = f"{l
+00011bb0: 6162 656c 7d20 287b 6c65 6e28 5829 7d29  abel} ({len(X)})
+00011bc0: 2220 6966 206c 6567 656e 6420 656c 7365  " if legend else
+00011bd0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00011be0: 2020 2020 2020 6c69 6e65 732e 6170 7065        lines.appe
+00011bf0: 6e64 2850 6f69 6e74 7328 582c 2059 2c20  nd(Points(X, Y, 
+00011c00: 4e6f 6e65 2c20 5945 2c20 7374 796c 653d  None, YE, style=
+00011c10: 7374 796c 652c 206c 6162 656c 3d6c 6162  style, label=lab
+00011c20: 656c 2c20 636f 6c6f 723d 636f 6c6f 722c  el, color=color,
+00011c30: 2061 6c70 6861 3d61 6c70 6861 2929 0a0a   alpha=alpha))..
+00011c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c50: 582c 592c 5945 203d 207a 6970 282a 6c32  X,Y,YE = zip(*l2
+00011c60: 5f77 696e 2920 6966 206c 325f 7769 6e20  _win) if l2_win 
+00011c70: 656c 7365 2028 2829 2c28 292c 4e6f 6e65  else ((),(),None
+00011c80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011c90: 2020 636f 6c6f 7220 203d 2073 656c 662e    color  = self.
+00011ca0: 5f67 6574 5f63 6f6c 6f72 2863 6f6c 6f72  _get_color(color
+00011cb0: 732c 2020 2020 2020 2020 2032 290a 2020  s,         2).  
+00011cc0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00011cd0: 6265 6c20 203d 2073 656c 662e 5f67 6574  bel  = self._get
+00011ce0: 5f6c 6162 656c 286c 6162 656c 732c 6c32  _label(labels,l2
+00011cf0: 5f6c 6162 656c 2c31 290a 2020 2020 2020  _label,1).      
+00011d00: 2020 2020 2020 2020 2020 6c61 6265 6c20            label 
+00011d10: 203d 2066 227b 6c61 6265 6c7d 2028 7b6c   = f"{label} ({l
+00011d20: 656e 2858 297d 2922 2069 6620 6c65 6765  en(X)})" if lege
+00011d30: 6e64 2065 6c73 6520 4e6f 6e65 0a20 2020  nd else None.   
+00011d40: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+00011d50: 6573 2e61 7070 656e 6428 506f 696e 7473  es.append(Points
+00011d60: 2858 2c20 592c 204e 6f6e 652c 2059 452c  (X, Y, None, YE,
+00011d70: 2073 7479 6c65 3d73 7479 6c65 2c20 6c61   style=style, la
+00011d80: 6265 6c3d 6c61 6265 6c2c 2063 6f6c 6f72  bel=label, color
+00011d90: 3d63 6f6c 6f72 2c20 616c 7068 613d 616c  =color, alpha=al
+00011da0: 7068 6129 290a 0a20 2020 2020 2020 2020  pha))..         
+00011db0: 2020 2078 726f 7461 7469 6f6e 203d 2039     xrotation = 9
+00011dc0: 3020 6966 2028 7820 213d 2027 696e 6465  0 if (x != 'inde
+00011dd0: 7827 206f 7220 786f 7264 6572 2920 616e  x' or xorder) an
+00011de0: 6420 6c65 6e28 585f 595f 5945 293e 3520  d len(X_Y_YE)>5 
+00011df0: 656c 7365 2030 0a20 2020 2020 2020 2020  else 0.         
+00011e00: 2020 2079 726f 7461 7469 6f6e 203d 2030     yrotation = 0
+00011e10: 0a0a 2020 2020 2020 2020 2020 2020 5f59  ..            _Y
+00011e20: 203d 2072 6177 5f64 6174 615b 7261 775f   = raw_data[raw_
+00011e30: 6461 7461 2e63 6f6c 756d 6e73 5b31 5d5d  data.columns[1]]
+00011e40: 5b30 5d0a 0a20 2020 2020 2020 2020 2020  [0]..           
+00011e50: 2078 6c61 6265 6c20 3d20 786c 6162 656c   xlabel = xlabel
+00011e60: 206f 7220 2822 496e 7465 7261 6374 696f   or ("Interactio
+00011e70: 6e22 2069 6620 783d 3d27 696e 6465 7827  n" if x=='index'
+00011e80: 2065 6c73 6520 785b 305d 2069 6620 6c65   else x[0] if le
+00011e90: 6e28 7829 203d 3d20 3120 656c 7365 2078  n(x) == 1 else x
+00011ea0: 290a 2020 2020 2020 2020 2020 2020 796c  ).            yl
+00011eb0: 6162 656c 203d 2079 6c61 6265 6c20 6f72  abel = ylabel or
+00011ec0: 2028 6622 245c 4465 6c74 6124 207b 797d   (f"$\Delta$ {y}
+00011ed0: 2220 6966 206d 6f64 653d 3d22 6469 6666  " if mode=="diff
+00011ee0: 2220 656c 7365 2066 2250 2824 5c44 656c  " else f"P($\Del
+00011ef0: 7461 2420 7b79 7d20 3e20 3029 2229 0a20  ta$ {y} > 0)"). 
+00011f00: 2020 2020 2020 2020 2020 2074 6974 6c65             title
+00011f10: 2020 3d20 7469 746c 6520 6966 2074 6974    = title if tit
+00011f20: 6c65 2069 7320 6e6f 7420 4e6f 6e65 2065  le is not None e
+00011f30: 6c73 6520 2866 227b 796c 6162 656c 7d20  lse (f"{ylabel} 
+00011f40: 287b 6c65 6e28 5f59 297d 2045 6e76 6972  ({len(_Y)} Envir
+00011f50: 6f6e 6d65 6e74 7329 2229 0a0a 2020 2020  onments)")..    
+00011f60: 2020 2020 2020 2020 616c 6c5f 7820 3d20          all_x = 
+00011f70: 6469 6374 2e66 726f 6d6b 6579 7328 6368  dict.fromkeys(ch
+00011f80: 6169 6e2e 6672 6f6d 5f69 7465 7261 626c  ain.from_iterabl
+00011f90: 6528 6c69 6e65 2e58 2066 6f72 206c 696e  e(line.X for lin
+00011fa0: 6520 696e 206c 696e 6573 2929 0a20 2020  e in lines)).   
+00011fb0: 2020 2020 2020 2020 2078 6f72 6465 7265           xordere
+00011fc0: 6420 3d20 6c69 7374 2861 6c6c 5f78 2e6b  d = list(all_x.k
+00011fd0: 6579 7328 2929 2069 6620 6e6f 7420 786f  eys()) if not xo
+00011fe0: 7264 6572 2065 6c73 6520 736f 7274 6564  rder else sorted
+00011ff0: 2861 6c6c 5f78 2c20 7265 7665 7273 653d  (all_x, reverse=
+00012000: 786f 7264 6572 3d3d 272d 2729 0a0a 2020  xorder=='-')..  
+00012010: 2020 2020 2020 2020 2020 6966 2062 6f75            if bou
+00012020: 6e64 6172 793a 0a20 2020 2020 2020 2020  ndary:.         
+00012030: 2020 2020 2020 206c 696e 6573 2e61 7070         lines.app
+00012040: 656e 6428 506f 696e 7473 2828 786f 7264  end(Points((xord
+00012050: 6572 6564 5b30 5d2c 786f 7264 6572 6564  ered[0],xordered
+00012060: 5b2d 315d 292c 285f 626f 756e 6461 7279  [-1]),(_boundary
+00012070: 2c5f 626f 756e 6461 7279 292c 204e 6f6e  ,_boundary), Non
+00012080: 652c 204e 6f6e 6520 2c20 2223 3838 3822  e, None , "#888"
+00012090: 2c20 312c 204e 6f6e 652c 2027 2d27 2c2e  , 1, None, '-',.
+000120a0: 3529 290a 0a20 2020 2020 2020 2020 2020  5))..           
+000120b0: 2069 6620 7820 3d3d 2027 696e 6465 7827   if x == 'index'
+000120c0: 2061 6e64 2078 6f72 6465 7220 696e 205b   and xorder in [
+000120d0: 272b 272c 4e6f 6e65 5d3a 0a20 2020 2020  '+',None]:.     
+000120e0: 2020 2020 2020 2020 2020 2078 6f72 6465             xorde
+000120f0: 7265 6420 3d20 4e6f 6e65 0a0a 2020 2020  red = None..    
+00012100: 2020 2020 2020 2020 7365 6c66 2e5f 706c          self._pl
+00012110: 6f74 7465 722e 706c 6f74 2861 782c 206c  otter.plot(ax, l
+00012120: 696e 6573 2c20 7469 746c 652c 2078 6c61  ines, title, xla
+00012130: 6265 6c2c 2079 6c61 6265 6c2c 2078 6c69  bel, ylabel, xli
+00012140: 6d2c 2079 6c69 6d2c 2078 7469 636b 732c  m, ylim, xticks,
+00012150: 2079 7469 636b 732c 206c 6567 656e 642c   yticks, legend,
+00012160: 2078 726f 7461 7469 6f6e 2c20 7972 6f74   xrotation, yrot
+00012170: 6174 696f 6e2c 2078 6f72 6465 7265 642c  ation, xordered,
+00012180: 206f 7574 290a 0a20 2020 2020 2020 2065   out)..        e
+00012190: 7863 6570 7420 436f 6261 4578 6365 7074  xcept CobaExcept
+000121a0: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
+000121b0: 2020 2020 2020 436f 6261 436f 6e74 6578        CobaContex
+000121c0: 742e 6c6f 6767 6572 2e6c 6f67 2873 7472  t.logger.log(str
+000121d0: 2865 2929 0a0a 2020 2020 6465 6620 5f5f  (e))..    def __
+000121e0: 7374 725f 5f28 7365 6c66 2920 2d3e 2073  str__(self) -> s
+000121f0: 7472 3a0a 2020 2020 2020 2020 7265 7475  tr:.        retu
+00012200: 726e 2073 7472 287b 224c 6561 726e 6572  rn str({"Learner
+00012210: 7322 3a20 6c65 6e28 7365 6c66 2e5f 6c65  s": len(self._le
+00012220: 6172 6e65 7273 292c 2022 456e 7669 726f  arners), "Enviro
+00012230: 6e6d 656e 7473 223a 206c 656e 2873 656c  nments": len(sel
+00012240: 662e 5f65 6e76 6972 6f6e 6d65 6e74 7329  f._environments)
+00012250: 2c20 2249 6e74 6572 6163 7469 6f6e 7322  , "Interactions"
+00012260: 3a20 6c65 6e28 7365 6c66 2e5f 696e 7465  : len(self._inte
+00012270: 7261 6374 696f 6e73 2920 7d29 0a0a 2020  ractions) })..  
+00012280: 2020 6465 6620 5f5f 6571 5f5f 2873 656c    def __eq__(sel
+00012290: 662c 206f 3a20 6f62 6a65 6374 2920 2d3e  f, o: object) ->
+000122a0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2072   bool:.        r
+000122b0: 6574 7572 6e20 6973 696e 7374 616e 6365  eturn isinstance
+000122c0: 286f 2c52 6573 756c 7429 205c 0a20 2020  (o,Result) \.   
+000122d0: 2020 2020 2020 2020 616e 6420 6f2e 656e          and o.en
+000122e0: 7669 726f 6e6d 656e 7473 203d 3d20 7365  vironments == se
+000122f0: 6c66 2e65 6e76 6972 6f6e 6d65 6e74 7320  lf.environments 
+00012300: 5c0a 2020 2020 2020 2020 2020 2061 6e64  \.           and
+00012310: 206f 2e6c 6561 726e 6572 7320 3d3d 2073   o.learners == s
+00012320: 656c 662e 6c65 6172 6e65 7273 205c 0a20  elf.learners \. 
+00012330: 2020 2020 2020 2020 2020 616e 6420 6f2e            and o.
+00012340: 6576 616c 7561 746f 7273 203d 3d20 7365  evaluators == se
+00012350: 6c66 2e65 7661 6c75 6174 6f72 730a 0a20  lf.evaluators.. 
+00012360: 2020 2064 6566 205f 6970 7974 686f 6e5f     def _ipython_
+00012370: 6469 7370 6c61 795f 2873 656c 6629 3a0a  display_(self):.
+00012380: 2020 2020 2020 2020 2370 7265 7474 7920          #pretty 
+00012390: 7072 696e 7420 696e 206a 7570 7974 6572  print in jupyter
+000123a0: 206e 6f74 6562 6f6f 6b20 2868 7474 7073   notebook (https
+000123b0: 3a2f 2f69 7079 7468 6f6e 2e72 6561 6474  ://ipython.readt
+000123c0: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
+000123d0: 626c 652f 636f 6e66 6967 2f69 6e74 6567  ble/config/integ
+000123e0: 7261 7469 6e67 2e68 746d 6c29 0a20 2020  rating.html).   
+000123f0: 2020 2020 2070 7269 6e74 2873 7472 2873       print(str(s
+00012400: 656c 6629 290a 0a20 2020 2064 6566 205f  elf))..    def _
+00012410: 6765 745f 636f 6c6f 7228 7365 6c66 2c20  get_color(self, 
+00012420: 636f 6c6f 7273 3a55 6e69 6f6e 5b4e 6f6e  colors:Union[Non
+00012430: 652c 5365 7175 656e 6365 5b55 6e69 6f6e  e,Sequence[Union
+00012440: 5b73 7472 2c69 6e74 5d5d 5d2c 2069 3a69  [str,int]]], i:i
+00012450: 6e74 2920 2d3e 2055 6e69 6f6e 5b73 7472  nt) -> Union[str
+00012460: 2c69 6e74 5d3a 0a20 2020 2020 2020 2074  ,int]:.        t
+00012470: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00012480: 7265 7475 726e 2063 6f6c 6f72 7320 6966  return colors if
+00012490: 2069 7369 6e73 7461 6e63 6528 636f 6c6f   isinstance(colo
+000124a0: 7273 2c73 7472 2920 656c 7365 2063 6f6c  rs,str) else col
+000124b0: 6f72 735b 695d 2069 6620 636f 6c6f 7273  ors[i] if colors
+000124c0: 2065 6c73 6520 690a 2020 2020 2020 2020   else i.        
+000124d0: 6578 6365 7074 2049 6e64 6578 4572 726f  except IndexErro
+000124e0: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+000124f0: 6574 7572 6e20 692b 6d61 7828 636f 6c6f  eturn i+max(colo
+00012500: 7273 2920 6966 2069 7369 6e73 7461 6e63  rs) if isinstanc
+00012510: 6528 636f 6c6f 7273 5b30 5d2c 2869 6e74  e(colors[0],(int
+00012520: 2c66 6c6f 6174 2929 2065 6c73 6520 690a  ,float)) else i.
+00012530: 2020 2020 2020 2020 6578 6365 7074 2054          except T
+00012540: 7970 6545 7272 6f72 3a0a 2020 2020 2020  ypeError:.      
+00012550: 2020 2020 2020 7265 7475 726e 2069 2b63        return i+c
+00012560: 6f6c 6f72 730a 0a20 2020 2064 6566 205f  olors..    def _
+00012570: 6765 745f 6c61 6265 6c28 7365 6c66 2c20  get_label(self, 
+00012580: 6c61 6265 6c73 3a53 6571 7565 6e63 655b  labels:Sequence[
+00012590: 7374 725d 2c20 6c61 6265 6c3a 7374 722c  str], label:str,
+000125a0: 2069 3a69 6e74 2920 2d3e 2073 7472 3a0a   i:int) -> str:.
+000125b0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000125c0: 2020 2020 2020 2020 206c 6162 656c 203d           label =
+000125d0: 206c 6162 656c 7320 6966 2069 7369 6e73   labels if isins
+000125e0: 7461 6e63 6528 6c61 6265 6c73 2c73 7472  tance(labels,str
+000125f0: 2920 656c 7365 206c 6162 656c 735b 695d  ) else labels[i]
+00012600: 2069 6620 6c61 6265 6c73 2065 6c73 6520   if labels else 
+00012610: 6c61 6265 6c0a 2020 2020 2020 2020 6578  label.        ex
+00012620: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+00012630: 2020 7061 7373 0a20 2020 2020 2020 2072    pass.        r
+00012640: 6574 7572 6e20 7374 7228 6c61 6265 6c29  eturn str(label)
+00012650: 0a0a 2020 2020 6465 6620 5f70 6c6f 7474  ..    def _plott
+00012660: 6162 6c65 2873 656c 662c 2078 3a53 6571  able(self, x:Seq
+00012670: 7565 6e63 655b 7374 725d 2c20 793a 7374  uence[str], y:st
+00012680: 7229 202d 3e20 2752 6573 756c 7427 3a0a  r) -> 'Result':.
+00012690: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000126a0: 6973 696e 7374 616e 6365 2878 2c73 7472  isinstance(x,str
+000126b0: 2920 616e 6420 2769 6e64 6578 2720 696e  ) and 'index' in
+000126c0: 2078 2061 6e64 206c 656e 2878 2920 3e20   x and len(x) > 
+000126d0: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
+000126e0: 6169 7365 2043 6f62 6145 7863 6570 7469  aise CobaExcepti
+000126f0: 6f6e 2827 5468 6520 782d 6178 6973 2063  on('The x-axis c
+00012700: 616e 6e6f 7420 636f 6e74 6169 6e20 626f  annot contain bo
+00012710: 7468 2069 6e64 6578 6573 2061 6e64 2070  th indexes and p
+00012720: 6172 616d 6574 6572 732e 2729 0a0a 2020  arameters.')..  
+00012730: 2020 2020 2020 6966 206c 656e 2873 656c        if len(sel
+00012740: 662e 696e 7465 7261 6374 696f 6e73 2920  f.interactions) 
+00012750: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00012760: 2020 7261 6973 6520 436f 6261 4578 6365    raise CobaExce
+00012770: 7074 696f 6e28 2254 6869 7320 7265 7375  ption("This resu
+00012780: 6c74 2064 6f65 7320 6e6f 7420 636f 6e74  lt does not cont
+00012790: 6169 6e20 616e 7920 6461 7461 2074 6f20  ain any data to 
+000127a0: 706c 6f74 2e22 290a 0a20 2020 2020 2020  plot.")..       
+000127b0: 2069 6620 7920 6e6f 7420 696e 2073 656c   if y not in sel
+000127c0: 662e 696e 7465 7261 6374 696f 6e73 2e63  f.interactions.c
+000127d0: 6f6c 756d 6e73 3a0a 2020 2020 2020 2020  olumns:.        
+000127e0: 2020 2020 7261 6973 6520 436f 6261 4578      raise CobaEx
+000127f0: 6365 7074 696f 6e28 6622 5468 6973 2072  ception(f"This r
+00012800: 6573 756c 7420 646f 6573 206e 6f74 2063  esult does not c
+00012810: 6f6e 7461 696e 2063 6f6c 756d 6e20 277b  ontain column '{
+00012820: 797d 2720 696e 2069 6e74 6572 6163 7469  y}' in interacti
+00012830: 6f6e 732e 2229 0a0a 2020 2020 2020 2020  ons.")..        
+00012840: 7265 7475 726e 2073 656c 660a 0a20 2020  return self..   
+00012850: 2064 6566 205f 6669 6e69 7368 6564 2873   def _finished(s
+00012860: 656c 662c 2078 3a53 6571 7565 6e63 655b  elf, x:Sequence[
+00012870: 7374 725d 2c20 793a 7374 722c 206c 3a53  str], y:str, l:S
+00012880: 6571 7565 6e63 655b 7374 725d 2c20 703a  equence[str], p:
+00012890: 5365 7175 656e 6365 5b73 7472 5d29 202d  Sequence[str]) -
+000128a0: 3e20 2752 6573 756c 7427 3a0a 2020 2020  > 'Result':.    
+000128b0: 2020 2020 6f6e 6c79 5f66 696e 6973 6865      only_finishe
+000128c0: 6420 3d20 7365 6c66 2e5f 6669 6c74 6572  d = self._filter
+000128d0: 5f66 696e 2827 6d69 6e27 2069 6620 7820  _fin('min' if x 
+000128e0: 3d3d 2027 696e 6465 7827 2065 6c73 6520  == 'index' else 
+000128f0: 4e6f 6e65 2c20 6c2c 2070 290a 2020 2020  None, l, p).    
+00012900: 2020 2020 6966 206c 656e 286f 6e6c 795f      if len(only_
+00012910: 6669 6e69 7368 6564 2e6c 6561 726e 6572  finished.learner
+00012920: 7329 203d 3d20 303a 0a20 2020 2020 2020  s) == 0:.       
+00012930: 2020 2020 2072 6169 7365 2043 6f62 6145       raise CobaE
+00012940: 7863 6570 7469 6f6e 2866 2254 6869 7320  xception(f"This 
+00012950: 7265 7375 6c74 2064 6f65 7320 6e6f 7420  result does not 
+00012960: 636f 6e74 6169 6e20 6120 7b70 7d20 7468  contain a {p} th
+00012970: 6174 2068 6173 2062 6565 6e20 6669 6e69  at has been fini
+00012980: 7368 6564 2066 6f72 2065 7665 7279 207b  shed for every {
+00012990: 6c7d 2e22 290a 2020 2020 2020 2020 7265  l}.").        re
+000129a0: 7475 726e 206f 6e6c 795f 6669 6e69 7368  turn only_finish
+000129b0: 6564 0a0a 2020 2020 6465 6620 5f63 6f6e  ed..    def _con
+000129c0: 6669 6465 6e63 6528 7365 6c66 2c20 6572  fidence(self, er
+000129d0: 723a 2055 6e69 6f6e 5b73 7472 2c50 6f69  r: Union[str,Poi
+000129e0: 6e74 416e 6449 6e74 6572 7661 6c5d 2c20  ntAndInterval], 
+000129f0: 6572 7265 7665 7279 3a69 6e74 203d 2031  errevery:int = 1
+00012a00: 293a 0a0a 2020 2020 2020 2020 6966 2065  ):..        if e
+00012a10: 7272 203d 3d20 2773 6527 3a0a 2020 2020  rr == 'se':.    
+00012a20: 2020 2020 2020 2020 6369 203d 2053 7464          ci = Std
+00012a30: 4572 7243 4928 2e39 3529 0a20 2020 2020  ErrCI(.95).     
+00012a40: 2020 2065 6c69 6620 6572 7220 3d3d 2027     elif err == '
+00012a50: 6273 273a 0a20 2020 2020 2020 2020 2020  bs':.           
+00012a60: 2063 6920 3d20 426f 6f74 7374 7261 7043   ci = BootstrapC
+00012a70: 4928 2e39 352c 206d 6561 6e29 0a20 2020  I(.95, mean).   
+00012a80: 2020 2020 2065 6c69 6620 6572 7220 3d3d       elif err ==
+00012a90: 2027 6269 273a 0a20 2020 2020 2020 2020   'bi':.         
+00012aa0: 2020 2063 6920 3d20 4269 6e6f 6d69 616c     ci = Binomial
+00012ab0: 4349 2827 7769 6c73 6f6e 2729 0a20 2020  CI('wilson').   
+00012ac0: 2020 2020 2065 6c69 6620 6572 7220 3d3d       elif err ==
+00012ad0: 2027 7364 273a 0a20 2020 2020 2020 2020   'sd':.         
+00012ae0: 2020 2063 6920 3d20 5374 6444 6576 4349     ci = StdDevCI
+00012af0: 2829 0a20 2020 2020 2020 2065 6c69 6620  ().        elif 
+00012b00: 6572 7220 6973 204e 6f6e 6520 6f72 2069  err is None or i
+00012b10: 7369 6e73 7461 6e63 6528 6572 722c 7374  sinstance(err,st
+00012b20: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00012b30: 6369 203d 204e 6f6e 650a 2020 2020 2020  ci = None.      
+00012b40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00012b50: 2020 2020 6369 203d 2065 7272 0a0a 2020      ci = err..  
+00012b60: 2020 2020 2020 6465 6620 6361 6c63 5f63        def calc_c
+00012b70: 6928 5a3a 5365 7175 656e 6365 5b66 6c6f  i(Z:Sequence[flo
+00012b80: 6174 5d2c 2069 3a69 6e74 203d 202d 3129  at], i:int = -1)
+00012b90: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00012ba0: 2063 6920 6973 204e 6f6e 653a 0a20 2020   ci is None:.   
+00012bb0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00012bc0: 7572 6e20 286d 6561 6e28 5a29 2c30 290a  urn (mean(Z),0).
+00012bd0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00012be0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012bf0: 2020 736b 6970 5f65 7272 203d 2028 692b    skip_err = (i+
+00012c00: 3129 2565 7272 6576 6572 790a 2020 2020  1)%errevery.    
+00012c10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00012c20: 726e 2028 6369 2e70 6f69 6e74 285a 292c  rn (ci.point(Z),
+00012c30: 2028 302c 3029 2920 6966 2073 6b69 705f   (0,0)) if skip_
+00012c40: 6572 7220 656c 7365 2063 692e 706f 696e  err else ci.poin
+00012c50: 745f 696e 7465 7276 616c 285a 290a 0a20  t_interval(Z).. 
+00012c60: 2020 2020 2020 2072 6574 7572 6e20 6361         return ca
+00012c70: 6c63 5f63 690a 0a20 2020 2064 6566 205f  lc_ci..    def _
+00012c80: 6772 6f75 7065 645f 7973 2873 656c 662c  grouped_ys(self,
+00012c90: 202a 6b65 7973 3a20 7374 722c 2079 3a4f   *keys: str, y:O
+00012ca0: 7074 696f 6e61 6c5b 7374 725d 2c20 6675  ptional[str], fu
+00012cb0: 6e63 3a20 4c69 7465 7261 6c5b 276c 6173  nc: Literal['las
+00012cc0: 7427 2c27 6c69 7374 275d 203d 204e 6f6e  t','list'] = Non
+00012cd0: 652c 2063 6172 643a 204c 6974 6572 616c  e, card: Literal
+00012ce0: 5b27 4727 2c27 5327 5d20 3d20 2747 272c  ['G','S'] = 'G',
+00012cf0: 2073 7061 6e3a 4f70 7469 6f6e 616c 5b69   span:Optional[i
+00012d00: 6e74 5d3d 3129 202d 3e20 5365 7175 656e  nt]=1) -> Sequen
+00012d10: 6365 5b54 7570 6c65 5d3a 0a0a 2020 2020  ce[Tuple]:..    
+00012d20: 2020 2020 656e 765f 6361 6368 6520 3d20      env_cache = 
+00012d30: 7365 6c66 2e5f 656e 765f 6361 6368 650a  self._env_cache.
+00012d40: 2020 2020 2020 2020 6c72 6e5f 6361 6368          lrn_cach
+00012d50: 6520 3d20 7365 6c66 2e5f 6c72 6e5f 6361  e = self._lrn_ca
+00012d60: 6368 650a 2020 2020 2020 2020 7661 6c5f  che.        val_
+00012d70: 6361 6368 6520 3d20 7365 6c66 2e5f 7661  cache = self._va
+00012d80: 6c5f 6361 6368 650a 0a20 2020 2020 2020  l_cache..       
+00012d90: 206e 6565 645f 6861 7368 6572 203d 204e   need_hasher = N
+00012da0: 6f6e 650a 0a20 2020 2020 2020 2044 203d  one..        D =
+00012db0: 2064 6963 7428 2920 6966 2063 6172 6420   dict() if card 
+00012dc0: 3d3d 2027 5327 2065 6c73 6520 6465 6661  == 'S' else defa
+00012dd0: 756c 7464 6963 7428 6c69 7374 290a 0a20  ultdict(list).. 
+00012de0: 2020 2020 2020 2064 6566 2069 735f 6963         def is_ic
+00012df0: 6f6c 286b 6579 293a 0a20 2020 2020 2020  ol(key):.       
+00012e00: 2020 2020 2072 6574 7572 6e20 6b65 7920       return key 
+00012e10: 6e6f 7420 696e 205b 2765 6e76 6972 6f6e  not in ['environ
+00012e20: 6d65 6e74 5f69 6427 2c27 6c65 6172 6e65  ment_id','learne
+00012e30: 725f 6964 272c 2765 7661 6c75 6174 6f72  r_id','evaluator
+00012e40: 5f69 6427 5d20 616e 6420 6b65 7920 696e  _id'] and key in
+00012e50: 2073 656c 662e 696e 7465 7261 6374 696f   self.interactio
+00012e60: 6e73 2e63 6f6c 756d 6e73 0a0a 2020 2020  ns.columns..    
+00012e70: 2020 2020 6465 6620 6765 745f 6963 6f6c      def get_icol
+00012e80: 7328 6b65 7973 293a 0a20 2020 2020 2020  s(keys):.       
+00012e90: 2020 2020 2066 6f72 206b 6579 2069 6e20       for key in 
+00012ea0: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+00012eb0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00012ec0: 6e63 6528 6b65 792c 286c 6973 742c 7475  nce(key,(list,tu
+00012ed0: 706c 6529 293a 0a20 2020 2020 2020 2020  ple)):.         
+00012ee0: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+00012ef0: 2066 726f 6d20 6765 745f 6963 6f6c 7328   from get_icols(
+00012f00: 6b65 7929 0a20 2020 2020 2020 2020 2020  key).           
+00012f10: 2020 2020 2065 6c69 6620 6973 5f69 636f       elif is_ico
+00012f20: 6c28 6b65 7929 3a0a 2020 2020 2020 2020  l(key):.        
+00012f30: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+00012f40: 6420 6b65 790a 0a20 2020 2020 2020 2064  d key..        d
+00012f50: 6566 206d 616b 655f 6765 7473 2863 6f6c  ef make_gets(col
+00012f60: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00012f70: 666f 7220 636f 6c20 696e 2063 6f6c 733a  for col in cols:
+00012f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012f90: 2069 6620 6973 696e 7374 616e 6365 2863   if isinstance(c
+00012fa0: 6f6c 2c28 7475 706c 652c 6c69 7374 2929  ol,(tuple,list))
+00012fb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012fc0: 2020 2020 2020 7969 656c 6420 6c61 6d62        yield lamb
+00012fd0: 6461 2065 2c6c 2c76 2c73 2c4e 2c47 3d6c  da e,l,v,s,N,G=l
+00012fe0: 6973 7428 6d61 6b65 5f67 6574 7328 636f  ist(make_gets(co
+00012ff0: 6c29 293a 207a 6970 282a 6d61 7028 6d65  l)): zip(*map(me
+00013000: 7468 6f64 6361 6c6c 6572 2827 5f5f 6361  thodcaller('__ca
+00013010: 6c6c 5f5f 272c 652c 6c2c 762c 732c 4e29  ll__',e,l,v,s,N)
+00013020: 2c47 2929 2069 6620 4e20 213d 2030 2065  ,G)) if N != 0 e
+00013030: 6c73 6520 7475 706c 6528 6d61 7028 6d65  lse tuple(map(me
+00013040: 7468 6f64 6361 6c6c 6572 2827 5f5f 6361  thodcaller('__ca
+00013050: 6c6c 5f5f 272c 652c 6c2c 762c 732c 4e29  ll__',e,l,v,s,N)
+00013060: 2c47 2929 0a20 2020 2020 2020 2020 2020  ,G)).           
+00013070: 2020 2020 2065 6c69 6620 636f 6c20 696e       elif col in
+00013080: 2073 656c 662e 656e 7669 726f 6e6d 656e   self.environmen
+00013090: 7473 2e63 6f6c 756d 6e73 3a0a 2020 2020  ts.columns:.    
+000130a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130b0: 7969 656c 6420 6c61 6d62 6461 2065 2c6c  yield lambda e,l
+000130c0: 2c76 2c73 2c4e 2c63 6f6c 3d63 6f6c 3a20  ,v,s,N,col=col: 
+000130d0: 7265 7065 6174 2865 5b63 6f6c 5d2c 4e29  repeat(e[col],N)
+000130e0: 2069 6620 4e20 213d 2030 2065 6c73 6520   if N != 0 else 
+000130f0: 655b 636f 6c5d 0a20 2020 2020 2020 2020  e[col].         
+00013100: 2020 2020 2020 2065 6c69 6620 636f 6c20         elif col 
+00013110: 696e 2073 656c 662e 6c65 6172 6e65 7273  in self.learners
+00013120: 2e63 6f6c 756d 6e73 206f 7220 636f 6c20  .columns or col 
+00013130: 3d3d 2027 6675 6c6c 5f6e 616d 6527 3a0a  == 'full_name':.
+00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013150: 2020 2020 7969 656c 6420 6c61 6d62 6461      yield lambda
+00013160: 2065 2c6c 2c76 2c73 2c4e 2c63 6f6c 3d63   e,l,v,s,N,col=c
+00013170: 6f6c 3a20 7265 7065 6174 286c 5b63 6f6c  ol: repeat(l[col
+00013180: 5d2c 4e29 2069 6620 4e20 213d 2030 2065  ],N) if N != 0 e
+00013190: 6c73 6520 6c5b 636f 6c5d 0a20 2020 2020  lse l[col].     
+000131a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000131b0: 636f 6c20 696e 2073 656c 662e 6576 616c  col in self.eval
+000131c0: 7561 746f 7273 2e63 6f6c 756d 6e73 3a0a  uators.columns:.
+000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131e0: 2020 2020 7969 656c 6420 6c61 6d62 6461      yield lambda
+000131f0: 2065 2c6c 2c76 2c73 2c4e 2c63 6f6c 3d63   e,l,v,s,N,col=c
+00013200: 6f6c 3a20 7265 7065 6174 2876 5b63 6f6c  ol: repeat(v[col
+00013210: 5d2c 4e29 2069 6620 4e20 213d 2030 2065  ],N) if N != 0 e
+00013220: 6c73 6520 765b 636f 6c5d 0a20 2020 2020  lse v[col].     
+00013230: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00013240: 636f 6c20 696e 2073 656c 662e 696e 7465  col in self.inte
+00013250: 7261 6374 696f 6e73 2e63 6f6c 756d 6e73  ractions.columns
+00013260: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013270: 2020 2020 2020 7969 656c 6420 6c61 6d62        yield lamb
+00013280: 6461 2065 2c6c 2c76 2c73 2c4e 2c63 6f6c  da e,l,v,s,N,col
+00013290: 3d63 6f6c 3a20 6974 6572 2873 2e70 6f70  =col: iter(s.pop
+000132a0: 2829 290a 0a20 2020 2020 2020 2067 6574  ())..        get
+000132b0: 7320 203d 206c 6973 7428 6d61 6b65 5f67  s  = list(make_g
+000132c0: 6574 7328 6b65 7973 2929 0a20 2020 2020  ets(keys)).     
+000132d0: 2020 2069 636f 6c73 203d 206c 6973 7428     icols = list(
+000132e0: 6765 745f 6963 6f6c 7328 6b65 7973 2929  get_icols(keys))
+000132f0: 0a20 2020 2020 2020 2069 636f 6c73 2e72  .        icols.r
+00013300: 6576 6572 7365 2829 0a0a 2020 2020 2020  everse()..      
+00013310: 2020 6966 2079 3a20 6963 6f6c 7320 2b3d    if y: icols +=
+00013320: 205b 795d 0a20 2020 2020 2020 2066 6f72   [y].        for
+00013330: 2028 6569 642c 6c69 642c 7669 6429 2c20   (eid,lid,vid), 
+00013340: 7365 6c20 696e 2073 656c 662e 696e 7465  sel in self.inte
+00013350: 7261 6374 696f 6e73 2e67 726f 7570 6279  ractions.groupby
+00013360: 2833 2c69 636f 6c73 293a 0a0a 2020 2020  (3,icols):..    
+00013370: 2020 2020 2020 2020 656e 7620 3d20 656e          env = en
+00013380: 765f 6361 6368 655b 6569 645d 0a20 2020  v_cache[eid].   
+00013390: 2020 2020 2020 2020 206c 726e 203d 206c           lrn = l
+000133a0: 726e 5f63 6163 6865 5b6c 6964 5d0a 2020  rn_cache[lid].  
+000133b0: 2020 2020 2020 2020 2020 7661 6c20 3d20            val = 
+000133c0: 7661 6c5f 6361 6368 655b 7669 645d 0a0a  val_cache[vid]..
+000133d0: 2020 2020 2020 2020 2020 2020 5920 3d20              Y = 
+000133e0: 7365 6c2e 706f 7028 2920 6966 2079 2065  sel.pop() if y e
+000133f0: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
+00013400: 2020 2020 204e 203d 2030 2069 6620 6e6f       N = 0 if no
+00013410: 7420 7365 6c20 656c 7365 206c 656e 2873  t sel else len(s
+00013420: 656c 5b30 5d29 0a0a 2020 2020 2020 2020  el[0])..        
+00013430: 2020 2020 6f75 7473 203d 2074 7570 6c65      outs = tuple
+00013440: 286d 6170 286d 6574 686f 6463 616c 6c65  (map(methodcalle
+00013450: 7228 275f 5f63 616c 6c5f 5f27 2c65 6e76  r('__call__',env
+00013460: 2c6c 726e 2c76 616c 2c73 656c 2c4e 292c  ,lrn,val,sel,N),
+00013470: 6765 7473 2929 0a0a 2020 2020 2020 2020  gets))..        
+00013480: 2020 2020 6966 204e 2021 3d20 303a 206f      if N != 0: o
+00013490: 7574 7320 3d20 7a69 7028 2a6f 7574 7329  uts = zip(*outs)
+000134a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000134b0: 4e20 3d3d 2030 2061 6e64 2066 756e 6320  N == 0 and func 
+000134c0: 6973 204e 6f6e 6520 616e 6420 7920 6973  is None and y is
+000134d0: 206e 6f74 204e 6f6e 653a 2066 756e 6320   not None: func 
+000134e0: 3d20 276c 6173 7427 0a0a 2020 2020 2020  = 'last'..      
+000134f0: 2020 2020 2020 6966 206e 6565 645f 6861        if need_ha
+00013500: 7368 6572 2069 7320 4e6f 6e65 3a0a 2020  sher is None:.  
+00013510: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00013520: 742c 206f 7574 7320 3d20 286f 7574 732c  t, outs = (outs,
+00013530: 206f 7574 7329 2069 6620 4e20 3d3d 2030   outs) if N == 0
+00013540: 2065 6c73 6520 7065 656b 5f66 6972 7374   else peek_first
+00013550: 286f 7574 7329 0a20 2020 2020 2020 2020  (outs).         
+00013560: 2020 2020 2020 206e 6565 645f 6861 7368         need_hash
+00013570: 6572 203d 2074 7279 5f65 6c73 6528 6c61  er = try_else(la
+00013580: 6d62 6461 3a20 6e6f 7420 626f 6f6c 2868  mbda: not bool(h
+00013590: 6173 6828 6f75 7429 292c 2054 7275 6529  ash(out)), True)
+000135a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000135b0: 2069 6620 6e65 6564 5f68 6173 6865 723a   if need_hasher:
+000135c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000135d0: 2020 2020 2072 6169 7365 2043 6f62 6145       raise CobaE
+000135e0: 7863 6570 7469 6f6e 2822 5265 7375 6c74  xception("Result
+000135f0: 2072 6571 7569 7265 7320 616c 6c20 6461   requires all da
+00013600: 7461 2074 6f20 6265 2068 6173 6861 626c  ta to be hashabl
+00013610: 652e 2229 0a0a 2020 2020 2020 2020 2020  e.")..          
+00013620: 2020 6966 204e 203d 3d20 303a 0a20 2020    if N == 0:.   
+00013630: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00013640: 7920 6973 204e 6f6e 653a 0a20 2020 2020  y is None:.     
+00013650: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00013660: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00013670: 2020 2020 2020 2020 656c 6966 2066 756e          elif fun
+00013680: 6320 3d3d 2027 6c61 7374 273a 0a20 2020  c == 'last':.   
+00013690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136a0: 2076 203d 2059 5b2d 315d 2069 6620 7370   v = Y[-1] if sp
+000136b0: 616e 203d 3d20 3120 656c 7365 206d 6561  an == 1 else mea
+000136c0: 6e28 595b 2d73 7061 6e3a 5d29 2069 6620  n(Y[-span:]) if 
+000136d0: 7370 616e 2065 6c73 6520 6d65 616e 2859  span else mean(Y
+000136e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000136f0: 2020 656c 6966 2066 756e 6320 3d3d 2027    elif func == '
+00013700: 6c69 7374 273a 0a20 2020 2020 2020 2020  list':.         
+00013710: 2020 2020 2020 2020 2020 2076 203d 2059             v = Y
+00013720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013730: 2069 6620 6361 7264 203d 3d20 2747 273a   if card == 'G':
+00013740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013750: 2020 2020 2044 5b6f 7574 735d 2e61 7070       D[outs].app
+00013760: 656e 6428 7629 0a20 2020 2020 2020 2020  end(v).         
+00013770: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013790: 2044 5b6f 7574 735d 203d 2076 0a20 2020   D[outs] = v.   
+000137a0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+000137b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000137c0: 6620 7920 6973 204e 6f6e 653a 0a20 2020  f y is None:.   
+000137d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137e0: 2076 203d 2072 6570 6561 7428 4e6f 6e65   v = repeat(None
+000137f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013800: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00013810: 2020 2020 2020 2020 2020 2020 7620 3d20              v = 
+00013820: 6d6f 7669 6e67 5f61 7665 7261 6765 2859  moving_average(Y
+00013830: 2c73 7061 6e29 0a20 2020 2020 2020 2020  ,span).         
+00013840: 2020 2020 2020 2069 6620 6361 7264 203d         if card =
+00013850: 3d20 2747 273a 0a20 2020 2020 2020 2020  = 'G':.         
+00013860: 2020 2020 2020 2020 2020 2066 6f72 206f             for o
+00013870: 2c79 5f20 696e 207a 6970 286f 7574 732c  ,y_ in zip(outs,
+00013880: 7629 3a0a 2020 2020 2020 2020 2020 2020  v):.            
+00013890: 2020 2020 2020 2020 2020 2020 445b 6f5d              D[o]
+000138a0: 2e61 7070 656e 6428 795f 290a 2020 2020  .append(y_).    
+000138b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000138c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000138d0: 2020 2020 2020 442e 7570 6461 7465 287a        D.update(z
+000138e0: 6970 286f 7574 732c 7629 290a 0a20 2020  ip(outs,v))..   
+000138f0: 2020 2020 2072 6574 7572 6e20 5b6b 202b       return [k +
+00013900: 2028 762c 2920 666f 7220 6b2c 7620 696e   (v,) for k,v in
+00013910: 2044 2e69 7465 6d73 2829 5d0a 0a20 2020   D.items()]..   
+00013920: 2064 6566 205f 676c 6f62 616c 5f6e 2873   def _global_n(s
+00013930: 656c 662c 206e 3a20 556e 696f 6e5b 696e  elf, n: Union[in
+00013940: 742c 4c69 7465 7261 6c5b 276d 696e 275d  t,Literal['min']
+00013950: 5d29 3a0a 0a20 2020 2020 2020 2065 6e76  ]):..        env
+00013960: 6972 6f6e 6d65 6e74 7320 3d20 7365 6c66  ironments = self
+00013970: 2e65 6e76 6972 6f6e 6d65 6e74 730a 2020  .environments.  
+00013980: 2020 2020 2020 6c65 6172 6e65 7273 2020        learners  
+00013990: 2020 203d 2073 656c 662e 6c65 6172 6e65     = self.learne
+000139a0: 7273 0a20 2020 2020 2020 2065 7661 6c75  rs.        evalu
+000139b0: 6174 6f72 7320 2020 3d20 7365 6c66 2e65  ators   = self.e
+000139c0: 7661 6c75 6174 6f72 730a 2020 2020 2020  valuators.      
+000139d0: 2020 696e 7465 7261 6374 696f 6e73 203d    interactions =
+000139e0: 2073 656c 662e 696e 7465 7261 6374 696f   self.interactio
+000139f0: 6e73 0a0a 2020 2020 2020 2020 656e 765f  ns..        env_
+00013a00: 6c65 6e67 7468 7320 3d20 5b5d 0a20 2020  lengths = [].   
+00013a10: 2020 2020 2074 6f5f 6472 6f70 2020 2020       to_drop    
+00013a20: 203d 205b 5d0a 2020 2020 2020 2020 746f   = [].        to
+00013a30: 5f6b 6565 7020 2020 2020 3d20 5b5d 0a20  _keep     = []. 
+00013a40: 2020 2020 2020 2069 6620 6e20 3d3d 2027         if n == '
+00013a50: 6d69 6e27 3a0a 2020 2020 2020 2020 2020  min':.          
+00013a60: 2020 666f 7220 656e 765f 6964 782c 2065    for env_idx, e
+00013a70: 6e76 5f6c 656e 2069 6e20 7365 6c66 2e69  nv_len in self.i
+00013a80: 6e74 6572 6163 7469 6f6e 732e 6772 6f75  nteractions.grou
+00013a90: 7062 7928 332c 2763 6f75 6e74 2729 3a0a  pby(3,'count'):.
+00013aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ab0: 656e 765f 6c65 6e67 7468 732e 6170 7065  env_lengths.appe
+00013ac0: 6e64 2865 6e76 5f6c 656e 290a 2020 2020  nd(env_len).    
+00013ad0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00013ae0: 2020 2020 2020 666f 7220 656e 765f 6964        for env_id
+00013af0: 782c 2065 6e76 5f6c 656e 2069 6e20 7365  x, env_len in se
+00013b00: 6c66 2e69 6e74 6572 6163 7469 6f6e 732e  lf.interactions.
+00013b10: 6772 6f75 7062 7928 332c 2763 6f75 6e74  groupby(3,'count
+00013b20: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+00013b30: 2020 2020 6966 2065 6e76 5f6c 656e 203c      if env_len <
+00013b40: 206e 3a0a 2020 2020 2020 2020 2020 2020   n:.            
+00013b50: 2020 2020 2020 2020 746f 5f64 726f 702e          to_drop.
+00013b60: 6170 7065 6e64 2865 6e76 5f69 6478 290a  append(env_idx).
+00013b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b80: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00013b90: 2020 2020 2020 2020 2020 656e 765f 6c65            env_le
+00013ba0: 6e67 7468 732e 6170 7065 6e64 2865 6e76  ngths.append(env
+00013bb0: 5f6c 656e 290a 2020 2020 2020 2020 2020  _len).          
+00013bc0: 2020 2020 2020 2020 2020 746f 5f6b 6565            to_kee
+00013bd0: 702e 6170 7065 6e64 2865 6e76 5f69 6478  p.append(env_idx
+00013be0: 290a 0a20 2020 2020 2020 2069 6620 746f  )..        if to
+00013bf0: 5f64 726f 703a 0a20 2020 2020 2020 2020  _drop:.         
+00013c00: 2020 206e 5f64 726f 7070 6564 203d 206c     n_dropped = l
+00013c10: 656e 2874 6f5f 6472 6f70 290a 2020 2020  en(to_drop).    
+00013c20: 2020 2020 2020 2020 696e 7465 7261 6374          interact
+00013c30: 696f 6e73 203d 2054 6162 6c65 2856 6965  ions = Table(Vie
+00013c40: 7728 696e 7465 7261 6374 696f 6e73 2e5f  w(interactions._
+00013c50: 6461 7461 2c73 656c 662e 5f72 656d 6f76  data,self._remov
+00013c60: 6528 746f 5f64 726f 702c 6e29 292c 2069  e(to_drop,n)), i
+00013c70: 6e74 6572 6163 7469 6f6e 732e 636f 6c75  nteractions.colu
+00013c80: 6d6e 732c 2069 6e74 6572 6163 7469 6f6e  mns, interaction
+00013c90: 732e 696e 6465 7865 7329 0a20 2020 2020  s.indexes).     
+00013ca0: 2020 2020 2020 2069 6620 6e5f 6472 6f70         if n_drop
+00013cb0: 7065 643d 3d31 3a20 436f 6261 436f 6e74  ped==1: CobaCont
+00013cc0: 6578 742e 6c6f 6767 6572 2e6c 6f67 2866  ext.logger.log(f
+00013cd0: 2257 6520 7265 6d6f 7665 6420 7b6e 5f64  "We removed {n_d
+00013ce0: 726f 7070 6564 7d20 6c65 6172 6e65 7220  ropped} learner 
+00013cf0: 6576 616c 7561 7469 6f6e 2062 6563 6175  evaluation becau
+00013d00: 7365 2069 7420 7761 7320 7368 6f72 7465  se it was shorte
+00013d10: 7220 7468 616e 207b 6e7d 2069 6e74 6572  r than {n} inter
+00013d20: 6163 7469 6f6e 732e 2229 0a20 2020 2020  actions.").     
+00013d30: 2020 2020 2020 2069 6620 6e5f 6472 6f70         if n_drop
+00013d40: 7065 643e 3d32 3a20 436f 6261 436f 6e74  ped>=2: CobaCont
+00013d50: 6578 742e 6c6f 6767 6572 2e6c 6f67 2866  ext.logger.log(f
+00013d60: 2257 6520 7265 6d6f 7665 6420 7b6e 5f64  "We removed {n_d
+00013d70: 726f 7070 6564 7d20 6c65 6172 6e65 7220  ropped} learner 
+00013d80: 6576 616c 7561 7469 6f6e 7320 6265 6361  evaluations beca
+00013d90: 7573 6520 7468 6579 2077 6572 6520 7368  use they were sh
+00013da0: 6f72 7465 7220 7468 616e 207b 6e7d 2069  orter than {n} i
+00013db0: 6e74 6572 6163 7469 6f6e 732e 2229 0a0a  nteractions.")..
+00013dc0: 2020 2020 2020 2020 656e 765f 6c65 6e67          env_leng
+00013dd0: 7468 7320 3d20 636f 6c6c 6563 7469 6f6e  ths = collection
+00013de0: 732e 436f 756e 7465 7228 656e 765f 6c65  s.Counter(env_le
+00013df0: 6e67 7468 7329 0a20 2020 2020 2020 2073  ngths).        s
+00013e00: 686f 7274 656e 5f74 6f20 3d20 6d69 6e28  horten_to = min(
+00013e10: 656e 765f 6c65 6e67 7468 7329 2069 6620  env_lengths) if 
+00013e20: 6e3d 3d27 6d69 6e27 2061 6e64 2065 6e76  n=='min' and env
+00013e30: 5f6c 656e 6774 6873 2065 6c73 6520 6e0a  _lengths else n.
+00013e40: 2020 2020 2020 2020 6966 206c 656e 2865          if len(e
+00013e50: 6e76 5f6c 656e 6774 6873 2920 3e20 3120  nv_lengths) > 1 
+00013e60: 6f72 2065 6e76 5f6c 656e 6774 6873 2e76  or env_lengths.v
+00013e70: 616c 7565 7328 2920 213d 207b 7368 6f72  alues() != {shor
+00013e80: 7465 6e5f 746f 7d3a 0a20 2020 2020 2020  ten_to}:.       
+00013e90: 2020 2020 206e 5f73 686f 7274 656e 6564       n_shortened
+00013ea0: 203d 2073 756d 2876 2066 6f72 206b 2c76   = sum(v for k,v
+00013eb0: 2069 6e20 656e 765f 6c65 6e67 7468 732e   in env_lengths.
+00013ec0: 6974 656d 7328 2920 6966 206b 203e 2073  items() if k > s
+00013ed0: 686f 7274 656e 5f74 6f29 0a20 2020 2020  horten_to).     
+00013ee0: 2020 2020 2020 2069 6e74 6572 6163 7469         interacti
+00013ef0: 6f6e 7320 3d20 696e 7465 7261 6374 696f  ons = interactio
+00013f00: 6e73 2e77 6865 7265 2869 6e64 6578 3d7b  ns.where(index={
+00013f10: 273c 3d27 3a73 686f 7274 656e 5f74 6f7d  '<=':shorten_to}
+00013f20: 2920 232e 340a 2020 2020 2020 2020 2020  ) #.4.          
+00013f30: 2020 6966 206e 5f73 686f 7274 656e 6564    if n_shortened
+00013f40: 3d3d 313a 2043 6f62 6143 6f6e 7465 7874  ==1: CobaContext
+00013f50: 2e6c 6f67 6765 722e 6c6f 6728 6622 5765  .logger.log(f"We
+00013f60: 2073 686f 7274 656e 6564 207b 6e5f 7368   shortened {n_sh
+00013f70: 6f72 7465 6e65 647d 206c 6561 726e 6572  ortened} learner
+00013f80: 2065 7661 6c75 6174 696f 6e20 6265 6361   evaluation beca
+00013f90: 7573 6520 6974 2077 6173 206c 6f6e 6765  use it was longe
+00013fa0: 7220 7468 616e 2074 6865 2073 686f 7274  r than the short
+00013fb0: 6573 7420 656e 7669 726f 6e6d 656e 742e  est environment.
+00013fc0: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+00013fd0: 6620 6e5f 7368 6f72 7465 6e65 643e 3d32  f n_shortened>=2
+00013fe0: 3a20 436f 6261 436f 6e74 6578 742e 6c6f  : CobaContext.lo
+00013ff0: 6767 6572 2e6c 6f67 2866 2257 6520 7368  gger.log(f"We sh
+00014000: 6f72 7465 6e65 6420 7b6e 5f73 686f 7274  ortened {n_short
+00014010: 656e 6564 7d20 6c65 6172 6e65 7220 6576  ened} learner ev
+00014020: 616c 7561 7469 6f6e 7320 6265 6361 7573  aluations becaus
+00014030: 6520 7468 6579 2077 6572 6520 6c6f 6e67  e they were long
+00014040: 6572 2074 6861 6e20 7468 6520 7368 6f72  er than the shor
+00014050: 7465 7374 2065 6e76 6972 6f6e 6d65 6e74  test environment
+00014060: 2e22 290a 0a20 2020 2020 2020 206b 6565  .")..        kee
+00014070: 705f 656e 7673 2c6b 6565 705f 6c72 6e73  p_envs,keep_lrns
+00014080: 2c6b 6565 705f 7661 6c73 203d 206d 6170  ,keep_vals = map
+00014090: 2873 6574 2c7a 6970 282a 746f 5f6b 6565  (set,zip(*to_kee
+000140a0: 7029 2920 6966 2074 6f5f 6b65 6570 2065  p)) if to_keep e
+000140b0: 6c73 6520 285b 5d2c 5b5d 2c5b 5d29 0a0a  lse ([],[],[])..
+000140c0: 2020 2020 2020 2020 6966 2074 6f5f 6472          if to_dr
+000140d0: 6f70 2061 6e64 206c 656e 286b 6565 705f  op and len(keep_
+000140e0: 656e 7673 2920 213d 206c 656e 2865 6e76  envs) != len(env
+000140f0: 6972 6f6e 6d65 6e74 7329 3a0a 2020 2020  ironments):.    
+00014100: 2020 2020 2020 2020 656e 7669 726f 6e6d          environm
+00014110: 656e 7473 203d 2065 6e76 6972 6f6e 6d65  ents = environme
+00014120: 6e74 732e 7768 6572 6528 656e 7669 726f  nts.where(enviro
+00014130: 6e6d 656e 745f 6964 3d6b 6565 705f 656e  nment_id=keep_en
+00014140: 7673 290a 0a20 2020 2020 2020 2069 6620  vs)..        if 
+00014150: 746f 5f64 726f 7020 616e 6420 6c65 6e28  to_drop and len(
+00014160: 6b65 6570 5f6c 726e 7329 2021 3d20 6c65  keep_lrns) != le
+00014170: 6e28 6c65 6172 6e65 7273 293a 0a20 2020  n(learners):.   
+00014180: 2020 2020 2020 2020 206c 6561 726e 6572           learner
+00014190: 7320 3d20 6c65 6172 6e65 7273 2e77 6865  s = learners.whe
+000141a0: 7265 286c 6561 726e 6572 5f69 643d 6b65  re(learner_id=ke
+000141b0: 6570 5f6c 726e 7329 0a0a 2020 2020 2020  ep_lrns)..      
+000141c0: 2020 6966 2074 6f5f 6472 6f70 2061 6e64    if to_drop and
+000141d0: 206c 656e 286b 6565 705f 7661 6c73 2920   len(keep_vals) 
+000141e0: 213d 206c 656e 2865 7661 6c75 6174 6f72  != len(evaluator
+000141f0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00014200: 6576 616c 7561 746f 7273 203d 2065 7661  evaluators = eva
+00014210: 6c75 6174 6f72 732e 7768 6572 6528 6576  luators.where(ev
+00014220: 616c 7561 746f 725f 6964 3d6b 6565 705f  aluator_id=keep_
+00014230: 7661 6c73 290a 0a20 2020 2020 2020 2072  vals)..        r
+00014240: 6574 7572 6e20 5265 7375 6c74 2865 6e76  eturn Result(env
+00014250: 6972 6f6e 6d65 6e74 732c 206c 6561 726e  ironments, learn
+00014260: 6572 732c 2065 7661 6c75 6174 6f72 732c  ers, evaluators,
+00014270: 2069 6e74 6572 6163 7469 6f6e 732c 2073   interactions, s
+00014280: 656c 662e 6578 7065 7269 6d65 6e74 290a  elf.experiment).
+00014290: 0a20 2020 2064 6566 205f 6772 6f75 705f  .    def _group_
+000142a0: 7028 7365 6c66 2c20 6c3a 556e 696f 6e5b  p(self, l:Union[
+000142b0: 7374 722c 2053 6571 7565 6e63 655b 7374  str, Sequence[st
+000142c0: 725d 5d2c 2070 3a55 6e69 6f6e 5b73 7472  r]], p:Union[str
+000142d0: 2c20 5365 7175 656e 6365 5b73 7472 5d5d  , Sequence[str]]
+000142e0: 293a 0a0a 2020 2020 2020 2020 656e 7669  ):..        envi
+000142f0: 726f 6e6d 656e 7473 203d 2073 656c 662e  ronments = self.
+00014300: 656e 7669 726f 6e6d 656e 7473 0a20 2020  environments.   
+00014310: 2020 2020 206c 6561 726e 6572 7320 2020       learners   
+00014320: 2020 3d20 7365 6c66 2e6c 6561 726e 6572    = self.learner
+00014330: 730a 2020 2020 2020 2020 6576 616c 7561  s.        evalua
+00014340: 746f 7273 2020 203d 2073 656c 662e 6576  tors   = self.ev
+00014350: 616c 7561 746f 7273 0a20 2020 2020 2020  aluators.       
+00014360: 2069 6e74 6572 6163 7469 6f6e 7320 3d20   interactions = 
+00014370: 7365 6c66 2e69 6e74 6572 6163 7469 6f6e  self.interaction
+00014380: 730a 0a20 2020 2020 2020 2069 6e64 6578  s..        index
+00014390: 6573 2020 3d20 6c69 7374 2873 656c 662e  es  = list(self.
+000143a0: 5f67 726f 7570 6564 5f79 7328 702c 6c2c  _grouped_ys(p,l,
+000143b0: 2765 6e76 6972 6f6e 6d65 6e74 5f69 6427  'environment_id'
+000143c0: 2c27 6c65 6172 6e65 725f 6964 272c 2765  ,'learner_id','e
+000143d0: 7661 6c75 6174 6f72 5f69 6427 2c79 3d4e  valuator_id',y=N
+000143e0: 6f6e 652c 6361 7264 3d27 5327 2929 0a20  one,card='S')). 
+000143f0: 2020 2020 2020 206e 5f6c 6576 656c 7320         n_levels 
+00014400: 3d20 6c65 6e28 7365 7428 6d61 7028 6974  = len(set(map(it
+00014410: 656d 6765 7474 6572 2831 292c 696e 6465  emgetter(1),inde
+00014420: 7865 7329 2929 0a0a 2020 2020 2020 2020  xes)))..        
+00014430: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00014440: 2069 6e64 6578 6573 203d 2073 6f72 7465   indexes = sorte
+00014450: 6428 696e 6465 7865 7329 0a20 2020 2020  d(indexes).     
+00014460: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+00014470: 2020 2020 2020 2073 6f72 7465 645f 3d46         sorted_=F
+00014480: 616c 7365 0a20 2020 2020 2020 2065 6c73  alse.        els
+00014490: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000144a0: 6f72 7465 645f 3d54 7275 650a 0a20 2020  orted_=True..   
+000144b0: 2020 2020 2074 6f5f 6b65 6570 2c20 746f       to_keep, to
+000144c0: 5f72 656d 6f76 652c 206e 5f6c 6172 6765  _remove, n_large
+000144d0: 722c 206e 5f73 6d61 6c6c 6572 203d 205b  r, n_smaller = [
+000144e0: 5d2c 205b 5d2c 2030 2c20 300a 2020 2020  ], [], 0, 0.    
+000144f0: 2020 2020 666f 7220 5f2c 2067 726f 7570      for _, group
+00014500: 2069 6e20 6772 6f75 7065 7228 696e 6465   in grouper(inde
+00014510: 7865 732c 6b65 793d 6974 656d 6765 7474  xes,key=itemgett
+00014520: 6572 2830 292c 2073 6f72 7465 645f 3d73  er(0), sorted_=s
+00014530: 6f72 7465 645f 293a 0a20 2020 2020 2020  orted_):.       
+00014540: 2020 2020 2067 726f 7570 203d 206c 6973       group = lis
+00014550: 7428 6772 6f75 7029 0a20 2020 2020 2020  t(group).       
+00014560: 2020 2020 2069 6620 6c65 6e28 6772 6f75       if len(grou
+00014570: 7029 203e 206e 5f6c 6576 656c 733a 0a20  p) > n_levels:. 
+00014580: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00014590: 5f6c 6172 6765 7220 2b3d 2031 0a20 2020  _larger += 1.   
+000145a0: 2020 2020 2020 2020 2020 2020 2074 6f5f               to_
+000145b0: 7265 6d6f 7665 2e65 7874 656e 6428 675b  remove.extend(g[
+000145c0: 323a 355d 2066 6f72 2067 2069 6e20 6772  2:5] for g in gr
+000145d0: 6f75 7029 0a20 2020 2020 2020 2020 2020  oup).           
+000145e0: 2065 6c69 6620 6c65 6e28 6772 6f75 7029   elif len(group)
+000145f0: 203c 206e 5f6c 6576 656c 733a 0a20 2020   < n_levels:.   
+00014600: 2020 2020 2020 2020 2020 2020 206e 5f73               n_s
+00014610: 6d61 6c6c 6572 202b 3d20 310a 2020 2020  maller += 1.    
+00014620: 2020 2020 2020 2020 2020 2020 746f 5f72              to_r
+00014630: 656d 6f76 652e 6578 7465 6e64 2867 5b32  emove.extend(g[2
+00014640: 3a35 5d20 666f 7220 6720 696e 2067 726f  :5] for g in gro
+00014650: 7570 290a 2020 2020 2020 2020 2020 2020  up).            
+00014660: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00014670: 2020 2020 2020 746f 5f6b 6565 702e 6578        to_keep.ex
+00014680: 7465 6e64 2867 5b32 3a35 5d20 666f 7220  tend(g[2:5] for 
+00014690: 6720 696e 2067 726f 7570 290a 0a20 2020  g in group)..   
+000146a0: 2020 2020 2069 6620 6e5f 6c61 7267 6572       if n_larger
+000146b0: 3a0a 2020 2020 2020 2020 2020 2020 436f  :.            Co
+000146c0: 6261 436f 6e74 6578 742e 6c6f 6767 6572  baContext.logger
+000146d0: 2e6c 6f67 2866 2257 6520 7265 6d6f 7665  .log(f"We remove
+000146e0: 6420 7b6e 5f6c 6172 6765 727d 207b 707d  d {n_larger} {p}
+000146f0: 2062 6563 6175 7365 206d 6f72 6520 7468   because more th
+00014700: 616e 206f 6e65 2065 7869 7374 6564 2066  an one existed f
+00014710: 6f72 2065 6163 6820 7b6c 7d2e 2229 0a0a  or each {l}.")..
+00014720: 2020 2020 2020 2020 6966 206e 5f73 6d61          if n_sma
+00014730: 6c6c 6572 3a0a 2020 2020 2020 2020 2020  ller:.          
+00014740: 2020 436f 6261 436f 6e74 6578 742e 6c6f    CobaContext.lo
+00014750: 6767 6572 2e6c 6f67 2866 2257 6520 7265  gger.log(f"We re
+00014760: 6d6f 7665 6420 7b6e 5f73 6d61 6c6c 6572  moved {n_smaller
+00014770: 7d20 7b70 7d20 6265 6361 7573 6520 7b27  } {p} because {'
+00014780: 7468 6579 2720 6966 206e 5f73 6d61 6c6c  they' if n_small
+00014790: 6572 3e31 2065 6c73 6520 2769 7427 7d20  er>1 else 'it'} 
+000147a0: 6469 6420 6e6f 7420 6578 6973 7420 666f  did not exist fo
+000147b0: 7220 6576 6572 7920 7b6c 7d2e 2229 0a0a  r every {l}.")..
+000147c0: 2020 2020 2020 2020 6966 2074 6f5f 7265          if to_re
+000147d0: 6d6f 7665 3a0a 2020 2020 2020 2020 2020  move:.          
+000147e0: 2020 7365 6c65 6374 203d 2073 656c 662e    select = self.
+000147f0: 5f72 656d 6f76 6528 746f 5f72 656d 6f76  _remove(to_remov
+00014800: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
+00014810: 6e74 6572 6163 7469 6f6e 7320 3d20 5461  nteractions = Ta
+00014820: 626c 6528 5669 6577 2869 6e74 6572 6163  ble(View(interac
+00014830: 7469 6f6e 732e 5f64 6174 612c 7365 6c65  tions._data,sele
+00014840: 6374 292c 2069 6e74 6572 6163 7469 6f6e  ct), interaction
+00014850: 732e 636f 6c75 6d6e 732c 2069 6e74 6572  s.columns, inter
+00014860: 6163 7469 6f6e 732e 696e 6465 7865 7329  actions.indexes)
+00014870: 0a0a 2020 2020 2020 2020 655f 6b65 6570  ..        e_keep
+00014880: 2c6c 5f6b 6565 702c 765f 6b65 6570 203d  ,l_keep,v_keep =
+00014890: 206d 6170 2873 6574 2c7a 6970 282a 746f   map(set,zip(*to
+000148a0: 5f6b 6565 7029 2920 6966 2074 6f5f 6b65  _keep)) if to_ke
+000148b0: 6570 2065 6c73 6520 285b 5d2c 5b5d 2c5b  ep else ([],[],[
+000148c0: 5d29 0a20 2020 2020 2020 2069 6620 6c65  ]).        if le
+000148d0: 6e28 655f 6b65 6570 2920 213d 206c 656e  n(e_keep) != len
+000148e0: 2865 6e76 6972 6f6e 6d65 6e74 7329 3a20  (environments): 
+000148f0: 656e 7669 726f 6e6d 656e 7473 203d 2065  environments = e
+00014900: 6e76 6972 6f6e 6d65 6e74 732e 7768 6572  nvironments.wher
+00014910: 6528 656e 7669 726f 6e6d 656e 745f 6964  e(environment_id
+00014920: 3d65 5f6b 6565 7029 0a20 2020 2020 2020  =e_keep).       
+00014930: 2069 6620 6c65 6e28 6c5f 6b65 6570 2920   if len(l_keep) 
+00014940: 213d 206c 656e 286c 6561 726e 6572 7329  != len(learners)
+00014950: 2020 2020 3a20 6c65 6172 6e65 7273 2020      : learners  
+00014960: 2020 203d 206c 6561 726e 6572 7320 2020     = learners   
+00014970: 202e 7768 6572 6528 6c65 6172 6e65 725f   .where(learner_
+00014980: 6964 2020 2020 3d6c 5f6b 6565 7029 0a20  id    =l_keep). 
+00014990: 2020 2020 2020 2069 6620 6c65 6e28 765f         if len(v_
+000149a0: 6b65 6570 2920 213d 206c 656e 2865 7661  keep) != len(eva
+000149b0: 6c75 6174 6f72 7329 2020 3a20 6576 616c  luators)  : eval
+000149c0: 7561 746f 7273 2020 203d 2065 7661 6c75  uators   = evalu
+000149d0: 6174 6f72 7320 202e 7768 6572 6528 6576  ators  .where(ev
+000149e0: 616c 7561 746f 725f 6964 2020 3d76 5f6b  aluator_id  =v_k
+000149f0: 6565 7029 0a0a 2020 2020 2020 2020 7265  eep)..        re
+00014a00: 7475 726e 2052 6573 756c 7428 656e 7669  turn Result(envi
+00014a10: 726f 6e6d 656e 7473 2c20 6c65 6172 6e65  ronments, learne
+00014a20: 7273 2c20 6576 616c 7561 746f 7273 2c20  rs, evaluators, 
+00014a30: 696e 7465 7261 6374 696f 6e73 2c20 7365  interactions, se
+00014a40: 6c66 2e65 7870 6572 696d 656e 7429 0a0a  lf.experiment)..
+00014a50: 2020 2020 6465 6620 5f66 696c 7465 725f      def _filter_
+00014a60: 6669 6e28 7365 6c66 2c0a 2020 2020 2020  fin(self,.      
+00014a70: 2020 6e3a 2055 6e69 6f6e 5b69 6e74 2c4c    n: Union[int,L
+00014a80: 6974 6572 616c 5b27 6d69 6e27 5d2c 204e  iteral['min'], N
+00014a90: 6f6e 655d 2c0a 2020 2020 2020 2020 6c3a  one],.        l:
+00014aa0: 2055 6e69 6f6e 5b73 7472 2c20 5365 7175   Union[str, Sequ
+00014ab0: 656e 6365 5b73 7472 5d2c 204e 6f6e 655d  ence[str], None]
+00014ac0: 2c0a 2020 2020 2020 2020 703a 2055 6e69  ,.        p: Uni
+00014ad0: 6f6e 5b73 7472 2c20 5365 7175 656e 6365  on[str, Sequence
+00014ae0: 5b73 7472 5d2c 204e 6f6e 655d 2920 2d3e  [str], None]) ->
+00014af0: 2027 5265 7375 6c74 273a 0a20 2020 2020   'Result':.     
+00014b00: 2020 2022 2222 4669 6c74 6572 2074 6865     """Filter the
+00014b10: 2072 6573 756c 7473 2064 6f77 6e20 746f   results down to
+00014b20: 2065 7665 6e20 6f75 7463 6f6d 6573 2073   even outcomes s
+00014b30: 6f20 7468 6174 2070 6c6f 7474 6564 2072  o that plotted r
+00014b40: 6573 756c 7473 2077 696c 6c20 6265 206d  esults will be m
+00014b50: 6561 6e69 6e67 6675 6c2e 0a0a 2020 2020  eaningful...    
+00014b60: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00014b70: 2020 2020 2020 6e3a 2054 6865 206e 756d        n: The num
+00014b80: 6265 7220 6f66 2069 6e74 6572 6163 7469  ber of interacti
+00014b90: 6f6e 7320 6120 7370 6563 6966 6963 2065  ons a specific e
+00014ba0: 7661 6c75 6174 696f 6e20 6d75 7374 2068  valuation must h
+00014bb0: 6176 6520 284e 6f6e 6520 696e 6469 6361  ave (None indica
+00014bc0: 7465 7320 6e6f 2063 6f6e 7374 7261 696e  tes no constrain
+00014bd0: 7429 2e0a 2020 2020 2020 2020 2020 2020  t)..            
+00014be0: 6c3a 2054 6865 206c 6576 656c 2061 7420  l: The level at 
+00014bf0: 7768 6963 6820 7765 2077 6973 6820 746f  which we wish to
+00014c00: 2063 6f6d 7061 7265 2065 7661 6c61 7469   compare evalati
+00014c10: 6f6e 206f 7574 636f 6d65 732e 0a20 2020  on outcomes..   
+00014c20: 2020 2020 2020 2020 2070 3a20 5468 6520           p: The 
+00014c30: 7061 6972 7320 7468 6174 206d 7573 7420  pairs that must 
+00014c40: 6578 6973 7420 6163 726f 7373 2061 6c6c  exist across all
+00014c50: 2063 6f6d 7061 7269 736f 6e20 6c65 7665   comparison leve
+00014c60: 6c73 2069 6e20 6f72 6465 7220 746f 2062  ls in order to b
+00014c70: 6520 696e 636c 7564 6564 2e0a 2020 2020  e included..    
+00014c80: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00014c90: 2072 6573 756c 7420 3d20 7365 6c66 2e63   result = self.c
+00014ca0: 6f70 7928 290a 2020 2020 2020 2020 6966  opy().        if
+00014cb0: 206c 206f 7220 703a 2072 6573 756c 7420   l or p: result 
+00014cc0: 3d20 7265 7375 6c74 2e5f 6772 6f75 705f  = result._group_
+00014cd0: 7028 6c2c 7029 0a20 2020 2020 2020 2069  p(l,p).        i
+00014ce0: 6620 6e20 2020 2020 3a20 7265 7375 6c74  f n     : result
+00014cf0: 203d 2072 6573 756c 742e 5f67 6c6f 6261   = result._globa
+00014d00: 6c5f 6e28 6e29 0a20 2020 2020 2020 2072  l_n(n).        r
+00014d10: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00014d20: 2020 6465 6620 5f72 656d 6f76 6528 7365    def _remove(se
+00014d30: 6c66 2c20 6964 733a 2053 6571 7565 6e63  lf, ids: Sequenc
+00014d40: 655b 5475 706c 655b 696e 742c 696e 742c  e[Tuple[int,int,
+00014d50: 696e 745d 5d2c 206e 3d30 2920 2d3e 2053  int]], n=0) -> S
+00014d60: 6571 7565 6e63 655b 696e 745d 3a0a 2020  equence[int]:.  
+00014d70: 2020 2020 2020 2374 6869 7320 6973 206d        #this is m
+00014d80: 7563 6820 6661 7374 6572 2074 6861 6e20  uch faster than 
+00014d90: 616e 7920 6275 696c 7420 696e 2054 6162  any built in Tab
+00014da0: 6c65 206d 6574 686f 6473 0a20 2020 2020  le methods.     
+00014db0: 2020 2023 746f 2077 6f72 6b20 696e 7465     #to work inte
+00014dc0: 7261 6374 696f 6e73 206d 7573 7420 6265  ractions must be
+00014dd0: 2073 6f72 7465 6420 6279 2065 6e76 5f69   sorted by env_i
+00014de0: 642c 6c72 6e5f 6964 2c76 616c 5f69 640a  d,lrn_id,val_id.
+00014df0: 2020 2020 2020 2020 6c6f 6320 2020 2020          loc     
+00014e00: 2020 2020 2020 203d 2030 0a20 2020 2020         = 0.     
+00014e10: 2020 2073 656c 6563 7420 2020 2020 2020     select       
+00014e20: 2020 3d20 5b5d 0a20 2020 2020 2020 206e    = [].        n
+00014e30: 5f69 6e74 6572 6163 7469 6f6e 7320 3d20  _interactions = 
+00014e40: 6c65 6e28 7365 6c66 2e69 6e74 6572 6163  len(self.interac
+00014e50: 7469 6f6e 7329 0a20 2020 2020 2020 2065  tions).        e
+00014e60: 6e76 5f69 6473 2c6c 726e 5f69 6473 2c76  nv_ids,lrn_ids,v
+00014e70: 616c 5f69 6473 203d 2073 656c 662e 696e  al_ids = self.in
+00014e80: 7465 7261 6374 696f 6e73 5b5b 2765 6e76  teractions[['env
+00014e90: 6972 6f6e 6d65 6e74 5f69 6427 2c27 6c65  ironment_id','le
+00014ea0: 6172 6e65 725f 6964 272c 2765 7661 6c75  arner_id','evalu
+00014eb0: 6174 6f72 5f69 6427 5d5d 0a20 2020 2020  ator_id']].     
+00014ec0: 2020 2069 6473 203d 2073 6f72 7465 6428     ids = sorted(
+00014ed0: 6964 7329 0a20 2020 2020 2020 2066 6f72  ids).        for
+00014ee0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00014ef0: 6964 7329 293a 0a20 2020 2020 2020 2020  ids)):.         
+00014f00: 2020 2065 2c6c 2c76 203d 2069 6473 5b69     e,l,v = ids[i
+00014f10: 5d0a 2020 2020 2020 2020 2020 2020 6c6f  ].            lo
+00014f20: 3120 3d20 6d79 5f62 6973 6563 745f 6c65  1 = my_bisect_le
+00014f30: 6674 2028 656e 765f 6964 732c 652c 6c6f  ft (env_ids,e,lo
+00014f40: 632c 6e5f 696e 7465 7261 6374 696f 6e73  c,n_interactions
+00014f50: 290a 2020 2020 2020 2020 2020 2020 6869  ).            hi
+00014f60: 3120 3d20 6d79 5f62 6973 6563 745f 7269  1 = my_bisect_ri
+00014f70: 6768 7428 656e 765f 6964 732c 652c 6c6f  ght(env_ids,e,lo
+00014f80: 632c 6e5f 696e 7465 7261 6374 696f 6e73  c,n_interactions
+00014f90: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00014fa0: 206c 6f31 3d3d 6869 313a 2063 6f6e 7469   lo1==hi1: conti
+00014fb0: 6e75 6520 2374 6865 2067 6976 656e 2069  nue #the given i
+00014fc0: 6473 2061 7265 6e27 7420 696e 2069 6e74  ds aren't in int
+00014fd0: 6572 6163 7469 6f6e 730a 2020 2020 2020  eractions.      
+00014fe0: 2020 2020 2020 6c6f 3220 3d20 6d79 5f62        lo2 = my_b
+00014ff0: 6973 6563 745f 6c65 6674 2028 6c72 6e5f  isect_left (lrn_
+00015000: 6964 732c 6c2c 6c6f 312c 6869 3129 0a20  ids,l,lo1,hi1). 
+00015010: 2020 2020 2020 2020 2020 2068 6932 203d             hi2 =
+00015020: 206d 795f 6269 7365 6374 5f72 6967 6874   my_bisect_right
+00015030: 286c 726e 5f69 6473 2c6c 2c6c 6f31 2c68  (lrn_ids,l,lo1,h
+00015040: 6931 290a 2020 2020 2020 2020 2020 2020  i1).            
+00015050: 6966 206c 6f32 3d3d 6869 323a 2063 6f6e  if lo2==hi2: con
+00015060: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+00015070: 2020 6c6f 3320 3d20 6d79 5f62 6973 6563    lo3 = my_bisec
+00015080: 745f 6c65 6674 2028 7661 6c5f 6964 732c  t_left (val_ids,
+00015090: 762c 6c6f 322c 6869 3229 0a20 2020 2020  v,lo2,hi2).     
+000150a0: 2020 2020 2020 2068 6933 203d 206d 795f         hi3 = my_
+000150b0: 6269 7365 6374 5f72 6967 6874 2876 616c  bisect_right(val
+000150c0: 5f69 6473 2c76 2c6c 6f32 2c68 6932 290a  _ids,v,lo2,hi2).
+000150d0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+000150e0: 6f33 3d3d 6869 333a 2063 6f6e 7469 6e75  o3==hi3: continu
+000150f0: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+00015100: 6c65 6374 2e65 7874 656e 6428 7261 6e67  lect.extend(rang
+00015110: 6528 6c6f 632c 6c6f 332b 286e 2069 6620  e(loc,lo3+(n if 
+00015120: 6869 332d 6c6f 333e 6e20 656c 7365 2030  hi3-lo3>n else 0
+00015130: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+00015140: 6c6f 6320 3d20 6869 330a 0a20 2020 2020  loc = hi3..     
+00015150: 2020 2073 656c 6563 742e 6578 7465 6e64     select.extend
+00015160: 2872 616e 6765 286c 6f63 2c6e 5f69 6e74  (range(loc,n_int
+00015170: 6572 6163 7469 6f6e 7329 290a 2020 2020  eractions)).    
+00015180: 2020 2020 7265 7475 726e 2073 656c 6563      return selec
+00015190: 740a                                     t.
```

### Comparing `coba-8.0.4/coba/results/errors.py` & `coba-8.0.5/coba/results/errors.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/safety.py` & `coba-8.0.5/coba/safety.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/statistics.py` & `coba-8.0.5/coba/statistics.py`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/coba/utilities.py` & `coba-8.0.5/coba/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             raise KeyError( key )
         else:
             value = self.default_factory(key)
             self[key] = value
             return value
 
 _T = TypeVar("_T")
-def peek_first(items: Iterable[_T], n:int=1, reduce:bool=True) -> Tuple[Union[_T,Sequence[_T]], Iterable[_T]]:
+def peek_first(items:Iterable[_T], n:int=1, reduce:bool=True) -> Tuple[Union[_T,Sequence[_T]], Iterable[_T]]:
     items = iter(items)
     first = list(islice(items,n))
 
     items = [] if not first and n>0 else chain(first,items)
     first = [] if n==0 else None if not first else first[0] if n==1 and reduce else first
 
     return first, items
@@ -180,15 +180,15 @@
                 else:
                     o[k] = minobj(v)
             return o
         obj = minobj(obj)
 
     return obj
 
-def grouper(items: Sequence[Any], key:Callable[[Any],Hashable]=None, val:Callable[[Any],Any]=None, sorted_: bool= False) -> Iterable[Tuple[Hashable,Iterable[Any]]]:
+def grouper(items:Sequence[Any], key:Callable[[Any],Hashable]=None, val:Callable[[Any],Any]=None, sorted_:bool=False) -> Iterable[Tuple[Hashable,Iterable[Any]]]:
 
     if sorted_:
         for k, group in groupby(items,key=key):
             if val: yield (k, map(val,group))
             else  : yield (k, group)
 
     else:
```

### Comparing `coba-8.0.4/coba.egg-info/PKG-INFO` & `coba-8.0.5/coba.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coba
-Version: 8.0.4
+Version: 8.0.5
 Summary: A contextual bandit research package
 Author-email: Mark Rucker <rucker.mark@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://coba-docs.readthedocs.io/
 Project-URL: Documentation, https://coba-docs.readthedocs.io/
 Project-URL: Repository, https://github.com/vowpalwabbit/coba
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coba-8.0.4/coba.egg-info/SOURCES.txt` & `coba-8.0.5/coba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coba-8.0.4/pyproject.toml` & `coba-8.0.5/pyproject.toml`

 * *Files identical despite different names*

