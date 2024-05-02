# Comparing `tmp/dascore-0.1.0.tar.gz` & `tmp/dascore-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dascore-0.1.0.tar", last modified: Thu Jan 11 22:46:27 2024, max compression
+gzip compressed data, was "dascore-0.1.1.tar", last modified: Thu May  2 15:56:51 2024, max compression
```

## Comparing `dascore-0.1.0.tar` & `dascore-0.1.1.tar`

### file list

```diff
@@ -1,201 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.214711 dascore-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-01-11 22:46:27.214711 dascore-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.186711 dascore-0.1.0/dascore/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.186711 dascore-0.1.0/dascore/clients/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/clients/dirspool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/clients/filespool.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.190711 dascore-0.1.0/dascore/core/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23464 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/core/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44729 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/core/coordmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    43366 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/core/coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/core/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/core/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    25549 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/core/spool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/data_registry.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.190711 dascore-0.1.0/dascore/io/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.190711 dascore-0.1.0/dascore/io/dasdae/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/dasdae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/dasdae/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/dasdae/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.190711 dascore-0.1.0/dascore/io/dashdf5/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/dashdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/dashdf5/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/dashdf5/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.190711 dascore-0.1.0/dascore/io/h5simple/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/h5simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/h5simple/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/h5simple/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.190711 dascore-0.1.0/dascore/io/pickle/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/pickle/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.190711 dascore-0.1.0/dascore/io/prodml/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/prodml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/prodml/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/prodml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.190711 dascore-0.1.0/dascore/io/rsf/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/rsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/rsf/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.194711 dascore-0.1.0/dascore/io/segy/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/segy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/segy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/segy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.194711 dascore-0.1.0/dascore/io/sentek/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/sentek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/sentek/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/sentek/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.194711 dascore-0.1.0/dascore/io/tdms/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/tdms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/tdms/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12673 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/tdms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.194711 dascore-0.1.0/dascore/io/terra15/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/terra15/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/terra15/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/terra15/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.194711 dascore-0.1.0/dascore/io/wav/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/wav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/io/wav/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.198711 dascore-0.1.0/dascore/proc/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15658 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/correlate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/detrend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/resample.py
--rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/rolling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/taper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/proc/whiten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.198711 dascore-0.1.0/dascore/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/transform/differentiate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/transform/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/transform/fft.py
--rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/transform/fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/transform/integrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/transform/spectro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/transform/strain.py
--rw-r--r--   0 runner    (1001) docker     (127)     9642 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.198711 dascore-0.1.0/dascore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15594 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    21607 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    17383 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    17215 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/pd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/utils/transformatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.202711 dascore-0.1.0/dascore/viz/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/viz/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/viz/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-01-11 22:45:34.000000 dascore-0.1.0/dascore/viz/wiggle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.210711 dascore-0.1.0/dascore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-01-11 22:46:27.000000 dascore-0.1.0/dascore.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.202711 dascore-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-01-11 22:45:34.000000 dascore-0.1.0/docs/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-01-11 22:45:34.000000 dascore-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-01-11 22:45:34.000000 dascore-0.1.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 22:46:27.214711 dascore-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.202711 dascore-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.202711 dascore-0.1.0/tests/test_clients/
--rw-r--r--   0 runner    (1001) docker     (127)    18958 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_clients/test_dirspool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_clients/test_filespool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.202711 dascore-0.1.0/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (127)    17117 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_core/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    50837 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_core/test_coordmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    52080 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_core/test_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)    25864 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_core/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18995 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_core/test_patch_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)    22212 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_core/test_spool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.202711 dascore-0.1.0/tests/test_integrations/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_integrations/test_doc_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.202711 dascore-0.1.0/tests/test_io/
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_common_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.202711 dascore-0.1.0/tests/test_io/test_dasdae/
--rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_dasdae/test_dasdae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.202711 dascore-0.1.0/tests/test_io/test_h5simple/
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_h5simple/test_h5simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_io_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.202711 dascore-0.1.0/tests/test_io/test_pickle/
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_pickle/test_pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.206711 dascore-0.1.0/tests/test_io/test_prodml/
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_prodml/test_prod_ml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.206711 dascore-0.1.0/tests/test_io/test_rsf/
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_rsf/test_rsf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.206711 dascore-0.1.0/tests/test_io/test_segy/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_segy/test_segy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.206711 dascore-0.1.0/tests/test_io/test_sentek/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_sentek/test_sentek.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.206711 dascore-0.1.0/tests/test_io/test_terra15/
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_terra15/test_terra15.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.206711 dascore-0.1.0/tests/test_io/test_wav/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_io/test_wav/test_wav.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.206711 dascore-0.1.0/tests/test_proc/
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_correlate.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_detrend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11589 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_proc_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_proc_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_rolling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_taper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_proc/test_whiten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.210711 dascore-0.1.0/tests/test_transform/
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_transform/test_differentiate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_transform/test_dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_transform/test_fft.py
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_transform/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_transform/test_integrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_transform/test_spectro_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_transform/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_transform/test_velocity_to_strainrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.210711 dascore-0.1.0/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_hdf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_mapping_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_patch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_pd.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    15698 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_utils/test_transformatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 22:46:27.210711 dascore-0.1.0/tests/test_viz/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_viz/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_viz/test_spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_viz/test_waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-01-11 22:45:34.000000 dascore-0.1.0/tests/test_viz/test_wiggle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.226145 dascore-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    12148 2024-05-02 15:56:51.226145 dascore-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.202145 dascore-0.1.1/dascore/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.202145 dascore-0.1.1/dascore/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/clients/dirspool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/clients/filespool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.202145 dascore-0.1.1/dascore/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23543 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/core/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46641 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/core/coordmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44740 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/core/coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/core/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25549 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/core/spool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/data_registry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15239 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.206145 dascore-0.1.1/dascore/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.206145 dascore-0.1.1/dascore/io/dasdae/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/dasdae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/dasdae/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/dasdae/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.206145 dascore-0.1.1/dascore/io/dashdf5/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/dashdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/dashdf5/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/dashdf5/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.206145 dascore-0.1.1/dascore/io/febus/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/febus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/febus/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/febus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.206145 dascore-0.1.1/dascore/io/h5simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/h5simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/h5simple/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/h5simple/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.206145 dascore-0.1.1/dascore/io/optodas/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/optodas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/optodas/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/optodas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.206145 dascore-0.1.1/dascore/io/pickle/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/pickle/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.206145 dascore-0.1.1/dascore/io/prodml/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/prodml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/prodml/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/prodml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.206145 dascore-0.1.1/dascore/io/rsf/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/rsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/rsf/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.206145 dascore-0.1.1/dascore/io/segy/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/segy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/segy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/segy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.210145 dascore-0.1.1/dascore/io/sentek/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/sentek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/sentek/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/sentek/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.210145 dascore-0.1.1/dascore/io/tdms/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/tdms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/tdms/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12673 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/tdms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.210145 dascore-0.1.1/dascore/io/terra15/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/terra15/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/terra15/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/terra15/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.210145 dascore-0.1.1/dascore/io/wav/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/wav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/io/wav/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.210145 dascore-0.1.1/dascore/proc/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15658 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/correlate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/detrend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/rolling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/taper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/proc/whiten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.214145 dascore-0.1.1/dascore/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/transform/differentiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/transform/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/transform/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/transform/fourier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/transform/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/transform/spectro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/transform/strain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9642 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.214145 dascore-0.1.1/dascore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15885 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17383 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17215 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/pd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/utils/transformatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.214145 dascore-0.1.1/dascore/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/viz/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/viz/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-02 15:54:59.000000 dascore-0.1.1/dascore/viz/wiggle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.226145 dascore-0.1.1/dascore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-02 15:56:51.000000 dascore-0.1.1/dascore.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.214145 dascore-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-05-02 15:54:59.000000 dascore-0.1.1/docs/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-02 15:54:59.000000 dascore-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-02 15:54:59.000000 dascore-0.1.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:56:51.226145 dascore-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.214145 dascore-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.214145 dascore-0.1.1/tests/test_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)    18958 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_clients/test_dirspool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_clients/test_filespool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_core/
+-rw-r--r--   0 runner    (1001) docker     (127)    17659 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_core/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52331 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_core/test_coordmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53264 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_core/test_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_core/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18995 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_core/test_patch_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22212 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_core/test_spool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_integrations/test_doc_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_io/
+-rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_common_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_io/test_dasdae/
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_dasdae/test_dasdae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_io/test_h5simple/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_h5simple/test_h5simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_io_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_io/test_pickle/
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_pickle/test_pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_io/test_prodml/
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_prodml/test_prod_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_io/test_rsf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_rsf/test_rsf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_io/test_segy/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_segy/test_segy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_io/test_sentek/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_sentek/test_sentek.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_io/test_terra15/
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_terra15/test_terra15.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.218145 dascore-0.1.1/tests/test_io/test_wav/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_io/test_wav/test_wav.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.222145 dascore-0.1.1/tests/test_proc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_correlate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_detrend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11589 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_proc_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_proc_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_rolling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_taper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_proc/test_whiten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.222145 dascore-0.1.1/tests/test_transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_transform/test_differentiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_transform/test_dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_transform/test_fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_transform/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_transform/test_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_transform/test_spectro_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_transform/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_transform/test_velocity_to_strainrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.222145 dascore-0.1.1/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_hdf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_mapping_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_patch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_pd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15698 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_utils/test_transformatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:56:51.226145 dascore-0.1.1/tests/test_viz/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_viz/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_viz/test_spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_viz/test_waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-02 15:54:59.000000 dascore-0.1.1/tests/test_viz/test_wiggle.py
```

### Comparing `dascore-0.1.0/PKG-INFO` & `dascore-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dascore
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python library distributed fiber optic sensing
 Author-email: Derrick Chambers <chambers.ja.derrick@gmail.com>
 License: dascore is licenced under LGPL version 3 licence:
         
                            GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `dascore-0.1.0/dascore/__init__.py` & `dascore-0.1.1/dascore/__init__.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/clients/dirspool.py` & `dascore-0.1.1/dascore/clients/dirspool.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/clients/filespool.py` & `dascore-0.1.1/dascore/clients/filespool.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/compat.py` & `dascore-0.1.1/dascore/compat.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/constants.py` & `dascore-0.1.1/dascore/constants.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/core/attrs.py` & `dascore-0.1.1/dascore/core/attrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,17 @@
             return attr_map
         out = {} if attr_map is None else attr_map
         return cls(**out)
 
     @property
     def dim_tuple(self):
         """Return a tuple of dimensions. The dims attr is a string."""
+        dim_str = self.dims
+        if not dim_str:
+            return tuple()
         return tuple(self.dims.split(","))
 
     def rename_dimension(self, **kwargs):
         """Rename one or more dimensions if in kwargs. Return new PatchAttrs."""
         if not (dims := set(kwargs) & set(self.dim_tuple)):
             return self
         new = self.model_dump(exclude_defaults=True)
```

### Comparing `dascore-0.1.0/dascore/core/coordmanager.py` & `dascore-0.1.1/dascore/core/coordmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 """
 from __future__ import annotations
 
 import warnings
 from collections import defaultdict
 from collections.abc import Mapping, Sequence, Sized
 from functools import reduce
