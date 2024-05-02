# Comparing `tmp/niche_vlaanderen-1.2b2.linux-x86_64.tar.gz` & `tmp/niche_vlaanderen-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niche_vlaanderen-1.2b2.linux-x86_64.tar", last modified: Mon Jan 30 14:40:36 2023, max compression
+gzip compressed data, was "niche_vlaanderen-1.3.tar", last modified: Thu May  2 15:22:04 2024, max compression
```

## Comparing `niche_vlaanderen-1.2b2.linux-x86_64.tar` & `niche_vlaanderen-1.3.tar`

### file list

```diff
@@ -1,61 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.308636 ./
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.308636 ./usr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.352636 ./usr/local/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.352636 ./usr/local/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-01-30 14:40:36.352636 ./usr/local/bin/niche
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.308636 ./usr/local/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.308636 ./usr/local/lib/python3.10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.332636 ./usr/local/lib/python3.10/dist-packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.316636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.332636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-01-30 14:40:36.320636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-01-30 14:40:36.332636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/acidity.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-01-30 14:40:36.316636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-01-30 14:40:36.328636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/codetables.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-30 14:40:36.316636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/exception.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-01-30 14:40:36.316636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/flooding.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    31610 2023-01-30 14:40:36.328636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/niche.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-01-30 14:40:36.328636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/nutrient_level.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-01-30 14:40:36.328636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/spatial_context.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-01-30 14:40:36.316636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/validation.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-01-30 14:40:36.320636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/vegetation.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-30 14:40:36.316636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/__pycache__/version.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/acidity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/codetables.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/flooding.py
--rw-r--r--   0 runner    (1001) docker     (123)    45902 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/niche.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/nutrient_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/spatial_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.312636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/acidity.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/example.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.312636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/flooding/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/flooding/depths.csv
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/flooding/duration.csv
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/flooding/frequency.csv
--rw-r--r--   0 runner    (1001) docker     (123)    22371 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/flooding/lnk_potential.csv
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/flooding/potential.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/hab_niche_join.csv
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/inundation.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/lnk_acidity.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/lnk_soil_nutrient_level.csv
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/management.csv
--rw-r--r--   0 runner    (1001) docker     (123)    58661 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/niche_vegetation.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/nitrogen_mineralisation.csv
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/nutrient_level.csv
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/seepage.csv
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/soil_codes.csv
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/soil_mlw_class.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/vegetation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-30 14:38:46.000000 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:40:36.332636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen-1.2b2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-01-30 14:40:36.292636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen-1.2b2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-01-30 14:40:36.304636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen-1.2b2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 14:40:36.292636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen-1.2b2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-30 14:40:36.292636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen-1.2b2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-30 14:40:36.292636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen-1.2b2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-30 14:40:36.292636 ./usr/local/lib/python3.10/dist-packages/niche_vlaanderen-1.2b2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.493317 niche_vlaanderen-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-02 15:22:04.493317 niche_vlaanderen-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.473316 niche_vlaanderen-1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.469316 niche_vlaanderen-1.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.477316 niche_vlaanderen-1.3/docs/_static/png/
+-rw-r--r--   0 runner    (1001) docker     (127)    28786 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/acidity_principle.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20430 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/acidity_table.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/advanced_properties.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/advanced_properties2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79694 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/bwk_overlay.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15434 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/environment_variables.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71908 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/exception.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37480 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/input_rasters.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/new_environment_variable.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29941 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/niche_principle.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34756 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/nutrient_classes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41222 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/nutrient_mineralcurve.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43532 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/nutrient_principle.png
+-rw-r--r--   0 runner    (1001) docker     (127)    67367 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/system_properties.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/_static/png/warning.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/codetables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    46047 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/invoer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/lowlevel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/notendop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/overstroming.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/principe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/running.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/trofie.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/validatie.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9172 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/vegetatie.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/vegetatie_reftabel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/vegetatietype.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/docs/zuur.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.477316 niche_vlaanderen-1.3/niche_vlaanderen/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/acidity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/codetables.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/flooding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46902 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/niche.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/nutrient_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/spatial_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.481316 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/acidity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/example.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.481316 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/flooding/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/flooding/depths.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/flooding/duration.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/flooding/frequency.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    22371 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/flooding/lnk_potential.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/flooding/potential.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/hab_niche_join.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/inundation.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/lnk_acidity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/lnk_soil_nutrient_level.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/management.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    58661 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/niche_vegetation.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/nitrogen_mineralisation.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/nutrient_level.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/seepage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/soil_codes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/system_tables/soil_mlw_class.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12460 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/vegetation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/niche_vlaanderen/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.477316 niche_vlaanderen-1.3/niche_vlaanderen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-02 15:22:04.000000 niche_vlaanderen-1.3/niche_vlaanderen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-02 15:22:04.000000 niche_vlaanderen-1.3/niche_vlaanderen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:22:04.000000 niche_vlaanderen-1.3/niche_vlaanderen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 15:22:04.000000 niche_vlaanderen-1.3/niche_vlaanderen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 15:22:04.000000 niche_vlaanderen-1.3/niche_vlaanderen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 15:22:04.000000 niche_vlaanderen-1.3/niche_vlaanderen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-02 15:22:04.493317 niche_vlaanderen-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.485316 niche_vlaanderen-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-02 15:19:19.000000 niche_vlaanderen-1.3/tests/_example.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.469316 niche_vlaanderen-1.3/tests/baseline_images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.485316 niche_vlaanderen-1.3/tests/baseline_images/test_niche/
+-rw-r--r--   0 runner    (1001) docker     (127)    22292 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/baseline_images/test_niche/zwb12.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    57123 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/baseline_images/test_niche/zwb12_full_legend.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.485316 niche_vlaanderen-1.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.485316 niche_vlaanderen-1.3/tests/data/bad_ct/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bad_ct/acidity_limited.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bad_ct/bad_boundaries.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bad_ct/bad_vegetation.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bad_ct/differentmlw.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bad_ct/lnk_acidity_limited.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    22371 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bad_ct/lnk_potential.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bad_ct/nutrient_level.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bad_ct/one_vegetation.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bad_ct/one_vegetation_limited.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bad_ct/vegetation_noinnerjoin.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.489316 niche_vlaanderen-1.3/tests/data/bwk/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)    29518 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek.sbn
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek.sbx
+-rw-r--r--   0 runner    (1001) docker     (127)    23436 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    15037 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek.shp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek.shx
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek_simplified.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek_simplified.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek_simplified.prj
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek_simplified.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    15037 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek_simplified.shp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/BWK_2020_clip_ZwarteBeek_simplified.shx
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk/bkw_brasschaat_part1.mshp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.489316 niche_vlaanderen-1.3/tests/data/bwk_fake/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_fake/bwk_fake_extentok.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_fake/bwk_fake_extentok.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_fake/bwk_fake_extentok.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_fake/bwk_fake_extentok.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_fake/bwk_fake_extentok.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_fake/bwk_fake_extentok.shx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.489316 niche_vlaanderen-1.3/tests/data/bwk_tiny/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/bwk_clip.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/bwk_clip.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/bwk_clip.prj
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/bwk_clip.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/bwk_clip.shx
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/mhw.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/mhw.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/mlw.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/mlw.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/soil.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/soil.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/soil14.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/soil14.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/bwk_tiny/tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    90446 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/depths_with_nodata.asc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.493317 niche_vlaanderen-1.3/tests/data/ff_bt_t10_h/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/ff_bt_t10_h/dblbnd.adf
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/ff_bt_t10_h/hdr.adf
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/ff_bt_t10_h/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/ff_bt_t10_h/prj.adf
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/ff_bt_t10_h/sta.adf
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/ff_bt_t10_h/vat.adf
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/ff_bt_t10_h/w001001.adf
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/ff_bt_t10_h/w001001x.adf
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/hab_niche_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/mlw_small.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/msw_small_moved.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/msw_small_moved.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/msw_small_wgs84.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/msw_small_wgs84.prj
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/part_zwarte_beek_mlw.asc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/part_zwarte_beek_mlw.prj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.493317 niche_vlaanderen-1.3/tests/data/small/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/T25.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/T25.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/acidity.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/acidity.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/conductivity.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/conductivity.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/inundation.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/inundation.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/inundation_nutrient.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/inundation_nutrient.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/mhw.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/mhw.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/mlw.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/mlw.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/msw.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/msw.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/nutrient_level.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/nutrient_level.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/soil_code.asc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small/soil_code.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/small_nocrs.asc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:04.493317 niche_vlaanderen-1.3/tests/data/tif/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/tif/soil_code.tif
+-rw-r--r--   0 runner    (1001) docker     (127)    67906 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/tif/soil_smallerextent_float.tif
+-rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/data/zwb_soils.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/flooding-codetables.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/floodplain.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/small.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/small_abiotic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/small_abiotic_extra.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/small_abiotic_invalid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/small_ct.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/small_nostrict.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/small_simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/test_acidity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/test_codetables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/test_flooding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24830 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/test_niche.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/test_nutrient_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/test_spatial_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-02 15:18:39.000000 niche_vlaanderen-1.3/tests/test_vegetation.py
```

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/acidity.py` & `niche_vlaanderen-1.3/niche_vlaanderen/acidity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from pkg_resources import resource_filename
-
 import numpy as np
 import pandas as pd
 
-from .codetables import validate_tables_acidity, check_codes_used
+from niche_vlaanderen.codetables import package_resource
+from niche_vlaanderen.codetables import validate_tables_acidity, check_codes_used
 
 
 class Acidity(object):
     """Class to calculate the Acidity
 
     The used codetables can be overwritten by using the corresponding ct_*
     arguments.
@@ -21,33 +20,28 @@
         ct_soil_mlw_class=None,
         ct_soil_codes=None,
         lnk_acidity=None,
         ct_seepage=None,
     ):
 
         if ct_acidity is None:
-            ct_acidity = resource_filename(
-                "niche_vlaanderen", "system_tables/acidity.csv"
-            )
+            ct_acidity = package_resource(
+                ["system_tables"], "acidity.csv")
         if ct_soil_mlw_class is None:
-            ct_soil_mlw_class = resource_filename(
-                "niche_vlaanderen", "system_tables/soil_mlw_class.csv"
-            )
+            ct_soil_mlw_class = package_resource(
+                ["system_tables"], "soil_mlw_class.csv")
         if ct_soil_codes is None:
-            ct_soil_codes = resource_filename(
-                "niche_vlaanderen", "system_tables/soil_codes.csv"
-            )
+            ct_soil_codes = package_resource(
+                ["system_tables"], "soil_codes.csv")
         if lnk_acidity is None:
-            lnk_acidity = resource_filename(
-                "niche_vlaanderen", "system_tables/lnk_acidity.csv"
-            )
+            lnk_acidity = package_resource(
+                ["system_tables"], "lnk_acidity.csv")
         if ct_seepage is None:
-            ct_seepage = resource_filename(
-                "niche_vlaanderen", "system_tables/seepage.csv"
-            )
+            ct_seepage = package_resource(
+                ["system_tables"], "seepage.csv")
 
         self._ct_acidity = pd.read_csv(ct_acidity)
         self._ct_soil_mlw = pd.read_csv(ct_soil_mlw_class)
         self._ct_soil_codes = pd.read_csv(ct_soil_codes)
         self._lnk_acidity = pd.read_csv(lnk_acidity)
         self._ct_seepage = pd.read_csv(ct_seepage)
 
@@ -67,22 +61,22 @@
     def _calculate_soil_mlw(self, soil_code, mlw):
         check_codes_used("soil_code", soil_code, self._ct_soil_codes.index)
 
         # determine soil_group for soil_code
         orig_shape = mlw.shape
         soil_code = soil_code.flatten()
         mlw = mlw.flatten()
-        soil_group = self._ct_soil_codes.soil_group.reindex(soil_code).values.astype(
-            "int8"
+        soil_group = (
+            self._ct_soil_codes.soil_group
+            .reindex(soil_code, fill_value=-99)  # Fill with -99 for no data
+            .values.astype("int8")
         )
-        # the function above gives 0 for no data
-        soil_group[soil_group == 0] = -99
 
         result = np.full(soil_code.shape, -99)
-        for sel_group, subtable in self._ct_soil_mlw.groupby(["soil_group"]):
+        for sel_group, subtable in self._ct_soil_mlw.groupby("soil_group"):
 
             subtable = subtable.copy().reset_index(drop=True)
             index = np.digitize(mlw, subtable.mlw_max, right=True)
             selection = soil_group == sel_group
             result[selection] = subtable.soil_mlw_class.reindex(index)[selection]
 
         result[mlw == -99] = -99
```

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/cli.py` & `niche_vlaanderen-1.3/niche_vlaanderen/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import click
+
 import niche_vlaanderen
