# Comparing `tmp/github_changelog_md-0.9.2.tar.gz` & `tmp/github_changelog_md-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_changelog_md-0.9.2.tar", max compression
+gzip compressed data, was "github_changelog_md-0.9.3.tar", max compression
```

## Comparing `github_changelog_md-0.9.2.tar` & `github_changelog_md-0.9.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-10-26 10:12:59.778343 github_changelog_md-0.9.2/LICENSE.txt
--rw-r--r--   0        0        0     7315 2023-11-19 20:14:22.938785 github_changelog_md-0.9.2/README.md
--rw-r--r--   0        0        0       27 2023-10-26 10:12:59.782343 github_changelog_md-0.9.2/github_changelog_md/__init__.py
--rw-r--r--   0        0        0       96 2023-10-26 10:12:59.782343 github_changelog_md-0.9.2/github_changelog_md/changelog/__init__.py
--rw-r--r--   0        0        0    29481 2024-03-07 15:33:41.874214 github_changelog_md-0.9.2/github_changelog_md/changelog/changelog.py
--rw-r--r--   0        0        0       98 2023-10-26 10:12:59.782343 github_changelog_md-0.9.2/github_changelog_md/config/__init__.py
--rw-r--r--   0        0        0     3834 2024-02-14 16:08:36.998377 github_changelog_md-0.9.2/github_changelog_md/config/settings.py
--rw-r--r--   0        0        0     1089 2024-02-14 16:08:36.998377 github_changelog_md-0.9.2/github_changelog_md/constants.py
--rw-r--r--   0        0        0     3314 2024-03-07 15:33:41.874214 github_changelog_md-0.9.2/github_changelog_md/helpers.py
--rw-r--r--   0        0        0     6034 2023-11-08 09:08:47.484093 github_changelog_md-0.9.2/github_changelog_md/main.py
--rw-r--r--   0        0        0     4541 2024-03-07 15:35:28.889975 github_changelog_md-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     8511 1970-01-01 00:00:00.000000 github_changelog_md-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-10-26 10:12:59.778343 github_changelog_md-0.9.3/LICENSE.txt
+-rw-r--r--   0        0        0     7502 2024-05-02 09:51:26.474005 github_changelog_md-0.9.3/README.md
+-rw-r--r--   0        0        0       27 2023-10-26 10:12:59.782343 github_changelog_md-0.9.3/github_changelog_md/__init__.py
+-rw-r--r--   0        0        0       97 2024-05-01 11:45:11.391136 github_changelog_md-0.9.3/github_changelog_md/changelog/__init__.py
+-rw-r--r--   0        0        0    29482 2024-05-02 09:51:22.842010 github_changelog_md-0.9.3/github_changelog_md/changelog/changelog.py
+-rw-r--r--   0        0        0       99 2024-05-01 11:45:11.391136 github_changelog_md-0.9.3/github_changelog_md/config/__init__.py
+-rw-r--r--   0        0        0     3835 2024-05-01 11:45:11.391136 github_changelog_md-0.9.3/github_changelog_md/config/settings.py
+-rw-r--r--   0        0        0     1090 2024-05-01 11:45:11.391136 github_changelog_md-0.9.3/github_changelog_md/constants.py
+-rw-r--r--   0        0        0     3315 2024-05-01 11:56:42.579089 github_changelog_md-0.9.3/github_changelog_md/helpers.py
+-rw-r--r--   0        0        0     6035 2024-05-01 11:45:11.391136 github_changelog_md-0.9.3/github_changelog_md/main.py
+-rw-r--r--   0        0        0     4558 2024-05-02 11:19:49.932437 github_changelog_md-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     8693 1970-01-01 00:00:00.000000 github_changelog_md-0.9.3/PKG-INFO
```

### Comparing `github_changelog_md-0.9.2/LICENSE.txt` & `github_changelog_md-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `github_changelog_md-0.9.2/README.md` & `github_changelog_md-0.9.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![PyPI
 version](https://badge.fury.io/py/github-changelog-md.svg)](https://badge.fury.io/py/github-changelog-md)
 ![PyPI - License](https://img.shields.io/pypi/l/github-changelog-md)
 [![Ruff](https://github.com/seapagan/github-changelog-md/actions/workflows/linting.yml/badge.svg)](https://github.com/seapagan/github-changelog-md/actions/workflows/linting.yml)
 [![Tests](https://github.com/seapagan/github-changelog-md/actions/workflows/tests.yml/badge.svg)](https://github.com/seapagan/github-changelog-md/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/seapagan/github-changelog-md/graph/badge.svg?token=27D8PGNX0E)](https://codecov.io/gh/seapagan/github-changelog-md)
 [![Dependency Review](https://github.com/seapagan/github-changelog-md/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/seapagan/github-changelog-md/actions/workflows/dependency-review.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/seapagan/github-changelog-md/main.svg)](https://results.pre-commit.ci/latest/github/seapagan/github-changelog-md/main)
 [![CodeQL](https://github.com/seapagan/github-changelog-md/actions/workflows/codeql.yml/badge.svg)](https://github.com/seapagan/github-changelog-md/actions/workflows/codeql.yml)
 [![Weekly Downloads](https://static.pepy.tech/personalized-badge/github-changelog-md?period=week&units=international_system&left_color=black&right_color=green&left_text=Weekly%20Downloads)](https://pepy.tech/project/github-changelog-md)
 [![Total Downloads](https://static.pepy.tech/personalized-badge/github-changelog-md?period=total&units=international_system&left_color=black&right_color=green&left_text=Total%20Downloads)](https://pepy.tech/project/github-changelog-md)
 
 **Generate a Markdown changelog from a Github repository.**
 
 This project will generate a Markdown-formatted changelog from a Github
```