+from itertools import zip_longest
 from operator import and_, or_
 from typing import Annotated, Any, TypeVar
 
 import numpy as np
 from pydantic import field_validator, model_validator
 from rich.text import Text
 from typing_extensions import Self
@@ -77,25 +78,25 @@
     frozen_dict_serializer,
     frozen_dict_validator,
 )
 
 MaybeArray = TypeVar("MaybeArray", ArrayLike, np.ndarray, None)
 
 
-def _validate_select_coords(coord, coord_name):
+def _validate_select_coords(coord, coord_name: str):
     """Ensure multi-dims are not used."""
     if not len(coord.shape) == 1:
         msg = (
             "Only 1 dimensional coordinates can be used for selection "
             f"{coord_name} has {len(coord.shape)} dimensions."
         )
         raise CoordError(msg)
 
 
-def _indirect_coord_updates(cm, dim_name, coord_name, reduction, new_coords):
+def _indirect_coord_updates(cm, dim_name, coord_name: str, reduction, new_coords):
     """
     Applies trim to coordinates.
 
     Assumes other associated coordinates are trimmed.
     """
     other_coords = set(cm.dim_to_coord_map[dim_name]) - {coord_name}
     # perform indirect updates.
@@ -556,14 +557,31 @@
             dims[dims.index(old_dim)] = new_dim
         # now loop over dim_maps and swap out old dims with new
         old_to_new = {i: v for i, v in zip(self.dims, dims, strict=True)}
         for coord_name, coord_dims in dim_map.items():
             dim_map[coord_name] = tuple(old_to_new[x] for x in coord_dims)
         return self.__class__(dims=dims, coord_map=coord_map, dim_map=dim_map)
 
+    def _get_single_dim_kwarg_list(self, kwargs):
+        """Get a list of dicts where each dict uses a dimension at most once."""
+        used_coords = sorted(set(self.coord_map) & set(kwargs))
+        dims = [self.dim_map[x] for x in used_coords]
+        # No duplicate usage, just return.
+        if len(set(dims)) == len(dims):
+            return [{i: kwargs[i] for i in used_coords}]
+        # We need to split kwargs up so each dimension is used no more
+        # than once in each dict (element of the list).
+        dim_dicts = defaultdict(list)
+        for coord, dim in zip(used_coords, dims):
+            dim_dicts[dim].append(coord)
+        out = []
+        for args in zip_longest(*dim_dicts.values()):
+            out.append({x: kwargs[x] for x in args if x is not None})
+        return out
+
     def select(
         self, array: MaybeArray = None, relative=False, samples=False, **kwargs
     ) -> tuple[Self, MaybeArray]:
         """
         Perform value-based selection on coordinates.
 
         Parameters
@@ -574,19 +592,32 @@
             If True, coordinate updates are relative.
         samples
             If True, the query meaning is in samples.
         **kwargs
             Used to specify select arguments. Can be of the form
             {coord_name: (lower_limit, upper_limit)}.
         """
-        new_coords, indexers = _get_indexers_and_new_coords_dict(
-            self, kwargs, samples=samples, relative=relative
-        )
-        new_cm = self.update(**new_coords)
-        return new_cm, self._get_new_data(indexers, array)
+        # Relative or sample queries cannot be performed multiple times on
+        # the same dimension (since multiple coords can reference the same dim)
+        if relative or samples:
+            used_dims = [self.dim_map[x] for x in kwargs if x in self.coord_map]
+            if len(set(used_dims)) < len(used_dims):
+                msg = (
+                    f"Cannot use {kwargs} for query; some coords " f"share a dimension."
+                )
+                raise CoordError(msg)
+        # Otherwise, we need to sort through kwargs and call in a loop.
+        kwarg_list = self._get_single_dim_kwarg_list(kwargs)
+        for kwargs in kwarg_list:
+            new_coords, indexers = _get_indexers_and_new_coords_dict(
+                self, kwargs, samples=samples, relative=relative
+            )
+            self = self.update(**new_coords)
+            array = self._get_new_data(indexers, array)
+        return self, array
 
     def _get_new_data(self, indexer, array: MaybeArray) -> MaybeArray:
         """Get new data array after applying some trimming."""
         if array is None:  # no array passed, just return.
             return array
         return array[indexer]
 
@@ -642,15 +673,15 @@
         # empty arrays return (0,) as their shape, so we must do the same.
         if not out:
             return (0,)
         return out
 
     @property
     def size(self):
