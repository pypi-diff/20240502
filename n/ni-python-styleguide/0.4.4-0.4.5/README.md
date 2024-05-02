# Comparing `tmp/ni_python_styleguide-0.4.4.tar.gz` & `tmp/ni_python_styleguide-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_python_styleguide-0.4.4.tar", max compression
+gzip compressed data, was "ni_python_styleguide-0.4.5.tar", max compression
```

## Comparing `ni_python_styleguide-0.4.4.tar` & `ni_python_styleguide-0.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1089 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/LICENSE
--rw-r--r--   0        0        0     2398 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/README.md
--rw-r--r--   0        0        0      214 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/__init__.py
--rw-r--r--   0        0        0      164 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/__main__.py
--rw-r--r--   0        0        0     6940 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/_acknowledge_existing_errors/__init__.py
--rw-r--r--   0        0        0     5948 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/_cli.py
--rw-r--r--   0        0        0      192 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/_config_constants.py
--rw-r--r--   0        0        0     5240 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/_fix.py
--rw-r--r--   0        0        0     1001 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/_format.py
--rw-r--r--   0        0        0     1652 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/_lint.py
--rw-r--r--   0        0        0      184 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/_utils/__init__.py
--rw-r--r--   0        0        0      806 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/_utils/code_analysis.py
--rw-r--r--   0        0        0     3131 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/_utils/lint.py
--rw-r--r--   0        0        0     2109 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/_utils/string_helpers.py
--rw-r--r--   0        0        0      518 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/_utils/temp_file.py
--rw-r--r--   0        0        0     3797 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/config.ini
--rw-r--r--   0        0        0      337 2023-10-17 19:34:39.419383 ni_python_styleguide-0.4.4/ni_python_styleguide/config.toml
--rw-r--r--   0        0        0     2047 2023-10-17 19:35:25.263994 ni_python_styleguide-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 ni_python_styleguide-0.4.4/setup.py
--rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 ni_python_styleguide-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/LICENSE
+-rw-r--r--   0        0        0     2398 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/README.md
+-rw-r--r--   0        0        0      214 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/__main__.py
+-rw-r--r--   0        0        0     6940 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/_acknowledge_existing_errors/__init__.py
+-rw-r--r--   0        0        0     5948 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/_cli.py
+-rw-r--r--   0        0        0      192 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/_config_constants.py
+-rw-r--r--   0        0        0     5240 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/_fix.py
+-rw-r--r--   0        0        0     1001 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/_format.py
+-rw-r--r--   0        0        0     1652 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/_lint.py
+-rw-r--r--   0        0        0      184 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/_utils/__init__.py
+-rw-r--r--   0        0        0      806 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/_utils/code_analysis.py
+-rw-r--r--   0        0        0     3131 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/_utils/lint.py
+-rw-r--r--   0        0        0     2109 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/_utils/string_helpers.py
+-rw-r--r--   0        0        0      518 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/_utils/temp_file.py
+-rw-r--r--   0        0        0     3909 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/config.ini
+-rw-r--r--   0        0        0      337 2024-05-02 12:37:13.151513 ni_python_styleguide-0.4.5/ni_python_styleguide/config.toml
+-rw-r--r--   0        0        0     2086 2024-05-02 12:37:50.707891 ni_python_styleguide-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     4042 1970-01-01 00:00:00.000000 ni_python_styleguide-0.4.5/setup.py
+-rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 ni_python_styleguide-0.4.5/PKG-INFO
```

### Comparing `ni_python_styleguide-0.4.4/LICENSE` & `ni_python_styleguide-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.4/README.md` & `ni_python_styleguide-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.4/ni_python_styleguide/_acknowledge_existing_errors/__init__.py` & `ni_python_styleguide-0.4.5/ni_python_styleguide/_acknowledge_existing_errors/__init__.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.4/ni_python_styleguide/_cli.py` & `ni_python_styleguide-0.4.5/ni_python_styleguide/_cli.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.4/ni_python_styleguide/_fix.py` & `ni_python_styleguide-0.4.5/ni_python_styleguide/_fix.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.4/ni_python_styleguide/_format.py` & `ni_python_styleguide-0.4.5/ni_python_styleguide/_format.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.4/ni_python_styleguide/_lint.py` & `ni_python_styleguide-0.4.5/ni_python_styleguide/_lint.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.4/ni_python_styleguide/_utils/code_analysis.py` & `ni_python_styleguide-0.4.5/ni_python_styleguide/_utils/code_analysis.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.4/ni_python_styleguide/_utils/lint.py` & `ni_python_styleguide-0.4.5/ni_python_styleguide/_utils/lint.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.4/ni_python_styleguide/_utils/string_helpers.py` & `ni_python_styleguide-0.4.5/ni_python_styleguide/_utils/string_helpers.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.4/ni_python_styleguide/_utils/temp_file.py` & `ni_python_styleguide-0.4.5/ni_python_styleguide/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `ni_python_styleguide-0.4.4/ni_python_styleguide/config.ini` & `ni_python_styleguide-0.4.5/ni_python_styleguide/config.ini`

 * *Files 8% similar despite different names*

