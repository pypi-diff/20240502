# Comparing `tmp/clishelf-0.2.1.tar.gz` & `tmp/clishelf-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "clishelf-0.2.2.tar", last modified: Thu May  2 14:35:42 2024, max compression
```

## Comparing `clishelf-0.2.1.tar` & `clishelf-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,24 @@
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 clishelf-0.2.1/.clishelf.yaml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 clishelf-0.2.1/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0    14146 2020-02-02 00:00:00.000000 clishelf-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 clishelf-0.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 clishelf-0.2.1/clishelf/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clishelf-0.2.1/clishelf/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 clishelf-0.2.1/clishelf/__main__.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 clishelf-0.2.1/clishelf/cli.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 clishelf-0.2.1/clishelf/emoji.py
--rw-r--r--   0        0        0    20608 2020-02-02 00:00:00.000000 clishelf-0.2.1/clishelf/git.py
--rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 clishelf-0.2.1/clishelf/settings.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 clishelf-0.2.1/clishelf/utils.py
--rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 clishelf-0.2.1/clishelf/version.py
--rw-r--r--   0        0        0   128416 2020-02-02 00:00:00.000000 clishelf-0.2.1/clishelf/assets/emoji.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clishelf-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 clishelf-0.2.1/tests/test_cli.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 clishelf-0.2.1/tests/test_cli_emoji.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 clishelf-0.2.1/tests/test_cli_git.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 clishelf-0.2.1/tests/test_cli_version.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 clishelf-0.2.1/tests/test_emoji.py
--rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 clishelf-0.2.1/tests/test_git.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 clishelf-0.2.1/tests/test_settings.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 clishelf-0.2.1/tests/test_utils.py
--rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 clishelf-0.2.1/tests/test_version.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 clishelf-0.2.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 clishelf-0.2.1/LICENSE
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 clishelf-0.2.1/README.md
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 clishelf-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 clishelf-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-02 14:35:38.247015 clishelf-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5632 2024-05-02 14:35:38.247015 clishelf-0.2.2/README.md
+-rw-r--r--   0        0        0       86 2024-05-02 14:35:38.247015 clishelf-0.2.2/clishelf/__about__.py
+-rw-r--r--   0        0        0        0 2024-05-02 14:35:38.247015 clishelf-0.2.2/clishelf/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-02 14:35:38.247015 clishelf-0.2.2/clishelf/__main__.py
+-rw-r--r--   0        0        0   128416 2024-05-02 14:35:38.247015 clishelf-0.2.2/clishelf/assets/emoji.json
+-rw-r--r--   0        0        0     3365 2024-05-02 14:35:38.247015 clishelf-0.2.2/clishelf/cli.py
+-rw-r--r--   0        0        0     2016 2024-05-02 14:35:38.247015 clishelf-0.2.2/clishelf/emoji.py
+-rw-r--r--   0        0        0    20608 2024-05-02 14:35:38.247015 clishelf-0.2.2/clishelf/git.py
+-rw-r--r--   0        0        0     8060 2024-05-02 14:35:38.247015 clishelf-0.2.2/clishelf/settings.py
+-rw-r--r--   0        0        0     2484 2024-05-02 14:35:38.247015 clishelf-0.2.2/clishelf/utils.py
+-rw-r--r--   0        0        0    11763 2024-05-02 14:35:38.247015 clishelf-0.2.2/clishelf/version.py
+-rw-r--r--   0        0        0     3116 2024-05-02 14:35:42.547067 clishelf-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-02 14:35:38.247015 clishelf-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      325 2024-05-02 14:35:38.247015 clishelf-0.2.2/tests/test_cli.py
+-rw-r--r--   0        0        0     1665 2024-05-02 14:35:38.247015 clishelf-0.2.2/tests/test_cli_emoji.py
+-rw-r--r--   0        0        0     4108 2024-05-02 14:35:38.247015 clishelf-0.2.2/tests/test_cli_git.py
+-rw-r--r--   0        0        0       67 2024-05-02 14:35:38.251015 clishelf-0.2.2/tests/test_cli_version.py
+-rw-r--r--   0        0        0      395 2024-05-02 14:35:38.251015 clishelf-0.2.2/tests/test_emoji.py
+-rw-r--r--   0        0        0     6955 2024-05-02 14:35:38.251015 clishelf-0.2.2/tests/test_git.py
+-rw-r--r--   0        0        0     3261 2024-05-02 14:35:38.251015 clishelf-0.2.2/tests/test_settings.py
+-rw-r--r--   0        0        0     1715 2024-05-02 14:35:38.251015 clishelf-0.2.2/tests/test_utils.py
+-rw-r--r--   0        0        0     7880 2024-05-02 14:35:38.251015 clishelf-0.2.2/tests/test_version.py
+-rw-r--r--   0        0        0     6675 1970-01-01 00:00:00.000000 clishelf-0.2.2/PKG-INFO
```

### Comparing `clishelf-0.2.1/clishelf/cli.py` & `clishelf-0.2.2/clishelf/cli.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/clishelf/emoji.py` & `clishelf-0.2.2/clishelf/emoji.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/clishelf/git.py` & `clishelf-0.2.2/clishelf/git.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/clishelf/settings.py` & `clishelf-0.2.2/clishelf/settings.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/clishelf/utils.py` & `clishelf-0.2.2/clishelf/utils.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/clishelf/version.py` & `clishelf-0.2.2/clishelf/version.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/clishelf/assets/emoji.json` & `clishelf-0.2.2/clishelf/assets/emoji.json`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/tests/test_cli_emoji.py` & `clishelf-0.2.2/tests/test_cli_emoji.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/tests/test_cli_git.py` & `clishelf-0.2.2/tests/test_cli_git.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/tests/test_git.py` & `clishelf-0.2.2/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/tests/test_settings.py` & `clishelf-0.2.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/tests/test_utils.py` & `clishelf-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/tests/test_version.py` & `clishelf-0.2.2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/LICENSE` & `clishelf-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.1/README.md` & `clishelf-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,24 +34,24 @@
 many style of config such as I want to make changelog file with style B by my
 custom message code.
 
 **Dependency supported**:
 
 | Python Version   | Installation                            |
 |------------------|-----------------------------------------|
-| `== 3.8`         | `pip install "clishelf>=0.1.10,<0.2.1"` |
+| `== 3.8`         | `pip install "clishelf>=0.1.10,<0.2.2"` |
 | `>=3.9.13,<3.13` | `pip install -U clishelf`               |
 
 ## Pre-Commit Hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 ```yaml
 - repo: https://github.com/korawica/clishelf