-        """Return the shape of the dimensions."""
+        """Return the size of the patch data matrix."""
         return np.prod(self.shape)
 
     def validate_data(self, data):
         """Ensure data conforms to coordinates."""
         data = np.array([]) if data is None else data
         if self.shape != data.shape:
             msg = (
@@ -865,15 +896,15 @@
         out[ind] = value
         return tuple(out)
 
     def keys(self):
         """Return the keys (coordinates) in the coord manager."""
         return self.coord_map.keys()
 
-    def to_summary_dict(self) -> dict[str, CoordSummary]:
+    def to_summary_dict(self) -> dict[str, CoordSummary | tuple[str, ...]]:
         """Convert the contents of the coordinate manager to a summary dict."""
         dim_map = self.dim_map
         out = {}
         for name, coord in self.coord_map.items():
             out[name] = coord.to_summary(dims=dim_map[name])
         return out
 
@@ -894,30 +925,38 @@
             msg = (
                 f"No coordinate named {coord_name} in coord manager. "
                 f"Valid coordinates are {list(self.coord_map)}."
             )
             raise CoordError(msg)
         return self.coord_map[coord_name]
 
-    def min(self, coord_name):
+    def min(self, coord_name: str):
         """Return the minimum value of a coordinate."""
         return self.get_coord(coord_name).min()
 
-    def max(self, coord_name):
+    def max(self, coord_name: str):
         """Return the maximum value of a coordinate."""
         return self.get_coord(coord_name).max()
 
-    def step(self, coord_name):
+    def step(self, coord_name: str):
         """Return the coordinate step."""
         return self.get_coord(coord_name).step
 
-    def get_array(self, coord_name) -> np.ndarray:
+    def get_array(self, coord_name: str) -> np.ndarray:
         """Return the coordinate values as a numpy array."""
         return np.array(self.get_coord(coord_name))
 
+    def coord_size(self, coord_name: str) -> int:
+        """Return the coordinate size."""
+        return self.get_coord(coord_name).size
+
+    def coord_range(self, coord_name: str):
+        """Return a scaler value for the coordinate (e.g., number of seconds)."""
+        return self.get_coord(coord_name).coord_range()
+
 
 def get_coord_manager(
     coords: Mapping[str, BaseCoord | np.ndarray] | CoordManager | None = None,
     dims: tuple[str, ...] | None = None,
     attrs: dc.PatchAttrs | dict[str, Any] | None = None,
 ) -> CoordManager:
     """
```

### Comparing `dascore-0.1.0/dascore/core/coords.py` & `dascore-0.1.1/dascore/core/coords.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,14 +320,19 @@
 
     @property
     def shape(self) -> tuple[int, ...]:
         """Return the shape of the coordinate data."""
         return self.data.shape
 
     @property
+    def size(self) -> int:
+        """Return the size of the coordinate data."""
+        return np.prod(self.shape)
+
+    @property
     def evenly_sampled(self) -> tuple[int, ...]:
         """Returns True if the coord is evenly sampled."""
         return self._evenly_sampled
 
     @property
     def sorted(self) -> tuple[int, ...]:
         """Returns True if the coord in sorted."""
@@ -345,14 +350,20 @@
         return self.__class__(**new)
 
     def simplify_units(self) -> Self:
         """Simplify the coordinate units."""
         _, unit = get_factor_and_unit(self.units, simplify=True)
         return self.convert_units(unit)
 
+    def coord_range(self):
+        """Return a scaler value for the coordinate (e.g., number of seconds)."""
+        if not self.evenly_sampled:
+            raise CoordError("coord_range has to be called on an evenly sampled data.")
+        return self.max() - self.min() + self.step
+
     @abc.abstractmethod
     def sort(self, reverse=False) -> tuple[BaseCoord, slice | ArrayLike]:
         """Sort the contents of the coord. Return new coord and slice for sorting."""
 
     def snap(self) -> CoordRange:
         """
         Snap the coordinates to evenly sampled grid points.
@@ -829,14 +840,34 @@
 
     def _max(self):
         """Return max value in range."""
         # like range, coord range is exclusive of final value.
         # the min/max are needed for reverse sorted coord.
         return np.max([self.stop - self.step, self.start])
 
+    def change_length(self, length: int) -> Self:
+        """
+        Adjust the length of the coordinate by changing the end value.
+
+        This is useful for floating point coordinates who frequently suffer
+        from off by one errors.
+
+        Parameters
+        ----------
+        length
+            The output length.
+        """
+        if (current := len(self)) == length:
+            return self
+        diff = length - current
+        stop, step = self.stop, self.step
+        out = self.update(stop=stop + step * diff)
+        assert len(out) == length
+        return out
+
     @property
     def sorted(self) -> bool:
         """Returns true if sorted in ascending order."""
         return self.step >= 0
 
     @property
     def reverse_sorted(self) -> bool:
@@ -881,14 +912,20 @@
         val2 = self._get_compatible_value(args[1])
         if val1 is not None:
             out = out & (values >= val1)
         if val2 is not None:
             out = out & (values <= val2)
         if not np.any(out):
             return self.empty(), out
+        if np.all(out):
+            return self, slice(None, None)
+        # Convert boolean to int indexes because these are supported for
+        # indexing pytables arrays but booleans are not.
+        if len(self.shape) == 1:
+            out = np.arange(len(out))[out]
         return self.new(values=values[out]), out
 
     def sort(self, reverse=False) -> tuple[BaseCoord, slice | ArrayLike]:
         """Sort the coord to be monotonic (maybe range)."""
         argsort: ArrayLike = np.argsort(self.values)[:: -1 if reverse else 1]
         arg_dict = self.model_dump()
         arg_dict["values"] = self.values[argsort]
@@ -1216,13 +1253,14 @@
             if not pd.isnull(step):
                 val = data[0]
                 return CoordRange(start=val, stop=val + step, step=step, units=units)
             return CoordMonotonicArray(values=data, units=units)
         start, stop, step, monotonic = _maybe_get_start_stop_step(data)
         if start is not None:
             out = CoordRange(start=start, stop=stop, step=step, units=units)
-            return out
+            # The change_length call helps with float off by one issues.
+            return out.change_length(len(data))
         elif monotonic:
             return CoordMonotonicArray(values=data, units=units)
         return CoordArray(values=data, units=units)
     else:
         return CoordRange(start=start, stop=stop, step=step, units=units)
```

### Comparing `dascore-0.1.0/dascore/core/patch.py` & `dascore-0.1.1/dascore/core/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from dascore import transform
 from dascore.compat import DataArray, array
 from dascore.core.attrs import PatchAttrs
 from dascore.core.coordmanager import CoordManager, get_coord_manager
 from dascore.core.coords import BaseCoord
 from dascore.utils.display import array_to_text, attrs_to_text, get_dascore_text
 from dascore.utils.models import ArrayLike
+from dascore.utils.time import to_float
 from dascore.viz import VizPatchNameSpace
 
 
 class Patch:
     """
     A Class for managing data and metadata.
 
@@ -88,14 +89,15 @@
         # the only case we allow attrs to include coords is if they are both
         # dicts, in which case attrs might have unit info for coords.
         if isinstance(attrs, Mapping) and attrs:
             coords, attrs = coords.update_from_attrs(attrs)
         else:
             # ensure attrs conforms to coords
             attrs = dc.PatchAttrs.from_dict(attrs).update(coords=coords)
+        assert coords.dims == attrs.dim_tuple, "dim mismatch on coords and attrs"
         self._coords = coords
         self._attrs = attrs
         self._data = array(self.coords.validate_data(data))
 
     def __eq__(self, other):
         """Compare one Patch."""
         return dascore.proc.equals(self, other)
@@ -156,27 +158,37 @@
     @property
     def coords(self) -> CoordManager:
         """Return the dimensions contained in patch."""
         return self._coords
 
     @property
     def data(self) -> ArrayLike:
-        """Return the dimensions contained in patch."""
+        """Return the data contained in patch."""
         return self._data
 
     @property
     def shape(self) -> tuple[int, ...]:
         """Return the shape of the data array."""
         return self.coords.shape
 
     @property
     def size(self) -> tuple[int, ...]:
-        """Return the shape of the data array."""
+        """Return the size of the data array."""
         return self.coords.size
 
+    @property
+    def seconds(self) -> float:
+        """Return number of seconds in the time coordinate."""
+        return to_float(self.coords.coord_range("time"))
+
+    @property
+    def channel_count(self) -> int:
+        """Return number of channels in the distance coordinate."""
+        return self.coords.coord_size("distance")
+
     # --- basic patch functionality.
 
     update = dascore.proc.update
     # Before 0.1.0 update was called new, this is for backwards compatibility.
     new = dascore.proc.update
     equals = dascore.proc.equals
     update_attrs = dascore.proc.update_attrs
```

### Comparing `dascore-0.1.0/dascore/core/spool.py` & `dascore-0.1.1/dascore/core/spool.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/data_registry.txt` & `dascore-0.1.1/dascore/data_registry.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,7 +13,10 @@
 h5_simple_1.h5 52803b26a5738da541cc9b32b867434cad0a845686c47dd93551b8eb431f8bc0 https://github.com/DASDAE/test_data/raw/master/das/h5_simple_1.h5
 h5_simple_2.h5 8a70b873c5c2c172871ecd63760d24fa2c305c015e2ca1c84018c6864d2fb304 https://github.com/dasdae/test_data/raw/master/das/h5_simple_2.h5
 conoco_segy_1.sgy 3944297d7c27dd265b40d56d4797f1a14caa5c2bed9f0af020b0f6ea193d4dfd https://github.com/dasdae/test_data/raw/master/das/conoco_segy_1.sgy
 brady_hs_DAS_DTS_coords.csv b2e766136aac6516ddbb757d7dc26a8df0d5de48af03c8be769cc50b6816648f https://github.com/dasdae/test_data/raw/master/meta/brady_hs_DAS_DTS_coords.csv
 dispersion_event.h5 598c8baa2a5610c930e1c003f2ba02da13f8d8686e3ccf2a034e94bfc5e1990c https://github.com/dasdae/test_data/raw/master/das/dispersion_event.h5
 PoroTomo_iDAS_1.h5 967a2885e79937ac0426b2022a9c03d5f24790ecf3abbaa9a16eb28055566fc6 https://github.com/dasdae/test_data/raw/master/das/PoroTomo_iDAS_1.h5
 DASDMSShot00_20230328155653619.das 12ac53f78b32d8b0e32cc674c43ff5b4c79a6c8b19de2ad577fd481679b2b7b3 https://github.com/dasdae/test_data/raw/master/das/DASDMSShot00_20230328155653619.das
+opto_das_1.hdf5 0437d1f02d93c9f00d31133388efaf6a28c21883bcfac457b97f1224464c7dca https://github.com/dasdae/test_data/raw/master/das/opto_das_1.hdf5
+whale_1.hdf5 a09922969e740307bf26dc6ffa7fb9fbb834dc7cd7d4ced02c66b159fb1ce0cd http://piweb.ooirsn.uw.edu/das/data/Optasense/NorthCable/TransmitFiber/North-C1-LR-P1kHz-GL50m-Sp2m-FS200Hz_2021-11-03T15_06_51-0700/North-C1-LR-P1kHz-GL50m-Sp2m-FS200Hz_2021-11-04T020002Z.h5
+febus_1.h5 73eba2b6e183b3bca51f8a1448c3b423c979d05ce6c18bfd7fb76b4f9bda5c0b https://github.com/dasdae/test_data/raw/master/das/febus_1.h5
```

### Comparing `dascore-0.1.0/dascore/examples.py` & `dascore-0.1.1/dascore/examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """A module for loading examples."""
 from __future__ import annotations
 
 import tempfile
 from collections.abc import Sequence
+from contextlib import suppress
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 import dascore as dc
 import dascore.core
@@ -409,27 +410,40 @@
 
     from dascore.utils.docs import objs_to_doc_df
 
     df = objs_to_doc_df(EXAMPLE_PATCHES)
     print(df.to_markdown(index=False, stralign="center"))
     ```
 
+    Using an entry from the data_registry file is also supported.
+    If multiple patches are contained in the specified file, only the
+    first is returned. Data registry files are:
+    ```{python}
+    #| echo: false
+    #| output: asis
+    from dascore.utils.downloader import get_registry_df
+    print(get_registry_df()[['name']].to_markdown(index=False, stralign="center"))
+    ```
+
     Parameters
     ----------
     example_name
-        The name of the example to load. Options are:
+        The name of the example to load. Options are listed above.
     **kwargs
         Passed to the corresponding functions to generate data.
 
     Raises
     ------
         (`UnknownExampleError`)['dascore.examples.UnknownExampleError`] if
         unregistered patch is requested.
     """
     if example_name not in EXAMPLE_PATCHES:
+        # Allow the example name to be a data registry entry.
+        with suppress(ValueError):
+            return dc.spool(fetch(example_name))[0]
         msg = (
             f"No example patch registered with name {example_name} "
             f"Registered example patches are {list(EXAMPLE_PATCHES)}"
         )
         raise UnknownExampleError(msg)
     return EXAMPLE_PATCHES[example_name](**kwargs)
 
@@ -447,25 +461,38 @@
 
     from dascore.utils.docs import objs_to_doc_df
 
     df = objs_to_doc_df(EXAMPLE_SPOOLS)
     print(df.to_markdown(index=False, stralign="center"))
     ```
 
+    Using an entry from the data_registry file is also supported.
+    These include:
+    ```{python}
+    #| echo: false
+    #| output: asis
+    from dascore.utils.downloader import get_registry_df
+    print(get_registry_df()[['name']].to_markdown(index=False, stralign="center"))
+    ```
+
     Parameters
     ----------
     example_name
         The name of the example to load. Options are:
     **kwargs
         Passed to the corresponding functions to generate data.
 
     Raises
     ------
-        UnknownExample if unregistered patch is requested.
+    (`UnknownExampleError`)['dascore.examples.UnknownExampleError`] if
+        unregistered patch is requested.
     """
     if example_name not in EXAMPLE_SPOOLS:
+        # Allow the example spool to be a data registry file.
+        with suppress(ValueError):
+            return dc.spool(fetch(example_name))
         msg = (
             f"No example spool registered with name {example_name} "
             f"Registered example spools are {list(EXAMPLE_SPOOLS)}"
         )
         raise UnknownExampleError(msg)
     return EXAMPLE_SPOOLS[example_name](**kwargs)
```

### Comparing `dascore-0.1.0/dascore/exceptions.py` & `dascore-0.1.1/dascore/exceptions.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/__init__.py` & `dascore-0.1.1/dascore/io/__init__.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/core.py` & `dascore-0.1.1/dascore/io/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/dasdae/core.py` & `dascore-0.1.1/dascore/io/dasdae/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/dasdae/utils.py` & `dascore-0.1.1/dascore/io/dasdae/utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/dashdf5/core.py` & `dascore-0.1.1/dascore/io/dashdf5/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/dashdf5/utils.py` & `dascore-0.1.1/dascore/io/dashdf5/utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/h5simple/core.py` & `dascore-0.1.1/dascore/io/h5simple/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/h5simple/utils.py` & `dascore-0.1.1/dascore/io/h5simple/utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/indexer.py` & `dascore-0.1.1/dascore/io/indexer.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/pickle/core.py` & `dascore-0.1.1/dascore/io/pickle/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/prodml/core.py` & `dascore-0.1.1/dascore/io/prodml/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 
     name = "PRODML"
     preferred_extensions = ("hdf5", "h5")
     version = "2.0"
 
     def get_format(self, resource: PyTablesReader) -> tuple[str, str] | bool:
         """
-        Return True if file contains terra15 version 2 data else False.
+        Return True if file contains prodML version 2 data else False.
 
         Parameters
         ----------
         resource
-            A path to the file which may contain terra15 data.
+            A path to the file which may contain prodML data.
         """
         version_str = _get_prodml_version_str(resource)
         if version_str:
             return (self.name, version_str)
 
     def scan(self, resource: PyTablesReader) -> list[dc.PatchAttrs]:
         """Scan a prodml file, return summary information about the file's contents."""
