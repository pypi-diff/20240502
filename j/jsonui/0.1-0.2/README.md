# Comparing `tmp/jsonui-0.1.tar.gz` & `tmp/jsonui-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonui-0.1.tar", last modified: Sat Feb 10 22:49:45 2024, max compression
+gzip compressed data, was "jsonui-0.2.tar", last modified: Wed May  1 23:34:05 2024, max compression
```

## Comparing `jsonui-0.1.tar` & `jsonui-0.2.tar`

### file list

```diff
@@ -1,33 +1,44 @@
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-02-10 22:49:45.970576 jsonui-0.1/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2024-02-10 22:42:27.000000 jsonui-0.1/.coveralls.yml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2024-02-10 22:42:27.000000 jsonui-0.1/.env
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      610 2024-02-10 22:42:27.000000 jsonui-0.1/.gitignore
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1422 2024-02-10 22:42:27.000000 jsonui-0.1/.pre-commit-config.yaml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      361 2024-02-10 22:42:27.000000 jsonui-0.1/.pre-commit-hooks.yaml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1020 2024-02-10 22:42:27.000000 jsonui-0.1/.readthedocs.yaml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      630 2024-02-10 22:42:27.000000 jsonui-0.1/CHANGELOG.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5397 2024-02-10 22:42:27.000000 jsonui-0.1/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1073 2024-02-07 22:41:20.000000 jsonui-0.1/LICENSE
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2280 2024-02-10 22:49:36.000000 jsonui-0.1/Makefile
--rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4376 2024-02-10 22:49:45.970576 jsonui-0.1/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2342 2024-02-10 22:42:27.000000 jsonui-0.1/README.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1378 2024-02-10 22:42:27.000000 jsonui-0.1/SECURITY.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-02-10 22:49:45.966576 jsonui-0.1/examples/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-02-10 22:49:45.966576 jsonui-0.1/examples/json_diff/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-02-10 22:49:45.966576 jsonui-0.1/examples/json_diff/example_1/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      245 2024-02-10 22:42:27.000000 jsonui-0.1/examples/json_diff/example_1/data_1.json
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      221 2024-02-10 22:42:27.000000 jsonui-0.1/examples/json_diff/example_1/data_2.json
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-02-10 22:49:45.966576 jsonui-0.1/examples/json_diff/example_2/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      617 2024-02-10 22:42:27.000000 jsonui-0.1/examples/json_diff/example_2/data_1.json
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      626 2024-02-10 22:42:27.000000 jsonui-0.1/examples/json_diff/example_2/data_2.json
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-02-10 22:49:45.970576 jsonui-0.1/jsonui.egg-info/
--rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4376 2024-02-10 22:49:45.000000 jsonui-0.1/jsonui.egg-info/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      550 2024-02-10 22:49:45.000000 jsonui-0.1/jsonui.egg-info/SOURCES.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2024-02-10 22:49:45.000000 jsonui-0.1/jsonui.egg-info/dependency_links.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       39 2024-02-10 22:49:45.000000 jsonui-0.1/jsonui.egg-info/entry_points.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      214 2024-02-10 22:49:45.000000 jsonui-0.1/jsonui.egg-info/requires.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        7 2024-02-10 22:49:45.000000 jsonui-0.1/jsonui.egg-info/top_level.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     8228 2024-02-10 22:42:27.000000 jsonui-0.1/jsonui.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3896 2024-02-10 22:42:27.000000 jsonui-0.1/pyproject.toml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       38 2024-02-10 22:49:45.970576 jsonui-0.1/setup.cfg
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1436 2024-02-10 22:42:27.000000 jsonui-0.1/tests.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.519773 jsonui-0.2/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2024-02-10 22:42:27.000000 jsonui-0.2/.coveralls.yml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2024-02-10 22:42:27.000000 jsonui-0.2/.env
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.511772 jsonui-0.2/.github/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.515772 jsonui-0.2/.github/workflows/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2543 2024-02-11 21:20:20.000000 jsonui-0.2/.github/workflows/test.yml
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      610 2024-02-10 22:42:27.000000 jsonui-0.2/.gitignore
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1422 2024-02-10 22:42:27.000000 jsonui-0.2/.pre-commit-config.yaml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      361 2024-02-10 22:42:27.000000 jsonui-0.2/.pre-commit-hooks.yaml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1020 2024-02-10 22:42:27.000000 jsonui-0.2/.readthedocs.yaml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2634 2024-02-11 21:20:20.000000 jsonui-0.2/.secrets.baseline
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      681 2024-05-01 23:33:32.000000 jsonui-0.2/CHANGELOG.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5397 2024-02-10 22:42:27.000000 jsonui-0.2/CODE_OF_CONDUCT.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1073 2024-02-07 22:41:20.000000 jsonui-0.2/LICENSE
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2280 2024-02-10 22:49:36.000000 jsonui-0.2/Makefile
+-rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4759 2024-05-01 23:34:05.519773 jsonui-0.2/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2725 2024-05-01 23:33:32.000000 jsonui-0.2/README.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1378 2024-02-10 22:42:27.000000 jsonui-0.2/SECURITY.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.511772 jsonui-0.2/docs/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.515772 jsonui-0.2/docs/screenshots/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    41193 2024-02-11 21:20:20.000000 jsonui-0.2/docs/screenshots/json_diff.png
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)   112217 2024-02-11 21:20:20.000000 jsonui-0.2/docs/screenshots/python_dict_to_json.png
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.515772 jsonui-0.2/examples/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.511772 jsonui-0.2/examples/json_diff/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.515772 jsonui-0.2/examples/json_diff/example_1/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      199 2024-02-11 21:20:20.000000 jsonui-0.2/examples/json_diff/example_1/data_1.json
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      221 2024-02-10 22:42:27.000000 jsonui-0.2/examples/json_diff/example_1/data_2.json
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.515772 jsonui-0.2/examples/json_diff/example_2/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      617 2024-02-10 22:42:27.000000 jsonui-0.2/examples/json_diff/example_2/data_1.json
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      626 2024-02-10 22:42:27.000000 jsonui-0.2/examples/json_diff/example_2/data_2.json
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.515772 jsonui-0.2/examples/python_dict_to_json/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.515772 jsonui-0.2/examples/python_dict_to_json/example_1/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      733 2024-02-11 21:20:20.000000 jsonui-0.2/examples/python_dict_to_json/example_1/data.txt
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-01 23:34:05.519773 jsonui-0.2/jsonui.egg-info/
+-rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4759 2024-05-01 23:34:05.000000 jsonui-0.2/jsonui.egg-info/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      715 2024-05-01 23:34:05.000000 jsonui-0.2/jsonui.egg-info/SOURCES.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2024-05-01 23:34:05.000000 jsonui-0.2/jsonui.egg-info/dependency_links.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       39 2024-05-01 23:34:05.000000 jsonui-0.2/jsonui.egg-info/entry_points.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      214 2024-05-01 23:34:05.000000 jsonui-0.2/jsonui.egg-info/requires.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        7 2024-05-01 23:34:05.000000 jsonui-0.2/jsonui.egg-info/top_level.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    10044 2024-05-01 23:33:32.000000 jsonui-0.2/jsonui.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3896 2024-05-01 23:33:32.000000 jsonui-0.2/pyproject.toml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       38 2024-05-01 23:34:05.519773 jsonui-0.2/setup.cfg
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2049 2024-05-01 23:33:32.000000 jsonui-0.2/tests.py
```

### Comparing `jsonui-0.1/.gitignore` & `jsonui-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jsonui-0.1/.pre-commit-config.yaml` & `jsonui-0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jsonui-0.1/.readthedocs.yaml` & `jsonui-0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `jsonui-0.1/CHANGELOG.rst` & `jsonui-0.2/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -12,12 +12,18 @@
 - It's always safe to upgrade within the same minor version (for example, from
   0.3 to 0.3.4).
 - Minor version changes might be backwards incompatible. Read the
   release notes carefully before upgrading (for example, when upgrading from
   0.3.4 to 0.4).
 - All backwards incompatible changes are mentioned in this document.
 
+0.2
+---
+2024-05-02
+
+- Add JSON to Dict converter.
+
 0.1
 ---
 2024-02-10
 
 - Initial beta release.
```