-from pkg_resources import resource_filename
+from niche_vlaanderen.codetables import package_resource
 
 
 @click.command()
 @click.pass_context
 @click.option("--example", is_flag=True, help="prints an example configuration file")
 @click.option("--version", is_flag=True, help="prints the version number")
 @click.argument("config", required=False, type=click.Path(exists=True))
 def cli(ctx, config, example, version):
     """Command line interface to the NICHE vegetation model"""
     if example:
-        ex = resource_filename("niche_vlaanderen", "system_tables/example.yaml")
+        ex = package_resource(
+            ["system_tables"], "example.yaml")
         with open(ex) as f:
             print(f.read())
 
     if config is not None:
         n = niche_vlaanderen.Niche()
         n.run_config_file(config, overwrite_ct=True)
         click.echo(n)
```

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/codetables.py` & `niche_vlaanderen-1.3/niche_vlaanderen/codetables.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,33 @@
-import numpy as np
-from .exception import NicheException
+import sys
 import warnings
 
+import numpy as np
+
+from niche_vlaanderen.exception import NicheException
+
+
+def package_resource(folder_paths, file_path):
+    """Provide backward compatbile package resources load function
+
+    Parameters
+    ----------
+    folder_paths : list
+        List of folders and subfolders to get resources from.
+    file_path : str
+        File name of the package resource.
+    """
+    if sys.version_info < (3, 10):
+        from pkg_resources import resource_filename
+        return resource_filename("niche_vlaanderen",
+                                 f"{'/'.join(folder_paths)}/{file_path}")
+    else:
+        from importlib.resources import files
+        return files(f"niche_vlaanderen.{'.'.join(folder_paths)}").joinpath(file_path)
+
 
 class CodeTableException(Exception):
     """
     Exception while validating the code tables
     """
 
 
@@ -19,15 +41,21 @@
     value: the column containing the reclassified value
 
     This function will check if there are no overlapping values when
     classifying the dataframe (df).
     """
 
     group_cols = set(df.columns.tolist()) - {min_col, max_col, value}
-    for sel_group, subtable in df.groupby(list(group_cols)):
+    # Tackle Pandas single key (no list) versus multiple keys 
+    # (in a list) as input to groupby
+    if len(list(group_cols)) > 1:
+        groups = list(group_cols)
+    else:
+        groups = list(group_cols)[0]
+    for sel_group, subtable in df.groupby(groups):
         min_values = subtable[min_col]
         max_values = subtable[max_col]
         for (i, index) in enumerate(min_values.index):
             if i > 0:
                 if min_values[index] != max_values[prev_index]:  # noqa: F821
                     raise CodeTableException(
                         "Min and max values in table do not correspond"
@@ -64,16 +92,14 @@
         if inner:
             raise CodeTableException("Different keys exist in tables.")
         else:
             if not np.all(np.isin(u1, u2)):
                 raise CodeTableException("Not all codes from table 1 are in table 2")
             else:
                 warnings.warn("Warning, different keys exist in tables")
-        print(u1)
-        print(u2)
 
 
 def check_unique(df, col):
     u = df[col].unique()
     if u.size != df[col].size:
         raise CodeTableException("Non unique fields in column {}".format(col))
```

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/flooding.py` & `niche_vlaanderen-1.3/niche_vlaanderen/flooding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import division
-
 import logging
 import rasterio
 import os