```

### Comparing `dascore-0.1.0/dascore/io/prodml/utils.py` & `dascore-0.1.1/dascore/io/prodml/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Utilities for terra15."""
+"""Utilities for prodML."""
 from __future__ import annotations
 
 import dascore as dc
 from dascore.constants import VALID_DATA_TYPES
 from dascore.core.coordmanager import get_coord_manager
 from dascore.core.coords import get_coord
 from dascore.utils.misc import iterate, maybe_get_attrs, unbyte
 
 # --- Getting format/version
 
 
 def _get_prodml_version_str(hdf_fi) -> str:
     """Return the version string for prodml file."""
-    # define a few root attrs that act as a "fingerprint" for terra15 files
+    # define a few root attrs that act as a "fingerprint" for prodML files
 
     acquisition = getattr(hdf_fi.root, "Acquisition", None)
     if acquisition is None:
         return ""
     acq_attrs = acquisition._v_attrs
     expected_attrs = (
         "GaugeLength",
@@ -111,15 +111,15 @@
     # it is indexed like Raw[0] there might be more.
     out = []
     for node in raw_nodes.values():
         info = dict(base_info)
         t_coord = _get_time_coord(node)
         info.update(t_coord.get_attrs_dict("time"))
         info.update(_get_data_unit_and_type(node))
-        info["dims"] = ["time", "distance"]
+        info["dims"] = _get_dims(node)
         if extras is not None:
             info.update(extras)
         info["coords"] = {"time": t_coord, "distance": d_coord}
         out.append(info)
     return out
```

### Comparing `dascore-0.1.0/dascore/io/rsf/core.py` & `dascore-0.1.1/dascore/io/rsf/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,17 @@
         data_path needs to be bindata_file.rsf or /location/of/bindata_file.rsf
         (NO '@')
 
         path needs to be hdr_file.rsf or /location/of/hdr_file.rsf
 
         spool needs to have a single patch in it
 
+        time origin is forced to 0.0 in the new RSF file, but a dummy
+        variable named 'starttime' still holds the real start time
+
         Parameters
         ----------
         spool
             The input spool to convert to rsf, must have exactly one patch.
         path
             Path to create the rsf file
         data_path
@@ -67,23 +70,27 @@
             raise ValueError("Data format is not integer or floating.")
         ## we are casting to float32 to ensure that esize=4 for m8r
         data = patch.data.astype(np.float32)
         dtype = np.dtype(data.dtype)
         file_esize = dtype.itemsize
         file_formt = 'data_format="native_float"'
 
-        data_bytes = data.astype(np.float32).tobytes()
+        data_bytes = data.astype(np.float32).tobytes("F")
 
         hdr_str = f"DASCORE {dc.__version__}   {dt.datetime.now()} \n"
 
         length = len(axis_lengs)
         hdr_info = [hdr_str, file_formt, f"esize={file_esize}"]
         for i in range(length):
             hdr_info.append(f"n{i+1}={axis_lengs[i]}")
-            hdr_info.append(f"o{i+1}={axis_origs[i]}")
+            if axis_names[i] == "time":
+                hdr_info.append(f"o{i+1}=0.0")
+                hdr_info.append(f"starttime={axis_origs[i]}")
+            else:
+                hdr_info.append(f"o{i+1}={axis_origs[i]}")
             hdr_info.append(f"d{i+1}={axis_steps[i]}")
             hdr_info.append(f'label{i+1}="{axis_names[i]}"')
             hdr_info.append(f'unit{i+1}="{axis_units[i]}"')
 
         if data_path is not None:
             # outputs header and binary separately (.rsf and .rsf@)
             outdatapath = Path(str(data_path) + "@")
```

### Comparing `dascore-0.1.0/dascore/io/segy/core.py` & `dascore-0.1.1/dascore/io/segy/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/segy/utils.py` & `dascore-0.1.1/dascore/io/segy/utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/sentek/core.py` & `dascore-0.1.1/dascore/io/sentek/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/sentek/utils.py` & `dascore-0.1.1/dascore/io/sentek/utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/tdms/core.py` & `dascore-0.1.1/dascore/io/tdms/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/tdms/utils.py` & `dascore-0.1.1/dascore/io/tdms/utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/terra15/__init__.py` & `dascore-0.1.1/dascore/io/terra15/__init__.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/terra15/core.py` & `dascore-0.1.1/dascore/io/terra15/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/terra15/utils.py` & `dascore-0.1.1/dascore/io/terra15/utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/io/wav/core.py` & `dascore-0.1.1/dascore/io/wav/core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/proc/__init__.py` & `dascore-0.1.1/dascore/proc/__init__.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/proc/aggregate.py` & `dascore-0.1.1/dascore/proc/aggregate.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/proc/basic.py` & `dascore-0.1.1/dascore/proc/basic.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/proc/coords.py` & `dascore-0.1.1/dascore/proc/coords.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/proc/correlate.py` & `dascore-0.1.1/dascore/proc/correlate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -72,21 +72,21 @@
     >>> import dascore as dc
     >>> from dascore.units import m, s
 
     >>> patch = dc.get_example_patch()
 
     >>> # Example 1
     >>> # Calculate cc for all channels as receivers and
-    >>> # the 10 m channel as the master channel. The new patch has dimensions
-    >>> # (lag_time, distance)
+    >>> # the 10 m channel as the master channel.
     >>> cc_patch = patch.correlate(distance = 10 * m)
 
     >>> # Example 2
     >>> # Calculate cc within (-2,2) sec of lag for all channels as receivers and
-    >>> # the 10 m channel as the master channel.
+    >>> # the 10 m channel as the master channel. The new patch has dimensions
+    >>> # (lag_time, distance)
     >>> cc_patch = patch.correlate(distance = 10 * m, lag = 2 * s)
 
     >>> # Example 3
     >>> # Use 2nd channel (python is 0 indexed) along distance as master channel
     >>> cc_patch = patch.correlate(distance=1, samples=True)
 
     >>> # Example 4
```

### Comparing `dascore-0.1.0/dascore/proc/detrend.py` & `dascore-0.1.1/dascore/proc/detrend.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/proc/filter.py` & `dascore-0.1.1/dascore/proc/filter.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/proc/resample.py` & `dascore-0.1.1/dascore/proc/resample.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/proc/rolling.py` & `dascore-0.1.1/dascore/proc/rolling.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/proc/select.py` & `dascore-0.1.1/dascore/proc/select.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/proc/taper.py` & `dascore-0.1.1/dascore/proc/taper.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/proc/units.py` & `dascore-0.1.1/dascore/proc/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 from dascore.units import convert_units as u_covert_units
 from dascore.utils.patch import patch_function
 
 
 def _update_attrs_coord_units(patch: dc.Patch, data_units, coords):
     """Update attributes with new units."""
     attrs = patch.attrs
-    data_units = data_units or attrs.get("data_units")
     # set data units
-    attrs = attrs.update(data_units=data_units, coords=coords.to_summary_dict())
+    attrs = attrs.update(
+        data_units=data_units,
+        coords=coords.to_summary_dict(),
+    )
     return attrs
 
 
 @patch_function()
 def set_units(
     patch: PatchType, data_units: str | Quantity | Unit | None = None, **kwargs
 ) -> PatchType:
@@ -42,14 +44,16 @@
     --------
     >>> import dascore as dc
     >>> patch = dc.get_example_patch()
     >>> # set the data units
     >>> patch_with_units = patch.set_units("km/ms")
     >>> # set the units of the distance coordinate
     >>> patch_feet = patch.set_units(distance='feet')
+    >>> # remove data units
+    >>> patch_removed_units = patch_with_units.set_units(None)
     """
     new_coords = patch.coords.set_units(**kwargs)
     new_attrs = _update_attrs_coord_units(patch, data_units, new_coords)
     return patch.new(attrs=new_attrs, coords=new_coords)
 
 
 @patch_function()
```

### Comparing `dascore-0.1.0/dascore/proc/whiten.py` & `dascore-0.1.1/dascore/proc/whiten.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 import numpy.fft as nft
 import pandas as pd
 from scipy.ndimage import convolve1d
 from scipy.signal.windows import tukey
 
 from dascore.constants import PatchType
 from dascore.exceptions import ParameterError
+from dascore.transform.fourier import _get_dft_attrs, _get_dft_new_coords
 from dascore.utils.misc import check_filter_kwargs, check_filter_range
-from dascore.utils.patch import get_dim_sampling_rate
+from dascore.utils.patch import _get_dx_or_spacing_and_axes, get_dim_sampling_rate
 
 
 def whiten(
     patch: PatchType,
     smooth_size: float | None = None,
     tukey_alpha: float = 0.1,
+    ifft: bool = True,
     **kwargs,
 ) -> PatchType:
     """
     Band-limited signal whitening.
+    The whitened signal is returned in either frequency or time domains.
 
     Parameters
     ----------
     patch
         Patch to transform. Has to have dimensions of time and distance.
     smooth_size
         Size (in Hz) of moving average window, used to compute the spectrum
@@ -34,14 +37,17 @@
         the entire spectrum.
     tukey_alpha
         Alpha parameter for Tukey window applied as windowing to the
         smoothed spectrum within the required frequency range. By default
         its value is 0.1.
         See more details at https://docs.scipy.org/doc/scipy/reference
         /generated/scipy.signal.windows.tukey.html
+    ifft
+        If False, returns the whitened result in the frequency domain without
+        converting it back to the time domain. Defaults to True.
     **kwargs
         Used to specify the dimension and frequency, wavelength, or equivalent
         limits. If no input is provided, whitening is also the last axis
         with frequency band of [0,Nyquist]
 
     Notes
     -----
@@ -51,14 +57,20 @@
     2) A tukey window (fixed) is applied to window the smoothed spectrum
        within the frequency range of interest. Be aware of its effect and
        consider enlarging the frequency range according to the tukey_alpha
        parameter.
 
     3) Amplitude is NOT preserved
 
+    4) If ifft = False, since for the purely real input data the negative
+       frequency terms are just the complex conjugates of the corresponding
+       positive-frequency terms, the output does not include the negative
+       frequency terms, and therefore the length of the transformed axis
+       of the output is n//2 + 1. Refer to the
+       [dft patch function](`dascore.transform.fourier.dft`) and its `real` flag.
 
     Example
     -------
     ```{python}
     import matplotlib.pyplot as plt
     import numpy as np
     import numpy.fft as fft
@@ -210,14 +222,24 @@
         if d > 1:
             tiled_win = np.tile(np.expand_dims(tiled_win, axis=-1), (1, d))
 
     tiled_win = np.transpose(tiled_win, np.roll(np.arange(len(exp_dims)), dim_ind))
 
     norm_amp *= tiled_win
 
-    # Revert back to time-domain, using the phase of the original signal
-    whitened_data = np.real(
-        nft.irfft(norm_amp * np.exp(1j * phase), n=comp_nsamp, axis=dim_ind)
-    )
-    whitened_data = np.take(whitened_data, np.arange(nsamp), axis=dim_ind)
-
-    return patch.new(data=whitened_data)
+    if ifft:
+        # revert back to time-domain, using the phase of the original signal
+        whitened_data = np.real(
+            nft.irfft(norm_amp * np.exp(1j * phase), n=comp_nsamp, axis=dim_ind)
+        )
+        whitened_data = np.take(whitened_data, np.arange(nsamp), axis=dim_ind)
+        return patch.new(data=whitened_data)
+    else:
+        dims = list(patch.dims)
+        dxs, axes = _get_dx_or_spacing_and_axes(patch, dims, require_evenly_spaced=True)
+        # get new coordinates
+        real = dims[dim_ind]
+        new_coords = _get_dft_new_coords(patch, dxs, dims, axes, real)
+        # get attributes
+        attrs = _get_dft_attrs(patch, dims, new_coords)
+        # return the frequency domain data directly without taking the inverse FFT
+        return patch.new(norm_amp * np.exp(1j * phase), coords=new_coords, attrs=attrs)
```

### Comparing `dascore-0.1.0/dascore/transform/differentiate.py` & `dascore-0.1.1/dascore/transform/differentiate.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/transform/dispersion.py` & `dascore-0.1.1/dascore/transform/dispersion.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/transform/fft.py` & `dascore-0.1.1/dascore/transform/fft.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/transform/fourier.py` & `dascore-0.1.1/dascore/transform/fourier.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/transform/integrate.py` & `dascore-0.1.1/dascore/transform/integrate.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,32 +54,36 @@
 def _get_indefinite_integral(patch, dxs_or_vals, axes):
     """
     Get indefinite integral along dimensions.
 
     We need to calculate the distance weighted average for the areas between
     samples for the integration dimension.
     """
-    array = np.array(patch.data)
+    out = np.zeros_like(patch.data)
+    array = patch.data
     for dx_or_val, ax in zip(dxs_or_vals, axes):
         # if coordinate values are provided need to get diffs.
         if isinstance(dx_or_val, np.ndarray):
             dx_or_val = dx_or_val[1:] - dx_or_val[:-1]
-        ndim = len(array.shape)
+        ndim = len(out.shape)
         # get diffs along dimension
         stop_indexer = broadcast_for_index(ndim, ax, slice(1, None), fill=slice(None))
         start_indexer = broadcast_for_index(ndim, ax, slice(None, -1), fill=slice(None))
+        # first_indexer = broadcast_for_index(ndim, ax, slice(0, 1), fill=slice(None))
         # get average values of trapezoid between points
-        avs = (array[stop_indexer] + array[start_indexer]) / (2 * dx_or_val)
-        array[stop_indexer] = np.cumsum(avs, axis=ax)
-    return array, patch.coords  # coords shouldn't change
+        avs = (array[stop_indexer] + array[start_indexer]) * (dx_or_val / 2)
+        out[stop_indexer] = np.cumsum(avs, axis=ax)
+    return out, patch.coords  # coords shouldn't change
 
 
 @patch_function()
 def integrate(
-    patch: PatchType, dim: Sequence[str] | str | None, definite: bool = False
+    patch: PatchType,
+    dim: Sequence[str] | str | None,
+    definite: bool = False,
 ) -> PatchType:
     """
     Integrate along a specified dimension using composite trapezoidal rule.
 
     Parameters
     ----------
     patch
