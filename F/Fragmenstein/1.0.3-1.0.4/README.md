# Comparing `tmp/Fragmenstein-1.0.3.tar.gz` & `tmp/Fragmenstein-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fragmenstein-1.0.3.tar", last modified: Fri Apr  5 10:22:39 2024, max compression
+gzip compressed data, was "Fragmenstein-1.0.4.tar", last modified: Thu May  2 12:49:28 2024, max compression
```

## Comparing `Fragmenstein-1.0.3.tar` & `Fragmenstein-1.0.4.tar`

### file list

```diff
@@ -1,720 +1,720 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:39.634111 Fragmenstein-1.0.3/
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:33.350539 Fragmenstein-1.0.3/Fragmenstein.egg-info/
--rw-r--r--   0 user       (502) staff       (20)    32364 2024-04-05 10:22:33.000000 Fragmenstein-1.0.3/Fragmenstein.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)    28971 2024-04-05 10:22:33.000000 Fragmenstein-1.0.3/Fragmenstein.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2024-04-05 10:22:33.000000 Fragmenstein-1.0.3/Fragmenstein.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)       55 2024-04-05 10:22:33.000000 Fragmenstein-1.0.3/Fragmenstein.egg-info/entry_points.txt
--rw-r--r--   0 user       (502) staff       (20)      340 2024-04-05 10:22:33.000000 Fragmenstein-1.0.3/Fragmenstein.egg-info/requires.txt
--rw-r--r--   0 user       (502) staff       (20)       19 2024-04-05 10:22:33.000000 Fragmenstein-1.0.3/Fragmenstein.egg-info/top_level.txt
--rw-r--r--   0 user       (502) staff       (20)     1069 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/LICENSE
--rw-r--r--   0 user       (502) staff       (20)      317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/MANIFEST.in
--rw-r--r--   0 user       (502) staff       (20)    32364 2024-04-05 10:22:39.631101 Fragmenstein-1.0.3/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)    31456 2024-02-21 13:22:43.000000 Fragmenstein-1.0.3/README.md
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:33.396355 Fragmenstein-1.0.3/fragmenstein/
--rw-r--r--   0 user       (502) staff       (20)     2059 2024-02-21 13:07:25.000000 Fragmenstein-1.0.3/fragmenstein/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     1465 2024-02-15 19:52:24.000000 Fragmenstein-1.0.3/fragmenstein/_cli_defaults.py
--rw-r--r--   0 user       (502) staff       (20)     1189 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/branding.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:33.437142 Fragmenstein-1.0.3/fragmenstein/cli/
--rw-r--r--   0 user       (502) staff       (20)      826 2024-01-17 13:24:24.000000 Fragmenstein-1.0.3/fragmenstein/cli/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     3175 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/cli/base.py
--rw-r--r--   0 user       (502) staff       (20)     5136 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/cli/laboratory.py
--rw-r--r--   0 user       (502) staff       (20)     1474 2023-04-27 17:14:38.000000 Fragmenstein-1.0.3/fragmenstein/cli/monster.py
--rw-r--r--   0 user       (502) staff       (20)     4904 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/cli/old.py
--rw-r--r--   0 user       (502) staff       (20)      600 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/cli/parser.py
--rw-r--r--   0 user       (502) staff       (20)     8987 2024-02-09 11:09:55.000000 Fragmenstein-1.0.3/fragmenstein/cli/pipeline.py
--rw-r--r--   0 user       (502) staff       (20)     3287 2024-01-17 13:54:57.000000 Fragmenstein-1.0.3/fragmenstein/cli/utils.py
--rw-r--r--   0 user       (502) staff       (20)     1730 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/cli/victor.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:33.446812 Fragmenstein-1.0.3/fragmenstein/demo/
--rw-r--r--   0 user       (502) staff       (20)     2101 2023-09-18 15:43:25.000000 Fragmenstein-1.0.3/fragmenstein/demo/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     4515 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/_base_dataset_holder.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:35.444557 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/
--rw-r--r--   0 user       (502) staff       (20)       85 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/__init__.py
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1592 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1592 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)      998 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol
--rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol
--rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1164 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol
--rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol
--rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1343 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1164 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol
--rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1343 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol
--rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol
--rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol
--rw-r--r--   0 user       (502) staff       (20)      998 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol
--rw-r--r--   0 user       (502) staff       (20)      902 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol
--rw-r--r--   0 user       (502) staff       (20)      902 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol
--rw-r--r--   0 user       (502) staff       (20)      570 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol
--rw-r--r--   0 user       (502) staff       (20)      570 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol
--rw-r--r--   0 user       (502) staff       (20)      557 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol
--rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol
--rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol
--rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1605 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0115.mol
--rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0116.mol
--rw-r--r--   0 user       (502) staff       (20)     1186 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0123.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0124.mol
--rw-r--r--   0 user       (502) staff       (20)     1601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0131.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0132.mol
--rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0137.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0138.mol
--rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0139.mol
--rw-r--r--   0 user       (502) staff       (20)     1531 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0142.mol
--rw-r--r--   0 user       (502) staff       (20)     1614 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0148.mol
--rw-r--r--   0 user       (502) staff       (20)     1518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0159.mol
--rw-r--r--   0 user       (502) staff       (20)     1601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0161.mol
--rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0163.mol
--rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0178.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0179.mol
--rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0180.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0182.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0188.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0190.mol
--rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0193.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0204.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0206.mol
--rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0212.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0213.mol
--rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0223.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0224.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0226.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0227.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0228.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0231.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0255.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0263.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0271.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0277.mol
--rw-r--r--   0 user       (502) staff       (20)      841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0282.mol
--rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0283.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0284.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0301.mol
--rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0302.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0303.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0305.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0306.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0309.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0319.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0321.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0326.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0328.mol
--rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0333.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0337.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0338.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0341.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0343.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0344.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0345.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0346.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0347.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0348.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0354.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0357.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0358.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0360.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0361.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0365.mol
--rw-r--r--   0 user       (502) staff       (20)     2073 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0371.mol
--rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0373.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0375.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0378.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0379.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0380.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0381.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0385.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0387.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0392.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0394.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0396.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0397.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0398.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0402.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0404.mol
--rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0411.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0412.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0415.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0417.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0433.mol
--rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0436.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0437.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0439.mol
--rw-r--r--   0 user       (502) staff       (20)     1505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0441.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0444.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0451.mol
--rw-r--r--   0 user       (502) staff       (20)      745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0453.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0455.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0472.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0482.mol
--rw-r--r--   0 user       (502) staff       (20)     1671 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0496.mol
--rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0509.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0510.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0511.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0522.mol
--rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0527.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0546.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0555.mol
--rw-r--r--   0 user       (502) staff       (20)     1269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0564.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0565.mol
--rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0567.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0568.mol
--rw-r--r--   0 user       (502) staff       (20)     2156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0570.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0572.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0576.mol
--rw-r--r--   0 user       (502) staff       (20)     1352 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0582.mol
--rw-r--r--   0 user       (502) staff       (20)     1614 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0584.mol
--rw-r--r--   0 user       (502) staff       (20)     1326 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0587.mol
--rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0588.mol
--rw-r--r--   0 user       (502) staff       (20)     3121 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0590.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x1493.mol
--rw-r--r--   0 user       (502) staff       (20)     1933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x1494.mol
--rw-r--r--   0 user       (502) staff       (20)   208424 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/template.pdb
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:38.711793 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/
--rw-r--r--   0 user       (502) staff       (20)     2850 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6lze.mol
--rw-r--r--   0 user       (502) staff       (20)     2933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol
--rw-r--r--   0 user       (502) staff       (20)     2933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6w63.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol
--rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol
--rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol
--rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol
--rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol
--rw-r--r--   0 user       (502) staff       (20)      404 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xbg.mol
--rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol
--rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol
--rw-r--r--   0 user       (502) staff       (20)      972 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xch.mol
--rw-r--r--   0 user       (502) staff       (20)      806 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol
--rw-r--r--   0 user       (502) staff       (20)     2920 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol
--rw-r--r--   0 user       (502) staff       (20)      640 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol
--rw-r--r--   0 user       (502) staff       (20)     2658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol
--rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol
--rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol
--rw-r--r--   0 user       (502) staff       (20)     3527 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol
--rw-r--r--   0 user       (502) staff       (20)     3680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol
--rw-r--r--   0 user       (502) staff       (20)     3680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol
--rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol
--rw-r--r--   0 user       (502) staff       (20)      832 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol
--rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol
--rw-r--r--   0 user       (502) staff       (20)      505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6yz6.mol
--rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6zru.mol
--rw-r--r--   0 user       (502) staff       (20)     2230 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7aku.mol
--rw-r--r--   0 user       (502) staff       (20)      754 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7brp.mol
--rw-r--r--   0 user       (502) staff       (20)      806 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7buy.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol
--rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol
--rw-r--r--   0 user       (502) staff       (20)      142 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c8b.mol
--rw-r--r--   0 user       (502) staff       (20)     3820 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol
--rw-r--r--   0 user       (502) staff       (20)     3667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7com.mol
--rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol
--rw-r--r--   0 user       (502) staff       (20)      142 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7d1m.mol
--rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol
--rw-r--r--   0 user       (502) staff       (20)     2850 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol
--rw-r--r--   0 user       (502) staff       (20)     3527 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol
--rw-r--r--   0 user       (502) staff       (20)      391 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7jr4.mol
--rw-r--r--   0 user       (502) staff       (20)     3112 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol
--rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7k40.mol
--rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol
--rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol
--rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol
--rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0072.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0104.mol
--rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0107.mol
--rw-r--r--   0 user       (502) staff       (20)     1239 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0161.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0165.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0177.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0194.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0195.mol
--rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0305.mol
--rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0336.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0350.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0354.mol
--rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0376.mol
--rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0387.mol
--rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0390.mol
--rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0395.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0397.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0398.mol
--rw-r--r--   0 user       (502) staff       (20)     1348 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0425.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0426.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0434.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0464.mol
--rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0478.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0499.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0540.mol
--rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0669.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0678.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0689.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0691.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0692.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0705.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0708.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0731.mol
--rw-r--r--   0 user       (502) staff       (20)     1693 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0734.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0736.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0748.mol
--rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0749.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0752.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0755.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0759.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0769.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0770.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0771.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0774.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0786.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0820.mol
--rw-r--r--   0 user       (502) staff       (20)     1846 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0830.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0831.mol
--rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0874.mol
--rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0887.mol
--rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0946.mol
--rw-r--r--   0 user       (502) staff       (20)     1737 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0967.mol
--rw-r--r--   0 user       (502) staff       (20)     1309 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0978.mol
--rw-r--r--   0 user       (502) staff       (20)     1392 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0981.mol
--rw-r--r--   0 user       (502) staff       (20)      479 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0991.mol
--rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0995.mol
--rw-r--r--   0 user       (502) staff       (20)     1930 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10019.mol
--rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1002.mol
--rw-r--r--   0 user       (502) staff       (20)     1502 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10022.mol
--rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10049.mol
--rw-r--r--   0 user       (502) staff       (20)     2160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10082.mol
--rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1012.mol
--rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10150.mol
--rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10155.mol
--rw-r--r--   0 user       (502) staff       (20)     1323 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10172.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10178.mol
--rw-r--r--   0 user       (502) staff       (20)     1502 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10201.mol
--rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10236.mol
--rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10237.mol
--rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10247.mol
--rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10248.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10296.mol
--rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10306.mol
--rw-r--r--   0 user       (502) staff       (20)     1668 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10314.mol
--rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10322.mol
--rw-r--r--   0 user       (502) staff       (20)     1943 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10324.mol
--rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10327.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10329.mol
--rw-r--r--   0 user       (502) staff       (20)     1668 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10334.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10338.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10355.mol
--rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10359.mol
--rw-r--r--   0 user       (502) staff       (20)     1930 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10371.mol
--rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10377.mol
--rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10387.mol
--rw-r--r--   0 user       (502) staff       (20)     1764 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10392.mol
--rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10395.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10396.mol
--rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10403.mol
--rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10417.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10419.mol
--rw-r--r--   0 user       (502) staff       (20)     1751 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10421.mol
--rw-r--r--   0 user       (502) staff       (20)     1751 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10422.mol
--rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10423.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10466.mol
--rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10473.mol
--rw-r--r--   0 user       (502) staff       (20)     1400 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10474.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10476.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10478.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10484.mol
--rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10488.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10494.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10506.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10513.mol
--rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10525.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10535.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10555.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10559.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10565.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10566.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10575.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10598.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10604.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10606.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10610.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10626.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10638.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10645.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10678.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10679.mol
--rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10700.mol
--rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10710.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10723.mol
--rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10728.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10733.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10756.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1077.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10787.mol
--rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10789.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10800.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10801.mol
--rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10812.mol
--rw-r--r--   0 user       (502) staff       (20)     2352 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10820.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10834.mol
--rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10856.mol
--rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1086.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10862.mol
--rw-r--r--   0 user       (502) staff       (20)     2697 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10870.mol
--rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10871.mol
--rw-r--r--   0 user       (502) staff       (20)     2435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10876.mol
--rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10888.mol
--rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10889.mol
--rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10898.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10899.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10900.mol
--rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10906.mol
--rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1093.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10942.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10959.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10976.mol
--rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10995.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10996.mol
--rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11001.mol
--rw-r--r--   0 user       (502) staff       (20)     2593 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1101.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11011.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11013.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11025.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11041.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11044.mol
--rw-r--r--   0 user       (502) staff       (20)     1854 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11159.mol
--rw-r--r--   0 user       (502) staff       (20)     2518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11164.mol
--rw-r--r--   0 user       (502) staff       (20)     1854 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11186.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1119.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11204.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11208.mol
--rw-r--r--   0 user       (502) staff       (20)     1675 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11212.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11223.mol
--rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11225.mol
--rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11231.mol
--rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11233.mol
--rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11254.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11258.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11271.mol
--rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11294.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11313.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11317.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11318.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1132.mol
--rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11339.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11346.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11354.mol
--rw-r--r--   0 user       (502) staff       (20)     2269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11366.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11368.mol
--rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11372.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11417.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11424.mol
--rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11426.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11427.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11428.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11431.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11432.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11454.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11458.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11473.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11475.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11485.mol
--rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11488.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11493.mol
--rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11498.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11499.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11541.mol
--rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11562.mol
--rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11564.mol
--rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11579.mol
--rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11587.mol
--rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11612.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1163.mol
--rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11642.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11723.mol
--rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11743.mol
--rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11764.mol
--rw-r--r--   0 user       (502) staff       (20)     2518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11790.mol
--rw-r--r--   0 user       (502) staff       (20)     2435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11797.mol
--rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11798.mol
--rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11801.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11809.mol
--rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11831.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1187.mol
--rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11894.mol
--rw-r--r--   0 user       (502) staff       (20)     2269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x12025.mol
--rw-r--r--   0 user       (502) staff       (20)     2186 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x12073.mol
--rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x12080.mol
--rw-r--r--   0 user       (502) staff       (20)      907 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1226.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1235.mol
--rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1237.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1249.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1308.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1311.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1334.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1336.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1348.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1351.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1358.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1374.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1375.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1380.mol
--rw-r--r--   0 user       (502) staff       (20)     1239 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1382.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1384.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1385.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1386.mol
--rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1392.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1402.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1412.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1418.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1425.mol
--rw-r--r--   0 user       (502) staff       (20)     1488 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1458.mol
--rw-r--r--   0 user       (502) staff       (20)     1073 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1478.mol
--rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1493.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2052.mol
--rw-r--r--   0 user       (502) staff       (20)      824 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2097.mol
--rw-r--r--   0 user       (502) staff       (20)      741 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2119.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2193.mol
--rw-r--r--   0 user       (502) staff       (20)     2497 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2540.mol
--rw-r--r--   0 user       (502) staff       (20)     1929 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2562.mol
--rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2563.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2569.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2572.mol
--rw-r--r--   0 user       (502) staff       (20)     1929 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2581.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2600.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2608.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2643.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2646.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2649.mol
--rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2659.mol
--rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2694.mol
--rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2703.mol
--rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2705.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2754.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2764.mol
--rw-r--r--   0 user       (502) staff       (20)     3008 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2776.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2779.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2908.mol
--rw-r--r--   0 user       (502) staff       (20)     2178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2910.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2912.mol
--rw-r--r--   0 user       (502) staff       (20)     1846 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2929.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2964.mol
--rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2971.mol
--rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3077.mol
--rw-r--r--   0 user       (502) staff       (20)     2261 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3080.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3108.mol
--rw-r--r--   0 user       (502) staff       (20)     2829 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3110.mol
--rw-r--r--   0 user       (502) staff       (20)     2663 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3113.mol
--rw-r--r--   0 user       (502) staff       (20)     2580 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3115.mol
--rw-r--r--   0 user       (502) staff       (20)     2759 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3117.mol
--rw-r--r--   0 user       (502) staff       (20)     2331 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3124.mol
--rw-r--r--   0 user       (502) staff       (20)     2427 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3298.mol
--rw-r--r--   0 user       (502) staff       (20)     2191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3303.mol
--rw-r--r--   0 user       (502) staff       (20)     2261 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3305.mol
--rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3324.mol
--rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3325.mol
--rw-r--r--   0 user       (502) staff       (20)     1488 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3333.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3348.mol
--rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3351.mol
--rw-r--r--   0 user       (502) staff       (20)     2414 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3359.mol
--rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3366.mol
--rw-r--r--   0 user       (502) staff       (20)       76 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/__init__.py
--rw-r--r--   0 user       (502) staff       (20)   379172 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/template.pdb
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:38.862731 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/
--rw-r--r--   0 user       (502) staff       (20)    17574 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/5SB7_mergers.sdf
--rw-r--r--   0 user       (502) staff       (20)     1254 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/F584.mol
--rw-r--r--   0 user       (502) staff       (20)      144 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/__init__.py
--rwxr-xr-x   0 user       (502) staff       (20)   467127 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/apo_example1.pdb
--rw-r--r--   0 user       (502) staff       (20)     6701 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/dummy.pdb
--rwxr-xr-x   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/mac-x0138.mol
--rwxr-xr-x   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/mac-x0398.mol
--rw-r--r--   0 user       (502) staff       (20)     4580 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/placed_example1.mol
--rw-r--r--   0 user       (502) staff       (20)      753 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/rototoluene.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/toluene.mol
--rw-r--r--   0 user       (502) staff       (20)      758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/transtoluene.mol
--rw-r--r--   0 user       (502) staff       (20)      763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/transtoluene2.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/x0032_0A.mol
--rw-r--r--   0 user       (502) staff       (20)     1421 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/demo/test_mols/x0103_0A.mol
--rw-r--r--   0 user       (502) staff       (20)     3115 2024-02-21 13:07:25.000000 Fragmenstein-1.0.3/fragmenstein/display.py
--rw-r--r--   0 user       (502) staff       (20)    56342 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/divergent_colors.json
--rw-r--r--   0 user       (502) staff       (20)     1801 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/error.py
--rw-r--r--   0 user       (502) staff       (20)     6425 2023-12-18 18:30:24.000000 Fragmenstein-1.0.3/fragmenstein/extraction_funs.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:38.903461 Fragmenstein-1.0.3/fragmenstein/faux_victors/
--rw-r--r--   0 user       (502) staff       (20)     1178 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/faux_victors/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     4793 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/faux_victors/brics.py
--rw-r--r--   0 user       (502) staff       (20)    13343 2023-12-11 16:13:15.000000 Fragmenstein-1.0.3/fragmenstein/faux_victors/mcs_monster.py
--rw-r--r--   0 user       (502) staff       (20)     1018 2024-03-13 10:07:19.000000 Fragmenstein-1.0.3/fragmenstein/faux_victors/mcs_victor.py
--rw-r--r--   0 user       (502) staff       (20)     5743 2024-03-13 10:05:02.000000 Fragmenstein-1.0.3/fragmenstein/faux_victors/no_pyrosetta.py
--rw-r--r--   0 user       (502) staff       (20)     3648 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/faux_victors/others.py
--rw-r--r--   0 user       (502) staff       (20)     2712 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/faux_victors/quick.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:38.934785 Fragmenstein-1.0.3/fragmenstein/igor/
--rw-r--r--   0 user       (502) staff       (20)     2432 2023-04-26 12:35:21.000000 Fragmenstein-1.0.3/fragmenstein/igor/__init__.py
--rw-r--r--   0 user       (502) staff       (20)      817 2023-04-26 12:34:04.000000 Fragmenstein-1.0.3/fragmenstein/igor/_igor_base.py
--rw-r--r--   0 user       (502) staff       (20)     7774 2024-01-16 11:13:08.000000 Fragmenstein-1.0.3/fragmenstein/igor/_igor_init.py
--rw-r--r--   0 user       (502) staff       (20)    18404 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/igor/_igor_min.py
--rw-r--r--   0 user       (502) staff       (20)    12183 2024-01-17 13:54:57.000000 Fragmenstein-1.0.3/fragmenstein/igor/_igor_utils.py
--rw-r--r--   0 user       (502) staff       (20)     1193 2023-10-27 10:05:23.000000 Fragmenstein-1.0.3/fragmenstein/igor/pyrosetta_import.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:38.997458 Fragmenstein-1.0.3/fragmenstein/laboratory/
--rw-r--r--   0 user       (502) staff       (20)     1565 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/laboratory/__init__.py
--rw-r--r--   0 user       (502) staff       (20)    12423 2024-04-04 13:08:08.000000 Fragmenstein-1.0.3/fragmenstein/laboratory/_base.py
--rw-r--r--   0 user       (502) staff       (20)     5609 2024-03-13 13:33:10.000000 Fragmenstein-1.0.3/fragmenstein/laboratory/_combine.py
--rw-r--r--   0 user       (502) staff       (20)    13365 2024-02-15 19:30:09.000000 Fragmenstein-1.0.3/fragmenstein/laboratory/_extras.py
--rw-r--r--   0 user       (502) staff       (20)     5089 2024-03-13 13:36:49.000000 Fragmenstein-1.0.3/fragmenstein/laboratory/_place.py
--rw-r--r--   0 user       (502) staff       (20)    10885 2024-03-13 12:16:17.000000 Fragmenstein-1.0.3/fragmenstein/laboratory/_score.py
--rw-r--r--   0 user       (502) staff       (20)     1419 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/laboratory/validator.py
--rw-r--r--   0 user       (502) staff       (20)     1715 2024-02-22 13:26:29.000000 Fragmenstein-1.0.3/fragmenstein/legacy.py
--rw-r--r--   0 user       (502) staff       (20)    21716 2023-07-13 16:14:35.000000 Fragmenstein-1.0.3/fragmenstein/m_rmsd.py
--rw-r--r--   0 user       (502) staff       (20)     4418 2024-02-21 12:47:15.000000 Fragmenstein-1.0.3/fragmenstein/mol3d_display.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:39.106315 Fragmenstein-1.0.3/fragmenstein/monster/
--rw-r--r--   0 user       (502) staff       (20)     6504 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/monster/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     9148 2023-10-19 15:02:50.000000 Fragmenstein-1.0.3/fragmenstein/monster/_base.py
--rw-r--r--   0 user       (502) staff       (20)    53383 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/monster/_collapse_ring.py
--rw-r--r--   0 user       (502) staff       (20)     4053 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/monster/_combine.py
--rw-r--r--   0 user       (502) staff       (20)    19282 2023-07-29 22:48:42.000000 Fragmenstein-1.0.3/fragmenstein/monster/_communal.py
--rw-r--r--   0 user       (502) staff       (20)    16303 2024-04-04 13:52:48.000000 Fragmenstein-1.0.3/fragmenstein/monster/_ff.py
--rw-r--r--   0 user       (502) staff       (20)     6371 2024-04-04 15:01:11.000000 Fragmenstein-1.0.3/fragmenstein/monster/_join_neighboring.py
--rw-r--r--   0 user       (502) staff       (20)    16359 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/monster/_merge.py
--rw-r--r--   0 user       (502) staff       (20)     1717 2024-04-04 15:25:19.000000 Fragmenstein-1.0.3/fragmenstein/monster/_modification_logging.py
--rw-r--r--   0 user       (502) staff       (20)     8371 2024-03-13 12:01:11.000000 Fragmenstein-1.0.3/fragmenstein/monster/_place.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:39.186739 Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/__init__.py
--rw-r--r--   0 user       (502) staff       (20)    13701 2023-07-12 11:22:55.000000 Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_expand.py
--rw-r--r--   0 user       (502) staff       (20)     1106 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_full.py
--rw-r--r--   0 user       (502) staff       (20)     8344 2023-07-05 11:51:56.000000 Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_make_chimera.py
--rw-r--r--   0 user       (502) staff       (20)    10200 2023-07-12 13:14:33.000000 Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_mappings.py
--rw-r--r--   0 user       (502) staff       (20)     9219 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_no_blending.py
--rw-r--r--   0 user       (502) staff       (20)     9905 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_partial.py
--rw-r--r--   0 user       (502) staff       (20)     6957 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_refine.py
--rw-r--r--   0 user       (502) staff       (20)    10464 2024-02-21 12:47:15.000000 Fragmenstein-1.0.3/fragmenstein/monster/_util_compare.py
--rw-r--r--   0 user       (502) staff       (20)    14404 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/monster/_utility.py
--rw-r--r--   0 user       (502) staff       (20)     1939 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/monster/bond_provenance.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:39.225724 Fragmenstein-1.0.3/fragmenstein/monster/mcs_mapping/
--rw-r--r--   0 user       (502) staff       (20)      342 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/monster/mcs_mapping/__init__.py
--rw-r--r--   0 user       (502) staff       (20)    11854 2023-07-12 14:59:39.000000 Fragmenstein-1.0.3/fragmenstein/monster/mcs_mapping/compare_atom.py
--rw-r--r--   0 user       (502) staff       (20)     1127 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/monster/mcs_mapping/types.py
--rw-r--r--   0 user       (502) staff       (20)     5354 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/monster/mcs_mapping/utils.py
--rw-r--r--   0 user       (502) staff       (20)     5087 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/monster/positional_mapping.py
--rw-r--r--   0 user       (502) staff       (20)    21692 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/monster/unmerge_mapper.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:39.240441 Fragmenstein-1.0.3/fragmenstein/mpro/
--rw-r--r--   0 user       (502) staff       (20)     6088 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/mpro/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     1439 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/mpro/dataframe.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:39.262884 Fragmenstein-1.0.3/fragmenstein/multivictor/
--rw-r--r--   0 user       (502) staff       (20)       70 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/multivictor/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     3254 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/multivictor/multivictor.py
--rw-r--r--   0 user       (502) staff       (20)     5508 2024-02-21 10:33:08.000000 Fragmenstein-1.0.3/fragmenstein/ngl_display.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:39.292689 Fragmenstein-1.0.3/fragmenstein/openmm/
--rw-r--r--   0 user       (502) staff       (20)       59 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/openmm/__init__.py
--rw-r--r--   0 user       (502) staff       (20)    24977 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/openmm/fritz.py
--rw-r--r--   0 user       (502) staff       (20)     7011 2024-03-13 10:05:02.000000 Fragmenstein-1.0.3/fragmenstein/openmm/openvictor.py
--rw-r--r--   0 user       (502) staff       (20)     2318 2023-11-23 13:18:06.000000 Fragmenstein-1.0.3/fragmenstein/settings.py
--rw-r--r--   0 user       (502) staff       (20)      676 2024-04-05 10:16:09.000000 Fragmenstein-1.0.3/fragmenstein/version.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:39.406508 Fragmenstein-1.0.3/fragmenstein/victor/
--rw-r--r--   0 user       (502) staff       (20)     6217 2024-03-13 11:43:40.000000 Fragmenstein-1.0.3/fragmenstein/victor/__init__.py
--rw-r--r--   0 user       (502) staff       (20)      802 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/victor/_loggerwriter.py
--rw-r--r--   0 user       (502) staff       (20)     9613 2024-03-13 11:55:09.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_base.py
--rw-r--r--   0 user       (502) staff       (20)     7215 2024-03-13 11:43:40.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_combine.py
--rw-r--r--   0 user       (502) staff       (20)    18020 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_common.py
--rw-r--r--   0 user       (502) staff       (20)     5547 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_igor.py
--rw-r--r--   0 user       (502) staff       (20)     4674 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_journal.py
--rw-r--r--   0 user       (502) staff       (20)      338 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_mode.py
--rw-r--r--   0 user       (502) staff       (20)      829 2023-12-18 18:30:40.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_overridables.py
--rw-r--r--   0 user       (502) staff       (20)     9337 2024-04-04 13:35:48.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_place.py
--rw-r--r--   0 user       (502) staff       (20)     9579 2024-04-04 14:52:49.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_plonk.py
--rw-r--r--   0 user       (502) staff       (20)     1863 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_safety.py
--rw-r--r--   0 user       (502) staff       (20)     6816 2024-02-13 16:18:01.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_show.py
--rw-r--r--   0 user       (502) staff       (20)     4674 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_store.py
--rw-r--r--   0 user       (502) staff       (20)    24750 2024-02-13 15:36:41.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_utils.py
--rw-r--r--   0 user       (502) staff       (20)     2202 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/fragmenstein/victor/_victor_validate.py
--rw-r--r--   0 user       (502) staff       (20)     5650 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/victor/minimalPDB.py
--rw-r--r--   0 user       (502) staff       (20)    10778 2023-08-22 10:47:34.000000 Fragmenstein-1.0.3/fragmenstein/victor/plip.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:39.463739 Fragmenstein-1.0.3/fragmenstein/walton/
--rw-r--r--   0 user       (502) staff       (20)     2277 2024-02-21 10:33:08.000000 Fragmenstein-1.0.3/fragmenstein/walton/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     8226 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/walton/_advmoves.py
--rw-r--r--   0 user       (502) staff       (20)     4004 2024-02-21 10:52:06.000000 Fragmenstein-1.0.3/fragmenstein/walton/_art.py
--rw-r--r--   0 user       (502) staff       (20)     4333 2024-02-21 13:07:25.000000 Fragmenstein-1.0.3/fragmenstein/walton/_base.py
--rw-r--r--   0 user       (502) staff       (20)     6289 2024-01-19 13:58:39.000000 Fragmenstein-1.0.3/fragmenstein/walton/_movements.py
--rw-r--r--   0 user       (502) staff       (20)     1693 2023-04-25 12:43:41.000000 Fragmenstein-1.0.3/fragmenstein/walton/_polygon.py
--rw-r--r--   0 user       (502) staff       (20)     1033 2024-02-22 13:18:08.000000 Fragmenstein-1.0.3/requirements.txt
--rw-r--r--   0 user       (502) staff       (20)       38 2024-04-05 10:22:39.634610 Fragmenstein-1.0.3/setup.cfg
--rw-r--r--   0 user       (502) staff       (20)     3377 2024-04-05 10:16:09.000000 Fragmenstein-1.0.3/setup.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:39.626632 Fragmenstein-1.0.3/tests/
--rw-r--r--   0 user       (502) staff       (20)     1689 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/MPro_combine.py
--rw-r--r--   0 user       (502) staff       (20)     4498 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/MPro_place.py
--rw-r--r--   0 user       (502) staff       (20)      404 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/__init__.py
--rw-r--r--   0 user       (502) staff       (20)      725 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/baffled.py
--rw-r--r--   0 user       (502) staff       (20)     2623 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/cli.py
--rw-r--r--   0 user       (502) staff       (20)     2130 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/dummy_victor.py
--rw-r--r--   0 user       (502) staff       (20)     6666 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/internals.py
--rw-r--r--   0 user       (502) staff       (20)      642 2023-12-18 18:30:26.000000 Fragmenstein-1.0.3/tests/lab.py
--rw-r--r--   0 user       (502) staff       (20)     6321 2023-07-12 14:51:49.000000 Fragmenstein-1.0.3/tests/mapping.py
--rw-r--r--   0 user       (502) staff       (20)     4376 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/monster_combine.py
--rw-r--r--   0 user       (502) staff       (20)    11927 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/monster_place.py
--rw-r--r--   0 user       (502) staff       (20)     1323 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/multivictor.py
--rw-r--r--   0 user       (502) staff       (20)     4492 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/problems.py
--rw-r--r--   0 user       (502) staff       (20)     2814 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/victor_combine.py
--rw-r--r--   0 user       (502) staff       (20)     2911 2023-12-18 18:30:42.000000 Fragmenstein-1.0.3/tests/victor_discard.py
--rw-r--r--   0 user       (502) staff       (20)     4320 2023-07-07 14:11:40.000000 Fragmenstein-1.0.3/tests/walton.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.927778 Fragmenstein-1.0.4/
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:22.237211 Fragmenstein-1.0.4/Fragmenstein.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)    32364 2024-05-02 12:49:21.000000 Fragmenstein-1.0.4/Fragmenstein.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)    28971 2024-05-02 12:49:21.000000 Fragmenstein-1.0.4/Fragmenstein.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2024-05-02 12:49:21.000000 Fragmenstein-1.0.4/Fragmenstein.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)       55 2024-05-02 12:49:21.000000 Fragmenstein-1.0.4/Fragmenstein.egg-info/entry_points.txt
+-rw-r--r--   0 user       (502) staff       (20)      340 2024-05-02 12:49:21.000000 Fragmenstein-1.0.4/Fragmenstein.egg-info/requires.txt
+-rw-r--r--   0 user       (502) staff       (20)       19 2024-05-02 12:49:21.000000 Fragmenstein-1.0.4/Fragmenstein.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)     1069 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/LICENSE
+-rw-r--r--   0 user       (502) staff       (20)      317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/MANIFEST.in
+-rw-r--r--   0 user       (502) staff       (20)    32364 2024-05-02 12:49:28.924858 Fragmenstein-1.0.4/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)    31456 2024-02-21 13:22:43.000000 Fragmenstein-1.0.4/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:22.345134 Fragmenstein-1.0.4/fragmenstein/
+-rw-r--r--   0 user       (502) staff       (20)     2059 2024-02-21 13:07:25.000000 Fragmenstein-1.0.4/fragmenstein/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     1465 2024-02-15 19:52:24.000000 Fragmenstein-1.0.4/fragmenstein/_cli_defaults.py
+-rw-r--r--   0 user       (502) staff       (20)     1189 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/branding.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:22.459542 Fragmenstein-1.0.4/fragmenstein/cli/
+-rw-r--r--   0 user       (502) staff       (20)      826 2024-01-17 13:24:24.000000 Fragmenstein-1.0.4/fragmenstein/cli/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     3175 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/cli/base.py
+-rw-r--r--   0 user       (502) staff       (20)     5136 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/cli/laboratory.py
+-rw-r--r--   0 user       (502) staff       (20)     1474 2023-04-27 17:14:38.000000 Fragmenstein-1.0.4/fragmenstein/cli/monster.py
+-rw-r--r--   0 user       (502) staff       (20)     4904 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/cli/old.py
+-rw-r--r--   0 user       (502) staff       (20)      600 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/cli/parser.py
+-rw-r--r--   0 user       (502) staff       (20)     8987 2024-02-09 11:09:55.000000 Fragmenstein-1.0.4/fragmenstein/cli/pipeline.py
+-rw-r--r--   0 user       (502) staff       (20)     3287 2024-01-17 13:54:57.000000 Fragmenstein-1.0.4/fragmenstein/cli/utils.py
+-rw-r--r--   0 user       (502) staff       (20)     1730 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/cli/victor.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:22.465553 Fragmenstein-1.0.4/fragmenstein/demo/
+-rw-r--r--   0 user       (502) staff       (20)     2101 2023-09-18 15:43:25.000000 Fragmenstein-1.0.4/fragmenstein/demo/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     4515 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/_base_dataset_holder.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:24.479973 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/
+-rw-r--r--   0 user       (502) staff       (20)       85 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/__init__.py
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1592 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1592 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)      998 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1164 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1343 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1164 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1343 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      998 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      902 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol
+-rw-r--r--   0 user       (502) staff       (20)      902 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      570 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol
+-rw-r--r--   0 user       (502) staff       (20)      570 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      557 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1605 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0115.mol
+-rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0116.mol
+-rw-r--r--   0 user       (502) staff       (20)     1186 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0123.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0124.mol
+-rw-r--r--   0 user       (502) staff       (20)     1601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0131.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0132.mol
+-rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0137.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0138.mol
+-rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0139.mol
+-rw-r--r--   0 user       (502) staff       (20)     1531 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0142.mol
+-rw-r--r--   0 user       (502) staff       (20)     1614 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0148.mol
+-rw-r--r--   0 user       (502) staff       (20)     1518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0159.mol
+-rw-r--r--   0 user       (502) staff       (20)     1601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0161.mol
+-rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0163.mol
+-rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0178.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0179.mol
+-rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0180.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0182.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0188.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0190.mol
+-rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0193.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0204.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0206.mol
+-rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0212.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0213.mol
+-rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0223.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0224.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0226.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0227.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0228.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0231.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0255.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0263.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0271.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0277.mol
+-rw-r--r--   0 user       (502) staff       (20)      841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0282.mol
+-rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0283.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0284.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0301.mol
+-rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0302.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0303.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0305.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0306.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0309.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0319.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0321.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0326.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0328.mol
+-rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0333.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0337.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0338.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0341.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0343.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0344.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0345.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0346.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0347.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0348.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0354.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0357.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0358.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0360.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0361.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0365.mol
+-rw-r--r--   0 user       (502) staff       (20)     2073 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0371.mol
+-rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0373.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0375.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0378.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0379.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0380.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0381.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0385.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0387.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0392.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0394.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0396.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0397.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0398.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0402.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0404.mol
+-rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0411.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0412.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0415.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0417.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0433.mol
+-rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0436.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0437.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0439.mol
+-rw-r--r--   0 user       (502) staff       (20)     1505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0441.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0444.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0451.mol
+-rw-r--r--   0 user       (502) staff       (20)      745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0453.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0455.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0472.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0482.mol
+-rw-r--r--   0 user       (502) staff       (20)     1671 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0496.mol
+-rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0509.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0510.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0511.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0522.mol
+-rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0527.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0546.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0555.mol
+-rw-r--r--   0 user       (502) staff       (20)     1269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0564.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0565.mol
+-rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0567.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0568.mol
+-rw-r--r--   0 user       (502) staff       (20)     2156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0570.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0572.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0576.mol
+-rw-r--r--   0 user       (502) staff       (20)     1352 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0582.mol
+-rw-r--r--   0 user       (502) staff       (20)     1614 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0584.mol
+-rw-r--r--   0 user       (502) staff       (20)     1326 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0587.mol
+-rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0588.mol
+-rw-r--r--   0 user       (502) staff       (20)     3121 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0590.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x1493.mol
+-rw-r--r--   0 user       (502) staff       (20)     1933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x1494.mol
+-rw-r--r--   0 user       (502) staff       (20)   208424 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/template.pdb
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.063649 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/
+-rw-r--r--   0 user       (502) staff       (20)     2850 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6lze.mol
+-rw-r--r--   0 user       (502) staff       (20)     2933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol
+-rw-r--r--   0 user       (502) staff       (20)     2933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6w63.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol
+-rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol
+-rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol
+-rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol
+-rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol
+-rw-r--r--   0 user       (502) staff       (20)      404 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xbg.mol
+-rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol
+-rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol
+-rw-r--r--   0 user       (502) staff       (20)      972 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xch.mol
+-rw-r--r--   0 user       (502) staff       (20)      806 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol
+-rw-r--r--   0 user       (502) staff       (20)     2920 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol
+-rw-r--r--   0 user       (502) staff       (20)      640 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol
+-rw-r--r--   0 user       (502) staff       (20)     2658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol
+-rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol
+-rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol
+-rw-r--r--   0 user       (502) staff       (20)     3527 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol
+-rw-r--r--   0 user       (502) staff       (20)     3680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol
+-rw-r--r--   0 user       (502) staff       (20)     3680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol
+-rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol
+-rw-r--r--   0 user       (502) staff       (20)      832 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol
+-rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol
+-rw-r--r--   0 user       (502) staff       (20)      505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6yz6.mol
+-rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6zru.mol
+-rw-r--r--   0 user       (502) staff       (20)     2230 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7aku.mol
+-rw-r--r--   0 user       (502) staff       (20)      754 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7brp.mol
+-rw-r--r--   0 user       (502) staff       (20)      806 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7buy.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol
+-rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol
+-rw-r--r--   0 user       (502) staff       (20)      142 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c8b.mol
+-rw-r--r--   0 user       (502) staff       (20)     3820 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol
+-rw-r--r--   0 user       (502) staff       (20)     3667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7com.mol
+-rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol
+-rw-r--r--   0 user       (502) staff       (20)      142 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7d1m.mol
+-rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol
+-rw-r--r--   0 user       (502) staff       (20)     2850 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol
+-rw-r--r--   0 user       (502) staff       (20)     3527 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol
+-rw-r--r--   0 user       (502) staff       (20)      391 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7jr4.mol
+-rw-r--r--   0 user       (502) staff       (20)     3112 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol
+-rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7k40.mol
+-rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol
+-rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol
+-rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol
+-rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0072.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0104.mol
+-rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0107.mol
+-rw-r--r--   0 user       (502) staff       (20)     1239 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0161.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0165.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0177.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0194.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0195.mol
+-rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0305.mol
+-rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0336.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0350.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0354.mol
+-rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0376.mol
+-rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0387.mol
+-rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0390.mol
+-rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0395.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0397.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0398.mol
+-rw-r--r--   0 user       (502) staff       (20)     1348 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0425.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0426.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0434.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0464.mol
+-rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0478.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0499.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0540.mol
+-rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0669.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0678.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0689.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0691.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0692.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0705.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0708.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0731.mol
+-rw-r--r--   0 user       (502) staff       (20)     1693 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0734.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0736.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0748.mol
+-rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0749.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0752.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0755.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0759.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0769.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0770.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0771.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0774.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0786.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0820.mol
+-rw-r--r--   0 user       (502) staff       (20)     1846 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0830.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0831.mol
+-rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0874.mol
+-rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0887.mol
+-rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0946.mol
+-rw-r--r--   0 user       (502) staff       (20)     1737 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0967.mol
+-rw-r--r--   0 user       (502) staff       (20)     1309 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0978.mol
+-rw-r--r--   0 user       (502) staff       (20)     1392 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0981.mol
+-rw-r--r--   0 user       (502) staff       (20)      479 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0991.mol
+-rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0995.mol
+-rw-r--r--   0 user       (502) staff       (20)     1930 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10019.mol
+-rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1002.mol
+-rw-r--r--   0 user       (502) staff       (20)     1502 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10022.mol
+-rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10049.mol
+-rw-r--r--   0 user       (502) staff       (20)     2160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10082.mol
+-rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1012.mol
+-rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10150.mol
+-rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10155.mol
+-rw-r--r--   0 user       (502) staff       (20)     1323 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10172.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10178.mol
+-rw-r--r--   0 user       (502) staff       (20)     1502 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10201.mol
+-rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10236.mol
+-rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10237.mol
+-rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10247.mol
+-rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10248.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10296.mol
+-rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10306.mol
+-rw-r--r--   0 user       (502) staff       (20)     1668 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10314.mol
+-rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10322.mol
+-rw-r--r--   0 user       (502) staff       (20)     1943 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10324.mol
+-rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10327.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10329.mol
+-rw-r--r--   0 user       (502) staff       (20)     1668 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10334.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10338.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10355.mol
+-rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10359.mol
+-rw-r--r--   0 user       (502) staff       (20)     1930 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10371.mol
+-rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10377.mol
+-rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10387.mol
+-rw-r--r--   0 user       (502) staff       (20)     1764 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10392.mol
+-rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10395.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10396.mol
+-rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10403.mol
+-rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10417.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10419.mol
+-rw-r--r--   0 user       (502) staff       (20)     1751 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10421.mol
+-rw-r--r--   0 user       (502) staff       (20)     1751 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10422.mol
+-rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10423.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10466.mol
+-rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10473.mol
+-rw-r--r--   0 user       (502) staff       (20)     1400 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10474.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10476.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10478.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10484.mol
+-rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10488.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10494.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10506.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10513.mol
+-rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10525.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10535.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10555.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10559.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10565.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10566.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10575.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10598.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10604.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10606.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10610.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10626.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10638.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10645.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10678.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10679.mol
+-rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10700.mol
+-rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10710.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10723.mol
+-rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10728.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10733.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10756.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1077.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10787.mol
+-rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10789.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10800.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10801.mol
+-rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10812.mol
+-rw-r--r--   0 user       (502) staff       (20)     2352 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10820.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10834.mol
+-rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10856.mol
+-rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1086.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10862.mol
+-rw-r--r--   0 user       (502) staff       (20)     2697 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10870.mol
+-rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10871.mol
+-rw-r--r--   0 user       (502) staff       (20)     2435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10876.mol
+-rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10888.mol
+-rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10889.mol
+-rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10898.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10899.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10900.mol
+-rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10906.mol
+-rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1093.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10942.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10959.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10976.mol
+-rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10995.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10996.mol
+-rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11001.mol
+-rw-r--r--   0 user       (502) staff       (20)     2593 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1101.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11011.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11013.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11025.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11041.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11044.mol
+-rw-r--r--   0 user       (502) staff       (20)     1854 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11159.mol
+-rw-r--r--   0 user       (502) staff       (20)     2518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11164.mol
+-rw-r--r--   0 user       (502) staff       (20)     1854 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11186.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1119.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11204.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11208.mol
+-rw-r--r--   0 user       (502) staff       (20)     1675 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11212.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11223.mol
+-rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11225.mol
+-rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11231.mol
+-rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11233.mol
+-rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11254.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11258.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11271.mol
+-rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11294.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11313.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11317.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11318.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1132.mol
+-rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11339.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11346.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11354.mol
+-rw-r--r--   0 user       (502) staff       (20)     2269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11366.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11368.mol
+-rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11372.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11417.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11424.mol
+-rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11426.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11427.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11428.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11431.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11432.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11454.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11458.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11473.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11475.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11485.mol
+-rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11488.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11493.mol
+-rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11498.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11499.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11541.mol
+-rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11562.mol
+-rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11564.mol
+-rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11579.mol
+-rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11587.mol
+-rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11612.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1163.mol
+-rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11642.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11723.mol
+-rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11743.mol
+-rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11764.mol
+-rw-r--r--   0 user       (502) staff       (20)     2518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11790.mol
+-rw-r--r--   0 user       (502) staff       (20)     2435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11797.mol
+-rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11798.mol
+-rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11801.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11809.mol
+-rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11831.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1187.mol
+-rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11894.mol
+-rw-r--r--   0 user       (502) staff       (20)     2269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x12025.mol
+-rw-r--r--   0 user       (502) staff       (20)     2186 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x12073.mol
+-rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x12080.mol
+-rw-r--r--   0 user       (502) staff       (20)      907 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1226.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1235.mol
+-rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1237.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1249.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1308.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1311.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1334.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1336.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1348.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1351.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1358.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1374.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1375.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1380.mol
+-rw-r--r--   0 user       (502) staff       (20)     1239 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1382.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1384.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1385.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1386.mol
+-rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1392.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1402.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1412.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1418.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1425.mol
+-rw-r--r--   0 user       (502) staff       (20)     1488 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1458.mol
+-rw-r--r--   0 user       (502) staff       (20)     1073 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1478.mol
+-rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1493.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2052.mol
+-rw-r--r--   0 user       (502) staff       (20)      824 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2097.mol
+-rw-r--r--   0 user       (502) staff       (20)      741 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2119.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2193.mol
+-rw-r--r--   0 user       (502) staff       (20)     2497 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2540.mol
+-rw-r--r--   0 user       (502) staff       (20)     1929 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2562.mol
+-rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2563.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2569.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2572.mol
+-rw-r--r--   0 user       (502) staff       (20)     1929 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2581.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2600.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2608.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2643.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2646.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2649.mol
+-rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2659.mol
+-rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2694.mol
+-rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2703.mol
+-rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2705.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2754.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2764.mol
+-rw-r--r--   0 user       (502) staff       (20)     3008 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2776.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2779.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2908.mol
+-rw-r--r--   0 user       (502) staff       (20)     2178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2910.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2912.mol
+-rw-r--r--   0 user       (502) staff       (20)     1846 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2929.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2964.mol
+-rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2971.mol
+-rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3077.mol
+-rw-r--r--   0 user       (502) staff       (20)     2261 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3080.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3108.mol
+-rw-r--r--   0 user       (502) staff       (20)     2829 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3110.mol
+-rw-r--r--   0 user       (502) staff       (20)     2663 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3113.mol
+-rw-r--r--   0 user       (502) staff       (20)     2580 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3115.mol
+-rw-r--r--   0 user       (502) staff       (20)     2759 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3117.mol
+-rw-r--r--   0 user       (502) staff       (20)     2331 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3124.mol
+-rw-r--r--   0 user       (502) staff       (20)     2427 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3298.mol
+-rw-r--r--   0 user       (502) staff       (20)     2191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3303.mol
+-rw-r--r--   0 user       (502) staff       (20)     2261 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3305.mol
+-rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3324.mol
+-rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3325.mol
+-rw-r--r--   0 user       (502) staff       (20)     1488 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3333.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3348.mol
+-rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3351.mol
+-rw-r--r--   0 user       (502) staff       (20)     2414 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3359.mol
+-rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3366.mol
+-rw-r--r--   0 user       (502) staff       (20)       76 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)   379172 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/template.pdb
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.194811 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/
+-rw-r--r--   0 user       (502) staff       (20)    17574 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/5SB7_mergers.sdf
+-rw-r--r--   0 user       (502) staff       (20)     1254 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/F584.mol
+-rw-r--r--   0 user       (502) staff       (20)      144 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/__init__.py
+-rwxr-xr-x   0 user       (502) staff       (20)   467127 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/apo_example1.pdb
+-rw-r--r--   0 user       (502) staff       (20)     6701 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/dummy.pdb
+-rwxr-xr-x   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/mac-x0138.mol
+-rwxr-xr-x   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/mac-x0398.mol
+-rw-r--r--   0 user       (502) staff       (20)     4580 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/placed_example1.mol
+-rw-r--r--   0 user       (502) staff       (20)      753 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/rototoluene.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/toluene.mol
+-rw-r--r--   0 user       (502) staff       (20)      758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/transtoluene.mol
+-rw-r--r--   0 user       (502) staff       (20)      763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/transtoluene2.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/x0032_0A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1421 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/demo/test_mols/x0103_0A.mol
+-rw-r--r--   0 user       (502) staff       (20)     3115 2024-02-21 13:07:25.000000 Fragmenstein-1.0.4/fragmenstein/display.py
+-rw-r--r--   0 user       (502) staff       (20)    56342 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/divergent_colors.json
+-rw-r--r--   0 user       (502) staff       (20)     1801 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/error.py
+-rw-r--r--   0 user       (502) staff       (20)     6425 2023-12-18 18:30:24.000000 Fragmenstein-1.0.4/fragmenstein/extraction_funs.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.228496 Fragmenstein-1.0.4/fragmenstein/faux_victors/
+-rw-r--r--   0 user       (502) staff       (20)     1178 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/faux_victors/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     4798 2024-05-02 12:01:05.000000 Fragmenstein-1.0.4/fragmenstein/faux_victors/brics.py
+-rw-r--r--   0 user       (502) staff       (20)    13343 2023-12-11 16:13:15.000000 Fragmenstein-1.0.4/fragmenstein/faux_victors/mcs_monster.py
+-rw-r--r--   0 user       (502) staff       (20)     1018 2024-03-13 10:07:19.000000 Fragmenstein-1.0.4/fragmenstein/faux_victors/mcs_victor.py
+-rw-r--r--   0 user       (502) staff       (20)     5743 2024-03-13 10:05:02.000000 Fragmenstein-1.0.4/fragmenstein/faux_victors/no_pyrosetta.py
+-rw-r--r--   0 user       (502) staff       (20)     3648 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/faux_victors/others.py
+-rw-r--r--   0 user       (502) staff       (20)     2712 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/faux_victors/quick.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.264109 Fragmenstein-1.0.4/fragmenstein/igor/
+-rw-r--r--   0 user       (502) staff       (20)     2432 2023-04-26 12:35:21.000000 Fragmenstein-1.0.4/fragmenstein/igor/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)      817 2023-04-26 12:34:04.000000 Fragmenstein-1.0.4/fragmenstein/igor/_igor_base.py
+-rw-r--r--   0 user       (502) staff       (20)     7774 2024-01-16 11:13:08.000000 Fragmenstein-1.0.4/fragmenstein/igor/_igor_init.py
+-rw-r--r--   0 user       (502) staff       (20)    18406 2024-05-02 12:01:05.000000 Fragmenstein-1.0.4/fragmenstein/igor/_igor_min.py
+-rw-r--r--   0 user       (502) staff       (20)    12183 2024-01-17 13:54:57.000000 Fragmenstein-1.0.4/fragmenstein/igor/_igor_utils.py
+-rw-r--r--   0 user       (502) staff       (20)     1193 2023-10-27 10:05:23.000000 Fragmenstein-1.0.4/fragmenstein/igor/pyrosetta_import.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.313470 Fragmenstein-1.0.4/fragmenstein/laboratory/
+-rw-r--r--   0 user       (502) staff       (20)     1565 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/laboratory/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    12423 2024-04-04 13:08:08.000000 Fragmenstein-1.0.4/fragmenstein/laboratory/_base.py
+-rw-r--r--   0 user       (502) staff       (20)     5609 2024-03-13 13:33:10.000000 Fragmenstein-1.0.4/fragmenstein/laboratory/_combine.py
+-rw-r--r--   0 user       (502) staff       (20)    13365 2024-02-15 19:30:09.000000 Fragmenstein-1.0.4/fragmenstein/laboratory/_extras.py
+-rw-r--r--   0 user       (502) staff       (20)     5089 2024-03-13 13:36:49.000000 Fragmenstein-1.0.4/fragmenstein/laboratory/_place.py
+-rw-r--r--   0 user       (502) staff       (20)    10885 2024-03-13 12:16:17.000000 Fragmenstein-1.0.4/fragmenstein/laboratory/_score.py
+-rw-r--r--   0 user       (502) staff       (20)     1419 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/laboratory/validator.py
+-rw-r--r--   0 user       (502) staff       (20)     1715 2024-02-22 13:26:29.000000 Fragmenstein-1.0.4/fragmenstein/legacy.py
+-rw-r--r--   0 user       (502) staff       (20)    21721 2024-05-02 12:01:05.000000 Fragmenstein-1.0.4/fragmenstein/m_rmsd.py
+-rw-r--r--   0 user       (502) staff       (20)     4418 2024-02-21 12:47:15.000000 Fragmenstein-1.0.4/fragmenstein/mol3d_display.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.417019 Fragmenstein-1.0.4/fragmenstein/monster/
+-rw-r--r--   0 user       (502) staff       (20)     6504 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/monster/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     9153 2024-05-02 12:12:36.000000 Fragmenstein-1.0.4/fragmenstein/monster/_base.py
+-rw-r--r--   0 user       (502) staff       (20)    53393 2024-05-02 12:26:18.000000 Fragmenstein-1.0.4/fragmenstein/monster/_collapse_ring.py
+-rw-r--r--   0 user       (502) staff       (20)     4053 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/monster/_combine.py
+-rw-r--r--   0 user       (502) staff       (20)    19282 2023-07-29 22:48:42.000000 Fragmenstein-1.0.4/fragmenstein/monster/_communal.py
+-rw-r--r--   0 user       (502) staff       (20)    16303 2024-04-04 13:52:48.000000 Fragmenstein-1.0.4/fragmenstein/monster/_ff.py
+-rw-r--r--   0 user       (502) staff       (20)     6371 2024-04-04 15:01:11.000000 Fragmenstein-1.0.4/fragmenstein/monster/_join_neighboring.py
+-rw-r--r--   0 user       (502) staff       (20)    16374 2024-05-02 12:26:18.000000 Fragmenstein-1.0.4/fragmenstein/monster/_merge.py
+-rw-r--r--   0 user       (502) staff       (20)     1722 2024-05-02 12:26:18.000000 Fragmenstein-1.0.4/fragmenstein/monster/_modification_logging.py
+-rw-r--r--   0 user       (502) staff       (20)     8371 2024-03-13 12:01:11.000000 Fragmenstein-1.0.4/fragmenstein/monster/_place.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.478829 Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    13701 2023-07-12 11:22:55.000000 Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_expand.py
+-rw-r--r--   0 user       (502) staff       (20)     1106 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_full.py
+-rw-r--r--   0 user       (502) staff       (20)     8354 2024-05-02 12:26:18.000000 Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_make_chimera.py
+-rw-r--r--   0 user       (502) staff       (20)    10200 2023-07-12 13:14:33.000000 Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_mappings.py
+-rw-r--r--   0 user       (502) staff       (20)     9219 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_no_blending.py
+-rw-r--r--   0 user       (502) staff       (20)     9905 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_partial.py
+-rw-r--r--   0 user       (502) staff       (20)     6957 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_refine.py
+-rw-r--r--   0 user       (502) staff       (20)    10464 2024-02-21 12:47:15.000000 Fragmenstein-1.0.4/fragmenstein/monster/_util_compare.py
+-rw-r--r--   0 user       (502) staff       (20)    14404 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/monster/_utility.py
+-rw-r--r--   0 user       (502) staff       (20)     1939 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/monster/bond_provenance.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.510858 Fragmenstein-1.0.4/fragmenstein/monster/mcs_mapping/
+-rw-r--r--   0 user       (502) staff       (20)      342 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/monster/mcs_mapping/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    11854 2023-07-12 14:59:39.000000 Fragmenstein-1.0.4/fragmenstein/monster/mcs_mapping/compare_atom.py
+-rw-r--r--   0 user       (502) staff       (20)     1127 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/monster/mcs_mapping/types.py
+-rw-r--r--   0 user       (502) staff       (20)     5354 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/monster/mcs_mapping/utils.py
+-rw-r--r--   0 user       (502) staff       (20)     5087 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/monster/positional_mapping.py
+-rw-r--r--   0 user       (502) staff       (20)    21692 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/monster/unmerge_mapper.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.526539 Fragmenstein-1.0.4/fragmenstein/mpro/
+-rw-r--r--   0 user       (502) staff       (20)     6088 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/mpro/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     1439 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/mpro/dataframe.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.548726 Fragmenstein-1.0.4/fragmenstein/multivictor/
+-rw-r--r--   0 user       (502) staff       (20)       70 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/multivictor/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     3254 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/multivictor/multivictor.py
+-rw-r--r--   0 user       (502) staff       (20)     5508 2024-02-21 10:33:08.000000 Fragmenstein-1.0.4/fragmenstein/ngl_display.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.574777 Fragmenstein-1.0.4/fragmenstein/openmm/
+-rw-r--r--   0 user       (502) staff       (20)       59 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/openmm/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    24977 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/openmm/fritz.py
+-rw-r--r--   0 user       (502) staff       (20)     7011 2024-03-13 10:05:02.000000 Fragmenstein-1.0.4/fragmenstein/openmm/openvictor.py
+-rw-r--r--   0 user       (502) staff       (20)     2318 2023-11-23 13:18:06.000000 Fragmenstein-1.0.4/fragmenstein/settings.py
+-rw-r--r--   0 user       (502) staff       (20)      676 2024-05-02 12:46:36.000000 Fragmenstein-1.0.4/fragmenstein/version.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.716300 Fragmenstein-1.0.4/fragmenstein/victor/
+-rw-r--r--   0 user       (502) staff       (20)     6217 2024-03-13 11:43:40.000000 Fragmenstein-1.0.4/fragmenstein/victor/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)      802 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/victor/_loggerwriter.py
+-rw-r--r--   0 user       (502) staff       (20)     9613 2024-03-13 11:55:09.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_base.py
+-rw-r--r--   0 user       (502) staff       (20)     7215 2024-03-13 11:43:40.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_combine.py
+-rw-r--r--   0 user       (502) staff       (20)    18020 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_common.py
+-rw-r--r--   0 user       (502) staff       (20)     5547 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_igor.py
+-rw-r--r--   0 user       (502) staff       (20)     4674 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_journal.py
+-rw-r--r--   0 user       (502) staff       (20)      338 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_mode.py
+-rw-r--r--   0 user       (502) staff       (20)      829 2023-12-18 18:30:40.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_overridables.py
+-rw-r--r--   0 user       (502) staff       (20)     9337 2024-04-04 13:35:48.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_place.py
+-rw-r--r--   0 user       (502) staff       (20)     9579 2024-04-04 14:52:49.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_plonk.py
+-rw-r--r--   0 user       (502) staff       (20)     1863 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_safety.py
+-rw-r--r--   0 user       (502) staff       (20)     6816 2024-02-13 16:18:01.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_show.py
+-rw-r--r--   0 user       (502) staff       (20)     4674 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_store.py
+-rw-r--r--   0 user       (502) staff       (20)    24750 2024-02-13 15:36:41.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_utils.py
+-rw-r--r--   0 user       (502) staff       (20)     2202 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/fragmenstein/victor/_victor_validate.py
+-rw-r--r--   0 user       (502) staff       (20)     5650 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/victor/minimalPDB.py
+-rw-r--r--   0 user       (502) staff       (20)    10778 2023-08-22 10:47:34.000000 Fragmenstein-1.0.4/fragmenstein/victor/plip.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.775900 Fragmenstein-1.0.4/fragmenstein/walton/
+-rw-r--r--   0 user       (502) staff       (20)     2277 2024-02-21 10:33:08.000000 Fragmenstein-1.0.4/fragmenstein/walton/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     8226 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/walton/_advmoves.py
+-rw-r--r--   0 user       (502) staff       (20)     4004 2024-02-21 10:52:06.000000 Fragmenstein-1.0.4/fragmenstein/walton/_art.py
+-rw-r--r--   0 user       (502) staff       (20)     4333 2024-02-21 13:07:25.000000 Fragmenstein-1.0.4/fragmenstein/walton/_base.py
+-rw-r--r--   0 user       (502) staff       (20)     6289 2024-01-19 13:58:39.000000 Fragmenstein-1.0.4/fragmenstein/walton/_movements.py
+-rw-r--r--   0 user       (502) staff       (20)     1693 2023-04-25 12:43:41.000000 Fragmenstein-1.0.4/fragmenstein/walton/_polygon.py
+-rw-r--r--   0 user       (502) staff       (20)     1033 2024-02-22 13:18:08.000000 Fragmenstein-1.0.4/requirements.txt
+-rw-r--r--   0 user       (502) staff       (20)       38 2024-05-02 12:49:28.928122 Fragmenstein-1.0.4/setup.cfg
+-rw-r--r--   0 user       (502) staff       (20)     3377 2024-05-02 12:46:36.000000 Fragmenstein-1.0.4/setup.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-02 12:49:28.922174 Fragmenstein-1.0.4/tests/
+-rw-r--r--   0 user       (502) staff       (20)     1689 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/MPro_combine.py
+-rw-r--r--   0 user       (502) staff       (20)     4498 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/MPro_place.py
+-rw-r--r--   0 user       (502) staff       (20)      404 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)      725 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/baffled.py
+-rw-r--r--   0 user       (502) staff       (20)     2623 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/cli.py
+-rw-r--r--   0 user       (502) staff       (20)     2130 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/dummy_victor.py
+-rw-r--r--   0 user       (502) staff       (20)     6666 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/internals.py
+-rw-r--r--   0 user       (502) staff       (20)      642 2023-12-18 18:30:26.000000 Fragmenstein-1.0.4/tests/lab.py
+-rw-r--r--   0 user       (502) staff       (20)     6321 2023-07-12 14:51:49.000000 Fragmenstein-1.0.4/tests/mapping.py
+-rw-r--r--   0 user       (502) staff       (20)     4376 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/monster_combine.py
+-rw-r--r--   0 user       (502) staff       (20)    11927 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/monster_place.py
+-rw-r--r--   0 user       (502) staff       (20)     1323 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/multivictor.py
+-rw-r--r--   0 user       (502) staff       (20)     4492 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/problems.py
+-rw-r--r--   0 user       (502) staff       (20)     2814 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/victor_combine.py
+-rw-r--r--   0 user       (502) staff       (20)     2911 2023-12-18 18:30:42.000000 Fragmenstein-1.0.4/tests/victor_discard.py
+-rw-r--r--   0 user       (502) staff       (20)     4320 2023-07-07 14:11:40.000000 Fragmenstein-1.0.4/tests/walton.py
```

### Comparing `Fragmenstein-1.0.3/Fragmenstein.egg-info/PKG-INFO` & `Fragmenstein-1.0.4/Fragmenstein.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fragmenstein
-Version: 1.0.3
+Version: 1.0.4
 Summary: Merging, linking and placing compounds by stitching them together like a reanimated corpse
 Home-page: https://github.com/matteoferla/Fragmenstein
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `Fragmenstein-1.0.3/Fragmenstein.egg-info/SOURCES.txt` & `Fragmenstein-1.0.4/Fragmenstein.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/LICENSE` & `Fragmenstein-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/PKG-INFO` & `Fragmenstein-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fragmenstein
-Version: 1.0.3
+Version: 1.0.4
 Summary: Merging, linking and placing compounds by stitching them together like a reanimated corpse
 Home-page: https://github.com/matteoferla/Fragmenstein
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `Fragmenstein-1.0.3/README.md` & `Fragmenstein-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/__init__.py` & `Fragmenstein-1.0.4/fragmenstein/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/_cli_defaults.py` & `Fragmenstein-1.0.4/fragmenstein/_cli_defaults.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/branding.py` & `Fragmenstein-1.0.4/fragmenstein/branding.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/cli/__init__.py` & `Fragmenstein-1.0.4/fragmenstein/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/cli/base.py` & `Fragmenstein-1.0.4/fragmenstein/cli/base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/cli/laboratory.py` & `Fragmenstein-1.0.4/fragmenstein/cli/laboratory.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/cli/monster.py` & `Fragmenstein-1.0.4/fragmenstein/cli/monster.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/cli/old.py` & `Fragmenstein-1.0.4/fragmenstein/cli/old.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/cli/parser.py` & `Fragmenstein-1.0.4/fragmenstein/cli/parser.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/cli/pipeline.py` & `Fragmenstein-1.0.4/fragmenstein/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/cli/utils.py` & `Fragmenstein-1.0.4/fragmenstein/cli/utils.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/cli/victor.py` & `Fragmenstein-1.0.4/fragmenstein/cli/victor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/__init__.py` & `Fragmenstein-1.0.4/fragmenstein/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/_base_dataset_holder.py` & `Fragmenstein-1.0.4/fragmenstein/demo/_base_dataset_holder.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0115.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0115.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0116.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0116.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0123.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0123.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0124.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0124.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0131.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0131.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0132.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0132.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0137.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0137.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0138.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0138.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0139.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0139.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0142.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0142.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0148.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0148.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0159.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0159.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0161.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0161.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0163.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0163.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0178.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0178.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0179.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0179.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0180.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0180.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0182.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0182.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0188.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0188.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0190.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0190.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0193.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0193.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0204.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0204.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0206.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0206.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0212.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0212.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0213.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0213.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0223.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0223.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0224.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0224.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0226.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0226.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0227.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0227.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0228.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0228.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0231.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0231.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0255.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0255.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0263.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0263.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0271.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0271.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0277.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0277.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0282.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0282.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0283.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0283.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0284.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0284.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0301.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0301.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0302.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0302.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0303.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0303.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0305.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0305.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0306.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0306.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0309.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0309.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0319.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0319.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0321.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0321.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0326.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0326.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0328.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0328.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0333.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0333.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0337.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0337.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0338.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0338.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0341.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0341.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0343.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0343.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0344.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0344.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0345.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0345.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0346.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0346.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0347.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0347.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0348.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0348.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0354.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0354.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0357.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0357.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0358.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0358.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0360.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0360.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0361.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0361.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0365.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0365.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0371.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0371.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0373.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0373.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0375.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0375.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0378.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0378.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0379.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0379.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0380.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0380.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0381.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0381.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0385.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0385.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0387.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0387.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0392.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0392.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0394.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0394.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0396.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0396.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0397.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0397.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0398.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0398.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0402.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0402.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0404.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0404.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0411.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0411.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0412.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0412.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0415.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0415.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0417.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0417.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0433.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0433.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0436.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0436.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0437.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0437.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0439.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0439.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0441.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0441.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0444.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0444.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0451.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0451.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0453.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0453.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0455.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0455.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0472.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0472.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0482.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0482.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0496.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0496.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0509.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0509.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0510.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0510.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0511.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0511.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0522.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0522.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0527.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0527.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0546.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0546.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0555.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0555.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0564.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0564.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0565.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0565.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0567.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0567.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0568.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0568.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0570.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0570.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0572.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0572.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0576.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0576.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0582.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0582.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0584.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0584.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0587.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0587.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0588.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0588.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x0590.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x0590.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x1493.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x1493.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/mac-x1494.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/mac-x1494.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mac1_mols/template.pdb` & `Fragmenstein-1.0.4/fragmenstein/demo/mac1_mols/template.pdb`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6lze.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6lze.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6w63.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6w63.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xch.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xch.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-6zru.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-6zru.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7aku.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7aku.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7brp.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7brp.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7buy.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7buy.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7com.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7com.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7k40.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7k40.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0072.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0072.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0104.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0104.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0107.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0107.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0161.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0161.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0165.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0165.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0177.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0177.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0194.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0194.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0195.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0195.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0305.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0305.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0336.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0336.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0350.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0350.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0354.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0354.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0376.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0376.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0387.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0387.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0390.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0390.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0395.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0395.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0397.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0397.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0398.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0398.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0425.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0425.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0426.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0426.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0434.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0434.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0464.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0464.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0478.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0478.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0499.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0499.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0540.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0540.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0669.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0669.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0678.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0678.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0689.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0689.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0691.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0691.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0692.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0692.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0705.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0705.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0708.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0708.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0731.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0731.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0734.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0734.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0736.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0736.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0748.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0748.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0749.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0749.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0752.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0752.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0755.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0755.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0759.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0759.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0769.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0769.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0770.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0770.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0771.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0771.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0774.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0774.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0786.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0786.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0820.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0820.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0830.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0830.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0831.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0831.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0874.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0874.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0887.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0887.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0946.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0946.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0967.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0967.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0978.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0978.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0981.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0981.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x0995.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x0995.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10019.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10019.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1002.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1002.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10022.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10022.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10049.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10049.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10082.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10082.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1012.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1012.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10150.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10150.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10155.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10155.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10172.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10172.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10178.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10178.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10201.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10201.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10236.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10236.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10237.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10237.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10247.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10247.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10248.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10248.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10296.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10296.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10306.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10306.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10314.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10314.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10322.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10322.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10324.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10324.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10327.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10327.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10329.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10329.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10334.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10334.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10338.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10338.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10355.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10355.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10359.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10359.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10371.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10371.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10377.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10377.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10387.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10387.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10392.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10392.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10395.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10395.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10396.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10396.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10403.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10403.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10417.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10417.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10419.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10419.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10421.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10421.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10422.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10422.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10423.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10423.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10466.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10466.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10473.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10473.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10474.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10474.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10476.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10476.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10478.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10478.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10484.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10484.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10488.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10488.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10494.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10494.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10506.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10506.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10513.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10513.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10525.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10525.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10535.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10535.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10555.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10555.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10559.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10559.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10565.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10565.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10566.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10566.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10575.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10575.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10598.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10598.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10604.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10604.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10606.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10606.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10610.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10610.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10626.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10626.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10638.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10638.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10645.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10645.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10678.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10678.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10679.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10679.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10700.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10700.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10710.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10710.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10723.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10723.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10728.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10728.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10733.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10733.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10756.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10756.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1077.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1077.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10787.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10787.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10789.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10789.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10800.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10800.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10801.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10801.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10812.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10812.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10820.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10820.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10834.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10834.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10856.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10856.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1086.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1086.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10862.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10862.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10870.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10870.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10871.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10871.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10876.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10876.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10888.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10888.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10889.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10889.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10898.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10898.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10899.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10899.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10900.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10900.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10906.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10906.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1093.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1093.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10942.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10942.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10959.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10959.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10976.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10976.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10995.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10995.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x10996.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x10996.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11001.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11001.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1101.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1101.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11011.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11011.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11013.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11013.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11025.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11025.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11041.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11041.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11044.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11044.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11159.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11159.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11164.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11164.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11186.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11186.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1119.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1119.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11204.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11204.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11208.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11208.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11212.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11212.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11223.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11223.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11225.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11225.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11231.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11231.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11233.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11233.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11254.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11254.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11258.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11258.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11271.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11271.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11294.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11294.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11313.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11313.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11317.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11317.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11318.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11318.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1132.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1132.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11339.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11339.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11346.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11346.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11354.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11354.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11366.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11366.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11368.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11368.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11372.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11372.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11417.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11417.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11424.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11424.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11426.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11426.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11427.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11427.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11428.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11428.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11431.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11431.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11432.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11432.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11454.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11454.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11458.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11458.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11473.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11473.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11475.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11475.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11485.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11485.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11488.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11488.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11493.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11493.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11498.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11498.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11499.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11499.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11541.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11541.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11562.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11562.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11564.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11564.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11579.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11579.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11587.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11587.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11612.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11612.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1163.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1163.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11642.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11642.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11723.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11723.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11743.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11743.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11764.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11764.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11790.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11790.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11797.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11797.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11798.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11798.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11801.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11801.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11809.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11809.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11831.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11831.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1187.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1187.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x11894.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x11894.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x12025.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x12025.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x12073.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x12073.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x12080.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x12080.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1226.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1226.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1235.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1235.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1237.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1237.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1249.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1249.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1308.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1308.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1311.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1311.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1334.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1334.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1336.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1336.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1348.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1348.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1351.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1351.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1358.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1358.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1374.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1374.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1375.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1375.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1380.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1380.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1382.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1382.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1384.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1384.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1385.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1385.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1386.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1386.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1392.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1392.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1402.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1402.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1412.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1412.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1418.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1418.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1425.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1425.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1458.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1458.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1478.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1478.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x1493.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x1493.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2052.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2052.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2097.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2097.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2119.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2119.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2193.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2193.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2540.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2540.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2562.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2562.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2563.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2563.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2569.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2569.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2572.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2572.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2581.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2581.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2600.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2600.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2608.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2608.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2643.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2643.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2646.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2646.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2649.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2649.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2659.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2659.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2694.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2694.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2703.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2703.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2705.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2705.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2754.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2754.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2764.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2764.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2776.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2776.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2779.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2779.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2908.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2908.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2910.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2910.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2912.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2912.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2929.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2929.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2964.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2964.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x2971.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x2971.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3077.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3077.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3080.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3080.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3108.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3108.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3110.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3110.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3113.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3113.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3115.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3115.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3117.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3117.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3124.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3124.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3298.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3298.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3303.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3303.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3305.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3305.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3324.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3324.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3325.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3325.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3333.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3333.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3348.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3348.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3351.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3351.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3359.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3359.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/Mpro-x3366.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/Mpro-x3366.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/mpro_mols/template.pdb` & `Fragmenstein-1.0.4/fragmenstein/demo/mpro_mols/template.pdb`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/5SB7_mergers.sdf` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/5SB7_mergers.sdf`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/F584.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/F584.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/apo_example1.pdb` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/apo_example1.pdb`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/dummy.pdb` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/dummy.pdb`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/mac-x0138.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/mac-x0138.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/mac-x0398.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/mac-x0398.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/placed_example1.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/placed_example1.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/rototoluene.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/rototoluene.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/toluene.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/toluene.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/transtoluene.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/transtoluene.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/transtoluene2.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/transtoluene2.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/x0032_0A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/x0032_0A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/demo/test_mols/x0103_0A.mol` & `Fragmenstein-1.0.4/fragmenstein/demo/test_mols/x0103_0A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/display.py` & `Fragmenstein-1.0.4/fragmenstein/display.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/divergent_colors.json` & `Fragmenstein-1.0.4/fragmenstein/divergent_colors.json`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/error.py` & `Fragmenstein-1.0.4/fragmenstein/error.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/extraction_funs.py` & `Fragmenstein-1.0.4/fragmenstein/extraction_funs.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/faux_victors/__init__.py` & `Fragmenstein-1.0.4/fragmenstein/faux_victors/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/faux_victors/brics.py` & `Fragmenstein-1.0.4/fragmenstein/faux_victors/brics.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                      'max_reached': False}
         self.fragments: List[Chem.Mol] = []
 
     def decompose(self, mol: Chem.Mol) -> List[Chem.Mol]:
         name = mol.GetProp('_Name')
         index = mol.GetIntProp('decompose_index')
         for atom in mol.GetAtoms():
-            atom.SetProp('ori_name', name)
+            atom.SetProp('ori_name', str(name))
             atom.SetIntProp('ori_i', atom.GetIdx())
         fragments = list(BRICS.BRICSDecompose(mol, keepNonLeafNodes=False, returnMols=True))
         # label
         for i, frag in enumerate(fragments):
             # this is a waste of time:
             frag.SetProp('_Name', f'{name}#{i}')
             for atom in frag.GetAtoms():
```