```diff
@@ -108,16 +108,19 @@
     D408
     D409
     D413
     # flake8-import-order
     # I101 - The names in your from import are in the wrong order. (Enforced by E401)
     I101
 
-# We want to ignore missing docstrings in test methods as they are self documenting
-per-file-ignores= tests/**/test_*.py,tests/test_*.py:D100,D103,D102
+per-file-ignores=
+    # We want to ignore missing docstrings in test methods as they are self documenting
+    tests/**/test_*.py,tests/test_*.py:D100,D103,D102
+    # __init__.py files routinely import other modules without directly using them
+    __init__.py:F401
 
 # Flake8 includes mccabe by default.
 # We have yet to evaluate it, so ignore the errors for now
 extend-ignore=C90
 
 # flake8-docstrings
 docstring-convention=all
```

### Comparing `ni_python_styleguide-0.4.4/pyproject.toml` & `ni_python_styleguide-0.4.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "ni-python-styleguide"
 # The a.0 here denotes a source based version
 # This is removed when released through the Publish-Package.yml GitHub action
 # Official PyPI releases follow Major.Minor.Patch
-version = "0.4.4"
+version = "0.4.5"
 description = "NI's internal and external Python linter rules and plugins"
 authors = ["NI <opensource@ni.com>"]
 readme = "README.md" # apply the repo readme to the package as well
 repository = "https://github.com/ni/python-styleguide"
 license = "MIT"
 include = ["ni_python_styleguide/config.toml"]
 
@@ -52,14 +52,15 @@
 pytest = ">=6.0.1"
 pytest_click = ">=1.0.2"
 pytest-snapshot = ">=0.6.3"
 
 
 [tool.poetry.scripts]
 ni-python-styleguide = 'ni_python_styleguide._cli:main'
+nps = 'ni_python_styleguide._cli:main'
 
 
 [tool.black]
 line-length = 100
 
 
 [tool.pytest.ini_options]
```

### Comparing `ni_python_styleguide-0.4.4/setup.py` & `ni_python_styleguide-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 {':python_version < "3.8"': ['importlib-metadata<5.0'],
  ':python_version >= "3.12" and python_version < "4.0"': ['flake8>=6.1,<7.0',
                                                           'pycodestyle>=2.11,<3.0'],
  ':python_version >= "3.7" and python_version < "3.12"': ['flake8>=5.0,<6.0',
                                                           'pycodestyle>=2.9,<3.0']}
 
 entry_points = \
-{'console_scripts': ['ni-python-styleguide = ni_python_styleguide._cli:main']}
+{'console_scripts': ['ni-python-styleguide = ni_python_styleguide._cli:main',
+                     'nps = ni_python_styleguide._cli:main']}
 
 setup_kwargs = {
     'name': 'ni-python-styleguide',
-    'version': '0.4.4',
+    'version': '0.4.5',
     'description': "NI's internal and external Python linter rules and plugins",
     'long_description': '# NI Python Style Guide\n\n![logo](https://raw.githubusercontent.com/ni/python-styleguide/main/docs/logo.svg)\n\n---\n\n[![PyPI version](https://badge.fury.io/py/ni-python-styleguide.svg)](https://badge.fury.io/py/ni-python-styleguide) ![Publish Package](https://github.com/ni/python-styleguide/workflows/Publish%20Package/badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\nWelcome to NI\'s internal and external Python conventions and enforcement tooling.\n\n## Written Conventions\n\nOur written conventions can be found at https://ni.github.io/python-styleguide/.\n\nTheir source is in [docs/Coding-Conventions.md](https://github.com/ni/python-styleguide/tree/main/docs/Coding-Conventions.md).\n\nNOTE: Using the GitHub Pages link is preferable to a GitHub `/blob` link.\n\n## Enforcement tooling\n\nAs a tool, `ni-python-styleguide` is installed like any other script:\n\n```bash\npip install ni-python-styleguide\n```\n\n### Linting\n\nTo lint, just run the `lint` subcommand (from within the project root, or lower):\n\n```bash\nni-python-styleguide lint\n# or\nni-python-styleguide lint ./dir/\n# or\nni-python-styleguide lint module.py\n```\n\nThe rules enforced are all rules documented in the written convention, which are marked as enforced.\n\n### Configuration\n\n`ni-python-styleguide` aims to keep the configuration to a bare minimum (none wherever possible).\nHowever there are some situations you might need to configure the tool.\n\n### Fix\n\n`ni-python-styleguide` has a subcommand `fix` which will run [black](https://pypi.org/project/black/) and [isort](https://pycqa.github.io/isort/).\n\nAdditionally, you can run `fix` with the `--aggressive` option and it will add acknowledgements (# noqa) for the remaining linting errors\nit cannot fix, in addition to running black and isort. \n\n#### When using `setup.py`\n\nIf you\'re using `setup.py`, you\'ll need to set your app\'s import names for import sorting.\n\n```toml\n# pyproject.toml\n[tool.ni-python-styleguide]\napplication-import-names = "<app_name>"\n```\n\n### Formatting\n\n`ni-python-styleguide` in the future will have a `format` command which we intend to fix as many lint issues as possible.\n\nUntil then you\'ll want to set the following to get `black` formatting as the styleguide expects.\n\n```toml\n# pyproject.toml\n[tool.black]\nline-length = 100\n```\n\n### Editor Integration\n\n(This section to come!)\n',
     'author': 'NI',
     'author_email': 'opensource@ni.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ni/python-styleguide',
```

### Comparing `ni_python_styleguide-0.4.4/PKG-INFO` & `ni_python_styleguide-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ni-python-styleguide
-Version: 0.4.4
+Version: 0.4.5
 Summary: NI's internal and external Python linter rules and plugins
 Home-page: https://github.com/ni/python-styleguide
 License: MIT
 Author: NI
 Author-email: opensource@ni.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