### Comparing `jsonui-0.1/CODE_OF_CONDUCT.rst` & `jsonui-0.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `jsonui-0.1/LICENSE` & `jsonui-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonui-0.1/Makefile` & `jsonui-0.2/Makefile`

 * *Files identical despite different names*

### Comparing `jsonui-0.1/PKG-INFO` & `jsonui-0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonui
-Version: 0.1
+Version: 0.2
 Summary: UI tools for JSON.
 Author-email: Artur Barseghyan <artur.barseghyan@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/barseghyanartur/jsonui/
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/jsonui/issues
 Project-URL: Documentation, https://jsonui.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/jsonui/
@@ -60,15 +60,15 @@
 
 .. Internal references
 
 .. _jsonui: https://github.com/barseghyanartur/jsonui/
 .. _Read the Docs: http://jsonui.readthedocs.io/
 .. _Contributor guidelines: https://fakepy.readthedocs.io/en/latest/contributor_guidelines.html
 
-UI to support JSON.
+UI/GUI for working with JSON.
 
 .. image:: https://img.shields.io/pypi/v/jsonui.svg
    :target: https://pypi.python.org/pypi/jsonui
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/pypi/pyversions/jsonui.svg
     :target: https://pypi.python.org/pypi/jsonui/
@@ -86,44 +86,66 @@
    :target: https://github.com/barseghyanartur/jsonui/#License
    :alt: MIT
 
 .. image:: https://coveralls.io/repos/github/barseghyanartur/jsonui/badge.svg?branch=main&service=github
     :target: https://coveralls.io/github/barseghyanartur/jsonui?branch=main
     :alt: Coverage
 
