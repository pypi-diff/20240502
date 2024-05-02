# Comparing `tmp/sharrow-2.8.2.tar.gz` & `tmp/sharrow-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharrow-2.8.2.tar", last modified: Thu Mar 28 14:35:43 2024, max compression
+gzip compressed data, was "sharrow-2.8.3.tar", last modified: Thu May  2 17:16:10 2024, max compression
```

## Comparing `sharrow-2.8.2.tar` & `sharrow-2.8.3.tar`

### file list

```diff
@@ -1,796 +1,796 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.237575 sharrow-2.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.113573 sharrow-2.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.137574 sharrow-2.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-03-28 14:34:06.000000 sharrow-2.8.2/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-28 14:34:06.000000 sharrow-2.8.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.137574 sharrow-2.8.2/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-28 14:34:06.000000 sharrow-2.8.2/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-28 14:34:06.000000 sharrow-2.8.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-28 14:34:06.000000 sharrow-2.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-28 14:35:43.237575 sharrow-2.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-28 14:34:06.000000 sharrow-2.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.137574 sharrow-2.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.137574 sharrow-2.8.2/docs/_script/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/_script/hide_test_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/_script/run_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/_script/update_version_number.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.137574 sharrow-2.8.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    10218 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/_static/ampo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/_static/sharrow-docs.css
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.141574 sharrow-2.8.2/docs/walkthrough/
--rw-r--r--   0 runner    (1001) docker     (127)    27222 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/walkthrough/encoding.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/walkthrough/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    46780 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/walkthrough/one-dim.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/walkthrough/sparse.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30440 2024-03-28 14:34:06.000000 sharrow-2.8.2/docs/walkthrough/two-dim.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.141574 sharrow-2.8.2/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-28 14:34:06.000000 sharrow-2.8.2/envs/development.yml
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-28 14:34:06.000000 sharrow-2.8.2/envs/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-28 14:34:06.000000 sharrow-2.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 14:35:43.237575 sharrow-2.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.145574 sharrow-2.8.2/sharrow/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/_infer_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-28 14:35:42.000000 sharrow-2.8.2/sharrow/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/accessors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    44465 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/aster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/categorical.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    48525 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    18435 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/digital_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.145574 sharrow-2.8.2/sharrow/example_data/
--rw-r--r--   0 runner    (1001) docker     (127)   106776 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/households.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/land_use.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/maz_to_maz_walk.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/maz_to_taz.csv
--rw-r--r--   0 runner    (1001) docker     (127)    84654 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/persons.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)  3674745 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.omx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.149574 sharrow-2.8.2/sharrow/example_data/skims.zarr/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.149574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DIST/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DIST/0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.153574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DISTBIKE/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DISTBIKE/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DISTBIKE/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DISTBIKE/0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.153574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DISTWALK/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DISTWALK/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DISTWALK/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DISTWALK/0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.153574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.153574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.153574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.153574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.153574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.153574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.157574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.157574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.157574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.157574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.157574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.157574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.157574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.157574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.157574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.161574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.161574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.161574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.161574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.161574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.161574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.161574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.161574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.165574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.165574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.165574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.165574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.165574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.165574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.165574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.165574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.165574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.169574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.169574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.169574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.169574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.169574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.169574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.169574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.169574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.173574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.173574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.173574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.173574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.173574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.173574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.173574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.173574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.173574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.177574 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.177574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.177574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.177574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.177574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.177574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.177574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_DIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.177574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_TIME/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.177574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.181574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.181574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.181574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.181574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.181574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_DIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.181574 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_TIME/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.181574 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.181574 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_DIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.181574 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_TIME/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.185574 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.185574 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_BTOLL/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_BTOLL/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_BTOLL/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_BTOLL/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.185574 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_DIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_DIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_DIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_DIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.185574 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_TIME/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_TIME/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_TIME/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_TIME/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.185574 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.185574 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.185574 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.185574 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.185574 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.189575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.189575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.189575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.189575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.189575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.189575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.189575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.189575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.189575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.193575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.193575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.193575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.193575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.193575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.193575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.193575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.193575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.197575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.197575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.197575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.197575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.197575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.197575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.197575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.197575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.197575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.201575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.201575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.201575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.201575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.201575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.201575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.201575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.201575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.205575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.205575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.205575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.205575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.205575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.205575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.205575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.205575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.209575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.209575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.209575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.209575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.209575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.209575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.209575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.209575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.209575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.213575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.213575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.213575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.213575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.213575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.213575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.213575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.213575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.217575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.217575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.217575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.217575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.217575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.217575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.217575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.217575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.217575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.221575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.221575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.221575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.221575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.221575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.221575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.221575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.221575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.225575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.225575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.225575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.225575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.225575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.225575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.225575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.225575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.229575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.229575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.229575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.229575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.229575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.229575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.229575 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/0.0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.229575 sharrow-2.8.2/sharrow/example_data/skims.zarr/dtaz/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/dtaz/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/dtaz/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/dtaz/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.233575 sharrow-2.8.2/sharrow/example_data/skims.zarr/otaz/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/otaz/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/otaz/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/otaz/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.233575 sharrow-2.8.2/sharrow/example_data/skims.zarr/time_period/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/time_period/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/time_period/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data/skims.zarr/time_period/0
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/filewrite.py
--rw-r--r--   0 runner    (1001) docker     (127)   112398 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/nested_logit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/omx.py
--rw-r--r--   0 runner    (1001) docker     (127)    59424 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17890 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.233575 sharrow-2.8.2/sharrow/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/test_categorical.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/test_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/test_nesting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.237575 sharrow-2.8.2/sharrow/tests/test_relationships/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_dict_encoded.csv
--rw-r--r--   0 runner    (1001) docker     (127)   375022 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_get.csv
--rw-r--r--   0 runner    (1001) docker     (127)    80926 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_isin.csv
--rw-r--r--   0 runner    (1001) docker     (127)   138552 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_isin_and_between.csv
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_joint_dict_encoded.csv
--rw-r--r--   0 runner    (1001) docker     (127)   213333 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_mixed_dtypes.csv
--rw-r--r--   0 runner    (1001) docker     (127)   185444 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_nested_where.csv
--rw-r--r--   0 runner    (1001) docker     (127)   243898 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_shared_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)   240111 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_shared_data_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   335532 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_shared_data_reversible.csv
--rw-r--r--   0 runner    (1001) docker     (127)   141376 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_tuple_slice.csv
--rw-r--r--   0 runner    (1001) docker     (127)   164893 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/tests/test_relationships/test_with_2d_base.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33515 2024-03-28 14:34:06.000000 sharrow-2.8.2/sharrow/tests/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.237575 sharrow-2.8.2/sharrow/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/utils/tar_zst.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/viz.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-03-28 14:34:07.000000 sharrow-2.8.2/sharrow/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:35:43.237575 sharrow-2.8.2/sharrow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-28 14:35:42.000000 sharrow-2.8.2/sharrow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    31599 2024-03-28 14:35:43.000000 sharrow-2.8.2/sharrow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:35:42.000000 sharrow-2.8.2/sharrow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-28 14:35:42.000000 sharrow-2.8.2/sharrow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 14:35:42.000000 sharrow-2.8.2/sharrow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.104096 sharrow-2.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:09.984097 sharrow-2.8.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.004097 sharrow-2.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-02 17:14:31.000000 sharrow-2.8.3/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-02 17:14:31.000000 sharrow-2.8.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.004097 sharrow-2.8.3/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 17:14:31.000000 sharrow-2.8.3/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-02 17:14:31.000000 sharrow-2.8.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-02 17:14:31.000000 sharrow-2.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-02 17:16:10.104096 sharrow-2.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-02 17:14:31.000000 sharrow-2.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.004097 sharrow-2.8.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.004097 sharrow-2.8.3/docs/_script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/_script/hide_test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/_script/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/_script/update_version_number.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.004097 sharrow-2.8.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    10218 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/_static/ampo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/_static/sharrow-docs.css
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.008097 sharrow-2.8.3/docs/walkthrough/
+-rw-r--r--   0 runner    (1001) docker     (127)    27222 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/walkthrough/encoding.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/walkthrough/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    46780 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/walkthrough/one-dim.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/walkthrough/sparse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30440 2024-05-02 17:14:31.000000 sharrow-2.8.3/docs/walkthrough/two-dim.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.008097 sharrow-2.8.3/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-02 17:14:31.000000 sharrow-2.8.3/envs/development.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-02 17:14:31.000000 sharrow-2.8.3/envs/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-02 17:14:31.000000 sharrow-2.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:16:10.104096 sharrow-2.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.012097 sharrow-2.8.3/sharrow/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/_infer_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 17:16:09.000000 sharrow-2.8.3/sharrow/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/accessors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45746 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/aster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/categorical.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48525 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18435 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/digital_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.012097 sharrow-2.8.3/sharrow/example_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   106776 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/example_data/households.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/example_data/land_use.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/example_data/maz_to_maz_walk.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/example_data/maz_to_taz.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    84654 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/example_data/persons.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  3674745 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.omx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.016097 sharrow-2.8.3/sharrow/example_data/skims.zarr/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.016097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DIST/0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.020097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DISTBIKE/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DISTBIKE/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DISTBIKE/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DISTBIKE/0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.020097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DISTWALK/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DISTWALK/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DISTWALK/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DISTWALK/0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.020097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.020097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.020097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.020097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.020097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.020097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.024097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.024097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.024097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.024097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.024097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.024097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.024097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.024097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.028097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.028097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.028097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.028097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.028097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.028097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.028097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.028097 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.032096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.032096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.032096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.032096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.032096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.032096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.032096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.032096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.036096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.036096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.036096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.036096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.036096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.036096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.036096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.036096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.040096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.040096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.040096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.040096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.040096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.040096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FERRYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.040096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.040096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.040096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.044096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.044096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.044096 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.044096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.044096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.044096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.044096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_VTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.044096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.048096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_DIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.048096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_TIME/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.048096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.048096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.048096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.048096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_VTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.048096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.052096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_DIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.052096 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_TIME/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.052096 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.052096 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_DIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.052096 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_TIME/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.052096 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_VTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.052096 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_BTOLL/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_BTOLL/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_BTOLL/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_BTOLL/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.052096 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_DIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_DIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_DIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_DIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.056096 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_TIME/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_TIME/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_TIME/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_TIME/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.056096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.056096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.056096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.056096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.056096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.056096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.056096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.060096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.060096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.060096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.060096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.060096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.060096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.060096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.060096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.064096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.064096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.064096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.064096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.064096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.064096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.064096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.064096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.068096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.068096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.068096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.068096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.068096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.068096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.068096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.068096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.068096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.068096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.072096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.072096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.072096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.072096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.072096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.072096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.072096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.072096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.072096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.076096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.076096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.076096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.076096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.076096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.076096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.076096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.076096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.076096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.080096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.080096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.080096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.080096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.080096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.080096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.080096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.080096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.080096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.080096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.084096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.084096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.084096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.084096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.084096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.084096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.084096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.084096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.084096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.088096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.088096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.088096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.088096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.088096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_FERRYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.088096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.088096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.088096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.088096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.088096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.092096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.092096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.092096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.092096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FERRYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.092096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.092096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.092096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.092096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.096096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.096096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.096096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.096096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.096096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.096096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WAUX/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.096096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.096096 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/0.0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.096096 sharrow-2.8.3/sharrow/example_data/skims.zarr/dtaz/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/dtaz/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/dtaz/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/dtaz/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.096096 sharrow-2.8.3/sharrow/example_data/skims.zarr/otaz/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/otaz/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/otaz/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/otaz/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.100096 sharrow-2.8.3/sharrow/example_data/skims.zarr/time_period/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/time_period/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/time_period/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/example_data/skims.zarr/time_period/0
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-02 17:14:31.000000 sharrow-2.8.3/sharrow/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/filewrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112398 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/nested_logit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/omx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59424 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19133 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.100096 sharrow-2.8.3/sharrow/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_nesting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.104096 sharrow-2.8.3/sharrow/tests/test_relationships/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_dict_encoded.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   375022 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_get.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    80926 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_isin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   138552 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_isin_and_between.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_joint_dict_encoded.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   213333 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_mixed_dtypes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   185444 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_nested_where.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   243898 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_shared_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   240111 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_shared_data_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   335532 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_shared_data_reversible.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   141376 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_tuple_slice.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   164893 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships/test_with_2d_base.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33515 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/tests/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.104096 sharrow-2.8.3/sharrow/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/utils/tar_zst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-02 17:14:32.000000 sharrow-2.8.3/sharrow/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:16:10.104096 sharrow-2.8.3/sharrow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-02 17:16:09.000000 sharrow-2.8.3/sharrow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    31599 2024-05-02 17:16:09.000000 sharrow-2.8.3/sharrow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:16:09.000000 sharrow-2.8.3/sharrow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 17:16:09.000000 sharrow-2.8.3/sharrow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 17:16:09.000000 sharrow-2.8.3/sharrow.egg-info/top_level.txt
```

### Comparing `sharrow-2.8.2/.github/workflows/run-tests.yml` & `sharrow-2.8.3/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/.gitignore` & `sharrow-2.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/.pre-commit-config.yaml` & `sharrow-2.8.3/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 repos:
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: check-yaml
   - id: end-of-file-fixer
     exclude: .*\.ipynb
   - id: trailing-whitespace
 
 - repo: https://github.com/kynan/nbstripout
   rev: 0.7.1
   hooks:
     - id: nbstripout
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
-  rev: v0.3.4
+  rev: v0.4.2
   hooks:
     # Run the linter.
     - id: ruff
       types_or: [ python, pyi, jupyter ]
       args: [ --fix ]
     # Run the formatter.
     - id: ruff-format
