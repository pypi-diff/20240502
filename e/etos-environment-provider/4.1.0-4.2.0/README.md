# Comparing `tmp/etos_environment_provider-4.1.0.tar.gz` & `tmp/etos_environment_provider-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_environment_provider-4.1.0.tar", last modified: Fri Apr 26 08:02:35 2024, max compression
+gzip compressed data, was "etos_environment_provider-4.2.0.tar", last modified: Thu May  2 11:00:02 2024, max compression
```

## Comparing `etos_environment_provider-4.1.0.tar` & `etos_environment_provider-4.2.0.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.458991 etos_environment_provider-4.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.462991 etos_environment_provider-4.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/.github/workflows/build-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.462991 etos_environment_provider-4.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.458991 etos_environment_provider-4.1.0/manifests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/manifests/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/manifests/base/api/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/api/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/api/service-account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/api/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/manifests/base/worker/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/worker/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/manifests/base/worker/service-account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.458991 etos_environment_provider-4.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/src/environment_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    22823 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/environment_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.466992 etos_environment_provider-4.1.0/src/environment_provider/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/join.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/json_dumps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/log_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/lib/uuid_generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.470991 etos_environment_provider-4.1.0/src/environment_provider/splitter/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/environment_provider/splitter/split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 08:02:35.000000 etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.470991 etos_environment_provider-4.1.0/src/execution_space_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/execution_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/execution_space_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.470991 etos_environment_provider-4.1.0/src/execution_space_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.470991 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/execution_space_provider/utilities/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.474991 etos_environment_provider-4.1.0/src/iut_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/iut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/iut_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.474991 etos_environment_provider-4.1.0/src/iut_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.474991 etos_environment_provider-4.1.0/src/iut_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    12346 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/iut_provider/utilities/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.474991 etos_environment_provider-4.1.0/src/log_area_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/log_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/log_area_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.474991 etos_environment_provider-4.1.0/src/log_area_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.478991 etos_environment_provider-4.1.0/src/log_area_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/src/log_area_provider/utilities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.478991 etos_environment_provider-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.478991 etos_environment_provider-4.1.0/tests/external_execution_space/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_execution_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_execution_space/test_external_execution_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/tests/external_iut/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_iut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24107 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_iut/test_external_iut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/tests/external_log_area/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_log_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/external_log_area/test_external_log_area.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/tests/library/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/library/fake_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/library/fake_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/library/graphql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:35.482992 etos_environment_provider-4.1.0/tests/splitter/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/splitter/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/tercc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tests/test_environment_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-26 08:02:30.000000 etos_environment_provider-4.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.759823 etos_environment_provider-4.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/.github/workflows/build-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.763823 etos_environment_provider-4.2.0/manifests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/manifests/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/manifests/base/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/api/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/api/service-account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/api/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.767823 etos_environment_provider-4.2.0/manifests/base/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/worker/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/manifests/base/worker/service-account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.763823 etos_environment_provider-4.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.771823 etos_environment_provider-4.2.0/src/environment_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23718 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/environment_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.771823 etos_environment_provider-4.2.0/src/environment_provider/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/json_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/log_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/lib/uuid_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.771823 etos_environment_provider-4.2.0/src/environment_provider/splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/environment_provider/splitter/split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 11:00:02.000000 etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.775823 etos_environment_provider-4.2.0/src/execution_space_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/execution_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/execution_space_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.775823 etos_environment_provider-4.2.0/src/execution_space_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.775823 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/execution_space_provider/utilities/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.775823 etos_environment_provider-4.2.0/src/iut_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/iut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/iut_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.775823 etos_environment_provider-4.2.0/src/iut_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/src/iut_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/iut_provider/utilities/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/src/log_area_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/log_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/log_area_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/src/log_area_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/src/log_area_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/src/log_area_provider/utilities/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/tests/external_execution_space/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_execution_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_execution_space/test_external_execution_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/tests/external_iut/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_iut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24107 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_iut/test_external_iut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.779823 etos_environment_provider-4.2.0/tests/external_log_area/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_log_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/external_log_area/test_external_log_area.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/library/fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/library/fake_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/library/graphql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:00:02.783823 etos_environment_provider-4.2.0/tests/splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/splitter/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/tercc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tests/test_environment_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-02 10:59:54.000000 etos_environment_provider-4.2.0/tox.ini
```

### Comparing `etos_environment_provider-4.1.0/.coveragerc` & `etos_environment_provider-4.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/.github/workflows/build-push.yml` & `etos_environment_provider-4.2.0/.github/workflows/build-push.yml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/.github/workflows/main.yml` & `etos_environment_provider-4.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/.gitignore` & `etos_environment_provider-4.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/LICENSE.txt` & `etos_environment_provider-4.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/PKG-INFO` & `etos_environment_provider-4.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_environment_provider
-Version: 4.1.0
+Version: 4.2.0
 Summary: Environment provider for ETOS.
 Home-page: https://github.com/eiffel-community/etos-environment-provider
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
@@ -20,15 +20,18 @@
 Requires-Dist: celery~=5.3
 Requires-Dist: cryptography<43.0.0,>=42.0.4
 Requires-Dist: gevent~=23.7
 Requires-Dist: gunicorn~=19.9
 Requires-Dist: jsontas~=1.3
 Requires-Dist: packageurl-python~=0.11
 Requires-Dist: etcd3gw~=2.3
-Requires-Dist: etos_lib==4.0.0
+Requires-Dist: etos_lib==4.2.0
+Requires-Dist: opentelemetry-api~=1.21
+Requires-Dist: opentelemetry-exporter-otlp~=1.21
+Requires-Dist: opentelemetry-sdk~=1.21
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 =========================
 ETOS Environment Provider
 =========================