### Comparing `github_changelog_md-0.9.2/github_changelog_md/changelog/changelog.py` & `github_changelog_md-0.9.3/github_changelog_md/changelog/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Define the Changelog class.
 
 This will encapsulate the logic for generating the changelog.
 """
+
 # mypy: disable-error-code="no-untyped-def"
 from __future__ import annotations
 
 import datetime
 import os
 import sys
 from pathlib import Path
```

### Comparing `github_changelog_md-0.9.2/github_changelog_md/config/settings.py` & `github_changelog_md-0.9.3/github_changelog_md/config/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Handle the settings for the project."""
+
 import sys
 from pathlib import Path
 from typing import ClassVar, Optional
 
 from rich import print  # pylint: disable=redefined-builtin
 from rich.prompt import Prompt
 from simple_toml_settings import TOMLSettings
```

### Comparing `github_changelog_md-0.9.2/github_changelog_md/constants.py` & `github_changelog_md-0.9.3/github_changelog_md/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define constants used throughout the application."""
+
 from enum import IntEnum
 from typing import Union
 
 SectionHeadings = tuple[str, Union[str, None]]
 
 
 class ExitErrors(IntEnum):
```

### Comparing `github_changelog_md-0.9.2/github_changelog_md/helpers.py` & `github_changelog_md-0.9.3/github_changelog_md/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define helper functions for the application."""
+
 from __future__ import annotations
 
 import sys
 from importlib import metadata, resources
 from pathlib import Path
 
 import rtoml
