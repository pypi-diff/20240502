# Comparing `tmp/aind_exaspim_pipeline_utils-0.8.1.tar.gz` & `tmp/aind_exaspim_pipeline_utils-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_exaspim_pipeline_utils-0.8.1.tar", last modified: Wed Apr 24 23:09:30 2024, max compression
+gzip compressed data, was "aind_exaspim_pipeline_utils-0.8.2.tar", last modified: Wed May  1 22:36:54 2024, max compression
```

## Comparing `aind_exaspim_pipeline_utils-0.8.1.tar` & `aind_exaspim_pipeline_utils-0.8.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.106714 aind_exaspim_pipeline_utils-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.090714 aind_exaspim_pipeline_utils-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.094714 aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.094714 aind_exaspim_pipeline_utils-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-24 23:09:30.106714 aind_exaspim_pipeline_utils-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.098713 aind_exaspim_pipeline_utils-0.8.1/capsule_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/capsule_scripts/imagej_postInstall
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/capsule_scripts/imagej_run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/capsule_scripts/n5tozarr_postInstall
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/capsule_scripts/n5tozarr_run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.098713 aind_exaspim_pipeline_utils-0.8.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.098713 aind_exaspim_pipeline_utils-0.8.1/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.098713 aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 23:09:30.106714 aind_exaspim_pipeline_utils-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.094714 aind_exaspim_pipeline_utils-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.098713 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-24 23:09:20.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23467 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/exaspim_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/imagej_macros.py
--rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/imagej_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/java_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/n5tozarr/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28034 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/trigger/capsule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/src/aind_trigger_codeocean/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_trigger_codeocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51638 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_trigger_codeocean/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/tests/test_capsule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/tests/test_imagej_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/tests/test_n5tozarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.759838 aind_exaspim_pipeline_utils-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.743838 aind_exaspim_pipeline_utils-0.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.747838 aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.747838 aind_exaspim_pipeline_utils-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-01 22:36:54.759838 aind_exaspim_pipeline_utils-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/capsule_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/capsule_scripts/imagej_postInstall
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/capsule_scripts/imagej_run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/capsule_scripts/n5tozarr_postInstall
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/capsule_scripts/n5tozarr_run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 22:36:54.759838 aind_exaspim_pipeline_utils-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.747838 aind_exaspim_pipeline_utils-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-01 22:36:45.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23467 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/exaspim_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/imagej_macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/imagej_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/java_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/n5tozarr/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.755838 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.755838 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28034 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/trigger/capsule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.755838 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.755838 aind_exaspim_pipeline_utils-0.8.2/src/aind_trigger_codeocean/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_trigger_codeocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51638 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_trigger_codeocean/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.755838 aind_exaspim_pipeline_utils-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/tests/test_capsule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/tests/test_imagej_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/tests/test_n5tozarr.py
```

### Comparing `aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/user-story.md` & `aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/.github/workflows/lint_and_test.yml` & `aind_exaspim_pipeline_utils-0.8.2/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/.github/workflows/tag_and_publish.yml` & `aind_exaspim_pipeline_utils-0.8.2/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/.gitignore` & `aind_exaspim_pipeline_utils-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/LICENSE` & `aind_exaspim_pipeline_utils-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/PKG-INFO` & `aind_exaspim_pipeline_utils-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_exaspim_pipeline_utils
-Version: 0.8.1
+Version: 0.8.2
 Summary: AIND exaSPIM pipeline utilities.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_exaspim_pipeline_utils-0.8.1/README.md` & `aind_exaspim_pipeline_utils-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/doc/Makefile` & `aind_exaspim_pipeline_utils-0.8.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/doc/make.bat` & `aind_exaspim_pipeline_utils-0.8.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/dark-logo.svg` & `aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/favicon.ico` & `aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/light-logo.svg` & `aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/doc/source/conf.py` & `aind_exaspim_pipeline_utils-0.8.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/pyproject.toml` & `aind_exaspim_pipeline_utils-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/exaspim_manifest.py` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/exaspim_manifest.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/imagej_macros.py` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/imagej_macros.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/imagej_wrapper.py` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/imagej_wrapper.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/java_utils.py` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/java_utils.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     LOGGER.debug("Initialize source N5 store")
     n5s = zarr.n5.N5FSStore(input_uri)
     zg = zarr.open(store=n5s, mode="r")
     LOGGER.debug("Initialize dask array from N5 source")
     arr = dask.array.from_array(zg["s0"], chunks=zg["s0"].chunks)
     arr = chunk_utils.ensure_array_5d(arr)
     LOGGER.debug("Re-chunk dask array to desired output chunk size.")
-    arr = arr.rechunk((1, 1, 256, 256, 256))
+    arr = arr.rechunk((1, 1, 128, 256, 256))
 
     LOGGER.info(f"Input array: {arr}")
     LOGGER.info(f"Input array size: {arr.nbytes / 2 ** 20} MiB")
 
     LOGGER.debug("Initialize target Zarr store")
     output_path = output_uri
     group = zarr.open_group(output_path, mode="a")
@@ -192,15 +192,15 @@
     LOGGER.debug("Initialize source Zarr store")
     zg = zarr.open_group(input_uri, mode="r")
     LOGGER.info("Get dask array from Zarr source for full resolution")
     arrZero = dask.array.from_array(
         zg["0"], chunks=zg["0"].chunks
     )  # For metadata writing we need the full resolution shape
     arrZero = chunk_utils.ensure_array_5d(arrZero)
-    arrZero = arrZero.rechunk((1, 1, 256, 256, 256))
+    arrZero = arrZero.rechunk((1, 1, 128, 256, 256))
 
     LOGGER.info(f"Full resolution array: {arrZero}")
     LOGGER.info(f"Full resolution input array size: {arrZero.nbytes / 2 ** 20} MiB")
 
     LOGGER.debug("Initialize target Zarr store")
     group = zarr.open_group(output_uri, mode="a")
 
@@ -222,15 +222,15 @@
     )
 
     if fromLevel > 1:
         prevLevel = str(fromLevel - 1)
         LOGGER.info("Initialize dask source array from Zarr source level %s", prevLevel)
         arr = dask.array.from_array(zg[prevLevel], chunks=zg[prevLevel].chunks)
         arr = chunk_utils.ensure_array_5d(arr)
-        arr = arr.rechunk((1, 1, 256, 256, 256))
+        arr = arr.rechunk((1, 1, 128, 256, 256))
     else:
         arr = arrZero
 
     del arrZero  # Can be garbage collected if different from arr
 
     block_shape = chunk_utils.ensure_shape_5d(
         io_utils.BlockedArrayWriter.get_block_shape(arr, target_size_mb=1048576)  # 8k**3 blocks of 16bit data
```

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/trigger/capsule.py` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/trigger/capsule.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_exaspim_pipeline_utils
-Version: 0.8.1
+Version: 0.8.2
 Summary: AIND exaSPIM pipeline utilities.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/src/aind_trigger_codeocean/pipelines.py` & `aind_exaspim_pipeline_utils-0.8.2/src/aind_trigger_codeocean/pipelines.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/tests/test_capsule.py` & `aind_exaspim_pipeline_utils-0.8.2/tests/test_capsule.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/tests/test_imagej_wrapper.py` & `aind_exaspim_pipeline_utils-0.8.2/tests/test_imagej_wrapper.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.1/tests/test_n5tozarr.py` & `aind_exaspim_pipeline_utils-0.8.2/tests/test_n5tozarr.py`

 * *Files identical despite different names*

