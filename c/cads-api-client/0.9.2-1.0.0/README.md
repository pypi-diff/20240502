# Comparing `tmp/cads-api-client-0.9.2.tar.gz` & `tmp/cads_api_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cads-api-client-0.9.2.tar", last modified: Wed Mar 20 18:16:39 2024, max compression
+gzip compressed data, was "cads_api_client-1.0.0.tar", last modified: Thu May  2 10:11:55 2024, max compression
```

## Comparing `cads-api-client-0.9.2.tar` & `cads_api_client-1.0.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.829143 cads-api-client-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.817142 cads-api-client-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.821143 cads-api-client-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-03-20 18:16:39.829143 cads-api-client-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.821143 cads-api-client-0.9.2/cads_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/legacy_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/cads_api_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.829143 cads-api-client-0.9.2/cads_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 18:16:39.000000 cads-api-client-0.9.2/cads_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/notebooks/cads_api_client_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/notebooks/cads_api_constraints_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/notebooks/cads_api_filters_and_pagination_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/notebooks/cads_api_licences_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 18:16:39.829143 cads-api-client-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:16:39.825142 cads-api-client-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/integration_test_10_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/integration_test_20_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/integration_test_30_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/integration_test_40_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/integration_test_50_legacy_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/test_10_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-03-20 18:16:31.000000 cads-api-client-0.9.2/tests/test_10_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.314057 cads_api_client-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.318057 cads_api_client-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.318057 cads_api_client-1.0.0/cads_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/legacy_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/cads_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.318057 cads_api_client-1.0.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.318057 cads_api_client-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/notebooks/cads_api_client_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/notebooks/cads_api_constraints_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/notebooks/cads_api_filters_and_pagination_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/notebooks/cads_api_licences_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/integration_test_10_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/integration_test_20_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/integration_test_30_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/integration_test_40_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/integration_test_50_legacy_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/test_10_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/test_10_processing.py
```

### Comparing `cads-api-client-0.9.2/.github/workflows/on-push.yml` & `cads_api_client-1.0.0/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/.gitignore` & `cads_api_client-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/.pre-commit-config.yaml` & `cads_api_client-1.0.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-json
   - id: check-yaml
   - id: check-toml
   - id: check-added-large-files
@@ -13,25 +13,25 @@
   - id: mixed-line-ending
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.9
   hooks:
   - id: blackdoc
     additional_dependencies: [black==23.11.0]
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.3.3
+  rev: v0.4.2
   hooks:
   - id: ruff
     args: [--fix, --show-fixes]
   - id: ruff-format
 - repo: https://github.com/executablebooks/mdformat
   rev: 0.7.17
   hooks:
   - id: mdformat
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.12.0
+  rev: v2.13.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --preserve-quotes]
   - id: pretty-format-toml
     args: [--autofix]
 - repo: https://github.com/gitleaks/gitleaks
   rev: v8.18.2
```

### Comparing `cads-api-client-0.9.2/LICENSE` & `cads_api_client-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/Makefile` & `cads_api_client-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/PKG-INFO` & `cads_api_client-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-api-client
-Version: 0.9.2
+Version: 1.0.0
 Summary: CADS API Python client
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -210,20 +210,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: multiurl
 Requires-Dist: requests
+Requires-Dist: typing-extensions
 
 # cads-api-client
 
 CADS API Python client
 
 The `ApiClient` needs the `url` to the API root and a valid API `key` to access protected resources.
 You can also set the `CADS_API_URL` and `CADS_API_KEY` environment variables.
```

### Comparing `cads-api-client-0.9.2/README.md` & `cads_api_client-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/cads_api_client/__init__.py` & `cads_api_client-1.0.0/cads_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/cads_api_client/api_client.py` & `cads_api_client-1.0.0/cads_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/cads_api_client/catalogue.py` & `cads_api_client-1.0.0/cads_api_client/catalogue.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+from __future__ import annotations
+
 import datetime
 from typing import Any, Dict, List, Optional
 
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
+
 import attrs
 import requests
 
 from . import processing
 
 
 @attrs.define
 class Collections(processing.ApiResponse):
     def collection_ids(self) -> List[str]:
         return [collection["id"] for collection in self.json["collections"]]
 
