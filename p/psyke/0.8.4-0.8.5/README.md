# Comparing `tmp/psyke-0.8.4.tar.gz` & `tmp/psyke-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.8.4.tar", last modified: Sat Apr 27 17:11:45 2024, max compression
+gzip compressed data, was "psyke-0.8.5.tar", last modified: Thu May  2 00:29:10 2024, max compression
```

## Comparing `psyke-0.8.4.tar` & `psyke-0.8.5.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.772245 psyke-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-27 17:10:31.000000 psyke-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 17:10:31.000000 psyke-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-27 17:11:45.772245 psyke-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-27 17:10:31.000000 psyke-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-27 17:11:45.000000 psyke-0.8.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-27 17:11:43.000000 psyke-0.8.4/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.760245 psyke-0.8.4/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/cosmik/
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/cosmik/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/divine/
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/divine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/gridrex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/hex/
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/hex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25430 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/extraction/trepan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/hypercubepredictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    17306 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/tuning/orchid/
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/tuning/orchid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.764245 psyke-0.8.4/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-27 17:10:31.000000 psyke-0.8.4/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.772245 psyke-0.8.4/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 17:11:45.000000 psyke-0.8.4/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 17:10:31.000000 psyke-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 17:11:45.772245 psyke-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-27 17:10:31.000000 psyke-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.756245 psyke-0.8.4/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-27 17:10:31.000000 psyke-0.8.4/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-27 17:10:33.000000 psyke-0.8.4/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.768245 psyke-0.8.4/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-27 17:10:33.000000 psyke-0.8.4/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.772245 psyke-0.8.4/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-27 17:10:33.000000 psyke-0.8.4/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:11:45.772245 psyke-0.8.4/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-27 17:10:33.000000 psyke-0.8.4/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.690924 psyke-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-02 00:27:50.000000 psyke-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 00:27:50.000000 psyke-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-02 00:29:10.690924 psyke-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-02 00:27:50.000000 psyke-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 00:29:10.000000 psyke-0.8.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.678924 psyke-0.8.5/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)    18545 2024-05-02 00:29:08.000000 psyke-0.8.5/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/hypercubic/cosmik/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/hypercubic/cosmik/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/hypercubic/divine/
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/hypercubic/divine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/hypercubic/gridrex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/hypercubic/hex/
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/hypercubic/hex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.682924 psyke-0.8.5/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/extraction/trepan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/hypercubepredictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/psyke/tuning/orchid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/tuning/orchid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-02 00:27:50.000000 psyke-0.8.5/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.690924 psyke-0.8.5/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-02 00:29:10.000000 psyke-0.8.5/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-02 00:29:10.000000 psyke-0.8.5/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:29:10.000000 psyke-0.8.5/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:29:10.000000 psyke-0.8.5/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 00:29:10.000000 psyke-0.8.5/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 00:29:10.000000 psyke-0.8.5/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 00:27:50.000000 psyke-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:29:10.690924 psyke-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-02 00:27:50.000000 psyke-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.678924 psyke-0.8.5/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/test/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.686924 psyke-0.8.5/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.690924 psyke-0.8.5/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.690924 psyke-0.8.5/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.690924 psyke-0.8.5/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-02 00:27:50.000000 psyke-0.8.5/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.690924 psyke-0.8.5/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 00:27:51.000000 psyke-0.8.5/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.690924 psyke-0.8.5/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-02 00:27:51.000000 psyke-0.8.5/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.690924 psyke-0.8.5/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-02 00:27:51.000000 psyke-0.8.5/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:29:10.690924 psyke-0.8.5/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-02 00:27:51.000000 psyke-0.8.5/test/resources/tests/__init__.py
```

### Comparing `psyke-0.8.4/LICENSE` & `psyke-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/PKG-INFO` & `psyke-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.4
+Version: 0.8.5
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.4/README.md` & `psyke-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/__init__.py` & `psyke-0.8.5/psyke/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,27 +57,27 @@
         """
         return self.__convert(self._predict(dataframe))
 
     def _predict(self, dataframe: pd.DataFrame) -> Iterable:
         raise NotImplementedError('predict')
 
     def __convert(self, ys: Iterable) -> Iterable:
-        if self.normalization is not None:
+        if self.normalization is not None and not isinstance([p for p in ys if p is not None][0], str):
             m, s = self.normalization[list(self.normalization.keys())[-1]]
             ys = [prediction if prediction is None else prediction * s + m for prediction in ys]
         return ys
 
     def brute_predict(self, dataframe: pd.DataFrame, criterion: str = 'corner', n: int = 2) -> Iterable:
         return self.__convert(self._brute_predict(dataframe, criterion, n))
 
     def _brute_predict(self, dataframe: pd.DataFrame, criterion: str = 'corner', n: int = 2) -> Iterable:
         raise NotImplementedError('brute_predict')
 
     def unscale(self, values, name):
-        if self.normalization is None or isinstance(values, LinearRegression):
+        if self.normalization is None or name not in self.normalization or isinstance(values, LinearRegression):
             return values
         if isinstance(values, Iterable):
             values = [None if value is None else
                       value * self.normalization[name][1] + self.normalization[name][0] for value in values]
         else:
             values = values * self.normalization[name][1] + self.normalization[name][0]
         return values
@@ -157,25 +157,28 @@
         Extracts rules from the underlying predictor.
 
         :param dataframe: is the set of instances to be used for the extraction.
         :return: the theory created from the extracted rules.
         """
         raise NotImplementedError('extract')
 