### Comparing `Fragmenstein-1.0.3/fragmenstein/faux_victors/mcs_monster.py` & `Fragmenstein-1.0.4/fragmenstein/faux_victors/mcs_monster.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/faux_victors/mcs_victor.py` & `Fragmenstein-1.0.4/fragmenstein/faux_victors/mcs_victor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/faux_victors/no_pyrosetta.py` & `Fragmenstein-1.0.4/fragmenstein/faux_victors/no_pyrosetta.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/faux_victors/others.py` & `Fragmenstein-1.0.4/fragmenstein/faux_victors/others.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/faux_victors/quick.py` & `Fragmenstein-1.0.4/fragmenstein/faux_victors/quick.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/igor/__init__.py` & `Fragmenstein-1.0.4/fragmenstein/igor/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/igor/_igor_base.py` & `Fragmenstein-1.0.4/fragmenstein/igor/_igor_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/igor/_igor_init.py` & `Fragmenstein-1.0.4/fragmenstein/igor/_igor_init.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/igor/_igor_min.py` & `Fragmenstein-1.0.4/fragmenstein/igor/_igor_min.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         # it is likely impossible and Igor does not know so, it is likely fine...
         ligand: Chem.Mol = Chem.SplitMolByPDBResidues(holo, whiteList=[ligand_resn])[ligand_resn]
         if add_dummy:
             ligand = add_dummy_to_mol(ligand, ligand_resn, holo)
         # store PDB atom names as molFileAlias
         for a in ligand.GetAtoms():
             name = a.GetPDBResidueInfo().GetName()