-    def next(self) -> Optional[processing.ApiResponse]:
+    def next(self) -> Optional[Self]:
         return self.from_rel_href(rel="next")
 
-    def prev(self) -> Optional[processing.ApiResponse]:
+    def prev(self) -> Optional[Self]:
         return self.from_rel_href(rel="prev")
 
 
 @attrs.define
 class Collection(processing.ApiResponse):
     headers: Dict[str, Any] = {}
```

### Comparing `cads-api-client-0.9.2/cads_api_client/config.py` & `cads_api_client-1.0.0/cads_api_client/config.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/cads_api_client/legacy_api_client.py` & `cads_api_client-1.0.0/cads_api_client/legacy_api_client.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/cads_api_client/processing.py` & `cads_api_client-1.0.0/cads_api_client/processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 import functools
 import logging
 import os
 import time
 import urllib
 from typing import Any, Dict, List, Optional, Type, TypeVar
 
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
+
 import attrs
 import multiurl
 import requests
 
 T_ApiResponse = TypeVar("T_ApiResponse", bound="ApiResponse")
 
 logger = logging.getLogger(__name__)
@@ -68,14 +73,16 @@
     def log_messages(self) -> None:
         messages = (
             self.json.get("metadata", {}).get("datasetMetadata", {}).get("messages", [])
         )
         for message in messages:
             if not (content := message.get("content")):
                 continue
+            if date := message.get("date"):
+                content = f"[{date}] {content}"
             severity = message.get("severity", "notset").upper()
             level = logging.getLevelName(severity)
             logger.log(level if isinstance(level, int) else 20, content)
 
     def get_links(self, rel: Optional[str] = None) -> List[Dict[str, str]]:
         links = []
         for link in self.json.get("links", []):
@@ -85,15 +92,15 @@
 
     def get_link_href(self, **kwargs: str) -> str:
         links = self.get_links(**kwargs)
         if len(links) != 1:
             raise RuntimeError(f"link not found or not unique {kwargs}")
         return links[0]["href"]
 
-    def from_rel_href(self, rel: str) -> Optional[ApiResponse]:
+    def from_rel_href(self, rel: str) -> Optional[Self]:
         rels = self.get_links(rel=rel)
         assert len(rels) <= 1
         if len(rels) == 1:
             out = self.from_request(
                 "get", rels[0]["href"], headers=self.headers, session=self.session
             )
         else:
@@ -156,35 +163,54 @@
         headers: Dict[str, Any] = {},
         session: requests.Session = requests.api,  # type: ignore
     ):
         self.url = url
         self.sleep_max = sleep_max
         self.headers = headers
         self.session = session
+        self.log_start_time = None
+
+    def log_metadata(self, metadata: dict[str, Any]) -> None:
+        logs = metadata.get("log", [])
+        for self.log_start_time, message in sorted(logs):
+            level = 20
+            for severity in ("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"):
+                if message.startswith(severity):
+                    level = logging.getLevelName(severity)
+                    message = message.replace(severity, "", 1).lstrip(":").lstrip()
+                    break
+            logger.log(level, message)
 
     @functools.cached_property
     def request_uid(self) -> str:
         return self.url.rpartition("/")[2]
 
-    @property
-    def status(self) -> str:
+    def _get_status(self, robust: bool, **retry_options: Any) -> str:
         # TODO: cache responses for a timeout (possibly reported nby the server)
-        requests_response = self.session.get(self.url, headers=self.headers)
+        get = self.session.get
+        if robust:
+            get = multiurl.robust(get, **retry_options)
+
+        params = {"log": True}
+        if self.log_start_time:
+            params["logStartTime"] = self.log_start_time
+
+        logger.debug(f"GET {self.url}")
+        requests_response = get(url=self.url, headers=self.headers, params=params)
         requests_response.raise_for_status()
         json = requests_response.json()
-        return json["status"]  # type: ignore
+        self.log_metadata(json.get("metadata", {}))
+        return str(json["status"])
+
+    @property
+    def status(self) -> str:
+        return self._get_status(robust=False)
 
     def _robust_status(self, retry_options: Dict[str, Any] = {}) -> str:
-        # TODO: cache responses for a timeout (possibly reported nby the server)
-        requests_response = multiurl.robust(self.session.get, **retry_options)(
-            self.url, headers=self.headers
-        )
-        requests_response.raise_for_status()
-        json = requests_response.json()
-        return json["status"]  # type: ignore
+        return self._get_status(robust=True, **retry_options)
 
     def wait_on_result(self, retry_options: Dict[str, Any] = {}) -> None:
         sleep = 1.0
         status = None
         while True:
             if status != (status := self._robust_status(retry_options=retry_options)):
                 logger.info(f"status has been updated to {status}")
```

### Comparing `cads-api-client-0.9.2/cads_api_client/profile.py` & `cads_api_client-1.0.0/cads_api_client/profile.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/cads_api_client.egg-info/PKG-INFO` & `cads_api_client-1.0.0/cads_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-api-client
-Version: 0.9.2
+Version: 1.0.0
 Summary: CADS API Python client
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -210,20 +210,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: multiurl
 Requires-Dist: requests
+Requires-Dist: typing-extensions
 
 # cads-api-client
 
 CADS API Python client
 
 The `ApiClient` needs the `url` to the API root and a valid API `key` to access protected resources.
 You can also set the `CADS_API_URL` and `CADS_API_KEY` environment variables.
```

### Comparing `cads-api-client-0.9.2/cads_api_client.egg-info/SOURCES.txt` & `cads_api_client-1.0.0/cads_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/docs/Makefile` & `cads_api_client-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/docs/conf.py` & `cads_api_client-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/docs/make.bat` & `cads_api_client-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/notebooks/cads_api_client_test.ipynb` & `cads_api_client-1.0.0/notebooks/cads_api_client_test.ipynb`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/notebooks/cads_api_constraints_test.ipynb` & `cads_api_client-1.0.0/notebooks/cads_api_constraints_test.ipynb`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/notebooks/cads_api_filters_and_pagination_tests.ipynb` & `cads_api_client-1.0.0/notebooks/cads_api_filters_and_pagination_tests.ipynb`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/notebooks/cads_api_licences_tests.ipynb` & `cads_api_client-1.0.0/notebooks/cads_api_licences_tests.ipynb`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/pyproject.toml` & `cads_api_client-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [build-system]
-requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
+build-backend = "setuptools.build_meta"
+requires = ["setuptools>=64", "setuptools_scm>=8"]
 
 [project]
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering"
 ]
-dependencies = ["attrs", "multiurl", "requests"]
+dependencies = ["attrs", "multiurl", "requests", "typing-extensions"]
 description = "CADS API Python client"
 dynamic = ["version"]
 license = {file = "LICENSE"}
 name = "cads-api-client"
 readme = "README.md"
 
 [tool.coverage.run]
```

### Comparing `cads-api-client-0.9.2/tests/conftest.py` & `cads_api_client-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/tests/integration_test_10_catalogue.py` & `cads_api_client-1.0.0/tests/integration_test_10_catalogue.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from cads_api_client import catalogue
 
 
 def test_collections(api_root_url: str) -> None:
     cat = catalogue.Catalogue(f"{api_root_url}/catalogue")
 
-    res = cat.collections()
+    res: catalogue.Collections | None = cat.collections()
 
     assert isinstance(res, catalogue.Collections)
     assert "collections" in res.json
     assert isinstance(res.json["collections"], list)
     assert "links" in res.json
     assert isinstance(res.json["links"], list)
 
-    expected_collection_id = "reanalysis-era5-single-levels"
+    collection_ids = res.collection_ids()
+    while len(collection_ids) != res.json["numberMatched"]:
+        res = res.next()
+        assert res is not None
+        collection_ids.extend(res.collection_ids())
 
-    assert expected_collection_id in res.collection_ids()
+    expected_collection_id = "reanalysis-era5-single-levels"
+    assert expected_collection_id in collection_ids
 
 
 def test_collections_limit(api_root_url: str) -> None:
     cat = catalogue.Catalogue(f"{api_root_url}/catalogue")
     collections = cat.collections(params={"limit": 1})
 
     res = collections.next()