-from pkg_resources import resource_filename
 import copy
 from collections import OrderedDict
 
 import pandas as pd
 import numpy as np
 import numpy.ma as ma
 
-from .spatial_context import SpatialContext
-from .codetables import validate_tables_flooding, check_codes_used
+from niche_vlaanderen.spatial_context import SpatialContext
+from niche_vlaanderen.codetables import (validate_tables_flooding,
+                                         check_codes_used,
+                                         package_resource)
 
 
 class FloodingException(Exception):
     """"""
 
 
 class Flooding(object):
@@ -43,17 +43,16 @@
     ):
         self._ct = dict()
         self._veg = dict()
         self._log = logging.getLogger("niche_vlaanderen")
 
         for i in ["depths", "duration", "frequency", "lnk_potential", "potential"]:
             if locals()[i] is None:
-                ct = resource_filename(
-                    "niche_vlaanderen", "system_tables/flooding/" + i + ".csv"
-                )
+                ct = package_resource(["system_tables", "flooding"],
+                                      f"{i}.csv")
             else:
                 ct = locals()[i]
             self._ct[i] = pd.read_csv(ct)
         self.name = name
 
         inner = all(v is None for v in self.__init__.__code__.co_varnames[1:])
 
@@ -105,15 +104,15 @@
         nodata = depth == -99
 
         check_codes_used("depth", depth, self._ct["depths"]["code"])
         check_codes_used("frequency", frequency, self._ct["frequency"]["code"])
         check_codes_used("duration", duration, self._ct["duration"]["code"])
         check_codes_used("period", period, ["summer", "winter"])
 
-        for veg_code, subtable_veg in self._ct["lnk_potential"].groupby(["veg_code"]):
+        for veg_code, subtable_veg in self._ct["lnk_potential"].groupby("veg_code"):
             subtable_veg = subtable_veg.reset_index()
             # by default we give code 4 (no information/flooding)
             # https://github.com/inbo/niche_vlaanderen/issues/87
             self._veg[veg_code] = np.full(depth.shape, 4, dtype="int16")
             self._veg[veg_code][nodata] = -99
             groupby_cols = ["period", "frequency", "duration"]
             for index, subtable in subtable_veg.groupby(groupby_cols):