-  rev: v0.2.1
+  rev: v0.2.2
   hooks:
     - id: shelf-commit-msg
       stages: [commit-msg]
 ```
 
 ## Features
 
@@ -71,15 +71,15 @@
   dep    List of Dependencies that was set in pyproject.toml file.
   echo   Echo Hello World
   emoji  The Emoji commands
   git    The Extended Git commands
   vs     The Versioning commands.
 ```
 
-**List of Features**:
+**List of Feature Groups**:
 
 * [Extended Git](#extended-git)
 * [Versioning](#versioning)
 * [Emoji](#emoji)
 
 ### Extended Git
 
@@ -143,14 +143,16 @@
 Commands:
   fetch  Refresh emoji metadata file on assets folder.
   ls     List all emojis from metadata file.
 ```
 
 ## Configuration
 
+### Basic Setting
+
 `.clishelf.yaml`:
 
 ```yaml
 version:
   version: "./clishelf/__about__.py"
   changelog: "CHANGELOG.md"
   mode: "normal"
```

### Comparing `clishelf-0.2.1/PKG-INFO` & `clishelf-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: clishelf
-Version: 0.2.1
+Version: 0.2.2
 Summary: Utility CLI Tools that reusable for develop any Python Package
-Project-URL: Homepage, https://github.com/korawica/clishelf/
-Project-URL: Source Code, https://github.com/korawica/clishelf/
-Author-email: korawica <korawich.anu@gmail.com>
-License-Expression: MIT
-License-File: LICENSE
-Keywords: cli,utility
-Classifier: Development Status :: 4 - Beta
+Keywords: utility,cli
+Author-Email: korawica <korawich.anu@gmail.com>
+Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
+Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Utilities
+Project-URL: Homepage, https://github.com/korawica/clishelf/
+Project-URL: Source code, https://github.com/korawica/clishelf/
 Requires-Python: >=3.9.13
-Requires-Dist: bump2version==1.0.1
-Requires-Dist: click<9.0.0,==8.1.7
-Requires-Dist: more-itertools==10.2.0
-Requires-Dist: pre-commit
 Requires-Dist: requests==2.31.0
+Requires-Dist: more-itertools==10.2.0
+Requires-Dist: click<9.0.0,==8.1.7
 Requires-Dist: tomli==2.0.1
-Provides-Extra: dev
-Requires-Dist: coverage[toml]==7.5.0; extra == 'dev'
-Requires-Dist: mypy==1.10.0; extra == 'dev'
-Requires-Dist: pytest==8.2.0; extra == 'dev'
+Requires-Dist: pre-commit
+Requires-Dist: bump2version==1.0.1
 Description-Content-Type: text/markdown
 
 # _CLI Shelf_
 
 [![test](https://github.com/korawica/clishelf/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korawica/clishelf/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/korawica/clishelf/graph/badge.svg?token=7PF8JN2EIG)](https://codecov.io/gh/korawica/clishelf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/clishelf?logo=pypi)](https://pypi.org/project/clishelf/)
@@ -67,24 +61,24 @@
 many style of config such as I want to make changelog file with style B by my
 custom message code.
 
 **Dependency supported**:
 
 | Python Version   | Installation                            |
 |------------------|-----------------------------------------|
-| `== 3.8`         | `pip install "clishelf>=0.1.10,<0.2.1"` |
+| `== 3.8`         | `pip install "clishelf>=0.1.10,<0.2.2"` |
 | `>=3.9.13,<3.13` | `pip install -U clishelf`               |
 
 ## Pre-Commit Hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 ```yaml
 - repo: https://github.com/korawica/clishelf
-  rev: v0.2.1
+  rev: v0.2.2
   hooks:
     - id: shelf-commit-msg
       stages: [commit-msg]
 ```
 
 ## Features
 
@@ -104,15 +98,15 @@
   dep    List of Dependencies that was set in pyproject.toml file.
   echo   Echo Hello World
   emoji  The Emoji commands
   git    The Extended Git commands
   vs     The Versioning commands.
 ```
 
-**List of Features**:
+**List of Feature Groups**:
 
 * [Extended Git](#extended-git)
 * [Versioning](#versioning)
 * [Emoji](#emoji)
 
 ### Extended Git
 
@@ -176,14 +170,16 @@
 Commands:
   fetch  Refresh emoji metadata file on assets folder.
   ls     List all emojis from metadata file.
 ```
 
 ## Configuration
 
+### Basic Setting
+
 `.clishelf.yaml`:
 
 ```yaml
 version:
   version: "./clishelf/__about__.py"
   changelog: "CHANGELOG.md"
   mode: "normal"
```

