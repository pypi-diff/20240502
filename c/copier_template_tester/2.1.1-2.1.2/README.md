# Comparing `tmp/copier_template_tester-2.1.1.tar.gz` & `tmp/copier_template_tester-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copier_template_tester-2.1.1.tar", max compression
+gzip compressed data, was "copier_template_tester-2.1.2.tar", max compression
```

## Comparing `copier_template_tester-2.1.1.tar` & `copier_template_tester-2.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-11-21 13:46:17.093159 copier_template_tester-2.1.1/LICENSE
--rw-r--r--   0        0        0     1876 2023-11-23 12:42:51.911075 copier_template_tester-2.1.1/copier_template_tester/__init__.py
--rw-r--r--   0        0        0      868 2023-10-14 16:44:48.551741 copier_template_tester-2.1.1/copier_template_tester/_config.py
--rw-r--r--   0        0        0      795 2023-11-23 12:38:51.636777 copier_template_tester-2.1.1/copier_template_tester/_pre_commit_support.py
--rw-r--r--   0        0        0     5800 2023-11-23 12:26:12.798275 copier_template_tester-2.1.1/copier_template_tester/_write_output.py
--rw-r--r--   0        0        0     2357 2023-11-23 12:40:06.923914 copier_template_tester-2.1.1/copier_template_tester/main.py
--rw-r--r--   0        0        0     3438 2023-11-23 12:42:56.676257 copier_template_tester-2.1.1/docs/README.md
--rw-r--r--   0        0        0     1529 2023-11-23 12:42:51.925985 copier_template_tester-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     4437 1970-01-01 00:00:00.000000 copier_template_tester-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-02 11:33:49.280964 copier_template_tester-2.1.2/LICENSE
+-rw-r--r--   0        0        0     1876 2024-05-02 12:47:32.534042 copier_template_tester-2.1.2/copier_template_tester/__init__.py
+-rw-r--r--   0        0        0      868 2023-10-14 16:44:48.551741 copier_template_tester-2.1.2/copier_template_tester/_config.py
+-rw-r--r--   0        0        0      795 2023-11-23 12:38:51.636777 copier_template_tester-2.1.2/copier_template_tester/_pre_commit_support.py
+-rw-r--r--   0        0        0     5810 2024-05-02 12:12:14.318929 copier_template_tester-2.1.2/copier_template_tester/_write_output.py
+-rw-r--r--   0        0        0     2357 2023-11-23 12:40:06.923914 copier_template_tester-2.1.2/copier_template_tester/main.py
+-rw-r--r--   0        0        0     3438 2024-05-02 12:47:37.317889 copier_template_tester-2.1.2/docs/README.md
+-rw-r--r--   0        0        0     1654 2024-05-02 12:47:32.548256 copier_template_tester-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4490 1970-01-01 00:00:00.000000 copier_template_tester-2.1.2/PKG-INFO
```

### Comparing `copier_template_tester-2.1.1/LICENSE` & `copier_template_tester-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `copier_template_tester-2.1.1/copier_template_tester/__init__.py` & `copier_template_tester-2.1.2/copier_template_tester/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from warnings import filterwarnings
 
 from beartype import BeartypeConf
 from beartype.claw import beartype_this_package
 from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
 from typing_extensions import Self
 
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 __pkg_name__ = 'copier_template_tester'
 
 
 class _RuntimeTypeCheckingModes(Enum):
     """Supported global runtime type checking modes."""
 
     ERROR = 'ERROR'
```

### Comparing `copier_template_tester-2.1.1/copier_template_tester/_config.py` & `copier_template_tester-2.1.2/copier_template_tester/_config.py`

 * *Files identical despite different names*

### Comparing `copier_template_tester-2.1.1/copier_template_tester/_pre_commit_support.py` & `copier_template_tester-2.1.2/copier_template_tester/_pre_commit_support.py`

 * *Files identical despite different names*

### Comparing `copier_template_tester-2.1.1/copier_template_tester/_write_output.py` & `copier_template_tester-2.1.2/copier_template_tester/_write_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import shutil
 from contextlib import contextmanager, suppress
 from functools import lru_cache
 from pathlib import Path
 
 import copier