```

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/niche.py` & `niche_vlaanderen-1.3/niche_vlaanderen/niche.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-import rasterio
-import rasterstats
 import warnings
 import inspect
-
-import numpy as np
-import numpy.ma as ma
-import pandas as pd
-
-from .vegetation import Vegetation, VegSuitable
-from .acidity import Acidity
-from .nutrient_level import NutrientLevel
-from .spatial_context import SpatialContext
-from .version import __version__
-from .flooding import Flooding
-from .exception import NicheException
-
-from pkg_resources import resource_filename
 import json
-from pkg_resources import parse_version
+from packaging.version import parse
 from urllib.request import urlopen, URLError
-
 import logging
 import os.path
 import numbers
 import yaml
 import datetime
 import sys
 
+import numpy as np
+import numpy.ma as ma
+import pandas as pd
+import rasterio
+import rasterstats
 from tqdm import tqdm
 
+from niche_vlaanderen.vegetation import Vegetation, VegSuitable
+from niche_vlaanderen.acidity import Acidity
+from niche_vlaanderen.nutrient_level import NutrientLevel
+from niche_vlaanderen.spatial_context import SpatialContext
+from niche_vlaanderen.version import __version__
+from niche_vlaanderen.flooding import Flooding
+from niche_vlaanderen.exception import NicheException
+from niche_vlaanderen.codetables import package_resource
+
+
 _allowed_input = {
     "soil_code",
     "mlw",
     "msw",
     "mhw",
     "seepage",
     "inundation_acidity",
@@ -199,16 +197,22 @@
 
     def _check_latest_version(self):
         url = "https://pypi.python.org/pypi/niche_vlaanderen/json"
         try:
             response = urlopen(url, timeout=5)
             json_response = json.loads(response.read().decode("utf-8"))
             releases = json_response["releases"]
-            v = sorted(releases, key=parse_version, reverse=True)
-            last = v[0]
+            versions = sorted(releases, key=parse, reverse=True)
+
+            # remove alpha, beta, rc versions
+            dev = ["rc", "a", "b"]
+            indev = lambda a: any(devstring in a for devstring in dev)
+            versions = [v for v in versions if not indev(v)]
+
+            last = versions[0]
 
             if last == __version__:
                 s = "# Using latest niche_vlaanderen  %s" % __version__
             else:
                 s = "# Newer niche_vlaanderen  %s available" % last  # pragma: no cover
         except URLError:  # pragma: no cover
             s = "# Error determinining last upstream version"
@@ -429,23 +433,27 @@
                 "nitrogen_atmospheric",
                 "mhw",
                 "mlw",
                 "msw",
             ):
                 band = band.astype("float32")
 
-            # convert old soil codes to new soil codes
-            if f == "soil_code" and np.all(band[band != nodata] >= 10000):
-                band[band != nodata] = np.round(band[band != nodata] / 10000)
-
             # create a mask for no-data values, taking into account data-types
             if band.dtype == "float32" and nodata is not None:
-                band[np.isclose(band, nodata)] = np.nan
+                band[np.isclose(nodata, band)] = np.nan
             else:
                 band[band == nodata] = -99
+            
+            # convert old soil codes to new soil codes
+            if f == "soil_code" and np.all((band >= 10000)|(band==-99)|np.isnan(band)):
+                band[band>=10000] = np.round(band[band>=10000] / 10000)
+            
+            if f == "soil_code" and band.dtype == "float32":
+                band[np.isnan(band)] = -99
+                band = band.astype(int)
 
             inputarray[f] = band
 
         # Load in all constant inputvalues
         for f in self._inputvalues:
             shape = (int(self._context.height), int(self._context.width))
             inputarray[f] = np.full(shape, self._inputvalues[f])
@@ -639,14 +647,15 @@
             Save detailed information on factor affecting vegetation possibility
 
         """
 
         if not self.vegetation_calculated:
             raise NicheException("A valid run must be done before writing the output.")
 
+        folder = str(folder)
         self._options["output_dir"] = folder
 
         if not os.path.exists(folder):
             os.makedirs(folder)
 
         params = dict(
             driver="GTiff",
@@ -774,14 +783,20 @@
             msg = "Could not import matplotlib\n"
             msg += "matplotlib required for plotting functions"
             raise ImportError(msg)
 
         norm = None
         v = None
 
+        # Inform user that data is not available to plot
+        # (key is present, but value is None)
+        if key not in self._inputfiles and key in self._inputarray:
+            if not self._inputarray[key]:
+                raise KeyError(f"{key} data is not available to plot.")
+
         if key in self._inputfiles and key not in self._inputarray:
             # if set_input has been done, but no model run yet
             # in this case we will open the file and fetch the data
             with rasterio.open(self._inputfiles[key], "r") as dst:
                 window = self._context.get_read_window(SpatialContext(dst))
                 v = dst.read(1, window=window)
                 v = ma.masked_equal(v, dst.nodatavals[0])
@@ -849,15 +864,15 @@
             colormap to use for the maps. Note that 9 combinations of
             presence/absence are possible, so keep this in mind if changing
             from the default value.
         """
         try:
             import matplotlib.pyplot as plt
             import matplotlib.patches as mpatches
-            from matplotlib import cm
+            import matplotlib
 
         except (ImportError, RuntimeError):  # pragma: no cover
             msg = "Could not import matplotlib\n"
             msg += "matplotlib required for plotting functions"
             raise ImportError(msg)
 
         if key not in self._vegetation.keys():
@@ -888,20 +903,20 @@
             vmax=len(VegSuitable.possible()) + 1,
         )
 
         if limit_legend:
             present = ma.unique(v_un[~v_un.mask])
 
             patches = [
-                mpatches.Patch(color=cm.get_cmap(cmap)(i), label=legend[legend_keys[i]])
+                mpatches.Patch(color=matplotlib.colormaps[cmap](i), label=legend[legend_keys[i]])
                 for i in present
             ]
         else:
             patches = [
-                mpatches.Patch(color=cm.get_cmap(cmap)(i), label=legend[j])
+                mpatches.Patch(color=matplotlib.colormaps[cmap](i), label=legend[j])
                 for i, j in enumerate(legend)
             ]
 
         plt.legend(handles=patches, bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.0)
 
         if self.name != "":
             title = self.name + " " + title
@@ -987,16 +1002,21 @@
         #warnings.simplefilter(action="ignore", category=DeprecationWarning)
 
         presence = dict({0: "not present", 1: "present", 255: "no data"})
 
         if vegetation_types is None:
             vegetation_types = self._vegetation.keys()
 
+        if len(vegetation_types) == 0:
+            raise NicheException("Can not calculate zonal statistics for "
+                                 "empty vegetation list")
+
         logger.debug(f"vegetation_types: {vegetation_types}")
         logger.debug(f"upscaling to {upscale}")
+
         for i in tqdm(vegetation_types):
             # Note we use -99 as nodata value to make sure the true nodata
             # value (255) is part of the result table.
 
             if upscale == 1:
                 raster = self._vegetation[i]
                 affine = self._context.transform
@@ -1012,15 +1032,15 @@
                 )
 
             td[i] = rasterstats.zonal_stats(
                 vectors=vectors,
                 raster=raster,
                 affine=affine,
                 categorical=True,
-                nodata=-99,
+                nodata=Vegetation.nodata_veg,
                 geojson_out=attribute is not None,
             )
         warnings.simplefilter("default")
 
         ti = []
         attribute_list = []
 
@@ -1070,17 +1090,16 @@
 
         Uses ct_vegetation columns veg_code and veg_type"""
 
         if not hasattr(self, "_vegcode2namedict"):
             if "ct_vegetation" in self._code_tables:
                 ct_vegetation = self._code_tables["ct_vegetation"]
             else:
-                ct_vegetation = resource_filename(
-                    "niche_vlaanderen", "system_tables/niche_vegetation.csv"
-                )
+                ct_vegetation = package_resource(
+                    ["system_tables"], "niche_vegetation.csv")
 
             ct_vegetation = pd.read_csv(ct_vegetation)
             subtable = ct_vegetation[["veg_code", "veg_type"]]
             veg_dict = subtable.set_index("veg_code").to_dict()["veg_type"]
             self._vegcode2namedict = veg_dict
         return self._vegcode2namedict[vegcode]
```

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/nutrient_level.py` & `niche_vlaanderen-1.3/niche_vlaanderen/nutrient_level.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from pkg_resources import resource_filename
-
 import numpy as np
 import pandas as pd