-`jsonui`_ is a UI/GUI tool for working with JSON.
-
 Features
 ========
 - Convert Python dict into JSON.
+- Convert JSON to Python dict.
 - Show diffs between two JSONs.
 
 Prerequisites
 =============
 - Python 3.8+
 - `PyQT5`_ (`GPL v3` license)
 - `QScintilla`_ (`GPL v3` license)
 - `deepdiff`_ (`MIT` license)
 
 Installation
 ============
-pipx
-----
+pipx (recommended)
+------------------
 
 .. code-block:: sh
 
     pipx install jsonui
 
 pip
 ---
 
 .. code-block:: sh
 
     pip install jsonui
 
+Usage
+=====
+Run
+---
+
+.. code-block:: sh
+
+    jsonui
+
+Screenshots
+-----------
+**Convert Python dict to JSON**
+
+.. image:: docs/screenshots/python_dict_to_json.png
+   :target: docs/screenshots/python_dict_to_json.png
+   :alt: Python dict to JSON
+
+**JSON diff**
+
+.. image:: docs/screenshots/json_diff.png
+   :target: docs/screenshots/json_diff.png
+   :alt: JSON diff
+
 Documentation
 =============
 - Documentation is available on `Read the Docs`_.
 - For guidelines on contributing check the `Contributor guidelines`_.
 
 Tests
 =====
```

### Comparing `jsonui-0.1/README.rst` & `jsonui-0.2/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 .. Internal references
 
 .. _jsonui: https://github.com/barseghyanartur/jsonui/
 .. _Read the Docs: http://jsonui.readthedocs.io/
 .. _Contributor guidelines: https://fakepy.readthedocs.io/en/latest/contributor_guidelines.html
 
-UI to support JSON.
+UI/GUI for working with JSON.
 
 .. image:: https://img.shields.io/pypi/v/jsonui.svg
    :target: https://pypi.python.org/pypi/jsonui
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/pypi/pyversions/jsonui.svg
     :target: https://pypi.python.org/pypi/jsonui/
@@ -35,44 +35,66 @@
    :target: https://github.com/barseghyanartur/jsonui/#License
    :alt: MIT
 
 .. image:: https://coveralls.io/repos/github/barseghyanartur/jsonui/badge.svg?branch=main&service=github
     :target: https://coveralls.io/github/barseghyanartur/jsonui?branch=main
     :alt: Coverage
 
-`jsonui`_ is a UI/GUI tool for working with JSON.
-
 Features
 ========
 - Convert Python dict into JSON.
+- Convert JSON to Python dict.
 - Show diffs between two JSONs.
 
 Prerequisites
 =============
 - Python 3.8+
 - `PyQT5`_ (`GPL v3` license)
 - `QScintilla`_ (`GPL v3` license)
 - `deepdiff`_ (`MIT` license)
 
 Installation
 ============
