# Comparing `tmp/ts3l-0.30.tar.gz` & `tmp/ts3l-0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts3l-0.30.tar", last modified: Mon Apr 22 05:18:57 2024, max compression
+gzip compressed data, was "ts3l-0.40.tar", last modified: Thu May  2 05:42:34 2024, max compression
```

## Comparing `ts3l-0.30.tar` & `ts3l-0.40.tar`

### file list

```diff
@@ -1,68 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 05:18:49.000000 ts3l-0.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-04-22 05:18:57.393371 ts3l-0.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-22 05:18:49.000000 ts3l-0.30/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 05:18:57.393371 ts3l-0.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-22 05:18:49.000000 ts3l-0.30/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.385371 ts3l-0.30/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-22 05:18:49.000000 ts3l-0.30/test/test_dae.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-22 05:18:49.000000 ts3l-0.30/test/test_scarf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-22 05:18:49.000000 ts3l-0.30/test/test_subtab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-22 05:18:49.000000 ts3l-0.30/test/test_vime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.385371 ts3l-0.30/ts3l/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/common/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/common/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/dae/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/dae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/dae/dae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/scarf/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/scarf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/scarf/scarf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/subtab/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/subtab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/subtab/subtab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/vime/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/vime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/vime/vime.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/vime/vime_self.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/vime/vime_semi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/pl_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/base_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/dae_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/scarf_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/subtab_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/vime_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/base_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l/utils/dae_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/dae_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/dae_utils/dae_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/dae_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l/utils/scarf_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/scarf_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/scarf_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/scarf_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/scarf_utils/scarf_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l/utils/subtab_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/subtab_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/subtab_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/subtab_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/subtab_utils/subtab_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l/utils/vime_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/vime_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/vime_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/vime_utils/vime_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-04-22 05:18:57.000000 ts3l-0.30/ts3l.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-22 05:18:57.000000 ts3l-0.30/ts3l.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:18:57.000000 ts3l-0.30/ts3l.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 05:18:57.000000 ts3l-0.30/ts3l.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 05:18:57.000000 ts3l-0.30/ts3l.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 05:42:25.000000 ts3l-0.40/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21158 2024-05-02 05:42:34.098232 ts3l-0.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20542 2024-05-02 05:42:25.000000 ts3l-0.40/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 05:42:34.098232 ts3l-0.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-02 05:42:25.000000 ts3l-0.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.090232 ts3l-0.40/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-02 05:42:25.000000 ts3l-0.40/test/test_dae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-02 05:42:25.000000 ts3l-0.40/test/test_scarf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-02 05:42:25.000000 ts3l-0.40/test/test_subtab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-02 05:42:25.000000 ts3l-0.40/test/test_switchtab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-02 05:42:25.000000 ts3l-0.40/test/test_vime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.090232 ts3l-0.40/ts3l/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.090232 ts3l-0.40/ts3l/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.090232 ts3l-0.40/ts3l/models/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/common/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/common/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/models/dae/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/dae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/dae/dae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/models/scarf/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/scarf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/scarf/scarf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/models/subtab/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/subtab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/subtab/subtab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/models/switchtab/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/switchtab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/switchtab/ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/switchtab/switchtab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/models/vime/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/vime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/vime/vime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/vime/vime_self.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/vime/vime_semi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/pl_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/dae_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/scarf_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/subtab_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/switchtab_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/vime_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/base_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l/utils/dae_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/dae_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/dae_utils/dae_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/dae_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l/utils/scarf_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/scarf_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/scarf_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/scarf_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/scarf_utils/scarf_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l/utils/subtab_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/subtab_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/subtab_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/subtab_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/subtab_utils/subtab_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l/utils/switchtab_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/switchtab_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/switchtab_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/switchtab_utils/switchtab_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l/utils/vime_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/vime_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/vime_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/vime_utils/vime_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21158 2024-05-02 05:42:34.000000 ts3l-0.40/ts3l.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-02 05:42:34.000000 ts3l-0.40/ts3l.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 05:42:34.000000 ts3l-0.40/ts3l.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 05:42:34.000000 ts3l-0.40/ts3l.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 05:42:34.000000 ts3l-0.40/ts3l.egg-info/top_level.txt
```

### Comparing `ts3l-0.30/LICENSE` & `ts3l-0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/PKG-INFO` & `ts3l-0.40/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ts3l
-Version: 0.30
+Version: 0.40
 Summary: A PyTorch Lightning-based library for self- and semi-supervised learning on tabular data.
 Home-page: https://github.com/Alcoholrithm/TabularS3L
 Author: Minwook Kim
 Author-email: kmiiiaa@pusan.ac.kr