-from .codetables import validate_tables_nutrient_level, check_codes_used
+
+from niche_vlaanderen.codetables import (validate_tables_nutrient_level,
+                                         check_codes_used, package_resource)
 
 
 class NutrientLevel(object):
     """
     Class to calculate the NutrientLevel
 
     The used codetables can be overwritten by using the corresponding ct_*
@@ -20,34 +20,28 @@
         ct_lnk_soil_nutrient_level=None,
         ct_management=None,
         ct_mineralisation=None,
         ct_soil_code=None,
         ct_nutrient_level=None,
     ):
         if ct_lnk_soil_nutrient_level is None:
-            ct_lnk_soil_nutrient_level = resource_filename(
-                "niche_vlaanderen", "system_tables/lnk_soil_nutrient_level.csv"
-            )
+            ct_lnk_soil_nutrient_level = package_resource(
+                ["system_tables"], "lnk_soil_nutrient_level.csv")
         if ct_management is None:
-            ct_management = resource_filename(
-                "niche_vlaanderen", "system_tables/management.csv"
-            )
+            ct_management = package_resource(
+                ["system_tables"], "management.csv")
         if ct_mineralisation is None:
-            ct_mineralisation = resource_filename(
-                "niche_vlaanderen", "system_tables/nitrogen_mineralisation.csv"
-            )
+            ct_mineralisation = package_resource(
+                ["system_tables"], "nitrogen_mineralisation.csv")
         if ct_soil_code is None:
-            ct_soil_code = resource_filename(
-                "niche_vlaanderen", "system_tables/soil_codes.csv"
-            )
-
+            ct_soil_code = package_resource(
+                ["system_tables"], "soil_codes.csv")
         if ct_nutrient_level is None:
-            ct_nutrient_level = resource_filename(
-                "niche_vlaanderen", "system_tables/nutrient_level.csv"
-            )
+            ct_nutrient_level = package_resource(
+                ["system_tables"], "nutrient_level.csv")
 
         self.ct_lnk_soil_nutrient_level = pd.read_csv(ct_lnk_soil_nutrient_level)
         self._ct_management = pd.read_csv(ct_management).set_index("management")
         self._ct_mineralisation = pd.read_csv(ct_mineralisation)
         self._ct_nutrient_level = pd.read_csv(ct_nutrient_level)
         self._ct_soil_code = pd.read_csv(ct_soil_code)
```

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/spatial_context.py` & `niche_vlaanderen-1.3/niche_vlaanderen/spatial_context.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from affine import Affine
 from textwrap import dedent
 import warnings
 
+from affine import Affine
 
 class SpatialContextError(Exception):
     """"""
 
 
 class SpatialContext(object):
     """Stores the spatial context of the grids in niche