```

### Comparing `etos_environment_provider-4.1.0/README.rst` & `etos_environment_provider-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/docs/Makefile` & `etos_environment_provider-4.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/docs/conf.py` & `etos_environment_provider-4.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/manifests/base/api/deployment.yaml` & `etos_environment_provider-4.2.0/manifests/base/api/deployment.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/manifests/base/kustomization.yaml` & `etos_environment_provider-4.2.0/manifests/base/kustomization.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/manifests/base/worker/deployment.yaml` & `etos_environment_provider-4.2.0/manifests/base/worker/deployment.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/setup.cfg` & `etos_environment_provider-4.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,18 @@
 	celery~=5.3
 	cryptography>=42.0.4,<43.0.0
 	gevent~=23.7
 	gunicorn~=19.9
 	jsontas~=1.3
 	packageurl-python~=0.11
 	etcd3gw~=2.3
-	etos_lib==4.0.0
+	etos_lib==4.2.0
+	opentelemetry-api~=1.21
+	opentelemetry-exporter-otlp~=1.21
+	opentelemetry-sdk~=1.21
 python_requires = >=3.8
 
 [options.package_data]
 * = *.json
 
 [options.packages.find]
 where = src
```

### Comparing `etos_environment_provider-4.1.0/setup.py` & `etos_environment_provider-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/__init__.py` & `etos_environment_provider-4.2.0/src/environment_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/environment.py` & `etos_environment_provider-4.2.0/src/environment_provider/environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,25 +16,29 @@
 """Backend for the environment requests."""
 import json
 import traceback
 from typing import Optional, Union
 
 from etos_lib import ETOS
 from jsontas.jsontas import JsonTas
+from opentelemetry import trace
 
 from environment_provider.lib.database import ETCDPath
 from environment_provider.lib.registry import ProviderRegistry
 from execution_space_provider import ExecutionSpaceProvider
 from execution_space_provider.execution_space import ExecutionSpace
 from iut_provider import IutProvider
 from iut_provider.iut import Iut
 from log_area_provider import LogAreaProvider
 from log_area_provider.log_area import LogArea
 
 
+TRACER = trace.get_tracer(__name__)
+
+
 def checkin_provider(
     item: dict, provider: Union[IutProvider, ExecutionSpaceProvider, LogAreaProvider]
 ) -> tuple[bool, Optional[Exception]]:
     """Check in a provider.
 
     :param item: Item to check in.
     :param provider: The provider to use for check in.
@@ -71,29 +75,44 @@
 
     log_area = sub_suite.get("log_area")
     log_area_ruleset = provider_registry.get_log_area_provider_by_id(
         log_area.get("provider_id")
     ).get("log")
 
     failure = None
-    success, exception = checkin_provider(Iut(**iut), IutProvider(etos, jsontas, iut_ruleset))
-    if not success:
-        failure = exception
 
-    success, exception = checkin_provider(
-        LogArea(**log_area), LogAreaProvider(etos, jsontas, log_area_ruleset)
-    )
-    if not success:
-        failure = exception
-    success, exception = checkin_provider(
-        ExecutionSpace(**executor),
-        ExecutionSpaceProvider(etos, jsontas, executor_ruleset),
-    )
-    if not success:
-        failure = exception
+    span_name = "stop_iuts"
+    with TRACER.start_as_current_span(span_name, kind=trace.SpanKind.CLIENT) as span:
+        success, exception = checkin_provider(Iut(**iut), IutProvider(etos, jsontas, iut_ruleset))
+        if not success:
+            span.record_exception(exception)
+            span.set_status(trace.Status(trace.StatusCode.ERROR))
+            failure = exception
+
+    span_name = "stop_log_area"
+    with TRACER.start_as_current_span(span_name, kind=trace.SpanKind.CLIENT) as span:
+        success, exception = checkin_provider(
+            LogArea(**log_area), LogAreaProvider(etos, jsontas, log_area_ruleset)
+        )
+        if not success:
+            span.record_exception(exception)
+            span.set_status(trace.Status(trace.StatusCode.ERROR))
+            failure = exception
+
+    span_name = "stop_execution_space"
+    with TRACER.start_as_current_span(span_name, kind=trace.SpanKind.CLIENT):
+        success, exception = checkin_provider(
+            ExecutionSpace(**executor),
+            ExecutionSpaceProvider(etos, jsontas, executor_ruleset),
+        )
+        if not success:
+            span.record_exception(exception)
+            span.set_status(trace.Status(trace.StatusCode.ERROR))
+            failure = exception
+
     return failure
 
 
 def release_full_environment(etos: ETOS, jsontas: JsonTas, suite_id: str) -> tuple[bool, str]:
     """Release an already requested environment.
 
     :param etos: ETOS library instance.