@@ -87,21 +91,22 @@
     dim
         The dimension(s) along which to integrate. If None, integrate along
         all dimensions.
     definite
         If True, consider the integration to be defined from the minimum to
         the maximum value along specified dimension(s). In essense, this
         collapses the integrated dimensions to a lenght of 1.
-        If define is False, the shape of the patch is preserved.
+        If define is False, the shape of the patch is preserved and a
+        "cumulative" type integration in performed.
 
     Notes
     -----
     The number of dimensions will always remain the same regardless of `definite`
-    value. To remove dimensions with length 1, see
-    [squeeze](`dascore.proc.basic.squeeze`)
+    value. To remove dimensions with length 1,
+    see [squeeze](`dascore.proc.basic.squeeze`).
 
     Examples
     --------
     >>> import dascore as dc
     >>> patch = dc.get_example_patch()
     >>> # integrate along time axis, preserve patch shape with indefinite integral
     >>> time_integrated = patch.integrate(dim="time", definite=False)
```

### Comparing `dascore-0.1.0/dascore/transform/spectro.py` & `dascore-0.1.1/dascore/transform/spectro.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/transform/strain.py` & `dascore-0.1.1/dascore/transform/strain.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/units.py` & `dascore-0.1.1/dascore/units.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/chunk.py` & `dascore-0.1.1/dascore/utils/chunk.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/display.py` & `dascore-0.1.1/dascore/utils/display.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/docs.py` & `dascore-0.1.1/dascore/utils/docs.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/downloader.py` & `dascore-0.1.1/dascore/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/hdf5.py` & `dascore-0.1.1/dascore/utils/hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,7 +452,19 @@
     mode = "a"
 
 
 # These are left here for backward compatibility, but should not be
 # used in new code.
 HDF5Writer = PyTablesWriter
 HDF5Reader = PyTablesReader
+
+
+def unpack_scalar_h5_dataset(dataset):
+    """
+    Unpack a scalar H5Py dataset.
+    """
+    assert dataset.size == 1
+    # This gets weird because datasets can be of shape () or (1,).
+    value = dataset[()]
+    if isinstance(value, np.ndarray):
+        value = value[0]
+    return value
```

### Comparing `dascore-0.1.0/dascore/utils/io.py` & `dascore-0.1.1/dascore/utils/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from dascore.constants import PatchType
 from dascore.exceptions import PatchConversionError
 from dascore.utils.misc import (
     _maybe_make_parent_directory,
     cached_method,
     optional_import,
 )
+from dascore.utils.time import to_float
 
 HANDLE_FUNCTIONS = {
     str: lambda x: str(x),
     Path: lambda x: Path(x),
 }
 
 
@@ -178,18 +179,22 @@
         if not has_time and is_2d:
             msg = "Can only convert 2d patches with a time dimension to stream."
             raise PatchConversionError(msg)
 
     def _get_time_stats(patch):
         """Get stats dict with time values."""
         coord = patch.get_coord("time")
+        tmin = dc.to_datetime64(coord.min())
+        tmax = dc.to_datetime64(coord.max())
+        dt = np.timedelta64(1, "s") / coord.step
+
         time_stats = {
-            "starttime": obspy.UTCDateTime(str(coord.min())),
-            "endtime": obspy.UTCDateTime(str(coord.max())),
-            "sampling_rate": np.timedelta64(1, "s") / coord.step,
+            "starttime": obspy.UTCDateTime(str(tmin)),
+            "endtime": obspy.UTCDateTime(str(tmax)),
+            "sampling_rate": to_float(dt),
         }
         return time_stats
 
     _check_patch(patch)
     # ensure time is last axis
     patch = patch.transpose(..., "time")
     other_dim = next(iter(set(patch.dims) - {"time"}))
```

### Comparing `dascore-0.1.0/dascore/utils/mapping.py` & `dascore-0.1.1/dascore/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/misc.py` & `dascore-0.1.1/dascore/utils/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -385,24 +385,47 @@
     for old_name, new_name in attr_map.items():
         if hasattr(obj, old_name):
             value = getattr(obj, old_name)
             out[new_name] = unbyte(value)
     return out
 
 
-def maybe_get_items(obj, attr_map: Mapping):
-    """Maybe get items from a mapping (if they exist)."""
+def maybe_get_items(
+    obj, attr_map: Mapping[str, str], unpack_names: None | set[str] = None
+):
+    """
+    Maybe get items from a mapping (if they exist).
+
+    Parameters
+    ----------
+    obj
+        Any map like object.
+    attr_map
+        A mapping of {current_name: output_name}
+    unpack_names
+        A set of names which should be unpacked (ie collapse 0d arrays).
+    """
+    unpack_names = set() if unpack_names is None else unpack_names
     out = {}
     for old_name, new_name in attr_map.items():
         if not (value := obj.get(old_name, None)):
             continue
-        out[new_name] = unbyte(value)
+        val = unbyte(value)
+        out[new_name] = _maybe_unpack(val) if old_name in unpack_names else val
     return out
 
 
+def _maybe_unpack(maybe_array):
+    """Unpack an array like object if it is size one, else return input."""
+    size = getattr(maybe_array, "size", 0)
+    if size == 1:
+        maybe_array = maybe_array[0]
+    return maybe_array
+
+
 @cache
 def _get_compiled_suffix_prefix_regex(
     suffixes: str | tuple[str],
     prefixes: str | tuple[str] | None,
 ):
     """Get a compiled regex which matches the form prefixes_suffixes."""
     suffixes = iterate(suffixes)
@@ -448,24 +471,40 @@
         names which cannot be on their own.
 
     Returns
     -------
     coord_dict and attrs_dict.
     """
 
-    def _meets_required(coord_dict):
-        """Return True coord dict meets the minimum required keys."""
+    def _meets_required(coord_dict, strict=True):
+        """
+        Return True coord dict meets the minimum required keys.
+
+        coord_dict represents potential coordinate fields.
+
+        Strict ensures all required values exist.
+        """
         if not coord_dict:
             return False
         if not required and (set(coord_dict) - cant_be_alone):
             return True
-        return set(coord_dict).issuperset(required)
+        if required or not strict:
+            return set(coord_dict).issuperset(required)
+        return False
 
     def _get_dims(obj):
         """Try to ascertain dims from keys in obj."""
+        # check first for coord manager
+        if isinstance(obj, dict) and hasattr(obj.get("coords", None), "dims"):
+            return obj["coords"].dims
+
+        # This object already has dims, just honor it.
+        if dims := obj.get("dims", None):
+            return tuple(dims.split(",")) if isinstance(dims, str) else dims
+
         potential_keys = defaultdict(set)
         for key in obj:
             if not is_valid_coord_str(key):
                 continue
             potential_keys[key.split("_")[0]].add(key.split("_")[1])
         return tuple(i for i, v in potential_keys.items() if _meets_required(v))
 
@@ -477,59 +516,64 @@
             }
             # nasty hack for handling d_{dim} for backward compatibility.
             if (bad_name := f"d_{dim}") in obj:
                 msg = f"d_{dim} is deprecated, use {dim}_step"
                 warnings.warn(msg, DeprecationWarning, stacklevel=3)
                 potential_coord["step"] = obj[bad_name]
 
-            if _meets_required(potential_coord):
+            if _meets_required(potential_coord, strict=False):
                 out[dim] = potential_coord
 
     def _get_coords_from_coord_level(obj, out):
         """Get coords from coordinate level."""
         coords = obj.get("coords", {})
         if hasattr(coords, "to_summary_dict"):
             coords = coords.to_summary_dict()
         for key, value in coords.items():
             if hasattr(value, "to_summary"):
                 value = value.to_summary()
             if hasattr(value, "model_dump"):
                 value = value.model_dump()
-            if _meets_required(value):
+            if _meets_required(value, strict=False):
                 out[key] = value
 
     def _pop_keys(obj, out):
         """Pop out old keys for attrs, and unused keys from out."""
         # first coord subdict
         obj.pop("coords", None)
         # then top-level
         for coord_name, sub_dict in out.items():
             for thing_name in sub_dict:
                 obj.pop(f"{coord_name}_{thing_name}", None)
             if "step" in sub_dict:
                 obj.pop(f"d_{coord_name}", None)
 
     # sequence of short-circuit checks
-    out = {}
+    coord_dict = {}
     required = set(required) if required is not None else set()
     cant_be_alone = set(cant_be_alone)
     if obj is None:
-        return out, {}
+        return coord_dict, {}
     if hasattr(obj, "model_dump"):
         obj = obj.model_dump()
-    if dims is None:
-        dims = _get_dims(obj)
+    obj = dict(obj)
+    # Check if dims need to be updated.
+    new_dims = _get_dims(obj)
+    if new_dims and new_dims != dims:
+        obj["dims"] = new_dims
+        dims = new_dims
     # this is already a dict of coord info.
-    if set(dims) == set(obj):
+    if dims and set(dims) == set(obj):
         return obj, {}
-    obj = dict(obj)
-    _get_coords_from_coord_level(obj, out)
-    _get_coords_from_top_level(obj, out, dims)
-    _pop_keys(obj, out)
-    return out, obj
+    _get_coords_from_coord_level(obj, coord_dict)
+    _get_coords_from_top_level(obj, coord_dict, dims)
+    _pop_keys(obj, coord_dict)
+    if "dims" not in obj and dims is not None:
+        obj["dims"] = dims
+    return coord_dict, obj
 
 
 def cached_method(func):
     """
     Cache decorated method.
 
     Simply uses the id of self for the key rather than hashing it.
