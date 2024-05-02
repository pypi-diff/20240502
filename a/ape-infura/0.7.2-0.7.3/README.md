# Comparing `tmp/ape-infura-0.7.2.tar.gz` & `tmp/ape-infura-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-infura-0.7.2.tar", last modified: Fri Mar 29 16:37:20 2024, max compression
+gzip compressed data, was "ape-infura-0.7.3.tar", last modified: Thu May  2 19:02:16 2024, max compression
```

## Comparing `ape-infura-0.7.2.tar` & `ape-infura-0.7.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:37:20.891012 ape-infura-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:37:20.887012 ape-infura-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:37:20.887012 ape-infura-0.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:37:20.891012 ape-infura-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-29 16:36:19.000000 ape-infura-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-29 16:36:19.000000 ape-infura-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-29 16:36:19.000000 ape-infura-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-29 16:37:20.891012 ape-infura-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-29 16:36:19.000000 ape-infura-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:37:20.891012 ape-infura-0.7.2/ape_infura/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-29 16:36:19.000000 ape-infura-0.7.2/ape_infura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-03-29 16:36:19.000000 ape-infura-0.7.2/ape_infura/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:36:19.000000 ape-infura-0.7.2/ape_infura/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-29 16:37:20.000000 ape-infura-0.7.2/ape_infura/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:37:20.891012 ape-infura-0.7.2/ape_infura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-29 16:37:20.000000 ape-infura-0.7.2/ape_infura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-29 16:37:20.000000 ape-infura-0.7.2/ape_infura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:37:20.000000 ape-infura-0.7.2/ape_infura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:37:20.000000 ape-infura-0.7.2/ape_infura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-29 16:37:20.000000 ape-infura-0.7.2/ape_infura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 16:37:20.000000 ape-infura-0.7.2/ape_infura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-29 16:36:19.000000 ape-infura-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-29 16:37:20.891012 ape-infura-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-29 16:36:19.000000 ape-infura-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:37:20.891012 ape-infura-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:36:19.000000 ape-infura-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-29 16:36:19.000000 ape-infura-0.7.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-29 16:36:19.000000 ape-infura-0.7.2/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-02 19:00:52.000000 ape-infura-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-02 19:00:52.000000 ape-infura-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-02 19:02:16.041879 ape-infura-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-02 19:00:52.000000 ape-infura-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/ape_infura/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-02 19:00:52.000000 ape-infura-0.7.3/ape_infura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-02 19:00:52.000000 ape-infura-0.7.3/ape_infura/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:00:52.000000 ape-infura-0.7.3/ape_infura/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/ape_infura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-02 19:02:16.000000 ape-infura-0.7.3/ape_infura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-02 19:00:52.000000 ape-infura-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 19:02:16.041879 ape-infura-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-02 19:00:52.000000 ape-infura-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:00:52.000000 ape-infura-0.7.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 19:00:52.000000 ape-infura-0.7.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-02 19:00:52.000000 ape-infura-0.7.3/tests/test_provider.py
```

### Comparing `ape-infura-0.7.2/.github/ISSUE_TEMPLATE/bug.md` & `ape-infura-0.7.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.2/.github/ISSUE_TEMPLATE/feature.md` & `ape-infura-0.7.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.2/.github/ISSUE_TEMPLATE/work-item.md` & `ape-infura-0.7.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.2/.github/release-drafter.yml` & `ape-infura-0.7.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.2/.github/workflows/commit.yaml` & `ape-infura-0.7.3/.github/workflows/commit.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # NOTE: Skip check on PR so as not to confuse contributors
 # NOTE: Also install a PR title checker so we don't mess up merges
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
           with:
               fetch-depth: 0
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check commit history
```

### Comparing `ape-infura-0.7.2/.github/workflows/prtitle.yaml` & `ape-infura-0.7.3/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
```

### Comparing `ape-infura-0.7.2/.github/workflows/publish.yaml` & `ape-infura-0.7.3/.github/workflows/publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
```

### Comparing `ape-infura-0.7.2/.github/workflows/test.yaml` & `ape-infura-0.7.3/.github/workflows/test.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,18 @@
   cancel-in-progress: true
 
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
@@ -58,22 +58,24 @@
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11"]
+                # TODO: Replace with macos-latest when works again.
+                #   https://github.com/actions/setup-python/issues/808
+                os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
+                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
@@ -87,18 +89,18 @@
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
 #
 #        steps:
-#        - uses: actions/checkout@v3
+#        - uses: actions/checkout@v4
 #
 #        - name: Setup Python
-#          uses: actions/setup-python@v4
+#          uses: actions/setup-python@v5
 #          with:
 #              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: |
 #            python -m pip install --upgrade pip
 #            pip install .[test]
```

### Comparing `ape-infura-0.7.2/.gitignore` & `ape-infura-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.2/.pre-commit-config.yaml` & `ape-infura-0.7.3/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-yaml
 
--   repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.10.1
+-   repo: https://github.com/PyCQA/isort
+    rev: 5.13.2
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 23.12.0
+    rev: 24.4.2
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.1
+    rev: v1.10.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-PyYAML, types-requests, types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
```

### Comparing `ape-infura-0.7.2/CONTRIBUTING.md` & `ape-infura-0.7.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.2/LICENSE` & `ape-infura-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.2/PKG-INFO` & `ape-infura-0.7.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-infura
-Version: 0.7.2
+Version: 0.7.3
 Summary: ape-infura: Infura Provider plugins for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-infura
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
@@ -32,19 +33,20 @@
 Use the [Infura](https://infura.io/) provider plugin to interact with blockchains via APIs.
 This plugin supports the following ecosystems:
 
 - Ethereum
 - Polygon
 - Arbitrum
 - Optimism
-- Linea
+- Blast
+- ~~Linea~~ (awaiting ape-linea update)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -74,15 +76,15 @@
 ```bash
 export WEB3_INFURA_PROJECT_ID=MY_API_TOKEN
 ```
 
 To use the Infura provider plugin in most commands, set it via the `--network` option:
 
 ```bash
-ape console --network ethereum:goerli:infura
+ape console --network ethereum:sepolia:infura
 ```
 
 To connect to Infura from a Python script, use the `networks` top-level manager:
 
 ```python
 from ape import networks
```

### Comparing `ape-infura-0.7.2/README.md` & `ape-infura-0.7.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 Use the [Infura](https://infura.io/) provider plugin to interact with blockchains via APIs.
 This plugin supports the following ecosystems:
 
 - Ethereum
 - Polygon
 - Arbitrum
 - Optimism
-- Linea
+- Blast
+- ~~Linea~~ (awaiting ape-linea update)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -45,15 +46,15 @@
 ```bash
 export WEB3_INFURA_PROJECT_ID=MY_API_TOKEN
 ```
 
 To use the Infura provider plugin in most commands, set it via the `--network` option:
 
 ```bash
-ape console --network ethereum:goerli:infura
+ape console --network ethereum:sepolia:infura
 ```
 
 To connect to Infura from a Python script, use the `networks` top-level manager:
 
 ```python
 from ape import networks
```

### Comparing `ape-infura-0.7.2/ape_infura/provider.py` & `ape-infura-0.7.3/ape_infura/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,20 +75,20 @@
     def connection_str(self) -> str:
         return self.uri
 
     def connect(self):
         self._web3 = Web3(HTTPProvider(self.uri))
 
         # Any chain that *began* as PoA needs the middleware for pre-merge blocks
-        ethereum_goerli = 5
         optimism = (10, 420)
         polygon = (137, 80001, 80002)
         linea = (59144, 59140)
+        blast = (11155111, 168587773)
 
-        if self._web3.eth.chain_id in (ethereum_goerli, *optimism, *polygon, *linea):
+        if self._web3.eth.chain_id in (*optimism, *polygon, *linea, *blast):
             self._web3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
         self._web3.eth.set_gas_price_strategy(rpc_gas_price_strategy)
 
     def disconnect(self):
         self._web3 = None
```

### Comparing `ape-infura-0.7.2/ape_infura.egg-info/PKG-INFO` & `ape-infura-0.7.3/ape_infura.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-infura
-Version: 0.7.2
+Version: 0.7.3
 Summary: ape-infura: Infura Provider plugins for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-infura
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
@@ -32,19 +33,20 @@
 Use the [Infura](https://infura.io/) provider plugin to interact with blockchains via APIs.
 This plugin supports the following ecosystems:
 
 - Ethereum
 - Polygon
 - Arbitrum
 - Optimism
-- Linea
+- Blast
+- ~~Linea~~ (awaiting ape-linea update)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -74,15 +76,15 @@
 ```bash
 export WEB3_INFURA_PROJECT_ID=MY_API_TOKEN
 ```
 
 To use the Infura provider plugin in most commands, set it via the `--network` option:
 
 ```bash
-ape console --network ethereum:goerli:infura
+ape console --network ethereum:sepolia:infura
 ```
 
 To connect to Infura from a Python script, use the `networks` top-level manager:
 
 ```python
 from ape import networks
```

### Comparing `ape-infura-0.7.2/ape_infura.egg-info/SOURCES.txt` & `ape-infura-0.7.3/ape_infura.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/feature.md
 .github/ISSUE_TEMPLATE/work-item.md
+.github/workflows/codeql.yml
 .github/workflows/commit.yaml
 .github/workflows/draft.yaml
 .github/workflows/prtitle.yaml
 .github/workflows/publish.yaml
 .github/workflows/test.yaml
 ape_infura/__init__.py
 ape_infura/provider.py
```

### Comparing `ape-infura-0.7.2/ape_infura.egg-info/requires.txt` & `ape-infura-0.7.3/ape_infura.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 ape-arbitrum
+ape-blast
 ape-optimism
 ape-polygon
 websocket-client
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 myst-parser<2,>=1.0.0
 sphinx-click<5,>=4.4.0
 Sphinx<7,>=6.1.3
@@ -41,21 +42,21 @@
 sphinx-click<5,>=4.4.0
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 sphinxcontrib-napoleon>=0.7
 sphinx-plausible<0.2,>=0.1.2
 
 [lint]
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 
 [release]
 setuptools
@@ -65,10 +66,11 @@
 
 [test]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 ape-arbitrum
+ape-blast
 ape-optimism
 ape-polygon
 websocket-client
```

### Comparing `ape-infura-0.7.2/pyproject.toml` & `ape-infura-0.7.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-infura-0.7.2/setup.py` & `ape-infura-0.7.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
-        "ape-arbitrum",
-        "ape-optimism",
-        "ape-polygon",
+        "ape-arbitrum",  # For integration testing
+        "ape-blast",  # For integration testing
+        "ape-optimism",  # For integration testing
+        "ape-polygon",  # For integration testing
         # "ape-linea",  # TODO: Comment out after supports 0.7
         "websocket-client",  # Used for web socket integration testing
     ],
     "lint": [
-        "black>=23.12.0,<24",  # Auto-formatter and linter
-        "mypy>=1.7.1,<2",  # Static type analyzer
+        "black>=24.4.2,<25",  # Auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
-        "flake8>=6.1.0,<7",  # Style linter
+        "flake8>=7.0.0,<8",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # Detect breakpoints left in code
         "flake8-print>=5.0.0,<6",  # Detect print statements left in code
-        "isort>=5.10.1,<6",  # Import sorting linter
+        "isort>=5.13.2,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "doc": [
         "myst-parser>=1.0.0,<2",  # Parse markdown docs
@@ -93,9 +94,10 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ape-infura-0.7.2/tests/test_provider.py` & `ape-infura-0.7.3/tests/test_provider.py`

 * *Files identical despite different names*