-            a.SetProp('molFileAlias', name)
+            a.SetProp('molFileAlias', str(a))
         # done. Bond order fixed later
         return ligand
 
     def make_ligand_only_pose(self) -> pyrosetta.Pose:
         """
 
         :return:
```

### Comparing `Fragmenstein-1.0.3/fragmenstein/igor/_igor_utils.py` & `Fragmenstein-1.0.4/fragmenstein/igor/_igor_utils.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/igor/pyrosetta_import.py` & `Fragmenstein-1.0.4/fragmenstein/igor/pyrosetta_import.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/laboratory/__init__.py` & `Fragmenstein-1.0.4/fragmenstein/laboratory/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/laboratory/_base.py` & `Fragmenstein-1.0.4/fragmenstein/laboratory/_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/laboratory/_combine.py` & `Fragmenstein-1.0.4/fragmenstein/laboratory/_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/laboratory/_extras.py` & `Fragmenstein-1.0.4/fragmenstein/laboratory/_extras.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/laboratory/_place.py` & `Fragmenstein-1.0.4/fragmenstein/laboratory/_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/laboratory/_score.py` & `Fragmenstein-1.0.4/fragmenstein/laboratory/_score.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/laboratory/validator.py` & `Fragmenstein-1.0.4/fragmenstein/laboratory/validator.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/legacy.py` & `Fragmenstein-1.0.4/fragmenstein/legacy.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/m_rmsd.py` & `Fragmenstein-1.0.4/fragmenstein/m_rmsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
             return  # no hits
         hitdex: Dict[str, Chem.Mol] = {hit.GetProp('_Name'): hit for hit in hits}
         for origin in origins:
             if origin == 'none':
                 # thank you human.
                 continue
             hit_name, idx = re.match(r'(.*)\.(\d+)', origin).groups()
-            atom.SetProp('_ori_name', hit_name)
+            atom.SetProp('_ori_name', str(hit_name))
             if hit_name not in hitdex:
                 return
             ref_conf = hitdex[hit_name].GetConformer()
             ref_xyz: Point3D = ref_conf.GetAtomPosition(int(idx))
             points.append(list(ref_xyz))  # noqa this is okay
         if points:
             xyz = np.mean(points, axis=0)
```

### Comparing `Fragmenstein-1.0.3/fragmenstein/mol3d_display.py` & `Fragmenstein-1.0.4/fragmenstein/mol3d_display.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/__init__.py` & `Fragmenstein-1.0.4/fragmenstein/monster/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_base.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         :return:
         """
         conf = mol.GetConformer()
         name = mol.GetProp('_Name')
         for i, atom in enumerate(mol.GetAtoms()):
             pos = conf.GetAtomPosition(i)
             atom.SetIntProp('_ori_i', i)