```

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/environment_provider.py` & `etos_environment_provider-4.2.0/src/environment_provider/environment_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 from tempfile import NamedTemporaryFile
 from threading import Lock
 from typing import Any, Union
 
 from etos_lib.etos import ETOS
 from etos_lib.lib.events import EiffelEnvironmentDefinedEvent
 from etos_lib.logging.logger import FORMAT_CONFIG
+from etos_lib.opentelemetry.semconv import Attributes as SemConvAttributes
 from jsontas.jsontas import JsonTas
+import opentelemetry
+from opentelemetry.trace import SpanKind
 
 from execution_space_provider.execution_space import ExecutionSpace
 from log_area_provider.log_area import LogArea
 
 from .lib.celery import APP
 from .lib.config import Config
 from .lib.database import ETCDPath
@@ -74,14 +77,15 @@
 
         :param suite_id: Suite ID to get an environment for
         :param suite_runner_ids: IDs from the suite runner to correlate sub suites.
         :param copy: Whether or not to copy the etos config. Set to False if not running celery.
         """
         FORMAT_CONFIG.identifier = suite_id
         self.logger.info("Initializing EnvironmentProvider task.")
+        self.tracer = opentelemetry.trace.get_tracer(__name__)
 
         self.etos = ETOS("ETOS Environment Provider", os.getenv("HOSTNAME"), "Environment Provider")
 
         self.suite_id = suite_id
         self.suite_runner_ids = suite_runner_ids
 
         with self.lock:
@@ -410,48 +414,60 @@
             main_suite_id,
             self.environment_provider_config,
         )
         finished = []
         timeout = self.checkout_timeout()
         while time.time() < timeout:
             self.set_total_test_count_and_test_runners(test_runners)
-            # Check out and assign IUTs to test runners.
-            iuts = self.iut_provider.wait_for_and_checkout_iuts(
-                minimum_amount=1,
-                maximum_amount=self.dataset.get(
-                    "maximum_amount", self.etos.config.get("TOTAL_TEST_COUNT")
-                ),
-            )
-            self.splitter.assign_iuts(test_runners, iuts)
+
+            with self.tracer.start_as_current_span("request_iuts", kind=SpanKind.CLIENT) as span:
+                # Check out and assign IUTs to test runners.
+                iuts = self.iut_provider.wait_for_and_checkout_iuts(
+                    minimum_amount=1,
+                    maximum_amount=self.dataset.get(
+                        "maximum_amount", self.etos.config.get("TOTAL_TEST_COUNT")
+                    ),
+                )
+                self.splitter.assign_iuts(test_runners, iuts)
+                span.set_attribute(SemConvAttributes.IUT_DESCRIPTION, str(iuts))
 
             for test_runner in test_runners.keys():
                 self.dataset.add("test_runner", test_runner)
 
                 # No IUTs assigned to test runner
                 if not test_runners[test_runner].get("iuts"):
                     continue
 
                 # Check out an executor and log area for each IUT.
                 for iut, suite in test_runners[test_runner].get("iuts", {}).items():
                     self.dataset.add("iut", iut)
                     self.dataset.add("suite", suite)
-                    suite["executor"] = self.checkout_an_execution_space()
-                    self.dataset.add("executor", suite["executor"])
-                    suite["log_area"] = self.checkout_a_log_area()
+
+                    with self.tracer.start_as_current_span(
+                        "request_execution_space", kind=SpanKind.CLIENT
+                    ) as span:
+                        span.set_attribute(SemConvAttributes.TEST_RUNNER_ID, test_runner)
+                        suite["executor"] = self.checkout_an_execution_space()
+                        self.dataset.add("executor", suite["executor"])
+
+                    with self.tracer.start_as_current_span(
+                        "request_log_area", kind=SpanKind.CLIENT
+                    ) as span:
+                        span.set_attribute(SemConvAttributes.TEST_RUNNER_ID, test_runner)
+                        suite["log_area"] = self.checkout_a_log_area()
 
                 # Split the tests into sub suites
                 self.splitter.split(test_runners[test_runner])
 
                 # Add sub suites to test suite structure and send environment events to the ESR.
                 for iut, suite in test_runners[test_runner].get("iuts", {}).items():
                     sub_suite = test_suite.add(
                         test_runner, iut, suite, test_runners[test_runner]["priority"]
                     )
-                    url = self.upload_sub_suite(sub_suite)
-                    self.send_environment_events(url, sub_suite)
+                    self.send_environment_events(self.upload_sub_suite(sub_suite), sub_suite)
 
                     self.logger.info(
                         "Environment for %r checked out and is ready for use",
                         sub_suite["name"],
                         extra={"user_log": True},
                     )
                 finished.append(test_runner)
```

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/__init__.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/celery.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/celery.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/config.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/config.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/database.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/database.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/encrypt.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/encrypt.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/graphql.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/graphql.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/join.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/join.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/json_dumps.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/json_dumps.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/log_area.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/registry.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/registry.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/test_suite.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/test_suite.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/lib/uuid_generate.py` & `etos_environment_provider-4.2.0/src/environment_provider/lib/uuid_generate.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/splitter/__init__.py` & `etos_environment_provider-4.2.0/src/environment_provider/splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/environment_provider/splitter/split.py` & `etos_environment_provider-4.2.0/src/environment_provider/splitter/split.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/PKG-INFO` & `etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_environment_provider
-Version: 4.1.0
+Version: 4.2.0
 Summary: Environment provider for ETOS.
 Home-page: https://github.com/eiffel-community/etos-environment-provider
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
@@ -20,15 +20,18 @@
 Requires-Dist: celery~=5.3
 Requires-Dist: cryptography<43.0.0,>=42.0.4
 Requires-Dist: gevent~=23.7
 Requires-Dist: gunicorn~=19.9
 Requires-Dist: jsontas~=1.3
 Requires-Dist: packageurl-python~=0.11
 Requires-Dist: etcd3gw~=2.3
-Requires-Dist: etos_lib==4.0.0
+Requires-Dist: etos_lib==4.2.0
+Requires-Dist: opentelemetry-api~=1.21
+Requires-Dist: opentelemetry-exporter-otlp~=1.21
+Requires-Dist: opentelemetry-sdk~=1.21
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 =========================
 ETOS Environment Provider
 =========================