-pipx
-----
+pipx (recommended)
+------------------
 
 .. code-block:: sh
 
     pipx install jsonui
 
 pip
 ---
 
 .. code-block:: sh
 
     pip install jsonui
 
+Usage
+=====
+Run
+---
+
+.. code-block:: sh
+
+    jsonui
+
+Screenshots
+-----------
+**Convert Python dict to JSON**
+
+.. image:: docs/screenshots/python_dict_to_json.png
+   :target: docs/screenshots/python_dict_to_json.png
+   :alt: Python dict to JSON
+
+**JSON diff**
+
+.. image:: docs/screenshots/json_diff.png
+   :target: docs/screenshots/json_diff.png
+   :alt: JSON diff
+
 Documentation
 =============
 - Documentation is available on `Read the Docs`_.
 - For guidelines on contributing check the `Contributor guidelines`_.
 
 Tests
 =====
```

### Comparing `jsonui-0.1/SECURITY.rst` & `jsonui-0.2/SECURITY.rst`

 * *Files identical despite different names*

### Comparing `jsonui-0.1/examples/json_diff/example_2/data_1.json` & `jsonui-0.2/examples/json_diff/example_2/data_1.json`

 * *Files identical despite different names*

### Comparing `jsonui-0.1/examples/json_diff/example_2/data_2.json` & `jsonui-0.2/examples/json_diff/example_2/data_2.json`

 * *Files identical despite different names*

### Comparing `jsonui-0.1/jsonui.egg-info/PKG-INFO` & `jsonui-0.2/jsonui.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonui
-Version: 0.1
+Version: 0.2
 Summary: UI tools for JSON.
 Author-email: Artur Barseghyan <artur.barseghyan@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/barseghyanartur/jsonui/
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/jsonui/issues
 Project-URL: Documentation, https://jsonui.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/jsonui/
@@ -60,15 +60,15 @@
 
 .. Internal references
 
 .. _jsonui: https://github.com/barseghyanartur/jsonui/
 .. _Read the Docs: http://jsonui.readthedocs.io/
 .. _Contributor guidelines: https://fakepy.readthedocs.io/en/latest/contributor_guidelines.html
 
-UI to support JSON.
+UI/GUI for working with JSON.
 
 .. image:: https://img.shields.io/pypi/v/jsonui.svg
    :target: https://pypi.python.org/pypi/jsonui
    :alt: PyPI Version
 
 .. image:: https://img.shields.io/pypi/pyversions/jsonui.svg
     :target: https://pypi.python.org/pypi/jsonui/
@@ -86,44 +86,66 @@
    :target: https://github.com/barseghyanartur/jsonui/#License
    :alt: MIT
 
 .. image:: https://coveralls.io/repos/github/barseghyanartur/jsonui/badge.svg?branch=main&service=github
     :target: https://coveralls.io/github/barseghyanartur/jsonui?branch=main
     :alt: Coverage
 
-`jsonui`_ is a UI/GUI tool for working with JSON.
-
 Features
 ========
 - Convert Python dict into JSON.
+- Convert JSON to Python dict.
 - Show diffs between two JSONs.
 
 Prerequisites
 =============
 - Python 3.8+
 - `PyQT5`_ (`GPL v3` license)
 - `QScintilla`_ (`GPL v3` license)
 - `deepdiff`_ (`MIT` license)
 
 Installation
 ============
-pipx
-----
+pipx (recommended)
+------------------
 
 .. code-block:: sh
 
     pipx install jsonui
 
 pip
 ---
 
 .. code-block:: sh
 
     pip install jsonui
 
+Usage
+=====
+Run
+---
+
+.. code-block:: sh
+
+    jsonui
+
+Screenshots
+-----------
+**Convert Python dict to JSON**
+
+.. image:: docs/screenshots/python_dict_to_json.png
+   :target: docs/screenshots/python_dict_to_json.png
+   :alt: Python dict to JSON
+
+**JSON diff**
+
+.. image:: docs/screenshots/json_diff.png
+   :target: docs/screenshots/json_diff.png
+   :alt: JSON diff
+
 Documentation
 =============
 - Documentation is available on `Read the Docs`_.
 - For guidelines on contributing check the `Contributor guidelines`_.
 
 Tests
 =====