```

### Comparing `sharrow-2.8.2/LICENSE` & `sharrow-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/PKG-INFO` & `sharrow-2.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharrow
-Version: 2.8.2
+Version: 2.8.3
 Summary: numba for ActivitySim-style spec files
 Project-URL: Documentation, https://activitysim.github.io/sharrow/
 Project-URL: Repository, https://github.com/activitysim/sharrow
 Keywords: activitysim,discrete choice
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sharrow-2.8.2/README.md` & `sharrow-2.8.3/README.md`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/_config.yml` & `sharrow-2.8.3/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/_script/hide_test_cells.py` & `sharrow-2.8.3/docs/_script/hide_test_cells.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/_static/ampo.png` & `sharrow-2.8.3/docs/_static/ampo.png`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/_static/favicon.png` & `sharrow-2.8.3/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/api.rst` & `sharrow-2.8.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/index.md` & `sharrow-2.8.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/intro.md` & `sharrow-2.8.3/docs/intro.md`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/logo.png` & `sharrow-2.8.3/docs/logo.png`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/walkthrough/encoding.ipynb` & `sharrow-2.8.3/docs/walkthrough/encoding.ipynb`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/walkthrough/one-dim.ipynb` & `sharrow-2.8.3/docs/walkthrough/one-dim.ipynb`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/walkthrough/sparse.ipynb` & `sharrow-2.8.3/docs/walkthrough/sparse.ipynb`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/docs/walkthrough/two-dim.ipynb` & `sharrow-2.8.3/docs/walkthrough/two-dim.ipynb`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/pyproject.toml` & `sharrow-2.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/__init__.py` & `sharrow-2.8.3/sharrow/__init__.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/accessors.py` & `sharrow-2.8.3/sharrow/accessors.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/aster.py` & `sharrow-2.8.3/sharrow/aster.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,15 +404,17 @@
         pref_topname = self.preferred_spacename or topname
 
         if self.spacevars is not None:
             if attr not in self.spacevars:
                 if self.get_default or (
                     topname == pref_topname and not self.swallow_errors
                 ):