```

### Comparing `etos_environment_provider-4.1.0/src/etos_environment_provider.egg-info/SOURCES.txt` & `etos_environment_provider-4.2.0/src/etos_environment_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/__init__.py` & `etos_environment_provider-4.2.0/src/execution_space_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/exceptions.py` & `etos_environment_provider-4.2.0/src/execution_space_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/execution_space.py` & `etos_environment_provider-4.2.0/src/execution_space_provider/execution_space.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/execution_space_provider.py` & `etos_environment_provider-4.2.0/src/execution_space_provider/execution_space_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/schemas/external_schema.json` & `etos_environment_provider-4.2.0/src/execution_space_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.2.0/src/execution_space_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/__init__.py` & `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/checkin.py` & `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/checkout.py` & `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/external_provider.py` & `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/external_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,19 +11,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """External Execution Space provider."""
 import logging
+import json
 import os
 import time
 from copy import deepcopy
 from json.decoder import JSONDecodeError
 
+import opentelemetry
+from opentelemetry.semconv.trace import SpanAttributes
+from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
+
 import requests
 from etos_lib import ETOS
 from etos_lib.lib.http import Http
 from jsontas.jsontas import JsonTas
 from packageurl import PackageURL
 from requests.exceptions import HTTPError, ConnectionError as RequestsConnectionError
 from urllib3.util import Retry
@@ -90,14 +95,22 @@
     def identity(self) -> PackageURL:
         """IUT Identity.
 
         :return: IUT identity as PURL object.
         """
         return self.dataset.get("identity")
 
+    @staticmethod
+    def _record_exception(exc) -> None:
+        """Record the given exception to the current OpenTelemetry span."""
+        span = opentelemetry.trace.get_current_span()
+        span.set_attribute("error.type", exc.__class__.__name__)
+        span.record_exception(exc)
+        span.set_status(opentelemetry.trace.Status(opentelemetry.trace.StatusCode.ERROR))
+
     def checkin(self, execution_space: ExecutionSpace) -> None:
         """Check in execution spaces.
 
         :param execution_space: Execution space to checkin.
         """
         end = self.etos.config.get("WAIT_FOR_EXECUTION_SPACE_TIMEOUT")
         if end is None:
@@ -110,41 +123,53 @@
             self.logger.debug("Check in execution space %r (timeout %ds)", execution_space, end)
             execution_space = [execution_space]
         else:
             self.logger.debug("Check in execution spaces %r (timeout %ds)", execution_space, end)
         execution_spaces = [execution_space.as_dict for execution_space in execution_space]
 
         host = self.ruleset.get("stop", {}).get("host")
+        headers = {"X-ETOS-ID": self.identifier}
+        TraceContextTextMapPropagator().inject(headers)
+        span = opentelemetry.trace.get_current_span()
+        span.set_attribute("http.request.body", json.dumps(execution_spaces))
+        span.set_attribute(SpanAttributes.URL_FULL, host)
+        for header, value in headers.items():
+            span.set_attribute(f"http.request.headers.{header.lower()}", value)
         timeout = time.time() + end
         first_iteration = True
         while time.time() < timeout:
             if first_iteration:
                 first_iteration = False
             else:
                 time.sleep(2)
             try:
-                response = requests.post(
-                    host, json=execution_spaces, headers={"X-ETOS-ID": self.identifier}
-                )
+                response = requests.post(host, json=execution_spaces, headers=headers)
+                span.set_attribute(SpanAttributes.HTTP_RESPONSE_STATUS_CODE, response.status_code)
                 if response.status_code == requests.codes["no_content"]:
                     return
                 response = response.json()
                 if response.get("error") is not None:
-                    raise ExecutionSpaceCheckinFailed(
+                    exc = ExecutionSpaceCheckinFailed(
                         f"Unable to check in {execution_spaces} " f"({response.get('error')})"
                     )
+                    self._record_exception(exc)
+                    raise exc
             except RequestsConnectionError as error:
                 if "connection refused" in str(error).lower():
                     self.logger.error("Error connecting to %r: %r", host, error)
                     continue
+                span.record_exception(exc)
+                raise exc
                 raise
             except ConnectionError:
                 self.logger.error("Error connecting to %r", host)
                 continue
-        raise TimeoutError(f"Unable to stop external provider {self.id!r}")
+        exc = TimeoutError(f"Unable to stop external provider {self.id!r}")
+        self._record_exception(exc)
+        raise exc
 
     def checkin_all(self) -> None:
         """Check in all execution spaces.
 
         This method does the same as 'checkin'. It exists for API consistency.
         """
         self.logger.debug("Checking in all checked out execution spaces")
@@ -187,89 +212,115 @@
             "artifact_id": self.dataset.get("artifact_id"),
             "artifact_created": self.dataset.get("artifact_created"),
             "artifact_published": self.dataset.get("artifact_published"),
             "tercc": self.dataset.get("tercc"),
             "dataset": self.dataset.get("dataset"),
             "context": self.dataset.get("context"),
         }
+        host = self.ruleset.get("start", {}).get("host")
+        headers = {"X-ETOS-ID": self.identifier}
+        TraceContextTextMapPropagator().inject(headers)
+        span = opentelemetry.trace.get_current_span()
+        span.set_attribute(SpanAttributes.HTTP_HOST, host)
+        span.set_attribute("http.request.body", json.dumps(data))
+        for header, value in headers.items():
+            span.set_attribute(f"http.request.headers.{header.lower()}", value)
+
         try:
             response = self.http.post(
-                self.ruleset.get("start", {}).get("host"),
+                host,
                 json=data,
-                headers={"X-ETOS-ID": self.identifier},
+                headers=headers,
             )