```

### Comparing `jsonui-0.1/jsonui.egg-info/SOURCES.txt` & `jsonui-0.2/jsonui.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 .coveralls.yml
 .env
 .gitignore
 .pre-commit-config.yaml
 .pre-commit-hooks.yaml
 .readthedocs.yaml
+.secrets.baseline
 CHANGELOG.rst
 CODE_OF_CONDUCT.rst
 LICENSE
 Makefile
 README.rst
 SECURITY.rst
 jsonui.py
 pyproject.toml
 tests.py
+.github/workflows/test.yml
+docs/screenshots/json_diff.png
+docs/screenshots/python_dict_to_json.png
 examples/json_diff/example_1/data_1.json
 examples/json_diff/example_1/data_2.json
 examples/json_diff/example_2/data_1.json
 examples/json_diff/example_2/data_2.json
+examples/python_dict_to_json/example_1/data.txt
 jsonui.egg-info/PKG-INFO
 jsonui.egg-info/SOURCES.txt
 jsonui.egg-info/dependency_links.txt
 jsonui.egg-info/entry_points.txt
 jsonui.egg-info/requires.txt
 jsonui.egg-info/top_level.txt
```

### Comparing `jsonui-0.1/jsonui.py` & `jsonui-0.2/jsonui.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,21 +11,22 @@
     QTabWidget,
     QTextEdit,
     QVBoxLayout,
     QWidget,
 )
 
 __title__ = "jsonui"
-__version__ = "0.1"
+__version__ = "0.2"
 __author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
 __copyright__ = "2023-2024 Artur Barseghyan"
 __license__ = "MIT"
 __all__ = (
     "DictToJsonConverter",
     "JsonDiff",
+    "JsonToDictConverter",
     "MainApplication",
     "apply_highlight",
     "find_line_number_for_path",
     "highlight_differences",
     "main",
 )
 
@@ -90,15 +91,16 @@
             print("No differences.")
 
 
 def highlight_differences(editor, diff):
     # Simplified approach: Iterate through the changes and highlight
     for change_type, changes in diff.items():
         if change_type == "dictionary_item_added":
-            # Handle new items (simplified example, assumes we can find the position)
+            # Handle new items (simplified example, assumes we can find the
+            # position)
             for added_path in changes:
                 # Here, you'd need to find the line number for the added item
                 line_num = find_line_number_for_path(editor, added_path)
                 apply_highlight(
                     editor, line_num, QColor("#4ba2ff")
                 )  # Example color for addition
 