-            atom.SetProp('_ori_name', name)
+            atom.SetProp('_ori_name', str(name))
             atom.SetDoubleProp('_x', pos.x)
             atom.SetDoubleProp('_y', pos.y)
             atom.SetDoubleProp('_z', pos.z)
         return mol
 
     @property
     def matched(self) -> List[str]:
```

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_collapse_ring.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_collapse_ring.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             zs = []
             elements = []
             # add elemental ring
             c = mol.AddAtom(Chem.Atom('C'))
             center_idxs.append(c)
             central = mol.GetAtomWithIdx(c)
             name = mol.GetProp('_Name') if mol.HasProp('_Name') else '???'
-            central.SetProp('_ori_name', name),
+            central.SetProp('_ori_name', str(name)),
             # get data for storage
             for i in atomset:
                 old2center[i].append(c)
                 atom = mol.GetAtomWithIdx(i)
                 neigh_i = [a.GetIdx() for a in atom.GetNeighbors()]
                 neighs.append(neigh_i)
                 bond = [mol.GetBondBetweenAtoms(i, j).GetBondType().name for j in neigh_i]
@@ -973,15 +973,15 @@
                 second = frags[p[1][0]]
                 mol = self.join_neighboring_mols(first, second)
                 frags.remove(first)
                 frags.remove(second)
                 # ---- reset variables ---------
                 for part in frags:
                     mol = Chem.CombineMols(mol, part)
-                    mol.SetProp('_Name', name)
+                    mol.SetProp('_Name', str(name))
                 frags = Chem.GetMolFrags(mol, asMols=True, sanitizeFrags=False)
                 n = len(frags)
             if is_rw:
                 return Chem.RWMol(mol)
             else:
                 return mol
```

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_combine.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_communal.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_communal.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_ff.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_ff.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_join_neighboring.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_join_neighboring.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_merge.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                     if self.throw_on_discard:
                         raise error
                     else:
                         warn(msg)
             else:
                 new_name = self._get_combined_name(scaffold, fragmentanda)
                 scaffold = rdmolops.CombineMols(scaffold, fragmentanda)