-Keywords: tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF DenoisingAutoEncoder
+Keywords: tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF Denoising-AutoEncoder SwitchTab
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: torch
@@ -20,18 +20,18 @@
 
 [**Overview**](#tabulars3l)
 | [**Installation**](#installation)
 | [**Available Models with Quick Start Guides**](#available-models-with-quick-start)
 | [**Benchmark**](#benchmark)
 | [**To DO**](#to-do)
 | [**Contributing**](#contributing)
-| [**Credit**](#credit)
 
 
 [![pypi](https://img.shields.io/pypi/v/ts3l)](https://pypi.org/project/ts3l/0.20/)
+[![Downloads](https://static.pepy.tech/badge/ts3l)](https://pepy.tech/project/ts3l)
 [![DOI](https://zenodo.org/badge/756740921.svg)](https://zenodo.org/doi/10.5281/zenodo.10776537)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 TabularS3L is a PyTorch Lightning-based library designed to facilitate self- and semi-supervised learning with tabular data. While numerous self- and semi-supervised learning tabular models have been proposed, there is a lack of a comprehensive library that addresses the needs of tabular practitioners. This library aims to fill this gap by providing a unified PyTorch Lightning-based framework for exploring and deploying such models.
 
 ## Installation
 We provide a Python package ts3l of TabularS3L for users who want to use semi- and self-supervised learning tabular models.
@@ -46,14 +46,15 @@
 
 | Model | First Phase | Second Phase |
 |:---:|:---:|:---:|
 | **DAE** ([GitHub](https://github.com/ryancheunggit/tabular_dae))| Self-SL | SL |
 | **VIME** ([NeurIPS'20](https://proceedings.neurips.cc/paper/2020/hash/7d97667a3e056acab9aaf653807b4a03-Abstract.html)) | Self-SL | Semi-SL or SL |
 | **SubTab** ([NeurIPS'21](https://proceedings.neurips.cc/paper/2021/hash/9c8661befae6dbcd08304dbf4dcaf0db-Abstract.html)) | Self-SL | SL |
 | **SCARF** ([ICLR'22](https://iclr.cc/virtual/2022/spotlight/6297))| Self-SL | SL |
+| **SwitchTab** ([AAAI'24](https://ojs.aaai.org/index.php/AAAI/article/view/29523)) | Self-SL | SL |
 
 #### Denoising AutoEncoder (DAE)
 DAE processes input data that has been partially corrupted, producing clean data and predicting which features are corrupted during the self-supervised learning.
 The denoising task enables the model to learn the input distribution and generate latent representations that are robust to corruption. 
 These latent representations can be utilized for a variety of downstream tasks.
 
 <details close>
@@ -400,14 +401,103 @@
   accuracy = accuracy_score(y_test, preds.argmax(1))
 
   print("Accuracy %.2f" % accuracy)
   ```
 
 </details>
 
+#### SwitchTab: Switched Autoencoders Are Effective Tabular Learners
+SwitchTab introduces a novel self-supervised method specifically designed to decuple mutual and salient features among data pair, resulting in more representative embeddings.
+Moreover, the pre-trained salient embeddings can be utilized as plug-and-play features to enhance the performance of various traditional classification methods.
+
+<details close>
+  <summary>Quick Start</summary>
+  
+  ```python
+  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
+
+  # Prepare the SwitchTabLightning Module
+  from ts3l.pl_modules import SwitchTabLightning
+  from ts3l.utils.switchtab_utils import SwitchTabDataset, SwitchTabFirstPhaseCollateFN
+  from ts3l.utils import TS3LDataModule
+  from ts3l.utils.switchtab_utils import SwitchTabConfig
+  from pytorch_lightning import Trainer
+
+  metric = "accuracy_score"
+  input_dim = X_train.shape[1]
+  hidden_dim = 1024
+  output_dim = 2
+
+  encoder_depth = 3
+  n_head = 2
+  u_label = -1
+
+  batch_size = 128
+
+  X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
+
+  config = SwitchTabConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
+  input_dim=input_dim, hidden_dim=hidden_dim,
+  output_dim=output_dim, encoder_depth=encoder_depth,
+  n_head = n_head,
+  u_label = u_label
+  )
+
+  pl_switchtab = SwitchTabLightning(config)
+
+  ### First Phase Learning
+  train_ds = SwitchTabDataset(X = X_train, unlabeled_data = X_unlabeled, Y = y_train.values, config=config, continuous_cols=continuous_cols, category_cols=category_cols)
+  valid_ds = SwitchTabDataset(X = X_valid, config=config, Y = y_valid.values, continuous_cols=continuous_cols, category_cols=category_cols)
+
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='weighted', train_collate_fn=SwitchTabFirstPhaseCollateFN(), valid_collate_fn=SwitchTabFirstPhaseCollateFN())
+
+  trainer = Trainer(
+                  accelerator = 'cpu',
+                  max_epochs = 20,
+                  num_sanity_val_steps = 2,
+  )
+
+  trainer.fit(pl_switchtab, datamodule)
+
+  ### Second Phase Learning
+
+  pl_switchtab.set_second_phase()
+
+  train_ds = SwitchTabDataset(X = X_train, Y = y_train.values, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  valid_ds = SwitchTabDataset(X = X_valid, Y = y_valid.values, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+      
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted")
+
+  trainer = Trainer(
+                  accelerator = 'cpu',
+                  max_epochs = 20,
+                  num_sanity_val_steps = 2,
+  )
+
+  trainer.fit(pl_switchtab, datamodule)
+
+  # Evaluation
+  from sklearn.metrics import accuracy_score
+  import torch
+  from torch.nn import functional as F
+  from torch.utils.data import DataLoader, SequentialSampler
+
+  test_ds = SwitchTabDataset(X_test, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds))
+
+  preds = trainer.predict(pl_switchtab, test_dl)
+      
+  preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
+
+  accuracy = accuracy_score(y_test, preds.argmax(1))
+
+  print("Accuracy %.2f" % accuracy)
+  ```
+
+</details>
 
 ## Benchmark
 
 We provide a simple benchmark using TabularS3L against XGBoost. The train-validation-test ratio is 6:2:2 and we tuned each model over 50 trials using Optuna. The results are the average of the random seeds [0,4]. The best results are bold. 'acc', 'b-acc', and 'mse' mean 'Accuracy', 'Balanced Accuracy', and 'Mean Squared Error', respectively.
 
 Use this benchmark for reference only, as only a small number of random seeds were used.
 
@@ -415,58 +505,36 @@
 
 | Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
 |:---:|:---:|:---:|:---:|
 | XGBoost | 0.7325 | 0.4763 | **5.5739** |
 | DAE | 0.7208 | 0.4885 | 5.6168 | 
 | VIME | 0.7182 | **0.5087** | 5.6637 |
 | SubTab | 0.7312 | 0.4930 | 7.2418 |
-| SCARF | **0.7416** | 0.4710 | 5.8888 | 
+| SCARF | **0.7416** | 0.4710 | 5.8888 |
+| SwitchTab |  0.7156 | 0.4886 | 5.9907 |
 
 --------
 
 ##### 100% labeled samples
 
 | Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
 |:---:|:---:|:---:|:---:|
 | XGBoost | 0.7234 | 0.5291 | 4.8377 |
 | DAE | 0.7390 | 0.5500 | 4.5758 |
 | VIME | **0.7688** | 0.5477 | 4.5804 |
 | SubTab | 0.7390 | 0.5432 | 6.3104 |
 | SCARF | 0.7442 | **0.5521** | **4.4443** |
+| SwitchTab | 0.7585 | 0.5411 | 4.7489 |
 
 ## To DO
 
 - [x] Release nn.Module and Dataset of VIME, SubTab, and SCARF
-  - [x] VIME
-  - [x] SubTab
-  - [x] SCARF
 - [x] Release LightningModules of VIME, SubTab, and SCARF
-  - [x] VIME
-  - [x] SubTab
-  - [x] SCARF
 - [x] Release Denoising AutoEncoder
-  - [x] nn.Module
-  - [x] LightningModule
-- [ ] Release SwitchTab
-  - [ ] nn.Module
-  - [ ] LightningModule
+- [x] Release SwitchTab
 - [x] Add example codes
+- [ ] Release more tabular models
 
 ## Contributing
 
 Contributions to this implementation are highly appreciated. Whether it's suggesting improvements, reporting bugs, or proposing new features, feel free to open an issue or submit a pull request.
 
-
-## Credit  
-```
-@software{alcoholrithm_2024_10776538,
-  author       = {Minwook Kim},
-  title        = {TabularS3L},
-  month        = mar,
-  year         = 2024,
-  publisher    = {Zenodo},
-  version      = {v0.21},
-  doi          = {10.5281/zenodo.10776538},
-  url          = {https://doi.org/10.5281/zenodo.10776538}
-}
-```
-
```

### Comparing `ts3l-0.30/README.md` & `ts3l-0.40/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 [**Overview**](#tabulars3l)
 | [**Installation**](#installation)
 | [**Available Models with Quick Start Guides**](#available-models-with-quick-start)
 | [**Benchmark**](#benchmark)
 | [**To DO**](#to-do)
 | [**Contributing**](#contributing)
-| [**Credit**](#credit)
 
 
 [![pypi](https://img.shields.io/pypi/v/ts3l)](https://pypi.org/project/ts3l/0.20/)
+[![Downloads](https://static.pepy.tech/badge/ts3l)](https://pepy.tech/project/ts3l)
 [![DOI](https://zenodo.org/badge/756740921.svg)](https://zenodo.org/doi/10.5281/zenodo.10776537)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 TabularS3L is a PyTorch Lightning-based library designed to facilitate self- and semi-supervised learning with tabular data. While numerous self- and semi-supervised learning tabular models have been proposed, there is a lack of a comprehensive library that addresses the needs of tabular practitioners. This library aims to fill this gap by providing a unified PyTorch Lightning-based framework for exploring and deploying such models.
 
 ## Installation
 We provide a Python package ts3l of TabularS3L for users who want to use semi- and self-supervised learning tabular models.
@@ -28,14 +28,15 @@
 
 | Model | First Phase | Second Phase |
 |:---:|:---:|:---:|
 | **DAE** ([GitHub](https://github.com/ryancheunggit/tabular_dae))| Self-SL | SL |
 | **VIME** ([NeurIPS'20](https://proceedings.neurips.cc/paper/2020/hash/7d97667a3e056acab9aaf653807b4a03-Abstract.html)) | Self-SL | Semi-SL or SL |
 | **SubTab** ([NeurIPS'21](https://proceedings.neurips.cc/paper/2021/hash/9c8661befae6dbcd08304dbf4dcaf0db-Abstract.html)) | Self-SL | SL |
 | **SCARF** ([ICLR'22](https://iclr.cc/virtual/2022/spotlight/6297))| Self-SL | SL |
+| **SwitchTab** ([AAAI'24](https://ojs.aaai.org/index.php/AAAI/article/view/29523)) | Self-SL | SL |
 
 #### Denoising AutoEncoder (DAE)
 DAE processes input data that has been partially corrupted, producing clean data and predicting which features are corrupted during the self-supervised learning.
 The denoising task enables the model to learn the input distribution and generate latent representations that are robust to corruption. 
 These latent representations can be utilized for a variety of downstream tasks.
 
 <details close>
@@ -382,14 +383,103 @@
   accuracy = accuracy_score(y_test, preds.argmax(1))
 
   print("Accuracy %.2f" % accuracy)
   ```
 
 </details>
 
+#### SwitchTab: Switched Autoencoders Are Effective Tabular Learners
+SwitchTab introduces a novel self-supervised method specifically designed to decuple mutual and salient features among data pair, resulting in more representative embeddings.
+Moreover, the pre-trained salient embeddings can be utilized as plug-and-play features to enhance the performance of various traditional classification methods.
+
+<details close>
+  <summary>Quick Start</summary>
+  
+  ```python
+  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
+
+  # Prepare the SwitchTabLightning Module
+  from ts3l.pl_modules import SwitchTabLightning
+  from ts3l.utils.switchtab_utils import SwitchTabDataset, SwitchTabFirstPhaseCollateFN
+  from ts3l.utils import TS3LDataModule
+  from ts3l.utils.switchtab_utils import SwitchTabConfig
+  from pytorch_lightning import Trainer
+
+  metric = "accuracy_score"
+  input_dim = X_train.shape[1]
+  hidden_dim = 1024
+  output_dim = 2
+
+  encoder_depth = 3
+  n_head = 2
+  u_label = -1
+
+  batch_size = 128
+
+  X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
+
+  config = SwitchTabConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
+  input_dim=input_dim, hidden_dim=hidden_dim,
+  output_dim=output_dim, encoder_depth=encoder_depth,
+  n_head = n_head,
+  u_label = u_label
+  )
+
+  pl_switchtab = SwitchTabLightning(config)
+
+  ### First Phase Learning
+  train_ds = SwitchTabDataset(X = X_train, unlabeled_data = X_unlabeled, Y = y_train.values, config=config, continuous_cols=continuous_cols, category_cols=category_cols)
+  valid_ds = SwitchTabDataset(X = X_valid, config=config, Y = y_valid.values, continuous_cols=continuous_cols, category_cols=category_cols)
+
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='weighted', train_collate_fn=SwitchTabFirstPhaseCollateFN(), valid_collate_fn=SwitchTabFirstPhaseCollateFN())
+
+  trainer = Trainer(
+                  accelerator = 'cpu',
+                  max_epochs = 20,
+                  num_sanity_val_steps = 2,
+  )
+
+  trainer.fit(pl_switchtab, datamodule)
+
+  ### Second Phase Learning
+
+  pl_switchtab.set_second_phase()
+
+  train_ds = SwitchTabDataset(X = X_train, Y = y_train.values, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  valid_ds = SwitchTabDataset(X = X_valid, Y = y_valid.values, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+      
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted")
+
+  trainer = Trainer(
+                  accelerator = 'cpu',
+                  max_epochs = 20,
+                  num_sanity_val_steps = 2,
+  )
+
+  trainer.fit(pl_switchtab, datamodule)
+
+  # Evaluation
+  from sklearn.metrics import accuracy_score
+  import torch
+  from torch.nn import functional as F
+  from torch.utils.data import DataLoader, SequentialSampler
+
+  test_ds = SwitchTabDataset(X_test, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds))
+
+  preds = trainer.predict(pl_switchtab, test_dl)
+      
+  preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
+
+  accuracy = accuracy_score(y_test, preds.argmax(1))
+
+  print("Accuracy %.2f" % accuracy)
+  ```
+
+</details>
 
 ## Benchmark
 
 We provide a simple benchmark using TabularS3L against XGBoost. The train-validation-test ratio is 6:2:2 and we tuned each model over 50 trials using Optuna. The results are the average of the random seeds [0,4]. The best results are bold. 'acc', 'b-acc', and 'mse' mean 'Accuracy', 'Balanced Accuracy', and 'Mean Squared Error', respectively.
 
 Use this benchmark for reference only, as only a small number of random seeds were used.
 
@@ -397,58 +487,36 @@
 
 | Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
 |:---:|:---:|:---:|:---:|
 | XGBoost | 0.7325 | 0.4763 | **5.5739** |
 | DAE | 0.7208 | 0.4885 | 5.6168 | 
 | VIME | 0.7182 | **0.5087** | 5.6637 |
 | SubTab | 0.7312 | 0.4930 | 7.2418 |
-| SCARF | **0.7416** | 0.4710 | 5.8888 | 
+| SCARF | **0.7416** | 0.4710 | 5.8888 |
+| SwitchTab |  0.7156 | 0.4886 | 5.9907 |
 
 --------
 
 ##### 100% labeled samples
 
 | Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
 |:---:|:---:|:---:|:---:|
 | XGBoost | 0.7234 | 0.5291 | 4.8377 |
 | DAE | 0.7390 | 0.5500 | 4.5758 |
 | VIME | **0.7688** | 0.5477 | 4.5804 |
 | SubTab | 0.7390 | 0.5432 | 6.3104 |
 | SCARF | 0.7442 | **0.5521** | **4.4443** |
+| SwitchTab | 0.7585 | 0.5411 | 4.7489 |
 
 ## To DO
 
 - [x] Release nn.Module and Dataset of VIME, SubTab, and SCARF
-  - [x] VIME
-  - [x] SubTab
-  - [x] SCARF
 - [x] Release LightningModules of VIME, SubTab, and SCARF
-  - [x] VIME
-  - [x] SubTab
-  - [x] SCARF
 - [x] Release Denoising AutoEncoder
-  - [x] nn.Module
-  - [x] LightningModule
-- [ ] Release SwitchTab
-  - [ ] nn.Module
-  - [ ] LightningModule
+- [x] Release SwitchTab
 - [x] Add example codes
+- [ ] Release more tabular models
 
 ## Contributing
 
 Contributions to this implementation are highly appreciated. Whether it's suggesting improvements, reporting bugs, or proposing new features, feel free to open an issue or submit a pull request.
 
-
-## Credit  
-```
-@software{alcoholrithm_2024_10776538,
-  author       = {Minwook Kim},
-  title        = {TabularS3L},
-  month        = mar,
-  year         = 2024,
-  publisher    = {Zenodo},
-  version      = {v0.21},
-  doi          = {10.5281/zenodo.10776538},
-  url          = {https://doi.org/10.5281/zenodo.10776538}
-}
-```
-
```

### Comparing `ts3l-0.30/setup.py` & `ts3l-0.40/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,24 +22,24 @@
         str(requirement)
         for requirement
         in pkg_resources.parse_requirements(requirements_txt)
     ]
 
 setup(
     name='ts3l',
-    version='v0.30',
+    version='v0.40',
     description='A PyTorch Lightning-based library for self- and semi-supervised learning on tabular data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Alcoholrithm/TabularS3L',
     author='Minwook Kim',
     author_email='kmiiiaa@pusan.ac.kr',
 
     # Note that this is a string of words separated by whitespace, not a list.
-    keywords='tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF DenoisingAutoEncoder',
+    keywords='tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF Denoising-AutoEncoder SwitchTab',
     packages=find_packages(),
     # The `include_package_data` parameter in the `setup()` function is used to specify whether to
     # include non-Python files (such as data files, configuration files, etc.) that are part of the
     # package when it is installed.
     include_package_data=False,
     install_requires=install_requires,
     python_requires='>=3.7',
```

### Comparing `ts3l-0.30/test/test_dae.py` & `ts3l-0.40/test/test_dae.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/test/test_scarf.py` & `ts3l-0.40/test/test_scarf.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/test/test_subtab.py` & `ts3l-0.40/test/test_subtab.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/test/test_vime.py` & `ts3l-0.40/test/test_vime.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/models/dae/dae.py` & `ts3l-0.40/ts3l/models/scarf/scarf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,74 @@
 from numpy.typing import NDArray
+from typing import OrderedDict
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.distributions.uniform import Uniform
 
 import numpy as np
-
 from ts3l.models.common import MLP
 
 
-class DAE(nn.Module):
+class SCARF(nn.Module):
     def __init__(
         self,
         input_dim,
         hidden_dim,
+        output_dim,
         encoder_depth=4,
         head_depth=2,
         dropout_rate = 0.04,
-        output_dim = 2,
     ):
-        """Implementation of Denoising AutoEncoder.
-        DAE processes input data that has been partially corrupted, producing clean data during the self-supervised learning stage. 
-        The denoising task enables the model to learn the input distribution and generate latent representations that are robust to corruption. 
-        These latent representations can be utilized for a variety of downstream tasks.
-        Args:
-            input_dim (int): The size of the inputs
-            hidden_dim (int): The dimension of the hidden layers
-            encoder_depth (int, optional): The number of layers of the encoder MLP. Defaults to 4.
-            head_depth (int, optional): The number of layers of the pretraining head. Defaults to 2.
-            dropout_rate (float, optional): The probability of setting the outputs of the dropout layer to zero during training. Defaults to 0.04.
-            output_dim (int, 2): The size of the outputs
+        """Implementation of SCARF: Self-Supervised Contrastive Learning using Random Feature Corruption.
+        It consists in an encoder that learns the embeddings.
+        It is done by minimizing the contrastive loss of a sample and a corrupted view of it.
+        The corrupted view is built by replacing a random set of features by another sample randomly drawn independently.
+            Args:
+                input_dim (int): The size of the inputs.
+                hidden_dim (int): The dimension of the hidden layers.
+                output_dim (int): The dimension of output.
+                encoder_depth (int, optional): The number of layers of the encoder MLP. Defaults to 4.
+                head_depth (int, optional): The number of layers of the pretraining head. Defaults to 2.
+                dropout_rate (float, optional): A hyperparameter that is to control dropout layer. Default is 0.04.
         """
         super().__init__()
 
-        self.encoder = MLP(input_dim, hidden_dim, encoder_depth, dropout_rate)
-        self.mask_predictor_head = MLP(hidden_dim, input_dim, head_depth, dropout_rate)
-        self.reconstruction_head = MLP(hidden_dim, input_dim, head_depth, dropout_rate)
+        self.encoder = MLP(input_dim, hidden_dim, encoder_depth)
+
+        self.pretraining_head = MLP(hidden_dim, hidden_dim, head_depth)
 
         self.head = nn.Sequential(
-            nn.ReLU(inplace=True),
-            nn.BatchNorm1d(hidden_dim),
-            nn.Dropout(dropout_rate),
-            nn.Linear(hidden_dim, output_dim)
+            OrderedDict([
+                ("head_activation", nn.ReLU(inplace=True)),
+                ("head_batchnorm", nn.BatchNorm1d(hidden_dim)),
+                ("head_dropout", nn.Dropout(dropout_rate)),
+                ("head_linear", nn.Linear(hidden_dim, output_dim))
+            ])
         )
-        # initialize weights
-        self.encoder.apply(self._init_weights)
-        self.mask_predictor_head.apply(self._init_weights)
-        self.reconstruction_head.apply(self._init_weights)
-        
 
-    
-    def _init_weights(self, module):
-        if isinstance(module, nn.Linear):
-            torch.nn.init.xavier_uniform_(module.weight)
-            module.bias.data.fill_(0.01)
             
     def set_first_phase(self):
         self.forward = self.__first_phase_step
     
     def set_second_phase(self):
         self.forward = self.__second_phase_step
 
-    def __first_phase_step(self, x):
+    def __first_phase_step(self, x, x_corrupted):
 
-        emb = self.encoder(x)
-        mask = torch.sigmoid(self.mask_predictor_head(emb))
-        feature = self.reconstruction_head(emb)
+        emb_anchor = self.encoder(x)
+        emb_anchor = self.pretraining_head(emb_anchor)
+
+        emb_anchor = F.normalize(emb_anchor, p=2)
+        
+        emb_corrupted = self.encoder(x_corrupted)
+        emb_corrupted = self.pretraining_head(emb_corrupted)
+        emb_corrupted = F.normalize(emb_corrupted, p=2)
 
-        return mask, feature
+        return emb_anchor, emb_corrupted
     
     def __second_phase_step(self, x):
         emb = self.encoder(x)
         output = self.head(emb)
+
         return output
```

### Comparing `ts3l-0.30/ts3l/models/subtab/subtab.py` & `ts3l-0.40/ts3l/models/subtab/subtab.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/models/vime/vime.py` & `ts3l-0.40/ts3l/models/vime/vime.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Tuple
+
+import torch
 import torch.nn as nn
 
 from .vime_self import VIMESelfSupervised
 from .vime_semi import VIMESemiSupervised
 
 class VIME(nn.Module):
     def __init__(self, 
@@ -26,23 +29,22 @@
         self.forward = self.__first_phase_step
     
     def set_second_phase(self):
         """Set second phase step as the forward pass
         """
         self.forward = self.__second_phase_step
         
-    def __first_phase_step(self, x):
+    def __first_phase_step(self, x: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
         """The first phase step of VIME
 
         Args:
-            x (torch.FloatTensor): The input batch
+            x (torch.Tensor): The input batch
 
         Returns:
-            torch.FloatTensor: The predicted mask vector of VIME
-            torch.FloatTensor: The predicted features of VIME
+            Tuple[torch.Tensor, torch.Tensor]: The predicted mask vector and predicted features
         """
         mask_output, feature_output = self.self_net(x)
         return mask_output, feature_output
     
     
     def __second_phase_step(self, x):
         """The second phase step of VIME
```

### Comparing `ts3l-0.30/ts3l/models/vime/vime_self.py` & `ts3l-0.40/ts3l/models/vime/vime_self.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/models/vime/vime_semi.py` & `ts3l-0.40/ts3l/models/vime/vime_semi.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/pl_modules/base_module.py` & `ts3l-0.40/ts3l/pl_modules/base_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Type
 from ts3l.utils import RegressionMetric, ClassificationMetric
 
 from abc import ABC, abstractmethod
 
 import torch
 from torch import nn
 
 import pytorch_lightning as pl
 
 from dataclasses import asdict
 from ts3l.utils import BaseConfig
-    
+from ts3l.models.common import initialize_weights
 
     
 class TS3LLightining(ABC, pl.LightningModule):
     """The pytorch lightning module of TabularS3L
     """
     def __init__(self, config: BaseConfig) -> None:
         """Initialize the pytorch lightining module of TabularS3L
@@ -59,14 +59,21 @@
         
         self.save_hyperparameters()
     
     @abstractmethod
     def _initialize(self, config: Dict[str, Any]) -> None:
         pass
     
+    def _init_model(self, model_class: Type[nn.Module], config: Dict[str, Any]) -> None:
+        initialization = config["initialization"]
+        del config["initialization"]
+        
+        self.model = model_class(**config)
+        initialize_weights(self.model, initialization)
+        
     def __configure_metric(self, task, metric, metric_hparams):
         
         if task == "regression":
             self.metric = RegressionMetric(metric, metric_hparams)
         else:
             self.metric = ClassificationMetric(metric, metric_hparams)
             
@@ -120,21 +127,21 @@
 
         Returns:
             torch.FloatTensor: The final loss of first phase step
         """
         pass
     
     def _first_phase_step(self,
-                      batch,
+                      batch: Any,
                       batch_idx: int
     ) -> Dict[str, Any]:
         """The first phase step of TabularS3L
 
         Args:
-            batch (Dict[str, Any]): The input batch
+            batch (Any): The input batch
             batch_idx (int): Only for compatibility
 
         Returns:
             Dict[str, Any]: The loss of the first phase step
         """
 
         loss = self._get_first_phase_loss(batch)
@@ -162,36 +169,36 @@
         val_loss = torch.Tensor([out["loss"] for out in self.first_phase_step_outputs]).cpu().mean()
 
         self.log("val_loss", val_loss, prog_bar = True)
         self.first_phase_step_outputs = []
         return super().on_validation_epoch_end()
 
     @abstractmethod
-    def _get_second_phase_loss(self, batch:Dict[str, Any]):
+    def _get_second_phase_loss(self, batch: Any):
         """Calculate the second phase loss
 
         Args:
-            batch (Dict[str, Any]): The input batch
+            batch (Any): The input batch
 
         Returns:
             torch.FloatTensor: The final loss of second phase step
             torch.Tensor: The label of the labeled data
             torch.Tensor: The predicted label of the labeled data
         """
         pass
         
     
     def _second_phase_step(self,
-                      batch,
+                      batch: Any,
                       batch_idx: int = 0
     ) -> Dict[str, Any]:
         """The second phase step of TabularS3L
 
         Args:
-            batch (Dict[str, Any]): The input batch
+            batch (Any): The input batch
             batch_idx (int): Only for compatibility
 
         Returns:
             Dict[str, Any]: The loss of the second phase step
         """
         loss, y, y_hat = self._get_second_phase_loss(batch)
 
@@ -234,19 +241,19 @@
 
         self.log("val_" + self.metric.__name__, val_score, prog_bar = True)
         self.log("val_loss", val_loss, prog_bar = True)
         self.second_phase_step_outputs = []      
         return super().on_validation_epoch_end()
     
     @abstractmethod
-    def predict_step(self, batch, batch_idx: int
-    ) -> torch.FloatTensor:
+    def predict_step(self, batch: Any, batch_idx: int
+    ) -> Any:
         """The perdict step
 
         Args:
-            batch (Dict[str, Any]): The input batch
+            batch (Any): The input batch
             batch_idx (int): Only for compatibility
 
         Returns:
-            torch.FloatTensor: The predicted output (logit)
+            Any: The predicted output and optional additional information.
         """
         pass
```

### Comparing `ts3l-0.30/ts3l/pl_modules/dae_lightning.py` & `ts3l-0.40/ts3l/pl_modules/dae_lightning.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         del config["noise_level"]
         del config["noise_ratio"]
         
         self.first_phase_mask_loss = nn.BCELoss()
         self.first_phase_feature_loss1 = nn.CrossEntropyLoss()
         self.first_phase_feature_loss2 = nn.MSELoss()
 
-        self.model = DAE(**config)
+        self._init_model(DAE, config)
     
     def _get_first_phase_loss(self, batch: Tuple[torch.Tensor, torch.Tensor, torch.Tensor]):
         """Calculate the first phase loss
 
         Args:
             batch (Tuple[torch.Tensor, torch.Tensor]): The input batch
```

### Comparing `ts3l-0.30/ts3l/pl_modules/scarf_lightning.py` & `ts3l-0.40/ts3l/pl_modules/scarf_lightning.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         Args:
             config (Dict[str, Any]): The given hyperparameter set for SCARF. 
         """
         self.first_phase_loss = NTXentLoss(config["tau"])
         del config["tau"]
         del config["corruption_rate"]
         
-        self.model = SCARF(**config)
+        self._init_model(SCARF, config)
     
     def _get_first_phase_loss(self, batch):
         """Calculate the first phase loss
 
         Args:
             batch (Dict[str, Any]): The input batch
```

### Comparing `ts3l-0.30/ts3l/pl_modules/subtab_lightning.py` & `ts3l-0.40/ts3l/pl_modules/subtab_lightning.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         del config["use_contrastive"]
         del config["use_distance"]
         del config["use_cosine_similarity"]
         del config["shuffle"]
         del config["mask_ratio"]
         del config["noise_type"]
         del config["noise_level"]
-        self.model = SubTab(**config)
+        
+        self._init_model(SubTab, config)
     
     def __get_recon_label(self, label: torch.Tensor) -> torch.Tensor:
         """Duplicates the input label tensor across the batch dimension to match the number of subsets for reconstruction loss.
 
         Args:
             label (torch.Tensor): The input tensor representing the label to be duplicated.
```

### Comparing `ts3l-0.30/ts3l/pl_modules/vime_lightning.py` & `ts3l-0.40/ts3l/pl_modules/vime_lightning.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         
         self.first_phase_mask_loss = nn.BCELoss()
         self.first_phase_feature_loss1 = nn.CrossEntropyLoss()
         self.first_phase_feature_loss2 = nn.MSELoss()
         
         self.consistency_loss = nn.MSELoss()
 
-        self.model = VIME(**config)
+        self._init_model(VIME, config)
     
     def _get_first_phase_loss(self, batch:Dict[str, Any]):
         """Calculate the first phase loss
 
         Args:
             batch (Dict[str, Any]): The input batch
```

### Comparing `ts3l-0.30/ts3l/utils/base_config.py` & `ts3l-0.40/ts3l/utils/base_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from dataclasses import dataclass, field
 
 from typing import Dict, Any, Optional
 from torch import optim, nn
 import torchmetrics
 import sklearn
 
+import sys
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 @dataclass
 class BaseConfig:
     """ Configuration class for initializing components of the TabularS3L Lightning Module, including optimizers, 
     learning rate schedulers, and loss functions, along with their respective hyperparameters.
 
     Attributes:
         task (str): Specify whether the problem is regression or classification.
@@ -18,14 +24,15 @@
         optim (str): Name of the optimizer to be used. Must be an attribute of 'torch.optim'. Default is 'AdamW'.
         optim_hparams (Dict[str, Any]): Hyperparameters for the optimizer. Default is {'lr': 0.0001, 'weight_decay': 0.00005}.
         scheduler (str): Name of the learning rate scheduler to be used. Must be an attribute of 'torch.optim.lr_scheduler' or None. Default is None.
         scheduler_hparams (Dict[str, Any]): Hyperparameters for the scheduler. Default is None, indicating no scheduler is used.
         loss_hparams (Dict[str, Any]): Hyperparameters for the loss function. Default is empty dictionary.
         metric (str): Name of the metric to be used. Must be an attribute of 'torchmetrics.functional' or 'sklearn.metrics'. Default is None.
         metric_hparams (Dict[str, Any]): Hyperparameters for the metric. Default is an empty dictionary.
+        initialization (str): The way to initialize neural network parameters. Default is 'kaiming_uniform'.
         random_seed (int): Seed for random number generators to ensure reproducibility. Defaults to 42.
 
     Raises:
         ValueError: If the specified 'optim' is not a valid optimizer in 'torch.optim'.
         ValueError: If the specified 'scheduler' is not None and is not a valid scheduler in 'torch.optim.lr_scheduler'.
 
         ValueError: If the specified 'loss_fn' is not None and is not a valid loss function in 'torch.nn'.
@@ -58,14 +65,16 @@
                                             }
                                         )
     
     scheduler: Optional[str] = field(default=None)
     
     scheduler_hparams: Optional[Dict[str, Any]] = field(default = None)
     
+    initialization: Literal['xavier_uniform', 'xavier_normal', 'kaiming_uniform', 'kaiming_normal', 'uniform', 'normal'] = "kaiming_uniform"
+    
     random_seed: int = field(default=42)
     
     def __post_init__(self):
 
         if (type(self.task) is not str or (self.task != "regression" and self.task != "classification")):
             raise ValueError(f"{self.task} is not a valid task. Choices are: ['regression', 'classification']")
```

### Comparing `ts3l-0.30/ts3l/utils/dae_utils/dae_config.py` & `ts3l-0.40/ts3l/utils/dae_utils/dae_config.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/utils/dae_utils/data_utils.py` & `ts3l-0.40/ts3l/utils/dae_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/utils/datamodule.py` & `ts3l-0.40/ts3l/utils/datamodule.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/utils/scarf_utils/data_utils.py` & `ts3l-0.40/ts3l/utils/scarf_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/utils/scarf_utils/loss.py` & `ts3l-0.40/ts3l/utils/scarf_utils/loss.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/utils/scarf_utils/scarf_config.py` & `ts3l-0.40/ts3l/utils/scarf_utils/scarf_config.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/utils/subtab_utils/data_utils.py` & `ts3l-0.40/ts3l/utils/subtab_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/utils/subtab_utils/loss.py` & `ts3l-0.40/ts3l/utils/subtab_utils/loss.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/utils/subtab_utils/subtab_config.py` & `ts3l-0.40/ts3l/utils/subtab_utils/subtab_config.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/utils/vime_utils/data_utils.py` & `ts3l-0.40/ts3l/utils/vime_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l/utils/vime_utils/vime_config.py` & `ts3l-0.40/ts3l/utils/vime_utils/vime_config.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.30/ts3l.egg-info/PKG-INFO` & `ts3l-0.40/ts3l.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ts3l
-Version: 0.30
+Version: 0.40
 Summary: A PyTorch Lightning-based library for self- and semi-supervised learning on tabular data.
 Home-page: https://github.com/Alcoholrithm/TabularS3L
 Author: Minwook Kim
 Author-email: kmiiiaa@pusan.ac.kr
-Keywords: tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF DenoisingAutoEncoder
+Keywords: tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF Denoising-AutoEncoder SwitchTab
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: torch
@@ -20,18 +20,18 @@
 
 [**Overview**](#tabulars3l)
 | [**Installation**](#installation)
 | [**Available Models with Quick Start Guides**](#available-models-with-quick-start)
 | [**Benchmark**](#benchmark)
 | [**To DO**](#to-do)
 | [**Contributing**](#contributing)
-| [**Credit**](#credit)
 
 
 [![pypi](https://img.shields.io/pypi/v/ts3l)](https://pypi.org/project/ts3l/0.20/)
+[![Downloads](https://static.pepy.tech/badge/ts3l)](https://pepy.tech/project/ts3l)
 [![DOI](https://zenodo.org/badge/756740921.svg)](https://zenodo.org/doi/10.5281/zenodo.10776537)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 TabularS3L is a PyTorch Lightning-based library designed to facilitate self- and semi-supervised learning with tabular data. While numerous self- and semi-supervised learning tabular models have been proposed, there is a lack of a comprehensive library that addresses the needs of tabular practitioners. This library aims to fill this gap by providing a unified PyTorch Lightning-based framework for exploring and deploying such models.
 
 ## Installation
 We provide a Python package ts3l of TabularS3L for users who want to use semi- and self-supervised learning tabular models.
@@ -46,14 +46,15 @@
 
 | Model | First Phase | Second Phase |
 |:---:|:---:|:---:|
 | **DAE** ([GitHub](https://github.com/ryancheunggit/tabular_dae))| Self-SL | SL |
 | **VIME** ([NeurIPS'20](https://proceedings.neurips.cc/paper/2020/hash/7d97667a3e056acab9aaf653807b4a03-Abstract.html)) | Self-SL | Semi-SL or SL |
 | **SubTab** ([NeurIPS'21](https://proceedings.neurips.cc/paper/2021/hash/9c8661befae6dbcd08304dbf4dcaf0db-Abstract.html)) | Self-SL | SL |
 | **SCARF** ([ICLR'22](https://iclr.cc/virtual/2022/spotlight/6297))| Self-SL | SL |
+| **SwitchTab** ([AAAI'24](https://ojs.aaai.org/index.php/AAAI/article/view/29523)) | Self-SL | SL |
 
 #### Denoising AutoEncoder (DAE)
 DAE processes input data that has been partially corrupted, producing clean data and predicting which features are corrupted during the self-supervised learning.
 The denoising task enables the model to learn the input distribution and generate latent representations that are robust to corruption. 
 These latent representations can be utilized for a variety of downstream tasks.
 
 <details close>
@@ -400,14 +401,103 @@
   accuracy = accuracy_score(y_test, preds.argmax(1))
 
   print("Accuracy %.2f" % accuracy)
   ```
 
 </details>
 
+#### SwitchTab: Switched Autoencoders Are Effective Tabular Learners
+SwitchTab introduces a novel self-supervised method specifically designed to decuple mutual and salient features among data pair, resulting in more representative embeddings.
+Moreover, the pre-trained salient embeddings can be utilized as plug-and-play features to enhance the performance of various traditional classification methods.
+
+<details close>
+  <summary>Quick Start</summary>
+  
+  ```python
+  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
+
+  # Prepare the SwitchTabLightning Module
+  from ts3l.pl_modules import SwitchTabLightning
+  from ts3l.utils.switchtab_utils import SwitchTabDataset, SwitchTabFirstPhaseCollateFN
+  from ts3l.utils import TS3LDataModule
+  from ts3l.utils.switchtab_utils import SwitchTabConfig
+  from pytorch_lightning import Trainer
+
+  metric = "accuracy_score"
+  input_dim = X_train.shape[1]
+  hidden_dim = 1024
+  output_dim = 2
+
+  encoder_depth = 3
+  n_head = 2
+  u_label = -1
+
+  batch_size = 128
+
+  X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
+
+  config = SwitchTabConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
+  input_dim=input_dim, hidden_dim=hidden_dim,
+  output_dim=output_dim, encoder_depth=encoder_depth,
+  n_head = n_head,
+  u_label = u_label
+  )
+
+  pl_switchtab = SwitchTabLightning(config)
+
+  ### First Phase Learning
+  train_ds = SwitchTabDataset(X = X_train, unlabeled_data = X_unlabeled, Y = y_train.values, config=config, continuous_cols=continuous_cols, category_cols=category_cols)
+  valid_ds = SwitchTabDataset(X = X_valid, config=config, Y = y_valid.values, continuous_cols=continuous_cols, category_cols=category_cols)
+
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='weighted', train_collate_fn=SwitchTabFirstPhaseCollateFN(), valid_collate_fn=SwitchTabFirstPhaseCollateFN())
+
+  trainer = Trainer(
+                  accelerator = 'cpu',
+                  max_epochs = 20,
+                  num_sanity_val_steps = 2,
+  )
+
+  trainer.fit(pl_switchtab, datamodule)
+
+  ### Second Phase Learning
+
+  pl_switchtab.set_second_phase()
+
+  train_ds = SwitchTabDataset(X = X_train, Y = y_train.values, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  valid_ds = SwitchTabDataset(X = X_valid, Y = y_valid.values, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+      
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted")
+
+  trainer = Trainer(
+                  accelerator = 'cpu',
+                  max_epochs = 20,
+                  num_sanity_val_steps = 2,
+  )
+
+  trainer.fit(pl_switchtab, datamodule)
+
+  # Evaluation
+  from sklearn.metrics import accuracy_score
+  import torch
+  from torch.nn import functional as F
+  from torch.utils.data import DataLoader, SequentialSampler
+
+  test_ds = SwitchTabDataset(X_test, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds))
+
+  preds = trainer.predict(pl_switchtab, test_dl)
+      
+  preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
+
+  accuracy = accuracy_score(y_test, preds.argmax(1))
+
+  print("Accuracy %.2f" % accuracy)
+  ```
+
+</details>
 
 ## Benchmark
 
 We provide a simple benchmark using TabularS3L against XGBoost. The train-validation-test ratio is 6:2:2 and we tuned each model over 50 trials using Optuna. The results are the average of the random seeds [0,4]. The best results are bold. 'acc', 'b-acc', and 'mse' mean 'Accuracy', 'Balanced Accuracy', and 'Mean Squared Error', respectively.
 
 Use this benchmark for reference only, as only a small number of random seeds were used.
 
@@ -415,58 +505,36 @@
 
 | Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
 |:---:|:---:|:---:|:---:|
 | XGBoost | 0.7325 | 0.4763 | **5.5739** |
 | DAE | 0.7208 | 0.4885 | 5.6168 | 
 | VIME | 0.7182 | **0.5087** | 5.6637 |
 | SubTab | 0.7312 | 0.4930 | 7.2418 |
-| SCARF | **0.7416** | 0.4710 | 5.8888 | 
+| SCARF | **0.7416** | 0.4710 | 5.8888 |
+| SwitchTab |  0.7156 | 0.4886 | 5.9907 |
 
 --------
 
 ##### 100% labeled samples
 
 | Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
 |:---:|:---:|:---:|:---:|
 | XGBoost | 0.7234 | 0.5291 | 4.8377 |
 | DAE | 0.7390 | 0.5500 | 4.5758 |
 | VIME | **0.7688** | 0.5477 | 4.5804 |
 | SubTab | 0.7390 | 0.5432 | 6.3104 |
 | SCARF | 0.7442 | **0.5521** | **4.4443** |
+| SwitchTab | 0.7585 | 0.5411 | 4.7489 |
 
 ## To DO
 
 - [x] Release nn.Module and Dataset of VIME, SubTab, and SCARF
-  - [x] VIME
-  - [x] SubTab
-  - [x] SCARF
 - [x] Release LightningModules of VIME, SubTab, and SCARF
-  - [x] VIME
-  - [x] SubTab
-  - [x] SCARF
 - [x] Release Denoising AutoEncoder
-  - [x] nn.Module
-  - [x] LightningModule
-- [ ] Release SwitchTab
-  - [ ] nn.Module
-  - [ ] LightningModule
+- [x] Release SwitchTab
 - [x] Add example codes
+- [ ] Release more tabular models
 
 ## Contributing
 
 Contributions to this implementation are highly appreciated. Whether it's suggesting improvements, reporting bugs, or proposing new features, feel free to open an issue or submit a pull request.
 
-
-## Credit  
-```
-@software{alcoholrithm_2024_10776538,
-  author       = {Minwook Kim},
-  title        = {TabularS3L},
-  month        = mar,
-  year         = 2024,
-  publisher    = {Zenodo},
-  version      = {v0.21},
-  doi          = {10.5281/zenodo.10776538},
-  url          = {https://doi.org/10.5281/zenodo.10776538}
-}
-```
-
```

### Comparing `ts3l-0.30/ts3l.egg-info/SOURCES.txt` & `ts3l-0.40/ts3l.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 LICENSE
 README.md
 setup.py
 test/test_dae.py
 test/test_scarf.py
 test/test_subtab.py
+test/test_switchtab.py
 test/test_vime.py
 ts3l/__init__.py
 ts3l.egg-info/PKG-INFO
 ts3l.egg-info/SOURCES.txt
 ts3l.egg-info/dependency_links.txt
 ts3l.egg-info/requires.txt
 ts3l.egg-info/top_level.txt
 ts3l/models/__init__.py
 ts3l/models/common/__init__.py
+ts3l/models/common/misc.py
 ts3l/models/common/mlp.py
 ts3l/models/dae/__init__.py
 ts3l/models/dae/dae.py
 ts3l/models/scarf/__init__.py
 ts3l/models/scarf/scarf.py
 ts3l/models/subtab/__init__.py
 ts3l/models/subtab/subtab.py
+ts3l/models/switchtab/__init__.py
+ts3l/models/switchtab/ft_transformer.py
+ts3l/models/switchtab/switchtab.py
 ts3l/models/vime/__init__.py
 ts3l/models/vime/vime.py
 ts3l/models/vime/vime_self.py
 ts3l/models/vime/vime_semi.py
 ts3l/pl_modules/__init__.py
 ts3l/pl_modules/base_module.py
 ts3l/pl_modules/dae_lightning.py
 ts3l/pl_modules/scarf_lightning.py
 ts3l/pl_modules/subtab_lightning.py
+ts3l/pl_modules/switchtab_lightning.py
 ts3l/pl_modules/vime_lightning.py
 ts3l/utils/__init__.py
 ts3l/utils/base_config.py
 ts3l/utils/datamodule.py
 ts3l/utils/misc.py
 ts3l/utils/dae_utils/__init__.py
 ts3l/utils/dae_utils/dae_config.py
@@ -41,10 +47,13 @@
 ts3l/utils/scarf_utils/data_utils.py
 ts3l/utils/scarf_utils/loss.py
 ts3l/utils/scarf_utils/scarf_config.py
 ts3l/utils/subtab_utils/__init__.py
 ts3l/utils/subtab_utils/data_utils.py
 ts3l/utils/subtab_utils/loss.py
 ts3l/utils/subtab_utils/subtab_config.py
+ts3l/utils/switchtab_utils/__init__.py
+ts3l/utils/switchtab_utils/data_utils.py
+ts3l/utils/switchtab_utils/switchtab_config.py
 ts3l/utils/vime_utils/__init__.py
 ts3l/utils/vime_utils/data_utils.py
 ts3l/utils/vime_utils/vime_config.py
```