-    def predict_why(self, data: dict[str, float]):
+    def predict_why(self, data: dict[str, float], verbose=True):
         """
         Provides a prediction and the corresponding explanation.
         :param data: is the instance to predict.
+        :param verbose: if the explanation has to be printed.
         """
         raise NotImplementedError('predict_why')
 
-    def predict_counter(self, data: dict[str, float]):
+    def predict_counter(self, data: dict[str, float], verbose=True, only_first=True):
         """
         Provides a prediction and counterfactual explanations.
         :param data: is the instance to predict.
+        :param verbose: if the counterfactual explanation has to be printed.
+        :param only_first: if only the closest counterfactual explanation is provided for each distinct class.
         """
         raise NotImplementedError('predict_counter')
 
     def mae(self, dataframe: pd.DataFrame, predictor=None, brute: bool = False, criterion: str = 'center',
             n: int = 3) -> float:
         """
         Calculates the predictions' MAE w.r.t. the instances given as input.
```

### Comparing `psyke-0.8.4/psyke/clustering/__init__.py` & `psyke-0.8.5/psyke/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/clustering/cream/__init__.py` & `psyke-0.8.5/psyke/clustering/cream/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/clustering/exact/__init__.py` & `psyke-0.8.5/psyke/clustering/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/clustering/utils.py` & `psyke-0.8.5/psyke/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/__init__.py` & `psyke-0.8.5/psyke/extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/cart/__init__.py` & `psyke-0.8.5/psyke/extraction/cart/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/cart/predictor.py` & `psyke-0.8.5/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/hypercubic/__init__.py` & `psyke-0.8.5/psyke/extraction/hypercubic/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     def extract(self, dataframe: pd.DataFrame) -> Theory:
         theory = PedagogicalExtractor.extract(self, dataframe)
         self._surrounding = HyperCube.create_surrounding_cube(dataframe, output=self._output)
         self._surrounding.update(dataframe, self.predictor)
         return theory
 
     def pairwise_fairness(self, data: dict[str, float], neighbor: dict[str, float]):
-        cube1 = self._find_cube(data.copy())
-        cube2 = self._find_cube(neighbor.copy())
+        cube1 = self._find_cube(data)
+        cube2 = self._find_cube(neighbor)
         different_prediction_reasons = []
 
         if cube1.output == cube2.output:
             print("Prediction", cube1.output, "is FAIR")
         else:
             print("Prediction", cube1.output, "may be UNFAIR")
             print("It could be", cube2.output, "if:")
@@ -59,84 +59,91 @@
                     print('    ', d, 'increases above', round(a, 1))
                     different_prediction_reasons.append(d)
                 elif data[d] > b:
                     print('    ', d, 'decreases below', round(b, 1))
                     different_prediction_reasons.append(d)
         return different_prediction_reasons
 
-    def predict_counter(self, data: dict[str, float], verbose=True):
+    def predict_counter(self, data: dict[str, float], verbose=True, only_first=True):
         output = ""
         prediction = None
-        cube = self._find_cube(data.copy())
+        cube = self._find_cube(data)
         if cube is None:
             output += "The extracted knowledge is not exhaustive; impossible to predict this instance"
         else:
             prediction = self._predict_from_cubes(data)
-            output += f"The output is {prediction}"
+            output += f"The output is {prediction}\n"
 
         point = Point(list(data.keys()), list(data.values()))
         cubes = self._hypercubes if cube is None else [c for c in self._hypercubes if cube.output != c.output]
         cubes = sorted([(cube.surface_distance(point), cube.volume(), i, cube) for i, cube in enumerate(cubes)])
-        outputs = []
-        different_prediction_reasons = []
+
+        counter_conditions = []
+
         for _, _, _, c in cubes:
-            if c.output not in outputs:
-                outputs.append(c.output)
-                output += f"\nThe output may be {c.output} if"
-
-                for d in point.dimensions.keys():
-                    lower, upper = c[d]
-                    p = point[d]
-                    if p < lower:
-                        output += f"\n     {d} increases above {round(lower, 1)}"
-                        different_prediction_reasons.append((d, '>=', lower))
-                    elif p > upper:
-                        output += f"\n     {d} decreses below {round(upper, 1)}"
-                        different_prediction_reasons.append((d, '<=', upper))
+            if not only_first or c.output not in [o for o, _ in counter_conditions]:
+                counter_conditions.append((c.output, {c: [val for val in v if val is not None and not val.is_in(
+                    self.unscale(data[c], c))] for c, v in self.__get_conditions(data, c).items()}))
+
         if verbose:
+            for o, conditions in counter_conditions:
+                output += f"The output may be {o} if\n" + HyperCubeExtractor.__conditions_to_string(conditions)
             print(output)
-        return prediction, different_prediction_reasons
 
-    def __get_local_conditions(self, data: dict[str, float], cube: GenericCube) -> dict[list[Value]]:
-        conditions = {d: [cube.interval_to_value(d, self.unscale)] for d in data.keys()}
-        subcubes = cube.subcubes(self._hypercubes)
-        subsubcubes = [c for cube_list in [c.subcubes(self._hypercubes) for c in subcubes] for c in cube_list]
-        for c in [c for c in subcubes if c not in subsubcubes]:
+        return prediction, counter_conditions
+
+    @staticmethod
+    def __conditions_to_string(conditions: dict[str, list[Value]]) -> str:
+        output = ""
+        for d in conditions:
+            for i, condition in enumerate(conditions[d]):
+                if i == 0:
+                    output += f'     {d} is '
+                else:
+                    output += ' and '
+                output += condition.print()
+                if i + 1 == len(conditions[d]):
+                    output += '\n'
+        return output
+
+    def __get_conditions(self, data: dict[str, float], cube: GenericCube) -> dict[str, list[Value]]:
+        conditions = {d: [cube.interval_to_value(d, self.unscale)] for d in data.keys()
+                      if d not in self._dimensions_to_ignore}
+        for c in cube.subcubes(self._hypercubes):
             for d in conditions:
                 condition = c.interval_to_value(d, self.unscale)
                 if condition is None:
                     continue
                 elif conditions[d][-1] is None:
                     conditions[d][-1] = -condition
-                elif (-condition).is_in(data[d]):
+                else:
                     try:
                         conditions[d][-1] *= -condition
                     except Exception:
                         conditions[d].append(-condition)
         return conditions
 
-    def predict_why(self, data: dict[str, float]):
-        cube = self._find_cube(data.copy())
+    def predict_why(self, data: dict[str, float], verbose=True):
+        cube = self._find_cube(data)
+        output = ""
         if cube is None:
-            print("The extracted knowledge is not exhaustive; impossible to predict this instance")
-        else:
-            output = self._predict_from_cubes(data)
-            print(f"The output is {output} because")
-            conditions = self.__get_local_conditions(data, cube)
-            for d in conditions:
-                for i, condition in enumerate(conditions[d]):
-                    if condition is None:
-                        continue
-                    elif i == 0:
-                        print('    ', d, 'is', end=' ')
-                    else:
-                        print('and', end=' ')
-                    print(condition.print(), end='')
-                    if i + 1 == len(conditions[d]):
-                        print()
+            output += "The extracted knowledge is not exhaustive; impossible to predict this instance\n"
+            if verbose:
+                print(output)
+            return None, {}
+        prediction = self._predict_from_cubes(data)
+        output += f"The output is {prediction} because\n"
+        conditions = {c: [val for val in v if val is not None and val.is_in(self.unscale(data[c], c))]
+                      for c, v in self.__get_conditions(data, cube).items()}
+
+        if verbose:
+            output += HyperCubeExtractor.__conditions_to_string(conditions)
+            print(output)
+
+        return prediction, conditions
 
     @staticmethod
     def _create_head(dataframe: pd.DataFrame, variables: list[Var], output: float | LinearRegression) -> Struct:
         return create_head(dataframe.columns[-1], variables[:-1], output) \
             if not isinstance(output, LinearRegression) else \
             create_head(dataframe.columns[-1], variables[:-1], variables[-1])
```

### Comparing `psyke-0.8.4/psyke/extraction/hypercubic/cosmik/__init__.py` & `psyke-0.8.5/psyke/extraction/hypercubic/cosmik/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.8.5/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                  ignore_threshold: float = 0.0, discretization=None, normalization=None,
                  seed: int = get_default_random_seed()):
         super().__init__(predictor, Target.CLASSIFICATION if isinstance(predictor, ClassifierMixin) else output,
                          discretization, normalization)
         self.clustering = clustering(depth, error_threshold, self._output, gauss_components, discretization,
                                      normalization, seed)
         self._default_surrounding_cube = True
-        self._dimensions_to_ignore = [dimension for dimension, relevance in ranks if relevance < ignore_threshold]
+        self._dimensions_to_ignore = set([dimension for dimension, relevance in ranks if relevance < ignore_threshold])
 
     def _extract(self, dataframe: pd.DataFrame) -> Theory:
         if not isinstance(self.clustering, HyperCubeClustering):
             raise TypeError("clustering must be a HyperCubeClustering")
 
         self.clustering.fit(dataframe)
         self._hypercubes = self.clustering.get_hypercubes()
```

### Comparing `psyke-0.8.4/psyke/extraction/hypercubic/divine/__init__.py` & `psyke-0.8.5/psyke/extraction/hypercubic/divine/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.8.5/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.8.5/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/hypercubic/hex/__init__.py` & `psyke-0.8.5/psyke/extraction/hypercubic/hex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.8.5/psyke/extraction/hypercubic/hypercube.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,16 +171,20 @@
     def error(self) -> float:
         return self._error
 
     @property
     def barycenter(self) -> Point:
         return self._barycenter
 
-    def subcubes(self, cubes: Iterable[GenericCube]) -> Iterable[GenericCube]:
-        return [c for c in cubes if c in self and c != self]
+    def subcubes(self, cubes: Iterable[GenericCube], only_largest: bool = True) -> Iterable[GenericCube]:
+        subcubes = [c for c in cubes if c in self and c.output != self.output]
+        if only_largest:
+            subsubcubes = [c for cube_list in [c.subcubes(cubes) for c in subcubes] for c in cube_list]
+            subcubes = [c for c in subcubes if c not in subsubcubes]
+        return subcubes
 
     def _fit_dimension(self, dimension: dict[str, tuple[float, float]]) -> dict[str, tuple[float, float]]:
         new_dimension: dict[str, tuple[float, float]] = {}
         for key, value in dimension.items():
             new_dimension[key] = (round(value[0], self.INT_PRECISION), round(value[1], self.INT_PRECISION))
         return new_dimension
```

### Comparing `psyke-0.8.4/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.8.5/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/hypercubic/strategy.py` & `psyke-0.8.5/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/hypercubic/utils.py` & `psyke-0.8.5/psyke/extraction/hypercubic/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/real/__init__.py` & `psyke-0.8.5/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/real/utils.py` & `psyke-0.8.5/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/trepan/__init__.py` & `psyke-0.8.5/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/extraction/trepan/utils.py` & `psyke-0.8.5/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/hypercubepredictor.py` & `psyke-0.8.5/psyke/hypercubepredictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,18 @@
             return None
         elif self._output == Target.CLASSIFICATION:
             return HyperCubePredictor._get_cube_output(cube, data)
         else:
             return round(HyperCubePredictor._get_cube_output(cube, data), get_int_precision())
 
     def _find_cube(self, data: dict[str, float]) -> GenericCube | None:
+        data = data.copy()
         for dimension in self._dimensions_to_ignore:
-            del data[dimension]
+            if dimension in data:
+                del data[dimension]
         for cube in self._hypercubes:
             if data in cube:
                 return cube.copy()
         if self._hypercubes[-1].is_default:
             return self._hypercubes[-1].copy()
 
     @property
```

### Comparing `psyke-0.8.4/psyke/schema/__init__.py` & `psyke-0.8.5/psyke/schema/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 import math
 from typing import Callable
 from psyke.utils import get_int_precision
 
 _EMPTY_INTERSECTION_EXCEPTION: Callable = lambda x, y: \
-    Exception("Empty intersection between two Value: " + str(x) + ' and ' + str(y))
+    Exception(f"Empty intersection between two Value: {str(x)} and {str(y)}")
 
 _NOT_IMPLEMENTED_INTERSECTION: Callable = lambda x, y: \
     Exception("Not implemented intersection between: " + str(x) + ' and ' + str(y))
 
 _INTERSECTION_WITH_WRONG_TYPE: Callable = lambda x, y: \
     Exception("Calling method with wrong type argument: " + str(x) + ' and ' + str(y))
 
@@ -246,14 +246,17 @@
         elif isinstance(self, LessThan):
             return intersection_with_less_than(self, other)
         elif isinstance(self, GreaterThan):
             return intersection_with_greater_than(self, other)
         else:
             raise _INTERSECTION_WITH_WRONG_TYPE(self, other)
 
+    def print(self) -> str:
+        pass
+
 
 class Interval(Value):
 
     def __init__(self, lower: float, upper: float, standard: bool = True):
         super().__init__()
         self.standard = standard
         self.lower = round(lower, PRECISION)
@@ -261,15 +264,15 @@
 
     def __str__(self):
         return f"[{self.lower:.2f}, {self.upper:.2f}]"
 
     def __repr__(self):
         return f"Interval({self.lower:.2f}, {self.upper:.2f})"
 
-    def __eq__(self, other: Between) -> bool:
+    def __eq__(self, other: Interval) -> bool:
         return (self.upper == other.upper) and (self.lower == other.lower) and (self.standard == other.standard)
 
 
 class LessThan(Interval):
 
     def __init__(self, value: float, standard: bool = True):
         super().__init__(-math.inf, value, standard)
@@ -287,15 +290,16 @@
     def __str__(self):
         return f"]-∞, {self.upper:.2f}" + ("]" if self.standard else "[")
 
     def __repr__(self):
         return f"LessThan({self.upper:.2f})"
 
     def __eq__(self, other: LessThan) -> bool:
-        return (self.upper == other.upper) and (self.value == other.value) and (self.standard == other.standard)
+        return isinstance(other, LessThan) and (self.upper == other.upper) and \
+               (self.value == other.value) and (self.standard == other.standard)
 
 
 class GreaterThan(Interval):
 
     def __init__(self, value: float, standard: bool = True):
         super().__init__(value, math.inf, standard)
 
@@ -312,15 +316,16 @@
     def __str__(self):
         return ("]" if self.standard else "[") + f"{self.lower:.2f}, ∞["
 
     def __repr__(self):
         return f"GreaterThan({self.lower:.2f})"
 
     def __eq__(self, other: GreaterThan) -> bool:
-        return (self.lower == other.lower) and (self.value == other.value) and (self.standard == other.standard)
+        return isinstance(other, GreaterThan) and (self.lower == other.lower) and \
+               (self.value == other.value) and (self.standard == other.standard)
 
 
 class Between(Interval):
 
     def __init__(self, lowerbound: float, upperbound: float, standard: bool = True):
         super().__init__(lowerbound, upperbound, standard)
```

### Comparing `psyke-0.8.4/psyke/tuning/__init__.py` & `psyke-0.8.5/psyke/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/tuning/crash/__init__.py` & `psyke-0.8.5/psyke/tuning/crash/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/tuning/orchid/__init__.py` & `psyke-0.8.5/psyke/tuning/orchid/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/tuning/pedro/__init__.py` & `psyke-0.8.5/psyke/tuning/pedro/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/utils/__init__.py` & `psyke-0.8.5/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/utils/dataframe.py` & `psyke-0.8.5/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/utils/logic.py` & `psyke-0.8.5/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/utils/metrics.py` & `psyke-0.8.5/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/utils/plot.py` & `psyke-0.8.5/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke/utils/sorted.py` & `psyke-0.8.5/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/psyke.egg-info/PKG-INFO` & `psyke-0.8.5/psyke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.4
+Version: 0.8.5
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.4/psyke.egg-info/SOURCES.txt` & `psyke-0.8.5/psyke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/setup.py` & `psyke-0.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/__init__.py` & `psyke-0.8.5/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/extraction/cart/test_cart.py` & `psyke-0.8.5/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.8.5/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.8.5/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.8.5/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.8.5/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/extraction/real/test_real.py` & `psyke-0.8.5/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/extraction/real/test_rule.py` & `psyke-0.8.5/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/extraction/trepan/test_node.py` & `psyke-0.8.5/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/extraction/trepan/test_split.py` & `psyke-0.8.5/test/psyke/extraction/trepan/test_split.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.8.5/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/utils/test_prune.py` & `psyke-0.8.5/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/utils/test_simplify.py` & `psyke-0.8.5/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.8.5/test/psyke/utils/test_simplify_formatter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.4/test/resources/tests/__init__.py` & `psyke-0.8.5/test/resources/tests/__init__.py`

 * *Files identical despite different names*