-                scaffold.SetProp('_Name', new_name)
+                scaffold.SetProp('_Name', str(new_name))
         return scaffold
 
 
     def merge_pair(self, scaffold: Chem.Mol, fragmentanda: Chem.Mol, mapping: Optional = None) -> Chem.Mol:
         """
         To specify attachments use ``.merge``.
         To understand what is going on see ``.categorize``
@@ -107,15 +107,15 @@
                 done_already.append(other)
             scaffold = self._merge_part(scaffold, fragmentanda,
                                         anchor_index=anchor_index,
                                         attachment_details=attachment_details,
                                         other_attachments=other_attachments,
                                         other_attachment_details=other_attachment_details)
         new_name = self._get_combined_name(scaffold, fragmentanda)
-        scaffold.SetProp('_Name', new_name)
+        scaffold.SetProp('_Name', str(new_name))
         self.keep_copy(scaffold, 'pair_merged')
         return scaffold
 
     def _get_combined_name(self, first_mol: Chem.Mol, second_mol: Chem.Mol):
         get_name = lambda mol: mol.GetProp('_Name') if mol.HasProp('_Name') else 'molecule'
         name_1 = get_name(first_mol)
         name_2 = get_name(second_mol)
@@ -155,15 +155,15 @@
             raise DistanceError(hits=[scaffold, fragmentanda])
         # store alternative atom symbols.
         for si, fi in A2B_mapping.items():
             sa = scaffold.GetAtomWithIdx(si)
             sn = sa.GetSymbol()
             fn = fragmentanda.GetAtomWithIdx(fi).GetSymbol()
             if sn != fn:
-                sa.SetProp('_AltSymbol', fn)
+                sa.SetProp('_AltSymbol', str(fn))
         # prepare.
         uniques = set(range(fragmentanda.GetNumAtoms())) - set(A2B_mapping.values())
         categories = self._categorize(fragmentanda, uniques)
         pairs = categories['pairs']
         for p in pairs:  # pairs:Dict[List[Dict]]
             for pp in pairs[p]:
                 pp['idx_F'] = pp['idx']  # less ambiguous: fragmentanda index
```

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_modification_logging.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_modification_logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     _MonsterBase -> _MonsterTracker -> _MonsterCommunal
     """
 
     def keep_copy(self, mol: Chem.Mol, label=None):
         copy = Chem.Mol(mol)
         if label is None:
             label = f'Mol#{len(self.modifications)}'