+            span.set_attribute(SpanAttributes.HTTP_RESPONSE_STATUS_CODE, response.status_code)
             response.raise_for_status()
             return response.json().get("id")
         except (HTTPError, JSONDecodeError) as error:
-            raise Exception(f"Could not start external provider {self.id!r}") from error
+            exc = Exception(f"Could not start external provider {self.id!r}")
+            self._record_exception(exc)
+            raise exc from error
 
     def wait(self, provider_id: str) -> dict:
         """Wait for external execution space provider to finish its request.
 
         :param provider_id: The ID of the external execution space provider request.
         :return: The response from the external execution space provider.
         """
         self.logger.debug(
             "Waiting for external execution space provider (%ds timeout)",
             self.etos.config.get("WAIT_FOR_EXECUTION_SPACE_TIMEOUT"),
         )
 
         host = self.ruleset.get("status", {}).get("host")
         timeout = time.time() + self.etos.config.get("WAIT_FOR_EXECUTION_SPACE_TIMEOUT")
-
+        params = {"id": provider_id}
         response = None
         first_iteration = True
+        headers = {"X-ETOS-ID": self.identifier}
+        TraceContextTextMapPropagator().inject(headers)
+        span = opentelemetry.trace.get_current_span()
+        span.set_attribute("http.request.params", json.dumps(params))
+        span.set_attribute(SpanAttributes.HTTP_HOST, host)
         while time.time() < timeout:
             if first_iteration:
                 first_iteration = False
             else:
                 time.sleep(2)
             try:
                 response = requests.get(
                     host,
-                    params={"id": provider_id},
-                    headers={"X-ETOS-ID": self.identifier},
+                    params=params,
+                    headers=headers,
                 )
                 self.check_error(response)
                 response = response.json()
             except ConnectionError:
                 self.logger.error("Error connecting to %r", host)
                 continue
 
             if response.get("status") == "FAILED":
-                raise ExecutionSpaceCheckoutFailed(response.get("description"))
+                exc = ExecutionSpaceCheckoutFailed(response.get("description"))
+                self._record_exception(exc)
+                raise exc
             if response.get("status") == "DONE":
                 break
         else:
-            raise TimeoutError(
+            exc = TimeoutError(
                 "Status request timed out after "
                 f"{self.etos.config.get('WAIT_FOR_EXECUTION_SPACE_TIMEOUT')}s"
             )
+            self._record_exception(exc)
+            raise exc
         return response
 
     def check_error(self, response: dict) -> None:
         """Check response for errors and try to translate them to something usable.
 
         :param response: The response from the external execution space provider.
         """
+        span = opentelemetry.trace.get_current_span()
         self.logger.debug("Checking response from external execution space provider")
         try:
             if response.json().get("error") is not None:
                 self.logger.error(response.json().get("error"))
         except JSONDecodeError:
             self.logger.error("Could not parse response as JSON")
 
         if response.status_code == requests.codes["not_found"]:
-            raise ExecutionSpaceNotAvailable(
+            exc = ExecutionSpaceNotAvailable(
                 f"External provider {self.id!r} did not respond properly"
             )
+            self._record_exception(exc)
+            raise exc
         if response.status_code == requests.codes["bad_request"]:
-            raise RuntimeError(
+            exc = RuntimeError(
                 f"Execution space provider for {self.id!r} is not properly configured"
             )
+            self._record_exception(exc)
+            raise exc
 
         # This should work, no other errors found.
         # If this does not work, propagate JSONDecodeError up the stack.
         self.logger.debug("Status for response %r", response.json().get("status"))
 
     def build_execution_spaces(self, response: dict) -> list[ExecutionSpace]:
         """Build execution space objects from external execution space provider response.
@@ -295,15 +346,17 @@
         :return: List of checked out execution spaces.
         """
         try:
             provider_id = self.start(minimum_amount, maximum_amount)
             response = self.wait(provider_id)
             execution_spaces = self.build_execution_spaces(response)
             if len(execution_spaces) < minimum_amount:
-                raise ExecutionSpaceNotAvailable(self.id)
+                exc = ExecutionSpaceNotAvailable(self.id)
+                self._record_exception(exc)
+                raise exc
             if len(execution_spaces) > maximum_amount:
                 self.logger.warning(
                     "Too many execution spaces from external execution space provider "
                     "%r. (Expected: %d, Got %d)",
                     self.id,
                     maximum_amount,
                     len(execution_spaces),
@@ -349,16 +402,17 @@
                         "type": "OTHER",
                         "description": f"Checking out execution spaces",
                     }
                 ],
             )
             self.etos.events.send_activity_started(triggered)
             return self.request_and_wait_for_execution_spaces(minimum_amount, maximum_amount)
-        except Exception as exception:
-            error = exception
+        except Exception as exc:
+            self._record_exception(exc)
+            error = exc
             raise
         finally:
             if error is None:
                 outcome = {"conclusion": "SUCCESSFUL"}
             else:
                 outcome = {"conclusion": "UNSUCCESSFUL", "description": str(error)}
             if triggered is not None:
```

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/instructions.py` & `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/instructions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/execution_space_provider/utilities/list.py` & `etos_environment_provider-4.2.0/src/execution_space_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/__init__.py` & `etos_environment_provider-4.2.0/src/iut_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/exceptions.py` & `etos_environment_provider-4.2.0/src/iut_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/iut.py` & `etos_environment_provider-4.2.0/src/iut_provider/iut.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/iut_provider.py` & `etos_environment_provider-4.2.0/src/iut_provider/iut_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/schemas/external_schema.json` & `etos_environment_provider-4.2.0/src/iut_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.2.0/src/iut_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/utilities/__init__.py` & `etos_environment_provider-4.2.0/src/iut_provider/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/utilities/checkin.py` & `etos_environment_provider-4.2.0/src/iut_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/utilities/checkout.py` & `etos_environment_provider-4.2.0/src/iut_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/utilities/external_provider.py` & `etos_environment_provider-4.2.0/src/iut_provider/utilities/external_provider.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,19 +11,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """IUT provider for external providers."""
 import logging
+import json
 import os
 import time
 from copy import deepcopy
 from json.decoder import JSONDecodeError
 
+import opentelemetry
+from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
+from opentelemetry.semconv.trace import SpanAttributes
 import requests
 from etos_lib import ETOS
 from etos_lib.lib.http import Http
 from jsontas.jsontas import JsonTas
 from packageurl import PackageURL
 from requests.exceptions import HTTPError, ConnectionError as RequestsConnectionError
 from urllib3.util import Retry
@@ -84,14 +88,22 @@
     def identity(self) -> PackageURL:
         """IUT Identity.
 
         :return: IUT identity as PURL object.
         """
         return self.dataset.get("identity")
 
+    @staticmethod
+    def _record_exception(exc) -> None:
+        """Record the given exception to the current OpenTelemetry span."""
+        span = opentelemetry.trace.get_current_span()
+        span.set_attribute("error.type", exc.__class__.__name__)
+        span.record_exception(exc)
+        span.set_status(opentelemetry.trace.Status(opentelemetry.trace.StatusCode.ERROR))
+
     def checkin(self, iut: Iut) -> None:
         """Check in IUTs.
 
         :param iut: IUT to checkin.
         """
         end = self.etos.config.get("WAIT_FOR_IUT_TIMEOUT")
         if end is None:
@@ -104,37 +116,49 @@
             self.logger.debug("Check in IUT %r (timeout %ds)", iut, end)
             iut = [iut]
         else:
             self.logger.debug("Check in IUTs %r (timeout %ds)", iut, end)
         iuts = [iut.as_dict for iut in iut]
 
         host = self.ruleset.get("stop", {}).get("host")
+        headers = {"X-ETOS-ID": self.identifier}
+        TraceContextTextMapPropagator().inject(headers)
+        span = opentelemetry.trace.get_current_span()
+        span.set_attribute(SpanAttributes.URL_FULL, host)
+        span.set_attribute("http.request.body", json.dumps(iuts))
+        for header, value in headers.items():
+            span.set_attribute(f"http.request.headers.{header.lower()}", value)
         timeout = time.time() + end
         first_iteration = True
         while time.time() < timeout:
             if first_iteration:
                 first_iteration = False
             else:
                 time.sleep(2)
             try:
-                response = requests.post(host, json=iuts, headers={"X-ETOS-ID": self.identifier})
+                response = requests.post(host, json=iuts, headers=headers)
                 if response.status_code == requests.codes["no_content"]:
                     return
                 response = response.json()
                 if response.get("error") is not None:
-                    raise IutCheckinFailed(f"Unable to check in {iuts} ({response.get('error')})")
+                    exc = IutCheckinFailed(f"Unable to check in {iuts} ({response.get('error')})")
+                    self._record_exception(exc)
+                    raise exc
             except RequestsConnectionError as error:
                 if "connection refused" in str(error).lower():
                     self.logger.error("Error connecting to %r: %r", host, error)
                     continue
+                self._record_exception(error)
                 raise
             except ConnectionError:
                 self.logger.error("Error connecting to %r", host)
                 continue
-        raise TimeoutError(f"Unable to stop external provider {self.id!r}")
+        exc = TimeoutError(f"Unable to stop external provider {self.id!r}")
+        self._record_exception(exc)
+        raise exc
 
     def checkin_all(self) -> None:
         """Check in all IUTs.
 
         This method does the same as 'checkin'. It exists for API consistency.
         """
         self.logger.debug("Checking in all checked out IUTs")
@@ -155,23 +179,32 @@
             "artifact_id": self.dataset.get("artifact_id"),
             "artifact_created": self.dataset.get("artifact_created"),
             "artifact_published": self.dataset.get("artifact_published"),
             "tercc": self.dataset.get("tercc"),
             "dataset": self.dataset.get("dataset"),
             "context": self.dataset.get("context"),
         }
+        host = self.ruleset.get("start", {}).get("host")
+        headers = {"X-ETOS-ID": self.identifier}
+        TraceContextTextMapPropagator().inject(headers)
+        span = opentelemetry.trace.get_current_span()
+        span.set_attribute(SpanAttributes.URL_FULL, host)
+        span.set_attribute("http.request.body", json.dumps(data))
+        for header, value in headers.items():
+            span.set_attribute(f"http.request.headers.{header.lower()}", value)
         try:
             response = self.http.post(
-                self.ruleset.get("start", {}).get("host"),
+                host,
                 json=data,
-                headers={"X-ETOS-ID": self.identifier},
+                headers=headers,
             )
             response.raise_for_status()
             return response.json().get("id")
         except (HTTPError, JSONDecodeError) as error:
+            self._record_exception(error)
             raise Exception(f"Could not start external provider {self.id!r}") from error
 
     def wait(self, provider_id: str) -> dict:
         """Wait for external IUT provider to finish its request.
 
         :param provider_id: The ID of the external IUT provider request.
         :return: The response from the external IUT provider.
@@ -181,21 +214,23 @@
             self.etos.config.get("WAIT_FOR_IUT_TIMEOUT"),
         )
 
         host = self.ruleset.get("status", {}).get("host")
         timeout = time.time() + self.etos.config.get("WAIT_FOR_IUT_TIMEOUT")
 
         response = None
+        headers = {"X-ETOS-ID": self.identifier}
+        TraceContextTextMapPropagator().inject(headers)
         while time.time() < timeout:
             time.sleep(2)
             try:
                 response = requests.get(
                     host,
                     params={"id": provider_id},
-                    headers={"X-ETOS-ID": self.identifier},
+                    headers=headers,
                 )
                 self.check_error(response)
                 response = response.json()
             except ConnectionError:
                 self.logger.error("Error connecting to %r", host)
                 continue
```

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.2.0/src/iut_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/utilities/list.py` & `etos_environment_provider-4.2.0/src/iut_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/iut_provider/utilities/prepare.py` & `etos_environment_provider-4.2.0/src/iut_provider/utilities/prepare.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/__init__.py` & `etos_environment_provider-4.2.0/src/log_area_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/exceptions.py` & `etos_environment_provider-4.2.0/src/log_area_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/log_area.py` & `etos_environment_provider-4.2.0/src/log_area_provider/log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/log_area_provider.py` & `etos_environment_provider-4.2.0/src/log_area_provider/log_area_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/schemas/external_schema.json` & `etos_environment_provider-4.2.0/src/log_area_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.2.0/src/log_area_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/utilities/__init__.py` & `etos_environment_provider-4.2.0/src/log_area_provider/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/utilities/checkin.py` & `etos_environment_provider-4.2.0/src/log_area_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/utilities/checkout.py` & `etos_environment_provider-4.2.0/src/log_area_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/utilities/external_provider.py` & `etos_environment_provider-4.2.0/src/log_area_provider/utilities/external_provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,19 +11,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """External log area provider."""
 import logging
+import json
 import os
 import time
 from copy import deepcopy
 from json.decoder import JSONDecodeError
 
+import opentelemetry
+from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
+from opentelemetry.semconv.trace import SpanAttributes
 import requests
 from etos_lib import ETOS
 from etos_lib.lib.http import Http
 from jsontas.jsontas import JsonTas
 from packageurl import PackageURL
 from requests.exceptions import HTTPError, ConnectionError as RequestsConnectionError
 from urllib3.util import Retry
@@ -84,14 +88,22 @@
     def identity(self) -> PackageURL:
         """IUT identity.
 
         :return: IUT identity as PURL object.
         """
         return self.dataset.get("identity")
 
+    @staticmethod
+    def _record_exception(exc) -> None:
+        """Record the given exception to the current OpenTelemetry span."""
+        span = opentelemetry.trace.get_current_span()
+        span.set_attribute("error.type", exc.__class__.__name__)
+        span.record_exception(exc)
+        span.set_status(opentelemetry.trace.Status(opentelemetry.trace.StatusCode.ERROR))
+
     def checkin(self, log_area: LogArea) -> None:
         """Check in log areas.
 
         :param log_area: Log area to check in.
         """
         end = self.etos.config.get("WAIT_FOR_LOG_AREA_TIMEOUT")
         if end is None:
@@ -104,41 +116,51 @@
             self.logger.debug("Check in log area %r (timeout %ds)", log_area, end)
             log_area = [log_area]
         else:
             self.logger.debug("Check in log areas %r (timeout %ds)", log_area, end)
         log_areas = [log_area.as_dict for log_area in log_area]
 
         host = self.ruleset.get("stop", {}).get("host")
+        headers = {"X-ETOS-ID": self.identifier}
+        TraceContextTextMapPropagator().inject(headers)
+        span = opentelemetry.trace.get_current_span()
+        span.set_attribute(SpanAttributes.URL_FULL, host)
+        span.set_attribute("http.request.body", json.dumps(log_areas))
+        for header, value in headers.items():
+            span.set_attribute(f"http.request.headers.{header.lower()}", value)
         timeout = time.time() + end
         first_iteration = True
         while time.time() < timeout:
             if first_iteration:
                 first_iteration = False
             else:
                 time.sleep(2)
             try:
-                response = requests.post(
-                    host, json=log_areas, headers={"X-ETOS-ID": self.identifier}
-                )
+                response = requests.post(host, json=log_areas, headers=headers)
                 if response.status_code == requests.codes["no_content"]:
                     return
                 response = response.json()
                 if response.get("error") is not None:
-                    raise LogAreaCheckinFailed(
+                    exc = LogAreaCheckinFailed(
                         f"Unable to check in {log_areas} ({response.get('error')})"
                     )
+                    self._record_exception(exc)
+                    raise exc
             except RequestsConnectionError as error:
                 if "connection refused" in str(error).lower():
                     self.logger.error("Error connecting to %r: %r", host, error)
                     continue
+                self._record_exception(error)
                 raise
             except ConnectionError:
                 self.logger.error("Error connecting to %r", host)
                 continue
-        raise TimeoutError(f"Unable to stop external provider {self.id!r}")
+        exc = TimeoutError(f"Unable to stop external provider {self.id!r}")
+        self._record_exception(exc)
+        raise exc
 
     def checkin_all(self) -> None:
         """Check in all log areas.
 
         This method does the same as 'checkin'. It exists for API consistency.
         """
         self.logger.debug("Checking in all checked out log areas")
@@ -159,23 +181,32 @@
             "artifact_id": self.dataset.get("artifact_id"),
             "artifact_created": self.dataset.get("artifact_created"),
             "artifact_published": self.dataset.get("artifact_published"),
             "tercc": self.dataset.get("tercc"),
             "dataset": self.dataset.get("dataset"),
             "context": self.dataset.get("context"),
         }
+        host = self.ruleset.get("start", {}).get("host")
+        headers = {"X-ETOS-ID": self.identifier}
+        TraceContextTextMapPropagator().inject(headers)
+        span = opentelemetry.trace.get_current_span()
+        span.set_attribute(SpanAttributes.URL_FULL, host)
+        span.set_attribute("http.request.body", json.dumps(data))
+        for header, value in headers.items():
+            span.set_attribute(f"http.request.headers.{header.lower()}", value)
         try:
             response = self.http.post(
-                self.ruleset.get("start", {}).get("host"),
+                host,
                 json=data,
-                headers={"X-ETOS-ID": self.identifier},
+                headers=headers,
             )
             response.raise_for_status()
             return response.json().get("id")
         except (HTTPError, JSONDecodeError) as error:
+            self._record_exception(error)
             raise Exception(f"Could not start external provider {self.id!r}") from error
 
     def wait(self, provider_id: str) -> dict:
         """Wait for external log area provider to finish its request.
 
         :param provider_id: The ID of the external log area provider request.
         :type provider_id: str
@@ -188,40 +219,46 @@
         )
 
         host = self.ruleset.get("status", {}).get("host")
         timeout = time.time() + self.etos.config.get("WAIT_FOR_LOG_AREA_TIMEOUT")
 
         response = None
         first_iteration = True
+        headers = {"X-ETOS-ID": self.identifier}
+        TraceContextTextMapPropagator().inject(headers)
         while time.time() < timeout:
             if first_iteration:
                 first_iteration = False
             else:
                 time.sleep(2)
             try:
                 response = requests.get(
                     host,
                     params={"id": provider_id},
-                    headers={"X-ETOS-ID": self.identifier},
+                    headers=headers,
                 )
                 self.check_error(response)
                 response = response.json()
             except ConnectionError:
                 self.logger.error("Error connecting to %r", host)
                 continue
 
             if response.get("status") == "FAILED":
-                raise LogAreaCheckoutFailed(response.get("description"))
+                exc = LogAreaCheckoutFailed(response.get("description"))
+                self._record_exception(exc)
+                raise exc
             if response.get("status") == "DONE":
                 break
         else:
-            raise TimeoutError(
+            exc = TimeoutError(
                 "Status request timed out after "
                 f"{self.etos.config.get('WAIT_FOR_LOG_AREA_TIMEOUT')}s"
             )
+            self._record_exception(exc)
+            raise exc
         return response
 
     def check_error(self, response: dict) -> None:
         """Check response for errors and try to translate them to something usable.
 
         :param response: The response from the external log area provider.
         """
@@ -229,17 +266,21 @@
         try:
             if response.json().get("error") is not None:
                 self.logger.error(response.json().get("error"))
         except JSONDecodeError:
             self.logger.error("Could not parse response as JSON")
 
         if response.status_code == requests.codes["not_found"]:
-            raise LogAreaNotAvailable(f"External provider {self.id!r} did not respond properly")
+            exc = LogAreaNotAvailable(f"External provider {self.id!r} did not respond properly")
+            self._record_exception(exc)
+            raise exc
         if response.status_code == requests.codes["bad_request"]:
-            raise RuntimeError(f"Log area provider for {self.id!r} is not properly configured")
+            exc = RuntimeError(f"Log area provider for {self.id!r} is not properly configured")
+            self._record_exception(exc)
+            raise exc
 
         # This should work, no other errors found.
         # If this does not work, propagate JSONDecodeError up the stack.
         self.logger.debug("Status for response %r", response.json().get("status"))
 
     def build_log_areas(self, response: dict) -> list[LogArea]:
         """Build log area objects from external log area provider response.
@@ -313,14 +354,15 @@
                         "description": f"Checking out log areas",
                     }
                 ],
             )
             self.etos.events.send_activity_started(triggered)
             return self.request_and_wait_for_log_areas(minimum_amount, maximum_amount)
         except Exception as exception:
+            self._record_exception(exception)
             error = exception
             raise
         finally:
             if error is None:
                 outcome = {"conclusion": "SUCCESSFUL"}
             else:
                 outcome = {"conclusion": "UNSUCCESSFUL", "description": str(error)}
```

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.2.0/src/log_area_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/src/log_area_provider/utilities/list.py` & `etos_environment_provider-4.2.0/src/log_area_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/__init__.py` & `etos_environment_provider-4.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/external_execution_space/__init__.py` & `etos_environment_provider-4.2.0/tests/external_execution_space/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/external_execution_space/test_external_execution_space.py` & `etos_environment_provider-4.2.0/tests/external_execution_space/test_external_execution_space.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/external_iut/__init__.py` & `etos_environment_provider-4.2.0/tests/external_iut/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/external_iut/test_external_iut.py` & `etos_environment_provider-4.2.0/tests/external_iut/test_external_iut.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/external_log_area/__init__.py` & `etos_environment_provider-4.2.0/tests/external_log_area/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/external_log_area/test_external_log_area.py` & `etos_environment_provider-4.2.0/tests/external_log_area/test_external_log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/library/__init__.py` & `etos_environment_provider-4.2.0/tests/library/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/library/fake_database.py` & `etos_environment_provider-4.2.0/tests/library/fake_database.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/library/fake_server.py` & `etos_environment_provider-4.2.0/tests/library/fake_server.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/library/graphql_handler.py` & `etos_environment_provider-4.2.0/tests/library/graphql_handler.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/splitter/test_splitter.py` & `etos_environment_provider-4.2.0/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/tercc.py` & `etos_environment_provider-4.2.0/tests/tercc.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tests/test_environment_provider.py` & `etos_environment_provider-4.2.0/tests/test_environment_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-4.1.0/tox.ini` & `etos_environment_provider-4.2.0/tox.ini`

 * *Files identical despite different names*