-import yaml
+from copier.template import load_template_config
 from corallium.file_helpers import read_lines
 from corallium.log import get_logger
 from corallium.shell import capture_shell
 
 logger = get_logger()
 
 DEFAULT_TEMPLATE_FILE_NAME = 'copier.yaml'
@@ -36,15 +36,15 @@
     copier_path = base_dir / DEFAULT_TEMPLATE_FILE_NAME
     if not copier_path.is_file():
         copier_path = copier_path.with_suffix('.yml')
     if not copier_path.is_file():  # pragma: no cover
         msg = f"Can't find the copier template file. Expected: {copier_path} (or .yaml)"
         raise FileNotFoundError(msg)
 
-    return yaml.safe_load(copier_path.read_text())  # type: ignore[no-any-return]
+    return load_template_config(conf_path=copier_path)
 
 
 @lru_cache(maxsize=1)
 def _find_answers_file(*, src_path: Path, dst_path: Path) -> Path:
     """Locate the copier answers file based on the copier template."""
     copier_config = read_copier_template(src_path)
     answers_filename = copier_config.get('_answers_file') or DEFAULT_ANSWER_FILE_NAME
```

### Comparing `copier_template_tester-2.1.1/copier_template_tester/main.py` & `copier_template_tester-2.1.2/copier_template_tester/main.py`

 * *Files identical despite different names*

### Comparing `copier_template_tester-2.1.1/docs/README.md` & `copier_template_tester-2.1.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `copier_template_tester-2.1.1/pyproject.toml` & `copier_template_tester-2.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "2.1.1"
+version = "2.1.2"
 version_files = ["copier_template_tester/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
-  "Development Status :: 4 - Beta",
+  "Development Status :: 6 - Mature",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ] # https://pypi.org/classifiers/
 description = "Test copier templates"
 documentation = "https://copier-template-tester.kyleking.me"
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "copier_template_tester"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/copier-template-tester"
-version = "2.1.1"
+version = "2.1.2"
 
 [tool.poetry.dependencies]
 python = "^3.10.5"
-copier = ">=8.2.0"
-corallium = ">=0.3.3"
+copier = ">=9.2.0"
+corallium = ">=1.0.0"
 
 [tool.poetry.group.dev.dependencies]
-calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=2.0.1"}
+calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=2.1.0"}
 pytest-shell-utilities = ">=1.7.0"
 types-pyyaml = ">=6.0.12.9"
 types-setuptools = ">=67.6.0.8"
-virtualenv = "^20.24.6"
 
 [tool.poetry.scripts]
 ctt = "copier_template_tester.main:run_cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kyleking/copier-template-tester/issues"
 "Changelog" = "https://github.com/kyleking/copier-template-tester/blob/main/docs/docs/CHANGELOG.md"
 
 [tool.pyright]
 include = ["copier_template_tester"]
 pythonVersion = "3.10"
+
+[tool.tomlsort]
+all = true
+in_place = true
+sort_first = ["python"]
+trailing_comma_inline_array = true
```

### Comparing `copier_template_tester-2.1.1/PKG-INFO` & `copier_template_tester-2.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
-Name: copier-template-tester
-Version: 2.1.1
+Name: copier_template_tester
+Version: 2.1.2
 Summary: Test copier templates
 Home-page: https://github.com/kyleking/copier-template-tester
 License: MIT
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.10.5,<4.0.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: copier (>=8.2.0)
-Requires-Dist: corallium (>=0.3.3)
+Requires-Dist: copier (>=9.2.0)
+Requires-Dist: corallium (>=1.0.0)
 Project-URL: Bug Tracker, https://github.com/kyleking/copier-template-tester/issues
 Project-URL: Changelog, https://github.com/kyleking/copier-template-tester/blob/main/docs/docs/CHANGELOG.md
 Project-URL: Documentation, https://copier-template-tester.kyleking.me
 Project-URL: Repository, https://github.com/kyleking/copier-template-tester
 Description-Content-Type: text/markdown
 
 # copier-template-tester
```