-        copy.SetProp('_Name', label)
+        copy.SetProp('_Name', str(label))
         if label not in self.modifications:
             self.modifications[label] = copy
         else:
             label += '_'
             self.keep_copy(mol, label)
```

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_place.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/__init__.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_expand.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_expand.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_full.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_full.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_make_chimera.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_make_chimera.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 elif owned.GetExplicitValence() > 4 and wanted.GetSymbol() not in ('P',):
                     continue
                 else:
                     newatom = Chem.Atom(wanted)
                     stdev = chimera.GetAtomWithIdx(scaff_ai).GetDoubleProp('_Stdev')
                     newatom.SetDoubleProp('_Stdev', stdev)
                     origin = chimera.GetAtomWithIdx(scaff_ai).GetProp('_Origin')
-                    newatom.SetProp('_Origin', origin)
+                    newatom.SetProp('_Origin', str(origin))
                     chimera.ReplaceAtom(scaff_ai, newatom)
                     if diff_valance > 0:
                         chimera.GetAtomWithIdx(scaff_ai).SetFormalCharge(diff_valance)
         try:
             chimera.UpdatePropertyCache()  # noqa
         except Chem.AtomValenceException as err:
             warn('Valance issue' + str(err))
@@ -110,15 +110,15 @@
             if i in atom_map:
                 ci = atom_map[i]
                 c_atom = template_mol.GetAtomWithIdx(ci)
                 if c_atom.HasProp('_Stdev'):
                     stdev = c_atom.GetDoubleProp('_Stdev')
                     origin = c_atom.GetProp('_Origin')
                     p_atom.SetDoubleProp('_Stdev', stdev)
-                    p_atom.SetProp('_Origin', origin)
+                    p_atom.SetProp('_Origin', str(origin))
                 pconf.SetAtomPosition(i, chimera_conf.GetAtomPosition(ci))
             else:
                 uniques.add(i)
         ######################################################
         # I be using a sextant for dead reckoning!
         # variables: sextant unique team
         categories = self._categorize(sextant, uniques)
```

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_mappings.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_mappings.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_no_blending.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_no_blending.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_partial.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_partial.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_place_modes/_refine.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_place_modes/_refine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_util_compare.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_util_compare.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/_utility.py` & `Fragmenstein-1.0.4/fragmenstein/monster/_utility.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/bond_provenance.py` & `Fragmenstein-1.0.4/fragmenstein/monster/bond_provenance.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/mcs_mapping/compare_atom.py` & `Fragmenstein-1.0.4/fragmenstein/monster/mcs_mapping/compare_atom.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/mcs_mapping/types.py` & `Fragmenstein-1.0.4/fragmenstein/monster/mcs_mapping/types.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/mcs_mapping/utils.py` & `Fragmenstein-1.0.4/fragmenstein/monster/mcs_mapping/utils.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/positional_mapping.py` & `Fragmenstein-1.0.4/fragmenstein/monster/positional_mapping.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/monster/unmerge_mapper.py` & `Fragmenstein-1.0.4/fragmenstein/monster/unmerge_mapper.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/mpro/__init__.py` & `Fragmenstein-1.0.4/fragmenstein/mpro/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/mpro/dataframe.py` & `Fragmenstein-1.0.4/fragmenstein/mpro/dataframe.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/multivictor/multivictor.py` & `Fragmenstein-1.0.4/fragmenstein/multivictor/multivictor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/ngl_display.py` & `Fragmenstein-1.0.4/fragmenstein/ngl_display.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/openmm/fritz.py` & `Fragmenstein-1.0.4/fragmenstein/openmm/fritz.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/openmm/openvictor.py` & `Fragmenstein-1.0.4/fragmenstein/openmm/openvictor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/settings.py` & `Fragmenstein-1.0.4/fragmenstein/settings.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/version.py` & `Fragmenstein-1.0.4/fragmenstein/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 from typing import Dict
 def get_versions() -> Dict[str, str]:
     """
     Return a dict of versions of os, python, fragmenstein etc.
     """
     import pkg_resources, sys, platform
