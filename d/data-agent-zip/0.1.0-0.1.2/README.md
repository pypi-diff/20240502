# Comparing `tmp/data-agent-zip-0.1.0.tar.gz` & `tmp/data_agent_zip-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-agent-zip-0.1.0.tar", last modified: Thu Sep 21 19:53:50 2023, max compression
+gzip compressed data, was "data_agent_zip-0.1.2.tar", last modified: Thu May  2 21:32:14 2024, max compression
```

## Comparing `data-agent-zip-0.1.0.tar` & `data_agent_zip-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 19:53:50.246409 data-agent-zip-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 19:53:50.242409 data-agent-zip-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 19:53:50.242409 data-agent-zip-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-09-21 19:53:50.246409 data-agent-zip-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 19:53:50.246409 data-agent-zip-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 19:53:50.246409 data-agent-zip-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-09-21 19:53:50.246409 data-agent-zip-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 19:53:50.242409 data-agent-zip-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 19:53:50.246409 data-agent-zip-0.1.0/src/data_agent_zip/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/src/data_agent_zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11414 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/src/data_agent_zip/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 19:53:50.246409 data-agent-zip-0.1.0/src/data_agent_zip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-09-21 19:53:50.000000 data-agent-zip-0.1.0/src/data_agent_zip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      776 2023-09-21 19:53:50.000000 data-agent-zip-0.1.0/src/data_agent_zip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 19:53:50.000000 data-agent-zip-0.1.0/src/data_agent_zip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-09-21 19:53:50.000000 data-agent-zip-0.1.0/src/data_agent_zip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 19:53:50.000000 data-agent-zip-0.1.0/src/data_agent_zip.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-09-21 19:53:50.000000 data-agent-zip-0.1.0/src/data_agent_zip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-21 19:53:50.000000 data-agent-zip-0.1.0/src/data_agent_zip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 19:53:50.246409 data-agent-zip-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/tests/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2023-09-21 19:53:18.000000 data-agent-zip-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:14.587354 data_agent_zip-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:14.579354 data_agent_zip-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:14.583354 data_agent_zip-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-02 21:32:14.587354 data_agent_zip-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:14.583354 data_agent_zip-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:14.583354 data_agent_zip-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-02 21:32:14.587354 data_agent_zip-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:14.579354 data_agent_zip-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:14.583354 data_agent_zip-0.1.2/src/data_agent_zip/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/src/data_agent_zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/src/data_agent_zip/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:14.587354 data_agent_zip-0.1.2/src/data_agent_zip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-02 21:32:14.000000 data_agent_zip-0.1.2/src/data_agent_zip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-02 21:32:14.000000 data_agent_zip-0.1.2/src/data_agent_zip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:32:14.000000 data_agent_zip-0.1.2/src/data_agent_zip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 21:32:14.000000 data_agent_zip-0.1.2/src/data_agent_zip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:32:14.000000 data_agent_zip-0.1.2/src/data_agent_zip.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-02 21:32:14.000000 data_agent_zip-0.1.2/src/data_agent_zip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 21:32:14.000000 data_agent_zip-0.1.2/src/data_agent_zip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:14.587354 data_agent_zip-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/tests/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-02 21:31:42.000000 data_agent_zip-0.1.2/tox.ini
```

### Comparing `data-agent-zip-0.1.0/.coveragerc` & `data_agent_zip-0.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/.github/workflows/ci.yml` & `data_agent_zip-0.1.2/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-# GitHub Actions configuration **EXAMPLE**,
-# MODIFY IT ACCORDING TO YOUR NEEDS!
-# Reference: https://docs.github.com/en/actions
-
-name: tests
+name: build
 
 on:
   push:
     # Avoid using all the resources/limits available by checking only
     # relevant branches and tags. Other branches can be checked via PRs.
     branches: [main]
     tags: ['v[0-9]*', '[0-9]+.[0-9]+*']  # Match tags that resemble a version
