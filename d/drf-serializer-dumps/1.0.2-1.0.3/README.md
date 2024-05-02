# Comparing `tmp/drf_serializer_dumps-1.0.2.tar.gz` & `tmp/drf_serializer_dumps-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_serializer_dumps-1.0.2.tar", last modified: Thu May  2 16:33:18 2024, max compression
+gzip compressed data, was "drf_serializer_dumps-1.0.3.tar", last modified: Thu May  2 17:17:38 2024, max compression
```

## Comparing `drf_serializer_dumps-1.0.2.tar` & `drf_serializer_dumps-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.094249 drf_serializer_dumps-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.086249 drf_serializer_dumps-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.090249 drf_serializer_dumps-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11660 2024-05-02 16:33:18.094249 drf_serializer_dumps-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12378 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:33:18.094249 drf_serializer_dumps-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.086249 drf_serializer_dumps-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.090249 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.090249 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11660 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.090249 drf_serializer_dumps-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/tests/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/tests/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.782069 drf_serializer_dumps-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.774069 drf_serializer_dumps-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.778069 drf_serializer_dumps-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-05-02 17:17:38.778069 drf_serializer_dumps-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-02 17:17:38.782069 drf_serializer_dumps-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.774069 drf_serializer_dumps-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.778069 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.778069 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.778069 drf_serializer_dumps-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/tests/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/tests/test_decorators.py
```

### Comparing `drf_serializer_dumps-1.0.2/.editorconfig` & `drf_serializer_dumps-1.0.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.2/.github/workflows/publish-to-pypi.yml` & `drf_serializer_dumps-1.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.2/.pre-commit-config.yaml` & `drf_serializer_dumps-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.2/CONTRIBUTING.md` & `drf_serializer_dumps-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.2/LICENSE` & `drf_serializer_dumps-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.2/PKG-INFO` & `drf_serializer_dumps-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: drf_serializer_dumps
-Version: 1.0.2
+Version: 1.0.3
 Summary: Decorator for creating dict based on the drf serializer class for swagger
+Home-page: https://github.com/Friskes/drf-serializer-dumps
+Author: Friskes
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,18 +23,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Documentation, https://github.com/Friskes/drf-serializer-dumps
-Project-URL: Repository, https://github.com/Friskes/drf-serializer-dumps
+Project-URL: Homepage, https://github.com/Friskes/drf-serializer-dumps
 Project-URL: Changelog, https://github.com/Friskes/drf-serializer-dumps/releases/
-Project-URL: Bug Reports, https://github.com/Friskes/drf-serializer-dumps/issues
+Project-URL: Issues, https://github.com/Friskes/drf-serializer-dumps/issues
 Keywords: Django,DRF,Spectacular,Swagger
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drf_serializer_dumps-1.0.2/README.md` & `drf_serializer_dumps-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.2/pyproject.toml` & `drf_serializer_dumps-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,17 @@
     "pytest>=7.0.1",
     "mypy>=1.10.0",
     "pytest-cov>=5.0.0",
 ]
 
 
 [project.urls]
-"Documentation" = "https://github.com/Friskes/drf-serializer-dumps"  # Home-page in pip show
-"Repository" = "https://github.com/Friskes/drf-serializer-dumps"
-"Changelog" = "https://github.com/Friskes/drf-serializer-dumps/releases/"
-"Bug Reports" = "https://github.com/Friskes/drf-serializer-dumps/issues"
+Homepage = "https://github.com/Friskes/drf-serializer-dumps"
+Changelog = "https://github.com/Friskes/drf-serializer-dumps/releases/"
+Issues = "https://github.com/Friskes/drf-serializer-dumps/issues"
 
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=8"]
 build-backend = "setuptools.build_meta"
```

### Comparing `drf_serializer_dumps-1.0.2/src/drf_serializer_dumps/decorators.py` & `drf_serializer_dumps-1.0.3/src/drf_serializer_dumps/decorators.py`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/PKG-INFO` & `drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: drf_serializer_dumps
-Version: 1.0.2
+Version: 1.0.3
 Summary: Decorator for creating dict based on the drf serializer class for swagger
+Home-page: https://github.com/Friskes/drf-serializer-dumps
+Author: Friskes
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,18 +23,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Documentation, https://github.com/Friskes/drf-serializer-dumps
-Project-URL: Repository, https://github.com/Friskes/drf-serializer-dumps
+Project-URL: Homepage, https://github.com/Friskes/drf-serializer-dumps
 Project-URL: Changelog, https://github.com/Friskes/drf-serializer-dumps/releases/
-Project-URL: Bug Reports, https://github.com/Friskes/drf-serializer-dumps/issues
+Project-URL: Issues, https://github.com/Friskes/drf-serializer-dumps/issues
 Keywords: Django,DRF,Spectacular,Swagger
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/SOURCES.txt` & `drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

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
 src/drf_serializer_dumps/__init__.py
 src/drf_serializer_dumps/decorators.py
 src/drf_serializer_dumps.egg-info/PKG-INFO
 src/drf_serializer_dumps.egg-info/SOURCES.txt
 src/drf_serializer_dumps.egg-info/dependency_links.txt
 src/drf_serializer_dumps.egg-info/entry_points.txt
```

### Comparing `drf_serializer_dumps-1.0.2/tests/serializers.py` & `drf_serializer_dumps-1.0.3/tests/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.2/tests/test_decorators.py` & `drf_serializer_dumps-1.0.3/tests/test_decorators.py`

 * *Files identical despite different names*