```

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/example.yaml` & `niche_vlaanderen-1.3/niche_vlaanderen/system_tables/example.yaml`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/flooding/lnk_potential.csv` & `niche_vlaanderen-1.3/niche_vlaanderen/system_tables/flooding/lnk_potential.csv`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/hab_niche_join.csv` & `niche_vlaanderen-1.3/niche_vlaanderen/system_tables/hab_niche_join.csv`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/lnk_acidity.csv` & `niche_vlaanderen-1.3/niche_vlaanderen/system_tables/lnk_acidity.csv`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/lnk_soil_nutrient_level.csv` & `niche_vlaanderen-1.3/niche_vlaanderen/system_tables/lnk_soil_nutrient_level.csv`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/niche_vegetation.csv` & `niche_vlaanderen-1.3/niche_vlaanderen/system_tables/niche_vegetation.csv`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/nitrogen_mineralisation.csv` & `niche_vlaanderen-1.3/niche_vlaanderen/system_tables/nitrogen_mineralisation.csv`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/system_tables/soil_codes.csv` & `niche_vlaanderen-1.3/niche_vlaanderen/system_tables/soil_codes.csv`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/validation.py` & `niche_vlaanderen-1.3/niche_vlaanderen/validation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 import warnings
+from collections import defaultdict
 from pathlib import Path
 
-from pkg_resources import resource_filename
-
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore", category=DeprecationWarning)
     warnings.filterwarnings("ignore", category=UserWarning)
     import geopandas as gpd
 
 import numpy as np
 import pandas as pd
 
 from niche_vlaanderen.niche import Niche
+from niche_vlaanderen.codetables import package_resource
 
 logger = logging.getLogger(__name__)
 
 
 class NicheValidationException(Exception):
     msg = "Error using Niche Overlay"
 
@@ -46,14 +46,28 @@
             and Niche vegetation types. The default mapping is a mapping of the
             BWK map (biologische waarderingskaart), and is
             part of the package at niche_vlaanderen/system_tables/hab_nich_join.csv
 
             If a mapping is provided by the user, it must contain a HAB and a NICHE column.
             Other columns are ignored.
 
+        upscale: int
+            optional upscale value that is used to increase the resolution of
+            the niche rasters while doing the overlay.
+            instead of using only the cell center, the comparison between the
+            vegetation map and the niche model is done at upscale*upscale places
+            in the cell. Defaults to 5.
+            More details in
+            https://inbo.github.io/niche_vlaanderen/validation.html
+
+        id: str
+            (optional) field to use as id for the provided map file. This id will
+            be used in the overlay. If no id is supplied, the shape_index (row number)
+            of the vector file will be used, starting from 0.
+
 
     """
 
     def __init__(self, niche, map, mapping_file=None, upscale=5, id=None):
         if type(niche) is Niche:
             self.niche = niche
         else:
@@ -72,20 +86,17 @@
             veg: list(columns.str.upper()).index(f"PHAB{veg}")
             for veg in vegetation_columns.str[-1]
         }
         self.proportion_columns = {
             i: columns[proportion_index[i]] for i in proportion_index
         }
 
-        print(self.proportion_columns)
-
         if mapping_file is None:
-            mapping_file = resource_filename(
-                "niche_vlaanderen", "system_tables/hab_niche_join.csv"
-            )
+            mapping_file = package_resource(["system_tables"],
+                                            "hab_niche_join.csv")
 
         mapping = pd.read_csv(mapping_file)
 
         # drop any row containing niche vegetation 0
         mapping = mapping[mapping["NICHE"] != 0]
 
         # convert to wide format
@@ -122,26 +133,30 @@
     def __repr__(self):
 
         o = "# Niche Validation object\n"
         o += f"map: {self.filename_map}\n"
         o += f"niche object: {self.niche.name}"
         return o
 
-    def overlay(self, upscale=4):
+    def overlay(self, upscale=5):
         """Overlays the map and the niche object"""
 
         # Remove any existing "NICH" columns
 
         present_vegetation_types = np.unique(self.map[self._niche_columns])
 
         present_vegetation_types = present_vegetation_types[
             ~np.isnan(present_vegetation_types)
         ]
-
         logger.debug(f"present niche types: {present_vegetation_types}")
+
+        if len(present_vegetation_types) == 0:
+            raise NicheValidationException(
+                "No Niche vegetation present in validation map"
+            )
         # get potential presence
         # upscale niche rasters to that before calculating statistics
         self.potential_presence = self.niche.zonal_stats(
             self.map,
             outside=False,
             vegetation_types=present_vegetation_types,
             upscale=upscale,
@@ -150,107 +165,114 @@
         self.potential_presence = self.potential_presence.pivot(
             columns=["vegetation"], index=["presence", "shape_id"]
         )
 
         self._tables = [
             "area_pot",
             "area_nonpot",
-            "area_nonpot_optimistic",
-            "area_pot_perc_optimistic",
+            "area_nonpot_phab",
+            "area_pot_perc_phab",
             "area_effective",
             "area_pot_perc",
             "veg_present",
         ]
 
         self.area_pot = self.potential_presence.loc["no data"]["area_ha"] * np.nan
         self.area_nonpot = self.potential_presence.loc["no data"]["area_ha"] * np.nan
         self.area_effective = self.potential_presence.loc["no data"]["area_ha"] * np.nan
         self.area_pot_perc = self.potential_presence.loc["no data"]["area_ha"] * np.nan
-        self.area_pot_perc_optimistic = self.area_pot_perc * np.nan
-        self.area_nonpot_optimistic = self.area_pot_perc * np.nan
-
+        self.area_pot_perc_phab = self.area_pot_perc * np.nan
+        self.area_nonpot_phab = self.area_pot_perc * np.nan
         self.veg_present = self.area_pot_perc * 0
 
         # Only if actual present: (pHAB * present) / (present + not present)
         for i, row in self.map.iterrows():
+            logger.debug(f"row: {row.area_shape}")
+            # different mappings can exist which lead to the same vegetation
+            # type. First we aggregate them in shape_veg which contains
+            # the niche vegetation and the sum of its pHAB
+            shape_veg = defaultdict(lambda: 0)
+
             for veg in self._niche_columns:
                 if np.isfinite(row[veg]) and row[veg] != 0:
-                    logger.debug(f"row: {row.area_shape}")
-                    area_pot = (
-                        self.potential_presence.loc["present"]
-                        .loc[i]
-                        .loc["area_ha"][row[veg]]
-                    )
-                    if np.isnan(self.area_pot[row[veg]].loc[i]):
-                        self.area_pot[row[veg]].loc[i] = area_pot
-                    else:
-                        self.area_pot[row[veg]].loc[i] += area_pot
-
-                    area_nonpot = (
-                        self.potential_presence.loc["not present"]
-                        .loc[i]
-                        .loc["area_ha"][row[veg]]
-                    )
-                    if np.isnan(self.area_nonpot[row[veg]].loc[i]):
-                        self.area_nonpot[row[veg]].loc[i] = area_nonpot
-                    else:
-                        self.area_nonpot[row[veg]].loc[i] += area_nonpot
+                    pHab = row[self.proportion_columns[veg[5]]]
+                    shape_veg[int(row[veg])] += pHab
 
-                    # TODO: case insensitive!
+            for veg in shape_veg:
+                pHab = shape_veg[veg]
 
-                    pHab = row[self.proportion_columns[veg[5]]]
+                area_pot = (
+                    self.potential_presence.loc["present"].loc[i].loc["area_ha"][veg]
+                )
+
+                self.area_pot.loc[i, veg] = area_pot
 
-                    area_effective = pHab * (area_pot + area_nonpot) / 100
-                    # area of the shape
-                    if np.isnan(self.area_effective[row[veg]].loc[i]):
-                        self.area_effective[row[veg]].loc[i] = area_effective
-                    else:
-                        self.area_effective[row[veg]].loc[i] += area_effective
-
-                    if (area_pot + area_nonpot) == 0:
-                        warnings.warn(
-                            f"No overlap between potential vegetation map and "
-                            f"shape_id {i}"
-                        )
-                    else:
-                        # vegetation type is present (actual presence)
-                        # used in polygon count
-                        self.veg_present[row[veg]].loc[i] = 1
+                area_nonpot = (
+                    self.potential_presence.loc["not present"]
+                    .loc[i]
+                    .loc["area_ha"][veg]
+                )
+
+                self.area_nonpot.loc[i, veg] = area_nonpot
+                area_effective = pHab * (area_pot + area_nonpot) / 100
+                self.area_effective.loc[i, veg] = area_effective
+
+                if (area_pot + area_nonpot) == 0:
+                    warnings.warn(
+                        f"No overlap between potential vegetation map and "
+                        f"shape_id {i}"
+                    )
+                else:
+                    # vegetation type is present (actual presence)
+                    # used in polygon count
+                    self.veg_present.loc[i, veg] = 1
 
         # aggregate statistics
-        self.area_pot_perc = self.area_pot / (self.area_pot + self.area_nonpot)
-        self.area_pot_perc_optimistic = np.minimum(
+        self.area_pot_perc = 100 * self.area_pot / (self.area_pot + self.area_nonpot)
+        self.area_pot_perc_phab = np.minimum(
             100 * self.area_pot / self.area_effective, 100
         )
-        self.area_nonpot_optimistic = np.maximum(0, self.area_effective - self.area_pot)
+        self.area_nonpot_phab = np.maximum(0, self.area_effective - self.area_pot)
 
         # Set id column for every polygon based table
         if self.id is not None:
             for table in self._tables:
                 setattr(self, table, getattr(self, table).set_index(self.map[self.id]))
 
         # create summary table per vegetation type
 
         summary = {}
         summary["area_effective"] = self.area_effective.sum()
         summary["nonpot"] = self.area_nonpot.sum()
-        summary["nonpot_opt"] = self.area_nonpot_optimistic.sum()
+        summary["nonpot_phab"] = self.area_nonpot_phab.sum()
         summary["pot"] = self.area_pot.sum()
         summary["polygon_count"] = self.veg_present.sum()
 
         summary["score"] = 100 * summary["pot"] / (summary["pot"] + summary["nonpot"])
-        summary["score_opt"] = (
-            100 * summary["pot"] / (summary["pot"] + summary["nonpot_opt"])
+        summary["score_phab"] = (
+            100 * summary["pot"] / (summary["pot"] + summary["nonpot_phab"])
         )
 
         self.summary = pd.DataFrame(summary)
 
-    def write(self, path, overwrite=False):
+    def write(self, path, overwrite_files=False):
+        """Write the result of the validation to a folder
+
+        path: string | pathlib.Path
+            Output folder to which files will be written. Parent directory must
+            already exist.
+
+        overwrite_files: bool
+            Overwrite files when saving.
+            Note writing will fail if any of the files to be written already
+            exists.
+        """
+
         path = Path(path)
-        if path.exists() and not overwrite:
+        if path.exists() and not overwrite_files:
             if not path.is_dir():
                 raise NicheValidationException(f"path {path} is not an empty folder")
             if any(path.iterdir()):
                 raise NicheValidationException(f"path {path} exists and is not empty")
         path.mkdir(parents=True, exist_ok=True)
 
         # save individual tables
@@ -260,15 +282,15 @@
 
         self.potential_presence.to_csv(path / "potential_presence.csv")
         self.summary.to_csv(path / "summary.csv")
 
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=DeprecationWarning)
             warnings.filterwarnings("ignore", category=FutureWarning)
-            self.joined_map().to_file(path / "overlay.gpkg")
+            self.joined_map().to_file(path / "validation.gpkg")
 
     def joined_map(self):
         """Create a geopandas dataframe with all tables joined"""
         merged = self.map
         if self.id:
             merged = merged.set_index(self.id)
         for table in self._tables:
```

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen/vegetation.py` & `niche_vlaanderen-1.3/niche_vlaanderen/vegetation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import division
-from pkg_resources import resource_filename
 from enum import IntEnum