```

### Comparing `github_changelog_md-0.9.2/github_changelog_md/main.py` & `github_changelog_md-0.9.3/github_changelog_md/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Entry point for the main application loop."""
+
 from __future__ import annotations
 
 import sys
 from typing import Any, Optional
 
 import typer
 from rich import print  # pylint: disable=redefined-builtin
```

### Comparing `github_changelog_md-0.9.2/pyproject.toml` & `github_changelog_md-0.9.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "github-changelog-md"
-version = "0.9.2"
+version = "0.9.3"
 description = "Generate a Markdown Changelog from your Github repository."
 authors = ["Grant Ramsay <seapagan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 packages = [{ include = "github_changelog_md" }]
 
@@ -19,49 +19,49 @@
 [tool.poetry.scripts]
 github-changelog-md = "github_changelog_md.main:app"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 pygithub = ">=1.59.1,<3.0.0"
 pydantic = "^2.3.0"
-rtoml = "^0.9.0"
+rtoml = ">=0.9.0,<1.0.0"
 simple-toml-settings = ">=0.4.0,<1.0.0"
-typer = "^0.9.0"
+typer = ">=0.9,<0.13"
 rich = "^13.6.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.group.dev.dependencies]
 # linting, type-checking and security checks
 pre-commit = "^3.3.3"
 pymarkdownlnt = "^0.9.12"
 mypy = "^1.4.1"
-ruff = ">=0.1.1,<0.3.0"
+ruff = ">=0.1.1,<0.5.0"
 
 # task runner
-poethepoet = ">=0.21.1,<0.26.0"
+poethepoet = ">=0.21.1,<0.27.0"
 
 # testing
-faker = ">=19.2,<24.0"
+faker = ">=19.2,<26.0"
 mock = "^5.1.0"
 pyfakefs = "^5.3.0"
 pytest = ">=7.4,<9.0"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4,<6"
 pytest-xdist = "^3.2.1"
 pytest-sugar = ">=0.9.7,<1.1.0"
 pytest-randomly = "^3.13.0"
 pytest-reverse = "^1.7.0"
 pytest-asyncio = "^0.21.1"
 pytest-mock = "^3.11.1"
 
 # documentation
 mkdocs = "^1.4.3"
-mkdocs-autorefs = "^0.5.0"
+mkdocs-autorefs = ">=0.5,<1.1"
 mkdocs-material = "^9.1.19"
 mkdocs-minify-plugin = ">=0.7,<0.9"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 pymdown-extensions = "^10.1"
 pygments = "^2.15.1"
 
 [tool.poe.tasks]
```

### Comparing `github_changelog_md-0.9.2/PKG-INFO` & `github_changelog_md-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-changelog-md
-Version: 0.9.2
+Version: 0.9.3
 Summary: Generate a Markdown Changelog from your Github repository.
 Home-page: https://changelog.seapagan.net
 License: MIT
 Author: Grant Ramsay
 Author-email: seapagan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,17 +12,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.3.0,<3.0.0)
 Requires-Dist: pygithub (>=1.59.1,<3.0.0)
 Requires-Dist: rich (>=13.6.0,<14.0.0)
-Requires-Dist: rtoml (>=0.9.0,<0.10.0)
+Requires-Dist: rtoml (>=0.9.0,<1.0.0)
 Requires-Dist: simple-toml-settings (>=0.4.0,<1.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.9,<0.13)
 Project-URL: Bug Tracker, https://github.com/seapagan/github-changelog-md/issues
 Project-URL: Changelog, https://github.com/seapagan/github-changelog-md/blob/main/CHANGELOG.md
 Project-URL: Pull Requests, https://github.com/seapagan/github-changelog-md/pulls
 Project-URL: Repository, https://github.com/seapagan/github-changelog-md
 Description-Content-Type: text/markdown
 
 # Markdown Changelog Generator <!-- omit in toc -->
@@ -30,14 +30,15 @@
 [![PyPI
 version](https://badge.fury.io/py/github-changelog-md.svg)](https://badge.fury.io/py/github-changelog-md)
 ![PyPI - License](https://img.shields.io/pypi/l/github-changelog-md)
 [![Ruff](https://github.com/seapagan/github-changelog-md/actions/workflows/linting.yml/badge.svg)](https://github.com/seapagan/github-changelog-md/actions/workflows/linting.yml)
 [![Tests](https://github.com/seapagan/github-changelog-md/actions/workflows/tests.yml/badge.svg)](https://github.com/seapagan/github-changelog-md/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/seapagan/github-changelog-md/graph/badge.svg?token=27D8PGNX0E)](https://codecov.io/gh/seapagan/github-changelog-md)
 [![Dependency Review](https://github.com/seapagan/github-changelog-md/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/seapagan/github-changelog-md/actions/workflows/dependency-review.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/seapagan/github-changelog-md/main.svg)](https://results.pre-commit.ci/latest/github/seapagan/github-changelog-md/main)
 [![CodeQL](https://github.com/seapagan/github-changelog-md/actions/workflows/codeql.yml/badge.svg)](https://github.com/seapagan/github-changelog-md/actions/workflows/codeql.yml)
 [![Weekly Downloads](https://static.pepy.tech/personalized-badge/github-changelog-md?period=week&units=international_system&left_color=black&right_color=green&left_text=Weekly%20Downloads)](https://pepy.tech/project/github-changelog-md)
 [![Total Downloads](https://static.pepy.tech/personalized-badge/github-changelog-md?period=total&units=international_system&left_color=black&right_color=green&left_text=Total%20Downloads)](https://pepy.tech/project/github-changelog-md)
 
 **Generate a Markdown changelog from a Github repository.**
 
 This project will generate a Markdown-formatted changelog from a Github
```

