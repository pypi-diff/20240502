# Comparing `tmp/drf_spectacular_websocket-1.2.6.tar.gz` & `tmp/drf_spectacular_websocket-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_spectacular_websocket-1.2.6.tar", last modified: Mon Apr 29 10:34:45 2024, max compression
+gzip compressed data, was "drf_spectacular_websocket-1.2.7.tar", last modified: Thu May  2 17:18:10 2024, max compression
```

## Comparing `drf_spectacular_websocket-1.2.6.tar` & `drf_spectacular_websocket-1.2.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.093299 drf_spectacular_websocket-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.081298 drf_spectacular_websocket-1.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.085298 drf_spectacular_websocket-1.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-29 10:34:45.093299 drf_spectacular_websocket-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.085298 drf_spectacular_websocket-1.2.6/images/
--rw-r--r--   0 runner    (1001) docker     (127)    66494 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/images/example_receive.png
--rw-r--r--   0 runner    (1001) docker     (127)    89056 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/images/example_send.png
--rw-r--r--   0 runner    (1001) docker     (127)    12793 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:34:45.093299 drf_spectacular_websocket-1.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.081298 drf_spectacular_websocket-1.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.085298 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.089298 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/consumer_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.085298 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.089298 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/templates/drf_spectacular/
--rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/templates/drf_spectacular/swagger_ui.js
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.089298 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.089298 drf_spectacular_websocket-1.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/consumers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.089298 drf_spectacular_websocket-1.2.6/tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/schemas/expected_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/schemas/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.533243 drf_spectacular_websocket-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.525243 drf_spectacular_websocket-1.2.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.529243 drf_spectacular_websocket-1.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-05-02 17:18:10.533243 drf_spectacular_websocket-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.529243 drf_spectacular_websocket-1.2.7/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    66494 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/images/example_receive.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89056 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/images/example_send.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 17:18:10.533243 drf_spectacular_websocket-1.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.525243 drf_spectacular_websocket-1.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.529243 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.529243 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/schemas/consumer_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/schemas/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.525243 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.529243 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/templates/drf_spectacular/
+-rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/templates/drf_spectacular/swagger_ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.533243 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-05-02 17:18:10.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-02 17:18:10.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:18:10.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 17:18:10.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-02 17:18:10.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 17:18:10.000000 drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.533243 drf_spectacular_websocket-1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/tests/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/tests/consumers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:10.533243 drf_spectacular_websocket-1.2.7/tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/tests/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/tests/schemas/expected_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/tests/schemas/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/tests/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-02 17:18:00.000000 drf_spectacular_websocket-1.2.7/tests/urls.py
```

### Comparing `drf_spectacular_websocket-1.2.6/.editorconfig` & `drf_spectacular_websocket-1.2.7/.editorconfig`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/.github/workflows/publish-to-pypi.yml` & `drf_spectacular_websocket-1.2.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/.pre-commit-config.yaml` & `drf_spectacular_websocket-1.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/CONTRIBUTING.md` & `drf_spectacular_websocket-1.2.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/LICENSE` & `drf_spectacular_websocket-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/PKG-INFO` & `drf_spectacular_websocket-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: drf_spectacular_websocket
-Version: 1.2.6
+Version: 1.2.7
 Summary: Extend websocket schema decorator for Django Channels
+Home-page: https://github.com/Friskes/drf-spectacular-websocket
+Author: Friskes
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,17 +23,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Repository, https://github.com/Friskes/drf-spectacular-websocket
+Project-URL: Homepage, https://github.com/Friskes/drf-spectacular-websocket
 Project-URL: Changelog, https://github.com/Friskes/drf-spectacular-websocket/releases/
-Project-URL: Bug Reports, https://github.com/Friskes/drf-spectacular-websocket/issues
+Project-URL: Issues, https://github.com/Friskes/drf-spectacular-websocket/issues
 Keywords: Django,DRF,Spectacular,Swagger,Channels
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drf_spectacular_websocket-1.2.6/README.md` & `drf_spectacular_websocket-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/images/example_receive.png` & `drf_spectacular_websocket-1.2.7/images/example_receive.png`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/images/example_send.png` & `drf_spectacular_websocket-1.2.7/images/example_send.png`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/pyproject.toml` & `drf_spectacular_websocket-1.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
     "pytest>=7.0.1",
     "mypy>=1.10.0",
     "pytest-cov>=5.0.0",
 ]
 
 
 [project.urls]
-"Repository" = "https://github.com/Friskes/drf-spectacular-websocket"
-"Changelog" = "https://github.com/Friskes/drf-spectacular-websocket/releases/"
-"Bug Reports" = "https://github.com/Friskes/drf-spectacular-websocket/issues"
+Homepage = "https://github.com/Friskes/drf-spectacular-websocket"
+Changelog = "https://github.com/Friskes/drf-spectacular-websocket/releases/"
+Issues = "https://github.com/Friskes/drf-spectacular-websocket/issues"
 
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=8"]
 build-backend = "setuptools.build_meta"
```

### Comparing `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/decorators.py` & `drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/decorators.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/consumer_schema.py` & `drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/schemas/consumer_schema.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/schema.py` & `drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/schemas/schema.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/settings.py` & `drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/settings.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/templates/drf_spectacular/swagger_ui.js` & `drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket/templates/drf_spectacular/swagger_ui.js`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/PKG-INFO` & `drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: drf_spectacular_websocket
-Version: 1.2.6
+Version: 1.2.7
 Summary: Extend websocket schema decorator for Django Channels
+Home-page: https://github.com/Friskes/drf-spectacular-websocket
+Author: Friskes
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,17 +23,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Repository, https://github.com/Friskes/drf-spectacular-websocket
+Project-URL: Homepage, https://github.com/Friskes/drf-spectacular-websocket
 Project-URL: Changelog, https://github.com/Friskes/drf-spectacular-websocket/releases/
-Project-URL: Bug Reports, https://github.com/Friskes/drf-spectacular-websocket/issues
+Project-URL: Issues, https://github.com/Friskes/drf-spectacular-websocket/issues
 Keywords: Django,DRF,Spectacular,Swagger,Channels
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/SOURCES.txt` & `drf_spectacular_websocket-1.2.7/src/drf_spectacular_websocket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 .github/workflows/publish-to-pypi.yml
 images/example_receive.png
 images/example_send.png
 src/drf_spectacular_websocket/__init__.py
 src/drf_spectacular_websocket/apps.py
 src/drf_spectacular_websocket/decorators.py
 src/drf_spectacular_websocket/settings.py
```

### Comparing `drf_spectacular_websocket-1.2.6/tests/consumers.py` & `drf_spectacular_websocket-1.2.7/tests/consumers.py`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.6/tests/schemas/expected_schema.py` & `drf_spectacular_websocket-1.2.7/tests/schemas/expected_schema.py`

 * *Files identical despite different names*