```

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/__init__.py` & `Fragmenstein-1.0.4/fragmenstein/victor/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_loggerwriter.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_loggerwriter.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_base.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_combine.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_common.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_common.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_igor.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_igor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_journal.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_journal.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_overridables.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_overridables.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_place.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_plonk.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_plonk.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_safety.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_safety.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_show.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_show.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_store.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_store.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_utils.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_utils.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/_victor_validate.py` & `Fragmenstein-1.0.4/fragmenstein/victor/_victor_validate.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/minimalPDB.py` & `Fragmenstein-1.0.4/fragmenstein/victor/minimalPDB.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/victor/plip.py` & `Fragmenstein-1.0.4/fragmenstein/victor/plip.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/walton/__init__.py` & `Fragmenstein-1.0.4/fragmenstein/walton/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/walton/_advmoves.py` & `Fragmenstein-1.0.4/fragmenstein/walton/_advmoves.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/walton/_art.py` & `Fragmenstein-1.0.4/fragmenstein/walton/_art.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/walton/_base.py` & `Fragmenstein-1.0.4/fragmenstein/walton/_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/walton/_movements.py` & `Fragmenstein-1.0.4/fragmenstein/walton/_movements.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/fragmenstein/walton/_polygon.py` & `Fragmenstein-1.0.4/fragmenstein/walton/_polygon.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/requirements.txt` & `Fragmenstein-1.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/setup.py` & `Fragmenstein-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version = '1.0.3'
+version = '1.0.4'
 
 
 from setuptools import setup, find_packages
 from warnings import warn
 from importlib import util
 import os
```

