# Comparing `tmp/bumpsemver-2.2.0.tar.gz` & `tmp/bumpsemver-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumpsemver-2.2.0.tar", max compression
+gzip compressed data, was "bumpsemver-2.2.1.tar", max compression
```

## Comparing `bumpsemver-2.2.0.tar` & `bumpsemver-2.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1066 2024-04-19 19:52:02.757204 bumpsemver-2.2.0/LICENSE
--rw-r--r--   0        0        0    14130 2024-04-21 20:25:23.922886 bumpsemver-2.2.0/README.md
--rw-r--r--   0        0        0      108 2024-04-21 20:25:23.923684 bumpsemver-2.2.0/bumpsemver/__init__.py
--rw-r--r--   0        0        0       40 2024-04-19 19:52:02.759096 bumpsemver-2.2.0/bumpsemver/__main__.py
--rw-r--r--   0        0        0    14360 2024-04-21 20:25:23.924388 bumpsemver-2.2.0/bumpsemver/cli.py
--rw-r--r--   0        0        0     6998 2024-04-21 20:25:23.925140 bumpsemver-2.2.0/bumpsemver/config.py
--rw-r--r--   0        0        0     3654 2024-04-21 00:37:46.138635 bumpsemver-2.2.0/bumpsemver/discovery.py
--rw-r--r--   0        0        0     4211 2024-04-21 20:25:23.926120 bumpsemver-2.2.0/bumpsemver/exceptions.py
--rw-r--r--   0        0        0        2 2024-04-19 19:52:02.760205 bumpsemver-2.2.0/bumpsemver/files/__init__.py
--rw-r--r--   0        0        0     3461 2024-04-19 19:52:02.760539 bumpsemver-2.2.0/bumpsemver/files/base.py
--rw-r--r--   0        0        0     3629 2024-04-19 19:52:02.761016 bumpsemver-2.2.0/bumpsemver/files/json.py
--rw-r--r--   0        0        0     3338 2024-04-19 19:52:02.761192 bumpsemver-2.2.0/bumpsemver/files/text.py
--rw-r--r--   0        0        0     2895 2024-04-19 19:52:02.761346 bumpsemver-2.2.0/bumpsemver/files/toml.py
--rw-r--r--   0        0        0     3886 2024-04-19 19:52:02.761496 bumpsemver-2.2.0/bumpsemver/files/tomlpath.py
--rw-r--r--   0        0        0     4313 2024-04-21 00:19:36.521238 bumpsemver-2.2.0/bumpsemver/files/yaml.py
--rw-r--r--   0        0        0     1150 2024-04-19 19:52:02.762360 bumpsemver-2.2.0/bumpsemver/functions.py
--rw-r--r--   0        0        0     4121 2024-04-21 00:37:46.139584 bumpsemver-2.2.0/bumpsemver/git.py
--rw-r--r--   0        0        0      228 2024-04-19 19:52:02.763044 bumpsemver-2.2.0/bumpsemver/utils.py
--rw-r--r--   0        0        0     5034 2024-04-21 19:59:55.915557 bumpsemver-2.2.0/bumpsemver/version_part.py
--rw-r--r--   0        0        0     3675 2024-04-21 20:25:23.927053 bumpsemver-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    15334 1970-01-01 00:00:00.000000 bumpsemver-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-19 19:52:02.757204 bumpsemver-2.2.1/LICENSE
+-rw-r--r--   0        0        0    14130 2024-04-21 22:14:45.121296 bumpsemver-2.2.1/README.md
+-rw-r--r--   0        0        0      108 2024-04-21 22:14:44.334072 bumpsemver-2.2.1/bumpsemver/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-19 19:52:02.759096 bumpsemver-2.2.1/bumpsemver/__main__.py
+-rw-r--r--   0        0        0    14360 2024-04-21 20:25:23.924388 bumpsemver-2.2.1/bumpsemver/cli.py
+-rw-r--r--   0        0        0     6998 2024-04-21 20:25:23.925140 bumpsemver-2.2.1/bumpsemver/config.py
+-rw-r--r--   0        0        0     3654 2024-04-21 00:37:46.138635 bumpsemver-2.2.1/bumpsemver/discovery.py
+-rw-r--r--   0        0        0     4159 2024-04-21 22:14:25.292648 bumpsemver-2.2.1/bumpsemver/exceptions.py
+-rw-r--r--   0        0        0        2 2024-04-19 19:52:02.760205 bumpsemver-2.2.1/bumpsemver/files/__init__.py
+-rw-r--r--   0        0        0     3461 2024-04-19 19:52:02.760539 bumpsemver-2.2.1/bumpsemver/files/base.py
+-rw-r--r--   0        0        0     3629 2024-04-19 19:52:02.761016 bumpsemver-2.2.1/bumpsemver/files/json.py
+-rw-r--r--   0        0        0     3338 2024-04-19 19:52:02.761192 bumpsemver-2.2.1/bumpsemver/files/text.py
+-rw-r--r--   0        0        0     2895 2024-04-19 19:52:02.761346 bumpsemver-2.2.1/bumpsemver/files/toml.py
+-rw-r--r--   0        0        0     3886 2024-04-19 19:52:02.761496 bumpsemver-2.2.1/bumpsemver/files/tomlpath.py
+-rw-r--r--   0        0        0     4313 2024-04-21 00:19:36.521238 bumpsemver-2.2.1/bumpsemver/files/yaml.py
+-rw-r--r--   0        0        0     1150 2024-04-19 19:52:02.762360 bumpsemver-2.2.1/bumpsemver/functions.py
+-rw-r--r--   0        0        0     4121 2024-04-21 00:37:46.139584 bumpsemver-2.2.1/bumpsemver/git.py
+-rw-r--r--   0        0        0      228 2024-04-19 19:52:02.763044 bumpsemver-2.2.1/bumpsemver/utils.py
+-rw-r--r--   0        0        0     5034 2024-04-21 19:59:55.915557 bumpsemver-2.2.1/bumpsemver/version_part.py
+-rw-r--r--   0        0        0     3675 2024-04-21 22:14:44.358275 bumpsemver-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0    15334 1970-01-01 00:00:00.000000 bumpsemver-2.2.1/PKG-INFO
```

### Comparing `bumpsemver-2.2.0/LICENSE` & `bumpsemver-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/README.md` & `bumpsemver-2.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![image](https://img.shields.io/pypi/v/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![image](https://img.shields.io/pypi/l/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![image](https://img.shields.io/pypi/pyversions/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![codecov](https://codecov.io/gh/zhaow-de/bumpsemver/graph/badge.svg?token=WP4O30YLO3)](https://codecov.io/gh/zhaow-de/bumpsemver)
 [![GitHub Actions](https://github.com/zhaow-de/bumpsemver/workflows/CI/badge.svg)](https://github.com/zhaow-de/bumpsemver/actions)
 
 
-Current version: **v2.2.0**
+Current version: **v2.2.1**
 
 ## Table of contents
 
 <!--TOC-->
 
 - [Overview](#overview)
 - [Installation](#installation)
```

### Comparing `bumpsemver-2.2.0/bumpsemver/cli.py` & `bumpsemver-2.2.1/bumpsemver/cli.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/bumpsemver/config.py` & `bumpsemver-2.2.1/bumpsemver/config.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/bumpsemver/discovery.py` & `bumpsemver-2.2.1/bumpsemver/discovery.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/bumpsemver/exceptions.py` & `bumpsemver-2.2.1/bumpsemver/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from typing import List, Tuple, Union
 
-from typing_extensions import Buffer
-
 
 class BumpVersionError(Exception):
     """Custom base class for all BumpVersion exception types."""
 
 
 class InvalidConfigSectionError(BumpVersionError):
     def __init__(self, message: str):
         super().__init__(message)
         self.message = message
 
 
 class WorkingDirectoryIsDirtyError(BumpVersionError):
-    def __init__(self, lines: List[Buffer]):
+    def __init__(self, lines):
         message = "Git working directory is not clean:\n{}".format(b"\n".join(lines).decode())
         super().__init__(message)
         self.message = message
 
 
 class CannotParseVersionError(BumpVersionError):
     def __init__(self):
```

### Comparing `bumpsemver-2.2.0/bumpsemver/files/base.py` & `bumpsemver-2.2.1/bumpsemver/files/base.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/bumpsemver/files/json.py` & `bumpsemver-2.2.1/bumpsemver/files/json.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/bumpsemver/files/text.py` & `bumpsemver-2.2.1/bumpsemver/files/text.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/bumpsemver/files/toml.py` & `bumpsemver-2.2.1/bumpsemver/files/toml.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/bumpsemver/files/tomlpath.py` & `bumpsemver-2.2.1/bumpsemver/files/tomlpath.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/bumpsemver/files/yaml.py` & `bumpsemver-2.2.1/bumpsemver/files/yaml.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/bumpsemver/functions.py` & `bumpsemver-2.2.1/bumpsemver/functions.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/bumpsemver/git.py` & `bumpsemver-2.2.1/bumpsemver/git.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/bumpsemver/version_part.py` & `bumpsemver-2.2.1/bumpsemver/version_part.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.2.0/pyproject.toml` & `bumpsemver-2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 max-complexity = 15
 
 [tool.ruff.lint.isort]
 order-by-type = true
 
 [tool.poetry]
 name = "bumpsemver"
-version = "2.2.0"
+version = "2.2.1"
 description = "Bump semver for git repos with a single command"
 readme = "README.md"
 authors = [ "Zhao Wang <zhaow.km@gmail.com>" ]
 license = "MIT"
 repository = "https://github.com/zhaow-de/bumpsemver"
 classifiers = [
     'Development Status :: 4 - Beta',
```

### Comparing `bumpsemver-2.2.0/PKG-INFO` & `bumpsemver-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpsemver
-Version: 2.2.0
+Version: 2.2.1
 Summary: Bump semver for git repos with a single command
 Home-page: https://github.com/zhaow-de/bumpsemver
 License: MIT
 Keywords: bumpsemver,semver,version,release
 Author: Zhao Wang
 Author-email: zhaow.km@gmail.com
 Requires-Python: >=3.10,<4
@@ -34,15 +34,15 @@
 [![image](https://img.shields.io/pypi/v/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![image](https://img.shields.io/pypi/l/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![image](https://img.shields.io/pypi/pyversions/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![codecov](https://codecov.io/gh/zhaow-de/bumpsemver/graph/badge.svg?token=WP4O30YLO3)](https://codecov.io/gh/zhaow-de/bumpsemver)
 [![GitHub Actions](https://github.com/zhaow-de/bumpsemver/workflows/CI/badge.svg)](https://github.com/zhaow-de/bumpsemver/actions)
 
 
-Current version: **v2.2.0**
+Current version: **v2.2.1**
 
 ## Table of contents
 
 <!--TOC-->
 
 - [Overview](#overview)
 - [Installation](#installation)
```