@@ -112,15 +114,16 @@
 
 
 def find_line_number_for_path(editor, path):
     """Find the line number for a given JSON path in a QScintilla editor.
 
     :param editor: QScintilla editor instance containing JSON text.
     :param path: String path in the format "root['key']['subkey']" or similar.
-    :return: Line number (int) where the path points to in the editor, or -1 if not found.
+    :return: Line number (int) where the path points to in the editor,
+        or -1 if not found.
     """
     # Convert the path string to a list of keys (assuming path is well-formed)
     keys = (
         path.strip("root")
         .replace("']['", ".")
         .strip("['")
         .rstrip("']")
@@ -146,15 +149,16 @@
             # Found the key, remove it from the path list and update line_number
             keys.pop(0)
             line_number = i
 
             if not keys:  # If no more keys, path fully matched
                 break
 
-            # Reset nesting level after matching a key (assuming keys are unique at each level)
+            # Reset nesting level after matching a key (assuming keys are
+            # unique at each level)
             current_nesting_level = 0
 
     if keys:  # Not all keys were matched
         return -1
 
     return line_number
 
@@ -211,31 +215,78 @@
             # Display the JSON string in the output text edit
             self.output_text_edit.setText(json_str)
         except Exception as e:
             self.output_text_edit.setText(f"Error: {str(e)}")
 
 
 # **************************************************************************
+# ************************* JSON to Dict converter *************************
+# **************************************************************************
+
+
+class JsonToDictConverter(QWidget):
+    def __init__(self):
+        super().__init__()
+        self.init_ui()
+
+    def init_ui(self):
+        layout = QVBoxLayout()
+
+        # Create the text edit widgets for input and output
+        self.input_text_edit = QTextEdit()
+        self.input_text_edit.setPlaceholderText("Enter JSON here...")
+        self.output_text_edit = QTextEdit()
+        self.output_text_edit.setPlaceholderText(
+            "Python dict will appear here..."
+        )
+        self.output_text_edit.setReadOnly(True)  # Make output read-only
+
+        # Create the convert button
+        self.convert_button = QPushButton("Convert to Dict")
+        self.convert_button.clicked.connect(self.convert_input)
+
+        # Add widgets to the layout
+        layout.addWidget(self.input_text_edit)
+        layout.addWidget(self.convert_button)
+        layout.addWidget(self.output_text_edit)
+
+        self.setLayout(layout)
+
+    def convert_input(self):
+        # Get the input text
+        input_text = self.input_text_edit.toPlainText()
+        try:
+            # Convert the JSON string to a Python dict
+            input_dict = json.loads(input_text)
+            # Display the Python dict in the output text edit
+            self.output_text_edit.setText(str(input_dict))
+        except json.JSONDecodeError as e:
+            self.output_text_edit.setText(f"Error: {str(e)}")
+
+
+# **************************************************************************
 # ******************************* Main app *********************************
 # **************************************************************************
 
 
 class MainApplication(QWidget):
     def __init__(self):
         super().__init__()
         self.init_ui()
 
     def init_ui(self):
         # Set up the layout
         self.layout = QVBoxLayout()
         self.tabs = QTabWidget()
         self.dict_to_json_tab = DictToJsonConverter()
+        self.json_to_dict_tab = JsonToDictConverter()
         self.json_diff_tab = JsonDiff()
 
         self.tabs.addTab(self.dict_to_json_tab, "Dict to JSON Converter")
+        self.tabs.addTab(self.json_to_dict_tab, "JSON to Dict Converter")
         self.tabs.addTab(self.json_diff_tab, "JSON Diff")
 
         self.layout.addWidget(self.tabs)
         self.setLayout(self.layout)
         self.setWindowTitle("Python JSON Tools")
         self.resize(1000, 800)  # Resize the window
```

### Comparing `jsonui-0.1/pyproject.toml` & `jsonui-0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "jsonui"
 description = "UI tools for JSON."
 readme = "README.rst"
-version = "0.1"
+version = "0.2"
 dependencies = ["PyQt5", "QScintilla", "deepdiff"]
 authors = [
     {name = "Artur Barseghyan", email = "artur.barseghyan@gmail.com"},
 ]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `jsonui-0.1/tests.py` & `jsonui-0.2/tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import unittest
 
-from jsonui import DictToJsonConverter, JsonDiff
+from jsonui import DictToJsonConverter, JsonDiff, JsonToDictConverter
 from PyQt5.QtCore import Qt
 from PyQt5.QtTest import QTest
 from PyQt5.QtWidgets import QApplication
 
 app = QApplication([])  # QApplication instance
 
 __author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
@@ -28,14 +28,31 @@
         QTest.keyClicks(converter.input_text_edit, input_dict)
         QTest.mouseClick(converter.convert_button, Qt.LeftButton)
 
         actual_output = converter.output_text_edit.toPlainText()
         self.assertEqual(actual_output, expected_output)
 
 
+class TestJsonToDictConverter(unittest.TestCase):
+    def test_conversion(self):
+        converter = JsonToDictConverter()
+
+        input_json = (
+            '{"hi": "you", "isTrue": true, "isFalse": false, "isNone": null}'
+        )
+        expected_output = json.loads(input_json)
+
+        QTest.qWaitForWindowExposed(converter)
+        QTest.keyClicks(converter.input_text_edit, input_json)
+        QTest.mouseClick(converter.convert_button, Qt.LeftButton)
+
+        actual_output = converter.output_text_edit.toPlainText()
+        self.assertEqual(eval(actual_output), expected_output)
+
+
 class TestJsonDiff(unittest.TestCase):
     def test_diff_detection(self):
         diff_viewer = JsonDiff()
 
         json1 = '{"name": "Alice", "age": 30}'
         json2 = '{"name": "Alice", "age": 31}'
```