### Comparing `Fragmenstein-1.0.3/tests/MPro_combine.py` & `Fragmenstein-1.0.4/tests/MPro_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/MPro_place.py` & `Fragmenstein-1.0.4/tests/MPro_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/baffled.py` & `Fragmenstein-1.0.4/tests/baffled.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/cli.py` & `Fragmenstein-1.0.4/tests/cli.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/dummy_victor.py` & `Fragmenstein-1.0.4/tests/dummy_victor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/internals.py` & `Fragmenstein-1.0.4/tests/internals.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/lab.py` & `Fragmenstein-1.0.4/tests/lab.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/mapping.py` & `Fragmenstein-1.0.4/tests/mapping.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/monster_combine.py` & `Fragmenstein-1.0.4/tests/monster_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/monster_place.py` & `Fragmenstein-1.0.4/tests/monster_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/multivictor.py` & `Fragmenstein-1.0.4/tests/multivictor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/problems.py` & `Fragmenstein-1.0.4/tests/problems.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/victor_combine.py` & `Fragmenstein-1.0.4/tests/victor_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/victor_discard.py` & `Fragmenstein-1.0.4/tests/victor_discard.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.3/tests/walton.py` & `Fragmenstein-1.0.4/tests/walton.py`

 * *Files identical despite different names*