+import warnings
 
 import numpy as np
 import pandas as pd
-import warnings
 
-from .nutrient_level import NutrientLevel
-from .acidity import Acidity
-from .codetables import validate_tables_vegetation, check_codes_used
-from .exception import NicheException
+from niche_vlaanderen.nutrient_level import NutrientLevel
+from niche_vlaanderen.acidity import Acidity
+from niche_vlaanderen.codetables import (validate_tables_vegetation,
+                                         check_codes_used, package_resource)
+from niche_vlaanderen.exception import NicheException
 
 
 class VegSuitable(IntEnum):
     SOIL = 1
     MXW = 2
     NUTRIENT = 4
     ACIDITY = 8
@@ -81,45 +81,39 @@
         This class initializes the Vegetation helper class. By default it uses
         the code tables supplied by the niche_vlaanderen package. It is
         possible to overwrite this by supplying the niche_vlaanderen parameter
 
         """
 
         if ct_vegetation is None:
-            ct_vegetation = resource_filename(
-                "niche_vlaanderen", "system_tables/niche_vegetation.csv"
-            )
+            ct_vegetation = package_resource(["system_tables"],
+                                             "niche_vegetation.csv")
 
         # Note that the next code tables are only used for validation, they are
         # not part of the logic of the vegetation class
 
         if ct_soil_code is None:
-            ct_soil_code = resource_filename(
-                "niche_vlaanderen", "system_tables/soil_codes.csv"
-            )
+            ct_soil_code = package_resource(["system_tables"],
+                                             "soil_codes.csv")
 
         if ct_acidity is None:
-            ct_acidity = resource_filename(
-                "niche_vlaanderen", "system_tables/acidity.csv"
-            )
+            ct_acidity = package_resource(["system_tables"],
+                                             "acidity.csv")
 
         if ct_nutrient_level is None:
-            ct_nutrient_level = resource_filename(
-                "niche_vlaanderen", "system_tables/nutrient_level.csv"
-            )
+            ct_nutrient_level = package_resource(["system_tables"],
+                                                 "nutrient_level.csv")
 
         if ct_management is None:
-            ct_management = resource_filename(
-                "niche_vlaanderen", "system_tables/management.csv"
-            )
+            ct_management = package_resource(["system_tables"],
+                                                 "management.csv")
 
         if ct_inundation is None:
-            ct_inundation = resource_filename(
-                "niche_vlaanderen", "system_tables/inundation.csv"
-            )
+            ct_inundation = package_resource(["system_tables"],
+                                             "inundation.csv")
 
         self._ct_vegetation = pd.read_csv(ct_vegetation)
         self._ct_soil_code = pd.read_csv(ct_soil_code)
         self._ct_acidity = pd.read_csv(ct_acidity)
         self._ct_nutrient_level = pd.read_csv(ct_nutrient_level)
         self._ct_management = pd.read_csv(ct_management)
         self._ct_inundation = pd.read_csv(ct_inundation)
@@ -166,16 +160,15 @@
             A boolean (default=True) whether all grids should be returned or
             only grids containing data.
 
         Returns
         -------
         veg: dict
             A dictionary containing the different output arrays per
-            veg_code value.
-            -99 is used for nodata_veg values
+            veg_code value. 255 is used for nodata_veg values
         expected: int
             Expected code in veg arrays if all conditions are met
         veg_occurrence: dict
             A dictionary containing the percentage of the area where the
             vegetation can occur.
 
         """
