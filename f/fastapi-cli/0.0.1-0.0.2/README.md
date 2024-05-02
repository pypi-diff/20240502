# Comparing `tmp/fastapi-cli-0.0.1.tar.gz` & `tmp/fastapi_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-cli-0.0.1.tar", last modified: Tue Feb  4 04:48:59 2020, max compression
+gzip compressed data, was "fastapi_cli-0.0.2.tar", last modified: Thu May  2 21:50:17 2024, max compression
```

## Comparing `fastapi-cli-0.0.1.tar` & `fastapi_cli-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,57 @@
--rw-r--r--   0        0        0       75 2020-02-04 04:48:44.593037 fastapi-cli-0.0.1/fastapi_cli/__init__.py
--rw-r--r--   0        0        0      326 2020-02-04 04:46:34.471846 fastapi-cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 fastapi-cli-0.0.1/setup.py
--rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 fastapi-cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5053 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/README.md
+-rw-r--r--   0        0        0     1718 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/pdm_build.py
+-rw-r--r--   0        0        0     3047 2024-05-02 21:50:17.219287 fastapi_cli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/requirements-tests.txt
+-rw-r--r--   0        0        0       60 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/requirements.txt
+-rwxr-xr-x   0        0        0       87 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/scripts/format.sh
+-rwxr-xr-x   0        0        0      110 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/scripts/lint.sh
+-rwxr-xr-x   0        0        0      124 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0       70 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/scripts/test.sh
+-rw-r--r--   0        0        0       22 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/__main__.py
+-rw-r--r--   0        0        0     8754 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/cli.py
+-rw-r--r--   0        0        0     5285 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/discover.py
+-rw-r--r--   0        0        0       47 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/exceptions.py
+-rw-r--r--   0        0        0      664 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/logging.py
+-rw-r--r--   0        0        0        0 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/py.typed
+-rw-r--r--   0        0        0        0 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/tests/assets/broken_package/mod/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/tests/assets/broken_package/mod/app.py
+-rw-r--r--   0        0        0       52 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/tests/assets/broken_package/utils.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/tests/assets/default_files/default_api/api.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app/api.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app/app.py
+-rw-r--r--   0        0        0        0 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_api/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_api/app/api.py
+-rw-r--r--   0        0        0        0 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_app/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_app/app/api.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_app/app/app.py
+-rw-r--r--   0        0        0        0 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_main/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_main/app/api.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_main/app/app.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_main/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_non_default/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_non_default/app/nondefault.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_main/api.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_main/app.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_main/main.py
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/non_default/nonstandard.py
+-rw-r--r--   0        0        0       64 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/core/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/core/utils.py
+-rw-r--r--   0        0        0       28 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/mod/__init__.py
+-rw-r--r--   0        0        0      359 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/mod/api.py
+-rw-r--r--   0        0        0      447 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/mod/app.py
+-rw-r--r--   0        0        0      271 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/mod/other.py
+-rw-r--r--   0        0        0      371 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/single_file_api.py
+-rw-r--r--   0        0        0      463 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/single_file_app.py
+-rw-r--r--   0        0        0      279 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/single_file_other.py
+-rw-r--r--   0        0        0      530 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     8393 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/test_cli.py
+-rw-r--r--   0        0        0     3905 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/test_utils_default_dir.py
+-rw-r--r--   0        0        0     4046 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/test_utils_default_file.py
+-rw-r--r--   0        0        0    20671 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/test_utils_package.py
+-rw-r--r--   0        0        0     4993 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/test_utils_single_file.py
+-rw-r--r--   0        0        0      325 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/utils.py
+-rw-r--r--   0        0        0     6780 1970-01-01 00:00:00.000000 fastapi_cli-0.0.2/PKG-INFO
```

