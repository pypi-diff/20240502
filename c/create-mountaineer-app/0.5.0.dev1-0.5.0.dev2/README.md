# Comparing `tmp/create_mountaineer_app-0.5.0.dev1.tar.gz` & `tmp/create_mountaineer_app-0.5.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_mountaineer_app-0.5.0.dev1.tar", max compression
+gzip compressed data, was "create_mountaineer_app-0.5.0.dev2.tar", max compression
```

## Comparing `create_mountaineer_app-0.5.0.dev1.tar` & `create_mountaineer_app-0.5.0.dev2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1593 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/README.md
--rw-r--r--   0        0        0        1 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/__tests__/__init__.py
--rw-r--r--   0        0        0     1055 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/__tests__/common.py
--rw-r--r--   0        0        0     7904 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/__tests__/test_builder.py
--rw-r--r--   0        0        0      292 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/__tests__/test_cli.py
--rw-r--r--   0        0        0      816 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/__tests__/test_generation.py
--rw-r--r--   0        0        0     4277 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/builder.py
--rw-r--r--   0        0        0     4656 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/cli.py
--rw-r--r--   0        0        0        0 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/environments/__init__.py
--rw-r--r--   0        0        0     1383 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/environments/base.py
--rw-r--r--   0        0        0     4591 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/environments/poetry.py
--rw-r--r--   0        0        0     1832 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/environments/venv.py
--rw-r--r--   0        0        0     1336 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/external.py
--rw-r--r--   0        0        0     1925 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/generation.py
--rw-r--r--   0        0        0      327 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/io.py
--rw-r--r--   0        0        0       30 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/.zed/settings.json
--rw-r--r--   0        0        0      212 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/__init__.py
--rw-r--r--   0        0        0      246 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/editor_configs/vim/.vimrc
--rw-r--r--   0        0        0      162 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
--rw-r--r--   0        0        0      109 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
--rw-r--r--   0        0        0      170 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/.env
--rw-r--r--   0        0        0     3383 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/.gitignore
--rw-r--r--   0        0        0      645 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/README.md
--rw-r--r--   0        0        0       17 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/__init__.py
--rw-r--r--   0        0        0      767 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/app.py
--rw-r--r--   0        0        0      947 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/cli.py
--rw-r--r--   0        0        0      282 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/config.py
--rw-r--r--   0        0        0      227 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
--rw-r--r--   0        0        0     1702 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
--rw-r--r--   0        0        0     1124 2024-05-01 23:34:02.600146 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
--rw-r--r--   0        0        0       84 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/main.py
--rw-r--r--   0        0        0      157 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
--rw-r--r--   0        0        0      208 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/models/detail.py
--rw-r--r--   0        0        0        0 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
--rw-r--r--   0        0        0     1219 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
--rw-r--r--   0        0        0      995 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
--rw-r--r--   0        0        0       95 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
--rw-r--r--   0        0        0      524 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/views/package.json
--rw-r--r--   0        0        0      117 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
--rw-r--r--   0        0        0      195 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
--rw-r--r--   0        0        0      332 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/docker-compose.yml
--rw-r--r--   0        0        0     1493 2024-05-01 23:34:02.604147 create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/pyproject.toml
--rw-r--r--   0        0        0     1219 2024-05-01 23:34:14.172342 create_mountaineer_app-0.5.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 create_mountaineer_app-0.5.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1593 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/README.md
+-rw-r--r--   0        0        0        1 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/__tests__/__init__.py
+-rw-r--r--   0        0        0     1055 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/__tests__/common.py
+-rw-r--r--   0        0        0     8021 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/__tests__/test_builder.py
+-rw-r--r--   0        0        0      292 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/__tests__/test_cli.py
+-rw-r--r--   0        0        0      816 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/__tests__/test_generation.py
+-rw-r--r--   0        0        0     4277 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/builder.py
+-rw-r--r--   0        0        0     4656 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/cli.py
+-rw-r--r--   0        0        0        0 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/environments/__init__.py
+-rw-r--r--   0        0        0     1383 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/environments/base.py
+-rw-r--r--   0        0        0     4591 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/environments/poetry.py
+-rw-r--r--   0        0        0     1832 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/environments/venv.py
+-rw-r--r--   0        0        0     1336 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/external.py
+-rw-r--r--   0        0        0     1919 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/generation.py
+-rw-r--r--   0        0        0      327 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/io.py
+-rw-r--r--   0        0        0       30 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/.zed/settings.json
+-rw-r--r--   0        0        0      212 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/editor_configs/vim/.vimrc
+-rw-r--r--   0        0        0      162 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
+-rw-r--r--   0        0        0      109 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
+-rw-r--r--   0        0        0      170 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/.env
+-rw-r--r--   0        0        0     3383 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/.gitignore
+-rw-r--r--   0        0        0      645 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/README.md
+-rw-r--r--   0        0        0       17 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/__init__.py
+-rw-r--r--   0        0        0      767 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/app.py
+-rw-r--r--   0        0        0      947 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/cli.py
+-rw-r--r--   0        0        0      282 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/config.py
+-rw-r--r--   0        0        0      227 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
+-rw-r--r--   0        0        0     1702 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
+-rw-r--r--   0        0        0     1124 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
+-rw-r--r--   0        0        0       84 2024-05-02 18:07:43.552228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/main.py
+-rw-r--r--   0        0        0      157 2024-05-02 18:07:43.556228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-02 18:07:43.556228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/models/detail.py
+-rw-r--r--   0        0        0        0 2024-05-02 18:07:43.556228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
+-rw-r--r--   0        0        0     1219 2024-05-02 18:07:43.556228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
+-rw-r--r--   0        0        0      995 2024-05-02 18:07:43.556228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
+-rw-r--r--   0        0        0       95 2024-05-02 18:07:43.556228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
+-rw-r--r--   0        0        0      524 2024-05-02 18:07:43.556228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/views/package.json
+-rw-r--r--   0        0        0      117 2024-05-02 18:07:43.556228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
+-rw-r--r--   0        0        0      195 2024-05-02 18:07:43.556228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
+-rw-r--r--   0        0        0      332 2024-05-02 18:07:43.556228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/docker-compose.yml
+-rw-r--r--   0        0        0     1493 2024-05-02 18:07:43.556228 create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/pyproject.toml
+-rw-r--r--   0        0        0     1323 2024-05-02 18:07:54.644396 create_mountaineer_app-0.5.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 create_mountaineer_app-0.5.0.dev2/PKG-INFO
```

### Comparing `create_mountaineer_app-0.5.0.dev1/README.md` & `create_mountaineer_app-0.5.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/__tests__/common.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/__tests__/common.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/__tests__/test_builder.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/__tests__/test_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import subprocess
+import sys
 from itertools import product
 from os import environ
 from pathlib import Path
 from time import sleep
 from uuid import uuid4
 
 import pytest
