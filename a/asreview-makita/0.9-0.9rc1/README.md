# Comparing `tmp/asreview_makita-0.9.tar.gz` & `tmp/asreview_makita-0.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asreview_makita-0.9.tar", last modified: Thu May  2 11:06:39 2024, max compression
+gzip compressed data, was "asreview_makita-0.9rc1.tar", last modified: Thu Apr 18 13:14:58 2024, max compression
```

## Comparing `asreview_makita-0.9.tar` & `asreview_makita-0.9rc1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.973718 asreview_makita-0.9/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 11:06:34.000000 asreview_makita-0.9/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.925718 asreview_makita-0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.929718 asreview_makita-0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-02 11:06:34.000000 asreview_makita-0.9/.github/workflows/ci-workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-02 11:06:34.000000 asreview_makita-0.9/.github/workflows/pythonpackage.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.929718 asreview_makita-0.9/.github/workflows/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-05-02 11:06:34.000000 asreview_makita-0.9/.github/workflows/test_data/labels.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-02 11:06:34.000000 asreview_makita-0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-02 11:06:34.000000 asreview_makita-0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-02 11:06:34.000000 asreview_makita-0.9/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-02 11:06:34.000000 asreview_makita-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 11:06:34.000000 asreview_makita-0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17296 2024-05-02 11:06:39.973718 asreview_makita-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16323 2024-05-02 11:06:34.000000 asreview_makita-0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.973718 asreview_makita-0.9/asreview_makita.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17296 2024-05-02 11:06:39.000000 asreview_makita-0.9/asreview_makita.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-02 11:06:39.000000 asreview_makita-0.9/asreview_makita.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:06:39.000000 asreview_makita-0.9/asreview_makita.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-02 11:06:39.000000 asreview_makita-0.9/asreview_makita.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 11:06:39.000000 asreview_makita-0.9/asreview_makita.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 11:06:39.000000 asreview_makita-0.9/asreview_makita.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.925718 asreview_makita-0.9/asreviewcontrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.929718 asreview_makita-0.9/asreviewcontrib/makita/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/template_arfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/template_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/template_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/template_multimodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.933718 asreview_makita-0.9/asreviewcontrib/makita/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/templates/doc_README.md.template
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/templates/script_get_plot.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/templates/script_merge_descriptives.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/templates/script_merge_metrics.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/templates/script_merge_tds.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/templates/template_arfi.txt.template
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/templates/template_basic.txt.template
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/templates/template_multimodel.txt.template
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-02 11:06:34.000000 asreview_makita-0.9/asreviewcontrib/makita/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.933718 asreview_makita-0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.933718 asreview_makita-0.9/examples/arfi_example/
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/arfi_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.937718 asreview_makita-0.9/examples/arfi_example/data/
--rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/arfi_example/data/Smid_2020.csv
--rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/arfi_example/data/van_de_Schoot_2018.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28187 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/arfi_example/jobs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.945718 asreview_makita-0.9/examples/arfi_example/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/arfi_example/scripts/get_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/arfi_example/scripts/merge_descriptives.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/arfi_example/scripts/merge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/arfi_example/scripts/merge_tds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.945718 asreview_makita-0.9/examples/basic_example/
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/basic_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.949718 asreview_makita-0.9/examples/basic_example/data/
--rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/basic_example/data/Smid_2020.csv
--rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/basic_example/data/van_de_Schoot_2018.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/basic_example/jobs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.957718 asreview_makita-0.9/examples/basic_example/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/basic_example/scripts/get_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/basic_example/scripts/merge_descriptives.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/basic_example/scripts/merge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/basic_example/scripts/merge_tds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.957718 asreview_makita-0.9/examples/multimodel_example/
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/multimodel_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.961718 asreview_makita-0.9/examples/multimodel_example/data/
--rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/multimodel_example/data/Smid_2020.csv
--rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/multimodel_example/data/van_de_Schoot_2018.csv
--rw-r--r--   0 runner    (1001) docker     (127)    13063 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/multimodel_example/jobs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:06:39.973718 asreview_makita-0.9/examples/multimodel_example/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/multimodel_example/scripts/get_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/multimodel_example/scripts/merge_descriptives.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/multimodel_example/scripts/merge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-02 11:06:34.000000 asreview_makita-0.9/examples/multimodel_example/scripts/merge_tds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-02 11:06:34.000000 asreview_makita-0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 11:06:39.973718 asreview_makita-0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.338782 asreview_makita-0.9rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.290781 asreview_makita-0.9rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.294781 asreview_makita-0.9rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.github/workflows/ci-workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.github/workflows/pythonpackage.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.294781 asreview_makita-0.9rc1/.github/workflows/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.github/workflows/test_data/labels.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17238 2024-04-18 13:14:58.338782 asreview_makita-0.9rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.338782 asreview_makita-0.9rc1/asreview_makita.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17238 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 13:14:58.000000 asreview_makita-0.9rc1/asreview_makita.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.290781 asreview_makita-0.9rc1/asreviewcontrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.298781 asreview_makita-0.9rc1/asreviewcontrib/makita/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/template_arfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/template_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/template_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/template_multimodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.298781 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/doc_README.md.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_get_plot.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_descriptives.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_metrics.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_tds.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_arfi.txt.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_basic.txt.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_multimodel.txt.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/asreviewcontrib/makita/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.298781 asreview_makita-0.9rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.298781 asreview_makita-0.9rc1/examples/arfi_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-18 13:14:49.000000 asreview_makita-0.9rc1/examples/arfi_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.302781 asreview_makita-0.9rc1/examples/arfi_example/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/data/Smid_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/data/van_de_Schoot_2018.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28187 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/jobs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.310781 asreview_makita-0.9rc1/examples/arfi_example/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/scripts/get_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_descriptives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_tds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.310781 asreview_makita-0.9rc1/examples/basic_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.314781 asreview_makita-0.9rc1/examples/basic_example/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/data/Smid_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/data/van_de_Schoot_2018.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/jobs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.326781 asreview_makita-0.9rc1/examples/basic_example/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/scripts/get_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/scripts/merge_descriptives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/scripts/merge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/basic_example/scripts/merge_tds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.326781 asreview_makita-0.9rc1/examples/multimodel_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.330782 asreview_makita-0.9rc1/examples/multimodel_example/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  3269037 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/data/Smid_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  6963698 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/data/van_de_Schoot_2018.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13063 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/jobs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:14:58.338782 asreview_makita-0.9rc1/examples/multimodel_example/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/scripts/get_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_descriptives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_tds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-18 13:14:50.000000 asreview_makita-0.9rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:14:58.338782 asreview_makita-0.9rc1/setup.cfg
```

### Comparing `asreview_makita-0.9/.github/workflows/ci-workflow.yml` & `asreview_makita-0.9rc1/.github/workflows/ci-workflow.yml`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/.github/workflows/pythonpackage.yml` & `asreview_makita-0.9rc1/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/.github/workflows/test_data/labels.csv` & `asreview_makita-0.9rc1/.github/workflows/test_data/labels.csv`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/.gitignore` & `asreview_makita-0.9rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/CITATION.cff` & `asreview_makita-0.9rc1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/LICENSE` & `asreview_makita-0.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/PKG-INFO` & `asreview_makita-0.9rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asreview-makita
-Version: 0.9
+Version: 0.9rc1
 Summary: Makita workflow tool for the ASReview project
 Author-email: ASReview LAB developers <asreview@uu.nl>
 License: MIT
 Project-URL: homepage, https://asreview.ai
 Project-URL: repository, https://github.com/asreview/asreview-makita
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -35,17 +35,17 @@
 A simulation involves mimicking the screening process for a systematic review of a human in interaction with an Active learning model (i.e., a combination of a feature extractor, classifier,
 balancing method, and a query strategy). The simulation reenacts the screening process as if a researcher were using active learning. The performance of one or multiple model(s) can then be
 measured by performance metrics, such as the Work Saved over Sampling, recall at a given point in the screening process, or the average time to discover a relevant record.
 
 Using Makita templates, different study structures can be generated to fit the needs of your very own study. If your study requires a unique template, you can create a new one and use it
 instead.
 