```

### Comparing `dascore-0.1.0/dascore/utils/models.py` & `dascore-0.1.1/dascore/utils/models.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/patch.py` & `dascore-0.1.1/dascore/utils/patch.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/pd.py` & `dascore-0.1.1/dascore/utils/pd.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/plotting.py` & `dascore-0.1.1/dascore/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/progress.py` & `dascore-0.1.1/dascore/utils/progress.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/time.py` & `dascore-0.1.1/dascore/utils/time.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/utils/transformatter.py` & `dascore-0.1.1/dascore/utils/transformatter.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/viz/spectrogram.py` & `dascore-0.1.1/dascore/viz/spectrogram.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/viz/waterfall.py` & `dascore-0.1.1/dascore/viz/waterfall.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore/viz/wiggle.py` & `dascore-0.1.1/dascore/viz/wiggle.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/dascore.egg-info/SOURCES.txt` & `dascore-0.1.1/dascore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,23 @@
 dascore/io/indexer.py
 dascore/io/dasdae/__init__.py
 dascore/io/dasdae/core.py
 dascore/io/dasdae/utils.py
 dascore/io/dashdf5/__init__.py
 dascore/io/dashdf5/core.py
 dascore/io/dashdf5/utils.py
+dascore/io/febus/__init__.py
+dascore/io/febus/core.py
+dascore/io/febus/utils.py
 dascore/io/h5simple/__init__.py
 dascore/io/h5simple/core.py
 dascore/io/h5simple/utils.py
+dascore/io/optodas/__init__.py
+dascore/io/optodas/core.py
+dascore/io/optodas/utils.py
 dascore/io/pickle/__init__.py
 dascore/io/pickle/core.py
 dascore/io/prodml/__init__.py
 dascore/io/prodml/core.py
 dascore/io/prodml/utils.py
 dascore/io/rsf/__init__.py
 dascore/io/rsf/core.py
```

### Comparing `dascore-0.1.0/docs/LICENSE` & `dascore-0.1.1/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/pyproject.toml` & `dascore-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,17 @@
 
 # --- Entry Points
 
 [project.entry-points."dascore.fiber_io"]
 DASDAE__V1 = "dascore.io.dasdae.core:DASDAEV1"
 DASHDF5__V1 = "dascore.io.dashdf5.core:DASHDF5"
 H5SIMPLE__V1_0 = "dascore.io.h5simple.core:H5Simple"
+FEBUS__V1 = "dascore.io.febus.core:Febus1"
+FEBUS__V2 = "dascore.io.febus.core:Febus2"
+OPTODAS__V8 = "dascore.io.optodas.core:OptoDASV8"
 PICKLE = "dascore.io.pickle.core:PickleIO"
 PRODML__V2_0 = "dascore.io.prodml.core:ProdMLV2_0"
 PRODML__V2_1 = "dascore.io.prodml.core:ProdMLV2_1"
 SENTEK__V5 = "dascore.io.sentek.core:SentekV5"
 TDMS__V4713 = "dascore.io.tdms.core:TDMSFormatterV4713"
 TERRA15__V4 = "dascore.io.terra15.core:Terra15FormatterV4"
 TERRA15__V5 = "dascore.io.terra15.core:Terra15FormatterV5"
```

### Comparing `dascore-0.1.0/readme.md` & `dascore-0.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/conftest.py` & `dascore-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_clients/test_dirspool.py` & `dascore-0.1.1/tests/test_clients/test_dirspool.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_clients/test_filespool.py` & `dascore-0.1.1/tests/test_clients/test_filespool.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_core/test_attrs.py` & `dascore-0.1.1/tests/test_core/test_attrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,19 @@
 
     def test_items(self, random_patch):
         """Ensure items works like a dict."""
         attrs = random_patch.attrs
         out = dict(attrs.items())
         assert out == attrs.model_dump()
 
+    def test_dims_match_attrs(self, random_patch):
+        """Ensure the dims from patch attrs matches patch dims."""
+        pat = random_patch.rename_coords(distance="channel")
+        assert pat.dims == pat.attrs.dim_tuple
+
 
 class TestSummaryAttrs:
     """Tests for summarizing a schema."""
 
     def test_attrs_reconstructed(self, random_patch, random_summary):
         """Ensure all the expected attrs are extracted."""
         summary1 = dict(random_summary)
@@ -284,14 +289,21 @@
 
     def test_attrs_can_update(self, random_attrs):
         """Ensure attributes can update coordinates."""
         attrs = random_attrs.update(distance_units="miles")
         expected = dc.get_quantity("miles")
         assert dc.get_quantity(attrs.coords["distance"].units) == expected
 
+    def test_update_from_coords(self, random_patch):
+        """Ensure attrs.update updates dims from coords."""
+        attrs = random_patch.attrs
+        new_patch = random_patch.rename_coords(distance="channel")
+        new = attrs.update(coords=new_patch.coords)
+        assert new.dim_tuple == new_patch.dims
+
 
 class TestMergeAttrs:
     """Tests for merging patch attrs."""
 
     def test_empty(self):
         """Empty PatchAttrs should work in all cases."""
         pa1, pa2 = PatchAttrs(), PatchAttrs()
```

### Comparing `dascore-0.1.0/tests/test_core/test_coordmanager.py` & `dascore-0.1.1/tests/test_core/test_coordmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,27 +252,27 @@
         assert set(sum_dict) == set(coord_manager.coord_map)
 
     def test_size(self, coord_manager):
         """Ensure all coord managers have a size."""
         assert isinstance(coord_manager.size, int | np.int_)
 
     def test_min(self, basic_coord_manager):
-        """Ensure we can git min value."""
+        """Ensure we can get min value."""
         expected = np.min(basic_coord_manager.time.data).astype(np.int64)
         got = basic_coord_manager.min("time").astype(np.int64)
         assert np.isclose(got, expected)
 
     def test_max(self, basic_coord_manager):
-        """Ensure we can git max value."""
+        """Ensure we can get max value."""
         expected = np.max(basic_coord_manager.time.data).astype(np.int64)
         got = basic_coord_manager.max("time").astype(np.int64)
         assert np.isclose(got, expected)
 
     def test_step(self, basic_coord_manager):
-        """Ensure we can git min value."""
+        """Ensure we can get min value."""
         expected = basic_coord_manager.time.step
         assert basic_coord_manager.step("time") == expected
 
     def test_getattr(self, basic_coord_manager):
         """Ensure getattr returns coordinate."""
         for dim in basic_coord_manager.dims:
             coord = getattr(basic_coord_manager, dim)
@@ -293,14 +293,27 @@
 
     def test_iterate(self, basic_coord_manager):
         """Ensure coordinates yield name an coordinate when iterated."""
         for dim, coord in iter(basic_coord_manager):
             expected = basic_coord_manager.get_coord(dim)
             assert all_close(coord, expected)
 
+    def test_coord_size(self, random_patch):
+        """Ensure we can get size of the coordinate."""
+        expected = len(random_patch.get_coord("time"))
+        assert random_patch.coords.coord_size("time") == expected
+
+    def test_coord_range(self, random_patch):
+        """Ensure we can get a scaler value for the coordinate."""
+        coord_array = random_patch.get_coord("time").data
+        expected = (
+            np.max(coord_array) - np.min(coord_array) + random_patch.attrs["time_step"]
+        )
+        assert random_patch.coords.coord_range("time") == expected
+
 
 class TestCoordManagerInputs:
     """Tests for coordinates management."""
 
     def test_simple_inputs(self):
         """Simplest input case."""
         out = get_coord_manager(COORDS, DIMS)
@@ -552,14 +565,34 @@
             assert coord.shape[time_id] == 2
 
     def test_samples_slice(self, coord_manager):
         """Ensure we can select when samples=True using ... or None."""
         new, _ = coord_manager.select(time=..., samples=True)
         assert new == coord_manager
 
+    def test_select_shared_dims(self, coord_manager):
+        """Ensure selections work when queries share a dimension."""
+        dist = coord_manager.get_coord("distance")
+        new_coord = np.arange(len(dist))
+        cm = coord_manager.update_coords(
+            d1=("distance", new_coord),
+            d2=("distance", new_coord),
+        )
+        # Relative values should raise when the same dim is targeted by
+        # multiple coords.
+        with pytest.raises(CoordError):
+            cm.select(d1=(3, None), d2=(None, 6), relative=True)
+        # Same for samples.
+        with pytest.raises(CoordError):
+            cm.select(d1=(3, None), d2=(None, 6), samples=True)
+        # But normal values should work and produce a shape of 4 for this case.
+        out, _ = cm.select(d1=(3, None), d2=(None, 6))
+        distance_dim = out.dims.index("distance")
+        assert out.shape[distance_dim] == 4
+
 
 class TestEquals:
     """Tests for coord manager equality."""
 
     def test_basic_equals(self, coord_manager):
         """All coord managers should equal themselves."""
         assert coord_manager == coord_manager
```

### Comparing `dascore-0.1.0/tests/test_core/test_coords.py` & `dascore-0.1.1/tests/test_core/test_coords.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     ar = dc.to_timedelta64(np.arange(1, 100_000, 1_000))
     return get_coord(data=ar)
 
 
 @pytest.fixture(scope="session")
 @register_func(COORDS)
 def monotonic_float_coord():
-    """Create coordinates which are evenly sampled."""
+    """Create coordinates which are not evenly sampled."""
     ar = np.cumsum(np.abs(np.random.rand(100)))
     return get_coord(data=ar)
 
 
 @pytest.fixture(scope="session")
 @register_func(COORDS)
 def reverse_monotonic_float_coord():
@@ -238,14 +238,15 @@
         assert isinstance(out, rich.text.Text)
 
     def test_snap(self, coord):
         """Tests for snapping coordinates."""
         out = coord.snap()
         assert isinstance(out, BaseCoord)
         assert out.shape == coord.shape
+        assert out.size == coord.size
         # sort order should stay the same
         if coord.reverse_sorted:
             assert out.reverse_sorted
         if coord.sorted:
             assert out.sorted
 
     def test_default_units(self):
@@ -324,14 +325,20 @@
     def test_both_values_and_data_raises(self):
         """Cannot specify both values and data."""
         data = np.empty(10)
         msg = "Cannot specify both data and values"
         with pytest.raises(CoordError, match=msg):
             get_coord(data=data, values=data)
 