-import tomllib
 from click import secho
 from packaging.requirements import Requirement
 from packaging.version import Version
 from requests import get
 
+if sys.version_info >= (3, 11):
+    from tomllib import loads as toml_loads
+else:
+    from toml import loads as toml_loads
+
 from create_mountaineer_app.__tests__.common import wait_for_database_to_be_ready
 from create_mountaineer_app.builder import (
     build_project,
     environment_from_metadata,
     should_copy_path,
 )
 from create_mountaineer_app.generation import EditorType, ProjectMetadata
@@ -223,15 +228,15 @@
         # the mountaineer_dev_path
         mountaineer_min_version="0.2.5",
         mountaineer_dev_path=None,
     )
     build_project(metadata, install_deps=False)
 
     pyproject_contents = (tmp_path / "pyproject.toml").read_text()
-    package_requirements = tomllib.loads(pyproject_contents)
+    package_requirements = toml_loads(pyproject_contents)
 
     if use_poetry:
         # Parse the poetry convention into the PEP 508 specifier format
         raw_version = package_requirements["tool"]["poetry"]["dependencies"][
             "mountaineer"
         ]
         assert raw_version == "^0.2.5"
```

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/__tests__/test_generation.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/__tests__/test_generation.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/builder.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/builder.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/cli.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/cli.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/environments/base.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/environments/base.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/environments/poetry.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/environments/venv.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/environments/venv.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/external.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/external.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/generation.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from enum import StrEnum
+from enum import Enum
 from pathlib import Path
 
 from jinja2 import Template
 from pydantic import BaseModel
 
 
-class EditorType(StrEnum):
+class EditorType(Enum):
     VSCODE = "vscode"
     VIM = "vim"
     ZED = "zed"
 
 
 class ProjectMetadata(BaseModel):
     project_name: str
```

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/.gitignore` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/README.md` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/app.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/app.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/cli.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/cli.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/controllers/home.py` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/controllers/home.py`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/[project_name]/views/package.json` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/[project_name]/views/package.json`

 * *Files identical despite different names*

### Comparing `create_mountaineer_app-0.5.0.dev1/create_mountaineer_app/templates/project/pyproject.toml` & `create_mountaineer_app-0.5.0.dev2/create_mountaineer_app/templates/project/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 name = "{{project_name}}"
 version = "0.1.0"
 description = ""
 authors = ["{{author_name}} <{{author_email}}>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 
 {% if mountaineer_dev_path %}
 mountaineer = { path = "{{mountaineer_dev_path}}", develop = true }
 {% else %}
 mountaineer = "^{{ mountaineer_min_version }}"
 {% endif %}
```

### Comparing `create_mountaineer_app-0.5.0.dev1/pyproject.toml` & `create_mountaineer_app-0.5.0.dev2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "create-mountaineer-app"
-version = "0.5.0.dev1"
+version = "0.5.0.dev2"
 description = ""
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 questionary = "^2.0.1"
 click = "^8.1.7"
 jinja2 = "^3.1.3"
 pydantic = "^2.6.1"
 
 [tool.poetry.scripts]
 create-mountaineer-app = 'create_mountaineer_app.cli:main'
@@ -22,14 +22,16 @@
 requests = "^2.31.0"
 types-requests = "^2.31.0.20240125"
 pytest-asyncio = "^0.23.4"
 pytest-xdist = "^3.5.0"
 psycopg2 = "^2.9.9"
 types-psycopg2 = "^2.9.21.20240218"
 pyright = "^1.1.352"
+toml = { version = "^0.10.2", python = "<3.11" }
+types-toml = { version = "^0.10.8", python = "<3.11" }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 exclude = ".*/templates/.*"
```

### Comparing `create_mountaineer_app-0.5.0.dev1/PKG-INFO` & `create_mountaineer_app-0.5.0.dev2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: create-mountaineer-app
-Version: 0.5.0.dev1
+Version: 0.5.0.dev2
 Summary: 
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
```