-With [ASReview LAB](https://github.com/asreview/asreview), you can [simulate](https://asreview.readthedocs.io/en/latest/simulation_overview.html#overview) with the [web
+With [ASReview LAB](https://github.com/asreview/asreview), you can [simulate]( https://asreview.readthedocs.io/en/latest/simulation_overview.html#overview) with the [web
 interface](https://asreview.readthedocs.io/en/latest/simulation_overview.html#simulating-with-asreview-lab), the [Python API](https://asreview.readthedocs.io/en/latest/simulation_api_example.html), or
-the [Command Line Interface (CLI)](https://asreview.readthedocs.io/en/latest/simulation_cli.html). Makita makes use of the CLI.
+the [Command Line Interface (CLI)]( https://asreview.readthedocs.io/en/latest/simulation_cli.html). Makita makes use of the CLI.
 
 What Makita does:
 
 - Setting up a workflow for running a large-scale simulation study
 - Preparing a Github repository
 - Automating the many lines of code needed
 - Creating a batch script for running the simulation study with just one line of code
@@ -58,29 +58,23 @@
 - Being a black-box
 - Writing your paper
 
 For a tutorial on using Makita we refer to the [Exercise on Using the ASReview Simulation Mode](https://github.com/asreview/asreview-academy/blob/main/introducing-simulation-mode/README.md).
 
 ## Installation
 
-### Prerequisites:
+Install the Makita extension with pip:
 
-```
-Requires Python 3.8 or higher.
-```
-
-### Install the Makita extension with pip:
-
-```bash
+``` bash
 pip install asreview-makita
 ```
 
-### For upgrading, use:
+For upgrading, use:
 
-```bash
+``` bash
 pip install --upgrade asreview-makita
 ```
 
 After installing the extension, ASReview should automatically detect Makita. If installed correctly, `asreview --help` should list Makita as an option.
 
 ## Getting started
 
@@ -149,15 +143,15 @@
   -s DATA_FOLDER                            Dataset folder
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
-  --skip_wordclouds                         Disables the generation of wordclouds.
+  --no_wordclouds                           Disables the generation of wordclouds.
   --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
@@ -177,15 +171,15 @@
   -s DATA_FOLDER                            Dataset folder
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_priors N_PRIORS                       Number of priors.                               Default: 10.
-  --skip_wordclouds                         Disables the generation of wordclouds.
+  --no_wordclouds                           Disables the generation of wordclouds.
   --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
@@ -205,22 +199,22 @@
   -s DATA_FOLDER                            Dataset folder
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
-  --skip_wordclouds                         Disables the generation of wordclouds.
+  --no_wordclouds                           Disables the generation of wordclouds.
   --overwrite                               Automatically accepts all overwrite requests.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
   --classifiers CLASSIFIERS                 Classifiers to use                              Default: ['logistic', 'nb', 'rf', 'svm']
   --feature_extractors FEATURE_EXTRACTOR    Feature extractors to use                       Default: ['doc2vec', 'sbert', 'tfidf']
   --query_strategies QUERY_STRATEGY         Query strategies to use                         Default: ['max']
-  --balance_strategies BALANCE_STRATEGY     Balance strategies to use                       Default: ['double']
+  --balance_strategies BALANCE_STRATEGY   Balance strategies to use                       Default: ['double']
   --impossible_models IMPOSSIBLE_MODELS     Model combinations to exclude                   Default: ['nb,doc2vec', 'nb,sbert']
 ```
 
 If you want to specify certain combinations of classifiers and feature
 extractors that should and should not be used, you can use the `--classifiers`,
 `--feature_extractors`, `--query_strategies`, `--balance_strategies` and `--impossible_models` option. For instance, if you
 want to exclude the combinations of `nb` with `doc2vec` and `logistic` with
@@ -241,31 +235,31 @@
    structure `template_*.txt.template`. For the ARFI example, the template is
    [template_arfi.txt.template](https://github.com/asreview/asreview-makita/blob/main/asreviewcontrib/makita/templates/template_arfi.txt.template).
 3. Save the downloaded template somewhere on your computer. The template is a so-called "Jinja" template. The template consists of [ASReview command line
    commands](https://asreview.readthedocs.io/en/latest/API/cli.html) combined with jinja syntax. The Jinja syntax is very intuitive. See this
    [Cheatsheet](https://cheatography.com/skalavala/cheat-sheets/jinja/).
 4. Edit the Jinja template to your needs.
 5. Run the custom template with the command line option `--template PATH_TO_MY_TEMPLATE.txt.template`. For the ARFI example, this would be `asreview makita template arfi --template
-PATH_TO_MY_TEMPLATE.txt.template`. Please keep in mind that you follow the usual steps for running a template.
+   PATH_TO_MY_TEMPLATE.txt.template`. Please keep in mind that you follow the usual steps for running a template.
 6. A `jobs.sh` file should be in the your folder.
 
 Please contribute your templates back to the project by making a Pull Request. Then, we can integrate it in the core of the makita package.
 
 ### Add and use scripts
 
 Makita can add scripts to your repository. The scripts are mainly pre- and postprocessing scripts. These scripts are not (yet) available in any existing ASReview software. Therefore, they can be added manually
 with `asreview makita add-script NAME_OF_SCRIPT`.
 
-For example, the results from _ASReview datatools_ are merged via the script `merge_descriptives.py` (or `merge_metrics.py` for _ASReview insights_), using:
+For example, the results from *ASReview datatools* are merged via the script `merge_descriptives.py` (or `merge_metrics.py` for *ASReview insights*), using:
 
 1. Collect statistics (with template)
-2. Run `asreview makita add-script merge_descriptives.py`
+2. Run  `asreview makita add-script merge_descriptives.py`
 3. Run `python scripts/merge_descriptives.py`
 
-Use `-s` (source) and `-o` (output) to tweak paths.
+Use `-s`  (source) and `-o` (output) to tweak paths.
 
 Some scripts are added automatically to the folder, as they are part of the
 template. For example, the `get_plot.py` script is added to the generated folder
 when using any template, as it is used to generate the plots.
 
 Still, `get_plot.py` can be used on its own, as it is a standalone script. To use it,
 use `-s` (source) and `-o` (output) to tweak paths.
```

### Comparing `asreview_makita-0.9/README.md` & `asreview_makita-0.9rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 A simulation involves mimicking the screening process for a systematic review of a human in interaction with an Active learning model (i.e., a combination of a feature extractor, classifier,
 balancing method, and a query strategy). The simulation reenacts the screening process as if a researcher were using active learning. The performance of one or multiple model(s) can then be
 measured by performance metrics, such as the Work Saved over Sampling, recall at a given point in the screening process, or the average time to discover a relevant record.
 
 Using Makita templates, different study structures can be generated to fit the needs of your very own study. If your study requires a unique template, you can create a new one and use it
 instead.
 
-With [ASReview LAB](https://github.com/asreview/asreview), you can [simulate](https://asreview.readthedocs.io/en/latest/simulation_overview.html#overview) with the [web
+With [ASReview LAB](https://github.com/asreview/asreview), you can [simulate]( https://asreview.readthedocs.io/en/latest/simulation_overview.html#overview) with the [web
 interface](https://asreview.readthedocs.io/en/latest/simulation_overview.html#simulating-with-asreview-lab), the [Python API](https://asreview.readthedocs.io/en/latest/simulation_api_example.html), or
-the [Command Line Interface (CLI)](https://asreview.readthedocs.io/en/latest/simulation_cli.html). Makita makes use of the CLI.
+the [Command Line Interface (CLI)]( https://asreview.readthedocs.io/en/latest/simulation_cli.html). Makita makes use of the CLI.
 
 What Makita does:
 
 - Setting up a workflow for running a large-scale simulation study
 - Preparing a Github repository
 - Automating the many lines of code needed
 - Creating a batch script for running the simulation study with just one line of code
@@ -31,29 +31,23 @@
 - Being a black-box
 - Writing your paper
 
 For a tutorial on using Makita we refer to the [Exercise on Using the ASReview Simulation Mode](https://github.com/asreview/asreview-academy/blob/main/introducing-simulation-mode/README.md).
 
 ## Installation
 
-### Prerequisites:
+Install the Makita extension with pip:
 
-```
-Requires Python 3.8 or higher.
-```
-
-### Install the Makita extension with pip:
-
-```bash
+``` bash
 pip install asreview-makita
 ```
 
-### For upgrading, use:
+For upgrading, use:
 
-```bash
+``` bash
 pip install --upgrade asreview-makita
 ```
 
 After installing the extension, ASReview should automatically detect Makita. If installed correctly, `asreview --help` should list Makita as an option.
 
 ## Getting started
 
@@ -122,15 +116,15 @@
   -s DATA_FOLDER                            Dataset folder
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
-  --skip_wordclouds                         Disables the generation of wordclouds.
+  --no_wordclouds                           Disables the generation of wordclouds.
   --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
@@ -150,15 +144,15 @@
   -s DATA_FOLDER                            Dataset folder
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_priors N_PRIORS                       Number of priors.                               Default: 10.
-  --skip_wordclouds                         Disables the generation of wordclouds.
+  --no_wordclouds                           Disables the generation of wordclouds.
   --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
@@ -178,22 +172,22 @@
   -s DATA_FOLDER                            Dataset folder
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
-  --skip_wordclouds                         Disables the generation of wordclouds.
+  --no_wordclouds                           Disables the generation of wordclouds.
   --overwrite                               Automatically accepts all overwrite requests.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
   --classifiers CLASSIFIERS                 Classifiers to use                              Default: ['logistic', 'nb', 'rf', 'svm']
   --feature_extractors FEATURE_EXTRACTOR    Feature extractors to use                       Default: ['doc2vec', 'sbert', 'tfidf']
   --query_strategies QUERY_STRATEGY         Query strategies to use                         Default: ['max']
-  --balance_strategies BALANCE_STRATEGY     Balance strategies to use                       Default: ['double']
+  --balance_strategies BALANCE_STRATEGY   Balance strategies to use                       Default: ['double']
   --impossible_models IMPOSSIBLE_MODELS     Model combinations to exclude                   Default: ['nb,doc2vec', 'nb,sbert']
 ```
 
 If you want to specify certain combinations of classifiers and feature
 extractors that should and should not be used, you can use the `--classifiers`,
 `--feature_extractors`, `--query_strategies`, `--balance_strategies` and `--impossible_models` option. For instance, if you
 want to exclude the combinations of `nb` with `doc2vec` and `logistic` with
@@ -214,31 +208,31 @@
    structure `template_*.txt.template`. For the ARFI example, the template is
    [template_arfi.txt.template](https://github.com/asreview/asreview-makita/blob/main/asreviewcontrib/makita/templates/template_arfi.txt.template).
 3. Save the downloaded template somewhere on your computer. The template is a so-called "Jinja" template. The template consists of [ASReview command line
    commands](https://asreview.readthedocs.io/en/latest/API/cli.html) combined with jinja syntax. The Jinja syntax is very intuitive. See this
    [Cheatsheet](https://cheatography.com/skalavala/cheat-sheets/jinja/).
 4. Edit the Jinja template to your needs.
 5. Run the custom template with the command line option `--template PATH_TO_MY_TEMPLATE.txt.template`. For the ARFI example, this would be `asreview makita template arfi --template
-PATH_TO_MY_TEMPLATE.txt.template`. Please keep in mind that you follow the usual steps for running a template.
+   PATH_TO_MY_TEMPLATE.txt.template`. Please keep in mind that you follow the usual steps for running a template.
 6. A `jobs.sh` file should be in the your folder.
 
 Please contribute your templates back to the project by making a Pull Request. Then, we can integrate it in the core of the makita package.
 
 ### Add and use scripts
 
 Makita can add scripts to your repository. The scripts are mainly pre- and postprocessing scripts. These scripts are not (yet) available in any existing ASReview software. Therefore, they can be added manually
 with `asreview makita add-script NAME_OF_SCRIPT`.
 
-For example, the results from _ASReview datatools_ are merged via the script `merge_descriptives.py` (or `merge_metrics.py` for _ASReview insights_), using:
+For example, the results from *ASReview datatools* are merged via the script `merge_descriptives.py` (or `merge_metrics.py` for *ASReview insights*), using:
 
 1. Collect statistics (with template)
-2. Run `asreview makita add-script merge_descriptives.py`
+2. Run  `asreview makita add-script merge_descriptives.py`
 3. Run `python scripts/merge_descriptives.py`
 
-Use `-s` (source) and `-o` (output) to tweak paths.
+Use `-s`  (source) and `-o` (output) to tweak paths.
 
 Some scripts are added automatically to the folder, as they are part of the
 template. For example, the `get_plot.py` script is added to the generated folder
 when using any template, as it is used to generate the plots.
 
 Still, `get_plot.py` can be used on its own, as it is a standalone script. To use it,
 use `-s` (source) and `-o` (output) to tweak paths.
```

### Comparing `asreview_makita-0.9/asreview_makita.egg-info/PKG-INFO` & `asreview_makita-0.9rc1/asreview_makita.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asreview-makita
-Version: 0.9
+Version: 0.9rc1
 Summary: Makita workflow tool for the ASReview project
 Author-email: ASReview LAB developers <asreview@uu.nl>
 License: MIT
 Project-URL: homepage, https://asreview.ai
 Project-URL: repository, https://github.com/asreview/asreview-makita
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -35,17 +35,17 @@
 A simulation involves mimicking the screening process for a systematic review of a human in interaction with an Active learning model (i.e., a combination of a feature extractor, classifier,
 balancing method, and a query strategy). The simulation reenacts the screening process as if a researcher were using active learning. The performance of one or multiple model(s) can then be
 measured by performance metrics, such as the Work Saved over Sampling, recall at a given point in the screening process, or the average time to discover a relevant record.
 
 Using Makita templates, different study structures can be generated to fit the needs of your very own study. If your study requires a unique template, you can create a new one and use it
 instead.
 
-With [ASReview LAB](https://github.com/asreview/asreview), you can [simulate](https://asreview.readthedocs.io/en/latest/simulation_overview.html#overview) with the [web
+With [ASReview LAB](https://github.com/asreview/asreview), you can [simulate]( https://asreview.readthedocs.io/en/latest/simulation_overview.html#overview) with the [web
 interface](https://asreview.readthedocs.io/en/latest/simulation_overview.html#simulating-with-asreview-lab), the [Python API](https://asreview.readthedocs.io/en/latest/simulation_api_example.html), or
-the [Command Line Interface (CLI)](https://asreview.readthedocs.io/en/latest/simulation_cli.html). Makita makes use of the CLI.
+the [Command Line Interface (CLI)]( https://asreview.readthedocs.io/en/latest/simulation_cli.html). Makita makes use of the CLI.
 
 What Makita does:
 
 - Setting up a workflow for running a large-scale simulation study
 - Preparing a Github repository
 - Automating the many lines of code needed
 - Creating a batch script for running the simulation study with just one line of code
@@ -58,29 +58,23 @@
 - Being a black-box
 - Writing your paper
 
 For a tutorial on using Makita we refer to the [Exercise on Using the ASReview Simulation Mode](https://github.com/asreview/asreview-academy/blob/main/introducing-simulation-mode/README.md).
 
 ## Installation
 
-### Prerequisites:
+Install the Makita extension with pip:
 
-```
-Requires Python 3.8 or higher.
-```
-
-### Install the Makita extension with pip:
-
-```bash
+``` bash
 pip install asreview-makita
 ```
 
-### For upgrading, use:
+For upgrading, use:
 
-```bash
+``` bash
 pip install --upgrade asreview-makita
 ```
 
 After installing the extension, ASReview should automatically detect Makita. If installed correctly, `asreview --help` should list Makita as an option.
 
 ## Getting started
 
@@ -149,15 +143,15 @@
   -s DATA_FOLDER                            Dataset folder
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
-  --skip_wordclouds                         Disables the generation of wordclouds.
+  --no_wordclouds                           Disables the generation of wordclouds.
   --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
@@ -177,15 +171,15 @@
   -s DATA_FOLDER                            Dataset folder
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_priors N_PRIORS                       Number of priors.                               Default: 10.
-  --skip_wordclouds                         Disables the generation of wordclouds.
+  --no_wordclouds                           Disables the generation of wordclouds.
   --overwrite                               Automatically accepts all overwrite requests.
   --classifier CLASSIFIER                   Classifier to use.                              Default: nb.
   --feature_extractor FEATURE_EXTRACTOR     Feature_extractor to use.                       Default: tfidf.
   --query_strategy QUERY_STRATEGY           Query strategy to use.                          Default: max.
   --balance_strategy BALANCE_STRATEGY       Balance strategy to use.                        Default: double.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
@@ -205,22 +199,22 @@
   -s DATA_FOLDER                            Dataset folder
   -o OUTPUT_FOLDER                          Output folder
   --init_seed INIT_SEED                     Seed of the priors.                             Seed is set to 535 by default.
   --model_seed MODEL_SEED                   Seed of the models.                             Seed is set to 165 by default.
   --template TEMPLATE                       Overwrite template with template file path.
   --platform PLATFORM                       Platform to run jobs: Windows, Darwin, Linux.   Default: the system of rendering templates.
   --n_runs N_RUNS                           Number of runs.                                 Default: 1.
-  --skip_wordclouds                         Disables the generation of wordclouds.
+  --no_wordclouds                           Disables the generation of wordclouds.
   --overwrite                               Automatically accepts all overwrite requests.
   --instances_per_query INSTANCES_PER_QUERY Number of instances per query.                  Default: 1.
   --stop_if STOP_IF                         The number of label actions to simulate.        Default 'min' will stop simulating when all relevant records are found.
   --classifiers CLASSIFIERS                 Classifiers to use                              Default: ['logistic', 'nb', 'rf', 'svm']
   --feature_extractors FEATURE_EXTRACTOR    Feature extractors to use                       Default: ['doc2vec', 'sbert', 'tfidf']
   --query_strategies QUERY_STRATEGY         Query strategies to use                         Default: ['max']
-  --balance_strategies BALANCE_STRATEGY     Balance strategies to use                       Default: ['double']
+  --balance_strategies BALANCE_STRATEGY   Balance strategies to use                       Default: ['double']
   --impossible_models IMPOSSIBLE_MODELS     Model combinations to exclude                   Default: ['nb,doc2vec', 'nb,sbert']
 ```
 
 If you want to specify certain combinations of classifiers and feature
 extractors that should and should not be used, you can use the `--classifiers`,
 `--feature_extractors`, `--query_strategies`, `--balance_strategies` and `--impossible_models` option. For instance, if you
 want to exclude the combinations of `nb` with `doc2vec` and `logistic` with
@@ -241,31 +235,31 @@
    structure `template_*.txt.template`. For the ARFI example, the template is
    [template_arfi.txt.template](https://github.com/asreview/asreview-makita/blob/main/asreviewcontrib/makita/templates/template_arfi.txt.template).
 3. Save the downloaded template somewhere on your computer. The template is a so-called "Jinja" template. The template consists of [ASReview command line
    commands](https://asreview.readthedocs.io/en/latest/API/cli.html) combined with jinja syntax. The Jinja syntax is very intuitive. See this
    [Cheatsheet](https://cheatography.com/skalavala/cheat-sheets/jinja/).
 4. Edit the Jinja template to your needs.
 5. Run the custom template with the command line option `--template PATH_TO_MY_TEMPLATE.txt.template`. For the ARFI example, this would be `asreview makita template arfi --template
-PATH_TO_MY_TEMPLATE.txt.template`. Please keep in mind that you follow the usual steps for running a template.
+   PATH_TO_MY_TEMPLATE.txt.template`. Please keep in mind that you follow the usual steps for running a template.
 6. A `jobs.sh` file should be in the your folder.
 
 Please contribute your templates back to the project by making a Pull Request. Then, we can integrate it in the core of the makita package.
 
 ### Add and use scripts
 
 Makita can add scripts to your repository. The scripts are mainly pre- and postprocessing scripts. These scripts are not (yet) available in any existing ASReview software. Therefore, they can be added manually
 with `asreview makita add-script NAME_OF_SCRIPT`.
 
-For example, the results from _ASReview datatools_ are merged via the script `merge_descriptives.py` (or `merge_metrics.py` for _ASReview insights_), using:
+For example, the results from *ASReview datatools* are merged via the script `merge_descriptives.py` (or `merge_metrics.py` for *ASReview insights*), using:
 
 1. Collect statistics (with template)
-2. Run `asreview makita add-script merge_descriptives.py`
+2. Run  `asreview makita add-script merge_descriptives.py`
 3. Run `python scripts/merge_descriptives.py`
 
-Use `-s` (source) and `-o` (output) to tweak paths.
+Use `-s`  (source) and `-o` (output) to tweak paths.
 
 Some scripts are added automatically to the folder, as they are part of the
 template. For example, the `get_plot.py` script is added to the generated folder
 when using any template, as it is used to generate the plots.
 
 Still, `get_plot.py` can be used on its own, as it is a standalone script. To use it,
 use `-s` (source) and `-o` (output) to tweak paths.
```

### Comparing `asreview_makita-0.9/asreview_makita.egg-info/SOURCES.txt` & `asreview_makita-0.9rc1/asreview_makita.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/entrypoint.py` & `asreview_makita-0.9rc1/asreviewcontrib/makita/entrypoint.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/template_arfi.py` & `asreview_makita-0.9rc1/asreviewcontrib/makita/template_arfi.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/template_base.py` & `asreview_makita-0.9rc1/asreviewcontrib/makita/template_base.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/template_basic.py` & `asreview_makita-0.9rc1/asreviewcontrib/makita/template_basic.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/template_multimodel.py` & `asreview_makita-0.9rc1/asreviewcontrib/makita/template_multimodel.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/templates/doc_README.md.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/doc_README.md.template`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/templates/script_get_plot.py.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_get_plot.py.template`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/templates/script_merge_descriptives.py.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_descriptives.py.template`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/templates/script_merge_metrics.py.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_metrics.py.template`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/templates/script_merge_tds.py.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_merge_tds.py.template`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/templates/template_arfi.txt.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_arfi.txt.template`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/templates/template_basic.txt.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_basic.txt.template`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/templates/template_multimodel.txt.template` & `asreview_makita-0.9rc1/asreviewcontrib/makita/templates/template_multimodel.txt.template`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/asreviewcontrib/makita/utils.py` & `asreview_makita-0.9rc1/asreviewcontrib/makita/utils.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/README.md` & `asreview_makita-0.9rc1/examples/README.md`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/arfi_example/README.md` & `asreview_makita-0.9rc1/examples/arfi_example/README.md`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/arfi_example/data/Smid_2020.csv` & `asreview_makita-0.9rc1/examples/arfi_example/data/Smid_2020.csv`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/arfi_example/data/van_de_Schoot_2018.csv` & `asreview_makita-0.9rc1/examples/arfi_example/data/van_de_Schoot_2018.csv`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/arfi_example/jobs.sh` & `asreview_makita-0.9rc1/examples/arfi_example/jobs.sh`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/arfi_example/scripts/get_plot.py` & `asreview_makita-0.9rc1/examples/arfi_example/scripts/get_plot.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/arfi_example/scripts/merge_descriptives.py` & `asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_descriptives.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/arfi_example/scripts/merge_metrics.py` & `asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_metrics.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/arfi_example/scripts/merge_tds.py` & `asreview_makita-0.9rc1/examples/arfi_example/scripts/merge_tds.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/basic_example/README.md` & `asreview_makita-0.9rc1/examples/basic_example/README.md`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/basic_example/data/Smid_2020.csv` & `asreview_makita-0.9rc1/examples/basic_example/data/Smid_2020.csv`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/basic_example/data/van_de_Schoot_2018.csv` & `asreview_makita-0.9rc1/examples/basic_example/data/van_de_Schoot_2018.csv`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/basic_example/jobs.sh` & `asreview_makita-0.9rc1/examples/basic_example/jobs.sh`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/basic_example/scripts/get_plot.py` & `asreview_makita-0.9rc1/examples/basic_example/scripts/get_plot.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/basic_example/scripts/merge_descriptives.py` & `asreview_makita-0.9rc1/examples/basic_example/scripts/merge_descriptives.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/basic_example/scripts/merge_metrics.py` & `asreview_makita-0.9rc1/examples/basic_example/scripts/merge_metrics.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/basic_example/scripts/merge_tds.py` & `asreview_makita-0.9rc1/examples/basic_example/scripts/merge_tds.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/multimodel_example/README.md` & `asreview_makita-0.9rc1/examples/multimodel_example/README.md`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/multimodel_example/data/Smid_2020.csv` & `asreview_makita-0.9rc1/examples/multimodel_example/data/Smid_2020.csv`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/multimodel_example/data/van_de_Schoot_2018.csv` & `asreview_makita-0.9rc1/examples/multimodel_example/data/van_de_Schoot_2018.csv`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/multimodel_example/jobs.sh` & `asreview_makita-0.9rc1/examples/multimodel_example/jobs.sh`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/multimodel_example/scripts/get_plot.py` & `asreview_makita-0.9rc1/examples/multimodel_example/scripts/get_plot.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/multimodel_example/scripts/merge_descriptives.py` & `asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_descriptives.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/multimodel_example/scripts/merge_metrics.py` & `asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_metrics.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/examples/multimodel_example/scripts/merge_tds.py` & `asreview_makita-0.9rc1/examples/multimodel_example/scripts/merge_tds.py`

 * *Files identical despite different names*

### Comparing `asreview_makita-0.9/pyproject.toml` & `asreview_makita-0.9rc1/pyproject.toml`

 * *Files identical despite different names*