-                    raise KeyError(f"{topname}..{attr}")
+                    raise KeyError(
+                        f"{topname}..{attr}\nexpression={self.original_expr}"
+                    )
                 # we originally raised a KeyError here regardless, but what if
                 # we just give back the original node, and see if other spaces,
                 # possibly fallback spaces, might work?  If nothing works then
                 # it will still eventually error out when compiling?
                 # The swallow errors option allows us to continue processing
                 # using the same rules, then circle back later to clean up
                 # errors, so that as-yet unprocessed Ast elements get the
@@ -1006,14 +1008,24 @@
                         warnings.warn(
                             f"right hand value {right.value!r} not found in "
                             f"categories for {left_varname} in {self.spacename}"
                             f"\nexpression: {self.original_expr}"
                             f"\ncategories: {left_dictionary}",
                             stacklevel=2,
                         )
+                        # at this point, the right value is not in the left's categories, so
+                        # it is guaranteed to be not equal to any of the categories.
+                        if isinstance(node.ops[0], ast.Eq):
+                            result = ast.Constant(False)
+                        elif isinstance(node.ops[0], ast.NotEq):
+                            result = ast.Constant(True)
+                        else:
+                            raise ValueError(
+                                f"unexpected operator {node.ops[0]}"
+                            ) from None
                     if right_decoded is not None:
                         result = ast.Compare(
                             left=left.slice,
                             ops=[self.visit(i) for i in node.ops],
                             comparators=[ast_Constant(right_decoded)],
                         )
             right_is_categorical = (
@@ -1039,14 +1051,24 @@
                         warnings.warn(
                             f"left hand value {left.value!r} not found in "
                             f"categories for {right_varname} in {self.spacename}"
                             f"\nexpression: {self.original_expr}"
                             f"\ncategories: {right_dictionary}",
                             stacklevel=2,
                         )
+                        # at this point, the left value is not in the right's categories, so
+                        # it is guaranteed to be not equal to any of the categories.
+                        if isinstance(node.ops[0], ast.Eq):
+                            result = ast.Constant(False)
+                        elif isinstance(node.ops[0], ast.NotEq):
+                            result = ast.Constant(True)
+                        else:
+                            raise ValueError(
+                                f"unexpected operator {node.ops[0]}"
+                            ) from None
                     if left_decoded is not None:
                         result = ast.Compare(
                             left=ast_Constant(left_decoded),
                             ops=[self.visit(i) for i in node.ops],
                             comparators=[right.slice],
                         )
```

### Comparing `sharrow-2.8.2/sharrow/categorical.py` & `sharrow-2.8.3/sharrow/categorical.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/dataset.py` & `sharrow-2.8.3/sharrow/dataset.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/datastore.py` & `sharrow-2.8.3/sharrow/datastore.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/digital_encoding.py` & `sharrow-2.8.3/sharrow/digital_encoding.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/households.csv.gz` & `sharrow-2.8.3/sharrow/example_data/households.csv.gz`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/land_use.csv.gz` & `sharrow-2.8.3/sharrow/example_data/land_use.csv.gz`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/maz_to_taz.csv` & `sharrow-2.8.3/sharrow/example_data/maz_to_taz.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/persons.csv.gz` & `sharrow-2.8.3/sharrow/example_data/persons.csv.gz`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.omx` & `sharrow-2.8.3/sharrow/example_data/skims.omx`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DIST/0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DIST/0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DISTBIKE/0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DISTBIKE/0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DISTWALK/0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DISTWALK/0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_WAUX/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_COM_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_EXP_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_HVY_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LOC_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/DRV_LRF_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2TOLL_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_BTOLL/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_DIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV2_TIME/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV2_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3TOLL_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_BTOLL/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_DIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/HOV3_TIME/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/HOV3_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_DIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/SOVTOLL_TIME/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/SOVTOLL_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_BTOLL/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_BTOLL/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_DIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_DIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/SOV_TIME/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/SOV_TIME/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_DRV_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_COM_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_DRV_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_EXP_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_DRV_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_HVY_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_DRV_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LOC_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DDIST/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_DTIM/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_DRV_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_BOARDS/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_FAR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_KEYIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_TOTIVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_WAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_LRF_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IVT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_IWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WACC/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_WEGR/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/0.0.0` & `sharrow-2.8.3/sharrow/example_data/skims.zarr/WLK_TRN_WLK_XWAIT/0.0.0`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/example_data.py` & `sharrow-2.8.3/sharrow/example_data.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/filewrite.py` & `sharrow-2.8.3/sharrow/filewrite.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/flows.py` & `sharrow-2.8.3/sharrow/flows.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/logging.py` & `sharrow-2.8.3/sharrow/logging.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/maths.py` & `sharrow-2.8.3/sharrow/maths.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/nested_logit.py` & `sharrow-2.8.3/sharrow/nested_logit.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/omx.py` & `sharrow-2.8.3/sharrow/omx.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/relationships.py` & `sharrow-2.8.3/sharrow/relationships.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/selectors.py` & `sharrow-2.8.3/sharrow/selectors.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/shared_memory.py` & `sharrow-2.8.3/sharrow/shared_memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import atexit
 import hashlib
 import logging
 import os
 import pickle
+import time
 
 import dask
 import dask.array as da
 import numpy as np
 import xarray as xr
 
 try:
@@ -243,32 +244,38 @@
         """Release shared memory allocated to this Dataset."""
         release_shared_memory(self._shared_memory_key_)
 
     @staticmethod
     def delete_shared_memory_files(key):
         delete_shared_memory_files(key)
 
-    def to_shared_memory(self, key=None, mode="r+", _dupe=True):
+    def to_shared_memory(
+        self, key=None, mode="r+", _dupe=True, dask_scheduler="threads"
+    ):
         """
         Load this Dataset into shared memory.
 
         The returned Dataset object references the shared memory and is the
         "owner" of this data.  When this object is destroyed, the data backing
         it may also be freed, which can result in a segfault or other unfortunate
         condition if that memory is still accessed from elsewhere.
 
         Parameters
         ----------
         key : str
             An identifying key for this shared memory.  Use the same key
             in `from_shared_memory` to recreate this Dataset elsewhere.
         mode : {‘r+’, ‘r’, ‘w+’, ‘c’}, optional
-            This methid returns a copy of the Dataset in shared memory.
+            This method returns a copy of the Dataset in shared memory.
             If memmapped, that copy can be opened in various modes.
             See numpy.memmap() for details.
+        dask_scheduler : str, default 'threads'
+            The scheduler to use when loading dask arrays into shared memory.
+            Typically "threads" for multi-threaded reads or "synchronous"
+            for single-threaded reads. See dask.compute() for details.
 
         Returns
         -------
         Dataset
         """
         logger.info(f"sharrow.Dataset.to_shared_memory({key})")
         if key is None:
@@ -283,14 +290,15 @@
         sizes = []
         names = []
         position = 0
 
         def emit(k, a, is_coord):
             nonlocal names, wrappers, sizes, position
             if sparse is not None and isinstance(a.data, sparse.GCXS):
+                logger.info(f"preparing sparse array {a.name}")
                 wrappers.append(
                     {
                         "sparse": True,
                         "dims": a.dims,
                         "name": a.name,
                         "attrs": a.attrs,
                         "dtype": a.dtype,
@@ -304,14 +312,15 @@
                         "data.dtype": a.data.data.dtype,
                         "indices.dtype": a.data.indices.dtype,
                         "indptr.dtype": a.data.indptr.dtype,
                     }
                 )
                 a_nbytes = a.data.nbytes
             else:
+                logger.info(f"preparing dense array {a.name}")
                 wrappers.append(
                     {
                         "dims": a.dims,
                         "name": a.name,
                         "attrs": a.attrs,
                         "dtype": a.dtype,
                         "shape": a.shape,
@@ -331,27 +340,31 @@
         for k in self._obj.variables:
             if k in names:
                 continue
             a = self._obj[k]
             emit(k, a, False)
 
         mem = create_shared_memory_array(key, size=position)
+
+        logger.info("declaring shared memory buffer")
         if key.startswith("memmap:"):
             buffer = memoryview(mem)
         else:
             buffer = mem.buf
 
         tasks = []
+        task_names = []
         for w in wrappers:
             _is_sparse = w.get("sparse", False)
             _size = w["nbytes"]
             _name = w["name"]
             _pos = w["position"]
             a = self._obj[_name]
             if _is_sparse:
+                logger.info(f"running load task: {_name} ({si_units(_size)})")
                 ad = a.data
                 _size_d = w["data.nbytes"]
                 _size_i = w["indices.nbytes"]
                 _size_p = w["indptr.nbytes"]
                 mem_arr_d = np.ndarray(
                     shape=(_size_d // ad.data.dtype.itemsize,),
                     dtype=ad.data.dtype,
@@ -369,27 +382,38 @@
                         _pos + _size_d + _size_i : _pos + _size_d + _size_i + _size_p
                     ],
                 )
                 mem_arr_d[:] = ad.data[:]
                 mem_arr_i[:] = ad.indices[:]
                 mem_arr_p[:] = ad.indptr[:]
             else:
+                logger.info(f"preparing load task: {_name} ({si_units(_size)})")
                 mem_arr = np.ndarray(
                     shape=a.shape, dtype=a.dtype, buffer=buffer[_pos : _pos + _size]
                 )
                 if isinstance(a, xr.DataArray) and isinstance(a.data, da.Array):
                     tasks.append(da.store(a.data, mem_arr, lock=False, compute=False))
+                    task_names.append(_name)
                 else:
                     mem_arr[:] = a[:]
         if tasks:
-            dask.compute(tasks, scheduler="threads")
+            t = time.time()
+            logger.info(f"running {len(tasks)} dask data load tasks")
+            if dask_scheduler == "synchronous":
+                for task, task_name in zip(tasks, task_names):
+                    logger.info(f"running load task: {task_name}")
+                    dask.compute(task, scheduler=dask_scheduler)
+            else:
+                dask.compute(tasks, scheduler=dask_scheduler)
+            logger.info(f"completed dask data load in {time.time()-t:.3f} seconds")
 
         if key.startswith("memmap:"):
             mem.flush()
 
+        logger.info("storing metadata in shared memory")
         create_shared_list(
             [pickle.dumps(self._obj.attrs)] + [pickle.dumps(i) for i in wrappers], key
         )
         return type(self).from_shared_memory(key, own_data=mem, mode=mode)
 
     @property
     def shared_memory_key(self):
```

### Comparing `sharrow-2.8.2/sharrow/sparse.py` & `sharrow-2.8.3/sharrow/sparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             i_ = i
             j_ = j
 
         if sparse is None:
             raise ImportError("sparse is not installed")
 
         sparse_data = sparse.GCXS(
-            sparse.COO((i_, j_), data, shape=shape), compressed_axes=(0,)
+            sparse.COO(np.stack((i_, j_)), data, shape=shape), compressed_axes=(0,)
         )
         self._obj[f"_s_{name}"] = xr.DataArray(
             sparse_data,
             dims=(i_dim, j_dim),
         )
         if not max_blend_distance:
             max_blend_distance = np.inf
```

### Comparing `sharrow-2.8.2/sharrow/table.py` & `sharrow-2.8.3/sharrow/table.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/conftest.py` & `sharrow-2.8.3/sharrow/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_categorical.py` & `sharrow-2.8.3/sharrow/tests/test_categorical.py`

 * *Files 17% similar despite different names*

```diff
@@ -173,14 +173,56 @@
 
     expr = "df.TourMode2 != 'Bus'"
     f7 = tree.setup_flow({expr: expr}, with_root_node_name="df")
     a = f7.load_dataarray(dtype=np.int8)
     a = a.isel(expressions=0)
     assert all(a == np.asarray([1, 0, 1, 1, 1, 1]))
 
+    expr = "df.TourMode2 != 'BAD'"
+    with pytest.warns(UserWarning):
+        f8 = tree.setup_flow({expr: expr}, with_root_node_name="df")
+    a = f8.load_dataarray(dtype=np.int8)
+    a = a.isel(expressions=0)
+    assert all(a == np.asarray([1, 1, 1, 1, 1, 1]))
+
+    expr = "'BAD' != df.TourMode2"
+    with pytest.warns(UserWarning):
+        f9 = tree.setup_flow({expr: expr}, with_root_node_name="df")
+    a = f9.load_dataarray(dtype=np.int8)
+    a = a.isel(expressions=0)
+    assert all(a == np.asarray([1, 1, 1, 1, 1, 1]))
+
+    expr = "(df.TourMode2 == 'BAD') * 2"
+    with pytest.warns(UserWarning):
+        fA = tree.setup_flow({expr: expr}, with_root_node_name="df")
+    a = fA.load_dataarray(dtype=np.int8)
+    a = a.isel(expressions=0)
+    assert all(a == np.asarray([0, 0, 0, 0, 0, 0]))
+
+    expr = "(df.TourMode2 == 'BAD') * 2.2"
+    with pytest.warns(UserWarning):
+        fB = tree.setup_flow({expr: expr}, with_root_node_name="df")
+    a = fB.load_dataarray(dtype=np.int8)
+    a = a.isel(expressions=0)
+    assert all(a == np.asarray([0, 0, 0, 0, 0, 0]))
+
+    expr = "np.exp(df.TourMode2 == 'BAD') * 2.2"
+    with pytest.warns(UserWarning):
+        fC = tree.setup_flow({expr: expr}, with_root_node_name="df")
+    a = fC.load_dataarray(dtype=np.float32)
+    a = a.isel(expressions=0)
+    assert all(a == np.asarray([2.2, 2.2, 2.2, 2.2, 2.2, 2.2], dtype=np.float32))
+
+    expr = "(df.TourMode2 != 'BAD') * 2"
+    with pytest.warns(UserWarning):
+        fD = tree.setup_flow({expr: expr}, with_root_node_name="df")
+    a = fD.load_dataarray(dtype=np.int8)
+    a = a.isel(expressions=0)
+    assert all(a == np.asarray([2, 2, 2, 2, 2, 2]))
+
 
 def test_categorical_indexing(tours_dataset: xr.Dataset, skims_dataset: xr.Dataset):
     tree = sharrow.DataTree(tours=tours_dataset)
     tree.add_dataset(
         "od_skims",
         skims_dataset,
         [
```

### Comparing `sharrow-2.8.2/sharrow/tests/test_datasets.py` & `sharrow-2.8.3/sharrow/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_datastore.py` & `sharrow-2.8.3/sharrow/tests/test_datastore.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_nesting.py` & `sharrow-2.8.3/sharrow/tests/test_nesting.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships/test_get.csv` & `sharrow-2.8.3/sharrow/tests/test_relationships/test_get.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships/test_isin.csv` & `sharrow-2.8.3/sharrow/tests/test_relationships/test_isin.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships/test_isin_and_between.csv` & `sharrow-2.8.3/sharrow/tests/test_relationships/test_isin_and_between.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships/test_joint_dict_encoded.csv` & `sharrow-2.8.3/sharrow/tests/test_relationships/test_joint_dict_encoded.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships/test_mixed_dtypes.csv` & `sharrow-2.8.3/sharrow/tests/test_relationships/test_mixed_dtypes.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships/test_nested_where.csv` & `sharrow-2.8.3/sharrow/tests/test_relationships/test_nested_where.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships/test_shared_data.csv` & `sharrow-2.8.3/sharrow/tests/test_relationships/test_shared_data.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships/test_shared_data_2.csv` & `sharrow-2.8.3/sharrow/tests/test_relationships/test_shared_data_2.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships/test_shared_data_reversible.csv` & `sharrow-2.8.3/sharrow/tests/test_relationships/test_shared_data_reversible.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships/test_tuple_slice.csv` & `sharrow-2.8.3/sharrow/tests/test_relationships/test_tuple_slice.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships/test_with_2d_base.csv` & `sharrow-2.8.3/sharrow/tests/test_relationships/test_with_2d_base.csv`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/tests/test_relationships.py` & `sharrow-2.8.3/sharrow/tests/test_relationships.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/translate.py` & `sharrow-2.8.3/sharrow/translate.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/utils/tar_zst.py` & `sharrow-2.8.3/sharrow/utils/tar_zst.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/viz.py` & `sharrow-2.8.3/sharrow/viz.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow/wrappers.py` & `sharrow-2.8.3/sharrow/wrappers.py`

 * *Files identical despite different names*

### Comparing `sharrow-2.8.2/sharrow.egg-info/PKG-INFO` & `sharrow-2.8.3/sharrow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharrow
-Version: 2.8.2
+Version: 2.8.3
 Summary: numba for ActivitySim-style spec files
 Project-URL: Documentation, https://activitysim.github.io/sharrow/
 Project-URL: Repository, https://github.com/activitysim/sharrow
 Keywords: activitysim,discrete choice
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sharrow-2.8.2/sharrow.egg-info/SOURCES.txt` & `sharrow-2.8.3/sharrow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