+    def test_coord_range(self, monotonic_float_coord):
+        """Ensure that coord_range raises an error for not evenly sampled patches."""
+        msg = "has to be called on an evenly sampled"
+        with pytest.raises(CoordError, match=msg):
+            monotonic_float_coord.coord_range()
+
 
 class TestCoordSummary:
     """tests for converting to and from summary coords."""
 
     cast_data_list: ClassVar = [
         {"min": 400.0, "step": 1.0, "units": "", "max": 1000.0},
         {"min": 0, "max": 10},
@@ -855,25 +862,45 @@
         """Ensure np.arange produces same len as get_coord, start, stop, step."""
         start = -120.02095199999974
         stop = 1055.2182894582486
         step = 1.0209523838714072
         ar = np.arange(start, stop, step)
         coord = get_coord(start=start, stop=stop, step=step)
         assert coord.shape == ar.shape
+        assert coord.size == ar.size
 
     def test_unchanged_len(self):
         """Ensure an array converted to Coord range has same len. See #229."""
         t_array = np.linspace(0.0, 1, 44100)
         t_coord = get_coord(data=t_array)
         assert t_array.shape == t_coord.shape
         # now test datetime
         time = dc.to_timedelta64(t_array) + np.datetime64("2020-01-01")
         time_coord = get_coord(data=time)
         assert len(time) == len(time_coord)
 
+    def test_change_length_no_change(self, evenly_sampled_coord):
+        """Ensure change_length works when no length change is needed."""
+        new = evenly_sampled_coord.change_length(len(evenly_sampled_coord))
+        assert new == evenly_sampled_coord
+
+    def test_change_length_lengthen(self, evenly_sampled_float_coord_with_units):
+        """Ensure the length can increase."""
+        coord = evenly_sampled_float_coord_with_units
+        current = len(coord)
+        new = coord.change_length(current + 1)
+        assert len(new) == current + 1
+
+    def test_change_length_shorten(self, evenly_sampled_float_coord_with_units):
+        """Ensure the length can increase."""
+        coord = evenly_sampled_float_coord_with_units
+        current = len(coord)
+        new = coord.change_length(current - 1)
+        assert len(new) == current - 1
+
 
 class TestMonotonicCoord:
     """Tests for monotonic array coords."""
 
     def test_select_basic(self, monotonic_float_coord):
         """Basic select tests for monotonic array."""
         coord = monotonic_float_coord
@@ -1023,18 +1050,17 @@
     """Tests for non-ordered array coords."""
 
     def test_select(self, random_coord):
         """Ensure selecting returns an ndarray."""
         min_v, max_v = np.min(random_coord.values), np.max(random_coord.values)
         dist = max_v - min_v
         val1, val2 = min_v + 0.2 * dist, max_v - 0.2 * dist
-        new, bool_array = random_coord.select((val1, val2))
+        new, ind_array = random_coord.select((val1, val2))
         assert np.all(new.values >= val1)
         assert np.all(new.values <= val2)
-        assert bool_array.sum() == len(new)
 
     def test_sort(self, random_coord):
         """Ensure the coord can be ordered."""
         new, ordering = random_coord.sort()
         assert isinstance(new, CoordMonotonicArray)
 
     def test_snap(self, random_coord):
```

### Comparing `dascore-0.1.0/tests/test_core/test_patch.py` & `dascore-0.1.1/tests/test_core/test_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,21 @@
         patch = dc.Patch(data=data, coords={"x": x, "y": y}, dims=("x", "y"))
         assert isinstance(patch, dc.Patch)
 
     def test_patch_has_size(self, random_patch):
         """Ensure patches have same size as data."""
         assert random_patch.size == random_patch.data.size
 
+    def test_new_patch_non_standard_dims(self):
+        """Ensure a non-standard dimension has matching dims in attrs and coords."""
+        data = np.random.rand(10, 5)
+        coords = {"time": np.arange(10), "can": np.arange(5)}
+        patch = dc.Patch(data=data, coords=coords, dims=("time", "can"))
+        assert patch.dims == patch.attrs.dim_tuple
+
 
 class TestNew:
     """Tests for `Patch.new` method."""
 
     def test_erase_history(self, random_patch):
         """Ensure new can erase history."""
         # do some processing, so history shows up.
@@ -548,14 +555,30 @@
         patch = multi_dim_coords_patch
         time = patch.coords.coord_map["time"]
         new = patch.select(time=(time.min(), time.min()))
         assert 1 in new.shape
         new_coords = new.coords.coord_map
         assert isinstance(new_coords["time"], CoordRange)
 
+    def test_seconds(self, random_patch_with_lat):
+        """Ensure we can get number of seconds in the patch."""
+        sampling_interval = random_patch_with_lat.attrs["time_step"] / np.timedelta64(
+            1, "s"
+        )
+        expected = (
+            random_patch_with_lat.attrs["time_max"]
+            - random_patch_with_lat.attrs["time_min"]
+        ) / np.timedelta64(1, "s") + sampling_interval
+        assert random_patch_with_lat.seconds == expected
+
+    def test_channel_count(self, random_patch_with_lat):
+        """Ensure we can get number of channels in the patch."""
+        expected = len(random_patch_with_lat.get_coord("distance"))
+        assert random_patch_with_lat.channel_count == expected
+
 
 class TestApplyOperator:
     """Tests for applying various ufunc-type operators."""
 
     ops = (
         operator.add,
         operator.sub,
```

### Comparing `dascore-0.1.0/tests/test_core/test_patch_chunk.py` & `dascore-0.1.1/tests/test_core/test_patch_chunk.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_core/test_spool.py` & `dascore-0.1.1/tests/test_core/test_spool.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_examples.py` & `dascore-0.1.1/tests/test_examples.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,28 +33,38 @@
         assert isinstance(out, dc.Patch)
 
     def test_sin_wav(self):
         """Ensure the sin wave example can be loaded. See issee 229."""
         out = dc.get_example_patch("sin_wav")
         assert isinstance(out, dc.Patch)
 
+    def test_data_file_name(self):
+        """Ensure get_example_spool works on a datafile."""
+        spool = dc.get_example_spool("dispersion_event.h5")
+        assert isinstance(spool, dc.BaseSpool)
+
 
 class TestGetExampleSpool:
     """Test suite for `get_example_spool`."""
 
     def test_default(self):
         """Ensure calling get_example_spool with no args returns a Spool."""
         patch = dc.get_example_spool()
         assert isinstance(patch, dc.BaseSpool)
 
     def test_raises_on_bad_key(self):
         """Ensure a bad key raises expected error."""
         with pytest.raises(UnknownExampleError, match="No example spool"):
             dc.get_example_spool("NotAnExampleRight????")
 
+    def test_data_file_name(self):
+        """Ensure get_example_spool works on a datafile."""
+        spool = dc.get_example_spool("dispersion_event.h5")
+        assert isinstance(spool, dc.BaseSpool)
+
 
 class TestRickerMoveout:
     """Tests for Ricker moveout patch."""
 
     def test_moveout(self):
         """Ensure peaks of ricker wavelet line up with expected moveout."""
         velocity = 100
```

### Comparing `dascore-0.1.0/tests/test_integrations/test_doc_examples.py` & `dascore-0.1.1/tests/test_integrations/test_doc_examples.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_io/test_common_io.py` & `dascore-0.1.1/tests/test_io/test_common_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 import pandas as pd
 import pytest
 
 import dascore as dc
 from dascore.io import BinaryReader
 from dascore.io.dasdae import DASDAEV1
 from dascore.io.dashdf5 import DASHDF5
+from dascore.io.febus import Febus2
 from dascore.io.h5simple import H5Simple
+from dascore.io.optodas import OptoDASV8
 from dascore.io.pickle import PickleIO
 from dascore.io.prodml import ProdMLV2_0, ProdMLV2_1
 from dascore.io.segy import SegyV2
 from dascore.io.sentek import SentekV5
 from dascore.io.tdms import TDMSFormatterV4713
 from dascore.io.terra15 import (
     Terra15FormatterV4,
@@ -43,14 +45,16 @@
 # read, scan, and get_format tests that all FiberIO instances which implement
 # more than just a write method should pass.
 # The format is {FiberIO class: [path_or_fetch_name]} where fetch_name
 # is the name passed to dascore.utils.downloader.fetch to load the file.
 # See the docs on adding a new IO format, in the contributing section,
 # for more details.
 COMMON_IO_READ_TESTS = {
+    Febus2(): ("febus_1.h5",),
+    OptoDASV8(): ("opto_das_1.hdf5",),
     DASDAEV1(): ("example_dasdae_event_1.h5",),
     H5Simple(): ("h5_simple_2.h5", "h5_simple_1.h5"),
     ProdMLV2_0(): ("prodml_2.0.h5", "opta_sense_quantx_v2.h5"),
     ProdMLV2_1(): (
         "prodml_2.1.h5",
         "iDAS005_hdf5_example.626.h5",
     ),
@@ -67,14 +71,17 @@
 }
 
 # This tuple is for fiber io which support a write method and can write
 # generic patches. If the patch has to be in some special form, for example
 # only flat patches can be written to WAV, don't put it here.
 COMMON_IO_WRITE_TESTS = (PickleIO(), DASDAEV1())
 
+# Specifies data registry entries which should not be tested.
+SKIP_DATA_FILES = {"whale_1.hdf5", "brady_hs_DAS_DTS_coords.csv"}
+
 
 @cache
 def _cached_read(path, io=None):
     """
     A function to read data without any params and cache.
     This ensures each files is read at most twice.
     """
@@ -107,18 +114,18 @@
     io, fetch_name = request.param
     return io, fetch(fetch_name)
 
 
 @pytest.fixture(scope="session", params=get_registry_df()["name"])
 def data_file_path(request):
     """A fixture of all data files. Will download if needed."""
-    # TODO remove this segy skip once we support it.
     param = request.param
-    if param.endswith("csv"):
-        pytest.skip("Not a DAS file.")
+    # Some files should be skipped if not DAS or too big.
+    if str(param) in SKIP_DATA_FILES:
+        pytest.skip(f"Skipping {param}")
     return fetch(request.param)
 
 
 @pytest.fixture(scope="session")
 def read_spool(data_file_path):
     """Read each file into a spool."""
     out = dc.read(data_file_path)
@@ -261,15 +268,15 @@
             pytest.skip("Haven't implemented test for multipatch files.")
         attrs_init = attrs_from_file[0]
         for dim in attrs_init.dim_tuple:
             start = getattr(attrs_init, f"{dim}_min")
             stop = getattr(attrs_init, f"{dim}_max")
             duration = stop - start
             # first test double ended query
-            trim_tuple = (start + duration / 10, start + 2 * duration // 10)
+            trim_tuple = (start + duration / 10, start + 2 * duration / 10)
             spool = io.read(path, **{dim: trim_tuple})
             assert len(spool) == 1
             patch = spool[0]
             _assert_coords_attrs_match(patch)
             coord = patch.get_coord(dim)
             _assert_op_or_close(coord.min(), trim_tuple[0], ge)
             _assert_op_or_close(coord.max(), trim_tuple[1], le)
```

### Comparing `dascore-0.1.0/tests/test_io/test_dasdae/test_dasdae.py` & `dascore-0.1.1/tests/test_io/test_dasdae/test_dasdae.py`

 * *Files 16% similar despite different names*

```diff
@@ -167,14 +167,16 @@
         common = list((set(df1) & set(df2)) - {"path"})
         assert df1[common].equals(df2[common])
 
 
 class TestRoundTrips:
     """Tests for round-tripping various patches/spools."""
 
+    formatter = DASDAEV1()
+
     def test_write_patch_with_lat_lon(
         self, random_patch_with_lat_lon, tmp_path_factory
     ):
         """
         DASDAE should support writing patches with non-dimensional
         coords.
         """
@@ -198,26 +200,49 @@
         path = tmp_path_factory.mktemp("round_trip_time_degenerate") / "out.h5"
         patch = random_patch
         # get degenerate patch
         time = patch.get_coord("time")
         time_max = time.max() + 3 * time.step
         empty_patch = patch.select(time=(time_max, ...))
         empty_patch.io.write(path, "dasdae")
-        formatter = DASDAEV1()
-        spool = formatter.read(path)
+        spool = self.formatter.read(path)
         new_patch = spool[0]
         assert empty_patch.equals(new_patch)
 
     def test_roundtrip_dim_1_patch(self, tmp_path_factory, random_patch):
         """A patch with length 1 time axis should roundtrip."""
         path = tmp_path_factory.mktemp("round_trip_dim_1") / "out.h5"
         patch = dc.get_example_patch(
             "random_das",
             time_step=0.999767552,
             shape=(100, 1),
             time_min="2023-06-13T15:38:00.49953408",
         )
         patch.io.write(path, "dasdae")
-        formatter = DASDAEV1()
-        spool = formatter.read(path)
+
+        spool = self.formatter.read(path)
         new_patch = spool[0]
         assert patch.equals(new_patch)
+
+    def test_roundtrip_datetime_coord(self, tmp_path_factory, random_patch):
+        """Ensure a patch with an attached datetime coord works."""
+        path = tmp_path_factory.mktemp("roundtrip_datetme_coord") / "out.h5"
+        dist = random_patch.get_coord("distance")
+        dt = dc.to_datetime64(np.zeros_like(dist))
+        dt[0] = dc.to_datetime64("2017-09-17")
+        new = random_patch.update_coords(dt=("distance", dt))
+        new.io.write(path, "dasdae")
+        patch = dc.spool(path, file_format="DASDAE")[0]
+        assert isinstance(patch, dc.Patch)
+
+    def test_roundtrip_nullish_datetime_coord(self, tmp_path_factory, random_patch):
+        """Ensure a patch with an attached datetime coord with nulls works."""
+        path = tmp_path_factory.mktemp("roundtrip_datetme_coord") / "out.h5"
+        dist = random_patch.get_coord("distance")
+        dt = dc.to_datetime64(np.zeros_like(dist))
+        dt[~dt.astype(bool)] = np.datetime64("nat")
+        dt[0] = dc.to_datetime64("2017-09-17")
+        dt[-4] = dc.to_datetime64("2020-01-03")
+        new = random_patch.update_coords(dt=("distance", dt))
+        new.io.write(path, "dasdae")
+        patch = dc.spool(path, file_format="DASDAE")[0]
+        assert isinstance(patch, dc.Patch)
```

### Comparing `dascore-0.1.0/tests/test_io/test_h5simple/test_h5simple.py` & `dascore-0.1.1/tests/test_io/test_h5simple/test_h5simple.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_io/test_indexer.py` & `dascore-0.1.1/tests/test_io/test_indexer.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_io/test_io_core.py` & `dascore-0.1.1/tests/test_io/test_io_core.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_io/test_pickle/test_pickle.py` & `dascore-0.1.1/tests/test_io/test_pickle/test_pickle.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_io/test_prodml/test_prod_ml.py` & `dascore-0.1.1/tests/test_io/test_prodml/test_prod_ml.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_io/test_rsf/test_rsf.py` & `dascore-0.1.1/tests/test_io/test_rsf/test_rsf.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_io/test_sentek/test_sentek.py` & `dascore-0.1.1/tests/test_io/test_sentek/test_sentek.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_io/test_terra15/test_terra15.py` & `dascore-0.1.1/tests/test_io/test_terra15/test_terra15.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_io/test_wav/test_wav.py` & `dascore-0.1.1/tests/test_io/test_wav/test_wav.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_proc/test_aggregate.py` & `dascore-0.1.1/tests/test_proc/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_proc/test_basic.py` & `dascore-0.1.1/tests/test_proc/test_basic.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_proc/test_correlate.py` & `dascore-0.1.1/tests/test_proc/test_correlate.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_proc/test_detrend.py` & `dascore-0.1.1/tests/test_proc/test_detrend.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_proc/test_filter.py` & `dascore-0.1.1/tests/test_proc/test_filter.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_proc/test_proc_coords.py` & `dascore-0.1.1/tests/test_proc/test_proc_coords.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_proc/test_proc_units.py` & `dascore-0.1.1/tests/test_proc/test_proc_units.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,14 +60,28 @@
     def test_set_data_and_coord_units(self, random_patch):
         """Ensure we can set data and coordinate units in 1 go."""
         out = random_patch.set_units("m/s", distance="ft")
         assert isinstance(random_patch, dc.Patch)
         assert get_quantity(out.attrs.data_units) == get_quantity("m/s")
         assert get_quantity(out.attrs.distance_units) == get_quantity("ft")
 
+    def test_remove_units(self, random_patch):
+        """Ensure set coords can remove units."""
+        patch = random_patch.set_units("m", distance="m")
+        # ensure data units can be removed
+        new_none = patch.set_units(None)
+        assert new_none.attrs.data_units is None
+        new_empty_str = patch.set_units("")
+        assert new_empty_str.attrs.data_units is None
+        # ensure coord units can be removed
+        new_dist_none = random_patch.set_units(distance=None)
+        assert new_dist_none.get_coord("distance").units is None
+        new_dist_empty = random_patch.set_units(distance="")
+        assert new_dist_empty.get_coord("distance").units is None
+
 
 class TestConvertUnits:
     """Tests for converting from one unit to another."""
 
     @pytest.fixture()
     def unit_patch(self, random_patch_with_lat_lon):
         """Get a patch with units indicated."""
```

### Comparing `dascore-0.1.0/tests/test_proc/test_resample.py` & `dascore-0.1.1/tests/test_proc/test_resample.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_proc/test_rolling.py` & `dascore-0.1.1/tests/test_proc/test_rolling.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_proc/test_select.py` & `dascore-0.1.1/tests/test_proc/test_select.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_proc/test_taper.py` & `dascore-0.1.1/tests/test_proc/test_taper.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_proc/test_whiten.py` & `dascore-0.1.1/tests/test_proc/test_whiten.py`

 * *Files 6% similar despite different names*

```diff
@@ -189,7 +189,20 @@
         assert np.array_equal(
             test_patch.coords.get_array("time"), whitened_patch.coords.get_array("time")
         )
         assert np.array_equal(
             test_patch.coords.get_array("distance"),
             whitened_patch.coords.get_array("distance"),
         )
+
+    def test_whiten_ifft_false(self, test_patch):
+        """
+        Ensure whiten function can return the result in the frequency domain
+        when the ifft flag is set to True.
+        """
+        # whiten the patch and return in frequency domain
+        whitened_patch_freq_domain = test_patch.whiten(smooth_size=5, ifft=False)
+
+        # check if the returned data is in the frequency domain
+        assert np.iscomplexobj(
+            whitened_patch_freq_domain.data
+        ), "Expected the data to be complex, indicating freq. domain representation."
```

### Comparing `dascore-0.1.0/tests/test_transform/test_differentiate.py` & `dascore-0.1.1/tests/test_transform/test_differentiate.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_transform/test_dispersion.py` & `dascore-0.1.1/tests/test_transform/test_dispersion.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_transform/test_fft.py` & `dascore-0.1.1/tests/test_transform/test_fft.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_transform/test_fourier.py` & `dascore-0.1.1/tests/test_transform/test_fourier.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_transform/test_integrate.py` & `dascore-0.1.1/tests/test_transform/test_integrate.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,22 +10,34 @@
 from dascore.units import get_quantity
 from dascore.utils.misc import broadcast_for_index
 from dascore.utils.time import to_float
 
 
 @pytest.fixture(scope="session")
 def ones_patch(random_patch):
-    """Return a patch of ones with nornal axis."""
+    """Return a patch of ones with normal axis."""
     array = np.ones_like(random_patch.data)
     return random_patch.new(data=array)
 
 
 class TestIndefiniteIntegrals:
     """Tests for indefinite integrals."""
 
+    @pytest.fixture(scope="class")
+    def simple_func_patch(self, random_patch):
+        """Create a simple function patch for testing. f(x) = x + 1."""
+        time = np.arange(100) * 0.1
+        data = time[:, None] + 1
+        out = dc.Patch(
+            data=data,
+            coords={"time": time, "other": np.array([1])},
+            dims=("time", "other"),
+        )
+        return out
+
     def test_indef_integration(self, ones_patch):
         """Happy path for default time/distance integrals."""
         for dim in ones_patch.dims:
             patch = integrate(ones_patch, dim=dim, definite=False)
             ax = patch.dims.index(dim)
             # We expect slice not on axis to be the identical
             non_dim_indexer = broadcast_for_index(
@@ -54,14 +66,22 @@
             data_units2 = get_quantity(out.attrs.data_units)
             assert data_units2 == (data_units1 * get_quantity(eu))
             for dim in patch.dims:
                 coord1 = patch.get_coord(dim)
                 coord2 = patch.get_coord(dim)
                 assert coord2.units == coord1.units
 
+    def test_simple_func(self, simple_func_patch):
+        """Ensure the values are approximate correct for a simple function."""
+        out = simple_func_patch.integrate(dim="time", definite=False)
+        time = simple_func_patch.get_coord("time").values
+        expected = (time**2) / 2 + time
+        data_out = out.data.flatten()
+        assert np.allclose(expected, data_out)
+
 
 class TestDefiniteIntegration:
     """Test case for definite path integration."""
 
     def test_simple_integration(self, ones_patch):
         """Ensure simple integration works."""
         patch = ones_patch
```

### Comparing `dascore-0.1.0/tests/test_transform/test_spectro_transform.py` & `dascore-0.1.1/tests/test_transform/test_spectro_transform.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_transform/test_velocity_to_strainrate.py` & `dascore-0.1.1/tests/test_transform/test_velocity_to_strainrate.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_units.py` & `dascore-0.1.1/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_chunk.py` & `dascore-0.1.1/tests/test_utils/test_chunk.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_display.py` & `dascore-0.1.1/tests/test_utils/test_display.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_doc_utils.py` & `dascore-0.1.1/tests/test_utils/test_doc_utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_downloader.py` & `dascore-0.1.1/tests/test_utils/test_downloader.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_hdf_utils.py` & `dascore-0.1.1/tests/test_utils/test_hdf_utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_io_utils.py` & `dascore-0.1.1/tests/test_utils/test_io_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,7 +211,16 @@
 
     def test_empty_stream(self):
         """An empty Stream should return an empty Patch."""
         obspy = pytest.importorskip("obspy")
         st = obspy.Stream([])
         patch = dc.io.obspy_to_patch(st)
         assert not patch.dims
+
+    def test_example_event(self, event_patch_2):
+        """Ensure example event can be converted to stream."""
+        obspy = pytest.importorskip("obspy")
+        # make patch smaller to make test faster
+        patch = event_patch_2.select(distance=(500, 550))
+        st = patch.io.to_obspy()
+        assert isinstance(st, obspy.Stream)
+        assert len(st) == len(patch.get_coord("distance"))
```

### Comparing `dascore-0.1.0/tests/test_utils/test_mapping_utils.py` & `dascore-0.1.1/tests/test_utils/test_mapping_utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_misc.py` & `dascore-0.1.1/tests/test_utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_patch_utils.py` & `dascore-0.1.1/tests/test_utils/test_patch_utils.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_pd.py` & `dascore-0.1.1/tests/test_utils/test_pd.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_progress.py` & `dascore-0.1.1/tests/test_utils/test_progress.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_time.py` & `dascore-0.1.1/tests/test_utils/test_time.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_utils/test_transformatter.py` & `dascore-0.1.1/tests/test_utils/test_transformatter.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_viz/test_spectrogram.py` & `dascore-0.1.1/tests/test_viz/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_viz/test_waterfall.py` & `dascore-0.1.1/tests/test_viz/test_waterfall.py`

 * *Files identical despite different names*

### Comparing `dascore-0.1.0/tests/test_viz/test_wiggle.py` & `dascore-0.1.1/tests/test_viz/test_wiggle.py`

 * *Files identical despite different names*

