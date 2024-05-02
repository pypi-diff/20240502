# Comparing `tmp/github_org_manager-0.1.0.tar.gz` & `tmp/github_org_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_org_manager-0.1.0.tar", max compression
+gzip compressed data, was "github_org_manager-0.2.0.tar", max compression
```

## Comparing `github_org_manager-0.1.0.tar` & `github_org_manager-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11361 2024-04-30 09:20:34.470498 github_org_manager-0.1.0/LICENSE.txt
-drwxr-xr-x   0        0        0        0 2024-04-30 09:30:09.240427 github_org_manager-0.1.0/LICENSES/
--rw-r--r--   0        0        0    11361 2024-04-30 09:30:23.380425 github_org_manager-0.1.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    17023 2024-04-30 09:30:08.660427 github_org_manager-0.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0        0        0     7048 2024-04-30 09:30:09.240427 github_org_manager-0.1.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0     1078 2024-04-30 09:30:08.850427 github_org_manager-0.1.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     3073 2024-04-30 09:34:20.850393 github_org_manager-0.1.0/README.md
--rw-r--r--   0        0        0      597 2024-04-30 09:24:33.520468 github_org_manager-0.1.0/gh_org_mgr/__init__.py
--rw-r--r--   0        0        0     4021 2024-04-30 09:24:33.530468 github_org_manager-0.1.0/gh_org_mgr/_config.py
--rw-r--r--   0        0        0      794 2024-04-30 09:24:33.530468 github_org_manager-0.1.0/gh_org_mgr/_gh_api.py
--rw-r--r--   0        0        0    17581 2024-04-30 09:24:33.530468 github_org_manager-0.1.0/gh_org_mgr/_gh_org.py
--rw-r--r--   0        0        0     2121 2024-04-30 09:24:33.520468 github_org_manager-0.1.0/gh_org_mgr/manage.py
--rw-r--r--   0        0        0      911 2024-04-30 09:24:33.520468 github_org_manager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3665 1970-01-01 00:00:00.000000 github_org_manager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11361 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSE.txt
+drwxr-xr-x   0        0        0        0 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSES/
+-rw-r--r--   0        0        0    11361 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    17023 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0     7048 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1078 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     3645 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/README.md
+-rw-r--r--   0        0        0      597 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/gh_org_mgr/__init__.py
+-rw-r--r--   0        0        0     4022 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/gh_org_mgr/_config.py
+-rw-r--r--   0        0        0      794 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/gh_org_mgr/_gh_api.py
+-rw-r--r--   0        0        0    17581 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/gh_org_mgr/_gh_org.py
+-rw-r--r--   0        0        0     2121 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/gh_org_mgr/manage.py
+-rw-r--r--   0        0        0      923 2024-05-02 07:51:24.145122 github_org_manager-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 github_org_manager-0.2.0/PKG-INFO
```

### Comparing `github_org_manager-0.1.0/LICENSE.txt` & `github_org_manager-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.1.0/LICENSES/Apache-2.0.txt` & `github_org_manager-0.2.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.1.0/LICENSES/CC-BY-4.0.txt` & `github_org_manager-0.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.1.0/LICENSES/CC0-1.0.txt` & `github_org_manager-0.2.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.1.0/LICENSES/MIT.txt` & `github_org_manager-0.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.1.0/README.md` & `github_org_manager-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,34 @@
+Metadata-Version: 2.1
+Name: github-org-manager
+Version: 0.2.0
+Summary: Manage a GitHub Organization, its teams, repository permissions, and more
+Author: Max Mehl
+Author-email: max.mehl@deutschebahn.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pygithub (>=2.3.0,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Description-Content-Type: text/markdown
+
 <!--
 SPDX-FileCopyrightText: 2024 DB Systel GmbH
 
 SPDX-License-Identifier: Apache-2.0
 -->
 
 # GitHub Organization Manager
 
+[![Test suites](https://github.com/OpenRailAssociation/github-org-manager/actions/workflows/test.yaml/badge.svg)](https://github.com/OpenRailAssociation/github-org-manager/actions/workflows/test.yaml)
 [![REUSE status](https://api.reuse.software/badge/github.com/OpenRailAssociation/github-org-manager)](https://api.reuse.software/info/github.com/OpenRailAssociation/github-org-manager)
+[![The latest version of GitHub Org Manager can be found on PyPI.](https://img.shields.io/pypi/v/github-org-manager.svg)](https://pypi.org/project/github-org-manager/)
+[![Information on what versions of Python GitHub Org Manager supports can be found on PyPI.](https://img.shields.io/pypi/pyversions/github-org-manager.svg)](https://pypi.org/project/github-org-manager/)
 
 A lightweight tool that helps with managing a GitHub organization, its members, teams, repository permissions and more.
 
 The basic principle: all settings reside in YAML configuration files which will be made effective during a run of this tool.
 
 ## Features
 
@@ -56,7 +74,8 @@
 ## License
 
 The content of this repository is licensed under the [Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0).
 
 There may be components under different, but compatible licenses or from different copyright holders. The project is REUSE compliant which makes these portions transparent. You will find all used licenses in the [LICENSES](./LICENSES/) directory.
 
 The project is has been started by the [OpenRail Association](https://openrailassociation.org). You are welcome to [contribute](./CONTRIBUTING.md)!
+
```

### Comparing `github_org_manager-0.1.0/gh_org_mgr/__init__.py` & `github_org_manager-0.2.0/gh_org_mgr/__init__.py`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.1.0/gh_org_mgr/_config.py` & `github_org_manager-0.2.0/gh_org_mgr/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 matching_files[0],
             )
 
     if not matching_files:
         logging.error(
             "No configuration file found for '%s' in '%s'. The program might not work as expected!",
             pattern,
-            directory
+            directory,
         )
 
     return matching_files
 
 
 def _read_config_file(file: str) -> dict:
     """Return dict of a YAML file"""
```

### Comparing `github_org_manager-0.1.0/gh_org_mgr/_gh_api.py` & `github_org_manager-0.2.0/gh_org_mgr/_gh_api.py`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.1.0/gh_org_mgr/_gh_org.py` & `github_org_manager-0.2.0/gh_org_mgr/_gh_org.py`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.1.0/gh_org_mgr/manage.py` & `github_org_manager-0.2.0/gh_org_mgr/manage.py`

 * *Files identical despite different names*

### Comparing `github_org_manager-0.1.0/pyproject.toml` & `github_org_manager-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 # SPDX-FileCopyrightText: 2024 DB Systel GmbH
 #
 # SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "github-org-manager"
-version = "0.1.0"
+version = "0.2.0"
 description = "Manage a GitHub Organization, its teams, repository permissions, and more"
 authors = ["Max Mehl <max.mehl@deutschebahn.com>"]
 readme = "README.md"
 packages = [{include = "gh_org_mgr"}]
 
 [tool.poetry.scripts]
 gh-org-mgr = 'gh_org_mgr.manage:main'
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pygithub = "^2.3.0"
 pyyaml = "^6.0.1"
-tqdm = "^4.66.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 isort = "^5.13.2"
 mypy = "^1.9.0"
 pylint = "^3.1.0"
 types-pyyaml = "^6.0.12.20240311"
-types-tqdm = "^4.66.0.20240106"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 # FORMATTING settings
@@ -38,7 +36,11 @@
 
 [tool.black]
 line-length = 100
 
 # MYPY settings
 [tool.mypy]
 files = ["gh_org_mgr/*.py"]
+
+# Pylint
+[tool.pylint.'MESSAGES CONTROL']
+disable = "fixme"
```

### Comparing `github_org_manager-0.1.0/PKG-INFO` & `github_org_manager-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,19 @@
-Metadata-Version: 2.1
-Name: github-org-manager
-Version: 0.1.0
-Summary: Manage a GitHub Organization, its teams, repository permissions, and more
-Author: Max Mehl
-Author-email: max.mehl@deutschebahn.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pygithub (>=2.3.0,<3.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: tqdm (>=4.66.2,<5.0.0)
-Description-Content-Type: text/markdown
-
 <!--
 SPDX-FileCopyrightText: 2024 DB Systel GmbH
 
 SPDX-License-Identifier: Apache-2.0
 -->
 
 # GitHub Organization Manager
 
+[![Test suites](https://github.com/OpenRailAssociation/github-org-manager/actions/workflows/test.yaml/badge.svg)](https://github.com/OpenRailAssociation/github-org-manager/actions/workflows/test.yaml)
 [![REUSE status](https://api.reuse.software/badge/github.com/OpenRailAssociation/github-org-manager)](https://api.reuse.software/info/github.com/OpenRailAssociation/github-org-manager)
+[![The latest version of GitHub Org Manager can be found on PyPI.](https://img.shields.io/pypi/v/github-org-manager.svg)](https://pypi.org/project/github-org-manager/)
+[![Information on what versions of Python GitHub Org Manager supports can be found on PyPI.](https://img.shields.io/pypi/pyversions/github-org-manager.svg)](https://pypi.org/project/github-org-manager/)
 
 A lightweight tool that helps with managing a GitHub organization, its members, teams, repository permissions and more.
 
 The basic principle: all settings reside in YAML configuration files which will be made effective during a run of this tool.
 
 ## Features
 
@@ -72,8 +59,7 @@
 ## License
 
 The content of this repository is licensed under the [Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0).
 
 There may be components under different, but compatible licenses or from different copyright holders. The project is REUSE compliant which makes these portions transparent. You will find all used licenses in the [LICENSES](./LICENSES/) directory.
 
 The project is has been started by the [OpenRail Association](https://openrailassociation.org). You are welcome to [contribute](./CONTRIBUTING.md)!
-
```