```

### Comparing `cads-api-client-0.9.2/tests/integration_test_20_processing.py` & `cads_api_client-1.0.0/tests/integration_test_20_processing.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/tests/integration_test_30_remote.py` & `cads_api_client-1.0.0/tests/integration_test_30_remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     headers = {"PRIVATE-TOKEN": api_key}
 
     cat = catalogue.Catalogue(f"{api_root_url}/catalogue", headers=headers)
     dataset = cat.collection(collection_id)
     target = str(tmpdir.join("era5-complete.grib"))
 
     res = dataset.retrieve(
-        levelist=1,
+        levelist="1",
         dataset="reanalysis",
         time="00:00:00",
         param="155",
         date="1940-01-01",
         expect="any",
         levtype="pl",
         number="all",
```

### Comparing `cads-api-client-0.9.2/tests/integration_test_40_api_client.py` & `cads_api_client-1.0.0/tests/integration_test_40_api_client.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/tests/integration_test_50_legacy_api_client.py` & `cads_api_client-1.0.0/tests/integration_test_50_legacy_api_client.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/tests/test_10_config.py` & `cads_api_client-1.0.0/tests/test_10_config.py`

 * *Files identical despite different names*

### Comparing `cads-api-client-0.9.2/tests/test_10_processing.py` & `cads_api_client-1.0.0/tests/test_10_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,20 +150,20 @@
     },
     "metadata": {
         "datasetMetadata": {
             "messages": [
                 {
                     "date": "2023-12-12T13:00:00",
                     "severity": "warning",
-                    "content": "This is a warning",
+                    "content": "This is a warning message",
                 },
                 {
-                    "date": "2023-12-12T13:00:00",
+                    "date": "2023-12-12T14:00:00",
                     "severity": "success",
-                    "content": "This is a success",
+                    "content": "This is a success message",
                 },
             ]
         }
     },
 }
 
 JOB_RUNNING_JSON = {
@@ -207,14 +207,20 @@
         {
             "href": f"{JOB_SUCCESSFUL_URL}",
             "rel": "monitor",
             "type": "application/json",
             "title": "job status info",
         },
     ],
+    "metadata": {
+        "log": [
+            ["2024-02-09T09:14:47.811223", "This is a log"],
+            ["2024-02-09T09:14:50.811223", "WARNING: This is a warning log"],
+        ]
+    },
 }
 
 RESULT_SUCCESSFUL_JSON = {
     "asset": {
         "value": {
             "type": "application/netcdf",
             "href": "./e7d452a747061ab880887d88814bfb0c27593a73cb7736d2dc340852",
@@ -335,14 +341,30 @@
 def test_log_messages(caplog: pytest.LogCaptureFixture) -> None:
     responses_add()
 
     catalogue = cads_api_client.Catalogue(CATALOGUE_URL)
     collection = catalogue.collection(COLLECTION_ID)
 
     with caplog.at_level(logging.DEBUG, logger="cads_api_client.processing"):
-        process = collection.retrieve_process()
-        _ = process.execute(inputs={"variable": "temperature", "year": "2022"})
+        remote = collection.submit(variable="temperature", year="2022")
+        remote.wait_on_result()
 
     assert caplog.record_tuples == [
-        ("cads_api_client.processing", 30, "This is a warning"),
-        ("cads_api_client.processing", 20, "This is a success"),
+        (
+            "cads_api_client.processing",
+            30,
+            "[2023-12-12T13:00:00] This is a warning message",
+        ),
+        (
+            "cads_api_client.processing",
+            20,
+            "[2023-12-12T14:00:00] This is a success message",
+        ),
+        (
+            "cads_api_client.processing",
+            10,
+            "GET http://localhost:8080/api/retrieve/v1/jobs/9bfc1362-2832-48e1-a235-359267420bb2",
+        ),
+        ("cads_api_client.processing", 20, "This is a log"),
+        ("cads_api_client.processing", 30, "This is a warning log"),
+        ("cads_api_client.processing", 20, "status has been updated to successful"),
     ]
```

