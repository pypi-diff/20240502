# Comparing `tmp/heudiconv-1.1.0.tar.gz` & `tmp/heudiconv-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heudiconv-1.1.0.tar", last modified: Wed Feb 28 15:22:18 2024, max compression
+gzip compressed data, was "heudiconv-1.1.1.tar", last modified: Thu May  2 02:50:53 2024, max compression
```

## Comparing `heudiconv-1.1.0.tar` & `heudiconv-1.1.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.469485 heudiconv-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-28 15:21:45.000000 heudiconv-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-28 15:22:18.469485 heudiconv-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-02-28 15:21:45.000000 heudiconv-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.441485 heudiconv-1.1.0/heudiconv/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-28 15:22:18.000000 heudiconv-1.1.0/heudiconv/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    43889 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/bids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.445485 heudiconv-1.1.0/heudiconv/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/cli/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    37837 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    26666 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/dicoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/due.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.445485 heudiconv-1.1.0/heudiconv/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/external/dlad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.445485 heudiconv-1.1.0/heudiconv/external/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/external/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/external/tests/test_dlad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.445485 heudiconv-1.1.0/heudiconv/heuristics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/banda-bids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/bids_ME.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/bids_PhoenixReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/bids_with_ses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/cmrr_heuristic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/convertall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/convertall_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/multires_7Tbold.py
--rw-r--r--   0 runner    (1001) docker     (127)    39104 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/reproin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/studyforrest_phase2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/test_b0dwi_for_fmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/test_reproin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/heuristics/uc_bids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.449485 heudiconv-1.1.0/heudiconv/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      414 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/tests/anonymize_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.449485 heudiconv-1.1.0/heudiconv/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.449485 heudiconv-1.1.0/heudiconv/tests/data/01-anat-scout/
--rw-r--r--   0 runner    (1001) docker     (127)   174070 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/tests/data/01-anat-scout/0001.dcm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.453485 heudiconv-1.1.0/heudiconv/tests/data/01-fmap_acq-3mm/
--rw-r--r--   0 runner    (1001) docker     (127)   122162 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/tests/data/01-fmap_acq-3mm/1.3.12.2.1107.5.2.43.66112.2016101409263663466202201.dcm
--rw-r--r--   0 runner    (1001) docker     (127)   316172 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/tests/data/MRI_102TD_PHA_S.MR.Chen_Matthews_1.3.1.2022.11.16.15.50.20.357.31204541.dcm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.437485 heudiconv-1.1.0/heudiconv/tests/data/Phoenix/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.453485 heudiconv-1.1.0/heudiconv/tests/data/Phoenix/01+AA/
--rw-r--r--   0 runner    (1001) docker     (127)   207270 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/tests/data/Phoenix/01+AA/01+AA+00001.dcm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.453485 heudiconv-1.1.0/heudiconv/tests/data/Phoenix/99+PhoenixDocument/
--rw-r--r--   0 runner    (1001) docker     (127)   255416 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/tests/data/Phoenix/99+PhoenixDocument/99+PhoenixDocument+00001.dcm
--rw-r--r--   0 runner    (1001) docker     (127)   383456 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/tests/data/axasc35.dcm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.461485 heudiconv-1.1.0/heudiconv/tests/data/b0dwiForFmap/
--rw-r--r--   0 runner    (1001) docker     (127)  3933300 2024-02-28 15:21:45.000000 heudiconv-1.1.0/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00001.dcm
--rw-r--r--   0 runner    (1001) docker     (127)  3933296 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00002.dcm
--rw-r--r--   0 runner    (1001) docker     (127)  3933300 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00003.dcm
--rw-r--r--   0 runner    (1001) docker     (127)   162304 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/data/phantom.dcm
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/data/sample_nifti.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/data/sample_nifti_params.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/test_archives.py
--rw-r--r--   0 runner    (1001) docker     (127)    47839 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/test_bids.py
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/test_dicoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/test_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/test_tarballs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21515 2024-02-28 15:21:46.000000 heudiconv-1.1.0/heudiconv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:22:18.465485 heudiconv-1.1.0/heudiconv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-28 15:22:18.000000 heudiconv-1.1.0/heudiconv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-28 15:22:18.000000 heudiconv-1.1.0/heudiconv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 15:22:18.000000 heudiconv-1.1.0/heudiconv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-28 15:22:18.000000 heudiconv-1.1.0/heudiconv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-28 15:22:18.000000 heudiconv-1.1.0/heudiconv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-28 15:22:18.000000 heudiconv-1.1.0/heudiconv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-28 15:21:46.000000 heudiconv-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 15:22:18.469485 heudiconv-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2769 2024-02-28 15:21:46.000000 heudiconv-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.781750 heudiconv-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-02 02:50:23.000000 heudiconv-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-02 02:50:53.781750 heudiconv-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-02 02:50:23.000000 heudiconv-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.753750 heudiconv-1.1.1/heudiconv/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 02:50:53.000000 heudiconv-1.1.1/heudiconv/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43889 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/bids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.753750 heudiconv-1.1.1/heudiconv/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/cli/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37837 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26672 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/dicoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/due.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.753750 heudiconv-1.1.1/heudiconv/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/external/dlad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.753750 heudiconv-1.1.1/heudiconv/external/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/external/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/external/tests/test_dlad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.757750 heudiconv-1.1.1/heudiconv/heuristics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/banda-bids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/bids_ME.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/bids_PhoenixReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/bids_with_ses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/cmrr_heuristic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/convertall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/convertall_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/multires_7Tbold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39104 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/reproin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/studyforrest_phase2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/test_b0dwi_for_fmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/test_reproin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/heuristics/uc_bids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.761750 heudiconv-1.1.1/heudiconv/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      414 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/anonymize_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.761750 heudiconv-1.1.1/heudiconv/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.761750 heudiconv-1.1.1/heudiconv/tests/data/01-anat-scout/
+-rw-r--r--   0 runner    (1001) docker     (127)   174070 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/01-anat-scout/0001.dcm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.765750 heudiconv-1.1.1/heudiconv/tests/data/01-fmap_acq-3mm/
+-rw-r--r--   0 runner    (1001) docker     (127)   122162 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/01-fmap_acq-3mm/1.3.12.2.1107.5.2.43.66112.2016101409263663466202201.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)   316172 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/MRI_102TD_PHA_S.MR.Chen_Matthews_1.3.1.2022.11.16.15.50.20.357.31204541.dcm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.749750 heudiconv-1.1.1/heudiconv/tests/data/Phoenix/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.765750 heudiconv-1.1.1/heudiconv/tests/data/Phoenix/01+AA/
+-rw-r--r--   0 runner    (1001) docker     (127)   207270 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/Phoenix/01+AA/01+AA+00001.dcm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.765750 heudiconv-1.1.1/heudiconv/tests/data/Phoenix/99+PhoenixDocument/
+-rw-r--r--   0 runner    (1001) docker     (127)   255416 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/Phoenix/99+PhoenixDocument/99+PhoenixDocument+00001.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)   383456 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/axasc35.dcm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.773750 heudiconv-1.1.1/heudiconv/tests/data/b0dwiForFmap/
+-rw-r--r--   0 runner    (1001) docker     (127)  3933300 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00001.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)  3933296 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00002.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)  3933300 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00003.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)   162304 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/phantom.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/sample_nifti.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/data/sample_nifti_params.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/test_archives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47839 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/test_bids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/test_dicoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/test_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/test_tarballs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21515 2024-05-02 02:50:23.000000 heudiconv-1.1.1/heudiconv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 02:50:53.781750 heudiconv-1.1.1/heudiconv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-02 02:50:53.000000 heudiconv-1.1.1/heudiconv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-02 02:50:53.000000 heudiconv-1.1.1/heudiconv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 02:50:53.000000 heudiconv-1.1.1/heudiconv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-02 02:50:53.000000 heudiconv-1.1.1/heudiconv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 02:50:53.000000 heudiconv-1.1.1/heudiconv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 02:50:53.000000 heudiconv-1.1.1/heudiconv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 02:50:23.000000 heudiconv-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 02:50:53.781750 heudiconv-1.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2769 2024-05-02 02:50:23.000000 heudiconv-1.1.1/setup.py
```

### Comparing `heudiconv-1.1.0/LICENSE` & `heudiconv-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/PKG-INFO` & `heudiconv-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heudiconv
-Version: 1.1.0
+Version: 1.1.1
 Summary: Heuristic DICOM Converter
 Author: HeuDiConv team and contributors
 License: Apache 2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `heudiconv-1.1.0/README.rst` & `heudiconv-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/bids.py` & `heudiconv-1.1.1/heudiconv/bids.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/cli/monitor.py` & `heudiconv-1.1.1/heudiconv/cli/monitor.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/cli/run.py` & `heudiconv-1.1.1/heudiconv/cli/run.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/convert.py` & `heudiconv-1.1.1/heudiconv/convert.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/dicoms.py` & `heudiconv-1.1.1/heudiconv/dicoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -522,26 +522,26 @@
     The following fields are checked in order
 
     1. AcquisitionDate & AcquisitionTime  (0008,0022); (0008,0032)
     2. AcquisitionDateTime (0008,002A);
     3. SeriesDate & SeriesTime  (0008,0021); (0008,0031)
 
     """
-    acq_date = dcm_data.get("AcquisitionDate")
-    acq_time = dcm_data.get("AcquisitionTime")
-    if not (acq_date is None or acq_time is None):
+    acq_date = dcm_data.get("AcquisitionDate", "").strip()
+    acq_time = dcm_data.get("AcquisitionTime", "").strip()
+    if acq_date and acq_time:
         return strptime_micr(acq_date + acq_time, "%Y%m%d%H%M%S[.%f]")
 
-    acq_dt = dcm_data.get("AcquisitionDateTime")
-    if acq_dt is not None:
+    acq_dt = dcm_data.get("AcquisitionDateTime", "").strip()
+    if acq_dt:
         return strptime_micr(acq_dt, "%Y%m%d%H%M%S[.%f]")
 
-    series_date = dcm_data.get("SeriesDate")
-    series_time = dcm_data.get("SeriesTime")
-    if not (series_date is None or series_time is None):
+    series_date = dcm_data.get("SeriesDate", "").strip()
+    series_time = dcm_data.get("SeriesTime", "").strip()
+    if series_date and series_time:
         return strptime_micr(series_date + series_time, "%Y%m%d%H%M%S[.%f]")
     return None
 
 
 def compress_dicoms(
     dicom_list: list[str], out_prefix: str, tempdirs: TempDirs, overwrite: bool
 ) -> Optional[str]:
```