@@ -211,15 +204,15 @@
         if management is not None:
             check_codes_used("management", management, self._ct_management["code"])
 
         veg_bands = dict()
         veg_detail = dict()
         occurrence = dict()
 
-        for veg_code, subtable in self._ct_vegetation.groupby(["veg_code"]):
+        for veg_code, subtable in self._ct_vegetation.groupby("veg_code"):
 
             subtable = subtable.reset_index()
             # vegi is the prediction for the current veg_code
             # it is a logical or of the result of every row:
             # if a row is 0 for a pixel, that vegetation can occur
 
             vegi = np.zeros(soil_code.shape, dtype="int64")
@@ -310,15 +303,15 @@
             ["veg_code", "soil_code", "mhw_min", "mhw_max", "mlw_min", "mlw_max"]
         ]
 
         veg = veg.drop_duplicates()
 
         warnings.simplefilter(action="ignore", category=RuntimeWarning)
 
-        for veg_code, subtable in veg.groupby(["veg_code"]):
+        for veg_code, subtable in veg.groupby("veg_code"):
             subtable = subtable.reset_index()
 
             mhw_diff = np.full(soil_code.shape, np.nan)
             mlw_diff = np.full(soil_code.shape, np.nan)
 
             for row in subtable.itertuples():
```

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen-1.2b2.egg-info/PKG-INFO` & `niche_vlaanderen-1.3/niche_vlaanderen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niche-vlaanderen
-Version: 1.2b2
+Version: 1.3
 Summary: NICHE Vlaanderen: hydro-ecological model for valley-ecosystems in Flanders
 Home-page: https://github.com/inbo/niche_vlaanderen
 Author: Johan Van de Wauw
 Author-email: johan.vandewauw@inbo.be
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `./usr/local/lib/python3.10/dist-packages/niche_vlaanderen-1.2b2.egg-info/SOURCES.txt` & `niche_vlaanderen-1.3/niche_vlaanderen.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,42 @@
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/Makefile
-docs/authors.rst
 docs/cli.rst
 docs/codetables.rst
 docs/conf.py
 docs/contributing.rst
+docs/credits.rst
 docs/faq.rst
 docs/index.rst
 docs/installation.rst
 docs/invoer.rst
-docs/kalibratie.rst
 docs/lowlevel.rst
 docs/make.bat
 docs/model.rst
 docs/notendop.rst
 docs/overstroming.rst
 docs/principe.rst
+docs/running.rst
 docs/trofie.rst
 docs/tutorials.rst
+docs/validatie.rst
 docs/vegetatie.rst
 docs/vegetatie_reftabel.rst
 docs/vegetatietype.rst
 docs/zuur.rst
 docs/_static/png/acidity_principle.png
 docs/_static/png/acidity_table.png
 docs/_static/png/advanced_properties.png
 docs/_static/png/advanced_properties2.png
+docs/_static/png/bwk_overlay.png
 docs/_static/png/environment_variables.png
 docs/_static/png/exception.png
 docs/_static/png/input_rasters.png
 docs/_static/png/new_environment_variable.png
 docs/_static/png/niche_principle.png
 docs/_static/png/nutrient_classes.png
 docs/_static/png/nutrient_mineralcurve.png
@@ -151,34 +153,39 @@
 tests/data/bwk_tiny/mhw.asc
 tests/data/bwk_tiny/mhw.prj
 tests/data/bwk_tiny/mlw.asc
 tests/data/bwk_tiny/mlw.prj
 tests/data/bwk_tiny/soil.asc
 tests/data/bwk_tiny/soil.prj
 tests/data/bwk_tiny/soil14.asc
+tests/data/bwk_tiny/soil14.prj
 tests/data/bwk_tiny/tiny.yaml
 tests/data/ff_bt_t10_h/dblbnd.adf
 tests/data/ff_bt_t10_h/hdr.adf
 tests/data/ff_bt_t10_h/metadata.xml
 tests/data/ff_bt_t10_h/prj.adf
 tests/data/ff_bt_t10_h/sta.adf
 tests/data/ff_bt_t10_h/vat.adf
 tests/data/ff_bt_t10_h/w001001.adf
 tests/data/ff_bt_t10_h/w001001x.adf
 tests/data/small/T25.asc
+tests/data/small/T25.prj
 tests/data/small/acidity.asc
 tests/data/small/acidity.prj
 tests/data/small/conductivity.asc
 tests/data/small/conductivity.prj
 tests/data/small/inundation.asc
 tests/data/small/inundation.prj
 tests/data/small/inundation_nutrient.asc
 tests/data/small/inundation_nutrient.prj
 tests/data/small/mhw.asc
 tests/data/small/mhw.prj
 tests/data/small/mlw.asc
+tests/data/small/mlw.prj
 tests/data/small/msw.asc
 tests/data/small/msw.prj
 tests/data/small/nutrient_level.asc
 tests/data/small/nutrient_level.prj
 tests/data/small/soil_code.asc
-tests/data/tif/soil_code.tif
+tests/data/small/soil_code.prj
+tests/data/tif/soil_code.tif
+tests/data/tif/soil_smallerextent_float.tif
```

