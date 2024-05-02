# Comparing `tmp/celery_starter-1.0.1.tar.gz` & `tmp/celery_starter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_starter-1.0.1.tar", last modified: Tue Apr 30 15:47:53 2024, max compression
+gzip compressed data, was "celery_starter-1.0.2.tar", last modified: Thu May  2 17:18:16 2024, max compression
```

## Comparing `celery_starter-1.0.1.tar` & `celery_starter-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.013289 celery_starter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 15:47:48.000000 celery_starter-1.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.005289 celery_starter-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-30 15:47:48.000000 celery_starter-1.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 15:47:48.000000 celery_starter-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-30 15:47:48.000000 celery_starter-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-30 15:47:48.000000 celery_starter-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 15:47:48.000000 celery_starter-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-30 15:47:53.013289 celery_starter-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-30 15:47:48.000000 celery_starter-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12646 2024-04-30 15:47:48.000000 celery_starter-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:47:53.013289 celery_starter-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.005289 celery_starter-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/src/celery_starter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/_localization.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/src/celery_starter/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/src/celery_starter/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-30 15:47:48.000000 celery_starter-1.0.1/src/celery_starter/management/commands/runcelery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/src/celery_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-30 15:47:52.000000 celery_starter-1.0.1/src/celery_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 15:47:53.000000 celery_starter-1.0.1/src/celery_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:47:52.000000 celery_starter-1.0.1/src/celery_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 15:47:52.000000 celery_starter-1.0.1/src/celery_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 15:47:52.000000 celery_starter-1.0.1/src/celery_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 15:47:52.000000 celery_starter-1.0.1/src/celery_starter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-30 15:47:48.000000 celery_starter-1.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/tests/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/tests/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:53.009289 celery_starter-1.0.1/tests/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:47:48.000000 celery_starter-1.0.1/tests/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 15:47:48.000000 celery_starter-1.0.1/tests/management/commands/test_runcelery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 17:18:09.000000 celery_starter-1.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.428094 celery_starter-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.432094 celery_starter-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-02 17:18:09.000000 celery_starter-1.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 17:18:09.000000 celery_starter-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-02 17:18:09.000000 celery_starter-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-02 17:18:09.000000 celery_starter-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 17:18:09.000000 celery_starter-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-02 17:18:16.436094 celery_starter-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-05-02 17:18:09.000000 celery_starter-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-05-02 17:18:09.000000 celery_starter-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-02 17:18:16.436094 celery_starter-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.428094 celery_starter-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.432094 celery_starter-1.0.2/src/celery_starter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/_localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.432094 celery_starter-1.0.2/src/celery_starter/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/src/celery_starter/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-05-02 17:18:09.000000 celery_starter-1.0.2/src/celery_starter/management/commands/runcelery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/src/celery_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 17:18:16.000000 celery_starter-1.0.2/src/celery_starter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-02 17:18:09.000000 celery_starter-1.0.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/tests/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/tests/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:16.436094 celery_starter-1.0.2/tests/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:18:09.000000 celery_starter-1.0.2/tests/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 17:18:09.000000 celery_starter-1.0.2/tests/management/commands/test_runcelery.py
```

### Comparing `celery_starter-1.0.1/.editorconfig` & `celery_starter-1.0.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.1/.github/workflows/publish-to-pypi.yml` & `celery_starter-1.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.1/.pre-commit-config.yaml` & `celery_starter-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.1/CONTRIBUTING.md` & `celery_starter-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.1/LICENSE` & `celery_starter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.1/PKG-INFO` & `celery_starter-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: celery_starter
-Version: 1.0.1
+Version: 1.0.2
 Summary: Django command to launch celery worker, beat, flower
+Home-page: https://github.com/Friskes/celery-starter
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
         
-Project-URL: Repository, https://github.com/Friskes/celery-starter
+Project-URL: Homepage, https://github.com/Friskes/celery-starter
 Project-URL: Changelog, https://github.com/Friskes/celery-starter/releases/
-Project-URL: Bug Reports, https://github.com/Friskes/celery-starter/issues
+Project-URL: Issues, https://github.com/Friskes/celery-starter/issues
 Keywords: Django,Celery,Beat,Flower,Autoreload
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `celery_starter-1.0.1/README.md` & `celery_starter-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.1/pyproject.toml` & `celery_starter-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     "pytest>=7.0.1",
     "mypy>=1.10.0",
     "pytest-cov>=5.0.0",
 ]
 
 
 [project.urls]
-"Repository" = "https://github.com/Friskes/celery-starter"
-"Changelog" = "https://github.com/Friskes/celery-starter/releases/"
-"Bug Reports" = "https://github.com/Friskes/celery-starter/issues"
+Homepage = "https://github.com/Friskes/celery-starter"
+Changelog = "https://github.com/Friskes/celery-starter/releases/"
+Issues = "https://github.com/Friskes/celery-starter/issues"
 
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=8"]
 build-backend = "setuptools.build_meta"
```

### Comparing `celery_starter-1.0.1/src/celery_starter/_localization.py` & `celery_starter-1.0.2/src/celery_starter/_localization.py`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.1/src/celery_starter/management/commands/runcelery.py` & `celery_starter-1.0.2/src/celery_starter/management/commands/runcelery.py`

 * *Files identical despite different names*

### Comparing `celery_starter-1.0.1/src/celery_starter.egg-info/PKG-INFO` & `celery_starter-1.0.2/src/celery_starter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: celery_starter
-Version: 1.0.1
+Version: 1.0.2
 Summary: Django command to launch celery worker, beat, flower
+Home-page: https://github.com/Friskes/celery-starter
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
         
-Project-URL: Repository, https://github.com/Friskes/celery-starter
+Project-URL: Homepage, https://github.com/Friskes/celery-starter
 Project-URL: Changelog, https://github.com/Friskes/celery-starter/releases/
-Project-URL: Bug Reports, https://github.com/Friskes/celery-starter/issues
+Project-URL: Issues, https://github.com/Friskes/celery-starter/issues
 Keywords: Django,Celery,Beat,Flower,Autoreload
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `celery_starter-1.0.1/src/celery_starter.egg-info/SOURCES.txt` & `celery_starter-1.0.2/src/celery_starter.egg-info/SOURCES.txt`

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
 src/celery_starter/__init__.py
 src/celery_starter/_localization.py
 src/celery_starter/apps.py
 src/celery_starter.egg-info/PKG-INFO
 src/celery_starter.egg-info/SOURCES.txt
 src/celery_starter.egg-info/dependency_links.txt
```