### Comparing `heudiconv-1.1.0/heudiconv/due.py` & `heudiconv-1.1.1/heudiconv/due.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/external/dlad.py` & `heudiconv-1.1.1/heudiconv/external/dlad.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/external/tests/test_dlad.py` & `heudiconv-1.1.1/heudiconv/external/tests/test_dlad.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/banda-bids.py` & `heudiconv-1.1.1/heudiconv/heuristics/banda-bids.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/bids_ME.py` & `heudiconv-1.1.1/heudiconv/heuristics/bids_ME.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/bids_PhoenixReport.py` & `heudiconv-1.1.1/heudiconv/heuristics/bids_PhoenixReport.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/bids_with_ses.py` & `heudiconv-1.1.1/heudiconv/heuristics/bids_with_ses.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/cmrr_heuristic.py` & `heudiconv-1.1.1/heudiconv/heuristics/cmrr_heuristic.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/convertall.py` & `heudiconv-1.1.1/heudiconv/heuristics/convertall.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/convertall_custom.py` & `heudiconv-1.1.1/heudiconv/heuristics/convertall_custom.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/example.py` & `heudiconv-1.1.1/heudiconv/heuristics/example.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/multires_7Tbold.py` & `heudiconv-1.1.1/heudiconv/heuristics/multires_7Tbold.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/reproin.py` & `heudiconv-1.1.1/heudiconv/heuristics/reproin.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/studyforrest_phase2.py` & `heudiconv-1.1.1/heudiconv/heuristics/studyforrest_phase2.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/test_b0dwi_for_fmap.py` & `heudiconv-1.1.1/heudiconv/heuristics/test_b0dwi_for_fmap.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/test_reproin.py` & `heudiconv-1.1.1/heudiconv/heuristics/test_reproin.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/heuristics/uc_bids.py` & `heudiconv-1.1.1/heudiconv/heuristics/uc_bids.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/info.py` & `heudiconv-1.1.1/heudiconv/info.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/main.py` & `heudiconv-1.1.1/heudiconv/main.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/parser.py` & `heudiconv-1.1.1/heudiconv/parser.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/queue.py` & `heudiconv-1.1.1/heudiconv/queue.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/data/01-anat-scout/0001.dcm` & `heudiconv-1.1.1/heudiconv/tests/data/01-anat-scout/0001.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/data/01-fmap_acq-3mm/1.3.12.2.1107.5.2.43.66112.2016101409263663466202201.dcm` & `heudiconv-1.1.1/heudiconv/tests/data/01-fmap_acq-3mm/1.3.12.2.1107.5.2.43.66112.2016101409263663466202201.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/data/MRI_102TD_PHA_S.MR.Chen_Matthews_1.3.1.2022.11.16.15.50.20.357.31204541.dcm` & `heudiconv-1.1.1/heudiconv/tests/data/MRI_102TD_PHA_S.MR.Chen_Matthews_1.3.1.2022.11.16.15.50.20.357.31204541.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/data/Phoenix/01+AA/01+AA+00001.dcm` & `heudiconv-1.1.1/heudiconv/tests/data/Phoenix/01+AA/01+AA+00001.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/data/Phoenix/99+PhoenixDocument/99+PhoenixDocument+00001.dcm` & `heudiconv-1.1.1/heudiconv/tests/data/Phoenix/99+PhoenixDocument/99+PhoenixDocument+00001.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/data/axasc35.dcm` & `heudiconv-1.1.1/heudiconv/tests/data/axasc35.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00001.dcm` & `heudiconv-1.1.1/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00001.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00002.dcm` & `heudiconv-1.1.1/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00002.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00003.dcm` & `heudiconv-1.1.1/heudiconv/tests/data/b0dwiForFmap/b0dwi_for_fmap+00003.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/data/phantom.dcm` & `heudiconv-1.1.1/heudiconv/tests/data/phantom.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/test_archives.py` & `heudiconv-1.1.1/heudiconv/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/test_bids.py` & `heudiconv-1.1.1/heudiconv/tests/test_bids.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/test_convert.py` & `heudiconv-1.1.1/heudiconv/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/test_dicoms.py` & `heudiconv-1.1.1/heudiconv/tests/test_dicoms.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/test_heuristics.py` & `heudiconv-1.1.1/heudiconv/tests/test_heuristics.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/test_main.py` & `heudiconv-1.1.1/heudiconv/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/test_monitor.py` & `heudiconv-1.1.1/heudiconv/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/test_queue.py` & `heudiconv-1.1.1/heudiconv/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/test_regression.py` & `heudiconv-1.1.1/heudiconv/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/test_tarballs.py` & `heudiconv-1.1.1/heudiconv/tests/test_tarballs.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/test_utils.py` & `heudiconv-1.1.1/heudiconv/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/tests/utils.py` & `heudiconv-1.1.1/heudiconv/tests/utils.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv/utils.py` & `heudiconv-1.1.1/heudiconv/utils.py`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/heudiconv.egg-info/PKG-INFO` & `heudiconv-1.1.1/heudiconv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heudiconv
-Version: 1.1.0
+Version: 1.1.1
 Summary: Heuristic DICOM Converter
 Author: HeuDiConv team and contributors
 License: Apache 2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `heudiconv-1.1.0/heudiconv.egg-info/SOURCES.txt` & `heudiconv-1.1.1/heudiconv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heudiconv-1.1.0/setup.py` & `heudiconv-1.1.1/setup.py`

 * *Files identical despite different names*