@@ -28,32 +24,32 @@
 
 jobs:
   prepare:
     runs-on: ubuntu-latest
     outputs:
       wheel-distribution: ${{ steps.wheel-distribution.outputs.path }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with: {fetch-depth: 0}  # deep clone for setuptools-scm
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         id: setup-python
         with: {python-version: "3.11"}
       - name: Run static analysis and format checkers
         run: pipx run pre-commit run --all-files --show-diff-on-failure
       - name: Build package distribution files
         run: >-
           pipx run --python '${{ steps.setup-python.outputs.python-path }}'
           tox -e clean,build
       - name: Record the path of wheel distribution
         id: wheel-distribution
         run: echo "path=$(ls dist/*.whl)" >> $GITHUB_OUTPUT
       - name: Store the distribution files for use in other stages
         # `tests` and `publish` will use the same pre-built distributions,
         # so we make sure to release the exact same package that was tested
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: python-distribution-files
           path: dist/
           retention-days: 1
 
   test:
     needs: prepare
@@ -63,21 +59,21 @@
         - "3.8"  # oldest Python supported by PSF
         - "3.11"  # newest Python that is stable
         platform:
         - ubuntu-latest
 #        - windows-latest
     runs-on: ${{ matrix.platform }}
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         id: setup-python
         with:
           python-version: ${{ matrix.python }}
       - name: Retrieve pre-built distribution files
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with: {name: python-distribution-files, path: dist/}
       - name: Run tests
         run: >-
           pipx run --python '${{ steps.setup-python.outputs.python-path }}'
           tox --installpkg '${{ needs.prepare.outputs.wheel-distribution }}'
           -- -rFEx --durations 10 --color yes  # pytest args
       - name: Generate coverage report
@@ -103,19 +99,19 @@
   publish:
     needs: finalize
     if: ${{ github.event_name == 'push' && contains(github.ref, 'refs/tags/') }}
     runs-on: ubuntu-latest
     permissions:
       contents: write
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with: {python-version: "3.11"}
       - name: Retrieve pre-built distribution files
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with: {name: python-distribution-files, path: dist/}
       - name: Publish Package
         env:
           # TODO: Set your PYPI_TOKEN as a secret using GitHub UI
           # - https://pypi.org/help/#apitoken
           # - https://docs.github.com/en/actions/security-guides/encrypted-secrets
           TWINE_REPOSITORY: pypi
```

### Comparing `data-agent-zip-0.1.0/.gitignore` & `data_agent_zip-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/.pre-commit-config.yaml` & `data_agent_zip-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/.readthedocs.yml` & `data_agent_zip-0.1.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/CONTRIBUTING.md` & `data_agent_zip-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/LICENSE.txt` & `data_agent_zip-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/PKG-INFO` & `data_agent_zip-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-agent-zip
-Version: 0.1.0
+Version: 0.1.2
 Summary: ZIP files plugin for `data-agent` package
 Home-page: https://github.com/imubit/data-agent-zip/
 Author: Meir Tseitlin
 Author-email: meir@imubit.com
 License: LGPLv3
 Project-URL: Documentation, https://github.com/imubit/data-agent-zip/
 Project-URL: Source, https://github.com/imubit/data-agent-zip/
```

### Comparing `data-agent-zip-0.1.0/README.md` & `data_agent_zip-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/docs/Makefile` & `data_agent_zip-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/docs/conf.py` & `data_agent_zip-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/docs/index.md` & `data_agent_zip-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/setup.cfg` & `data_agent_zip-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/setup.py` & `data_agent_zip-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/src/data_agent_zip/__init__.py` & `data_agent_zip-0.1.2/src/data_agent_zip/__init__.py`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/src/data_agent_zip/connector.py` & `data_agent_zip-0.1.2/src/data_agent_zip/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import tempfile
 import zipfile
 from functools import wraps
 from typing import Union
 
 import pandas as pd
 from data_agent.abstract_connector import (
+    STANDARD_ATTRIBUTES,
     AbstractConnector,
     SupportedOperation,
     active_connection,
     group_exists,
 )
 
 __author__ = "Meir Tseitlin"
@@ -38,38 +39,42 @@
     SUPPORTED_FILTERS = []
     SUPPORTED_OPERATIONS = [
         SupportedOperation.READ_TAG_PERIOD,
         SupportedOperation.WRITE_TAG_PERIOD,
         SupportedOperation.WRITE_TAG_META,
     ]
     DEFAULT_ATTRIBUTES = [
-        ("Name", {"Type": "str", "Name": "Tag"}),
+        ("Name", {"Type": "str", "Name": "Tag Name"}),
+        ("engunits", {"Type": "str", "Name": "Units"}),
+        ("descriptor", {"Type": "str", "Name": "Description"}),
         ("FirstTimestamp", {"Type": "str", "Name": "First Timestamp"}),
         ("FirstValue", {"Type": "int", "Name": "First Value"}),
         ("LastTimestamp", {"Type": "int", "Name": "Last Timestamp"}),
         ("LastValue", {"Type": "int", "Name": "Last Value"}),
         ("TotalRows", {"Type": "int", "Name": "Total Rows"}),
         ("FileSize", {"Type": "int", "Name": "File Size"}),
     ]
 
     TIMESTAMP_COL = "timestamp"
     SYSTEM_COLUMNS = [TIMESTAMP_COL]
     GROUP_DELIMITER = "::"
     DATA_FOLDER = "data"
     META_FOLDER = "meta"
+    TAGS_LIST_FILE = "tags_list.csv"
 
     def __init__(self, conn_name="zip_archive", zipfile_path=None):
         super(ZipConnector, self).__init__(conn_name)
 
         self._zipfile_path = zipfile_path
         self._zipfile = None
         if self._zipfile_path is None:
             self._zipfile_path = os.path.join(
                 tempfile.gettempdir(), f"{os.urandom(10).hex()}.zip"
             )
+        self._tags_list_file = None
 
         log.debug(f"ZIP file path - {self._zipfile_path}")
         print(f"ZIP file path - {self._zipfile_path}")
 
     @staticmethod
     def list_connection_fields():
         return {
@@ -77,30 +82,47 @@
                 "name": "ZIP File",
                 "type": "local_file",
                 "default_value": "c:\\temp\\data.zip",
                 "optional": False,
             }
         }
 
+    @staticmethod
+    def target_info(target_ref):
+        return {}
+
     @property
     def connected(self):
         return self._zipfile is not None
 
     def connect(self):
         self._zipfile = zipfile.ZipFile(
             self._zipfile_path, mode="a", compression=zipfile.ZIP_DEFLATED
         )
 
+        # Start tags list df
+        self._tags_list_df = pd.DataFrame(columns=list(STANDARD_ATTRIBUTES.keys()))
+
         # Not available until Python 3.11
         # self._zipfile.mkdir(self.DATA_FOLDER)
         # self._zipfile.mkdir(self.META_FOLDER)
 
     @active_connection
     def disconnect(self):
         if self._zipfile:
+            try:
+                tags_list_file = self._zipfile.getinfo(self.TAGS_LIST_FILE)
+            except KeyError:
+                tags_list_file = zipfile.ZipInfo(self.TAGS_LIST_FILE)
+
+            # Write tags list
+            self._zipfile.writestr(
+                tags_list_file, self._tags_list_df.to_csv(index=False)
+            )
+
             self._zipfile.close()
             self._zipfile = None
 
     @active_connection
     def connection_info(self):
         return {
             "OneLiner": f"[{self.TYPE}] {self._zipfile_path}",
@@ -219,21 +241,31 @@
             df.index.name = "attribute"
 
             fqn = f"{self.META_FOLDER}/{group}.csv"
 
             try:
                 zip_info = self._zipfile.getinfo(fqn)
             except KeyError:
-                zip_info = None
-
-            if not zip_info:
                 zip_info = zipfile.ZipInfo(fqn)
 
             self._zipfile.writestr(zip_info, df.to_csv())
 
+        # Add standard attrs to df
+        for tag in tags:
+            self._tags_list_df.loc[len(self._tags_list_df.index)] = [
+                tags[tag][a] if a in tags[tag] else None
+                for a in STANDARD_ATTRIBUTES.keys()
+            ]
+
+            # row = ','.join([tags[tag][a] if a in tags[tag] else '' for a in STANDARD_ATTRIBUTES.keys()])
+
+            # with self._zipfile.open(self.TAGS_LIST_FILE, "w") as fl:
+            #     fl.write(row.encode())
+            # self._zipfile.writestr(self._tags_list_file, df.to_csv(index=False))
+
     @active_connection
     def read_tag_values(self, tags: list):
         return pd.read_csv(self._path, index_col=self.TIMESTAMP_COL, usecols=tags)
 
     @active_connection
     def read_tag_values_period(
         self,
@@ -271,15 +303,17 @@
     @csv_file_extension_validate
     def write_tag_values_period(self, group_name, df, attributes=None):
         pass
 
     @active_connection
     def list_groups(self) -> list:
         return [
-            os.path.basename(g) for g in self._zipfile.namelist() if g.endswith("csv")
+            os.path.basename(g)
+            for g in self._zipfile.namelist()
+            if g.endswith("csv") and os.path.dirname(g) == self.DATA_FOLDER
         ]
 
     @csv_file_extension_validate
     def group_period(self, group_name):
         pass
 
     @active_connection
```

### Comparing `data-agent-zip-0.1.0/src/data_agent_zip.egg-info/PKG-INFO` & `data_agent_zip-0.1.2/src/data_agent_zip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-agent-zip
-Version: 0.1.0
+Version: 0.1.2
 Summary: ZIP files plugin for `data-agent` package
 Home-page: https://github.com/imubit/data-agent-zip/
 Author: Meir Tseitlin
 Author-email: meir@imubit.com
 License: LGPLv3
 Project-URL: Documentation, https://github.com/imubit/data-agent-zip/
 Project-URL: Source, https://github.com/imubit/data-agent-zip/
```

### Comparing `data-agent-zip-0.1.0/src/data_agent_zip.egg-info/SOURCES.txt` & `data_agent_zip-0.1.2/src/data_agent_zip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/tests/conftest.py` & `data_agent_zip-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `data-agent-zip-0.1.0/tests/test_connector.py` & `data_agent_zip-0.1.2/tests/test_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,21 @@
         index=pd.date_range("1980-01-01", freq="19S", periods=10**4),
     )
     df.index.name = "timestamp"
 
     zip_archive.write_group_values_period(group_name, df)
 
     tags = zip_archive.list_tags()
+
     assert tags[group_name]["Name"] == "test_group.csv"
     assert tags[group_name]["FileSize"] > 200000
     assert tags[group_name]["HasChildren"] is True
 
+    zip_archive.list_groups() == ["test_group.csv"]
+
     df1 = zip_archive.read_group_values_period(group_name)
     pd.testing.assert_frame_equal(df1, df, check_freq=False, check_dtype=False)
 
     df2 = zip_archive.read_tag_values_period(["test_group.csv::B", "test_group.csv::D"])
     pd.testing.assert_frame_equal(
         df2, df[["B", "D"]], check_freq=False, check_dtype=False
     )
@@ -129,16 +132,20 @@
 #     df_res = csv_store.read_group_values_period(group_name)
 #     assert len(df_res) == 100 * 2
 
 
 def test_write_tag_attributes(zip_archive):
     attr = {
         "tag1": {"Name": "Tag 1", "Type": "bool"},
-        "tag2": {"Name": "Tag 2", "Type": "int"},
-        "tag23": {"Name": "Tag 23", "Type": "double"},
+        "tag2": {"Name": "Tag 2", "Type": "int", "non_standard": 0},
+        "tag23": {
+            "Name": "Tag 23",
+            "Type": "double",
+            "Description": "Non interesting tag",
+        },
     }
 
     zip_archive.write_tag_attributes(attr)
 
     attr = {
         "tag1": {"Name": "Tag 1", "Type": "bool"},
         "group::tag2": {"Name": "Tag 2", "Type": "int"},
```

### Comparing `data-agent-zip-0.1.0/tox.ini` & `data_agent_zip-0.1.2/tox.ini`

 * *Files identical despite different names*

